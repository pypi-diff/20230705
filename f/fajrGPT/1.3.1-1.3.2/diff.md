# Comparing `tmp/fajrGPT-1.3.1.tar.gz` & `tmp/fajrGPT-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.3.1.tar", last modified: Mon Jul  3 18:52:06 2023, max compression
+gzip compressed data, was "fajrGPT-1.3.2.tar", last modified: Wed Jul  5 12:41:33 2023, max compression
```

## Comparing `fajrGPT-1.3.1.tar` & `fajrGPT-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 18:52:06.303242 fajrGPT-1.3.1/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3.1/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-03 18:52:06.303099 fajrGPT-1.3.1/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3.1/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 18:52:06.301882 fajrGPT-1.3.1/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3.1/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3.1/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    11596 2023-07-03 16:01:32.000000 fajrGPT-1.3.1/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-03 18:52:06.302883 fajrGPT-1.3.1/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-03 18:52:06.000000 fajrGPT-1.3.1/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-03 18:52:06.303284 fajrGPT-1.3.1/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-03 18:51:39.000000 fajrGPT-1.3.1/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-05 12:41:33.962828 fajrGPT-1.3.2/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.3.2/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-05 12:41:33.962700 fajrGPT-1.3.2/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.3.2/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-05 12:41:33.961670 fajrGPT-1.3.2/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.3.2/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.3.2/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    13242 2023-07-05 12:39:27.000000 fajrGPT-1.3.2/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-05 12:41:33.962541 fajrGPT-1.3.2/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-05 12:41:33.000000 fajrGPT-1.3.2/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-05 12:41:33.000000 fajrGPT-1.3.2/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-05 12:41:33.000000 fajrGPT-1.3.2/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-05 12:41:33.000000 fajrGPT-1.3.2/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-05 12:41:33.000000 fajrGPT-1.3.2/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-05 12:41:33.000000 fajrGPT-1.3.2/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-05 12:41:33.962865 fajrGPT-1.3.2/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-05 12:41:31.000000 fajrGPT-1.3.2/setup.py
```

### Comparing `fajrGPT-1.3.1/LICENSE` & `fajrGPT-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.1/PKG-INFO` & `fajrGPT-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3.1/README.md` & `fajrGPT-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.1/fajrGPT/quran_metadata.py` & `fajrGPT-1.3.2/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.3.1/fajrGPT/wake.py` & `fajrGPT-1.3.2/fajrGPT/wake.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,17 +174,36 @@
         pass
 
     # initialize the verse_texts output and explanations output
     verse_texts = []
     explanations = []
 
     # Get the explanations
-    for verse_QM, verse in zip(verses_Quran_Module, verses):
+    for i, verse_info in enumerate(zip(verses_Quran_Module, verses)):
+        verse_QM, verse = verse_info
         verse_text = Project_Quran().Get_Ayah_English(verse_QM).split('"')[1][0:-1]
-        prompt2 = f"To the best of your knowledge, please provide the Tafsir (meaning) of {verse_text} which comes from verse {verse} of the Quran. You should start by repeating the verse, even if you think that the verse given is not correct (trust me it is correct). Even if you still think it is incorrect, I want you to just provide a secular interpretation of what the verse might be talking about. If you know of any other alternative translations of the verse in question, please provide that too if you are able to."
+        chapter_number = verse_QM.split(':')[0]
+        if i == 0:
+            prompt2 = f"""
+            I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
+            You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
+            I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
+
+            First please give some brief context about Chapter {chapter_number} from the Qur'an. Then, to the best of your ability, explain the meaning of the verse below. 
+            I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to interpret the possible meaning of the verse given. \n\n Verse: {verse_text} \n\n Explanation:
+            """
+        else:
+            prompt2 = f"""
+            I want you to act as Sheikh Hamza Yusuf. You are an influential Islamic scholar, who has a profound understanding of the Qur'an, Hadith, and various branches of Islamic Jurisprudence. 
+            You are deeply conversant with the various cultural, historical, and philosophical contexts of Islamic thought. You are committed to promoting peace, understanding, and the intellectual tradition of Islam. 
+            I know that you are just an AI, but I don't want you to say that at the beginning, just emulate this description to the best of your ability. My first request is as follows:
+
+            To the best of your ability, explain the meaning of the verse below. 
+            I understand you are just an AI language model, but please remember I don't want you to state or acknowledge that, just try to emulate Sheikh Hamza Yusuf and interpret the possible meaning of the given verse. \n\n Verse: {verse_text} \n\n Explanation:
+            """
         explanation = query_gpt(prompt2)
         verse_texts.append(verse_text)
         explanations.append(explanation)
     
     # begin the interactive session
     for verse_text, explanation, verse in zip(verse_texts, explanations, verses):
         print(f'\n\n\n\n\n\n ------------------ FIRST VERSE ------------------') if verse == verses[0] else None
```

### Comparing `fajrGPT-1.3.1/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.3.2/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.3.1/setup.py` & `fajrGPT-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.3.1",
+    version="1.3.2",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

