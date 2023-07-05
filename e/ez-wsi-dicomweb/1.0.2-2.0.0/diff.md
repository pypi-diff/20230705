# Comparing `tmp/ez_wsi_dicomweb-1.0.2.tar.gz` & `tmp/ez_wsi_dicomweb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_wsi_dicomweb-1.0.2.tar", last modified: Fri Jun 30 04:54:43 2023, max compression
+gzip compressed data, was "ez_wsi_dicomweb-2.0.0.tar", last modified: Wed Jul  5 21:05:15 2023, max compression
```

## Comparing `ez_wsi_dicomweb-1.0.2.tar` & `ez_wsi_dicomweb-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-x---   0 armant   (1130519) primarygroup (89939)        0 2023-06-30 04:54:43.890592 ez_wsi_dicomweb-1.0.2/
--rw-r-----   0 armant   (1130519) primarygroup (89939)    11358 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/LICENSE
--rw-r-----   0 armant   (1130519) primarygroup (89939)      334 2023-06-30 04:54:43.890592 ez_wsi_dicomweb-1.0.2/PKG-INFO
--rw-r-----   0 armant   (1130519) primarygroup (89939)     3135 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/README.md
-drwxr-x---   0 armant   (1130519) primarygroup (89939)        0 2023-06-30 04:54:43.886592 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/
--rw-r-----   0 armant   (1130519) primarygroup (89939)        0 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/__init__.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     2440 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/abstract_slide_frame_cache.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1959 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_frame_decoder.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     2565 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_frame_decoder_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    31620 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_slide.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    46763 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_slide_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     3295 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_store.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1563 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_store_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     2475 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_test_utils.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    11455 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_web_interface.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    13493 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_web_interface_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1893 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/ez_wsi_errors.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1157 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/ez_wsi_errors_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     8126 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/magnification.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     8326 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/magnification_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     8084 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/patch_generator.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     9674 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/patch_generator_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     6671 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     2060 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing_converter.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1738 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing_converter_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    16095 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing_test.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    18293 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/slide_level_map.py
--rw-r-----   0 armant   (1130519) primarygroup (89939)    12233 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/slide_level_map_test.py
-drwxr-x---   0 armant   (1130519) primarygroup (89939)        0 2023-06-30 04:54:43.886592 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/
--rw-r-----   0 armant   (1130519) primarygroup (89939)      334 2023-06-30 04:54:43.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/PKG-INFO
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1084 2023-06-30 04:54:43.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/SOURCES.txt
--rw-r-----   0 armant   (1130519) primarygroup (89939)        1 2023-06-30 04:54:43.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/dependency_links.txt
--rw-r-----   0 armant   (1130519) primarygroup (89939)      166 2023-06-30 04:54:43.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/requires.txt
--rw-r-----   0 armant   (1130519) primarygroup (89939)       16 2023-06-30 04:54:43.000000 ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/top_level.txt
--rw-r-----   0 armant   (1130519) primarygroup (89939)       38 2023-06-30 04:54:43.890592 ez_wsi_dicomweb-1.0.2/setup.cfg
--rw-r-----   0 armant   (1130519) primarygroup (89939)     1469 2023-06-30 04:53:33.000000 ez_wsi_dicomweb-1.0.2/setup.py
+drwxr-x---   0 armant   (1130519) primarygroup (89939)        0 2023-07-05 21:05:15.524872 ez_wsi_dicomweb-2.0.0/
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    11358 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/LICENSE
+-rw-r-----   0 armant   (1130519) primarygroup (89939)      334 2023-07-05 21:05:15.524872 ez_wsi_dicomweb-2.0.0/PKG-INFO
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     3135 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/README.md
+drwxr-x---   0 armant   (1130519) primarygroup (89939)        0 2023-07-05 21:05:15.524872 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/
+-rw-r-----   0 armant   (1130519) primarygroup (89939)        0 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/__init__.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     2440 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/abstract_slide_frame_cache.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1959 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_frame_decoder.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     2565 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_frame_decoder_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    31508 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_slide.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    48037 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_slide_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     3295 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_store.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1563 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_store_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     2475 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_test_utils.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    11455 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_web_interface.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    13493 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_web_interface_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1999 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/ez_wsi_errors.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1157 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/ez_wsi_errors_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     8126 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/magnification.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     8326 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/magnification_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     8084 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/patch_generator.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     9829 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/patch_generator_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     6671 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     2060 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing_converter.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1738 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing_converter_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    16095 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing_test.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    18280 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/slide_level_map.py
+-rw-r-----   0 armant   (1130519) primarygroup (89939)    12233 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/slide_level_map_test.py
+drwxr-x---   0 armant   (1130519) primarygroup (89939)        0 2023-07-05 21:05:15.524872 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/
+-rw-r-----   0 armant   (1130519) primarygroup (89939)      334 2023-07-05 21:05:15.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/PKG-INFO
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1084 2023-07-05 21:05:15.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/SOURCES.txt
+-rw-r-----   0 armant   (1130519) primarygroup (89939)        1 2023-07-05 21:05:15.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/dependency_links.txt
+-rw-r-----   0 armant   (1130519) primarygroup (89939)      166 2023-07-05 21:05:15.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/requires.txt
+-rw-r-----   0 armant   (1130519) primarygroup (89939)       16 2023-07-05 21:05:15.000000 ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/top_level.txt
+-rw-r-----   0 armant   (1130519) primarygroup (89939)       38 2023-07-05 21:05:15.524872 ez_wsi_dicomweb-2.0.0/setup.cfg
+-rw-r-----   0 armant   (1130519) primarygroup (89939)     1469 2023-07-05 21:03:43.000000 ez_wsi_dicomweb-2.0.0/setup.py
```

### Comparing `ez_wsi_dicomweb-1.0.2/LICENSE` & `ez_wsi_dicomweb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/README.md` & `ez_wsi_dicomweb-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/abstract_slide_frame_cache.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/abstract_slide_frame_cache.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_frame_decoder.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_frame_decoder.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_frame_decoder_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_frame_decoder_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_slide.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_slide.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,22 +31,22 @@
      |--> DicomImagePatch: a rectangular patch/tile of an Image
 """
 from __future__ import annotations
 
 import dataclasses
 import heapq
 import math
-from typing import Any, Generator, Iterator, List, Mapping, MutableMapping, Optional, Tuple
+from typing import Any, Iterator, List, Mapping, MutableMapping, Optional, Tuple
 
 import cachetools
 from ez_wsi_dicomweb import abstract_slide_frame_cache
 from ez_wsi_dicomweb import dicom_frame_decoder
 from ez_wsi_dicomweb import dicom_web_interface
 from ez_wsi_dicomweb import ez_wsi_errors
-from ez_wsi_dicomweb import magnification as magnification_module
+from ez_wsi_dicomweb import pixel_spacing as pixel_spacing_module
 from ez_wsi_dicomweb import slide_level_map
 import numpy as np
 
 from hcls_imaging_ml_toolkit import dicom_path
 from hcls_imaging_ml_toolkit import tags
 
 
@@ -89,39 +89,41 @@
   return (
       dicom_frame_decoder.can_decompress_dicom_transfer_syntax(transfer_syntax)
       or transfer_syntax in _SUPPORTED_CLIENT_SIDE_DECODING_RAW_TRANSFER_SYNTAXS
   )
 
 
 class Image:
-  """Represents an image at a specific magnification in a DicomSlide."""
+  """Represents an image at a specific pixel spacing in a DicomSlide."""
 
   def __init__(
-      self, magnification: magnification_module.Magnification, slide: DicomSlide
+      self, pixel_spacing: pixel_spacing_module.PixelSpacing, slide: DicomSlide
   ):
     """Constructor for DicomImage.
 
     Args:
-      magnification: The magnification level the image belongs to.
+      pixel_spacing: The pixel_spacing of the image.
       slide: The parent slide this image belongs to.
 
     Raises:
-      ValueError if the requested magnification is not valid.
+      ValueError if the requested pixel spacing is not valid.
+      PixelSpacingLevelNotFoundError if the pixel spacing does not exist.
     """
-    self.magnification = magnification
+    self.pixel_spacing = pixel_spacing
     self._slide = slide
 
-    level_at_mag = slide.get_level_by_magnification(magnification)
-    if not level_at_mag:
-      raise ez_wsi_errors.MagnificationLevelNotFoundError(
-          f'No level found at magnification {magnification}'
+    level_at_ps = self._slide.get_level_by_pixel_spacing(self.pixel_spacing)
+    if not level_at_ps:
+      raise ez_wsi_errors.PixelSpacingLevelNotFoundError(
+          'No level found at pixel spacing:'
+          f' {self.pixel_spacing.pixel_spacing_mm}'
       )
 
-    self.width = level_at_mag.width
-    self.height = level_at_mag.height
+    self.width = level_at_ps.width
+    self.height = level_at_ps.height
 
   @property
   def slide(self):
     return self._slide
 
   def image_bytes(self) -> np.ndarray:
     """Loads the pixel bytes of the DICOM Image.
@@ -129,15 +131,15 @@
     Returns:
       Numpy array representing the DICOM Image.
     """
     # Internally reuses the Patch implementation for bytes fetching.
     # An image can be represented as a giant patch starting from (0, 0)
     # and spans the whole slide.
     return self._slide.get_patch(
-        magnification=self.magnification,
+        pixel_spacing=self.pixel_spacing,
         x=0,
         y=0,
         width=self.width,
         height=self.height,
     ).image_bytes()
 
 
@@ -148,72 +150,71 @@
   x_origin: int  # The upper leftmost x coordinate of the patch intersection.
   y_origin: int  # The upper leftmost y coordinate of the patch intersection.
   width: int
   height: int
 
 
 class Patch:
-  """A rectangular patch/tile/view of an Image at a specific magnification.
+  """A rectangular patch/tile/view of an Image at a specific pixel spacing.
 
   A Patch's data is composed from its overlap with one or more DICOM Frames.
   """
 
   def __init__(
       self,
-      magnification: magnification_module.Magnification,
+      pixel_spacing: pixel_spacing_module.PixelSpacing,
       x: int,
       y: int,
       width: int,
       height: int,
       slide: DicomSlide = None,
   ):
     """Constructor.
 
     Args:
-      magnification: The magnification level the patch belongs to. It defines
-        the pixel space for the coordinates (x, y, width, height).
+      pixel_spacing: The pixel spacing the patch belongs to.
       x: The X coordinate of the starting point (upper-left corner) of the
         patch.
       y: The Y coordinate of the starting point (upper-left corner) of the
         patch.
       width: The width of the patch.
       height: The height of the patch.
       slide: The parent DICOM Slide this patch belongs to.
     """
-    self.magnification = magnification
+    self.pixel_spacing = pixel_spacing
     self.x = x
     self.y = y
     self.width = width
     self.height = height
     self._slide = slide
 
   def __eq__(self, other: Any) -> bool:
     if not isinstance(other, Patch):
       return False
 
     return (
-        self.magnification == other.magnification
+        self.pixel_spacing == other.pixel_spacing
         and self.x == other.x
         and self.y == other.y
         and self.width == other.width
         and self.height == other.height
         and self._slide == other._slide
     )
 
   @property
   def id(self) -> str:
     if not self.slide or not self.slide.accession_number:
       return (
-          f'M_{self.magnification.as_string}:'
+          f'M_{self.pixel_spacing.as_magnification_string}:'
           f'{self.width:06d}x{self.height:06d}{self.x:+07d}{self.y:+07d}'
       )
     # Be consistent with internal id format.
     # "%s:%06dx%06d%+07d%+07d", image_id, width, height, left, top
     return (
-        f'{self.slide.accession_number}:M_{self.magnification.as_string}:'
+        f'{self.slide.accession_number}:M_{self.pixel_spacing.as_magnification_string}:'
         f'{self.width:06d}x{self.height:06d}{self.x:+07d}{self.y:+07d}'
     )
 
   @property
   def slide(self):
     return self._slide
 
@@ -294,60 +295,68 @@
         dst_image_np,
         x - self.x,
         y - self.y,
     )
     # pylint: enable=protected-access
     return width, height
 
-  def frame_number(self) -> Generator[int, None, None]:
-    """Yields slide level frame numbers required to render patch.
+  def frame_number(self) -> Iterator[int]:
+    """Generates slide level frame numbers required to render patch.
 
     Frame numbering starts at 0.
+
+    Yields:
+      A generator that produces frame numbers.
+
+    Raises:
+      PixelSpacingNotFoundError if the pixel spacing does not exist.
     """
     if self._slide is None:
       raise ez_wsi_errors.DicomSlideMissingError(
           'Unable to get image pixels. Parent slide is None.'
       )
-    level = self._slide.get_level_by_magnification(self.magnification)
-    if not level:
-      raise ez_wsi_errors.MagnificationLevelNotFoundError(
-          f'No level found at magnification {self.magnification}'
+
+    level_at_ps = self._slide.get_level_by_pixel_spacing(self.pixel_spacing)
+    if not level_at_ps:
+      raise ez_wsi_errors.PixelSpacingLevelNotFoundError(
+          'No level found at pixel spacing:'
+          f' {self.pixel_spacing.pixel_spacing_mm}'
       )
 
     y = self.y
     x = self.x
     width = self.width
     height = self.height
     cy = y
-    frame_width = level.frame_width
-    frame_height = level.frame_height
+    frame_width = level_at_ps.frame_width
+    frame_height = level_at_ps.frame_height
     cached_instance = None
     last_instance_frame_index = -1
     while cy < y + height:
       cx = x
       region_height = 0
       while cx < x + width:
         try:
-          frame_number = level.get_frame_number_by_point(cx, cy)
+          frame_number = level_at_ps.get_frame_number_by_point(cx, cy)
           if (
               cached_instance is None
               or frame_number - cached_instance.frame_offset
               >= cached_instance.frame_count
           ):
-            cached_instance = level.get_instance_by_frame(frame_number)
+            cached_instance = level_at_ps.get_instance_by_frame(frame_number)
             last_instance_frame_index = -1
             if cached_instance is None:
               raise ez_wsi_errors.FrameNumberOutofBoundsError()
           instance_frame_index = cached_instance.frame_index_from_frame_number(
               frame_number
           )
           if instance_frame_index > last_instance_frame_index:
             yield instance_frame_index + cached_instance.frame_offset - 1
           last_instance_frame_index = instance_frame_index
-          pos_x, pos_y = level.get_frame_position(frame_number)
+          pos_x, pos_y = level_at_ps.get_frame_position(frame_number)
           intersection = self._get_intersection(
               pos_x, pos_y, frame_width, frame_height
           )
           region_width = intersection.width
           region_height = intersection.height
         except ez_wsi_errors.EZWsiError:
           # No frame found at (cx, cy), move 1 pixel in both X, and Y direction.
@@ -362,33 +371,35 @@
     Returns:
       Numpy array type image.
 
     Raises:
       DicomSlideMissingError if slide used to create self is None.
       PatchOutOfBoundsError if the patch is not within the bounds of the DICOM
       image.
+      PixelSpacingNotFoundError if the pixel spacing does not exist.
     """
     if self._slide is None:
       raise ez_wsi_errors.DicomSlideMissingError(
           'Unable to get image pixels. Parent slide is None.'
       )
-    level = self._slide.get_level_by_magnification(self.magnification)
-    if not level:
-      raise ez_wsi_errors.MagnificationLevelNotFoundError(
-          f'No level found at magnification {self.magnification}'
+    level_at_ps = self._slide.get_level_by_pixel_spacing(self.pixel_spacing)
+    if not level_at_ps:
+      raise ez_wsi_errors.PixelSpacingLevelNotFoundError(
+          'No level found at pixel spacing:'
+          f' {self.pixel_spacing.pixel_spacing_mm}'
       )
 
     image_bytes = np.zeros(
-        (self.height, self.width, level.samples_per_pixel),
+        (self.height, self.width, level_at_ps.samples_per_pixel),
         self.slide.pixel_format,
     )
     pixel_copied = False
     # Copies image pixels from all overlapped frames.
     for frame_number in self.frame_number():
-      frame = self.slide.get_frame(self.magnification, frame_number)
+      frame = self.slide.get_frame(self.pixel_spacing, frame_number)
       if frame is None:
         continue
       try:
         self._copy_overlapped_region(frame, image_bytes)
         pixel_copied = True
       except ez_wsi_errors.EZWsiError:
         continue
@@ -409,40 +420,21 @@
   Args:
     slm: The source SlideLevelMap to get the native level from.
 
   Returns:
     The level that has the lowest index in the slide.
 
   Raises:
-    MagnificationLevelNotFoundError if the native level does not exist.
+    LevelNotFoundError if the native level does not exist.
   """
   level = slm.get_level(slm.level_index_min)
   if level is not None:
     return level
   else:
-    raise ez_wsi_errors.MagnificationLevelNotFoundError(
-        'The native level is missing.'
-    )
-
-
-def _get_magnification(
-    level: slide_level_map.Level,
-) -> magnification_module.Magnification:
-  """Gets the magnification corresponding to the input level.
-
-  Args:
-    level: The level to find the magnification of.
-
-  Returns:
-    The magnification corresponding to the input level.
-  """
-  pixel_spacing_um = (
-      max(level.pixel_spacing_x_mm, level.pixel_spacing_y_mm) * 1000
-  )
-  return magnification_module.Magnification.FromPixelSize(pixel_spacing_um)
+    raise ez_wsi_errors.LevelNotFoundError('The native level is missing.')
 
 
 def _get_pixel_format(level: slide_level_map.Level) -> np.dtype:
   """Gets the pixel format of the provided level.
 
   Args:
     level: The level to get the pixel format for.
@@ -542,15 +534,17 @@
     """
     self._level_map = slide_level_map.SlideLevelMap(dwi.get_instances(path))
     self._dwi = dwi
     self.path = path
     self.accession_number = accession_number
     native_level = _get_native_level(self._level_map)
     self.pixel_format = _get_pixel_format(native_level)
-    self.native_magnification = _get_magnification(native_level)
+    self.native_pixel_spacing = pixel_spacing_module.PixelSpacing(
+        native_level.pixel_spacing_x_mm, native_level.pixel_spacing_y_mm
+    )
     # Native height
     self.total_pixel_matrix_rows = native_level.height
     # Native width
     self.total_pixel_matrix_columns = native_level.width
     self._server_request_frame_lru_cache_size = frame_cache_size
     self._server_request_frame_cache = cachetools.LRUCache(frame_cache_size)
     self._enable_client_slide_frame_decompression = (
@@ -612,39 +606,38 @@
     return self._dwi
 
   @dwi.setter
   def dwi(self, val: dicom_web_interface.DicomWebInterface) -> None:
     self._dwi = val
 
   @property
-  def magnifications(self) -> list[magnification_module.Magnification]:
-    """Lists all Magnifications in the DicomSlide."""
+  def all_pixel_spacing_mms(self) -> list[float]:
+    """Lists all Pixel Spacings in mm in the DicomSlide."""
     return [
-        magnification_module.Magnification.FromPixelSize(
-            level.pixel_spacing_x_mm * 1000
-        )
-        for level in self._level_map.level_map.values()
+        level.pixel_spacing_x_mm for level in self._level_map.level_map.values()
     ]
 
-  def get_level_by_magnification(
-      self, magnification: magnification_module.Magnification
+  def get_level_by_pixel_spacing(
+      self,
+      pixel_spacing: pixel_spacing_module.PixelSpacing,
   ) -> Optional[slide_level_map.Level]:
-    """Gets the level corresponding to the input magnification.
+    """Gets the level corresponding to the input pixel spacing.
 
     Args:
-      magnification: The magnification to use for level lookup.
+      pixel_spacing: The pixel spacing to use for level lookup.
 
     Returns:
-      The level corresponding to the input magnification. None if the requested
-      magnification level does not exist.
+      The level corresponding to the input pixel spacing. None if the requested
+      pixel spacing does not exist.
     """
     # Converts pixel spacing returned by Magnification.NominalPixelSize() from
     # micrometers to millimeters.
-    pixel_spacing_mm = magnification.nominal_pixel_size / 1000
-    return self._level_map.get_level_by_pixel_spacing(pixel_spacing_mm)
+    return self._level_map.get_level_by_pixel_spacing(
+        pixel_spacing.pixel_spacing_mm
+    )
 
   def _get_cached_frame_bytes(
       self,
       instance: slide_level_map.Instance,
       frame_number: int,
   ) -> Optional[bytes]:
     """Returns frame bytes from frame cache if possible.
@@ -760,39 +753,42 @@
           dicom_web_interface.TranscodeDicomFrame.UNCOMPRESSED_LITTLE_ENDIAN,
       )
     return np.frombuffer(frame_raw_bytes, self.pixel_format).reshape(
         (level.frame_height, level.frame_width, level.samples_per_pixel)
     )
 
   def get_frame(
-      self, magnification: magnification_module.Magnification, frame_number: int
+      self, pixel_spacing: pixel_spacing_module.PixelSpacing, frame_number: int
   ) -> Optional[Frame]:
-    """Gets a frame at a specific magnification level.
+    """Gets a frame at a specific pixel_spacing in mm.
 
     The DICOMWeb API serves image pixels by the unit of frames. Frames have
     fixed size (width and height). Call get_patch() instead if you want to get
     an image patch at a specific loation, or with a specific dimension.
 
     The function utilizes a LRUCache to cache the most recent used frames.
 
     Args:
-      magnification: The magnification level to fetch the frame from.
+      pixel_spacing: The pixel spacing to fetch the frame from.
       frame_number: The frame number to be fetched. The frames are stored in
         arrays with 1-based indexing.
 
     Returns:
       Returns the requested frame if exists, None otherwise.
 
     Raises:
       InputFrameNumberOutOfRangeError if the input frame_number is
       out of range.
     """
-    level = self.get_level_by_magnification(magnification)
-    if level is None:
+    level = self._level_map.get_level_by_pixel_spacing(
+        pixel_spacing.pixel_spacing_mm
+    )
+    if not level:
       return None
+
     if (
         frame_number < level.frame_number_min
         or frame_number > level.frame_number_max
     ):
       raise ez_wsi_errors.InputFrameNumberOutOfRangeError(
           f'frame_number value [{frame_number}] is out of range: '
           f'[{level.frame_number_min}, {level.frame_number_max}]'
@@ -826,83 +822,88 @@
         width=level.frame_width,
         height=level.frame_height,
         image_np=frame_ndarray,
     )
     return frame
 
   def get_image(
-      self, magnification: magnification_module.Magnification
+      self, pixel_spacing: pixel_spacing_module.PixelSpacing
   ) -> Image:
-    """Gets an image from a specific magnification."""
-    return Image(magnification, self)
+    """Gets an image from a specific pixel spacing."""
+    return Image(pixel_spacing, self)
 
   def get_patch(
       self,
-      magnification: magnification_module.Magnification,
+      pixel_spacing: pixel_spacing_module.PixelSpacing,
       x: int,
       y: int,
       width: int,
       height: int,
   ) -> Patch:
-    """Gets a patch from a specific magnification level of the slide.
+    """Gets a patch from a specific pixel spacing of the slide.
 
     The area of a patch is defined by its position(x, y) and its dimension
     (width, height). The position of a patch corresponds to the first pixel in
     the patch and has the smallest coordinates. All coordinates(x, y, width and
-    height) are defined in the pixel space of the requested magnification level.
+    height) are defined in the pixel space of the requested pixel spacing.
 
     This routine creates the requested patch on-the-fly, by sampling image
     pixels from all frames that are overlapped with the patch.
 
     Args:
-      magnification: The magnification level to fetch the frame from.
+      pixel_spacing: The pixel spacing to fetch the frame from.
       x: The X coordinate of the patch position.
       y: The Y coordinate of the patch position.
       width: The width of the patch.
       height: The height of the patch.
 
     Returns:
       Returns the requested patch if exists, None otherwise.
 
     Raises:
-      MagnificationLevelNotFoundError if the requested level does not exist, or
+      PixelSpacingNotFoundError if the requested level does not exist, or
       if the requested patch is out of the scope of the image.
     """
-    level = self.get_level_by_magnification(magnification)
-    if level is None:
-      raise ez_wsi_errors.MagnificationLevelNotFoundError(
-          f'The requested magnification level {magnification.as_string} '
-          'does not exist.'
+    level = self._level_map.get_level_by_pixel_spacing(
+        pixel_spacing.pixel_spacing_mm
+    )
+    if not level:
+      raise ez_wsi_errors.PixelSpacingLevelNotFoundError(
+          f'No level found at pixel spacing: {pixel_spacing.pixel_spacing_mm}'
       )
-    patch = Patch(magnification, x, y, width, height, slide=self)
+
+    patch = Patch(pixel_spacing, x, y, width, height, slide=self)
     return patch
 
   def get_patch_bounds_dicom_instance_frame_numbers(
       self,
-      mag: magnification_module.Magnification,
+      pixel_spacing: pixel_spacing_module.PixelSpacing,
       patch_bounds_list: List[PatchBounds],
   ) -> Mapping[str, List[int]]:
     """Returns Map[DICOM instances: frame numbers] that fall in patch bounds.
 
     Args:
-      mag: Magnification patch bounding list was generated at.
+      pixel_spacing: pixel spacing patch bounding list was generated at.
       patch_bounds_list: List of PatchBounds to return frame indexes for.
 
     Returns:
       Mapping between DICOM instances, path, and list of frames numbers required
       to render patches.
     """
-    level = self.get_level_by_magnification(mag)
-    if level is None:
+    level = self._level_map.get_level_by_pixel_spacing(
+        pixel_spacing.pixel_spacing_mm
+    )
+    if not level:
       return {}
+
     slide_instance_frame_map = {}
     indexes_required_for_inference = []
     for patch_bounds in patch_bounds_list:
       patch = self.get_patch(
-          mag,
+          pixel_spacing,
           patch_bounds.x_origin,
           patch_bounds.y_origin,
           patch_bounds.width,
           patch_bounds.height,
       )
       # Frame indexes returns a list of indexes in the patch. Indexes
       # are returned in sorted order.
```

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_slide_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_slide_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from absl.testing import absltest
 from absl.testing import parameterized
 from ez_wsi_dicomweb import abstract_slide_frame_cache
 from ez_wsi_dicomweb import dicom_slide
 from ez_wsi_dicomweb import dicom_test_utils
 from ez_wsi_dicomweb import dicom_web_interface
 from ez_wsi_dicomweb import ez_wsi_errors
-from ez_wsi_dicomweb import magnification
+from ez_wsi_dicomweb import pixel_spacing
 from ez_wsi_dicomweb import slide_level_map
 import numpy as np
 import PIL.Image
 
 from hcls_imaging_ml_toolkit import dicom_path
 
 
@@ -284,74 +284,94 @@
     )
 
     val = mock.MagicMock()
     slide.dwi = val
     self.assertIs(slide.dwi, val)
     self.assertIs(slide._dwi, val)
 
-  def test_get_magnifications(self):
+  def test_get_ps(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
     self.assertListEqual(
-        slide.magnifications,
+        slide.all_pixel_spacing_mms,
         [
-            magnification.Magnification.FromString('40X'),
-            magnification.Magnification.FromString('20X'),
-            magnification.Magnification.FromString('10X'),
-            magnification.Magnification.FromString('5X'),
-            magnification.Magnification.FromString('2.5X'),
-            magnification.Magnification.FromString('1.25X'),
-            magnification.Magnification.FromString('0.625X'),
-            magnification.Magnification.FromString('0.3125X'),
-            magnification.Magnification.FromString('0.15625X'),
-            magnification.Magnification.FromString('0.078125X'),
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.00024309399214433264
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.0004861879842886653
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.0009723759685773306
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.0019447519371546612
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.0038895038743093223
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.007779007748618645
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.01555801549723729
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.03111603099447458
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.06223206198894916
+            ).pixel_spacing_mm,
+            pixel_spacing.PixelSpacing.FromDouble(
+                0.12446412397789831
+            ).pixel_spacing_mm,
         ],
     )
 
   def test_constructor(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
     self.assertIsNotNone(slide._level_map)
     self.assertEqual(
-        '40X',
-        slide.native_magnification.as_string,
-        'The native mangification of the test slide must be 40X.',
+        '41.13635117994051X',
+        slide.native_pixel_spacing.as_magnification_string,
+        'The native pixel spacing of the test slide must be 40X.',
     )
     self.assertEqual(199168, slide.total_pixel_matrix_rows)  # Tag: 00480007
     self.assertEqual(98816, slide.total_pixel_matrix_columns)  # Tag: 00480006
     self.assertEqual(
         np.uint8, slide.pixel_format, 'The pixel format is incorrect.'
     )
 
   def test_get_pixel_format_with_valid_input(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
-    level = slide.get_level_by_magnification(slide.native_magnification)
+    level = slide.get_level_by_pixel_spacing(slide.native_pixel_spacing)
     self.assertEqual(
         np.uint8,
         dicom_slide._get_pixel_format(level),
         'The pixel format is not correct.',
     )
 
   def test_get_pixel_format_with_unsupported_pixel_format_raises_error(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
-    level = slide.get_level_by_magnification(slide.native_magnification)
+    level = slide.get_level_by_pixel_spacing(slide.native_pixel_spacing)
     level = dataclasses.replace(level, bits_allocated=32)
     with self.assertRaises(ez_wsi_errors.UnsupportedPixelFormatError):
       dicom_slide._get_pixel_format(level)
 
   def test_get_native_level_with_valid_input(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
@@ -368,39 +388,39 @@
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
     slide._level_map._level_map[slide._level_map.level_index_min] = (
         None  # pytype: disable=unsupported-operands  # always-use-return-annotations
     )
-    with self.assertRaises(ez_wsi_errors.MagnificationLevelNotFoundError):
+    with self.assertRaises(ez_wsi_errors.LevelNotFoundError):
       dicom_slide._get_native_level(slide._level_map)
 
-  def test_get_level_with_nonexsting_mag_returns_none(self):
+  def test_get_level_with_nonexsting_ps_returns_none(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
-    level = slide.get_level_by_magnification(
-        magnification.Magnification.FromString('80X')
+    level = slide.get_level_by_pixel_spacing(
+        pixel_spacing.PixelSpacing.FromMagnificationString('80X')
     )
-    self.assertIsNone(level, 'There should be no level at magnification 80X.')
+    self.assertIsNone(level, 'There should be no level at pixel spacing 80X.')
 
-  def test_get_level_with_existing_mag_returns_valid_level(self):
+  def test_get_level_with_existing_ps_returns_valid_level(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
-    level = slide.get_level_by_magnification(
-        magnification.Magnification.FromString('10X')
+    level = slide.get_level_by_pixel_spacing(
+        pixel_spacing.PixelSpacing.FromMagnificationString('10X')
     )
     self.assertIsNotNone(
-        level, 'The testing slide should contain a level at magnification 10X.'
+        level, 'The testing slide should contain a level at ps 10X.'
     )
     if level is not None:
       self.assertEqual(24704, level.width)
       self.assertEqual(49792, level.height)
       self.assertEqual(500, level.frame_width)
       self.assertEqual(500, level.frame_height)
 
@@ -411,15 +431,15 @@
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
     with self.assertRaises(ez_wsi_errors.InputFrameNumberOutOfRangeError):
       slide.get_frame(
-          magnification.Magnification.FromString(mag),
+          pixel_spacing.PixelSpacing.FromMagnificationString(mag),
           frame_number,
       )
 
   def test_get_frame_normal(self):
     self.mock_dwi.get_frame_image.return_value = b'abc123abc123'
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
@@ -435,20 +455,20 @@
         2,
         2,
         level_1.frame_number_min,
         level_1.frame_number_max,
         level_1.samples_per_pixel,
         level_1.transfer_syntax_uid,
     )
-    frame = slide.get_frame(slide.native_magnification, 1)
+    frame = slide.get_frame(slide.native_pixel_spacing, 1)
     self.assertIsNotNone(
         frame,
         (
             'The testing slide must contain a frame at index 1 on the native '
-            'magnification level.'
+            'pixel spacing.'
         ),
     )
     if frame is not None:
       self.assertEqual(
           (2, 0, 2, 2),
           (frame.x_origin, frame.y_origin, frame.width, frame.height),
           'The location and dimension of the frame are not correct.',
@@ -519,15 +539,15 @@
             self.mock_dwi,
             self.dicom_series_path,
             enable_client_slide_frame_decompression=True,
         )
         _init_test_slide_level_map(
             slide, 6, 6, 1, 1, 0, 8, 1, transfer_syntax_uid
         )
-        level = slide.get_level_by_magnification(slide.native_magnification)
+        level = slide.get_level_by_pixel_spacing(slide.native_pixel_spacing)
         result = slide._get_frame_server_transcoding(
             level, level.instances[0], 1  # pytype: disable=attribute-error
         )
         self.assertEqual(
             mock_get_frame_from_cache.call_count,
             expected_mock_get_frame_from_cache_call_count,
         )
@@ -553,32 +573,34 @@
         2,
         2,
         level_1.frame_number_min,
         level_1.frame_number_max,
         level_1.samples_per_pixel,
         level_1.transfer_syntax_uid,
     )
-    frame_1 = slide.get_frame(slide.native_magnification, 1)
-    frame_2 = slide.get_frame(slide.native_magnification, 1)
+    frame_1 = slide.get_frame(slide.native_pixel_spacing, 1)
+    frame_2 = slide.get_frame(slide.native_pixel_spacing, 1)
     self.assertIsNotNone(frame_1)
     self.assertIsNotNone(frame_2)
     self.assertTrue(
         np.array_equal(frame_1.image_np, frame_2.image_np),
         'Cached frame not equal to original frame.',
     )
     self.mock_dwi.get_frame_image.assert_called_once()
 
-  def test_get_patch_with_invalid_magnification_raise_error(self):
+  def test_get_patch_with_invalid_pixel_spacing_raise_error(self):
     slide = dicom_slide.DicomSlide(
         self.mock_dwi,
         self.dicom_series_path,
         enable_client_slide_frame_decompression=True,
     )
-    with self.assertRaises(ez_wsi_errors.MagnificationLevelNotFoundError):
-      slide.get_patch(magnification.Magnification.FromString('80X'), 0, 0, 1, 1)
+    with self.assertRaises(ez_wsi_errors.PixelSpacingLevelNotFoundError):
+      slide.get_patch(
+          pixel_spacing.PixelSpacing.FromMagnificationString('80X'), 0, 0, 1, 1
+      )
 
   @parameterized.parameters(
       (-4, -4, 4, 4),
       (0, 7, 4, 4),
       (6, 7, 1, 2),
   )
   def test_get_patch_with_out_of_scope_patch_raise_error(
@@ -596,15 +618,15 @@
     # samples per pixel = 1
     # The image pixel values, with frame boundaries, are shown below:
     _init_test_slide_level_map(
         slide, 6, 6, 2, 2, 0, 8, 1, '1.2.840.10008.1.2.1'
     )
     with self.assertRaises(ez_wsi_errors.SectionOutOfImageBoundsError):
       slide.get_patch(
-          slide.native_magnification, x, y, width, height
+          slide.native_pixel_spacing, x, y, width, height
       ).image_bytes()
 
   @parameterized.named_parameters(
       dict(
           testcase_name='align_with_frame_boundary',
           x=0,
           y=0,
@@ -775,16 +797,19 @@
     # 24  25  | 28  29  | 32 33
     # 26  27  | 30  31  | 34 35
     # --------+---------+-------
     _init_test_slide_level_map(
         slide, 6, 6, 2, 2, 0, 8, 1, '1.2.840.10008.1.2.1'
     )
     self.mock_dwi.get_frame_image.side_effect = _fake_get_frame_raw_image
-    patch = slide.get_patch(slide.native_magnification, x, y, width, height)
-    self.assertEqual(patch.magnification, slide.native_magnification)
+    patch = slide.get_patch(slide.native_pixel_spacing, x, y, width, height)
+    self.assertEqual(
+        patch.pixel_spacing.pixel_spacing_mm,
+        slide.native_pixel_spacing.pixel_spacing_mm,
+    )
     self.assertEqual(
         [patch.x, patch.y, patch.width, patch.height], [x, y, width, height]
     )
     self.assertEqual(
         np.asarray(expected_array, np.uint8).reshape(height, width, 1).tolist(),
         patch.image_bytes().tolist(),
     )
@@ -860,19 +885,19 @@
         slide, 6, 6, 2, 2, 0, 8, 1, '1.2.840.10008.1.2.1', mock_path=True
     )
     self.mock_dwi.get_frame_image.side_effect = _fake_get_frame_raw_image
     expected = {
         str(dicom_path.FromPath(slide.path, instance_uid='1')): expected_array
     }
     patch_list = [
-        slide.get_patch(slide.native_magnification, x, y, width, height)
+        slide.get_patch(slide.native_pixel_spacing, x, y, width, height)
         for x, y, width, height in patch_pos_dim_list
     ]
     instance_frame_map = slide.get_patch_bounds_dicom_instance_frame_numbers(
-        patch_list[0].magnification,
+        patch_list[0].pixel_spacing,
         [patch.patch_bounds for patch in patch_list],
     )
 
     self.assertEqual(instance_frame_map, expected)
 
   def test_get_dicom_instance_frames_across_concat_instances(self):
     mock_dwi = dicom_test_utils.create_mock_dicom_web_interface(
@@ -896,17 +921,17 @@
         level_1.frame_number_min,
         level_1.frame_number_max,
         1,
         level_1.transfer_syntax_uid,
         mock_path=True,
     )
     mock_dwi.get_frame_image.side_effect = _fake_get_frame_raw_image
-    patch_list = [slide.get_patch(slide.native_magnification, 0, 0, 8, 6)]
+    patch_list = [slide.get_patch(slide.native_pixel_spacing, 0, 0, 8, 6)]
     instance_frame_map = slide.get_patch_bounds_dicom_instance_frame_numbers(
-        patch_list[0].magnification,
+        patch_list[0].pixel_spacing,
         [patch.patch_bounds for patch in patch_list],
     )
     expected = {
         str(dicom_path.FromPath(slide.path, instance_uid='1')): [
             1,
             2,
             3,
@@ -947,17 +972,17 @@
         level_1.frame_number_min,
         level_1.frame_number_max,
         1,
         level_1.transfer_syntax_uid,
         mock_path=True,
     )
     mock_dwi.get_frame_image.side_effect = _fake_get_frame_raw_image
-    patch_list = [slide.get_patch(slide.native_magnification, 0, 0, 8, 6)]
+    patch_list = [slide.get_patch(slide.native_pixel_spacing, 0, 0, 8, 6)]
     instance_frame_map = slide.get_patch_bounds_dicom_instance_frame_numbers(
-        patch_list[0].magnification.next_higher_magnification,
+        pixel_spacing.PixelSpacing.FromMagnificationString('500X'),
         [patch.patch_bounds for patch in patch_list],
     )
     self.assertEmpty(instance_frame_map)
 
   @parameterized.named_parameters(
       dict(
           testcase_name='align_with_frame_boundary',
@@ -1068,16 +1093,19 @@
     # ----+----+-----
     #  7  |  8 |  9
     # ----+----+-----
     _init_test_slide_level_map(
         slide, 6, 6, 2, 2, 0, 8, 1, '1.2.840.10008.1.2.1'
     )
     self.mock_dwi.get_frame_image.side_effect = _fake_get_frame_raw_image
-    patch = slide.get_patch(slide.native_magnification, x, y, width, height)
-    self.assertEqual(patch.magnification, slide.native_magnification)
+    patch = slide.get_patch(slide.native_pixel_spacing, x, y, width, height)
+    self.assertEqual(
+        patch.pixel_spacing.pixel_spacing_mm,
+        slide.native_pixel_spacing.pixel_spacing_mm,
+    )
     self.assertEqual(
         [patch.x, patch.y, patch.width, patch.height], [x, y, width, height]
     )
     # sort order is expected
     self.assertEqual(expected_array, list(patch.frame_number()))
 
   def test_get_image(self):
@@ -1104,16 +1132,19 @@
     # 24  25  | 28  29  | 32 33
     # 26  27  | 30  31  | 34 35
     # --------+---------+-------
     _init_test_slide_level_map(
         slide, 6, 6, 2, 2, 0, 8, 1, '1.2.840.10008.1.2.1'
     )
     self.mock_dwi.get_frame_image.side_effect = _fake_get_frame_raw_image
-    image = slide.get_image(slide.native_magnification)
-    self.assertEqual(image.magnification, slide.native_magnification)
+    image = slide.get_image(slide.native_pixel_spacing)
+    self.assertEqual(
+        image.pixel_spacing.pixel_spacing_mm,
+        slide.native_pixel_spacing.pixel_spacing_mm,
+    )
     self.assertEqual([image.width, image.height], [6, 6])
     self.assertEqual(
         np.asarray(
             [
                 0,
                 1,
                 4,
@@ -1224,19 +1255,24 @@
     # --------+---------+-------
     # 12  13  | 16  17  | 20 21
     # 14  15  | 18  19  | 22 23
     # --------+---------+-------
     # 24  25  | 28  29  | 32 33
     # 26  27  | 30  31  | 34 35
     # --------+---------+-------
-    _init_test_slide_level_map(
-        slide, 6, 6, 2, 2, 0, 8, 1, '1.2.840.10008.1.2.1'
-    )
-    image = slide.get_image(slide.native_magnification)
-    self.assertEqual(image.magnification, slide.native_magnification)
+    slide._level_map._level_map[1].width = 6
+    slide._level_map._level_map[1].height = 6
+    slide._level_map._level_map[1].frame_width = 2
+    slide._level_map._level_map[1].frame_height = 2
+    slide._level_map._level_map[1].frame_number_min = 0
+    slide._level_map._level_map[1].frame_number_max = 8
+    slide._level_map._level_map[1].samples_per_pixel = 1
+    slide._level_map._level_map[1].transfer_syntax_uid = '1.2.840.10008.1.2.1'
+    image = slide.get_image(slide.native_pixel_spacing)
+    self.assertEqual(image.pixel_spacing, slide.native_pixel_spacing)
     self.assertEqual([image.width, image.height], [6, 6])
     self.assertEqual(
         np.asarray(
             [
                 0,
                 1,
                 4,
@@ -1282,17 +1318,17 @@
     )
     self.assertEqual(self.mock_dwi.get_frame_image.call_count, 0)
 
   @parameterized.parameters((3, 3, 2, 2), (4, 5, 3, 3), (-1, -1, 1, 1))
   def test_copy_overlapped_region_with_invalid_input_raise_error(
       self, dst_x: int, dst_y: int, dst_width: int, dst_height: int
   ):
-    mag = magnification.Magnification.FromString('40X')
+    ps = pixel_spacing.PixelSpacing.FromMagnificationString('40X')
     src_frame = dicom_slide.Frame(0, 0, 3, 3, np.ndarray((3, 3, 3), np.uint8))
-    dst_patch = dicom_slide.Patch(mag, dst_x, dst_y, dst_width, dst_height)
+    dst_patch = dicom_slide.Patch(ps, dst_x, dst_y, dst_width, dst_height)
     with self.assertRaises(ez_wsi_errors.PatchIntersectionNotFoundError):
       dst_np = np.ndarray((dst_height, dst_width, 3), np.uint8)
       dst_patch._copy_overlapped_region(src_frame, dst_np)
 
   @parameterized.parameters(
       (1, 0, 2, 1, [[[0, 0, 0], [0, 0, 0]], [[1, 1, 1], [2, 2, 2]]]),
       (1, 1, 2, 2, [[[1, 1, 1], [2, 2, 2]], [[4, 4, 4], [5, 5, 5]]]),
@@ -1302,30 +1338,30 @@
       self,
       dst_x: int,
       dst_y: int,
       expected_region_width: int,
       expected_region_height: int,
       expected_array: np.ndarray,
   ):
-    mag = magnification.Magnification.FromString('40X')
+    ps = pixel_spacing.PixelSpacing.FromMagnificationString('40X')
     src_frame = dicom_slide.Frame(
         1,
         1,
         3,
         3,
         np.array(
             [
                 [[1, 1, 1], [2, 2, 2], [3, 3, 3]],
                 [[4, 4, 4], [5, 5, 5], [6, 6, 6]],
                 [[7, 7, 7], [8, 8, 8], [9, 9, 9]],
             ],
             np.uint8,
         ),
     )
-    dst_patch = dicom_slide.Patch(mag, dst_x, dst_y, 2, 2)
+    dst_patch = dicom_slide.Patch(ps, dst_x, dst_y, 2, 2)
     dst_np = np.zeros((2, 2, 3), np.uint8)
 
     region_width, region_height = dst_patch._copy_overlapped_region(
         src_frame, dst_np
     )
 
     self.assertEqual(
@@ -1386,15 +1422,15 @@
         self.mock_dwi,
         self.dicom_series_path,
         accession_number='slideid',
         enable_client_slide_frame_decompression=True,
     )
     self.assertEqual('slideid', slide.accession_number)
     patch = slide.get_patch(
-        magnification.Magnification.FromString('10X'),
+        pixel_spacing=pixel_spacing.PixelSpacing.FromMagnificationString('10X'),
         x=10,
         y=20,
         width=100,
         height=200,
     )
     self.assertEqual('slideid:M_10X:000100x000200+000010+000020', patch.id)
 
@@ -1426,16 +1462,19 @@
     x = 100
     y = 50
     width = 300
     height = 100
     expected_array = np.asarray(PIL.Image.open(dicom_test_utils.TEST_JPEG_PATH))
     expected_array = expected_array[y : y + height, x : x + width, :]
 
-    patch = slide.get_patch(slide.native_magnification, x, y, width, height)
-    self.assertEqual(patch.magnification, slide.native_magnification)
+    patch = slide.get_patch(slide.native_pixel_spacing, x, y, width, height)
+    self.assertEqual(
+        patch.pixel_spacing.pixel_spacing_mm,
+        slide.native_pixel_spacing.pixel_spacing_mm,
+    )
     self.assertEqual(
         [patch.x, patch.y, patch.width, patch.height], [x, y, width, height]
     )
     self.assertTrue(np.array_equal(expected_array, patch.image_bytes()))
     self.mock_dwi.get_frame_image.assert_called_once()
 
   def test_get_patch_from_jpeg_locally_fails_over_server_side_decoding(self):
@@ -1470,16 +1509,16 @@
     y = 2
     width = 4
     height = 2
     expected_array = np.asarray(
         [13, 16, 17, 20, 15, 18, 19, 22], np.uint8
     ).reshape(height, width, 1)
 
-    patch = slide.get_patch(slide.native_magnification, x, y, width, height)
-    self.assertEqual(patch.magnification, slide.native_magnification)
+    patch = slide.get_patch(slide.native_pixel_spacing, x, y, width, height)
+    self.assertEqual(patch.pixel_spacing, slide.native_pixel_spacing)
     self.assertEqual(
         [patch.x, patch.y, patch.width, patch.height], [x, y, width, height]
     )
     self.assertTrue(np.array_equal(expected_array, patch.image_bytes()))
     self.assertEqual(self.mock_dwi.get_frame_image.call_count, 3)
 
   def test_slide_levels(self):
```

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_store.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_store.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_store_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_store_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_test_utils.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_test_utils.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_web_interface.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_web_interface.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/dicom_web_interface_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/dicom_web_interface_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/ez_wsi_errors.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/ez_wsi_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,18 @@
   pass
 
 
 class InvalidMagnificationStringError(EZWsiError):
   pass
 
 
+class LevelNotFoundError(EZWsiError):
+  pass
+
+
 class MagnificationLevelNotFoundError(EZWsiError):
   pass
 
 
 class NoDicomLevelsDetectedError(EZWsiError):
   pass
 
@@ -67,14 +71,18 @@
   pass
 
 
 class PatchIntersectionNotFoundError(EZWsiError):
   pass
 
 
+class PixelSpacingLevelNotFoundError(EZWsiError):
+  pass
+
+
 class SectionOutOfImageBoundsError(EZWsiError):
   pass
 
 
 class SlideLevelContainsInstancesWithDifferentTransferSyntaxUIDError(
     EZWsiError
 ):
```

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/ez_wsi_errors_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/ez_wsi_errors_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/magnification.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/magnification.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/magnification_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/magnification_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/patch_generator_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/patch_generator_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from unittest import mock
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from ez_wsi_dicomweb import dicom_slide
 from ez_wsi_dicomweb import dicom_test_utils
 from ez_wsi_dicomweb import ez_wsi_errors
-from ez_wsi_dicomweb import magnification as mag_lib
 from ez_wsi_dicomweb import patch_generator as patch_generator_lib
+from ez_wsi_dicomweb import pixel_spacing
 import numpy as np
 from PIL import Image
 
 from hcls_imaging_ml_toolkit import dicom_path
 
 
 class PatchGeneratorTest(parameterized.TestCase):
@@ -49,15 +49,15 @@
             os.path.join(
                 dicom_test_utils.TEST_DATA_PATH, 'golden_inference_mask.png'
             )
         )
     )
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size=128,
         patch_size=patch_arr.shape[0],
         max_luminance=0.8,
     )
     np.testing.assert_array_almost_equal(
         expected,
         patch_generator._normalized_tissue_mask().astype(np.uint8) * 255,
@@ -77,15 +77,15 @@
     )
     mock_slide = mock.create_autospec(dicom_slide.DicomSlide)
     mock_image = mock.create_autospec(dicom_slide.Image)
     mock_slide.get_image.return_value = mock_image
     mock_image.image_bytes.return_value = patch_arr
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size=128,
         patch_size=patch_arr.shape[0],
         max_luminance=0.8,
     )
 
     # stride size 128 at 40X is 4 at 1.25X. Expected number of tissue patches is
     # 8 * 8 / 4 / 4 = 4
@@ -99,34 +99,36 @@
 
     mock_slide = mock.create_autospec(dicom_slide.DicomSlide)
     mock_image = mock.create_autospec(dicom_slide.Image)
     mock_slide.get_image.return_value = mock_image
     mock_image.image_bytes.return_value = patch_arr
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size=128,
         patch_size=patch_arr.shape[0],
         max_luminance=0.8,
-        tissue_mask_magnification=mag_lib.Magnification.FromString('2.5X'),
+        tissue_mask_pixel_spacing=pixel_spacing.PixelSpacing.FromMagnificationString(
+            '2.5X'
+        ),
     )
 
     # stride size 128 at 40X is 8 at 2.5X. Expected number of tissue patches is
     # 8 * 8 / 8 / 8 = 1
     self.assertEqual(1, patch_generator.total_num_patches())
 
   def test_total_strides(self):
     patch_arr = np.ones((8, 8, 3)) * 0.1
     mock_slide = mock.create_autospec(dicom_slide.DicomSlide)
     mock_image = mock.create_autospec(dicom_slide.Image)
     mock_slide.get_image.return_value = mock_image
     mock_image.image_bytes.return_value = patch_arr
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size=128,
         patch_size=patch_arr.shape[0],
         max_luminance=0.8,
     )
 
     # stride size 128 at 40X is 4 at 1.25X. Expected y_strides is 8 / 4 = 2,
     # expected x_strides is 8 / 4 = 2.
@@ -139,15 +141,15 @@
     patch_arr = np.ones((8, 8, 3)) * 0.1
     mock_slide = mock.create_autospec(dicom_slide.DicomSlide)
     mock_image = mock.create_autospec(dicom_slide.Image)
     mock_slide.get_image.return_value = mock_image
     mock_image.image_bytes.return_value = patch_arr
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size=512,
         patch_size=patch_arr.shape[0],
         max_luminance=0.8,
     )
 
     # stride size 512 at 40X is 16 at 1.25X. Expected y_strides is
     # max(8 / 16, 1) = 1, expected x_strides is max(8 / 16, 1) = 1.
@@ -176,15 +178,15 @@
         f'studies/{slide_uid}/series/{series_uid}'
     )
     mock_slide.path = dicom_path.FromString(dicom_full_path)
 
     threshold = 0
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size=128,
         patch_size=patch_arr.shape[0],
         max_luminance=threshold,
     )
     with self.assertRaisesRegex(
         ez_wsi_errors.DicomImageMissingRegionError,
         (
@@ -253,15 +255,15 @@
   )
   def test_coordinates_conversion(
       self, y_strides, x_strides, patch_size, stride_size, expected_patch_bounds
   ):
     mock_slide = mock.create_autospec(dicom_slide.DicomSlide)
     patch_generator = patch_generator_lib.PatchGenerator(
         mock_slide,
-        mag_lib.Magnification.FromString('40X'),
+        pixel_spacing.PixelSpacing.FromMagnificationString('40X'),
         stride_size,
         patch_size,
     )
     self.assertEqual(
         expected_patch_bounds,
         patch_generator.strides_to_patch_bounds(
             patch_generator_lib.StrideCoordinate(y_strides, x_strides)
```

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing_converter.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing_converter.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing_converter_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing_converter_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/pixel_spacing_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/pixel_spacing_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/slide_level_map.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/slide_level_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     Returns:
      The index of the frame within this instance.
     """
     return frame_number - self.frame_offset + 1
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass
 class Level:
   """Represents the dimensions and instances of a specific magnification level.
 
   Attributes:
     level_index: The index of the level using 1-based indexing. A level with a
       higher index corresponding to a lower magnification level.
     width: The width, in number of pixels, of the entire level.
```

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb/slide_level_map_test.py` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb/slide_level_map_test.py`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/ez_wsi_dicomweb.egg-info/SOURCES.txt` & `ez_wsi_dicomweb-2.0.0/ez_wsi_dicomweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez_wsi_dicomweb-1.0.2/setup.py` & `ez_wsi_dicomweb-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ==============================================================================
 """Install script for ez-wsi-dicomweb."""
 
 import setuptools
 
 setuptools.setup(
     name='ez_wsi_dicomweb',
-    version='1.0.2',
+    version='2.0.0',
     url='https://github.com/GoogleCloudPlatform/ez-wsi-dicomweb',
     author='Google LLC.',
     author_email='no-reply@google.com',
     license='Apache 2.0',
     description=(
         'A library that provides the ability to extract an image patch from a'
         ' pathology DICOM whole slide image.'
```

