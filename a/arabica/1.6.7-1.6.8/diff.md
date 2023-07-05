# Comparing `tmp/arabica-1.6.7.tar.gz` & `tmp/arabica-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.7.tar", last modified: Thu Jun 29 22:45:36 2023, max compression
+gzip compressed data, was "arabica-1.6.8.tar", last modified: Wed Jul  5 10:35:55 2023, max compression
```

## Comparing `arabica-1.6.7.tar` & `arabica-1.6.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:45:36.838075 arabica-1.6.7/
--rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.7/LICENSE
--rw-rw-rw-   0        0        0     7815 2023-06-29 22:45:36.838075 arabica-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     7012 2023-06-29 22:20:39.000000 arabica-1.6.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 22:45:36.838075 arabica-1.6.7/arabica/
--rw-rw-rw-   0        0        0      105 2023-06-29 22:43:08.000000 arabica-1.6.7/arabica/__init__.py
--rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.7/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.7/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.7/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.7/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.7/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.7/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.7/arabica/preprocess.py
--rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.7/arabica/sentiment.py
--rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.7/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:45:36.838075 arabica-1.6.7/arabica.egg-info/
--rw-rw-rw-   0        0        0     7815 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 22:45:36.000000 arabica-1.6.7/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-06-29 22:44:49.000000 arabica-1.6.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 22:45:36.838075 arabica-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-29 22:44:49.000000 arabica-1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:55.961370 arabica-1.6.8/
+-rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.8/LICENSE
+-rw-rw-rw-   0        0        0     7819 2023-07-05 10:35:55.961370 arabica-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7012 2023-07-05 10:30:26.000000 arabica-1.6.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:55.961370 arabica-1.6.8/arabica/
+-rw-rw-rw-   0        0        0      105 2023-06-29 22:43:08.000000 arabica-1.6.8/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.8/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.8/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.8/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.8/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.8/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.8/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.8/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.8/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.8/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:55.961370 arabica-1.6.8/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7819 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-07-05 10:33:39.000000 arabica-1.6.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:35:55.961370 arabica-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-07-05 10:33:39.000000 arabica-1.6.8/setup.py
```

### Comparing `arabica-1.6.7/PKG-INFO` & `arabica-1.6.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.7
+Version: 1.6.8
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arabica
@@ -97,14 +97,15 @@
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for common stop words
                skip: [] ,                # Remove additional list of stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
+)
 ```
 
 **coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
 * **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
 * **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
@@ -135,13 +136,13 @@
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
 * Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
-* **Meta-data description:** TBA
-* **Twitter tweets analysis:** TBA
+* **Twitter tweets analysis**
+* **Journal meta-data description**
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.6.7/README.md` & `arabica-1.6.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for common stop words
                skip: [] ,                # Remove additional list of stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
+)
 ```
 
 **coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
 * **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
 * **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
@@ -118,13 +119,13 @@
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
 * Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
-* **Meta-data description:** TBA
-* **Twitter tweets analysis:** TBA
+* **Twitter tweets analysis**
+* **Journal meta-data description**
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.6.7/arabica/arabica_freq.py` & `arabica-1.6.8/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica/cappuccino.py` & `arabica-1.6.8/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica/clean_ngram.py` & `arabica-1.6.8/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica/coffee_break.py` & `arabica-1.6.8/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica/group.py` & `arabica-1.6.8/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica/preprocess.py` & `arabica-1.6.8/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica/sentiment.py` & `arabica-1.6.8/arabica/sentiment.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.7/arabica.egg-info/PKG-INFO` & `arabica-1.6.8/arabica.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.7
+Version: 1.6.8
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arabica
@@ -97,14 +97,15 @@
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
                stopwords: [],            # Languages for common stop words
                skip: [] ,                # Remove additional list of stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
+)
 ```
 
 **coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
 * **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
 
 * **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
@@ -135,13 +136,13 @@
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
 * Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
-* **Meta-data description:** TBA
-* **Twitter tweets analysis:** TBA
+* **Twitter tweets analysis**
+* **Journal meta-data description**
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.6.7/pyproject.toml` & `arabica-1.6.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 
 [project]
 name = "arabica"
-version = "1.6.7"
+version = "1.6.8"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">3.9, <3.11"
 
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/PetrKorab/Arabica"
-"Bug Tracker" = "https://github.com/PetrKorab/Arabica/issues"
-
-
+"Bug Tracker" = "https://github.com/PetrKorab/Arabica/issues"
```

### Comparing `arabica-1.6.7/setup.py` & `arabica-1.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.7",
+        version="1.6.8",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

