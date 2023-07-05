# Comparing `tmp/whisper_mic-1.0.1.tar.gz` & `tmp/whisper_mic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_mic-1.0.1.tar", last modified: Thu Jun 29 22:25:42 2023, max compression
+gzip compressed data, was "whisper_mic-1.1.0.tar", last modified: Wed Jul  5 05:55:37 2023, max compression
```

## Comparing `whisper_mic-1.0.1.tar` & `whisper_mic-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-06-29 22:25:42.756684 whisper_mic-1.0.1/
--rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.0.1/LICENSE
--rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-06-29 22:25:42.756684 whisper_mic-1.0.1/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)     3231 2023-06-29 22:23:36.000000 whisper_mic-1.0.1/README.md
--rw-rw-r--   0 blake     (1000) blake     (1000)      809 2023-06-29 22:24:52.000000 whisper_mic-1.0.1/pyproject.toml
--rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-06-29 22:25:42.756684 whisper_mic-1.0.1/setup.cfg
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-06-29 22:25:42.756684 whisper_mic-1.0.1/whisper_mic/
--rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.0.1/whisper_mic/__init__.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)     1600 2023-06-29 19:44:37.000000 whisper_mic-1.0.1/whisper_mic/cli.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)     3640 2023-06-29 19:44:37.000000 whisper_mic-1.0.1/whisper_mic/whisper_mic.py
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-06-29 22:25:42.756684 whisper_mic-1.0.1/whisper_mic.egg-info/
--rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-06-29 22:25:42.000000 whisper_mic-1.0.1/whisper_mic.egg-info/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)      314 2023-06-29 22:25:42.000000 whisper_mic-1.0.1/whisper_mic.egg-info/SOURCES.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-06-29 22:25:42.000000 whisper_mic-1.0.1/whisper_mic.egg-info/dependency_links.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-06-29 22:25:42.000000 whisper_mic-1.0.1/whisper_mic.egg-info/entry_points.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)      182 2023-06-29 22:25:42.000000 whisper_mic-1.0.1/whisper_mic.egg-info/requires.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-06-29 22:25:42.000000 whisper_mic-1.0.1/whisper_mic.egg-info/top_level.txt
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.1.0/LICENSE
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3231 2023-06-29 22:23:36.000000 whisper_mic-1.1.0/README.md
+-rw-rw-r--   0 blake     (1000) blake     (1000)      821 2023-07-05 05:54:48.000000 whisper_mic-1.1.0/pyproject.toml
+-rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/setup.cfg
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/whisper_mic/
+-rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.1.0/whisper_mic/__init__.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     1600 2023-06-29 19:44:37.000000 whisper_mic-1.1.0/whisper_mic/cli.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)      480 2023-07-05 05:53:32.000000 whisper_mic-1.1.0/whisper_mic/utils.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     4077 2023-07-05 05:53:32.000000 whisper_mic-1.1.0/whisper_mic/whisper_mic.py
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/whisper_mic.egg-info/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)      335 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/SOURCES.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/dependency_links.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/entry_points.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)      187 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/requires.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/top_level.txt
```

### Comparing `whisper_mic-1.0.1/LICENSE` & `whisper_mic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_mic-1.0.1/PKG-INFO` & `whisper_mic-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_mic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `whisper_mic-1.0.1/README.md` & `whisper_mic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `whisper_mic-1.0.1/pyproject.toml` & `whisper_mic-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_mic"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -27,13 +27,14 @@
     "tdqm",
     "more-itertools",
     "transformers",
     "torch",
     "ffmpeg-python",
     "click",
     "openai-whisper",
+    "rich",
     'importlib-metadata; python_version>"3.9"'
 ]
 
 [project.scripts]
 whisper_mic = "whisper_mic.cli:main"
```

### Comparing `whisper_mic-1.0.1/whisper_mic/cli.py` & `whisper_mic-1.1.0/whisper_mic/cli.py`

 * *Files identical despite different names*

### Comparing `whisper_mic-1.0.1/whisper_mic/whisper_mic.py` & `whisper_mic-1.1.0/whisper_mic/whisper_mic.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 import io
 import numpy as np
 from pydub import AudioSegment
 import os
 import tempfile
 import time
 
+from whisper_mic.utils import get_logger
+
 
 class WhisperMic:
     def __init__(self,model="base",device=("cuda" if torch.cuda.is_available() else "cpu"),english=False,verbose=False,energy=300,pause=0.8,dynamic_energy=False,save_file=False):
+        self.logger = get_logger("whisper_mic", "info")
         self.energy = energy
         self.pause = pause
         self.dynamic_energy = dynamic_energy
         self.save_file = save_file
         self.verbose = verbose
         self.english = english
 
@@ -28,82 +31,96 @@
 
         self.audio_queue = queue.Queue()
         self.result_queue = queue.Queue()
 
         self.break_threads = False
         self.mic_active = False
 
-        self.mic_thread = threading.Thread(target=self.record_audio, daemon=True)
-        self.mic_thread.start()
+        self.banned_results = [""," ","\n",None]
 
+        self.setup_mic()
 
-    def record_audio(self):
-        r = sr.Recognizer()
-        r.energy_threshold = self.energy
-        r.pause_threshold = self.pause
-        r.dynamic_energy_threshold = self.dynamic_energy
-        
-        with sr.Microphone(sample_rate=16000) as source:
-            self.mic_active = True
-            print("Say something!")
-            i = 0
-            while True:
-                if not self.mic_active:
-                    break
-                #get and save audio to wav file
-                audio = r.listen(source)
-                if self.save_file:
-                    data = io.BytesIO(audio.get_wav_data())
-                    audio_clip = AudioSegment.from_file(data)
-                    filename = os.path.join(self.temp_dir, f"temp{i}.wav")
-                    audio_clip.export(filename, format="wav")
-                    audio_data = filename
-                else:
-                    torch_audio = torch.from_numpy(np.frombuffer(audio.get_raw_data(), np.int16).flatten().astype(np.float32) / 32768.0)
-                    audio_data = torch_audio
-                
-                self.audio_queue.put_nowait(audio_data)
-                i += 1
+
+    def setup_mic(self):
+        self.source = sr.Microphone(sample_rate=16000)
+
+        self.recorder = sr.Recognizer()
+        self.recorder.energy_threshold = self.energy
+        self.recorder.pause_threshold = self.pause
+        self.recorder.dynamic_energy_threshold = self.dynamic_energy
+
+        with self.source:
+            self.recorder.adjust_for_ambient_noise(self.source)
+
+        self.recorder.listen_in_background(self.source, self.record_callback, phrase_time_limit=2)
+        self.logger.info("Mic setup complete, you can now talk")
 
 
+    def preprocess(self, data):
+        return torch.from_numpy(np.frombuffer(data, np.int16).flatten().astype(np.float32) / 32768.0)
+    
+    def get_all_audio(self,min_time=-1):
+        audio = bytes()
+        got_audio = False
+        time_start = time.time()
+        while not got_audio or time.time() - time_start < min_time:
+            while not self.audio_queue.empty():
+                audio += self.audio_queue.get()
+                got_audio = True
+
+        data = sr.AudioData(audio,16000,2)
+        data = data.get_raw_data()
+        return data
+
+
+    def record_callback(self,_, audio:sr.AudioData) -> None:
+        data = audio.get_raw_data()
+        self.audio_queue.put_nowait(data)
+
 
     def transcribe_forever(self):
         while True:
             if self.break_threads:
                 break
             self.transcribe()
 
 
-    def transcribe(self,data=None):
+    def transcribe(self,data=None,realtime=False):
         if data is None:
-            audio_data = self.audio_queue.get()
+            # audio_data = self.audio_queue.get()
+            audio_data = self.get_all_audio()
         else:
             audio_data = data
+        audio_data = self.preprocess(audio_data)
         if self.english:
             result = self.audio_model.transcribe(audio_data,language='english')
         else:
             result = self.audio_model.transcribe(audio_data)
 
+        predicted_text = result["text"]
         if not self.verbose:
-            predicted_text = result["text"]
-            self.result_queue.put_nowait(predicted_text)
+            if predicted_text not in self.banned_results:
+                self.result_queue.put_nowait(predicted_text)
         else:
-            self.result_queue.put_nowait(result)
+            if predicted_text not in self.banned_results:
+                self.result_queue.put_nowait(result)
 
         if self.save_file:
             os.remove(audio_data)
 
 
     def listen_loop(self):
         threading.Thread(target=self.transcribe_forever).start()
         while True:
-            print(self.result_queue.get())
+            result = self.result_queue.get()
+            print(result)
+                
 
-    def listen(self):
-        audio_data = self.audio_queue.get()
+    def listen(self,timout=3):
+        audio_data = self.get_all_audio(timout)
         self.transcribe(data=audio_data)
         while True:
             if not self.result_queue.empty():
                 return self.result_queue.get()
             
     def toggle_microphone(self):
         #TO DO: make this work
```

### Comparing `whisper_mic-1.0.1/whisper_mic.egg-info/PKG-INFO` & `whisper_mic-1.1.0/whisper_mic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-mic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

