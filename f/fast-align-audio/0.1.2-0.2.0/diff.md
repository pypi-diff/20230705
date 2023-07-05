# Comparing `tmp/fast_align_audio-0.1.2-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/fast_align_audio-0.2.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10739 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    11776 b- defN 23-Jul-04 08:43 _fast_align_audio.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       68 b- defN 23-Jul-04 08:37 fast_align_audio/__init__.py
--rw-rw-rw-  2.0 fat      618 b- defN 23-Jul-04 08:37 fast_align_audio/_alignment_cffi.py
--rw-rw-rw-  2.0 fat     3379 b- defN 23-Jul-04 08:37 fast_align_audio/alignment.py
--rw-rw-rw-  2.0 fat      761 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2510 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      792 b- defN 23-Jul-04 08:43 fast_align_audio-0.1.2.dist-info/RECORD
-9 files, 20046 bytes uncompressed, 9355 bytes compressed:  53.3%
+Zip file size: 12269 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    12288 b- defN 23-Jul-05 12:33 _fast_align_audio.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      113 b- defN 23-Jul-05 12:28 fast_align_audio/__init__.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-Jul-05 12:28 fast_align_audio/_alignment_cffi.py
+-rw-rw-rw-  2.0 fat     7372 b- defN 23-Jul-05 12:28 fast_align_audio/alignment.py
+-rw-rw-rw-  2.0 fat      761 b- defN 23-Jul-05 12:33 fast_align_audio-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3634 b- defN 23-Jul-05 12:33 fast_align_audio-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-05 12:33 fast_align_audio-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-05 12:33 fast_align_audio-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      793 b- defN 23-Jul-05 12:33 fast_align_audio-0.2.0.dist-info/RECORD
+9 files, 25840 bytes uncompressed, 10885 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fast_align_audio/_alignment_cffi.py
 Comment: 
 
 Filename: fast_align_audio/alignment.py
 Comment: 
 
-Filename: fast_align_audio-0.1.2.dist-info/LICENSE
+Filename: fast_align_audio-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: fast_align_audio-0.1.2.dist-info/METADATA
+Filename: fast_align_audio-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: fast_align_audio-0.1.2.dist-info/WHEEL
+Filename: fast_align_audio-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: fast_align_audio-0.1.2.dist-info/top_level.txt
+Filename: fast_align_audio-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fast_align_audio-0.1.2.dist-info/RECORD
+Filename: fast_align_audio-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fast_align_audio/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .alignment import best_offset, align
+from .alignment import find_best_alignment_offset, align_delayed_signal_with_reference
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
```

## fast_align_audio/_alignment_cffi.py

```diff
@@ -1,14 +1,20 @@
 import os
 from cffi import FFI
 
 
 ffibuilder = FFI()
+ffibuilder.cdef("""
+    typedef struct {
+        ssize_t min_idx;
+        float min_val;
+    } MinResult;
+""")
 ffibuilder.cdef(
-    "ssize_t fast_find_alignment(size_t, float *, size_t, float *, size_t, size_t);"
+    "MinResult fast_find_alignment(size_t, float *, size_t, float *, size_t, size_t);"
 )
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 c_file_path = os.path.join(script_dir, "_faa.c")
 
 with open(c_file_path, "r") as file:
     c_code = file.read()
```

## fast_align_audio/alignment.py

```diff
@@ -1,95 +1,173 @@
+from typing import Optional, Tuple
+
 import numpy as np
 import _fast_align_audio
+from numpy.typing import NDArray
+
 
+def fast_autocorr(original, delayed, t=1):
+    """Only every 4th sample is considered in order to improve execution time"""
+    if t == 0:
+        return np.corrcoef([original[::4], delayed[::4]])[1, 0]
+    elif t < 0:
+        return np.corrcoef([original[-t::4], delayed[:t:4]])[1, 0]
+    else:
+        return np.corrcoef([original[:-t:4], delayed[t::4]])[1, 0]
 
-def best_offset(a, b, max_offset, max_lookahead=None):
+
+def find_best_alignment_offset_with_corr_coef(
+    reference_signal: NDArray[np.float32],
+    delayed_signal: NDArray[np.float32],
+    min_offset_samples: int,
+    max_offset_samples: int,
+    lookahead_samples: Optional[int] = None,
+    consider_both_polarities: bool = True,
+):
     """
-    Find best offset of `a` w.r.t. `b`.
+    Returns the estimated delay (in samples) between the original and delayed signal,
+    calculated using correlation coefficients. The delay is optimized to maximize the
+    correlation between the signals.
 
-    Best = smallest mean squared error (mse).
+    Args:
+        reference_signal (NDArray[np.float32]): The original signal array.
+        delayed_signal (NDArray[np.float32]): The delayed signal array.
+        min_offset_samples (int): The minimum delay offset to consider, in samples.
+                                  Can be negative.
+        max_offset_samples (int): The maximum delay offset to consider, in samples.
+        lookahead_samples (Optional[int]): The number of samples to look at
+                                           while estimating the delay. If None, the
+                                           whole delayed signal is considered.
+        consider_both_polarities (bool): If True, the function will consider both positive
+                                         and negative correlations, which corresponds to
+                                         the same or opposite polarities in signals,
+                                         respectively. Defaults to True.
 
-    If the returned offset is positive, it means the smallest mse is:
+    Returns:
+        tuple: Estimated delay (int) and correlation coefficient (float).
+    """
+    if lookahead_samples is not None and len(reference_signal) > lookahead_samples:
+        middle_of_signal_index = int(np.floor(len(reference_signal) / 2))
+        original_signal_slice = reference_signal[
+            middle_of_signal_index : middle_of_signal_index + lookahead_samples
+        ]
+        delayed_signal_slice = delayed_signal[
+            middle_of_signal_index : middle_of_signal_index + lookahead_samples
+        ]
+    else:
+        original_signal_slice = reference_signal
+        delayed_signal_slice = delayed_signal
 
-        ((a[n:...] - b[:...])**2).mean()
+    coefs = []
+    for lag in range(min_offset_samples, max_offset_samples):
+        correlation_coef = fast_autocorr(
+            original_signal_slice, delayed_signal_slice, t=lag
+        )
+        coefs.append(correlation_coef)
+
+    if consider_both_polarities:
+        # In this mode we aim to find the correlation coefficient of highest magnitude.
+        # We do this to consider the possibility that the delayed signal has opposite
+        # polarity compared to the original signal, in which case the correlation
+        # coefficient would be negative.
+        most_extreme_coef_index = int(np.argmax(np.abs(coefs)))
+    else:
+        most_extreme_coef_index = int(np.argmax(coefs))
+    most_extreme_coef = coefs[most_extreme_coef_index]
+    offset = most_extreme_coef_index + min_offset_samples
+    return offset, most_extreme_coef
 
-    If the returned is negative, it means the smallest mse is:
 
-        ((a[:...] - b[n:...])**2).mean()
+def find_best_alignment_offset(
+    reference_signal: NDArray[np.float32],
+    delayed_signal: NDArray[np.float32],
+    max_offset_samples: int,
+    lookahead_samples: Optional[int] = None,
+    method: str = "mse",
+    consider_both_polarities: bool = False,
+) -> Tuple[int, float]:
+    """
+    Find best offset of `delayed_audio` w.r.t. `reference_audio`.
 
-    (Here, `...` means that you have to account for different array lengths for
-    this computation to actually work.)
+    Best = smallest mean squared error (mse).
 
     Args:
-        a, b (float32 C-contiguous NumPy arrays):
+        reference_audio, delayed_audio (float32 C-contiguous NumPy arrays):
             The arrays to compare
-        max_offset (int > 0):
+        max_offset_samples (int > 0):
             Maximum expected offset. It will not find any larger offsets.
-        max_lookahead (int > 0, optional):
+        lookahead_samples (int > 0, optional):
             Maximum number of array elements to use for each mse computation.
             If `None` (the default), there is no maximum.
+        method: "mse" (fast) or "corr" (slow)
+        consider_both_polarities: If set to true, also consider the possibility that the
+            delayed signal could possibly have opposite polarity compared to the
+            reference_signal. This doubles the execution time when method=="mse".
+
+    Return offset and metric (mse or corr coef)
     """
-    assert {a.dtype, b.dtype} == {np.dtype("float32")}, "Arrays must be float32"
-    assert (
-        a.flags["C_CONTIGUOUS"] and b.flags["C_CONTIGUOUS"]
-    ), "Arrays must be C-contiguous"
-    if max_lookahead is None:
-        max_lookahead = max(len(a), len(b))
-    return _fast_align_audio.lib.fast_find_alignment(
-        len(a),
-        _fast_align_audio.ffi.cast("float *", a.ctypes.data),
-        len(b),
-        _fast_align_audio.ffi.cast("float *", b.ctypes.data),
-        max_offset,
-        max_lookahead,
-    )
+    assert {reference_signal.dtype, delayed_signal.dtype} == {
+        np.dtype("float32")
+    }, "Arrays must be float32"
+    assert reference_signal.ndim == 1
+    assert delayed_signal.ndim == 1
+
+    if method == "mse":
+        assert (
+            reference_signal.flags["C_CONTIGUOUS"]
+            and delayed_signal.flags["C_CONTIGUOUS"]
+        ), "Arrays must be C-contiguous"
+        if lookahead_samples is None:
+            lookahead_samples = max(len(reference_signal), len(delayed_signal))
+
+        result = _fast_align_audio.lib.fast_find_alignment(
+            len(delayed_signal),
+            _fast_align_audio.ffi.cast("float *", delayed_signal.ctypes.data),
+            len(reference_signal),
+            _fast_align_audio.ffi.cast("float *", reference_signal.ctypes.data),
+            max_offset_samples,
+            lookahead_samples,
+        )
+        if consider_both_polarities:
+            inverse_polarity_result = _fast_align_audio.lib.fast_find_alignment(
+                len(delayed_signal),
+                _fast_align_audio.ffi.cast("float *", (-delayed_signal).ctypes.data),
+                len(reference_signal),
+                _fast_align_audio.ffi.cast("float *", reference_signal.ctypes.data),
+                max_offset_samples,
+                lookahead_samples,
+            )
+            if inverse_polarity_result.min_val < result.min_val:
+                return inverse_polarity_result.min_idx, inverse_polarity_result.min_val
+        return result.min_idx, result.min_val
+    elif method == "corr":
+        return find_best_alignment_offset_with_corr_coef(
+            reference_signal=reference_signal,
+            delayed_signal=delayed_signal,
+            min_offset_samples=-max_offset_samples,
+            max_offset_samples=max_offset_samples,
+            consider_both_polarities=consider_both_polarities,
+        )
+    else:
+        raise ValueError("Unknown method")
 
 
-def align(a, b, max_offset, max_lookahead=None, *, align_mode, fix_length=None):
+def align_delayed_signal_with_reference(
+    reference_signal: NDArray[np.float32],
+    delayed_signal: NDArray[np.float32],
+    offset: int,
+):
     """
-    Align `a` and `b`. See the documentation of `best_offset` for most of the args.
+    Align delayed_signal with the reference signal, given the offset.
+    The start or end is filled with `offset` amount of zeros.
 
-    Args:
-        align_mode (Either `"crop"` or `"pad"`): How to align `a` and `b`.
-            If `crop`, `best_offset` number of elements are removed from the
-            front of the "too-long" array. If `pad`, `best_offset` number of
-            elements are padding to the front of the "too-short" array.
-        fix_length (Either `"shortest"`, `"longest"` or `None`): How to fix the
-            lengths of `a` and `b` after alignment. If `shortest`, the longer
-            array is cropped (at the end/right) to the length of the shorter one.
-            If `longest`, the shorter array is padded (to the end/right) to the
-            length of the longest one.  If `None`, lengths are not changed.
-    """
-    offset = best_offset(a, b, max_offset, max_lookahead)
-    if offset > 0:
-        # mse(a[offset:], b) = min
-        a, b = _align(a, b, offset, align_mode)
-    else:
-        # mse(a, b[offset:]) = min
-        b, a = _align(b, a, -offset, align_mode)
-    a, b = _fix(a, b, fix_length)
-    return a, b
-
-
-def _align(x, y, offset, align_mode):
-    if align_mode == "crop":
-        x = x[offset:]
-    elif align_mode == "pad":
-        y = np.pad(y, (offset, 0))
-    return x, y
-
-
-def _fix(x, y, fix_mode):
-    if fix_mode is None:
-        return x, y
-    elif fix_mode == "shortest":
-        min_len = min(len(x), len(y))
-        x = x[:min_len]
-        y = y[:min_len]
-        return x, y
-    elif fix_mode == "longest":
-        max_len = max(len(x), len(y))
-        x = np.pad(x, (0, max_len - len(x)))
-        y = np.pad(y, (0, max_len - len(y)))
-        return x, y
+    This function assumes that reference_signal and delayed_signal have the same length.
+
+    The returned array has the same length as the reference signal.
+    """
+    placeholder = np.zeros_like(reference_signal)
+    if offset < 0:
+        offset = -offset
+        placeholder[offset:] = delayed_signal[0:-offset]
     else:
-        raise ValueError(f"fix_length={fix_mode!r} not understood")
+        placeholder[0:-offset] = delayed_signal[offset:]
+    return placeholder
```

## Comparing `fast_align_audio-0.1.2.dist-info/LICENSE` & `fast_align_audio-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fast_align_audio-0.1.2.dist-info/RECORD` & `fast_align_audio-0.2.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-_fast_align_audio.pypy39-pp73-win_amd64.pyd,sha256=FCSsC3LyqwKqv1KO5pl81XH90k-2Pn5zH3HREbGg9a4,11776
-fast_align_audio/__init__.py,sha256=PdczRZiBp0xDiiXqLH6H3zMlXp-0MEsxrYp0ZXS4CUY,68
-fast_align_audio/_alignment_cffi.py,sha256=wxkZEshCgPjq3R1nHAGlCgkAFzHzFcCSTilAfoUrY5I,618
-fast_align_audio/alignment.py,sha256=BnNKk7MBPE0uFu76vJGL47OwytiYhzVYokKr29qlMXM,3379
-fast_align_audio-0.1.2.dist-info/LICENSE,sha256=tPBrKL5kSF5qsi2Sigy2FBz6E5Vj72tIAOUV63e8d5w,761
-fast_align_audio-0.1.2.dist-info/METADATA,sha256=3X5LCkU9LJxS6w4EwE46dkJgXH0roDYgpwDCbcQbS1s,2510
-fast_align_audio-0.1.2.dist-info/WHEEL,sha256=QQY0XPJVcbNrDwRnZBTwtxGbMWJnHaWRpMJLfPEPCFM,107
-fast_align_audio-0.1.2.dist-info/top_level.txt,sha256=Ll1Ggww3-RoLC_LESKBjfjTd1cbVlwQEjljxtvCzz7w,35
-fast_align_audio-0.1.2.dist-info/RECORD,,
+_fast_align_audio.pypy39-pp73-win_amd64.pyd,sha256=6bSndClgjpu4koNGiNKDujxanMvWlvDoMUO1LkbfNDA,12288
+fast_align_audio/__init__.py,sha256=N8Z2AG94KAJ_2C6kamLjTMjK2e3aQsep3twzQdl_Wlo,113
+fast_align_audio/_alignment_cffi.py,sha256=gWQ6RX_Sm4XuIGDA9gnh3x5AYD_B9wI9wMVeEUDEN0k,737
+fast_align_audio/alignment.py,sha256=sXbDwVitZi9WOTQygi6PmUyvNMh4HSKzjbOl48Rzwek,7372
+fast_align_audio-0.2.0.dist-info/LICENSE,sha256=tPBrKL5kSF5qsi2Sigy2FBz6E5Vj72tIAOUV63e8d5w,761
+fast_align_audio-0.2.0.dist-info/METADATA,sha256=RkEk0dUFw1G_ZVEd5XJZij05QRjQFlM9CQ8MIG_UplI,3634
+fast_align_audio-0.2.0.dist-info/WHEEL,sha256=QQY0XPJVcbNrDwRnZBTwtxGbMWJnHaWRpMJLfPEPCFM,107
+fast_align_audio-0.2.0.dist-info/top_level.txt,sha256=Ll1Ggww3-RoLC_LESKBjfjTd1cbVlwQEjljxtvCzz7w,35
+fast_align_audio-0.2.0.dist-info/RECORD,,
```

