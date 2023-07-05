# Comparing `tmp/spike2py-0.2.0.tar.gz` & `tmp/spike2py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spike2py-0.2.0.tar", last modified: Mon Jun 19 05:34:37 2023, max compression
+gzip compressed data, was "spike2py-0.2.1.tar", last modified: Wed Jul  5 05:21:06 2023, max compression
```

## Comparing `spike2py-0.2.0.tar` & `spike2py-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,23 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.577507 spike2py-0.2.0/
--rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-04-08 08:32:31.000000 spike2py-0.2.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     3069 2023-06-19 05:34:37.573507 spike2py-0.2.0/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     2595 2023-04-08 08:32:31.000000 spike2py-0.2.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-19 05:34:37.577507 spike2py-0.2.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      945 2023-06-19 05:34:18.000000 spike2py-0.2.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.573507 spike2py-0.2.0/spike2py/
--rw-r--r--   0 martin    (1000) martin    (1000)      166 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     7329 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/channels.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1264 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/demo.py
--rw-r--r--   0 martin    (1000) martin    (1000)     7464 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/plot.py
--rw-r--r--   0 martin    (1000) martin    (1000)     7263 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/read.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1569 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/reflex.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6980 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/sig_proc.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      606 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/temp_script.py
--rw-r--r--   0 martin    (1000) martin    (1000)     6056 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/trial.py
--rw-r--r--   0 martin    (1000) martin    (1000)      865 2023-04-08 08:32:31.000000 spike2py-0.2.0/spike2py/types.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.573507 spike2py-0.2.0/spike2py.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     3069 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      532 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       23 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-06-19 05:34:37.000000 spike2py-0.2.0/spike2py.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 05:34:37.573507 spike2py-0.2.0/tests/
--rw-r--r--   0 martin    (1000) martin    (1000)     3305 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_channels.py
--rw-r--r--   0 martin    (1000) martin    (1000)      858 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_demo.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1725 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_figures.py
--rw-r--r--   0 martin    (1000) martin    (1000)      773 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_plot.py
--rw-r--r--   0 martin    (1000) martin    (1000)     3350 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_read.py
--rw-r--r--   0 martin    (1000) martin    (1000)     9162 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_signal_processing.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1844 2023-04-08 08:32:31.000000 spike2py-0.2.0/tests/test_trial.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 05:21:06.684959 spike2py-0.2.1/
+-rw-r--r--   0 martin    (1000) martin    (1000)    35149 2023-04-08 08:32:31.000000 spike2py-0.2.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3396 2023-07-05 05:21:06.684959 spike2py-0.2.1/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)     2922 2023-07-05 05:17:42.000000 spike2py-0.2.1/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-05 05:21:06.684959 spike2py-0.2.1/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      945 2023-07-05 05:18:35.000000 spike2py-0.2.1/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 05:21:06.684959 spike2py-0.2.1/spike2py/
+-rw-r--r--   0 martin    (1000) martin    (1000)      166 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     8662 2023-07-05 04:37:33.000000 spike2py-0.2.1/spike2py/channels.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1264 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/demo.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7474 2023-07-03 02:40:10.000000 spike2py-0.2.1/spike2py/plot.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     7891 2023-07-05 05:12:52.000000 spike2py-0.2.1/spike2py/read.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1569 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/reflex.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6980 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/sig_proc.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      606 2023-04-08 08:32:31.000000 spike2py-0.2.1/spike2py/temp_script.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     6091 2023-07-05 04:38:10.000000 spike2py-0.2.1/spike2py/trial.py
+-rw-r--r--   0 martin    (1000) martin    (1000)      934 2023-07-05 04:25:25.000000 spike2py-0.2.1/spike2py/types.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 05:21:06.684959 spike2py-0.2.1/spike2py.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3396 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      378 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       23 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2023-07-05 05:21:06.000000 spike2py-0.2.1/spike2py.egg-info/top_level.txt
```

### Comparing `spike2py-0.2.0/LICENSE` & `spike2py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.0/PKG-INFO` & `spike2py-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spike2py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Import, parse and process data collected with Spike2
 Home-page: https://github.com/MartinHeroux/spike2py
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
@@ -48,14 +48,19 @@
 
 ```console
 $ python -m pip install spike2py
 ```
 
 **spike2py** officially supports Python 3.8+.
 
+## Caveat
+**spike2py** works with Matlab files exported from Spike2 v7, or any other Spike2 version that exports to Matlab 5.0 format.
+Spike2 v10 exports files to Matlab 7.3 format, which is currently not supported by **spike2py**.
+The ability to open both Matlab file formats will be added in future version of **spike2py**.
+
 ## Contributing
 
 Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
 
 ## Code of conduct
 
 This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
```

### Comparing `spike2py-0.2.0/README.md` & `spike2py-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 
 ```console
 $ python -m pip install spike2py
 ```
 
 **spike2py** officially supports Python 3.8+.
 
+## Caveat
+**spike2py** works with Matlab files exported from Spike2 v7, or any other Spike2 version that exports to Matlab 5.0 format.
+Spike2 v10 exports files to Matlab 7.3 format, which is currently not supported by **spike2py**.
+The ability to open both Matlab file formats will be added in future version of **spike2py**.
+
 ## Contributing
 
 Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
 
 ## Code of conduct
 
 This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
```

### Comparing `spike2py-0.2.0/setup.py` & `spike2py-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="spike2py",
-    version="0.2.0",
+    version="0.2.1",
     description="Import, parse and process data collected with Spike2",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MartinHeroux/spike2py",
     author="Martin Héroux",
     author_email="heroux.martin@gmail.com",
     license="GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `spike2py-0.2.0/spike2py/channels.py` & `spike2py-0.2.1/spike2py/channels.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import spike2py.plot as plot
 import spike2py.sig_proc as sig_proc
 
 from spike2py.types import (
     parsed_wavemark,
     parsed_waveform,
+    parsed_textmark,
     parsed_event,
     parsed_keyboard,
 )
 
 
 class ChannelInfo(NamedTuple):
     """Information about channel
@@ -138,14 +139,59 @@
             Set to `True` to save Keyboard figure to `path_save_figures`
         """
 
         plot.plot_channel(self, save=save)
         return self
 
 
+class Textmark(Channel):
+    """Textmark channel class
+
+    Inherits from Channel
+
+    Parameters
+    ----------
+    name
+        Name of textmark channel; default is 'Memory'
+    data_dict:
+        - ['path_save_figures']: Path - Directory where channel figure saved
+        - ['trial_name']: str - Name of trial where Keyboard was recorded
+        - ['subject_id']: str - Identifier
+        - ['times']: np.ndarray - Event times in seconds
+        - ['codes']: np.ndarray of str associated with keyboard events
+    """
+
+    def __init__(self, name: str, data_dict: parsed_textmark) -> None:
+        self.codes = data_dict["codes"]
+        super().__init__(
+            ChannelInfo(
+                name=name,
+                path_save_figures=data_dict["path_save_figures"],
+                trial_name=data_dict["trial_name"],
+                subject_id=data_dict["subject_id"],
+            ),
+            data_dict["times"],
+        )
+
+    def __repr__(self) -> str:
+        return "Textmark channel"
+
+    def plot(self, save: Literal[True, False] = False) -> None:
+        """Save Textmark channel figure
+
+        Parameters
+        ----------
+        save
+            Set to `True` to save Textmark figure to `path_save_figures`
+        """
+
+        plot.plot_channel(self, save=save)
+        return self
+
+
 class Waveform(Channel, sig_proc.SignalProcessing):
     """Waveform channel class
 
     Inherits from Channel and sig_proc.SignalProcessing
 
     Parameters
     ----------
```

### Comparing `spike2py-0.2.0/spike2py/demo.py` & `spike2py-0.2.1/spike2py/demo.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.0/spike2py/plot.py` & `spike2py-0.2.1/spike2py/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,26 +178,26 @@
         ax1.grid()
 
 
 def plot_trial(spike2py_trial: "trial.Trial", save: Literal[True, False]) -> None:
     fig_height, n_subplots = _fig_height_n_subplots(spike2py_trial)
     if n_subplots == 1:
         print(
-            f"The trial `{spike2py_trial.name}` has only one plottable channel."
+            f"The trial `{spike2py_trial.info.name}` has only one plottable channel."
             "\nPlease use `trial_name.ch_name.plot()` instead."
         )
     fig, ax = plt.subplots(
         sharex=True,
         nrows=n_subplots,
         figsize=(12, fig_height),
         gridspec_kw={"hspace": 0},
     )
     _plot_trial(spike2py_trial, ax)
     if save:
-        _save_plot(spike2py_trial.name)
+        _save_plot(spike2py_trial.info.name)
 
 
 def _fig_height_n_subplots(spike2py_trial: "trial.Trial") -> Tuple[int, int]:
     """Determine height and number of subplots to plot trial.
 
     Event, Keyboard and Wavemark channels are all plotted on same subplot at the top of the figure.
     Need to make sure these channels have data."""
```

### Comparing `spike2py-0.2.0/spike2py/read.py` & `spike2py-0.2.1/spike2py/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 import numpy as np
 
 from spike2py.types import (
     mat_data,
     parsed_wavemark,
     parsed_waveform,
     parsed_event,
+    parsed_textmark,
     parsed_keyboard,
     parsed_spike2py_data,
     parsed_mat_data,
 )
 
 CHANNEL_DATA_LENGTH: Final = {
     "event": 5,
     "keyboard": 6,
+    "textmark": 8,
     "waveform": 10,
     "wavemark": 14,
 }
 
 
 class WrongFileType(Exception):
     """Custom exception to use when `.mat` file not provided"""
@@ -100,14 +102,15 @@
     dict
         Channel data and metadata.
         The `keys` and `values` will differ for the different channel types.
         See the `_parse_mat_<channel type>` helper functions for details.
     """
     parser_lookup = {
         CHANNEL_DATA_LENGTH["event"]: _parse_mat_events,
+        CHANNEL_DATA_LENGTH["textmark"]: _parse_mat_textmark,
         CHANNEL_DATA_LENGTH["keyboard"]: _parse_mat_keyboard,
         CHANNEL_DATA_LENGTH["waveform"]: _parse_mat_waveform,
         CHANNEL_DATA_LENGTH["wavemark"]: _parse_mat_wavemark,
     }
     parsed_data = dict()
     for key, value in mat_data.items():
         parsed_data[key] = parser_lookup[len(value.dtype)](value)
@@ -159,14 +162,36 @@
     return {
         "codes": characters,
         "times": _flatten_array(mat_keyboard["times"]),
         "ch_type": "keyboard",
     }
 
 
+def _parse_mat_textmark(mat_textmark: np.ndarray) -> parsed_textmark:
+    """Parse textmark ('Memory') channel data as exported by Spike2 to .mat
+
+    Parameters
+    ----------
+    mat_textmark
+         Deeply nested array containing keyboard channel data and metadata.
+
+    Returns
+    -------
+    dict
+        Data from textmark channel.
+    """
+
+    codes = list(mat_textmark['text'][0][0])
+    return {
+        "codes": codes,
+        "times": _flatten_array(mat_textmark["times"]),
+        "ch_type": "textmark",
+    }
+
+
 def _keyboard_codes_to_characters(keyboard_codes: List[int]) -> List[str]:
     """Helper function that converts encoded character(s) into list of str
 
     Parameters
     ----------
     keyboard_codes
          List of int values, where each keyboard entry is encoded by four int
```

### Comparing `spike2py-0.2.0/spike2py/reflex.py` & `spike2py-0.2.1/spike2py/reflex.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.0/spike2py/sig_proc.py` & `spike2py-0.2.1/spike2py/sig_proc.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.0/spike2py/temp_script.py` & `spike2py-0.2.1/spike2py/temp_script.py`

 * *Files identical despite different names*

### Comparing `spike2py-0.2.0/spike2py/trial.py` & `spike2py-0.2.1/spike2py/trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from spike2py import channels, read, plot
 
 
 CHANNEL_GENERATOR = {
     "event": channels.Event,
     "keyboard": channels.Keyboard,
+    "textmark": channels.Textmark,
     "waveform": channels.Waveform,
     "wavemark": channels.Wavemark,
 }
 
 
 class TrialInfo(NamedTuple):
     """Information about trial
```

### Comparing `spike2py-0.2.0/spike2py/types.py` & `spike2py-0.2.1/spike2py/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 
 mat_data = Dict[str, np.ndarray]
 parsed_mat_data = Dict[str, dict]
 parsed_event = Dict[str, Union[np.ndarray, str, Path]]
 parsed_keyboard = Dict[str, Union[List[str], np.ndarray, str, Path]]
+parsed_textmark = Dict[str, Union[List[str], np.ndarray, str, Path]]
 parsed_waveform = Dict[str, Union[int, np.ndarray, str, Path]]
 parsed_wavemark = Dict[str, Union[int, List[int], str, np.ndarray, Path]]
 parsed_spike2py_data = Dict[
     str, Union[parsed_event, parsed_keyboard, parsed_waveform, parsed_wavemark]
 ]
 filt_cutoff_single = Union[float, int]
 filt_cutoff_pair = Union[List[float], List[float]]
```

### Comparing `spike2py-0.2.0/spike2py.egg-info/PKG-INFO` & `spike2py-0.2.1/spike2py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spike2py
-Version: 0.2.0
+Version: 0.2.1
 Summary: Import, parse and process data collected with Spike2
 Home-page: https://github.com/MartinHeroux/spike2py
 Author: Martin Héroux
 Author-email: heroux.martin@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
@@ -48,14 +48,19 @@
 
 ```console
 $ python -m pip install spike2py
 ```
 
 **spike2py** officially supports Python 3.8+.
 
+## Caveat
+**spike2py** works with Matlab files exported from Spike2 v7, or any other Spike2 version that exports to Matlab 5.0 format.
+Spike2 v10 exports files to Matlab 7.3 format, which is currently not supported by **spike2py**.
+The ability to open both Matlab file formats will be added in future version of **spike2py**.
+
 ## Contributing
 
 Like this project? Want to help? We would love to have your contribution! Please see [CONTRIBUTING](CONTRIBUTING.md) to get started.
 
 ## Code of conduct
 
 This project adheres to the Contributor Covenant code of conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [heroux.martin@gmail.com](heroux.martin@gmail.com).
```

