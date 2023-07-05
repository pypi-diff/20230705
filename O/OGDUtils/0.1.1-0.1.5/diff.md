# Comparing `tmp/OGDUtils-0.1.1.tar.gz` & `tmp/OGDUtils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OGDUtils-0.1.1.tar", last modified: Tue Jul  4 14:31:00 2023, max compression
+gzip compressed data, was "OGDUtils-0.1.5.tar", last modified: Wed Jul  5 18:20:54 2023, max compression
```

## Comparing `OGDUtils-0.1.1.tar` & `OGDUtils-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/
--rw-rw-rw-   0        0        0     1117 2022-06-09 19:09:23.000000 OGDUtils-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1434 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      824 2023-06-30 19:27:15.000000 OGDUtils-0.1.1/README.md
--rw-rw-rw-   0        0        0      697 2023-07-04 14:30:14.000000 OGDUtils-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.949756 OGDUtils-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.960530 OGDUtils-0.1.1/src/OGDUtils/
-drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.982488 OGDUtils-0.1.1/src/OGDUtils/JOWILDER/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:36.000000 OGDUtils-0.1.1/src/OGDUtils/JOWILDER/__init__.py
--rw-rw-rw-   0        0        0    38315 2023-06-30 18:01:34.000000 OGDUtils-0.1.1/src/OGDUtils/JOWILDER/jowilder_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.987990 OGDUtils-0.1.1/src/OGDUtils/LAKELAND/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:44.000000 OGDUtils-0.1.1/src/OGDUtils/LAKELAND/__init__.py
--rw-rw-rw-   0        0        0     8530 2023-06-30 18:01:31.000000 OGDUtils-0.1.1/src/OGDUtils/LAKELAND/lakeland_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.995861 OGDUtils-0.1.1/src/OGDUtils/WAVES/
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:50.000000 OGDUtils-0.1.1/src/OGDUtils/WAVES/__init__.py
--rw-rw-rw-   0        0        0     3758 2023-06-30 18:01:22.000000 OGDUtils-0.1.1/src/OGDUtils/WAVES/waves_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:31:00.031884 OGDUtils-0.1.1/src/OGDUtils/general/
--rw-rw-rw-   0        0        0     1240 2023-06-30 17:47:12.000000 OGDUtils-0.1.1/src/OGDUtils/general/FeatureSetOptions.py
--rw-rw-rw-   0        0        0    21204 2023-07-03 20:47:05.000000 OGDUtils-0.1.1/src/OGDUtils/general/Workflow.py
--rw-rw-rw-   0        0        0        0 2023-06-30 18:02:29.000000 OGDUtils-0.1.1/src/OGDUtils/general/__init__.py
--rw-rw-rw-   0        0        0    25380 2023-06-30 20:25:30.000000 OGDUtils-0.1.1/src/OGDUtils/general/feature_utils.py
--rw-rw-rw-   0        0        0     3065 2023-06-30 20:25:43.000000 OGDUtils-0.1.1/src/OGDUtils/general/import_utils.py
--rw-rw-rw-   0        0        0     4343 2023-06-30 17:47:12.000000 OGDUtils-0.1.1/src/OGDUtils/general/ogd_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:30:59.974300 OGDUtils-0.1.1/src/OGDUtils.egg-info/
--rw-rw-rw-   0        0        0     1434 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 14:30:59.000000 OGDUtils-0.1.1/src/OGDUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.688113 OGDUtils-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.688113 OGDUtils-0.1.5/src/OGDUtils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/src/OGDUtils/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/JOWILDER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37301 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/JOWILDER/jowilder_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/src/OGDUtils/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/LAKELAND/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/LAKELAND/lakeland_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/src/OGDUtils/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/WAVES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/WAVES/waves_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/src/OGDUtils/general/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/general/FeatureSetOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/general/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24764 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/general/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/general/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-05 18:20:14.000000 OGDUtils-0.1.5/src/OGDUtils/general/ogd_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:20:54.692113 OGDUtils-0.1.5/src/OGDUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-05 18:20:54.000000 OGDUtils-0.1.5/src/OGDUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-05 18:20:54.000000 OGDUtils-0.1.5/src/OGDUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:20:54.000000 OGDUtils-0.1.5/src/OGDUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 18:20:54.000000 OGDUtils-0.1.5/src/OGDUtils.egg-info/top_level.txt
```

### Comparing `OGDUtils-0.1.1/LICENSE` & `OGDUtils-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 University of Wisconsin - Field Day Lab
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 University of Wisconsin - Field Day Lab
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `OGDUtils-0.1.1/README.md` & `OGDUtils-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# OGDUtils
-
-This project contains several utilities developed to ease the process of working with data from the OpenGameData core.
-There are a set of `general` utilities, which include importing of files into a standard pandas environment, and some basic organization of large datasets.
-In addition, some games have specific utility packages, typically developed as part of existing analysis projects.
-These projects are typically made available in the `opengamedata-samples` repository.
-
-**Warning:** Outside the import utilities, this package has very little active support.
-We make no guarantees anything else in the package works or is of practical use;
+# OGDUtils
+
+This project contains several utilities developed to ease the process of working with data from the OpenGameData core.
+There are a set of `general` utilities, which include importing of files into a standard pandas environment, and some basic organization of large datasets.
+In addition, some games have specific utility packages, typically developed as part of existing analysis projects.
+These projects are typically made available in the `opengamedata-samples` repository.
+
+**Warning:** Outside the import utilities, this package has very little active support.
+We make no guarantees anything else in the package works or is of practical use;
 most of the utilities included here are just to increase the odds of success for anyone trying to work with older analysis files from `opengamedata-samples`.
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/JOWILDER/jowilder_utils.py` & `OGDUtils-0.1.5/src/OGDUtils/JOWILDER/jowilder_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1014 +1,1014 @@
-# google imports
-
-# standard library imports
-import sys
-import copy
-import pickle
-import os
-from collections import Counter
-from io import BytesIO
-from zipfile import ZipFile
-import copy
-import pickle
-from math import ceil
-import importlib
-import urllib.request
-
-# math imports
-from matplotlib import pyplot as plt
-import numpy as np
-import pandas as pd
-from scipy import stats
-import seaborn as sns
-sns.set()
-
-# Jupyter Imports
-from IPython.display import display
-import ipywidgets as widgets
-# from google.colab import files
-
-# ML imports
-# models
-from sklearn.naive_bayes import CategoricalNB
-from sklearn.tree import ExtraTreeClassifier, DecisionTreeClassifier
-from sklearn.neural_network import MLPClassifier
-from xgboost import XGBClassifier
-from sklearn.linear_model import RidgeCV, SGDRegressor
-from sklearn.svm import LinearSVR
-
-
-# preprocessing
-from sklearn.impute import SimpleImputer
-from sklearn.compose import ColumnTransformer
-from sklearn.preprocessing import StandardScaler, OneHotEncoder, KBinsDiscretizer
-from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
-from sklearn.model_selection import train_test_split
-
-# sampling
-from imblearn.over_sampling import RandomOverSampler
-from imblearn.under_sampling import RandomUnderSampler, EditedNearestNeighbours, RepeatedEditedNearestNeighbours
-from imblearn.combine import SMOTEENN, SMOTETomek
-
-# metrics
-from sklearn.metrics import confusion_matrix, classification_report
-from sklearn.metrics import plot_precision_recall_curve, plot_confusion_matrix, plot_roc_curve
-from sklearn.metrics import f1_score, roc_auc_score, roc_curve, accuracy_score
-
-# other
-from imblearn.pipeline import make_pipeline
-from sklearn.model_selection import GridSearchCV
-
-# custom imports
-import feature_utils as feat_util
-
-
-def response_boxplot(df, category, verbose=False):
-    print('\n'+category)
-    fig, axs = plt.subplots(1, 3, figsize=(20, 10))
-    qs = ['EFL_yes_no', 'skill_low_med_high', 'enjoy_high_med_low_none']
-    for i, f in enumerate(['R0_quiz_response', 'R1_quiz_response', 'R2_quiz_response', ]):
-        if verbose:
-            print(qs[i])
-        bp = df.boxplot(column=category, by=df[f].astype(
-            'category'), ax=axs[i])
-        bp.set_xlabel('')
-        for choice in range(df[f].min(), df[f].max()+1):
-            query = f"{f}=={choice}"
-            cat_df = df.query(query)[category]
-            num_chose = len(cat_df)
-            mean = cat_df.mean()
-            std = cat_df.std()
-            if verbose:
-                print(
-                    f'{f} # chose {choice}: {num_chose} ({round(num_chose/len(df)*100)}%). Avg {mean}, std {std}.')
-    plt.suptitle(f'{category} Boxplot')
-    fig.show()
-
-
-def group_by_func(df, func, title='', show=True):
-    r0_groups = {0: 'native', 1: 'nonnative'}
-    r1_groups = {0: 'not very good skill',
-                 1: 'okay skill', 2: 'very good skill'}
-    r2_groups = {0: 'really enjoy', 1: 'enjoy', 2: 'okay', 3: 'not enjoy'}
-    def group_string(r0, r1, r2): return ', '.join(
-        [r0_groups[r0], r1_groups[r1], r2_groups[r2]])
-    result_dfs = [pd.DataFrame(index=r1_groups.values(), columns=r2_groups.values(
-    )), pd.DataFrame(index=r1_groups.values(), columns=r2_groups.values())]
-    if show:
-        print(f'{"-"*6}  {title}  {"-"*6}')
-    for r0 in [0, 1]:
-        subtitle = "Nonnatives" if r0 else "Natives"
-        if show:
-            print(f'\n{subtitle}:')
-        tdf0 = df.query(f"R0_quiz_response == {r0}")
-        for r1 in [0, 1, 2]:
-            tdf1 = tdf0.query(f"R1_quiz_response == {r1}")
-            for r2 in [0, 1, 2, 3]:
-                tdf2 = tdf1.query(f"R2_quiz_response == {r2}")
-                result_dfs[r0].loc[r1_groups[r1], r2_groups[r2]
-                                   ] = func(df, tdf0, tdf1, tdf2)
-        if show:
-            display(result_dfs[r0])
-    return result_dfs
-
-
-def standard_group_by_func(fulldf, per_category_stats_list=None):
-    per_category_stats_list = None or ['sess_count_clicks',
-                                       'sess_count_hovers',
-                                       'sess_meaningful_action_count',
-                                       'sess_EventCount',
-                                       'sess_count_notebook_uses',
-                                       'sess_avg_time_between_clicks',
-                                       'sess_first_enc_words_read',
-                                       'sess_first_enc_boxes_read',
-                                       'sess_num_enc',
-                                       'sess_first_enc_duration',
-                                       'sess_first_enc_avg_wps',
-                                       'sess_first_enc_var_wps',
-                                       'sess_first_enc_avg_tbps',
-                                       'sess_first_enc_var_tbps',
-                                       'sess_start_obj',
-                                       'sess_end_obj',
-                                       'start_level',
-                                       'max_level',
-                                       'sessDuration']
-    dfs_list = []
-    title_list = []
-
-    def df_func(df, tdf0, tdf1, tdf2): return len(tdf2)
-    title = 'count'
-    dfs = group_by_func(fulldf, df_func, title)
-    dfs_list.append(dfs)
-    title_list.append(title)
-
-    def df_func(df, tdf0, tdf1, tdf2): return round(len(tdf2)/len(df)*100, 2)
-    title = 'percent total pop'
-    dfs = group_by_func(fulldf, df_func, title)
-    dfs_list.append(dfs)
-    title_list.append(title)
-
-    def df_func(df, tdf0, tdf1, tdf2): return round(len(tdf2)/len(tdf0)*100, 2)
-    title = 'percent native class pop'
-    dfs = group_by_func(fulldf, df_func, title)
-    dfs_list.append(dfs)
-    title_list.append(title)
-
-    for category in per_category_stats_list:
-        df_func = get_avg_std_df_func(category)
-        title = f'(avg, std) {category}'
-        dfs = group_by_func(fulldf, df_func, title)
-        dfs_list.append(dfs)
-        title_list.append(title)
-    return title_list, dfs_list
-
-
-def get_avg_std_df_func(category_name):
-    def inner(df, tdf0, tdf1, tdf2):
-        mean = tdf2[category_name].mean()
-        std = tdf2[category_name].std()
-        if not pd.isna(mean):
-            mean = round(mean, 2)
-        if not pd.isna(std):
-            std = round(std, 2)
-        return (mean, std)
-    return inner
-
-
-def html_stats(df):
-    html_strs = ['<div class="container">', '<h3>{Stats}</h3>']
-    qs = ['EFL_yes_no', 'skill_low_med_high', 'enjoy_high_med_low_none']
-    html_strs.append(f'<p> Total pop {len(df)} </p>')
-    for i, f in enumerate(['R0_quiz_response', 'R1_quiz_response', 'R2_quiz_response', ]):
-        html_strs.append(f'<p> {qs[i]}</p>')
-        for choice in range(df[f].min(), df[f].max()+1):
-            query = f"{f}=={choice}"
-            cat_df = df.query(query)
-            num_chose = len(cat_df)
-            html_strs.append(
-                f'<p>{f} # chose {choice}: {num_chose} ({round(num_chose/len(df)*100)}%).</p>')
-    return '\n'.join(html_strs+['</div>'])
-
-
-def full_html(base_df, title_list, dfs_list, suptitle=None):
-    HEADER = '''<!DOCTYPE html>
-<html lang="en">
-
-<head>
-  <meta charset="UTF-8">
-  <meta name="viewport" content="width=device-width, initial-scale=1.0">
-  <title>Document</title>
-</head>
-
-<body>
-  <style>
-    .flex-container {
-      display: flex;
-      flex-wrap: wrap;
-    }
-
-    .container {
-      border: thick solid black;
-      padding: 10px;
-      margin: 5px;
-    }
-
-    .container table:nth-of-type(2) td {
-      background-color: rgb(161, 161, 230);
-    }
-
-    .container table:nth-of-type(2) th {
-      background-color: rgb(20, 20, 194);
-      color: white;
-    }
-
-    .container table:nth-of-type(2n-1) td {
-      background-color: rgb(235, 158, 158);
-    }
-
-    .container table:nth-of-type(2n-1) th {
-      background-color: rgb(160, 11, 11);
-      color: white;
-    }
-    .break {
-  flex-basis: 100%;
-  height: 0;
-}
-  </style>
-  <div class="flex-container">'''
-    FOOTER = '''  </div>
-    </body>
-
-    </html>'''
-
-    def table_header(title): return f'''    <div class="container">
-        <h3>{title}</h3>'''
-    table_footer = '''    </div>'''
-    def table_html(title, dfs): return '\n'.join([table_header(
-        title), "<p>Natives:</p>", dfs[0].to_html(), "<p>Nonnatives:</p>", dfs[1].to_html(), table_footer])
-
-    if suptitle is not None:
-        suptitle = f'<h2>{suptitle}</h2>\n<div class="break"></div> <!-- break -->'
-    else:
-        suptitle = ''
-    return '\n'.join([HEADER, suptitle, html_stats(base_df)] +
-                     [table_html(t, dfs) for t, dfs in zip(title_list, dfs_list)] +
-                     [FOOTER])
-
-
-def download_full_html(base_df, title_list, dfs_list, filename, suptitle=None):
-    with open(filename, 'w+') as f:
-        f.write(full_html(base_df, title_list, dfs_list, suptitle=suptitle))
-        print("Wrote to", filename)
-    files.download(filename)
-
-
-onext_int_feats = [f'obj{i}_onext_int' for i in range(80)]
-onext_int_cats = [["nan", 1],
-                  ["nan", 11],
-                  ["nan", 12, 86, 111, 125],
-                  ["nan", 13, 14, 113, 116, 118],
-                  ["nan", 14, 15, 113, 114, 116, 118],
-                  ["nan", 13, 15, 113, 114, 116, 118],
-                  ["nan", 16, 86, 115, 118, 132, 161],
-                  ["nan", 17, 86, 115, 118, 128, 161],
-                  ["nan", 18, 86, 115, 118, 161],
-                  ["nan", 19, 86, 117, 118, 127, 133, 134, 161],
-                  ["nan", 20, 133, 134, 136],
-                  ["nan", 2, 80, 81, 82, 83],
-                  ["nan", 21, 86, 117, 127, 136, 137, 161],
-                  ["nan", 22, 137, 141],
-                  ["nan", 23, 24, 86, 117, 127, 136, 161],
-                  ["nan", 23, 24, 117, 127, 136, 161],
-                  ["nan", 25, 86, 117, 118, 127, 136, 140, 147, 151, 161],
-                  ["nan", 26, 142, 145],
-                  ["nan", 27, 143],
-                  ["nan", 28, 86, 117, 118, 136, 140, 150, 161],
-                  ["nan", 29, 119, 130],
-                  ["nan", 29, 30, 35, 86, 117, 118, 126, 136, 140, 149],
-                  ["nan", 3, 80, 82, 83, 86, 87, 88, 93],
-                  ["nan", 31, 38],
-                  ["nan", 32, 153],
-                  ["nan", 33, 154],
-                  ["nan", 34, 155],
-                  ["nan", 35, 156],
-                  ["nan", 36, 157],
-                  ["nan", 37, 158],
-                  ["nan", 30],
-                  ["nan", 39, 163],
-                  ["nan", 40, 160],
-                  ["nan", 3],
-                  ["nan", 41, 164, 166],
-                  ["nan", 42, 166],
-                  ["nan", 30],
-                  ["nan", 44, 85, 125],
-                  ["nan", 29, 45, 47, 84, 118, 125, 136, 140, 149, 168, 169, 184],
-                  ["nan", 45, 46, 169, 170],
-                  ["nan", 29, 45, 47, 92, 118, 136, 140, 149, 169, 184],
-                  ["nan", 29, 45, 48, 92, 118, 140, 149, 168, 184],
-                  ["nan", 46, 49, 168],
-                  ["nan", 46, 50, 168, 170],
-                  ["nan", 5, 80, 82, 83, 86, 89, 91, 95, 97, 125],
-                  ["nan", 29, 51, 92, 118, 136, 140, 149, 168, 184],
-                  ["nan", 52, 92, 118, 136, 149, 171, 184],
-                  ["nan", 53, 54, 92, 118, 136, 140, 149, 184],
-                  ["nan", 53, 54, 55, 59, 60, 90, 92, 94,
-                      118, 136, 140, 149, 168, 184],
-                  ["nan", 53, 55, 59, 60, 90, 92, 94, 118, 136, 140, 149, 184],
-                  ["nan", 55, 56, 59, 60, 149, 174],
-                  ["nan", 57, 59, 60, 174],
-                  ["nan", 58, 59, 60, 136, 172, 174, 184],
-                  ["nan", 29, 59, 60, 61, 92, 118, 136, 149, 168, 172, 184],
-                  ["nan", 55, 56, 57, 58, 60, 61, 140, 172, 174, 184],
-                  ["nan", 6, 80, 82, 83, 86, 98, 100, 125],
-                  ["nan", 55, 56, 57, 58, 59, 61, 92, 118,
-                      136, 140, 149, 172, 174, 184],
-                  ["nan", 59, 62, 136, 140, 149, 172, 173, 175, 184],
-                  ["nan", 63, 64, 176],
-                  ["nan", 64, 66, 149, 175, 184],
-                  ["nan", 29, 65, 66, 92, 118, 136, 140, 172, 175, 177, 184],
-                  ["nan", 66, 67, 68, 92, 118, 136, 140, 146, 175, 177, 184],
-                  ["nan", 67, 144],
-                  ["nan", 29, 64, 65, 68, 92, 118, 131, 136,
-                      140, 148, 149, 172, 175, 177, 184],
-                  ["nan", 92, 118, 122, 123, 124, 131, 136, 140,
-                      146, 148, 168, 172, 175, 177, 184],
-                  ["nan", 70],
-                  ["nan", 7],
-                  ["nan", 71, 178],
-                  ["nan", 72, 179],
-                  ["nan", 73, 180],
-                  ["nan", 74, 181],
-                  ["nan", 75, 182],
-                  ["nan", 69],
-                  ["nan", 77, 78, 185],
-                  ["nan", 78, 185],
-                  ["nan", 79],
-                  [0],
-                  ["nan", 8],
-                  ["nan", 9, 103],
-                  ["nan", 104, 105, 108]]
-
-QA_1_feats = [f'Q{i}_A1' for i in range(19)]
-QA_1_cats = [['0', 'A', 'B', 'C', 'D'],
-             ['0', 'A', 'B', 'C', 'D'],
-             ['0', 'A', 'B', 'C', 'D'],
-             ['0', 'A', 'B', 'C', 'D'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', '?', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
-              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
-             ['0', 'A', 'B', 'C', 'D', 'F', 'G', 'I', 'M', 'N', 'O', 'P', 'Q',
-              'R', 'S', 'V', 'W', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f'],
-             ['0', 'Q', 'V', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f'],
-             ['0', '?', 'X', 'Y', 'Z', 'b', 'c', 'd', 'e', 'f'],
-             ['0', 'X', 'Y', 'b', 'c', 'd', 'e', 'f'],
-             ['0', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f']]
-
-
-def get_preprocessor(df, scaler=StandardScaler(), imputer=SimpleImputer(strategy='constant'), bool_dtype='int64'):
-    """
-    By default has a number of steps:
-    1. drops columns from use in preprocessor if present:
-       - [f'Q{q}_answers' for q in range(19)]
-       - ["play_year", "play_month", "play_day", "play_hour", "play_minute", "play_second"]
-       - ["_continue", "continue", "save_code", "music", "hq", "fullscreen", "persistentSessionID"]
-    2. Creates a preprocessor for all non-y columns and non-boolean columns with the following steps:
-       a. Standard Scaler (0 mean, 1 std)
-       b. Simple Imputer(strategy='constant') (fill NaN with 0)
-    3. Fits the preprocessor to the given X
-    4. returns the unfitted preprocessor (sklearn pipeline), and the unprocessed X dataframe
-    :param df: jowilder dataframe
-    :param scaler: sklearn compatible scaler
-    :param imputer: sklearn compatible imputer
-    :return: the unfitted preprocessor (sklearn pipeline), and the unprocessed X dataframe
-    """
-    df = df.drop(
-        [f'Q{q}_answers' for q in range(19)] + ["play_year", "play_month", "play_day", "play_hour", "play_minute",
-                                                "play_second",
-                                                "_continue", "continue", "save_code", "music", "hq", "fullscreen",
-                                                "persistentSessionID", ], axis=1, errors='ignore').copy()
-    y_cols, bool_cols, num_cols = separate_columns(df, bool_dtype=bool_dtype)
-    X = df.loc[:, num_cols+bool_cols]
-
-    # too complicated to allow for pipeline order
-    # pipeline_strings = [pipeline_order[i:i+2] for i in range(0,len(pipeline_order),2)]
-    # transformers = []
-    # num_sa, num_sc, num_im = 0,0,0
-    # for s in pipeline_strings:
-    #     if s == 'Sa':
-    #         transformer = make_pipeline(sampler)
-    #         cols = num_cols + bool_cols
-    #         name = f'{s}{num_sa}'
-    #         num_sa += 1
-    #     elif s == 'Sc':
-    #         transformer = scaler
-    #         name = f'{s}{num_sc}'
-    #         cols = num_cols
-    #         num_sc += 1
-    #     elif s == 'Im':
-    #         transformer = imputer
-    #         name = f'{s}{num_im}'
-    #         cols = num_cols
-    #         num_im += 1
-    #     else:
-    #         raise ValueError("Pipeline substrings must be Sa Sc or Im")
-    #     transformers.append((name, transformer, cols))
-
-    def col_str_to_int(col_strs): return [
-        X.columns.get_loc(s) for s in col_strs]
-    column_transformer = ColumnTransformer(
-        transformers=[
-            ('num', make_pipeline(scaler, imputer), col_str_to_int(num_cols)),
-            ('bool', 'passthrough', col_str_to_int(bool_cols))
-        ],
-        remainder='drop')
-    return column_transformer, X
-
-
-def get_ys(df):
-    """
-
-    :rtype: dictionary of y columns (df series). keys: y0,y1,y2,y1_bin,y2_bin,y1_bin_x,y2_bin_x
-    """
-    ys = {}
-    for key, y_col in [
-        ('y0', 'R0_quiz_response'),
-        ('y1', 'R1_quiz_response'),
-        ('y2', 'R2_quiz_response'),
-        ('y1_bin', 'R1_quiz_response_bin'),
-        ('y1_bin_0v12', 'R1_quiz_response_0v12'),
-        ('y1_bin_01v2', 'R1_quiz_response_01v2'),
-        ('y1_bin_x', 'R1_quiz_response_bin_x'),
-        ('y2_bin', 'R2_quiz_response_bin'),
-        ('y2_bin_x', 'R2_quiz_response_bin_x'),
-        ('y2_bin_0v123', 'R2_quiz_response_bin0v123'),
-        ('y2_bin_01v23', 'R2_quiz_response_bin01v23'),
-        ('y2_bin_012v3', 'R2_quiz_response_bin012v3'),
-    ]:
-        if y_col in df.columns:
-            ys[key] = df.loc[:, y_col].astype('category').copy()
-    return ys
-
-
-def separate_columns(df, bool_dtype='int64', expect_bool_cols = True) -> (list, list, list):
-    """
-
-    :param df:
-    :param bool_dtype: Defaults to 'int64'. Should be int64 if coming from import csv otherwise could be 'uint8'
-    if coming from the pd dummies.
-    :return: tuple of lists of column names for y_columns, bool_columns, and integer_columns
-    """
-    y_cols = [col for col in df.columns if 'quiz_response' in col]
-    bool_cols = [col for col in df.select_dtypes(include=[bool_dtype])
-                 if np.isin(df[col].dropna().unique(), [0, 1]).all() and
-                 col not in y_cols]
-    num_cols = [
-        col for col in df.columns if col not in bool_cols and col not in y_cols]
-    if not bool_cols and expect_bool_cols:
-        print('Warning! No bool columns. Consider changing bool_dtype="int_64" to "uint8"')
-    return y_cols, bool_cols, num_cols
-
-
-end_obj_to_last_Q = {
-    9: 0,
-    10: 3,
-    11: 3,
-    12: 3,
-    13: 3,
-    14: 3,
-    15: 3,
-    16: 3,
-    17: 3,
-    18: 3,
-    19: 3,
-    20: 3,
-    21: 3,
-    22: 3,
-    23: 3,
-    24: 3,
-    25: 3,
-    26: 3,
-    27: 3,
-    28: 3,
-    29: 3,
-    30: 3,
-    31: 3,
-    32: 4,
-    33: 5,
-    34: 6,
-    35: 7,
-    36: 8,
-    37: 9,
-    38: 9,
-    39: 10,
-    40: 11,
-    41: 12,
-    42: 13,
-    43: 13,
-    44: 13,
-    45: 13,
-    46: 13,
-    47: 13,
-    48: 13,
-    49: 13,
-    50: 13,
-    51: 13,
-    52: 13,
-    53: 13,
-    54: 13,
-    55: 13,
-    56: 13,
-    57: 13,
-    58: 13,
-    59: 13,
-    60: 13,
-    61: 13,
-    62: 13,
-    63: 13,
-    64: 13,
-    65: 13,
-    66: 13,
-    67: 13,
-    68: 13,
-    69: 13,
-    70: 13,
-    71: 14,
-    72: 15,
-    73: 16,
-    74: 17,
-    75: 18,
-    76: 18,
-    77: 18,
-    78: 18,
-    79: 18,
-}
-
-end_obj_to_last_lvl = {
-    0:	0,
-    1:	0,
-    2:	0,
-    3:	1,
-    4:	2,
-    5:	2,
-    6:	3,
-    7:	3,
-    8:	4,
-    9: 4,
-    10: 4,
-    11: 4,
-    12: 5,
-    13: 6,
-    14: 6,
-    15: 6,
-    16: 6,
-    17: 6,
-    18: 6,
-    19: 7,
-    20: 7,
-    21: 8,
-    22: 8,
-    23: 9,
-    24: 9,
-    25: 9,
-    26: 10,
-    27: 10,
-    28: 11,
-    29: 11,
-    30: 12,
-    31: 12,
-    32: 12,
-    33: 12,
-    34: 12,
-    35: 12,
-    36: 12,
-    37: 12,
-    38: 12,
-    39: 12,
-    40: 12,
-    41: 12,
-    42: 12,
-    43: 13,
-    44: 13,
-    45: 14,
-    46: 15,
-    47: 15,
-    48: 16,
-    49: 16,
-    50: 17,
-    51: 17,
-    52: 18,
-    53: 18,
-    54: 18,
-    55: 18,
-    56: 18,
-    57: 18,
-    58: 18,
-    59: 18,
-    60: 18,
-    61: 18,
-    62: 19,
-    63: 19,
-    64: 19,
-    65: 20,
-    66: 20,
-    67: 21,
-    68: 21,
-    69: 22,
-    70: 22,
-    71: 22,
-    72: 22,
-    73: 22,
-    74: 22,
-    75: 22,
-    76: 22,
-    77: 23,
-    78: 23,
-    79: 23,
-}
-
-
-class GridSearcher():
-
-    def __init__(self, csv_fpath=None, df=None, preprocessor=None, fillna=0, meta=[], expect_bool_cols=True):
-        # either give csv_fpath or df.
-        assert csv_fpath or not df.empty
-        print(f'Loading from {csv_fpath}...')
-        # load df
-        if df is None:
-            print(f'Loading from {csv_fpath}...')
-            self.df, self.meta = feat_util.open_csv_from_path_with_meta(
-                csv_fpath, index_col=0)
-        else:
-            self.df, self.meta = df, meta
-
-        # set X and ys, and preprocessor
-        if not preprocessor:
-            self.preprocessor, self.X = get_preprocessor(self.df)
-            self.X = self.X.fillna(fillna)
-        else:
-            _, bool_cols, num_cols = separate_columns(self.df, expect_bool_cols=expect_bool_cols)
-            self.X = df[bool_cols+num_cols]
-            self.preprocessor = preprocessor
-        self.ys = get_ys(self.df)
-
-        # set object vars
-        self.model_dict = {}
-        self.cur_model = None
-
-    def split_data(self):
-        nonnull_X, nonnull_y = feat_util.remove_nan_labels(self.X, self.y)
-        X_train, X_test, y_train, y_test = train_test_split(
-            nonnull_X, nonnull_y, test_size=0.2, random_state=1)
-        self.X_train, self.X_test, self.y_train, self.y_test = X_train, X_test, y_train, y_test
-
-    def set_y(self, y_key=None, other_col=None):
-        if y_key:
-            print(f'Switching to {y_key}...')
-            self.y = self.ys[y_key]
-        elif other_col:
-            self.y = self.X[other_col]
-            self.X = self.X.drop(other_col, axis=1)
-        else:
-            print("Did not change y. Invalid inputs.")
-        self.split_data()
-
-    def run_fit(self, classifier, sampler=None, verbose=False, preprocess_twice=True, sampler_index=None, full_pipeline=False):
-        # fit self.cur_model as a pipeline of the given preprocessor, sampler, preprocessor, classifer
-        # if preprocess_twice is false, self.cur_model is sampler, preprocessor, classifier
-        # if full_pipeline and sampler index, self.cur_model is the classifier 
-        # (must be a pipeline containing a sampler or a placeholder (None) for the sampler)
-        if full_pipeline:
-            assert sampler_index is not None
-            clf = classifier
-        elif preprocess_twice:
-            clf = make_pipeline(self.preprocessor, sampler,
-                                copy.deepcopy(self.preprocessor), classifier)
-            sampler_index = 1
-        else:
-            clf = make_pipeline(sampler, self.preprocessor, classifier)
-            sampler_index = 0
-
-        self._sampling_pipeline = clf[:sampler_index+1]
-        self._classifying_pipeline = clf[sampler_index+1:]
-        if clf[sampler_index] is not None:
-            self.X_train_sampled, self.y_train_sampled = self._sampling_pipeline.fit_resample(
-                self.X_train, self.y_train)
-        else:
-            self.X_train_sampled, self.y_train_sampled = self.X_train, self.y_train
-            clf = self._classifying_pipeline
-
-        # model_name = f'{sampler} {classifier}'
-        # if verbose:
-        #     print(f'Running {model_name}.')
-        self._classifying_pipeline.fit(
-            self.X_train_sampled, self.y_train_sampled)
-        self.cur_model = clf
-        # if verbose:
-        #     print("model trained to: %.3f" %
-        #           clf.score(self.X_train, self.y_train))
-        #     print("model score: %.3f" % clf.score(self.X_test, self.y_test))
-        return clf
-
-    def metrics(self, graph_dir=None, graph_prefix=None, binary_classification=True):
-        # return list of (metric: float, metric_name: str) tuples of metrics of given classifier (default: self.cur_model)
-        # can only do metrics for binary classification as of right now
-        assert binary_classification
-        metric_list = []
-        clf = self.cur_model
-
-        # label metrics
-        if graph_prefix:
-            for flipped_labels in [False, True]:
-                flipped_labels_suffix = '' if not flipped_labels else '_flipped'
-                fig, axes = plt.subplots(3, 3, figsize=(20, 20))
-                for i, (yarray, Xarray, label) in enumerate([(self.y_test, self.X_test, 'test'),
-                                                             (self.y_train_sampled,
-                                                              self.X_train_sampled, 'train'),
-                                                             (self.y_train,
-                                                              self.X_train, 'train_raw'),
-                                                             ]):
-                    for j, (graph_type, func) in enumerate([
-                        ('', plot_confusion_matrix),
-                        ('_PR', plot_precision_recall_curve),
-                        ('_ROC', plot_roc_curve),
-                    ]):
-                        ax = axes[j, i]
-                        graph_yarray = yarray.astype(bool)
-                        if flipped_labels:
-                            graph_yarray = ~graph_yarray
-                        disp = func(clf, Xarray, graph_yarray, ax=ax)
-                        title = f'{label}{graph_type}{flipped_labels_suffix}'
-                        ax.set_title(title)
-                        if graph_type in ['_PR', '_ROC']:
-                            ax.set_xlim(-0.05, 1.05)
-                            ax.set_ylim(-0.05, 1.05)
-                            ax.set_aspect('equal', adjustable='box')
-                suptitle = f'{graph_prefix}{flipped_labels_suffix}'
-                plt.suptitle(suptitle)
-                savepath = os.path.join(graph_dir, f'{suptitle}.png')
-                fig.savefig(savepath, dpi=100)
-                plt.close()
-
-        for i, (yarray, Xarray, label) in enumerate([(self.y_test, self.X_test, 'test'),
-                                                     (self.y_train_sampled,
-                                                      self.X_train_sampled, 'train'),
-                                                     (self.y_train,
-                                                      self.X_train, 'train_raw'),
-                                                     ]):
-
-            y_pred = clf.predict(Xarray)
-            y_prob = clf.predict_proba(Xarray)[:, 1]
-            y_true = yarray
-            X_shape = Xarray.shape
-            metric_list.extend(feat_util.binary_metric_list(
-                y_true=y_true, y_pred=y_pred, y_prob=y_prob, X_shape=X_shape,
-                label_prefix=f'{label}_'
-            ))
-
-
-
-        return metric_list
-
-    def model_stats(self, classifier=None, graph=True):
-        # counter, auc, and optional graph of given classifer (default: self.cur_model)
-        classifier = classifier or self.cur_model
-        y_prob = classifier.predict_proba(self.X_test)[:, 1]
-        print(f"dimension y_prob: {y_prob.shape}")
-        print(f"dimension y_test: {self.y_test.shape}")
-        print(f'Predicts:', Counter(list(classifier.predict(self.X_test))))
-        print(f'True Labels:', Counter(self.y_test))
-        if graph:
-            fpr, tpr, thres = roc_curve(self.y_test, y_prob)
-            plt.plot(fpr, tpr, color='green')
-            plt.plot([0, 1], [0, 1], color='red', linestyle='--')
-            plt.show()
-        roc_auc = roc_auc_score(self.y_test, y_prob)
-        print(f"ROC-AUC Score: {roc_auc}")
-
-    def classification_report(self):
-        # classification report on current model
-        y_true = self.y_test
-        y_pred = self.cur_model.predict(self.X_test)
-        print(classification_report(y_true, y_pred))
-
-
-class JWWindowSelector:
-
-    ycols = ['R0_quiz_response','R1_quiz_response','R2_quiz_response','R1_quiz_response_bin',
-            'R1_quiz_response_0v12','R1_quiz_response_01v2','R1_quiz_response_bin_x',
-            'R2_quiz_response_bin','R2_quiz_response_bin_x','R2_quiz_response_bin0v123',
-            'R2_quiz_response_bin01v23','R2_quiz_response_bin012v3']
-    INTERACTION = 0
-    LEVEL = 1
-    QUIZ = 2
-    OBJECTIVE = 3
-
-    def __init__(self, csv_fpath=None, df=None, meta=None):
-        assert csv_fpath is not None or df is not None
-        # load df
-        if df is None:
-            print(f'Loading from {csv_fpath}...')
-            self.df, self.meta = feat_util.open_csv_from_path_with_meta(
-                csv_fpath, index_col=0)
-        else:
-            self.df = df
-            self.meta = meta or []
-
-        self.df_cols = list(df.columns)
-
-    @staticmethod
-    def get_abbrev(window_type):
-        if window_type == JWWindowSelector.INTERACTION:
-            return 'int'
-        if window_type == JWWindowSelector.LEVEL:
-            return 'lvl'
-        if window_type == JWWindowSelector.QUIZ:
-            return 'q'
-        if window_type == JWWindowSelector.OBJECTIVE:
-            return 'obj'
-
-    @staticmethod
-    def get_prefix(n, window_type):
-        if window_type == JWWindowSelector.INTERACTION:
-            return f'int{n}_i'
-        if window_type == JWWindowSelector.LEVEL:
-            return f'lvl{n}_'
-        if window_type == JWWindowSelector.QUIZ:
-            return f'Q{n}_'
-        if window_type == JWWindowSelector.OBJECTIVE:
-            return f'obj{n}_o'
-
-    @staticmethod
-    def get_window_range(window_type, skip_Q23=False):
-        if window_type == JWWindowSelector.INTERACTION:
-            return range(189)
-        if window_type == JWWindowSelector.LEVEL:
-            return range(24)
-        if window_type == JWWindowSelector.QUIZ:
-            if not skip_Q23:
-                return range(19)
-            else:
-                return [0,1,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18]
-        if window_type == JWWindowSelector.OBJECTIVE:
-            return range(80)
-
-
-    def cols_startwith(self, prefix):
-        return [c for c in self.df_cols if c.startswith(prefix)]
-    def get_feats(self, n, window_type):
-        prefix = self.get_prefix(n, window_type)
-        feats = self.cols_startwith(prefix)
-        return feats
-
-    def get_filter_queries(self, n, window_type, max_seconds_per_word=2):
-        prefix = JWWindowSelector.get_prefix(n, window_type)
-        queries = [f"R1_quiz_response == R1_quiz_response"]
-        if window_type in [JWWindowSelector.INTERACTION, JWWindowSelector.LEVEL]:
-            queries.extend([
-                        f"{prefix}first_enc_duration == {prefix}first_enc_duration",
-                        f"{prefix}first_enc_duration > 0",
-            ])
-        if window_type == JWWindowSelector.QUIZ:
-            queries.extend([
-                f'{prefix}A1_nan!=1'
-            ])
-        elif window_type == JWWindowSelector.INTERACTION:
-            num_words = self.df[f"int{n}_ifirst_enc_words_read"].max()
-            queries.extend([
-                    f"{prefix}first_enc_words_read == {num_words}",
-                    f"{prefix}time_to > 0",
-                    f"{prefix}first_enc_duration < {prefix}first_enc_words_read*{max_seconds_per_word}",
-                    ])
-        elif window_type == JWWindowSelector.OBJECTIVE:
-            if n < 79:
-                queries.append(f'obj{n}_onext_int_nan==0')
-                queries.append(f"obj{n}_otime_to_next_obj < 600")
-                queries.append(f"obj{n}_otime_to_next_obj > 0 ")
-
-        elif window_type == JWWindowSelector.LEVEL:
-            queries.append(f"{prefix}time_in_level < 1200")
-            queries.append(f"{prefix}time_in_level > 0")
-
-        queries.extend([f"R{i}_quiz_response == R{i}_quiz_response" for i in [0,1,2]])
-        return queries
-
-    def get_base_meta(self):
-        return self.meta
-    
-    @staticmethod
-    def join_XY(X,Y):
-        return X.join(Y)
-    
-    def get_X_Y_meta(self, n, window_type, max_seconds_per_word=2,nbins=0, drop_first_next_int_col = True):
-        meta = []
-        prefix = JWWindowSelector.get_prefix(n, window_type)
-        Xfeats = self.get_feats(n, window_type)
-        meta.append(f'Using feats: {Xfeats}')
-
-        if window_type==JWWindowSelector.INTERACTION:
-            total_words = self.df[f"int{n}_ifirst_enc_words_read"].max() 
-            if total_words is np.nan:
-                return None, None, meta
-            elif total_words < 10:
-                print('Total words < 10!')
-        queries = self.get_filter_queries(n, window_type, max_seconds_per_word=max_seconds_per_word)
-        filtered_df, filtered_df_meta = feat_util.filter_df(self.df[Xfeats+JWWindowSelector.ycols], query_list=queries, verbose=True, fillna=None)
-        meta.extend(filtered_df_meta)
-        X = filtered_df[Xfeats].fillna(0).copy()
-        meta.append(f'Filled X with 0')
-        Y = filtered_df[JWWindowSelector.ycols].copy()
-        drop_cols = []
-        if window_type in [JWWindowSelector.INTERACTION, JWWindowSelector.LEVEL]:
-            drop_cols = [
-                f"{prefix}first_enc_boxes_read",
-                f"{prefix}first_enc_words_read",
-            ]
-        if window_type==JWWindowSelector.INTERACTION:
-            drop_cols.extend([
-            f"{prefix}time_to",
-            f"{prefix}total_duration"
-            ])
-        if window_type==JWWindowSelector.OBJECTIVE:
-            drop_cols.append(f"{prefix}next_int_nan")
-
-        # if window_type==JWWindowSelector.QUIZ:
-        #     drop_cols.append(f"{prefix}answers")
-
-        X = X.drop(columns=drop_cols)
-        meta.append(f"Dropped drop_cols: {drop_cols}")
-        constant_cols = X.columns[X.nunique()==1]
-        X = X.drop(columns=constant_cols)
-        meta.append(f'Dropped constant_cols: {constant_cols}')
-        if not len(X):
-            return None, None, meta 
-        if window_type == JWWindowSelector.OBJECTIVE and drop_first_next_int_col:
-            next_int_cols = [c for c in X.columns if 'next_int' in c]
-            if next_int_cols:
-                X = X.drop(columns=next_int_cols[0])
-                meta.append(f'Dropped onehot column {next_int_cols[0]} from {next_int_cols}')
-
-        ## does not bin by default
-        if nbins:
-            est = KBinsDiscretizer(n_bins=nbins, encode='onehot-dense', strategy='quantile')
-            bin_feats = [f'{prefix}first_enc_avg_tbps', 
-                        f'{prefix}first_enc_avg_wps',
-                        # f'{prefix}first_enc_duration',
-                        f'{prefix}first_enc_var_tbps',
-                        f'{prefix}first_enc_var_wps']
-            bin_feats = [c for c in bin_feats if c in X.columns]
-            if bin_feats:
-                    
-                Xt = est.fit_transform(X[bin_feats])
-                new_feat_names = [f'{feat}>{x:.2f}' for bins,feat in zip(est.bin_edges_,bin_feats) for x in list(bins)[:-1]]
-
-                Xt_df = pd.DataFrame(Xt, index=X.index, columns=new_feat_names)
-                X = X.join(Xt_df)
-                X = X.drop(columns=bin_feats)
-                meta.append(f'Quantized n_bins={nbins} feats {bin_feats} to {new_feat_names}')
-
-        return (X, Y, meta)
-
-    def get_X_Y_meta_range(self, ns, window_type, max_seconds_per_word=2,nbins=0, drop_first_next_int_col = True, verbose=True):
-        X, Y, meta = None, None, []
-        for n in ns:
-            tX, tY, tmeta = self.get_X_Y_meta(n, window_type, max_seconds_per_word=max_seconds_per_word, nbins=nbins, drop_first_next_int_col=drop_first_next_int_col)
-            X, Y, meta = JWWindowSelector.join_X_Y_meta(X, Y, meta, tX, tY, tmeta, copy=False)
-            print('Join Size:', X.shape)
-        X, Y = X.copy(), Y.copy()
-        return X, Y, meta
-
-    @staticmethod
-    def join_X_Y_meta(X1, Y1, meta1, X2, Y2, meta2, copy=True):
-        meta = meta1+meta2
-        if X1 is None:
-            X = X2
-            Y = Y2
-        elif X2 is None:
-            X = X1
-            Y = Y1
-        else:
-            X = X1.join(X2, how='inner')
-            Y = Y1.loc[X.index, :]
-            meta = meta1+['--Inner Join--']+meta2+[f'Resultant Join Shape: {X.shape}']
-        if copy and X is not None:
-            X, Y = X.copy(), Y.copy()
-        return X, Y, meta
-        
-                
-
+# google imports
+
+# standard library imports
+import sys
+import copy
+import pickle
+import os
+from collections import Counter
+from io import BytesIO
+from zipfile import ZipFile
+import copy
+import pickle
+from math import ceil
+import importlib
+import urllib.request
+
+# math imports
+from matplotlib import pyplot as plt
+import numpy as np
+import pandas as pd
+from scipy import stats
+import seaborn as sns
+sns.set()
+
+# Jupyter Imports
+from IPython.display import display
+import ipywidgets as widgets
+# from google.colab import files
+
+# ML imports
+# models
+from sklearn.naive_bayes import CategoricalNB
+from sklearn.tree import ExtraTreeClassifier, DecisionTreeClassifier
+from sklearn.neural_network import MLPClassifier
+from xgboost import XGBClassifier
+from sklearn.linear_model import RidgeCV, SGDRegressor
+from sklearn.svm import LinearSVR
+
+
+# preprocessing
+from sklearn.impute import SimpleImputer
+from sklearn.compose import ColumnTransformer
+from sklearn.preprocessing import StandardScaler, OneHotEncoder, KBinsDiscretizer
+from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
+from sklearn.model_selection import train_test_split
+
+# sampling
+from imblearn.over_sampling import RandomOverSampler
+from imblearn.under_sampling import RandomUnderSampler, EditedNearestNeighbours, RepeatedEditedNearestNeighbours
+from imblearn.combine import SMOTEENN, SMOTETomek
+
+# metrics
+from sklearn.metrics import confusion_matrix, classification_report
+from sklearn.metrics import plot_precision_recall_curve, plot_confusion_matrix, plot_roc_curve
+from sklearn.metrics import f1_score, roc_auc_score, roc_curve, accuracy_score
+
+# other
+from imblearn.pipeline import make_pipeline
+from sklearn.model_selection import GridSearchCV
+
+# custom imports
+import feature_utils as feat_util
+
+
+def response_boxplot(df, category, verbose=False):
+    print('\n'+category)
+    fig, axs = plt.subplots(1, 3, figsize=(20, 10))
+    qs = ['EFL_yes_no', 'skill_low_med_high', 'enjoy_high_med_low_none']
+    for i, f in enumerate(['R0_quiz_response', 'R1_quiz_response', 'R2_quiz_response', ]):
+        if verbose:
+            print(qs[i])
+        bp = df.boxplot(column=category, by=df[f].astype(
+            'category'), ax=axs[i])
+        bp.set_xlabel('')
+        for choice in range(df[f].min(), df[f].max()+1):
+            query = f"{f}=={choice}"
+            cat_df = df.query(query)[category]
+            num_chose = len(cat_df)
+            mean = cat_df.mean()
+            std = cat_df.std()
+            if verbose:
+                print(
+                    f'{f} # chose {choice}: {num_chose} ({round(num_chose/len(df)*100)}%). Avg {mean}, std {std}.')
+    plt.suptitle(f'{category} Boxplot')
+    fig.show()
+
+
+def group_by_func(df, func, title='', show=True):
+    r0_groups = {0: 'native', 1: 'nonnative'}
+    r1_groups = {0: 'not very good skill',
+                 1: 'okay skill', 2: 'very good skill'}
+    r2_groups = {0: 'really enjoy', 1: 'enjoy', 2: 'okay', 3: 'not enjoy'}
+    def group_string(r0, r1, r2): return ', '.join(
+        [r0_groups[r0], r1_groups[r1], r2_groups[r2]])
+    result_dfs = [pd.DataFrame(index=r1_groups.values(), columns=r2_groups.values(
+    )), pd.DataFrame(index=r1_groups.values(), columns=r2_groups.values())]
+    if show:
+        print(f'{"-"*6}  {title}  {"-"*6}')
+    for r0 in [0, 1]:
+        subtitle = "Nonnatives" if r0 else "Natives"
+        if show:
+            print(f'\n{subtitle}:')
+        tdf0 = df.query(f"R0_quiz_response == {r0}")
+        for r1 in [0, 1, 2]:
+            tdf1 = tdf0.query(f"R1_quiz_response == {r1}")
+            for r2 in [0, 1, 2, 3]:
+                tdf2 = tdf1.query(f"R2_quiz_response == {r2}")
+                result_dfs[r0].loc[r1_groups[r1], r2_groups[r2]
+                                   ] = func(df, tdf0, tdf1, tdf2)
+        if show:
+            display(result_dfs[r0])
+    return result_dfs
+
+
+def standard_group_by_func(fulldf, per_category_stats_list=None):
+    per_category_stats_list = None or ['sess_count_clicks',
+                                       'sess_count_hovers',
+                                       'sess_meaningful_action_count',
+                                       'sess_EventCount',
+                                       'sess_count_notebook_uses',
+                                       'sess_avg_time_between_clicks',
+                                       'sess_first_enc_words_read',
+                                       'sess_first_enc_boxes_read',
+                                       'sess_num_enc',
+                                       'sess_first_enc_duration',
+                                       'sess_first_enc_avg_wps',
+                                       'sess_first_enc_var_wps',
+                                       'sess_first_enc_avg_tbps',
+                                       'sess_first_enc_var_tbps',
+                                       'sess_start_obj',
+                                       'sess_end_obj',
+                                       'start_level',
+                                       'max_level',
+                                       'sessDuration']
+    dfs_list = []
+    title_list = []
+
+    def df_func(df, tdf0, tdf1, tdf2): return len(tdf2)
+    title = 'count'
+    dfs = group_by_func(fulldf, df_func, title)
+    dfs_list.append(dfs)
+    title_list.append(title)
+
+    def df_func(df, tdf0, tdf1, tdf2): return round(len(tdf2)/len(df)*100, 2)
+    title = 'percent total pop'
+    dfs = group_by_func(fulldf, df_func, title)
+    dfs_list.append(dfs)
+    title_list.append(title)
+
+    def df_func(df, tdf0, tdf1, tdf2): return round(len(tdf2)/len(tdf0)*100, 2)
+    title = 'percent native class pop'
+    dfs = group_by_func(fulldf, df_func, title)
+    dfs_list.append(dfs)
+    title_list.append(title)
+
+    for category in per_category_stats_list:
+        df_func = get_avg_std_df_func(category)
+        title = f'(avg, std) {category}'
+        dfs = group_by_func(fulldf, df_func, title)
+        dfs_list.append(dfs)
+        title_list.append(title)
+    return title_list, dfs_list
+
+
+def get_avg_std_df_func(category_name):
+    def inner(df, tdf0, tdf1, tdf2):
+        mean = tdf2[category_name].mean()
+        std = tdf2[category_name].std()
+        if not pd.isna(mean):
+            mean = round(mean, 2)
+        if not pd.isna(std):
+            std = round(std, 2)
+        return (mean, std)
+    return inner
+
+
+def html_stats(df):
+    html_strs = ['<div class="container">', '<h3>{Stats}</h3>']
+    qs = ['EFL_yes_no', 'skill_low_med_high', 'enjoy_high_med_low_none']
+    html_strs.append(f'<p> Total pop {len(df)} </p>')
+    for i, f in enumerate(['R0_quiz_response', 'R1_quiz_response', 'R2_quiz_response', ]):
+        html_strs.append(f'<p> {qs[i]}</p>')
+        for choice in range(df[f].min(), df[f].max()+1):
+            query = f"{f}=={choice}"
+            cat_df = df.query(query)
+            num_chose = len(cat_df)
+            html_strs.append(
+                f'<p>{f} # chose {choice}: {num_chose} ({round(num_chose/len(df)*100)}%).</p>')
+    return '\n'.join(html_strs+['</div>'])
+
+
+def full_html(base_df, title_list, dfs_list, suptitle=None):
+    HEADER = '''<!DOCTYPE html>
+<html lang="en">
+
+<head>
+  <meta charset="UTF-8">
+  <meta name="viewport" content="width=device-width, initial-scale=1.0">
+  <title>Document</title>
+</head>
+
+<body>
+  <style>
+    .flex-container {
+      display: flex;
+      flex-wrap: wrap;
+    }
+
+    .container {
+      border: thick solid black;
+      padding: 10px;
+      margin: 5px;
+    }
+
+    .container table:nth-of-type(2) td {
+      background-color: rgb(161, 161, 230);
+    }
+
+    .container table:nth-of-type(2) th {
+      background-color: rgb(20, 20, 194);
+      color: white;
+    }
+
+    .container table:nth-of-type(2n-1) td {
+      background-color: rgb(235, 158, 158);
+    }
+
+    .container table:nth-of-type(2n-1) th {
+      background-color: rgb(160, 11, 11);
+      color: white;
+    }
+    .break {
+  flex-basis: 100%;
+  height: 0;
+}
+  </style>
+  <div class="flex-container">'''
+    FOOTER = '''  </div>
+    </body>
+
+    </html>'''
+
+    def table_header(title): return f'''    <div class="container">
+        <h3>{title}</h3>'''
+    table_footer = '''    </div>'''
+    def table_html(title, dfs): return '\n'.join([table_header(
+        title), "<p>Natives:</p>", dfs[0].to_html(), "<p>Nonnatives:</p>", dfs[1].to_html(), table_footer])
+
+    if suptitle is not None:
+        suptitle = f'<h2>{suptitle}</h2>\n<div class="break"></div> <!-- break -->'
+    else:
+        suptitle = ''
+    return '\n'.join([HEADER, suptitle, html_stats(base_df)] +
+                     [table_html(t, dfs) for t, dfs in zip(title_list, dfs_list)] +
+                     [FOOTER])
+
+
+def download_full_html(base_df, title_list, dfs_list, filename, suptitle=None):
+    with open(filename, 'w+') as f:
+        f.write(full_html(base_df, title_list, dfs_list, suptitle=suptitle))
+        print("Wrote to", filename)
+    files.download(filename)
+
+
+onext_int_feats = [f'obj{i}_onext_int' for i in range(80)]
+onext_int_cats = [["nan", 1],
+                  ["nan", 11],
+                  ["nan", 12, 86, 111, 125],
+                  ["nan", 13, 14, 113, 116, 118],
+                  ["nan", 14, 15, 113, 114, 116, 118],
+                  ["nan", 13, 15, 113, 114, 116, 118],
+                  ["nan", 16, 86, 115, 118, 132, 161],
+                  ["nan", 17, 86, 115, 118, 128, 161],
+                  ["nan", 18, 86, 115, 118, 161],
+                  ["nan", 19, 86, 117, 118, 127, 133, 134, 161],
+                  ["nan", 20, 133, 134, 136],
+                  ["nan", 2, 80, 81, 82, 83],
+                  ["nan", 21, 86, 117, 127, 136, 137, 161],
+                  ["nan", 22, 137, 141],
+                  ["nan", 23, 24, 86, 117, 127, 136, 161],
+                  ["nan", 23, 24, 117, 127, 136, 161],
+                  ["nan", 25, 86, 117, 118, 127, 136, 140, 147, 151, 161],
+                  ["nan", 26, 142, 145],
+                  ["nan", 27, 143],
+                  ["nan", 28, 86, 117, 118, 136, 140, 150, 161],
+                  ["nan", 29, 119, 130],
+                  ["nan", 29, 30, 35, 86, 117, 118, 126, 136, 140, 149],
+                  ["nan", 3, 80, 82, 83, 86, 87, 88, 93],
+                  ["nan", 31, 38],
+                  ["nan", 32, 153],
+                  ["nan", 33, 154],
+                  ["nan", 34, 155],
+                  ["nan", 35, 156],
+                  ["nan", 36, 157],
+                  ["nan", 37, 158],
+                  ["nan", 30],
+                  ["nan", 39, 163],
+                  ["nan", 40, 160],
+                  ["nan", 3],
+                  ["nan", 41, 164, 166],
+                  ["nan", 42, 166],
+                  ["nan", 30],
+                  ["nan", 44, 85, 125],
+                  ["nan", 29, 45, 47, 84, 118, 125, 136, 140, 149, 168, 169, 184],
+                  ["nan", 45, 46, 169, 170],
+                  ["nan", 29, 45, 47, 92, 118, 136, 140, 149, 169, 184],
+                  ["nan", 29, 45, 48, 92, 118, 140, 149, 168, 184],
+                  ["nan", 46, 49, 168],
+                  ["nan", 46, 50, 168, 170],
+                  ["nan", 5, 80, 82, 83, 86, 89, 91, 95, 97, 125],
+                  ["nan", 29, 51, 92, 118, 136, 140, 149, 168, 184],
+                  ["nan", 52, 92, 118, 136, 149, 171, 184],
+                  ["nan", 53, 54, 92, 118, 136, 140, 149, 184],
+                  ["nan", 53, 54, 55, 59, 60, 90, 92, 94,
+                      118, 136, 140, 149, 168, 184],
+                  ["nan", 53, 55, 59, 60, 90, 92, 94, 118, 136, 140, 149, 184],
+                  ["nan", 55, 56, 59, 60, 149, 174],
+                  ["nan", 57, 59, 60, 174],
+                  ["nan", 58, 59, 60, 136, 172, 174, 184],
+                  ["nan", 29, 59, 60, 61, 92, 118, 136, 149, 168, 172, 184],
+                  ["nan", 55, 56, 57, 58, 60, 61, 140, 172, 174, 184],
+                  ["nan", 6, 80, 82, 83, 86, 98, 100, 125],
+                  ["nan", 55, 56, 57, 58, 59, 61, 92, 118,
+                      136, 140, 149, 172, 174, 184],
+                  ["nan", 59, 62, 136, 140, 149, 172, 173, 175, 184],
+                  ["nan", 63, 64, 176],
+                  ["nan", 64, 66, 149, 175, 184],
+                  ["nan", 29, 65, 66, 92, 118, 136, 140, 172, 175, 177, 184],
+                  ["nan", 66, 67, 68, 92, 118, 136, 140, 146, 175, 177, 184],
+                  ["nan", 67, 144],
+                  ["nan", 29, 64, 65, 68, 92, 118, 131, 136,
+                      140, 148, 149, 172, 175, 177, 184],
+                  ["nan", 92, 118, 122, 123, 124, 131, 136, 140,
+                      146, 148, 168, 172, 175, 177, 184],
+                  ["nan", 70],
+                  ["nan", 7],
+                  ["nan", 71, 178],
+                  ["nan", 72, 179],
+                  ["nan", 73, 180],
+                  ["nan", 74, 181],
+                  ["nan", 75, 182],
+                  ["nan", 69],
+                  ["nan", 77, 78, 185],
+                  ["nan", 78, 185],
+                  ["nan", 79],
+                  [0],
+                  ["nan", 8],
+                  ["nan", 9, 103],
+                  ["nan", 104, 105, 108]]
+
+QA_1_feats = [f'Q{i}_A1' for i in range(19)]
+QA_1_cats = [['0', 'A', 'B', 'C', 'D'],
+             ['0', 'A', 'B', 'C', 'D'],
+             ['0', 'A', 'B', 'C', 'D'],
+             ['0', 'A', 'B', 'C', 'D'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', '?', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H',
+              'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q'],
+             ['0', 'A', 'B', 'C', 'D', 'F', 'G', 'I', 'M', 'N', 'O', 'P', 'Q',
+              'R', 'S', 'V', 'W', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f'],
+             ['0', 'Q', 'V', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f'],
+             ['0', '?', 'X', 'Y', 'Z', 'b', 'c', 'd', 'e', 'f'],
+             ['0', 'X', 'Y', 'b', 'c', 'd', 'e', 'f'],
+             ['0', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f']]
+
+
+def get_preprocessor(df, scaler=StandardScaler(), imputer=SimpleImputer(strategy='constant'), bool_dtype='int64'):
+    """
+    By default has a number of steps:
+    1. drops columns from use in preprocessor if present:
+       - [f'Q{q}_answers' for q in range(19)]
+       - ["play_year", "play_month", "play_day", "play_hour", "play_minute", "play_second"]
+       - ["_continue", "continue", "save_code", "music", "hq", "fullscreen", "persistentSessionID"]
+    2. Creates a preprocessor for all non-y columns and non-boolean columns with the following steps:
+       a. Standard Scaler (0 mean, 1 std)
+       b. Simple Imputer(strategy='constant') (fill NaN with 0)
+    3. Fits the preprocessor to the given X
+    4. returns the unfitted preprocessor (sklearn pipeline), and the unprocessed X dataframe
+    :param df: jowilder dataframe
+    :param scaler: sklearn compatible scaler
+    :param imputer: sklearn compatible imputer
+    :return: the unfitted preprocessor (sklearn pipeline), and the unprocessed X dataframe
+    """
+    df = df.drop(
+        [f'Q{q}_answers' for q in range(19)] + ["play_year", "play_month", "play_day", "play_hour", "play_minute",
+                                                "play_second",
+                                                "_continue", "continue", "save_code", "music", "hq", "fullscreen",
+                                                "persistentSessionID", ], axis=1, errors='ignore').copy()
+    y_cols, bool_cols, num_cols = separate_columns(df, bool_dtype=bool_dtype)
+    X = df.loc[:, num_cols+bool_cols]
+
+    # too complicated to allow for pipeline order
+    # pipeline_strings = [pipeline_order[i:i+2] for i in range(0,len(pipeline_order),2)]
+    # transformers = []
+    # num_sa, num_sc, num_im = 0,0,0
+    # for s in pipeline_strings:
+    #     if s == 'Sa':
+    #         transformer = make_pipeline(sampler)
+    #         cols = num_cols + bool_cols
+    #         name = f'{s}{num_sa}'
+    #         num_sa += 1
+    #     elif s == 'Sc':
+    #         transformer = scaler
+    #         name = f'{s}{num_sc}'
+    #         cols = num_cols
+    #         num_sc += 1
+    #     elif s == 'Im':
+    #         transformer = imputer
+    #         name = f'{s}{num_im}'
+    #         cols = num_cols
+    #         num_im += 1
+    #     else:
+    #         raise ValueError("Pipeline substrings must be Sa Sc or Im")
+    #     transformers.append((name, transformer, cols))
+
+    def col_str_to_int(col_strs): return [
+        X.columns.get_loc(s) for s in col_strs]
+    column_transformer = ColumnTransformer(
+        transformers=[
+            ('num', make_pipeline(scaler, imputer), col_str_to_int(num_cols)),
+            ('bool', 'passthrough', col_str_to_int(bool_cols))
+        ],
+        remainder='drop')
+    return column_transformer, X
+
+
+def get_ys(df):
+    """
+
+    :rtype: dictionary of y columns (df series). keys: y0,y1,y2,y1_bin,y2_bin,y1_bin_x,y2_bin_x
+    """
+    ys = {}
+    for key, y_col in [
+        ('y0', 'R0_quiz_response'),
+        ('y1', 'R1_quiz_response'),
+        ('y2', 'R2_quiz_response'),
+        ('y1_bin', 'R1_quiz_response_bin'),
+        ('y1_bin_0v12', 'R1_quiz_response_0v12'),
+        ('y1_bin_01v2', 'R1_quiz_response_01v2'),
+        ('y1_bin_x', 'R1_quiz_response_bin_x'),
+        ('y2_bin', 'R2_quiz_response_bin'),
+        ('y2_bin_x', 'R2_quiz_response_bin_x'),
+        ('y2_bin_0v123', 'R2_quiz_response_bin0v123'),
+        ('y2_bin_01v23', 'R2_quiz_response_bin01v23'),
+        ('y2_bin_012v3', 'R2_quiz_response_bin012v3'),
+    ]:
+        if y_col in df.columns:
+            ys[key] = df.loc[:, y_col].astype('category').copy()
+    return ys
+
+
+def separate_columns(df, bool_dtype='int64', expect_bool_cols = True) -> (list, list, list):
+    """
+
+    :param df:
+    :param bool_dtype: Defaults to 'int64'. Should be int64 if coming from import csv otherwise could be 'uint8'
+    if coming from the pd dummies.
+    :return: tuple of lists of column names for y_columns, bool_columns, and integer_columns
+    """
+    y_cols = [col for col in df.columns if 'quiz_response' in col]
+    bool_cols = [col for col in df.select_dtypes(include=[bool_dtype])
+                 if np.isin(df[col].dropna().unique(), [0, 1]).all() and
+                 col not in y_cols]
+    num_cols = [
+        col for col in df.columns if col not in bool_cols and col not in y_cols]
+    if not bool_cols and expect_bool_cols:
+        print('Warning! No bool columns. Consider changing bool_dtype="int_64" to "uint8"')
+    return y_cols, bool_cols, num_cols
+
+
+end_obj_to_last_Q = {
+    9: 0,
+    10: 3,
+    11: 3,
+    12: 3,
+    13: 3,
+    14: 3,
+    15: 3,
+    16: 3,
+    17: 3,
+    18: 3,
+    19: 3,
+    20: 3,
+    21: 3,
+    22: 3,
+    23: 3,
+    24: 3,
+    25: 3,
+    26: 3,
+    27: 3,
+    28: 3,
+    29: 3,
+    30: 3,
+    31: 3,
+    32: 4,
+    33: 5,
+    34: 6,
+    35: 7,
+    36: 8,
+    37: 9,
+    38: 9,
+    39: 10,
+    40: 11,
+    41: 12,
+    42: 13,
+    43: 13,
+    44: 13,
+    45: 13,
+    46: 13,
+    47: 13,
+    48: 13,
+    49: 13,
+    50: 13,
+    51: 13,
+    52: 13,
+    53: 13,
+    54: 13,
+    55: 13,
+    56: 13,
+    57: 13,
+    58: 13,
+    59: 13,
+    60: 13,
+    61: 13,
+    62: 13,
+    63: 13,
+    64: 13,
+    65: 13,
+    66: 13,
+    67: 13,
+    68: 13,
+    69: 13,
+    70: 13,
+    71: 14,
+    72: 15,
+    73: 16,
+    74: 17,
+    75: 18,
+    76: 18,
+    77: 18,
+    78: 18,
+    79: 18,
+}
+
+end_obj_to_last_lvl = {
+    0:	0,
+    1:	0,
+    2:	0,
+    3:	1,
+    4:	2,
+    5:	2,
+    6:	3,
+    7:	3,
+    8:	4,
+    9: 4,
+    10: 4,
+    11: 4,
+    12: 5,
+    13: 6,
+    14: 6,
+    15: 6,
+    16: 6,
+    17: 6,
+    18: 6,
+    19: 7,
+    20: 7,
+    21: 8,
+    22: 8,
+    23: 9,
+    24: 9,
+    25: 9,
+    26: 10,
+    27: 10,
+    28: 11,
+    29: 11,
+    30: 12,
+    31: 12,
+    32: 12,
+    33: 12,
+    34: 12,
+    35: 12,
+    36: 12,
+    37: 12,
+    38: 12,
+    39: 12,
+    40: 12,
+    41: 12,
+    42: 12,
+    43: 13,
+    44: 13,
+    45: 14,
+    46: 15,
+    47: 15,
+    48: 16,
+    49: 16,
+    50: 17,
+    51: 17,
+    52: 18,
+    53: 18,
+    54: 18,
+    55: 18,
+    56: 18,
+    57: 18,
+    58: 18,
+    59: 18,
+    60: 18,
+    61: 18,
+    62: 19,
+    63: 19,
+    64: 19,
+    65: 20,
+    66: 20,
+    67: 21,
+    68: 21,
+    69: 22,
+    70: 22,
+    71: 22,
+    72: 22,
+    73: 22,
+    74: 22,
+    75: 22,
+    76: 22,
+    77: 23,
+    78: 23,
+    79: 23,
+}
+
+
+class GridSearcher():
+
+    def __init__(self, csv_fpath=None, df=None, preprocessor=None, fillna=0, meta=[], expect_bool_cols=True):
+        # either give csv_fpath or df.
+        assert csv_fpath or not df.empty
+        print(f'Loading from {csv_fpath}...')
+        # load df
+        if df is None:
+            print(f'Loading from {csv_fpath}...')
+            self.df, self.meta = feat_util.open_csv_from_path_with_meta(
+                csv_fpath, index_col=0)
+        else:
+            self.df, self.meta = df, meta
+
+        # set X and ys, and preprocessor
+        if not preprocessor:
+            self.preprocessor, self.X = get_preprocessor(self.df)
+            self.X = self.X.fillna(fillna)
+        else:
+            _, bool_cols, num_cols = separate_columns(self.df, expect_bool_cols=expect_bool_cols)
+            self.X = df[bool_cols+num_cols]
+            self.preprocessor = preprocessor
+        self.ys = get_ys(self.df)
+
+        # set object vars
+        self.model_dict = {}
+        self.cur_model = None
+
+    def split_data(self):
+        nonnull_X, nonnull_y = feat_util.remove_nan_labels(self.X, self.y)
+        X_train, X_test, y_train, y_test = train_test_split(
+            nonnull_X, nonnull_y, test_size=0.2, random_state=1)
+        self.X_train, self.X_test, self.y_train, self.y_test = X_train, X_test, y_train, y_test
+
+    def set_y(self, y_key=None, other_col=None):
+        if y_key:
+            print(f'Switching to {y_key}...')
+            self.y = self.ys[y_key]
+        elif other_col:
+            self.y = self.X[other_col]
+            self.X = self.X.drop(other_col, axis=1)
+        else:
+            print("Did not change y. Invalid inputs.")
+        self.split_data()
+
+    def run_fit(self, classifier, sampler=None, verbose=False, preprocess_twice=True, sampler_index=None, full_pipeline=False):
+        # fit self.cur_model as a pipeline of the given preprocessor, sampler, preprocessor, classifer
+        # if preprocess_twice is false, self.cur_model is sampler, preprocessor, classifier
+        # if full_pipeline and sampler index, self.cur_model is the classifier 
+        # (must be a pipeline containing a sampler or a placeholder (None) for the sampler)
+        if full_pipeline:
+            assert sampler_index is not None
+            clf = classifier
+        elif preprocess_twice:
+            clf = make_pipeline(self.preprocessor, sampler,
+                                copy.deepcopy(self.preprocessor), classifier)
+            sampler_index = 1
+        else:
+            clf = make_pipeline(sampler, self.preprocessor, classifier)
+            sampler_index = 0
+
+        self._sampling_pipeline = clf[:sampler_index+1]
+        self._classifying_pipeline = clf[sampler_index+1:]
+        if clf[sampler_index] is not None:
+            self.X_train_sampled, self.y_train_sampled = self._sampling_pipeline.fit_resample(
+                self.X_train, self.y_train)
+        else:
+            self.X_train_sampled, self.y_train_sampled = self.X_train, self.y_train
+            clf = self._classifying_pipeline
+
+        # model_name = f'{sampler} {classifier}'
+        # if verbose:
+        #     print(f'Running {model_name}.')
+        self._classifying_pipeline.fit(
+            self.X_train_sampled, self.y_train_sampled)
+        self.cur_model = clf
+        # if verbose:
+        #     print("model trained to: %.3f" %
+        #           clf.score(self.X_train, self.y_train))
+        #     print("model score: %.3f" % clf.score(self.X_test, self.y_test))
+        return clf
+
+    def metrics(self, graph_dir=None, graph_prefix=None, binary_classification=True):
+        # return list of (metric: float, metric_name: str) tuples of metrics of given classifier (default: self.cur_model)
+        # can only do metrics for binary classification as of right now
+        assert binary_classification
+        metric_list = []
+        clf = self.cur_model
+
+        # label metrics
+        if graph_prefix:
+            for flipped_labels in [False, True]:
+                flipped_labels_suffix = '' if not flipped_labels else '_flipped'
+                fig, axes = plt.subplots(3, 3, figsize=(20, 20))
+                for i, (yarray, Xarray, label) in enumerate([(self.y_test, self.X_test, 'test'),
+                                                             (self.y_train_sampled,
+                                                              self.X_train_sampled, 'train'),
+                                                             (self.y_train,
+                                                              self.X_train, 'train_raw'),
+                                                             ]):
+                    for j, (graph_type, func) in enumerate([
+                        ('', plot_confusion_matrix),
+                        ('_PR', plot_precision_recall_curve),
+                        ('_ROC', plot_roc_curve),
+                    ]):
+                        ax = axes[j, i]
+                        graph_yarray = yarray.astype(bool)
+                        if flipped_labels:
+                            graph_yarray = ~graph_yarray
+                        disp = func(clf, Xarray, graph_yarray, ax=ax)
+                        title = f'{label}{graph_type}{flipped_labels_suffix}'
+                        ax.set_title(title)
+                        if graph_type in ['_PR', '_ROC']:
+                            ax.set_xlim(-0.05, 1.05)
+                            ax.set_ylim(-0.05, 1.05)
+                            ax.set_aspect('equal', adjustable='box')
+                suptitle = f'{graph_prefix}{flipped_labels_suffix}'
+                plt.suptitle(suptitle)
+                savepath = os.path.join(graph_dir, f'{suptitle}.png')
+                fig.savefig(savepath, dpi=100)
+                plt.close()
+
+        for i, (yarray, Xarray, label) in enumerate([(self.y_test, self.X_test, 'test'),
+                                                     (self.y_train_sampled,
+                                                      self.X_train_sampled, 'train'),
+                                                     (self.y_train,
+                                                      self.X_train, 'train_raw'),
+                                                     ]):
+
+            y_pred = clf.predict(Xarray)
+            y_prob = clf.predict_proba(Xarray)[:, 1]
+            y_true = yarray
+            X_shape = Xarray.shape
+            metric_list.extend(feat_util.binary_metric_list(
+                y_true=y_true, y_pred=y_pred, y_prob=y_prob, X_shape=X_shape,
+                label_prefix=f'{label}_'
+            ))
+
+
+
+        return metric_list
+
+    def model_stats(self, classifier=None, graph=True):
+        # counter, auc, and optional graph of given classifer (default: self.cur_model)
+        classifier = classifier or self.cur_model
+        y_prob = classifier.predict_proba(self.X_test)[:, 1]
+        print(f"dimension y_prob: {y_prob.shape}")
+        print(f"dimension y_test: {self.y_test.shape}")
+        print(f'Predicts:', Counter(list(classifier.predict(self.X_test))))
+        print(f'True Labels:', Counter(self.y_test))
+        if graph:
+            fpr, tpr, thres = roc_curve(self.y_test, y_prob)
+            plt.plot(fpr, tpr, color='green')
+            plt.plot([0, 1], [0, 1], color='red', linestyle='--')
+            plt.show()
+        roc_auc = roc_auc_score(self.y_test, y_prob)
+        print(f"ROC-AUC Score: {roc_auc}")
+
+    def classification_report(self):
+        # classification report on current model
+        y_true = self.y_test
+        y_pred = self.cur_model.predict(self.X_test)
+        print(classification_report(y_true, y_pred))
+
+
+class JWWindowSelector:
+
+    ycols = ['R0_quiz_response','R1_quiz_response','R2_quiz_response','R1_quiz_response_bin',
+            'R1_quiz_response_0v12','R1_quiz_response_01v2','R1_quiz_response_bin_x',
+            'R2_quiz_response_bin','R2_quiz_response_bin_x','R2_quiz_response_bin0v123',
+            'R2_quiz_response_bin01v23','R2_quiz_response_bin012v3']
+    INTERACTION = 0
+    LEVEL = 1
+    QUIZ = 2
+    OBJECTIVE = 3
+
+    def __init__(self, csv_fpath=None, df=None, meta=None):
+        assert csv_fpath is not None or df is not None
+        # load df
+        if df is None:
+            print(f'Loading from {csv_fpath}...')
+            self.df, self.meta = feat_util.open_csv_from_path_with_meta(
+                csv_fpath, index_col=0)
+        else:
+            self.df = df
+            self.meta = meta or []
+
+        self.df_cols = list(df.columns)
+
+    @staticmethod
+    def get_abbrev(window_type):
+        if window_type == JWWindowSelector.INTERACTION:
+            return 'int'
+        if window_type == JWWindowSelector.LEVEL:
+            return 'lvl'
+        if window_type == JWWindowSelector.QUIZ:
+            return 'q'
+        if window_type == JWWindowSelector.OBJECTIVE:
+            return 'obj'
+
+    @staticmethod
+    def get_prefix(n, window_type):
+        if window_type == JWWindowSelector.INTERACTION:
+            return f'int{n}_i'
+        if window_type == JWWindowSelector.LEVEL:
+            return f'lvl{n}_'
+        if window_type == JWWindowSelector.QUIZ:
+            return f'Q{n}_'
+        if window_type == JWWindowSelector.OBJECTIVE:
+            return f'obj{n}_o'
+
+    @staticmethod
+    def get_window_range(window_type, skip_Q23=False):
+        if window_type == JWWindowSelector.INTERACTION:
+            return range(189)
+        if window_type == JWWindowSelector.LEVEL:
+            return range(24)
+        if window_type == JWWindowSelector.QUIZ:
+            if not skip_Q23:
+                return range(19)
+            else:
+                return [0,1,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18]
+        if window_type == JWWindowSelector.OBJECTIVE:
+            return range(80)
+
+
+    def cols_startwith(self, prefix):
+        return [c for c in self.df_cols if c.startswith(prefix)]
+    def get_feats(self, n, window_type):
+        prefix = self.get_prefix(n, window_type)
+        feats = self.cols_startwith(prefix)
+        return feats
+
+    def get_filter_queries(self, n, window_type, max_seconds_per_word=2):
+        prefix = JWWindowSelector.get_prefix(n, window_type)
+        queries = [f"R1_quiz_response == R1_quiz_response"]
+        if window_type in [JWWindowSelector.INTERACTION, JWWindowSelector.LEVEL]:
+            queries.extend([
+                        f"{prefix}first_enc_duration == {prefix}first_enc_duration",
+                        f"{prefix}first_enc_duration > 0",
+            ])
+        if window_type == JWWindowSelector.QUIZ:
+            queries.extend([
+                f'{prefix}A1_nan!=1'
+            ])
+        elif window_type == JWWindowSelector.INTERACTION:
+            num_words = self.df[f"int{n}_ifirst_enc_words_read"].max()
+            queries.extend([
+                    f"{prefix}first_enc_words_read == {num_words}",
+                    f"{prefix}time_to > 0",
+                    f"{prefix}first_enc_duration < {prefix}first_enc_words_read*{max_seconds_per_word}",
+                    ])
+        elif window_type == JWWindowSelector.OBJECTIVE:
+            if n < 79:
+                queries.append(f'obj{n}_onext_int_nan==0')
+                queries.append(f"obj{n}_otime_to_next_obj < 600")
+                queries.append(f"obj{n}_otime_to_next_obj > 0 ")
+
+        elif window_type == JWWindowSelector.LEVEL:
+            queries.append(f"{prefix}time_in_level < 1200")
+            queries.append(f"{prefix}time_in_level > 0")
+
+        queries.extend([f"R{i}_quiz_response == R{i}_quiz_response" for i in [0,1,2]])
+        return queries
+
+    def get_base_meta(self):
+        return self.meta
+    
+    @staticmethod
+    def join_XY(X,Y):
+        return X.join(Y)
+    
+    def get_X_Y_meta(self, n, window_type, max_seconds_per_word=2,nbins=0, drop_first_next_int_col = True):
+        meta = []
+        prefix = JWWindowSelector.get_prefix(n, window_type)
+        Xfeats = self.get_feats(n, window_type)
+        meta.append(f'Using feats: {Xfeats}')
+
+        if window_type==JWWindowSelector.INTERACTION:
+            total_words = self.df[f"int{n}_ifirst_enc_words_read"].max() 
+            if total_words is np.nan:
+                return None, None, meta
+            elif total_words < 10:
+                print('Total words < 10!')
+        queries = self.get_filter_queries(n, window_type, max_seconds_per_word=max_seconds_per_word)
+        filtered_df, filtered_df_meta = feat_util.filter_df(self.df[Xfeats+JWWindowSelector.ycols], query_list=queries, verbose=True, fillna=None)
+        meta.extend(filtered_df_meta)
+        X = filtered_df[Xfeats].fillna(0).copy()
+        meta.append(f'Filled X with 0')
+        Y = filtered_df[JWWindowSelector.ycols].copy()
+        drop_cols = []
+        if window_type in [JWWindowSelector.INTERACTION, JWWindowSelector.LEVEL]:
+            drop_cols = [
+                f"{prefix}first_enc_boxes_read",
+                f"{prefix}first_enc_words_read",
+            ]
+        if window_type==JWWindowSelector.INTERACTION:
+            drop_cols.extend([
+            f"{prefix}time_to",
+            f"{prefix}total_duration"
+            ])
+        if window_type==JWWindowSelector.OBJECTIVE:
+            drop_cols.append(f"{prefix}next_int_nan")
+
+        # if window_type==JWWindowSelector.QUIZ:
+        #     drop_cols.append(f"{prefix}answers")
+
+        X = X.drop(columns=drop_cols)
+        meta.append(f"Dropped drop_cols: {drop_cols}")
+        constant_cols = X.columns[X.nunique()==1]
+        X = X.drop(columns=constant_cols)
+        meta.append(f'Dropped constant_cols: {constant_cols}')
+        if not len(X):
+            return None, None, meta 
+        if window_type == JWWindowSelector.OBJECTIVE and drop_first_next_int_col:
+            next_int_cols = [c for c in X.columns if 'next_int' in c]
+            if next_int_cols:
+                X = X.drop(columns=next_int_cols[0])
+                meta.append(f'Dropped onehot column {next_int_cols[0]} from {next_int_cols}')
+
+        ## does not bin by default
+        if nbins:
+            est = KBinsDiscretizer(n_bins=nbins, encode='onehot-dense', strategy='quantile')
+            bin_feats = [f'{prefix}first_enc_avg_tbps', 
+                        f'{prefix}first_enc_avg_wps',
+                        # f'{prefix}first_enc_duration',
+                        f'{prefix}first_enc_var_tbps',
+                        f'{prefix}first_enc_var_wps']
+            bin_feats = [c for c in bin_feats if c in X.columns]
+            if bin_feats:
+                    
+                Xt = est.fit_transform(X[bin_feats])
+                new_feat_names = [f'{feat}>{x:.2f}' for bins,feat in zip(est.bin_edges_,bin_feats) for x in list(bins)[:-1]]
+
+                Xt_df = pd.DataFrame(Xt, index=X.index, columns=new_feat_names)
+                X = X.join(Xt_df)
+                X = X.drop(columns=bin_feats)
+                meta.append(f'Quantized n_bins={nbins} feats {bin_feats} to {new_feat_names}')
+
+        return (X, Y, meta)
+
+    def get_X_Y_meta_range(self, ns, window_type, max_seconds_per_word=2,nbins=0, drop_first_next_int_col = True, verbose=True):
+        X, Y, meta = None, None, []
+        for n in ns:
+            tX, tY, tmeta = self.get_X_Y_meta(n, window_type, max_seconds_per_word=max_seconds_per_word, nbins=nbins, drop_first_next_int_col=drop_first_next_int_col)
+            X, Y, meta = JWWindowSelector.join_X_Y_meta(X, Y, meta, tX, tY, tmeta, copy=False)
+            print('Join Size:', X.shape)
+        X, Y = X.copy(), Y.copy()
+        return X, Y, meta
+
+    @staticmethod
+    def join_X_Y_meta(X1, Y1, meta1, X2, Y2, meta2, copy=True):
+        meta = meta1+meta2
+        if X1 is None:
+            X = X2
+            Y = Y2
+        elif X2 is None:
+            X = X1
+            Y = Y1
+        else:
+            X = X1.join(X2, how='inner')
+            Y = Y1.loc[X.index, :]
+            meta = meta1+['--Inner Join--']+meta2+[f'Resultant Join Shape: {X.shape}']
+        if copy and X is not None:
+            X, Y = X.copy(), Y.copy()
+        return X, Y, meta
+        
+                
+
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/LAKELAND/lakeland_utils.py` & `OGDUtils-0.1.5/src/OGDUtils/LAKELAND/lakeland_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-# standard library imports
-import sys
-import copy
-import pickle
-import os
-from collections import Counter
-from io import BytesIO
-from zipfile import ZipFile
-import copy
-import pickle
-from math import ceil
-import importlib
-import urllib.request
-
-# math imports
-from matplotlib import pyplot as plt
-import numpy as np
-import pandas as pd
-from scipy import stats
-import seaborn as sns
-sns.set()
-
-# google imports
-
-# Jupyter Imports
-from IPython.display import display
-import ipywidgets as widgets
-# from google.colab import files
-
-# ML imports
-# models
-from sklearn.naive_bayes import CategoricalNB
-from sklearn.tree import ExtraTreeClassifier, DecisionTreeClassifier
-from sklearn.neural_network import MLPClassifier
-from xgboost import XGBClassifier
-from sklearn.linear_model import RidgeCV, SGDRegressor
-from sklearn.svm import LinearSVR
-
-# preprocessing
-from sklearn.impute import SimpleImputer
-from sklearn.compose import ColumnTransformer
-from sklearn.preprocessing import StandardScaler, OneHotEncoder, KBinsDiscretizer
-from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
-from sklearn.model_selection import train_test_split
-
-# sampling
-from imblearn.over_sampling import RandomOverSampler
-from imblearn.under_sampling import RandomUnderSampler, EditedNearestNeighbours, RepeatedEditedNearestNeighbours
-from imblearn.combine import SMOTEENN, SMOTETomek
-
-# metrics
-from sklearn.metrics import confusion_matrix, classification_report
-from sklearn.metrics import plot_precision_recall_curve, plot_confusion_matrix, plot_roc_curve
-from sklearn.metrics import f1_score, roc_auc_score, roc_curve, accuracy_score
-
-# other
-from imblearn.pipeline import make_pipeline
-from sklearn.model_selection import GridSearchCV
-
-# custom imports
-import general.feature_utils as feat_util
-
-# consider making a general version with parameter for filename, index columns
-# def getLakelandDecJanLogDF():
-#     """
-
-#     :return: (df, metadata List[str])
-#     """
-#     # define paths for DecJanLog
-#     _proc_zip_url_dec = 'https://opengamedata.fielddaylab.wisc.edu/data/LAKELAND/LAKELAND_20191201_to_20191231_de09c18_proc.zip'
-#     _proc_zip_path_jan = 'Data/Raw Log Data/LAKELAND_20200101_to_20200131_a9720c1_proc.zip'
-#     # get the data
-#     metadata = []
-#     zipfile_dec, meta = openZipFromURL(_proc_zip_url_dec)
-#     metadata.extend(meta)
-#     zipfile_jan, meta = openZipFromPath(_proc_zip_path_jan)
-#     metadata.extend(meta)
-#     # put the data into a dataframe
-#     df = pd.DataFrame()
-#     for zf in [zipfile_dec, zipfile_jan]:
-#         with zf.open(zf.namelist()[0]) as f:
-#             df = pd.concat([df, pd.read_csv(f, index_col=['sessID', 'num_play'], comment='#')], sort=True)
-#     df['sessID'] = [x[0] for x in df.index]
-#     df['num_play'] = [x[1] for x in df.index]
-#     return df, metadata
-
-
-def get_lakeland_default_filter(lvlstart: Optional[int] = None, lvlend: Optional[bool] = None, no_debug: Optional[bool] = True,
-                                min_sessActiveEventCount: Optional[int] = 10,
-                                min_lvlstart_ActiveEventCount: Optional[int] = 3,
-                                min_lvlend_ActiveEventCount: Optional[int] = 3, min_sessDuration: Optional[int] = 300, max_sessDuration: Optional[int] = None, cont: Optional[bool] = False) -> List[str]:
-    """
-
-    :param lvlstart: levelstart to be used for other parameters (None if not used)
-    :param lvlend: levelend to be used for other parameters (None if not used)
-    :param no_debug: boolean whether or not to use only players that have used SPYPARTY or only not used SPYPARTY  (None if not used)
-    :param min_sessActiveEventCount:  (None if not used)
-    :param min_lvlstart_ActiveEventCount:  (None if not used)
-    :param min_lvlend_ActiveEventCount:  (None if not used)
-    :param min_sessDuration:  (None if not used)
-    :param max_sessDuration:  (None if not used)
-    :param cont:  (None if not used)
-    :return:
-    """
-    get_lakeland_default_filter()
-    query_list = []
-
-    if no_debug:
-        query_list.append('debug == 0')
-    if min_sessActiveEventCount is not None:
-        query_list.append(
-            f'sess_ActiveEventCount >= {min_sessActiveEventCount}')
-    if lvlstart is not None and min_lvlstart_ActiveEventCount is not None:
-        query_list.append(
-            f'lvl{lvlstart}_ActiveEventCount >= {min_lvlstart_ActiveEventCount}')
-    if lvlend is not None and min_lvlend_ActiveEventCount is not None:
-        query_list.append(
-            f'lvl{lvlend}_ActiveEventCount >= {min_lvlend_ActiveEventCount}')
-    if min_sessDuration is not None:
-        query_list.append(f'sessDuration >= {min_sessDuration}')
-    if max_sessDuration is not None:
-        query_list.append(f'sessDuration <= {max_sessDuration}')
-    if cont is not None:
-        query_list.append(f'_continue == {int(cont)}')
-
-    return query_list
-
-# def describe_lvl_feats_lakeland(df, fbase_list, lvl_range, level_time=300, level_overlap=30):
-#     """
-#     Calculates sum/avg of given level base features (fnames without lvlN_ prefix) in the level range.
-#     Will automatically filter out players who did not complete the given level range in the df
-#     May have a bug.
-
-#     :param level_time: number of seconds per level (window)
-#     :param level_overlap: number of overlap seconds per level (window)
-#     :rtype: (df, List[str]) where the new df includes sum_ and avg_lvl_A_to_B.
-#     :param df: dataframe to pull from and append to
-#     :param fbase_list: list of feature bases (fnames without lvlN_ prefix)
-#     :param lvl_range: range of levels to choose. typically range(min_level, max_level+1)
-#     """
-#     metadata = []
-#     metadata.append(f'*arg* lvlfeats = {fbase_list}')
-#     metadata.append(f'*arg* lvlrange = {lvl_range}')
-#     if not fbase_list:
-#         return df, metadata
-#     lvl_start, lvl_end = lvl_range[0], lvl_range[-1]
-#     query = f'sessDuration > {(level_time - level_overlap) * (lvl_end) + level_time}'
-#     df = df.query(query)
-#     metadata.append(
-#         f'Describe Level Feats lvls {lvl_start} to {lvl_end}. Assuming WINDOW_SIZE_SECONDS={level_time} and WINDOW_OVERLAP_SECONDS={level_overlap}, filtered by ({query})')
-#     fromlvl, tolvl = lvl_range[0], lvl_range[-1]
-#     sum_prefix = f'sum_lvl_{fromlvl}_to_{tolvl}_'
-#     avg_prefix = f'avg_lvl_{fromlvl}_to_{tolvl}_'
-#     for fn in fbase_list:
-#         tdf = df[[f'lvl{i}_{fn}' for i in lvl_range]].fillna(0).copy()
-#         df[sum_prefix + fn] = tdf.sum(axis=1)
-#         df[avg_prefix + fn] = tdf.mean(axis=1)
-#     return df, metadata
-
-def get_feat_selection_lakeland(df,  max_lvl=9):
-    """
-    Gets the feature selection widget.
-    :param df:
-    :param max_lvl:
-    :return:
-    """
-    start_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='Start Level:',
-                                    disabled=False, continuous_update=False, orientation='horizontal', readout=True, readout_format='d')
-    end_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='End Level:',
-                                  disabled=False, continuous_update=False, orientation='horizontal', readout=True, readout_format='d')
-    level_selection = widgets.GridBox([start_level, end_level])
-
-    def change_start_level(change):
-        end_level.min = start_level.value
-        if end_level.value < start_level.value:
-            end_level.value = start_level.value
-    start_level.observe(change_start_level, names="value")
-
-    lvl_feats = sorted(set([f[5:] for f in df.columns if f.startswith('lvl')]))
-    sess_feats = sorted(
-        set([f[5:] for f in df.columns if f.startswith('sess_')]))
-    other_feats = sorted(set([f for f in df.columns if not f.startswith(
-        'lvl') and not f.startswith('sess_')]))
-    selection_widget = widgets.GridBox([multi_checkbox_widget(lvl_feats, 'lvl'),
-                                        multi_checkbox_widget(
-                                            sess_feats, 'sess'),
-                                        multi_checkbox_widget(
-                                            other_feats, 'other'),
-                                        level_selection],
-                                       layout=widgets.Layout(grid_template_columns=f"repeat(3, 500px)"))
-
-    return selection_widget
+# standard library imports
+import sys
+import copy
+import pickle
+import os
+from collections import Counter
+from io import BytesIO
+from zipfile import ZipFile
+import copy
+import pickle
+from math import ceil
+import importlib
+import urllib.request
+
+# math imports
+from matplotlib import pyplot as plt
+import numpy as np
+import pandas as pd
+from scipy import stats
+import seaborn as sns
+sns.set()
+
+# google imports
+
+# Jupyter Imports
+from IPython.display import display
+import ipywidgets as widgets
+# from google.colab import files
+
+# ML imports
+# models
+from sklearn.naive_bayes import CategoricalNB
+from sklearn.tree import ExtraTreeClassifier, DecisionTreeClassifier
+from sklearn.neural_network import MLPClassifier
+from xgboost import XGBClassifier
+from sklearn.linear_model import RidgeCV, SGDRegressor
+from sklearn.svm import LinearSVR
+
+# preprocessing
+from sklearn.impute import SimpleImputer
+from sklearn.compose import ColumnTransformer
+from sklearn.preprocessing import StandardScaler, OneHotEncoder, KBinsDiscretizer
+from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
+from sklearn.model_selection import train_test_split
+
+# sampling
+from imblearn.over_sampling import RandomOverSampler
+from imblearn.under_sampling import RandomUnderSampler, EditedNearestNeighbours, RepeatedEditedNearestNeighbours
+from imblearn.combine import SMOTEENN, SMOTETomek
+
+# metrics
+from sklearn.metrics import confusion_matrix, classification_report
+from sklearn.metrics import plot_precision_recall_curve, plot_confusion_matrix, plot_roc_curve
+from sklearn.metrics import f1_score, roc_auc_score, roc_curve, accuracy_score
+
+# other
+from imblearn.pipeline import make_pipeline
+from sklearn.model_selection import GridSearchCV
+
+# custom imports
+import general.feature_utils as feat_util
+
+# consider making a general version with parameter for filename, index columns
+# def getLakelandDecJanLogDF():
+#     """
+
+#     :return: (df, metadata List[str])
+#     """
+#     # define paths for DecJanLog
+#     _proc_zip_url_dec = 'https://opengamedata.fielddaylab.wisc.edu/data/LAKELAND/LAKELAND_20191201_to_20191231_de09c18_proc.zip'
+#     _proc_zip_path_jan = 'Data/Raw Log Data/LAKELAND_20200101_to_20200131_a9720c1_proc.zip'
+#     # get the data
+#     metadata = []
+#     zipfile_dec, meta = openZipFromURL(_proc_zip_url_dec)
+#     metadata.extend(meta)
+#     zipfile_jan, meta = openZipFromPath(_proc_zip_path_jan)
+#     metadata.extend(meta)
+#     # put the data into a dataframe
+#     df = pd.DataFrame()
+#     for zf in [zipfile_dec, zipfile_jan]:
+#         with zf.open(zf.namelist()[0]) as f:
+#             df = pd.concat([df, pd.read_csv(f, index_col=['sessID', 'num_play'], comment='#')], sort=True)
+#     df['sessID'] = [x[0] for x in df.index]
+#     df['num_play'] = [x[1] for x in df.index]
+#     return df, metadata
+
+
+def get_lakeland_default_filter(lvlstart: Optional[int] = None, lvlend: Optional[bool] = None, no_debug: Optional[bool] = True,
+                                min_sessActiveEventCount: Optional[int] = 10,
+                                min_lvlstart_ActiveEventCount: Optional[int] = 3,
+                                min_lvlend_ActiveEventCount: Optional[int] = 3, min_sessDuration: Optional[int] = 300, max_sessDuration: Optional[int] = None, cont: Optional[bool] = False) -> List[str]:
+    """
+
+    :param lvlstart: levelstart to be used for other parameters (None if not used)
+    :param lvlend: levelend to be used for other parameters (None if not used)
+    :param no_debug: boolean whether or not to use only players that have used SPYPARTY or only not used SPYPARTY  (None if not used)
+    :param min_sessActiveEventCount:  (None if not used)
+    :param min_lvlstart_ActiveEventCount:  (None if not used)
+    :param min_lvlend_ActiveEventCount:  (None if not used)
+    :param min_sessDuration:  (None if not used)
+    :param max_sessDuration:  (None if not used)
+    :param cont:  (None if not used)
+    :return:
+    """
+    get_lakeland_default_filter()
+    query_list = []
+
+    if no_debug:
+        query_list.append('debug == 0')
+    if min_sessActiveEventCount is not None:
+        query_list.append(
+            f'sess_ActiveEventCount >= {min_sessActiveEventCount}')
+    if lvlstart is not None and min_lvlstart_ActiveEventCount is not None:
+        query_list.append(
+            f'lvl{lvlstart}_ActiveEventCount >= {min_lvlstart_ActiveEventCount}')
+    if lvlend is not None and min_lvlend_ActiveEventCount is not None:
+        query_list.append(
+            f'lvl{lvlend}_ActiveEventCount >= {min_lvlend_ActiveEventCount}')
+    if min_sessDuration is not None:
+        query_list.append(f'sessDuration >= {min_sessDuration}')
+    if max_sessDuration is not None:
+        query_list.append(f'sessDuration <= {max_sessDuration}')
+    if cont is not None:
+        query_list.append(f'_continue == {int(cont)}')
+
+    return query_list
+
+# def describe_lvl_feats_lakeland(df, fbase_list, lvl_range, level_time=300, level_overlap=30):
+#     """
+#     Calculates sum/avg of given level base features (fnames without lvlN_ prefix) in the level range.
+#     Will automatically filter out players who did not complete the given level range in the df
+#     May have a bug.
+
+#     :param level_time: number of seconds per level (window)
+#     :param level_overlap: number of overlap seconds per level (window)
+#     :rtype: (df, List[str]) where the new df includes sum_ and avg_lvl_A_to_B.
+#     :param df: dataframe to pull from and append to
+#     :param fbase_list: list of feature bases (fnames without lvlN_ prefix)
+#     :param lvl_range: range of levels to choose. typically range(min_level, max_level+1)
+#     """
+#     metadata = []
+#     metadata.append(f'*arg* lvlfeats = {fbase_list}')
+#     metadata.append(f'*arg* lvlrange = {lvl_range}')
+#     if not fbase_list:
+#         return df, metadata
+#     lvl_start, lvl_end = lvl_range[0], lvl_range[-1]
+#     query = f'sessDuration > {(level_time - level_overlap) * (lvl_end) + level_time}'
+#     df = df.query(query)
+#     metadata.append(
+#         f'Describe Level Feats lvls {lvl_start} to {lvl_end}. Assuming WINDOW_SIZE_SECONDS={level_time} and WINDOW_OVERLAP_SECONDS={level_overlap}, filtered by ({query})')
+#     fromlvl, tolvl = lvl_range[0], lvl_range[-1]
+#     sum_prefix = f'sum_lvl_{fromlvl}_to_{tolvl}_'
+#     avg_prefix = f'avg_lvl_{fromlvl}_to_{tolvl}_'
+#     for fn in fbase_list:
+#         tdf = df[[f'lvl{i}_{fn}' for i in lvl_range]].fillna(0).copy()
+#         df[sum_prefix + fn] = tdf.sum(axis=1)
+#         df[avg_prefix + fn] = tdf.mean(axis=1)
+#     return df, metadata
+
+def get_feat_selection_lakeland(df,  max_lvl=9):
+    """
+    Gets the feature selection widget.
+    :param df:
+    :param max_lvl:
+    :return:
+    """
+    start_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='Start Level:',
+                                    disabled=False, continuous_update=False, orientation='horizontal', readout=True, readout_format='d')
+    end_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='End Level:',
+                                  disabled=False, continuous_update=False, orientation='horizontal', readout=True, readout_format='d')
+    level_selection = widgets.GridBox([start_level, end_level])
+
+    def change_start_level(change):
+        end_level.min = start_level.value
+        if end_level.value < start_level.value:
+            end_level.value = start_level.value
+    start_level.observe(change_start_level, names="value")
+
+    lvl_feats = sorted(set([f[5:] for f in df.columns if f.startswith('lvl')]))
+    sess_feats = sorted(
+        set([f[5:] for f in df.columns if f.startswith('sess_')]))
+    other_feats = sorted(set([f for f in df.columns if not f.startswith(
+        'lvl') and not f.startswith('sess_')]))
+    selection_widget = widgets.GridBox([multi_checkbox_widget(lvl_feats, 'lvl'),
+                                        multi_checkbox_widget(
+                                            sess_feats, 'sess'),
+                                        multi_checkbox_widget(
+                                            other_feats, 'other'),
+                                        level_selection],
+                                       layout=widgets.Layout(grid_template_columns=f"repeat(3, 500px)"))
+
+    return selection_widget
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/WAVES/waves_utils.py` & `OGDUtils-0.1.5/src/OGDUtils/WAVES/waves_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-# standard library imports
-import sys
-import copy
-import pickle
-import os
-from collections import Counter
-from io import BytesIO
-from zipfile import ZipFile
-import copy
-import pickle
-from math import ceil
-import importlib
-import urllib.request
-
-# math imports
-from matplotlib import pyplot as plt
-import numpy as np
-import pandas as pd
-from scipy import stats
-import seaborn as sns
-sns.set()
-
-# google imports
-
-# Jupyter Imports
-from IPython.display import display
-import ipywidgets as widgets
-# from google.colab import files
-
-# ML imports
-# models
-from sklearn.naive_bayes import CategoricalNB
-from sklearn.tree import ExtraTreeClassifier, DecisionTreeClassifier
-from sklearn.neural_network import MLPClassifier
-from xgboost import XGBClassifier
-from sklearn.linear_model import RidgeCV, SGDRegressor
-from sklearn.svm import LinearSVR
-
-# preprocessing
-from sklearn.impute import SimpleImputer
-from sklearn.compose import ColumnTransformer
-from sklearn.preprocessing import StandardScaler, OneHotEncoder, KBinsDiscretizer
-from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
-from sklearn.model_selection import train_test_split
-
-# sampling
-from imblearn.over_sampling import RandomOverSampler
-from imblearn.under_sampling import RandomUnderSampler, EditedNearestNeighbours, RepeatedEditedNearestNeighbours
-from imblearn.combine import SMOTEENN, SMOTETomek
-
-# metrics
-from sklearn.metrics import confusion_matrix, classification_report
-from sklearn.metrics import plot_precision_recall_curve, plot_confusion_matrix, plot_roc_curve
-from sklearn.metrics import f1_score, roc_auc_score, roc_curve, accuracy_score
-
-# other
-from imblearn.pipeline import make_pipeline
-from sklearn.model_selection import GridSearchCV
-
-# custom imports
-import general.feature_utils as feat_util
-
-def get_feat_selection_waves(df, max_lvl=34):
-    """
-    Gets the feature selection widget.
-    :param df:
-    :param max_lvl:
-    :return:
-    """
-    start_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='Start Level:',
-                                    disabled=False, continuous_update=False, orientation='horizontal', readout=True,
-                                    readout_format='d')
-    end_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='End Level:',
-                                  disabled=False, continuous_update=False, orientation='horizontal', readout=True,
-                                  readout_format='d')
-    level_selection = widgets.GridBox([start_level, end_level])
-
-    def change_start_level(change):
-        end_level.min = start_level.value
-        if end_level.value < start_level.value:
-            end_level.value = start_level.value
-
-    start_level.observe(change_start_level, names="value")
-
-    lvl_feats = sorted(set([''.join(f.split('_')[1:])
-                            for f in df.columns if f.startswith('lvl')]))
-    sess_feats = sorted(
-        set([f[7:] for f in df.columns if f.startswith('session')]))
-    other_feats = sorted(set([f for f in df.columns if not f.startswith(
-        'lvl') and not f.startswith('session')]))
-    selection_widget = widgets.GridBox([multi_checkbox_widget(lvl_feats, 'lvl'),
-                                        multi_checkbox_widget(
-                                            sess_feats, 'sess'),
-                                        multi_checkbox_widget(
-                                            other_feats, 'other'),
-                                        level_selection],
-                                       layout=widgets.Layout(grid_template_columns=f"repeat(3, 500px)"))
-
-    return selection_widget
+# standard library imports
+import sys
+import copy
+import pickle
+import os
+from collections import Counter
+from io import BytesIO
+from zipfile import ZipFile
+import copy
+import pickle
+from math import ceil
+import importlib
+import urllib.request
+
+# math imports
+from matplotlib import pyplot as plt
+import numpy as np
+import pandas as pd
+from scipy import stats
+import seaborn as sns
+sns.set()
+
+# google imports
+
+# Jupyter Imports
+from IPython.display import display
+import ipywidgets as widgets
+# from google.colab import files
+
+# ML imports
+# models
+from sklearn.naive_bayes import CategoricalNB
+from sklearn.tree import ExtraTreeClassifier, DecisionTreeClassifier
+from sklearn.neural_network import MLPClassifier
+from xgboost import XGBClassifier
+from sklearn.linear_model import RidgeCV, SGDRegressor
+from sklearn.svm import LinearSVR
+
+# preprocessing
+from sklearn.impute import SimpleImputer
+from sklearn.compose import ColumnTransformer
+from sklearn.preprocessing import StandardScaler, OneHotEncoder, KBinsDiscretizer
+from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
+from sklearn.model_selection import train_test_split
+
+# sampling
+from imblearn.over_sampling import RandomOverSampler
+from imblearn.under_sampling import RandomUnderSampler, EditedNearestNeighbours, RepeatedEditedNearestNeighbours
+from imblearn.combine import SMOTEENN, SMOTETomek
+
+# metrics
+from sklearn.metrics import confusion_matrix, classification_report
+from sklearn.metrics import plot_precision_recall_curve, plot_confusion_matrix, plot_roc_curve
+from sklearn.metrics import f1_score, roc_auc_score, roc_curve, accuracy_score
+
+# other
+from imblearn.pipeline import make_pipeline
+from sklearn.model_selection import GridSearchCV
+
+# custom imports
+import general.feature_utils as feat_util
+
+def get_feat_selection_waves(df, max_lvl=34):
+    """
+    Gets the feature selection widget.
+    :param df:
+    :param max_lvl:
+    :return:
+    """
+    start_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='Start Level:',
+                                    disabled=False, continuous_update=False, orientation='horizontal', readout=True,
+                                    readout_format='d')
+    end_level = widgets.IntSlider(value=0, min=0, max=max_lvl, step=1, description='End Level:',
+                                  disabled=False, continuous_update=False, orientation='horizontal', readout=True,
+                                  readout_format='d')
+    level_selection = widgets.GridBox([start_level, end_level])
+
+    def change_start_level(change):
+        end_level.min = start_level.value
+        if end_level.value < start_level.value:
+            end_level.value = start_level.value
+
+    start_level.observe(change_start_level, names="value")
+
+    lvl_feats = sorted(set([''.join(f.split('_')[1:])
+                            for f in df.columns if f.startswith('lvl')]))
+    sess_feats = sorted(
+        set([f[7:] for f in df.columns if f.startswith('session')]))
+    other_feats = sorted(set([f for f in df.columns if not f.startswith(
+        'lvl') and not f.startswith('session')]))
+    selection_widget = widgets.GridBox([multi_checkbox_widget(lvl_feats, 'lvl'),
+                                        multi_checkbox_widget(
+                                            sess_feats, 'sess'),
+                                        multi_checkbox_widget(
+                                            other_feats, 'other'),
+                                        level_selection],
+                                       layout=widgets.Layout(grid_template_columns=f"repeat(3, 500px)"))
+
+    return selection_widget
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/general/FeatureSetOptions.py` & `OGDUtils-0.1.5/src/OGDUtils/general/FeatureSetOptions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from collections import namedtuple
-
-class FeatureSetOptions:
-    feature_set_options = namedtuple('FeatureSetOptions', ['game','name','filter_args','new_feat_args','lvlfeats','lvlrange','finalfeats','zthresh','finalfeats_readable'])
-    jowilder_demo_set = feature_set_options('jowilder',
-                              'demo',
-                              {'query_list':['sess_avg_num_tiles_hovered_before_placing_home > 1'],
-                               'verbose':False, 
-                               'fillna':0},
-                               {'avg_tile_hover_lvl_range': range(0,1)},
-                              ['count_buy_home', 'count_buy_farm','count_buy_livestock','count_buys'],
-                              range(0, 1),
-                              ['weighted_avg_lvl_0_to_0_avg_num_tiles_hovered_before_placing_farm',
-                                'sum_lvl_0_to_0_count_buy_home',
-                              'sum_lvl_0_to_0_count_buy_farm',
-                              'sum_lvl_0_to_0_count_buy_livestock',
-                              'sum_lvl_0_to_0_count_buys'],
-                              3,
-                              ['hovers\nbefore\nfarm','home','farm','livestock','buys']
+from collections import namedtuple
+
+class FeatureSetOptions:
+    feature_set_options = namedtuple('FeatureSetOptions', ['game','name','filter_args','new_feat_args','lvlfeats','lvlrange','finalfeats','zthresh','finalfeats_readable'])
+    jowilder_demo_set = feature_set_options('jowilder',
+                              'demo',
+                              {'query_list':['sess_avg_num_tiles_hovered_before_placing_home > 1'],
+                               'verbose':False, 
+                               'fillna':0},
+                               {'avg_tile_hover_lvl_range': range(0,1)},
+                              ['count_buy_home', 'count_buy_farm','count_buy_livestock','count_buys'],
+                              range(0, 1),
+                              ['weighted_avg_lvl_0_to_0_avg_num_tiles_hovered_before_placing_farm',
+                                'sum_lvl_0_to_0_count_buy_home',
+                              'sum_lvl_0_to_0_count_buy_farm',
+                              'sum_lvl_0_to_0_count_buy_livestock',
+                              'sum_lvl_0_to_0_count_buys'],
+                              3,
+                              ['hovers\nbefore\nfarm','home','farm','livestock','buys']
     )
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/general/Workflow.py` & `OGDUtils-0.1.5/src/OGDUtils/general/Workflow.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,501 +1,501 @@
-from typing import Optional
-from pathlib import Path
-from sklearn.decomposition import PCA
-from sklearn.manifold import TSNE
-from sklearn.cluster import KMeans, DBSCAN
-from sklearn.preprocessing import StandardScaler, RobustScaler, PowerTransformer, Normalizer, FunctionTransformer
-from sklearn.pipeline import make_pipeline
-from sklearn.metrics import silhouette_samples
-import matplotlib.pyplot as plt
-import matplotlib as mpl
-import seaborn
-import numpy as np
-import pandas as pd
-from math import pi
-import feature_utils as cu
-import os
-
-
-def df_np_df(func):
-    def convert_call_reconvert_df(self, df, *args, **kwargs):
-        nparray = df.to_numpy()
-        nparray, meta = func(self, nparray, *args, **kwargs)
-        assert nparray.shape[1] == len(df.columns)
-        return pd.DataFrame(nparray, columns=df.columns), meta
-
-    return convert_call_reconvert_df
-
-
-class Workflow:
-    # fields
-    DEFAULT_SCALE = "robust"
-    DEFAULT_PCA   = 2
-    DEFAULT_CLUSTERS = [3]
-    DEFAULT_CLUSTER_METHOD = "KMeans"
-
-    def __init__(self, init_df, import_meta, filter_options=None, base_output_dir=None, nested_folder_output=True):
-        self.further_filter_query_list = None
-        # utils.init_path()
-        self._df = init_df
-        self._df_import_meta = import_meta
-        self.filter_options = filter_options
-        self._nested_folder_output:bool = nested_folder_output
-        self._base_output_dir = base_output_dir
-
-        # flags
-        self.verbose = True
-
-        # steps
-        self.pre_histogram = True
-        self.do_logtransform = True
-        self.do_scaling = True
-        self.do_normalization = False
-        self.post_histogram = True
-        self.plot_correlation = True
-        self.do_PCA = True
-        self.plot_scree = True
-        self.do_clustering = True
-        self.plot_cluster_scatter = True
-        self.plot_silhouettes = True
-        self.plot_radars = True
-
-        # scikitlearn
-        self.outlier_method = None
-        self.scaling_method = Workflow.DEFAULT_SCALE
-        self.normalization_method = 'Normalizer'
-        self.pca_dimension_count = Workflow.DEFAULT_PCA
-        self.clustering_method = Workflow.DEFAULT_CLUSTER_METHOD
-        self.clustering_counts = Workflow.DEFAULT_CLUSTERS
-        self.clustering_count = self.clustering_counts[0]
-
-        # viz
-        self.color_dict = {i: v for i, v in enumerate(mpl.cm.get_cmap('tab10').colors)}
-        self.color_dict.update({10+i:mpl.cm.get_cmap('tab20').colors[2*i+1] for i in range(10) })
-        self.color_dict[-1] = (.2, .2, .2)
-        self.feature_names = None
-
-
-    def clustering_abbrev(self):
-        cluster_abbrev = 'k' if self.clustering_method is "KMeans" else self.clustering_method
-        return f'z{self.filter_options.zthresh}pca{self.pca_dimension_count}{cluster_abbrev}{self.clustering_count}'
-
-    def get_base_output_dir(self):
-        if self._base_output_dir:
-            save_dir = self._base_output_dir
-        else:
-            logtransform = '_logtransform' if self.do_logtransform else ''
-            clustering_suffix = '' if self._nested_folder_output else '_'+ self.clustering_abbrev()
-            suffix = f'{logtransform}{clustering_suffix}'
-            save_dir = os.path.join('Results',self.filter_options.game.lower().capitalize(), self.filter_options.name+suffix)
-        Path(save_dir).mkdir(parents=True, exist_ok=True)
-        return save_dir
-
-    def get_cluster_output_dir(self):
-        if not self._nested_folder_output:
-            save_dir = self.get_base_output_dir()
-        else:
-            save_dir = os.path.join(self.get_base_output_dir(), self.clustering_abbrev())
-        Path(save_dir).mkdir(parents=True, exist_ok=True)
-        return save_dir
-
-    def get_filename(self):
-        return None  # some_string
-
-    def query(self, df, query_list):
-        meta = []
-        for q in query_list:
-            df = df.query(q)
-            outstr = f'Query: {q}, output_shape: {df.shape}'
-            meta.append(outstr)
-
-        return df, meta
-
-    @staticmethod
-    def Histogram(df: pd.DataFrame, num_bins: Optional[int] = None, title: Optional[str] = None, log_scale=True, save=False, save_loc=None):
-        title = title or 'Histograms'
-        num_rows = len(df.index)
-        num_bins = num_bins or min(25, num_rows)
-
-        axes = df.plot(kind='hist', subplots=True, figsize=(20, 5), bins=num_bins,
-                       title=title, layout=(1, len(df.columns)), color='k', sharex=False,
-                       sharey=True, logy=log_scale, bottom=1)
-        # for axrow in axes:
-        #     for ax in axrow:
-        #         print(ax)
-        #         ax.set_yscale('log')
-        if save:
-            savepath = os.path.join(save_loc, f'{title}.png')
-            plt.savefig(savepath)
-            plt.close()
-
-    # TODO: Graph is part cut off, i think there might be some stuff hardcoded.
-    @staticmethod
-    def Correlations(df, heat_range=0.3, save=False, save_loc=None):
-        plt.figure()
-        seaborn.set(style="ticks")
-        corr = df.corr()
-        g = seaborn.heatmap(corr, vmax=heat_range, center=0,
-                            square=True, linewidths=.5, cbar_kws={"shrink": .5}, annot=True, fmt='.2f', cmap='coolwarm')
-        seaborn.despine()
-        g.figure.set_size_inches(14, 10)
-
-        title = 'Correlations'
-        if save:
-            savepath = os.path.join(save_loc, f'{title}.png')
-            g.figure.savefig(savepath)
-
-    @staticmethod
-    def LogTransformed(df):
-        meta = []
-        nparray = df.to_numpy()
-        nparray = np.log1p(nparray)
-        meta.append('LogTransform using np.long1p')
-        return pd.DataFrame(nparray, columns=df.columns), meta
-
-    # @df_np_df
-    @staticmethod
-    def Scaled(df, scaling_method:str = DEFAULT_SCALE):
-        meta = []
-        nparray = df.to_numpy()
-        if scaling_method == "Standard":
-            scaler = StandardScaler()
-        elif scaling_method == "Robust":
-            scaler = RobustScaler()
-        else:
-            scaler = None
-        meta.append(f'Scaled with scikitlearn {scaler}' )
-        nparray = scaler.fit_transform(nparray)
-        return pd.DataFrame(nparray, columns=df.columns), meta
-
-    # @df_np_df
-    @staticmethod
-    def Normalized(df):
-        meta = []
-        nparray = df.to_numpy()
-        normalizer = Normalizer()
-        meta.append(f'Normalized with scikitlearn {normalizer}')
-        nparray = normalizer.fit_transform(nparray)
-        return pd.DataFrame(nparray, columns=df.columns), meta
-
-    @staticmethod
-    def PCA(df, dimension_count:int = DEFAULT_PCA):
-        meta = []
-        nparray = df.to_numpy()
-        pca = PCA(n_components=dimension_count)
-        meta.append(f'PCA df calculated with scikitlearn {pca}')
-        nparray = pca.fit_transform(nparray)
-        PCA_names = [f"PCA_{i}" for i in range(dimension_count)]
-        return pd.DataFrame(nparray, columns=PCA_names), meta
-
-    @staticmethod
-    def PlotScree(df, save=False, save_loc=None):
-        nparray = df.to_numpy()
-        U, S, V = np.linalg.svd(nparray)
-        eigvals = S ** 2 / np.sum(S ** 2)
-        fig = plt.figure(figsize=(8, 5))
-        singular_vals = np.arange(nparray.shape[1]) + 1
-        plt.plot(singular_vals, eigvals, 'ro-', linewidth=2)
-        title = 'Scree Plot'
-        plt.title(title)
-        plt.xlabel('Principal Component')
-        plt.ylabel('Eigenvalue')
-
-        if save:
-            savepath = os.path.join(save_loc, f'{title}.png')
-            plt.savefig(savepath)
-            plt.close()
-        return
-
-    @staticmethod
-    def Cluster(df, cluster_count: int=DEFAULT_CLUSTERS[0], clustering_method=DEFAULT_CLUSTER_METHOD):
-        meta = []
-        nparray = df.to_numpy()
-        if clustering_method == "KMeans":
-            clusterer = KMeans(n_clusters=cluster_count)
-            # For future, include calculated distances.
-            # In the future, this will let us find centers:
-            # distances = clusterer.transform(nparray)
-            # nparray = np.concatenate((distances, labels))
-        # elif clustering_method == "FuzzyCMeans":
-        #     pass
-        elif clustering_method == "DBSCAN":
-            clusterer = DBSCAN(eps=0.3, min_samples=10)
-        else:
-            return [], meta
-        labels = clusterer.fit_predict(nparray)
-        meta.append(f'Labels calculated via clusterer: {clusterer}')
-        return labels, meta
-
-        # for a,l in zip(PCA_dims, labels):
-        #     b =  clustering.cluster_centers_[l]
-        #     distances.append(a-b)
-        # labels = labels
-        # df['PCA1 Offset'] = np.array(distances)[:,0]
-        # df['PCA2 Offset'] = np.array(distances)[:,1]
-
-    @staticmethod
-    def PlotSilhouettes(dimension_data: pd.DataFrame, labels: pd.DataFrame, title=None, clustering_abbrev=None, save=False, save_loc=None):
-        np_dimensions = dimension_data.to_numpy()
-        silhouette_vals = silhouette_samples(np_dimensions, labels)
-
-        # Silhouette plot
-        fig, ax1 = plt.subplots(1, 1)
-        fig.set_size_inches(18, 7)
-        y_ticks = []
-        y_lower, y_upper = 0, 0
-        for i, cluster in enumerate(np.unique(labels)):
-            cluster_silhouette_vals = silhouette_vals[labels == cluster]
-            cluster_silhouette_vals.sort()
-            y_upper += len(cluster_silhouette_vals)
-            ax1.barh(range(y_lower, y_upper), cluster_silhouette_vals, edgecolor='none', height=1)
-            ax1.text(-0.03, (y_lower + y_upper) / 2, str(i + 1))
-            y_lower += len(cluster_silhouette_vals)
-
-        # Get the average silhouette score and plot it
-        avg_score = np.mean(silhouette_vals)
-        ax1.axvline(avg_score, linestyle='--', linewidth=2, color='green')
-        ax1.set_yticks([])
-        ax1.set_xlim([-0.1, 1])
-        ax1.set_xlabel('Silhouette coefficient values')
-        ax1.set_ylabel('Cluster labels')
-        title = title or f'Silhouettes {clustering_abbrev} Avg={int(avg_score*100)}%'
-        ax1.set_title(title, y=1.02)
-        if save:
-            savepath = os.path.join(save_loc, f'{title}.png')
-            plt.savefig(savepath)
-            plt.close()
-
-        return
-
-    @staticmethod
-    def scatter(df, labels, color_dict, title='Scatter', save=False, save_loc=None):
-        num_cols = len(df.columns)
-        color_array = [color_dict[c] for c in labels]
-        fig, axs = plt.subplots(num_cols, num_cols, figsize=(30, 30))
-        for x in range(num_cols):
-            for y in range(num_cols):
-                axs[x, y].scatter(df.iloc[:, x], df.iloc[:, y], c=color_array)
-                axs[x, y].set_xlabel(df.columns[x])
-                axs[x, y].set_ylabel(df.columns[y])
-        if save:
-            savepath = os.path.join(save_loc, f'{title}.png')
-            plt.savefig(savepath)
-            plt.close()
-
-    @staticmethod
-    def radar_from_cluster_csv(csv_path, optionsgroup, savedir=None ):
-        print('here')
-        index_col = [0,1] if optionsgroup.game.upper() == 'LAKELAND' else 0
-        df = pd.read_csv(csv_path, index_col=index_col, comment='#')
-        labels = list(df['label'].to_numpy())
-        df = df.drop('label', axis=1)
-        w = Workflow(init_df=df, import_meta="", filter_options=optionsgroup)
-        w.radarCharts(df, labels, savedir=savedir)
-
-    def radarCharts(self, df, labels, save=True, savedir=None):
-        print('radarCharts')
-        categories = self.filter_options.finalfeats_readable
-        description_df = df.describe()
-        summary_df = pd.DataFrame(columns=description_df.columns)
-        clusters = set(labels)
-        cluster_dict = {}
-        for c in clusters:
-            cluster_dict[c] = df[labels == c]
-            cluster_df = cluster_dict[c].describe()
-            summary_df.loc[f'C{c}_zscore', :] = (cluster_df.loc['mean', :] - description_df.loc['mean', :]) / description_df.loc[
-                                                                                                       'std', :]
-            summary_df.loc[f'C{c}_%mean', :] = (cluster_df.loc['mean', :] / description_df.loc['mean', :]) * 100
-            summary_df.loc[f'C{c}_%std', :] = (cluster_df.loc['std', :] / description_df.loc['std', :]) * 100
-        summary_df = summary_df.apply(lambda x: (x * 100) // 1 * .01)
-
-        def make_spider(color, i):
-            offset = .25 * pi
-            # What will be the angle of each axis in the plot? (we divide the plot / number of variable)
-            angles = [n / float(N) * 2 * pi + offset for n in range(N)]
-            angles += angles[:1]
-            ax = plt.subplot(nrows, ncols, i + 1, polar=True)
-            plt.xticks(angles[:-1], categories, color='grey', size=12)
-            ax.set_rlabel_position(0)
-            if var == 'zscore':
-                plt.yticks([-2, -1, 0, 1, 2], color="grey", size=7)
-                plt.ylim(-2, 2)
-            elif '%' in var:
-                plt.yticks(range(0, 1000, 100), color="grey", size=7)
-                plt.ylim(0, 400)
-            values = list(tdf.iloc[i, :])
-            values += values[:1]
-            graph_name = tdf.index[i]
-            ax.plot(angles, values, color=color, linewidth=2, linestyle='solid')
-            ax.fill(angles, values, color=color, alpha=0.4)
-            plt.title(f'Cluster {i} (n={len(cluster_dict[i])})', size=11, color=color, y=1.1)
-
-        # number of variable
-        for var in ['zscore', '%mean', '%std']:
-            tdf = summary_df.loc[[idx for idx in summary_df.index if var in idx], :]
-            if not categories:
-                categories = list(tdf.columns)
-            N = len(categories)
-            num_groups = len(tdf.index)
-            #   nrows = 2
-            #   ncols = num_groups//2 if not num_groups%2 else num_groups//2 + 1
-            nrows = 1
-            ncols = num_groups
-            fig = plt.figure(figsize=(20, 5))
-            fig.suptitle(f'{var} Radar Charts')
-            for i in range(num_groups):
-                make_spider(self.color_dict[i], i)
-            fig.subplots_adjust(wspace=0.4)
-            if save:
-                plt.savefig(os.path.join(self.get_cluster_output_dir(),f'radar_{var}.png'))
-                plt.close()
-        pass
-
-    def save_csv_and_meta(self, df, meta_list, save_dir, csv_name, meta_name=None, permissions='w+'):
-        if csv_name.endswith(('.tsv', '.csv')):
-            extension = csv_name[-4:]
-            csv_name = csv_name[:-4]
-        else:
-            extension = '.csv'
-        separator = '\t' if extension == '.tsv' else ','
-        meta_name = meta_name or csv_name+ '_meta.txt'
-        meta_text = 'Metadata:\n'+'\n'.join(meta_list)
-        with open(os.path.join(save_dir, meta_name), permissions) as f:
-            f.write(meta_text)
-        with open(os.path.join(save_dir, csv_name)+extension, permissions) as f:
-            for l in meta_text.splitlines():
-                f.write(f'# {l}\n')
-            f.write('\n')
-            df.to_csv(f, sep=separator)
-
-        return None, []
-
-    def RunWorkflow(self):
-        def requestPCADims():
-            inp = input('pca dims? ')
-            try:
-                self.pca_dimension_count = int(inp.strip())
-            except:
-                pass
-        def requestClusterCount():
-            inp = input('k? ')
-            try:
-                self.clustering_counts = [int(inp.strip())]
-            except:
-                pass
-
-        if self.verbose:
-            print('Starting workflow.')
-            print('Saving to:', self.get_base_output_dir())
-        original_df, meta = cu.full_filter(df=self._df, import_meta=self._df_import_meta, options=self.filter_options, outpath=self.get_base_output_dir())
-        if self.further_filter_query_list is not None:
-            original_df, md = self.query(original_df, self.further_filter_query_list)
-            meta.extend(md)
-        self.save_csv_and_meta(original_df, meta, self.get_base_output_dir(), 'filtered_data')
-        working_df = original_df.copy()
-        original_cols = list(working_df.columns)
-
-        print(f"Ok, we've done the filtering and such, time to get a random sample of session ids. First, let's check the start")
-        print(working_df.head())
-        print("alright, now on to the actual sample:")
-        subsample = working_df.sample(n=26)
-        print(subsample.head(26))
-
-
-        # Preprocessing - LogTransform, Scaling, Normalization #
-        # show working_df before any processing
-
-        if self.pre_histogram:
-            Workflow.Histogram(working_df, title='Raw Histogram', save=True, save_loc=self.get_base_output_dir())
-        # do log transform
-        if self.do_logtransform:
-            working_df, md = Workflow.LogTransformed(working_df)
-            meta.extend(md)
-        # scale working_df
-        if self.do_scaling:
-            working_df, md = Workflow.Scaled(working_df, self.scaling_method)
-            meta.extend(md)
-        # do normalization
-        if self.do_normalization:
-            working_df, md = Workflow.Normalized(working_df)
-            meta.extend(md)
-        # show working_df after transformation
-        if self.post_histogram:
-            Workflow.Histogram(working_df, title='Preprocessed Histogram', save=True, save_loc=self.get_base_output_dir())
-
-        # correlation
-        if self.plot_correlation:
-            Workflow.Correlations(working_df, save=True, save_loc=self.get_base_output_dir())
-
-        # scree and PCA
-        if self.plot_scree:
-            Workflow.PlotScree(working_df, save=True, save_loc=self.get_base_output_dir())
-        if self.do_PCA:
-            while self.pca_dimension_count is None:
-                requestPCADims()
-            if self.verbose:
-                print('Starting PCA.')
-            pca_df, md = Workflow.PCA(working_df, self.pca_dimension_count)
-            meta.extend(md)
-            cluster_df = pca_df
-            meta.append('Cluster on PCA dims')
-        else:
-            cluster_df = working_df
-            meta.append('Cluster on non-PCA dims')
-
-        # silhouette and clustering
-        if self.do_clustering:
-            while self.clustering_counts is None:
-                requestClusterCount()
-            for cluster_count in self.clustering_counts:
-                self.clustering_count = cluster_count
-                if self.verbose:
-                    print(f'Starting clustering k={self.clustering_count}')
-                labels, md = Workflow.Cluster(cluster_df, clustering_method=self.clustering_method, cluster_count=cluster_count)
-                meta.extend(md)
-
-                if self.plot_silhouettes:
-                    Workflow.PlotSilhouettes(cluster_df, labels, save=True, save_loc=self.get_base_output_dir())
-                if self.plot_cluster_scatter:
-                    Workflow.scatter(pca_df, [0]*len(labels), color_dict=self.color_dict, title='PCA No Label Scatter', save=True, save_loc=self.get_base_output_dir())
-                    Workflow.scatter(working_df, labels, color_dict=self.color_dict, title='Preprocessed Scatter', save=True, save_loc=self.get_base_output_dir())
-                    Workflow.scatter(pca_df, labels, color_dict=self.color_dict, title=f'PCA Scatter', save=True, save_loc=self.get_base_output_dir())
-                    Workflow.scatter(original_df, labels, color_dict=self.color_dict, title='Raw Scatter', save=True, save_loc=self.get_base_output_dir())
-
-                if self.plot_radars:
-                    self.radarCharts(original_df, labels)
-                self.save_csv_and_meta(cluster_df, meta, self.get_cluster_output_dir(), 'data_clustered_on')
-                original_df['label'] = labels
-                self.save_csv_and_meta(original_df, meta, self.get_cluster_output_dir(), 'clusters')
-                original_df = original_df.drop('label', axis=1)
-
-        return working_df, meta
-
-
-
-
-def add_cluster_features_to_df(pipeline, df, data):
-    pipeline.fit(data)
-    PCA_dims = pipeline[:-1].transform(data)
-    clustering = pipeline[-1]
-    labels = clustering.predict(PCA_dims)
-    distances = []
-    for a, l in zip(PCA_dims, labels):
-        b = clustering.cluster_centers_[l]
-        distances.append(a - b)
-    labels = labels
-    df['PCA1 Offset'] = np.array(distances)[:, 0]
-    df['PCA2 Offset'] = np.array(distances)[:, 1]
-
-
-# def main():
-    # utils.init_path()
-    # filter_options = cu.options.lakeland_actions_lvl01
-    # output_foler = r'G:\My Drive\Field Day\Research and Writing Projects\2020 CHI Play - Lakeland Clustering\Jupyter\Results\Lakeland\test'
-    # df_getter = cu.getLakelandDecJanLogDF
-
-    # w = Workflow(filter_options=filter_options, base_output_dir=output_foler)
-    # w.RunWorkflow(get_df_func=df_getter)
-
-
-# if __name__ == '__main__':
-#     main()
+from typing import Optional
+from pathlib import Path
+from sklearn.decomposition import PCA
+from sklearn.manifold import TSNE
+from sklearn.cluster import KMeans, DBSCAN
+from sklearn.preprocessing import StandardScaler, RobustScaler, PowerTransformer, Normalizer, FunctionTransformer
+from sklearn.pipeline import make_pipeline
+from sklearn.metrics import silhouette_samples
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+import seaborn
+import numpy as np
+import pandas as pd
+from math import pi
+import feature_utils as cu
+import os
+
+
+def df_np_df(func):
+    def convert_call_reconvert_df(self, df, *args, **kwargs):
+        nparray = df.to_numpy()
+        nparray, meta = func(self, nparray, *args, **kwargs)
+        assert nparray.shape[1] == len(df.columns)
+        return pd.DataFrame(nparray, columns=df.columns), meta
+
+    return convert_call_reconvert_df
+
+
+class Workflow:
+    # fields
+    DEFAULT_SCALE = "robust"
+    DEFAULT_PCA   = 2
+    DEFAULT_CLUSTERS = [3]
+    DEFAULT_CLUSTER_METHOD = "KMeans"
+
+    def __init__(self, init_df, import_meta, filter_options=None, base_output_dir=None, nested_folder_output=True):
+        self.further_filter_query_list = None
+        # utils.init_path()
+        self._df = init_df
+        self._df_import_meta = import_meta
+        self.filter_options = filter_options
+        self._nested_folder_output:bool = nested_folder_output
+        self._base_output_dir = base_output_dir
+
+        # flags
+        self.verbose = True
+
+        # steps
+        self.pre_histogram = True
+        self.do_logtransform = True
+        self.do_scaling = True
+        self.do_normalization = False
+        self.post_histogram = True
+        self.plot_correlation = True
+        self.do_PCA = True
+        self.plot_scree = True
+        self.do_clustering = True
+        self.plot_cluster_scatter = True
+        self.plot_silhouettes = True
+        self.plot_radars = True
+
+        # scikitlearn
+        self.outlier_method = None
+        self.scaling_method = Workflow.DEFAULT_SCALE
+        self.normalization_method = 'Normalizer'
+        self.pca_dimension_count = Workflow.DEFAULT_PCA
+        self.clustering_method = Workflow.DEFAULT_CLUSTER_METHOD
+        self.clustering_counts = Workflow.DEFAULT_CLUSTERS
+        self.clustering_count = self.clustering_counts[0]
+
+        # viz
+        self.color_dict = {i: v for i, v in enumerate(mpl.cm.get_cmap('tab10').colors)}
+        self.color_dict.update({10+i:mpl.cm.get_cmap('tab20').colors[2*i+1] for i in range(10) })
+        self.color_dict[-1] = (.2, .2, .2)
+        self.feature_names = None
+
+
+    def clustering_abbrev(self):
+        cluster_abbrev = 'k' if self.clustering_method is "KMeans" else self.clustering_method
+        return f'z{self.filter_options.zthresh}pca{self.pca_dimension_count}{cluster_abbrev}{self.clustering_count}'
+
+    def get_base_output_dir(self):
+        if self._base_output_dir:
+            save_dir = self._base_output_dir
+        else:
+            logtransform = '_logtransform' if self.do_logtransform else ''
+            clustering_suffix = '' if self._nested_folder_output else '_'+ self.clustering_abbrev()
+            suffix = f'{logtransform}{clustering_suffix}'
+            save_dir = os.path.join('Results',self.filter_options.game.lower().capitalize(), self.filter_options.name+suffix)
+        Path(save_dir).mkdir(parents=True, exist_ok=True)
+        return save_dir
+
+    def get_cluster_output_dir(self):
+        if not self._nested_folder_output:
+            save_dir = self.get_base_output_dir()
+        else:
+            save_dir = os.path.join(self.get_base_output_dir(), self.clustering_abbrev())
+        Path(save_dir).mkdir(parents=True, exist_ok=True)
+        return save_dir
+
+    def get_filename(self):
+        return None  # some_string
+
+    def query(self, df, query_list):
+        meta = []
+        for q in query_list:
+            df = df.query(q)
+            outstr = f'Query: {q}, output_shape: {df.shape}'
+            meta.append(outstr)
+
+        return df, meta
+
+    @staticmethod
+    def Histogram(df: pd.DataFrame, num_bins: Optional[int] = None, title: Optional[str] = None, log_scale=True, save=False, save_loc=None):
+        title = title or 'Histograms'
+        num_rows = len(df.index)
+        num_bins = num_bins or min(25, num_rows)
+
+        axes = df.plot(kind='hist', subplots=True, figsize=(20, 5), bins=num_bins,
+                       title=title, layout=(1, len(df.columns)), color='k', sharex=False,
+                       sharey=True, logy=log_scale, bottom=1)
+        # for axrow in axes:
+        #     for ax in axrow:
+        #         print(ax)
+        #         ax.set_yscale('log')
+        if save:
+            savepath = os.path.join(save_loc, f'{title}.png')
+            plt.savefig(savepath)
+            plt.close()
+
+    # TODO: Graph is part cut off, i think there might be some stuff hardcoded.
+    @staticmethod
+    def Correlations(df, heat_range=0.3, save=False, save_loc=None):
+        plt.figure()
+        seaborn.set(style="ticks")
+        corr = df.corr()
+        g = seaborn.heatmap(corr, vmax=heat_range, center=0,
+                            square=True, linewidths=.5, cbar_kws={"shrink": .5}, annot=True, fmt='.2f', cmap='coolwarm')
+        seaborn.despine()
+        g.figure.set_size_inches(14, 10)
+
+        title = 'Correlations'
+        if save:
+            savepath = os.path.join(save_loc, f'{title}.png')
+            g.figure.savefig(savepath)
+
+    @staticmethod
+    def LogTransformed(df):
+        meta = []
+        nparray = df.to_numpy()
+        nparray = np.log1p(nparray)
+        meta.append('LogTransform using np.long1p')
+        return pd.DataFrame(nparray, columns=df.columns), meta
+
+    # @df_np_df
+    @staticmethod
+    def Scaled(df, scaling_method:str = DEFAULT_SCALE):
+        meta = []
+        nparray = df.to_numpy()
+        if scaling_method == "Standard":
+            scaler = StandardScaler()
+        elif scaling_method == "Robust":
+            scaler = RobustScaler()
+        else:
+            scaler = None
+        meta.append(f'Scaled with scikitlearn {scaler}' )
+        nparray = scaler.fit_transform(nparray)
+        return pd.DataFrame(nparray, columns=df.columns), meta
+
+    # @df_np_df
+    @staticmethod
+    def Normalized(df):
+        meta = []
+        nparray = df.to_numpy()
+        normalizer = Normalizer()
+        meta.append(f'Normalized with scikitlearn {normalizer}')
+        nparray = normalizer.fit_transform(nparray)
+        return pd.DataFrame(nparray, columns=df.columns), meta
+
+    @staticmethod
+    def PCA(df, dimension_count:int = DEFAULT_PCA):
+        meta = []
+        nparray = df.to_numpy()
+        pca = PCA(n_components=dimension_count)
+        meta.append(f'PCA df calculated with scikitlearn {pca}')
+        nparray = pca.fit_transform(nparray)
+        PCA_names = [f"PCA_{i}" for i in range(dimension_count)]
+        return pd.DataFrame(nparray, columns=PCA_names), meta
+
+    @staticmethod
+    def PlotScree(df, save=False, save_loc=None):
+        nparray = df.to_numpy()
+        U, S, V = np.linalg.svd(nparray)
+        eigvals = S ** 2 / np.sum(S ** 2)
+        fig = plt.figure(figsize=(8, 5))
+        singular_vals = np.arange(nparray.shape[1]) + 1
+        plt.plot(singular_vals, eigvals, 'ro-', linewidth=2)
+        title = 'Scree Plot'
+        plt.title(title)
+        plt.xlabel('Principal Component')
+        plt.ylabel('Eigenvalue')
+
+        if save:
+            savepath = os.path.join(save_loc, f'{title}.png')
+            plt.savefig(savepath)
+            plt.close()
+        return
+
+    @staticmethod
+    def Cluster(df, cluster_count: int=DEFAULT_CLUSTERS[0], clustering_method=DEFAULT_CLUSTER_METHOD):
+        meta = []
+        nparray = df.to_numpy()
+        if clustering_method == "KMeans":
+            clusterer = KMeans(n_clusters=cluster_count)
+            # For future, include calculated distances.
+            # In the future, this will let us find centers:
+            # distances = clusterer.transform(nparray)
+            # nparray = np.concatenate((distances, labels))
+        # elif clustering_method == "FuzzyCMeans":
+        #     pass
+        elif clustering_method == "DBSCAN":
+            clusterer = DBSCAN(eps=0.3, min_samples=10)
+        else:
+            return [], meta
+        labels = clusterer.fit_predict(nparray)
+        meta.append(f'Labels calculated via clusterer: {clusterer}')
+        return labels, meta
+
+        # for a,l in zip(PCA_dims, labels):
+        #     b =  clustering.cluster_centers_[l]
+        #     distances.append(a-b)
+        # labels = labels
+        # df['PCA1 Offset'] = np.array(distances)[:,0]
+        # df['PCA2 Offset'] = np.array(distances)[:,1]
+
+    @staticmethod
+    def PlotSilhouettes(dimension_data: pd.DataFrame, labels: pd.DataFrame, title=None, clustering_abbrev=None, save=False, save_loc=None):
+        np_dimensions = dimension_data.to_numpy()
+        silhouette_vals = silhouette_samples(np_dimensions, labels)
+
+        # Silhouette plot
+        fig, ax1 = plt.subplots(1, 1)
+        fig.set_size_inches(18, 7)
+        y_ticks = []
+        y_lower, y_upper = 0, 0
+        for i, cluster in enumerate(np.unique(labels)):
+            cluster_silhouette_vals = silhouette_vals[labels == cluster]
+            cluster_silhouette_vals.sort()
+            y_upper += len(cluster_silhouette_vals)
+            ax1.barh(range(y_lower, y_upper), cluster_silhouette_vals, edgecolor='none', height=1)
+            ax1.text(-0.03, (y_lower + y_upper) / 2, str(i + 1))
+            y_lower += len(cluster_silhouette_vals)
+
+        # Get the average silhouette score and plot it
+        avg_score = np.mean(silhouette_vals)
+        ax1.axvline(avg_score, linestyle='--', linewidth=2, color='green')
+        ax1.set_yticks([])
+        ax1.set_xlim([-0.1, 1])
+        ax1.set_xlabel('Silhouette coefficient values')
+        ax1.set_ylabel('Cluster labels')
+        title = title or f'Silhouettes {clustering_abbrev} Avg={int(avg_score*100)}%'
+        ax1.set_title(title, y=1.02)
+        if save:
+            savepath = os.path.join(save_loc, f'{title}.png')
+            plt.savefig(savepath)
+            plt.close()
+
+        return
+
+    @staticmethod
+    def scatter(df, labels, color_dict, title='Scatter', save=False, save_loc=None):
+        num_cols = len(df.columns)
+        color_array = [color_dict[c] for c in labels]
+        fig, axs = plt.subplots(num_cols, num_cols, figsize=(30, 30))
+        for x in range(num_cols):
+            for y in range(num_cols):
+                axs[x, y].scatter(df.iloc[:, x], df.iloc[:, y], c=color_array)
+                axs[x, y].set_xlabel(df.columns[x])
+                axs[x, y].set_ylabel(df.columns[y])
+        if save:
+            savepath = os.path.join(save_loc, f'{title}.png')
+            plt.savefig(savepath)
+            plt.close()
+
+    @staticmethod
+    def radar_from_cluster_csv(csv_path, optionsgroup, savedir=None ):
+        print('here')
+        index_col = [0,1] if optionsgroup.game.upper() == 'LAKELAND' else 0
+        df = pd.read_csv(csv_path, index_col=index_col, comment='#')
+        labels = list(df['label'].to_numpy())
+        df = df.drop('label', axis=1)
+        w = Workflow(init_df=df, import_meta="", filter_options=optionsgroup)
+        w.radarCharts(df, labels, savedir=savedir)
+
+    def radarCharts(self, df, labels, save=True, savedir=None):
+        print('radarCharts')
+        categories = self.filter_options.finalfeats_readable
+        description_df = df.describe()
+        summary_df = pd.DataFrame(columns=description_df.columns)
+        clusters = set(labels)
+        cluster_dict = {}
+        for c in clusters:
+            cluster_dict[c] = df[labels == c]
+            cluster_df = cluster_dict[c].describe()
+            summary_df.loc[f'C{c}_zscore', :] = (cluster_df.loc['mean', :] - description_df.loc['mean', :]) / description_df.loc[
+                                                                                                       'std', :]
+            summary_df.loc[f'C{c}_%mean', :] = (cluster_df.loc['mean', :] / description_df.loc['mean', :]) * 100
+            summary_df.loc[f'C{c}_%std', :] = (cluster_df.loc['std', :] / description_df.loc['std', :]) * 100
+        summary_df = summary_df.apply(lambda x: (x * 100) // 1 * .01)
+
+        def make_spider(color, i):
+            offset = .25 * pi
+            # What will be the angle of each axis in the plot? (we divide the plot / number of variable)
+            angles = [n / float(N) * 2 * pi + offset for n in range(N)]
+            angles += angles[:1]
+            ax = plt.subplot(nrows, ncols, i + 1, polar=True)
+            plt.xticks(angles[:-1], categories, color='grey', size=12)
+            ax.set_rlabel_position(0)
+            if var == 'zscore':
+                plt.yticks([-2, -1, 0, 1, 2], color="grey", size=7)
+                plt.ylim(-2, 2)
+            elif '%' in var:
+                plt.yticks(range(0, 1000, 100), color="grey", size=7)
+                plt.ylim(0, 400)
+            values = list(tdf.iloc[i, :])
+            values += values[:1]
+            graph_name = tdf.index[i]
+            ax.plot(angles, values, color=color, linewidth=2, linestyle='solid')
+            ax.fill(angles, values, color=color, alpha=0.4)
+            plt.title(f'Cluster {i} (n={len(cluster_dict[i])})', size=11, color=color, y=1.1)
+
+        # number of variable
+        for var in ['zscore', '%mean', '%std']:
+            tdf = summary_df.loc[[idx for idx in summary_df.index if var in idx], :]
+            if not categories:
+                categories = list(tdf.columns)
+            N = len(categories)
+            num_groups = len(tdf.index)
+            #   nrows = 2
+            #   ncols = num_groups//2 if not num_groups%2 else num_groups//2 + 1
+            nrows = 1
+            ncols = num_groups
+            fig = plt.figure(figsize=(20, 5))
+            fig.suptitle(f'{var} Radar Charts')
+            for i in range(num_groups):
+                make_spider(self.color_dict[i], i)
+            fig.subplots_adjust(wspace=0.4)
+            if save:
+                plt.savefig(os.path.join(self.get_cluster_output_dir(),f'radar_{var}.png'))
+                plt.close()
+        pass
+
+    def save_csv_and_meta(self, df, meta_list, save_dir, csv_name, meta_name=None, permissions='w+'):
+        if csv_name.endswith(('.tsv', '.csv')):
+            extension = csv_name[-4:]
+            csv_name = csv_name[:-4]
+        else:
+            extension = '.csv'
+        separator = '\t' if extension == '.tsv' else ','
+        meta_name = meta_name or csv_name+ '_meta.txt'
+        meta_text = 'Metadata:\n'+'\n'.join(meta_list)
+        with open(os.path.join(save_dir, meta_name), permissions) as f:
+            f.write(meta_text)
+        with open(os.path.join(save_dir, csv_name)+extension, permissions) as f:
+            for l in meta_text.splitlines():
+                f.write(f'# {l}\n')
+            f.write('\n')
+            df.to_csv(f, sep=separator)
+
+        return None, []
+
+    def RunWorkflow(self):
+        def requestPCADims():
+            inp = input('pca dims? ')
+            try:
+                self.pca_dimension_count = int(inp.strip())
+            except:
+                pass
+        def requestClusterCount():
+            inp = input('k? ')
+            try:
+                self.clustering_counts = [int(inp.strip())]
+            except:
+                pass
+
+        if self.verbose:
+            print('Starting workflow.')
+            print('Saving to:', self.get_base_output_dir())
+        original_df, meta = cu.full_filter(df=self._df, import_meta=self._df_import_meta, options=self.filter_options, outpath=self.get_base_output_dir())
+        if self.further_filter_query_list is not None:
+            original_df, md = self.query(original_df, self.further_filter_query_list)
+            meta.extend(md)
+        self.save_csv_and_meta(original_df, meta, self.get_base_output_dir(), 'filtered_data')
+        working_df = original_df.copy()
+        original_cols = list(working_df.columns)
+
+        print(f"Ok, we've done the filtering and such, time to get a random sample of session ids. First, let's check the start")
+        print(working_df.head())
+        print("alright, now on to the actual sample:")
+        subsample = working_df.sample(n=26)
+        print(subsample.head(26))
+
+
+        # Preprocessing - LogTransform, Scaling, Normalization #
+        # show working_df before any processing
+
+        if self.pre_histogram:
+            Workflow.Histogram(working_df, title='Raw Histogram', save=True, save_loc=self.get_base_output_dir())
+        # do log transform
+        if self.do_logtransform:
+            working_df, md = Workflow.LogTransformed(working_df)
+            meta.extend(md)
+        # scale working_df
+        if self.do_scaling:
+            working_df, md = Workflow.Scaled(working_df, self.scaling_method)
+            meta.extend(md)
+        # do normalization
+        if self.do_normalization:
+            working_df, md = Workflow.Normalized(working_df)
+            meta.extend(md)
+        # show working_df after transformation
+        if self.post_histogram:
+            Workflow.Histogram(working_df, title='Preprocessed Histogram', save=True, save_loc=self.get_base_output_dir())
+
+        # correlation
+        if self.plot_correlation:
+            Workflow.Correlations(working_df, save=True, save_loc=self.get_base_output_dir())
+
+        # scree and PCA
+        if self.plot_scree:
+            Workflow.PlotScree(working_df, save=True, save_loc=self.get_base_output_dir())
+        if self.do_PCA:
+            while self.pca_dimension_count is None:
+                requestPCADims()
+            if self.verbose:
+                print('Starting PCA.')
+            pca_df, md = Workflow.PCA(working_df, self.pca_dimension_count)
+            meta.extend(md)
+            cluster_df = pca_df
+            meta.append('Cluster on PCA dims')
+        else:
+            cluster_df = working_df
+            meta.append('Cluster on non-PCA dims')
+
+        # silhouette and clustering
+        if self.do_clustering:
+            while self.clustering_counts is None:
+                requestClusterCount()
+            for cluster_count in self.clustering_counts:
+                self.clustering_count = cluster_count
+                if self.verbose:
+                    print(f'Starting clustering k={self.clustering_count}')
+                labels, md = Workflow.Cluster(cluster_df, clustering_method=self.clustering_method, cluster_count=cluster_count)
+                meta.extend(md)
+
+                if self.plot_silhouettes:
+                    Workflow.PlotSilhouettes(cluster_df, labels, save=True, save_loc=self.get_base_output_dir())
+                if self.plot_cluster_scatter:
+                    Workflow.scatter(pca_df, [0]*len(labels), color_dict=self.color_dict, title='PCA No Label Scatter', save=True, save_loc=self.get_base_output_dir())
+                    Workflow.scatter(working_df, labels, color_dict=self.color_dict, title='Preprocessed Scatter', save=True, save_loc=self.get_base_output_dir())
+                    Workflow.scatter(pca_df, labels, color_dict=self.color_dict, title=f'PCA Scatter', save=True, save_loc=self.get_base_output_dir())
+                    Workflow.scatter(original_df, labels, color_dict=self.color_dict, title='Raw Scatter', save=True, save_loc=self.get_base_output_dir())
+
+                if self.plot_radars:
+                    self.radarCharts(original_df, labels)
+                self.save_csv_and_meta(cluster_df, meta, self.get_cluster_output_dir(), 'data_clustered_on')
+                original_df['label'] = labels
+                self.save_csv_and_meta(original_df, meta, self.get_cluster_output_dir(), 'clusters')
+                original_df = original_df.drop('label', axis=1)
+
+        return working_df, meta
+
+
+
+
+def add_cluster_features_to_df(pipeline, df, data):
+    pipeline.fit(data)
+    PCA_dims = pipeline[:-1].transform(data)
+    clustering = pipeline[-1]
+    labels = clustering.predict(PCA_dims)
+    distances = []
+    for a, l in zip(PCA_dims, labels):
+        b = clustering.cluster_centers_[l]
+        distances.append(a - b)
+    labels = labels
+    df['PCA1 Offset'] = np.array(distances)[:, 0]
+    df['PCA2 Offset'] = np.array(distances)[:, 1]
+
+
+# def main():
+    # utils.init_path()
+    # filter_options = cu.options.lakeland_actions_lvl01
+    # output_foler = r'G:\My Drive\Field Day\Research and Writing Projects\2020 CHI Play - Lakeland Clustering\Jupyter\Results\Lakeland\test'
+    # df_getter = cu.getLakelandDecJanLogDF
+
+    # w = Workflow(filter_options=filter_options, base_output_dir=output_foler)
+    # w.RunWorkflow(get_df_func=df_getter)
+
+
+# if __name__ == '__main__':
+#     main()
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/general/feature_utils.py` & `OGDUtils-0.1.5/src/OGDUtils/general/feature_utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,616 +1,616 @@
-"""
-Note: Utils in this file are 
-
-Usage:
-If the first cell ran correctly, changing the CWD to the Jupyter file and adding '.' to sys path, then.
-import Notebooks.Clustering.cluster_utils as cu
-
-Otherwise:
-from google.colab import drive
-drive.mount('/content/drive')
-
-import os
-FIELDDAY_DIR = '/content/drive/My Drive/Field Day' # the field day directory on the mounted drive
-JUPYTER_DIR = os.path.join(FIELDDAY_DIR,'Research and Writing Projects/2020 Lakeland EDM/Jupyter')
-os.chdir(JUPYTER_DIR)
-
-import sys
-sys.path.append('.')
-import Notebooks.Clustering.cluster_utils as cu
-
-"""
-import copy
-import os
-import numpy as np
-import pandas as pd
-import seaborn as sns
-sns.set()
-import ipywidgets as widgets
-from matplotlib import pyplot as plt
-from scipy import stats
-from typing import Iterable, Optional, List, Tuple, Union
-from sklearn.metrics import confusion_matrix
-from sklearn.metrics import f1_score, roc_auc_score, accuracy_score
-from datetime import datetime
-import pickle
-from collections import Counter
-
-
-
-def print_options(meta):
-    """
-    Takes in meta text and outputs text for an options group.
-    :param meta: meta text. Expected format will be like:
-
-        Metadata:
-        Import from fhttps://opengamedata.fielddaylab.wisc.edu/data/LAKELAND/LAKELAND_20191201_to_20191231_de09c18_proc.zip
-        Import from fData/Raw Log Data/LAKELAND_20200101_to_20200131_a9720c1_proc.zip
-        *arg* filter_args = {'query_list': ['debug == 0', 'sess_ActiveEventCount >= 10', 'sessDuration >= 300', '_continue == 0'], 'one_query': False, 'fillna': 0, 'verbose': True}
-        Query: Intial Shape, output_shape: (32227, 1647)
-        Query: debug == 0, output_shape: (32221, 1647)
-        Query: sess_ActiveEventCount >= 10, output_shape: (26934, 1647)
-        Query: sessDuration >= 300, output_shape: (16109, 1647)
-        Query: _continue == 0, output_shape: (10591, 1647)
-        Filled NaN with 0
-        *arg* new_feat_args = {'verbose': False, 'avg_tile_hover_lvl_range': None}
-        *arg* lvlfeats = ['count_blooms', 'count_deaths', 'count_farmfails', 'count_food_produced', 'count_milk_produced']
-        *arg* lvlrange = range(0, 2)
-        Describe Level Feats lvls 0 to 1. Assuming WINDOW_SIZE_SECONDS=300 and WINDOW_OVERLAP_SECONDS=30, filtered by (sessDuration > 570)
-        *arg* finalfeats = ['avg_lvl_0_to_1_count_deaths', 'avg_lvl_0_to_1_count_farmfails', 'avg_lvl_0_to_1_count_food_produced', 'avg_lvl_0_to_1_count_milk_produced']
-        Original Num Rows: 6712
-        *arg* zthresh = 3
-        Removed points with abs(ZScore) >= 3. Reduced num rows: 6497
-
-    where all args are denoted by an initial *arg* and values are after =.
-
-
-    """
-    if type(meta) == str:
-        meta = meta.split('\n')
-    inner = ',\n\t'.join(["'GAME'", "'NAME'"] + [l[6:].split(' = ')[1]
-                                                 for l in meta if l.startswith('*arg*')] + ['[]'])
-    print(f'options({inner}\n)')
-
-
-# split out query creation per-game
-def filter_df(df: pd.DataFrame, query_list: List[str], one_query: bool = False, fillna: object = 0, verbose: bool = True) -> Tuple[pd.DataFrame, List[str]]:
-    """
-
-    :param df: dataframe to filter
-    :param query_list: list of queries for filter
-    :param one_query: bool to do the query (faster) as one query or seperate queries (slower, gives more info)
-    :param fillna: value to fill NaNs with
-    :param verbose: whether to input information
-    :return: (df, List[str])
-    """
-    df = df.rename({'continue': '_continue'}, axis=1)
-    filter_args = locals()
-    filter_args.pop('df')
-    filter_meta = [f'*arg* filter_args = {filter_args}']
-
-    def append_meta_str(q, shape):
-        outstr = f'Query: {q}, output_shape: {shape}'
-        filter_meta.append(outstr)
-        if verbose:
-            print(outstr)
-
-    append_meta_str('Intial Shape', df.shape)
-
-    if not one_query:
-        for q in query_list:
-            df = df.query(q)
-            append_meta_str(q, df.shape)
-    else:  # do the whole query at once
-        full_query = ' & '.join([f"({q})" for q in query_list])
-        print('full_query:', full_query)
-        df = df.query(full_query)
-        append_meta_str(full_query, df.shape)
-
-    if fillna is not None:
-        df = df.fillna(fillna)
-        filter_meta.append(f'Filled NaN with {fillna}')
-    return df.rename({'_continue': 'continue'}), filter_meta
-
-
-def create_new_base_features(df, verbose=False):
-    """
-
-    Currently a stub. Used to create new features from existing ones. See create_new_base_features_lakeland for example.
-    :param df:
-    :param verbose:
-    :return:
-    """
-    new_base_feature_args = locals()
-    new_base_feature_args.pop('df')
-    new_feat_meta = [f'*arg* new_feat_args = {new_base_feature_args}']
-
-    return df, new_feat_meta
-
-def describe_lvl_feats(df, fbase_list, lvl_range):
-    """
-    Calculates sum/avg of given level base features (fnames without lvlN_ prefix) in the level range.
-    May have a bug.
-
-    :rtype: (df, List[str]) where the new df includes sum_ and avg_lvl_A_to_B
-    :param df: dataframe to pull from and append to
-    :param fbase_list: list of feature bases (fnames without lvlN_ prefix)
-    :param lvl_range: range of levels to choose. typically range(min_level, max_level+1)
-    """
-    metadata = []
-    metadata.append(f'*arg* lvlfeats = {fbase_list}')
-    metadata.append(f'*arg* lvlrange = {lvl_range}')
-    if not fbase_list:
-        return df, metadata
-
-    # TODO: Add filter for levels we don't want, like the one from lakeland
-    # query = f'sessDuration > {(level_time - level_overlap) * (lvl_end) + level_time}'
-    # df = df.query(query)
-    # metadata.append(
-    #     f'Describe Level Feats lvls {lvl_start} to {lvl_end}. Assuming WINDOW_SIZE_SECONDS={level_time} and WINDOW_OVERLAP_SECONDS={level_overlap}, filtered by ({query})')
-
-    fromlvl, tolvl = lvl_range[0], lvl_range[-1]
-    sum_prefix = f'sum_lvl_{fromlvl}_to_{tolvl}_'
-    avg_prefix = f'avg_lvl_{fromlvl}_to_{tolvl}_'
-    for fn in fbase_list:
-        tdf = df[[f'lvl{i}_{fn}' for i in lvl_range]].fillna(0)
-        df[sum_prefix + fn] = tdf.sum(axis=1)
-        df[avg_prefix + fn] = tdf.mean(axis=1)
-    return df, metadata
-
-
-def describe_range_feats(df, range_feats_and_range, cc_prefix_max_list):
-    """
-    Calculates sum/avg of given level base features (fnames without lvlN_ prefix) in the level range.
-    May have a bug.
-
-    :rtype: (df, List[str]) where the new df includes sum_ and avg_lvl_A_to_B
-    :param df: dataframe to pull from and append to
-    :param fbase_list: list of feature bases (fnames without lvlN_ prefix)
-    :param lvl_range: range of levels to choose. typically range(min_level, max_level+1)
-    """
-    metadata = []
-    metadata.append(f'*arg* range_feats_and_range = {range_feats_and_range}')
-    metadata.append(f'*arg* cc_prefix_max_list = {cc_prefix_max_list}')
-    if not range_feats_and_range:
-        return df, metadata
-
-    # TODO: Add filter for levels we don't want, like the one from lakeland
-    # query = f'sessDuration > {(level_time - level_overlap) * (lvl_end) + level_time}'
-    # df = df.query(query)
-    # metadata.append(
-    #     f'Describe Level Feats lvls {lvl_start} to {lvl_end}. Assuming WINDOW_SIZE_SECONDS={level_time} and WINDOW_OVERLAP_SECONDS={level_overlap}, filtered by ({query})')
-
-    range_prefix_max_list = [('lvl', None)]+cc_prefix_max_list
-    for i in range(len(range_feats_and_range)):
-        range_feats, rang = range_feats_and_range[i]
-        prefix, _ = range_prefix_max_list[i]
-        fromval, toval = rang[0], rang[-1]
-        sum_prefix = f'sum_{prefix}_{fromval}_to_{toval}_'
-        avg_prefix = f'avg_{prefix}_{fromval}_to_{toval}_'
-        for fn in range_feats:
-            tdf = df[[f'{prefix}{i}_{fn}' for i in rang]].fillna(0)
-            df[sum_prefix + fn] = tdf.sum(axis=1)
-            df[avg_prefix + fn] = tdf.mean(axis=1)
-    return df, metadata
-
-
-def get_feat_selection(df, session_prefix, max_lvl, cc_prefix_max_list=None):
-    """
-    Gets the feature selection widget.
-    :param df:
-    :param max_lvl:
-    :return:
-    """
-
-    cc_prefix_max_list = cc_prefix_max_list or []
-    checkbox_widgets = []
-    slider_widgets = []
-    feats = set()
-
-    for prefix, max_val in [('lvl', max_lvl)] + cc_prefix_max_list:
-        start_val = widgets.IntSlider(value=0, min=0, max=max_val, step=1, description=f'Start {prefix}:',
-                                      disabled=False, continuous_update=False, orientation='horizontal', readout=True,
-                                      readout_format='d')
-        end_val = widgets.IntSlider(value=0, min=0, max=max_val, step=1, description=f'End {prefix}:',
-                                    disabled=False, continuous_update=False, orientation='horizontal', readout=True,
-                                    readout_format='d')
-        val_selection = widgets.GridBox([start_val, end_val])
-        slider_widgets.append(val_selection)
-        val_feats_set = set(['_'.join(f.split('_')[1:])
-                             for f in df.columns if f.startswith(prefix)])
-        feats = feats.union(
-            [f'{prefix}{n}_{v}' for n in range(max_val+1) for v in val_feats_set])
-        val_feats = sorted(val_feats_set)
-        val_feats_checkbox = multi_checkbox_widget(val_feats, prefix)
-        checkbox_widgets.append(val_feats_checkbox)
-
-    other_feats = sorted(set(df.columns).difference(feats))
-    selection_widget = widgets.GridBox(checkbox_widgets+slider_widgets+[multi_checkbox_widget(other_feats, 'other')],
-                                       layout=widgets.Layout(grid_template_columns=f"repeat({len(slider_widgets)}, 500px)"))
-
-    return selection_widget
-
-
-def get_selected_feature_list(selection_widget, session_prefix, cc_prefix_max_list=None):
-    """
-
-    :param selection_widget:
-    :return: list of features selected
-    """
-    cc_prefix_max_list = cc_prefix_max_list or []
-    prefix_list = ['lvl']+[prefix_max[0] for prefix_max in cc_prefix_max_list]
-    other_feats = [
-        s.description for s in selection_widget.children[-1].children[1].children if s.value]
-    range_feats_and_range = get_range_feats_and_range(selection_widget)
-    range_feats_list = []
-    for i in range(len(range_feats_and_range)):
-        prefix = prefix_list[i]
-        feats = range_feats_and_range[i][0]
-        rang = range_feats_and_range[i][1]
-        range_feats_list += [f'{prefix}{n}_{f}' for f in feats for n in rang]
-    return range_feats_list + other_feats
-
-
-def get_range_feats_and_range(selection_widget) -> Union[List[str], Iterable]:
-    """
-
-    :param selection_widget:
-    :return: List of fbases from selection_widget and level range
-    """
-    ret = []
-    widgets = selection_widget.children
-    assert len(widgets) % 2
-    num_range_groups = (len(widgets)-1)//2
-    for i in range(num_range_groups):
-        checkbox = widgets[i]
-        slider = widgets[i+num_range_groups]
-        start_widget = slider.children[0]
-        end_widget = slider.children[1]
-        feat_list = [
-            s.description for s in checkbox.children[1].children if s.value]
-        val_range = range(start_widget.value, end_widget.value + 1)
-        ret.append((feat_list, val_range))
-
-    return ret
-
-
-def multi_checkbox_widget(descriptions, category):
-    """ Widget with a search field and lots of checkboxes """
-    search_widget = widgets.Text(
-        layout={'width': '400px'}, description=f'Search {category}:')
-    options_dict = {description: widgets.Checkbox(description=description, value=False,
-                                                  layout={'overflow-x': 'scroll', 'width': '400px'}, indent=False) for
-                    description in descriptions}
-    options = [options_dict[description] for description in descriptions]
-    options_widget = widgets.VBox(
-        options, layout={'overflow': 'scroll', 'height': '400px'})
-    multi_select = widgets.VBox([search_widget, options_widget])
-
-    # Wire the search field to the checkboxes
-    def on_text_change(change):
-        search_input = change['new']
-        if search_input == '':
-            # Reset search field
-            for d in descriptions:
-                options_dict[d].layout.visibility = 'visible'
-                options_dict[d].layout.height = 'auto'
-        elif search_input[-1] == '$':
-            search_input = search_input[:-1]
-            # Filter by search field using difflib.
-            for d in descriptions:
-                if search_input in d:
-                    options_dict[d].layout.visibility = 'visible'
-                    options_dict[d].layout.height = 'auto'
-                else:
-                    options_dict[d].layout.visibility = 'hidden'
-                    options_dict[d].layout.height = '0px'
-            # close_matches = [d for d in descriptions if search_input in d] #difflib.get_close_matches(search_input, descriptions, cutoff=0.0)
-            # new_options = [options_dict[description] for description in close_matches]
-        # options_widget.children = new_options
-
-    search_widget.observe(on_text_change, names='value')
-    return multi_select
-
-
-def reduce_feats(df, featlist):
-    """
-    Takes in a df and outputs only the given columns in featlist
-    :param df:
-    :param featlist:
-    :return:
-    """
-    return df[featlist].copy(), [f'*arg* finalfeats = {featlist}']
-
-
-def reduce_outliers(df, z_thresh, show_graphs=True, outpath=None):
-    """
-    Takes in df and z_thresh, shows box plots, and outputs graph with points of zscore>z_thresh removed.
-    Does not always work properly. Does not seem to tolerate NaNs.
-    TODO: fix.
-    :param df:
-    :param z_thresh:
-    :param show_graphs:
-    :return:
-    """
-    meta = []
-    meta.append(f"Original Num Rows: {len(df)}")
-    meta.append(f"*arg* zthresh = {z_thresh}")
-    title = f'Raw Boxplot Original Data n={len(df)}'
-    df.plot(kind='box', title=title, figsize=(20, 5))
-    if outpath:
-        savepath = os.path.join(outpath, f'Raw Boxplot Original.png')
-        plt.savefig(savepath)
-    plt.close()
-
-    if z_thresh is None:
-        return df, meta
-
-    z = np.abs(stats.zscore(df))
-    no_outlier_df = df[(z < z_thresh).all(axis=1)]
-    meta.append(
-        f'Removed points with abs(ZScore) >= {z_thresh}. Reduced num rows: {len(no_outlier_df)}')
-    title = f'Raw Boxplot ZThresh={z_thresh} n={len(no_outlier_df)}'
-    no_outlier_df.plot(kind='box', title=title, figsize=(20, 5))
-    if outpath:
-        savepath = os.path.join(outpath, f'Raw Boxplot Zthresh Removed.png')
-        plt.savefig(savepath)
-    plt.close()
-    return no_outlier_df, meta
-
-
-jw_cc_max = [('obj', 80), ('int', 188), ('Q', 18)]
-
-
-def full_filter(df, import_meta, options, outpath) -> Tuple[pd.DataFrame, List[str]]:
-    """
-    Takes in a df, metadata, and options group.
-    Outputs the filtered df and the meta.
-    :param get_df_func:
-    :param options:
-    :return:
-    """
-    # df, import_meta = get_df_func()
-    filtered_df, filter_meta = filter_df(df, **options.filter_args)
-    game = options.game.upper()
-    # if game == 'LAKELAND':
-    #     new_feat_df, new_feat_meta = create_new_base_features_lakeland(filtered_df, **options.new_feat_args)
-    #     aggregate_df, aggregate_meta = describe_lvl_feats_lakeland(new_feat_df, options.lvlfeats, options.lvlrange)
-    # elif game == 'CRYSTAL':
-    #     new_feat_df, new_feat_meta = create_new_base_features_crystal(filtered_df, **options.new_feat_args)
-    #     aggregate_df, aggregate_meta = describe_lvl_feats_crystal(new_feat_df, options.lvlfeats, options.lvlrange)
-    # elif game == 'WAVES':
-    #     new_feat_df, new_feat_meta = create_new_base_features_waves(filtered_df, **options.new_feat_args)
-    #     aggregate_df, aggregate_meta = describe_lvl_feats_waves(new_feat_df, options.lvlfeats, options.lvlrange)
-    # else:
-    #     assert False
-    new_feat_df, new_feat_meta = create_new_base_features(
-        filtered_df, **options.new_feat_args)
-    aggregate_df, aggregate_meta = describe_lvl_feats(
-        new_feat_df, options.lvlfeats, options.lvlrange)
-    reduced_df, reduced_meta = reduce_feats(aggregate_df, options.finalfeats)
-    # hack while NaNs are popping up in aggregate df or newfeatdf TODO: Fix this. It never used to be an issue.
-    reduced_df = reduced_df.fillna(0)
-    final_df, outlier_meta = reduce_outliers(
-        reduced_df, options.zthresh, outpath=outpath)
-    final_meta = import_meta + filter_meta + new_feat_meta + \
-        aggregate_meta + reduced_meta + outlier_meta
-    return final_df, final_meta
-
-
-def save_csv_and_meta(df, meta_list, save_dir, csv_name, meta_name=None, permissions='w+', add_columns=True):
-    if csv_name.endswith(('.tsv', '.csv')):
-        extension = csv_name[-4:]
-        csv_name = csv_name[:-4]
-    else:
-        extension = '.csv'
-    separator = '\t' if extension == '.tsv' else ','
-
-    # hardcopy
-    meta_list = [x for x in meta_list]
-    meta_list.append(f'OUTPUT_SHAPE: {df.shape}')
-    meta_list.append(f'OUTPUT_FILE: {csv_name}')
-    meta_list.append(f'CSV OUTPUT_DATE: {datetime.now()}')
-    if add_columns:
-        meta_list.append(f'OUTPUT_COLUMNS: {sorted(list(df.columns))}')
-
-    meta_name = meta_name or csv_name + '_meta.txt'
-    meta_text = save_meta(meta_list, save_dir, meta_name, permissions=permissions)
-
-    with open(os.path.join(save_dir, csv_name)+extension, permissions) as f:
-        for l in meta_text.splitlines():
-            f.write(f'# {l}\n')
-        f.write('\n')
-        df.to_csv(f, sep=separator)
-
-    return None, []
-
-def save_meta(meta_list, save_dir, meta_name, permissions='w+'):
-    meta_text = 'Metadata:\n'+'\n'.join(meta_list+[
-        f'META OUTPUT_DATE: {datetime.now()}'
-    ])
-    with open(os.path.join(save_dir, meta_name), permissions) as f:
-        f.write(meta_text)
-    return meta_text
-
-
-def open_csv_from_path_with_meta(csv_fpath, index_col=0):
-    metadata = []
-    with open(csv_fpath) as f:
-        for line in f.readlines():
-            if line.startswith('#'):
-                metadata.append(line[2:].strip())
-            else:
-                break
-    df = pd.read_csv(csv_fpath, comment='#', index_col=index_col)
-    return df, metadata
-
-def remove_nan_labels(X, y):
-    nonnull_indices = ~y.isna()
-    ret_X = X.loc[nonnull_indices, :].copy()
-    ret_y = y.loc[nonnull_indices].copy()
-    return ret_X, ret_y
-
-def get_PSPC_pipeline(classifier, preprocessor=None, sampler=None):
-    """
-Returns a Preporcessor Sampler Preprocessor Classifier pipeline
-imblearn.pipeline.make_pipeline(preprocessor, sampler, copy.deepcopy(preprocessor),classifier)
-    :param classifier: sklearn compatible classifier
-    :param preprocessor: sklearn compatible classifier (Make sure it won't change the data if applied iteratively!)
-    :param sampler: sklearn compatible sampler
-    :return:
-    """
-    clf = imblearn.pipeline.make_pipeline(preprocessor, sampler, copy.deepcopy(preprocessor),classifier)
-    return clf
-
-
-
-
-def save_model(savedir, savename, model, X_test, y_test, meta_list=None):
-    name, ext = os.path.splitext(savename)
-    if meta_list:
-        meta_list = [x for x in meta_list]
-        meta_list.append(f'MODEL_USED: {model}')
-        meta_list.append(f'TEST_SHAPE: {X_test.shape}')
-        meta_list.append(f'MODEL_Ytest_Xtest_SAVEPATH: {savename}')
-        meta_list.append(f'OUTPUT_FILE: {savename}')
-        meta_list.append(f'MODEL_OUTPUT_DATE: {datetime.now()}')
-        meta_list.append(f'TEST_COLUMNS: {sorted(list(X_test.columns))}')
-        meta_name = name + '_meta.txt'
-        save_meta(meta_list, savedir, meta_name, permissions='w+')
-    with open(os.path.join(savedir, savename),'wb+') as f:
-        pickle.dump((model, y_test, X_test), f)
-
-def load_model(loadpath):
-    ## Do NOT load ANYTHING that you don't 100% trust! Malicious contents could easily harm your computer.
-    with open(loadpath, 'rb') as f:
-        model, y_test, X_test = pickle.load(f)
-    return model, X_test, y_test, 
-
-def corr_heatmap(df,figsize=(20,20),max_corr=.3, max_rows=3000):
-    corr = fast_corr(df, max_rows)
-    # Generate a mask for the upper triangle
-    mask = np.triu(np.ones_like(corr, dtype=bool))
-
-    # Set up the matplotlib figure
-    f, ax = plt.subplots(figsize=figsize)
-
-    # Generate a custom diverging colormap
-    cmap = sns.diverging_palette(220, 10, as_cmap=True)
-
-    # Draw the heatmap with the mask and correct aspect ratio
-    sns.heatmap(corr, mask=mask, cmap=cmap, vmax=max_corr, vmin=-1*max_corr, center=0,
-                square=True, linewidths=.5, cbar_kws={"shrink": .5})
-def fast_corr(df, max_rows):
-    num_rows = min(max_rows, len(df))
-    corr_matrix = df.iloc[:num_rows,:].corr()
-    return corr_matrix
-
-def get_high_corr_columns(df, thresh=.95,max_rows=3000):
-    corr_matrix = fast_corr(df,max_rows=max_rows).abs()
-    # Select upper triangle of correlation matrix
-    upper = corr_matrix.where(np.triu(np.ones(corr_matrix.shape), k=1).astype(bool))
-
-    # Find index of feature columns with correlation greater or equal to thresh
-    to_drop = [column for column in upper.columns if any(upper[column] >= thresh)]
-    return to_drop
-
-def fb(prec, recall, beta=1):
-    if prec == 0 or recall == 0:
-        return 0
-    numerator = prec*recall
-    denominator = prec*beta*beta + recall
-    return (1+beta*beta)*numerator/denominator
-
-def f1(prec, recall):
-    return fb(prec, recall, beta=1)
-
-def f2(prec, recall):
-    return fb(prec, recall, beta=2)
-
-def binary_metric_list(y_true, y_pred, y_prob, X_shape=None, label_prefix='', majority_class=1):
-    metric_list = []
-
-    baseline_pred = [majority_class]*len(y_true)
-
-    auc = roc_auc_score(y_true=y_true, y_score=y_prob)
-    metric_list.append((auc, f'{label_prefix}AUC'))
-    f1macro = f1_score(y_true=y_true, y_pred=y_pred, average='macro')
-    metric_list.append((f1macro, f'{label_prefix}f1_avg'))
-    acc = accuracy_score(y_true=y_true, y_pred=y_pred)
-    metric_list.append((acc, f'{label_prefix}acc'))
-    baseline_acc = accuracy_score(y_true=y_true, y_pred=baseline_pred)
-    metric_list.append((acc, f'{label_prefix}acc'))
-    metric_list.append((baseline_acc, f'{label_prefix}baseline_acc'))
-    baseline_auc = roc_auc_score(y_true=y_true, y_score=baseline_pred)
-    metric_list.append((baseline_auc, f'{label_prefix}baseline_auc'))
-    dAcc = acc - baseline_acc
-    dAuc = auc - baseline_auc
-    metric_list.append((dAuc, f'{label_prefix}dAuc'))
-    metric_list.append((dAcc, f'{label_prefix}dAcc'))
-
-
-    counter = Counter(y_true)
-    size_0s, size_1s = counter[0], counter[1]
-    if X_shape:
-        num_rows, num_cols = X_shape
-        assert (size_0s + size_1s) == num_rows
-        metric_list.append((num_rows, f'{label_prefix}total_size'))
-        metric_list.append((num_cols, f'{label_prefix}num_feats'))
-
-
-    metric_list.append((size_0s, f'{label_prefix}size_0s'))
-    metric_list.append((size_1s, f'{label_prefix}size_1s'))
-
-    confusion_mat = confusion_matrix(y_true, y_pred)
-    tn, fp, fn, tp = confusion_mat.ravel()        
-    precision_1 = tp/(tp+fp)
-    b_precision_1 = size_1s/(size_1s+size_0s)
-    precision_0 = tn/(tn+fn)
-    b_precision_0 = size_0s/(size_1s+size_0s)
-    recall_1 = tp/(tp+fn)
-    recall_0 = tn/(tn+fp)
-    b_recall = 1
-    f1_1 = f1(precision_1, recall_1)
-    b_f1_1 = f1(b_precision_1, b_recall)
-    f1_0 = f1(precision_0, recall_0)
-    b_f1_0 = f1(b_precision_0, b_recall)
-    f2_1 = f2(precision_1, recall_1)
-    b_f2_1 = f2(b_precision_1, b_recall)
-    f2_0 = f2(precision_0, recall_0)
-    b_f2_0 = f2(b_precision_0, b_recall)
-    f1_avg = (f1_1+f1_0)/2
-
-    metric_list.extend([
-        (tp, f'{label_prefix}tp'),
-        (fp, f'{label_prefix}fp'),
-        (tn, f'{label_prefix}tn'),
-        (fn, f'{label_prefix}fn'),
-        (precision_1, f'{label_prefix}prec_1'),
-        (precision_0, f'{label_prefix}prec_0'),
-        (recall_1, f'{label_prefix}recall_1'),
-        (recall_0, f'{label_prefix}recall_0'),
-        (f1_1, f'{label_prefix}f1_1'),
-        (f1_0, f'{label_prefix}f1_0'),
-        (f2_1, f'{label_prefix}f2_1'),
-        (f2_0, f'{label_prefix}f2_0'),
-
-        (b_precision_1, f'{label_prefix}prec_1_baseline'),
-        (b_precision_0, f'{label_prefix}prec_0_baseline'),
-        (b_f1_1, f'{label_prefix}f1_1_baseline'),
-        (b_f1_0, f'{label_prefix}f1_0_baseline'),
-        (b_f2_1, f'{label_prefix}f2_1_baseline'),
-        (b_f2_0, f'{label_prefix}f2_0_baseline'),
-
-        (precision_1 - b_precision_1, f'{label_prefix}dPrec_1'),
-        (precision_0 - b_precision_0, f'{label_prefix}dPrec_0'),
-        (f1_1 - b_f1_1, f'{label_prefix}dF1_1'),
-        (f1_0 - b_f1_0, f'{label_prefix}dF1_0'),
-        (f2_1 - b_f2_1, f'{label_prefix}dF2_1'),
-        (f2_0 - b_f2_0, f'{label_prefix}dF2_0'),
-    ])
-
-    return metric_list
-
-
-if __name__ == '__main__':
-    pass
+"""
+Note: Utils in this file are 
+
+Usage:
+If the first cell ran correctly, changing the CWD to the Jupyter file and adding '.' to sys path, then.
+import Notebooks.Clustering.cluster_utils as cu
+
+Otherwise:
+from google.colab import drive
+drive.mount('/content/drive')
+
+import os
+FIELDDAY_DIR = '/content/drive/My Drive/Field Day' # the field day directory on the mounted drive
+JUPYTER_DIR = os.path.join(FIELDDAY_DIR,'Research and Writing Projects/2020 Lakeland EDM/Jupyter')
+os.chdir(JUPYTER_DIR)
+
+import sys
+sys.path.append('.')
+import Notebooks.Clustering.cluster_utils as cu
+
+"""
+import copy
+import os
+import numpy as np
+import pandas as pd
+import seaborn as sns
+sns.set()
+import ipywidgets as widgets
+from matplotlib import pyplot as plt
+from scipy import stats
+from typing import Iterable, Optional, List, Tuple, Union
+from sklearn.metrics import confusion_matrix
+from sklearn.metrics import f1_score, roc_auc_score, accuracy_score
+from datetime import datetime
+import pickle
+from collections import Counter
+
+
+
+def print_options(meta):
+    """
+    Takes in meta text and outputs text for an options group.
+    :param meta: meta text. Expected format will be like:
+
+        Metadata:
+        Import from fhttps://opengamedata.fielddaylab.wisc.edu/data/LAKELAND/LAKELAND_20191201_to_20191231_de09c18_proc.zip
+        Import from fData/Raw Log Data/LAKELAND_20200101_to_20200131_a9720c1_proc.zip
+        *arg* filter_args = {'query_list': ['debug == 0', 'sess_ActiveEventCount >= 10', 'sessDuration >= 300', '_continue == 0'], 'one_query': False, 'fillna': 0, 'verbose': True}
+        Query: Intial Shape, output_shape: (32227, 1647)
+        Query: debug == 0, output_shape: (32221, 1647)
+        Query: sess_ActiveEventCount >= 10, output_shape: (26934, 1647)
+        Query: sessDuration >= 300, output_shape: (16109, 1647)
+        Query: _continue == 0, output_shape: (10591, 1647)
+        Filled NaN with 0
+        *arg* new_feat_args = {'verbose': False, 'avg_tile_hover_lvl_range': None}
+        *arg* lvlfeats = ['count_blooms', 'count_deaths', 'count_farmfails', 'count_food_produced', 'count_milk_produced']
+        *arg* lvlrange = range(0, 2)
+        Describe Level Feats lvls 0 to 1. Assuming WINDOW_SIZE_SECONDS=300 and WINDOW_OVERLAP_SECONDS=30, filtered by (sessDuration > 570)
+        *arg* finalfeats = ['avg_lvl_0_to_1_count_deaths', 'avg_lvl_0_to_1_count_farmfails', 'avg_lvl_0_to_1_count_food_produced', 'avg_lvl_0_to_1_count_milk_produced']
+        Original Num Rows: 6712
+        *arg* zthresh = 3
+        Removed points with abs(ZScore) >= 3. Reduced num rows: 6497
+
+    where all args are denoted by an initial *arg* and values are after =.
+
+
+    """
+    if type(meta) == str:
+        meta = meta.split('\n')
+    inner = ',\n\t'.join(["'GAME'", "'NAME'"] + [l[6:].split(' = ')[1]
+                                                 for l in meta if l.startswith('*arg*')] + ['[]'])
+    print(f'options({inner}\n)')
+
+
+# split out query creation per-game
+def filter_df(df: pd.DataFrame, query_list: List[str], one_query: bool = False, fillna: object = 0, verbose: bool = True) -> Tuple[pd.DataFrame, List[str]]:
+    """
+
+    :param df: dataframe to filter
+    :param query_list: list of queries for filter
+    :param one_query: bool to do the query (faster) as one query or seperate queries (slower, gives more info)
+    :param fillna: value to fill NaNs with
+    :param verbose: whether to input information
+    :return: (df, List[str])
+    """
+    df = df.rename({'continue': '_continue'}, axis=1)
+    filter_args = locals()
+    filter_args.pop('df')
+    filter_meta = [f'*arg* filter_args = {filter_args}']
+
+    def append_meta_str(q, shape):
+        outstr = f'Query: {q}, output_shape: {shape}'
+        filter_meta.append(outstr)
+        if verbose:
+            print(outstr)
+
+    append_meta_str('Intial Shape', df.shape)
+
+    if not one_query:
+        for q in query_list:
+            df = df.query(q)
+            append_meta_str(q, df.shape)
+    else:  # do the whole query at once
+        full_query = ' & '.join([f"({q})" for q in query_list])
+        print('full_query:', full_query)
+        df = df.query(full_query)
+        append_meta_str(full_query, df.shape)
+
+    if fillna is not None:
+        df = df.fillna(fillna)
+        filter_meta.append(f'Filled NaN with {fillna}')
+    return df.rename({'_continue': 'continue'}), filter_meta
+
+
+def create_new_base_features(df, verbose=False):
+    """
+
+    Currently a stub. Used to create new features from existing ones. See create_new_base_features_lakeland for example.
+    :param df:
+    :param verbose:
+    :return:
+    """
+    new_base_feature_args = locals()
+    new_base_feature_args.pop('df')
+    new_feat_meta = [f'*arg* new_feat_args = {new_base_feature_args}']
+
+    return df, new_feat_meta
+
+def describe_lvl_feats(df, fbase_list, lvl_range):
+    """
+    Calculates sum/avg of given level base features (fnames without lvlN_ prefix) in the level range.
+    May have a bug.
+
+    :rtype: (df, List[str]) where the new df includes sum_ and avg_lvl_A_to_B
+    :param df: dataframe to pull from and append to
+    :param fbase_list: list of feature bases (fnames without lvlN_ prefix)
+    :param lvl_range: range of levels to choose. typically range(min_level, max_level+1)
+    """
+    metadata = []
+    metadata.append(f'*arg* lvlfeats = {fbase_list}')
+    metadata.append(f'*arg* lvlrange = {lvl_range}')
+    if not fbase_list:
+        return df, metadata
+
+    # TODO: Add filter for levels we don't want, like the one from lakeland
+    # query = f'sessDuration > {(level_time - level_overlap) * (lvl_end) + level_time}'
+    # df = df.query(query)
+    # metadata.append(
+    #     f'Describe Level Feats lvls {lvl_start} to {lvl_end}. Assuming WINDOW_SIZE_SECONDS={level_time} and WINDOW_OVERLAP_SECONDS={level_overlap}, filtered by ({query})')
+
+    fromlvl, tolvl = lvl_range[0], lvl_range[-1]
+    sum_prefix = f'sum_lvl_{fromlvl}_to_{tolvl}_'
+    avg_prefix = f'avg_lvl_{fromlvl}_to_{tolvl}_'
+    for fn in fbase_list:
+        tdf = df[[f'lvl{i}_{fn}' for i in lvl_range]].fillna(0)
+        df[sum_prefix + fn] = tdf.sum(axis=1)
+        df[avg_prefix + fn] = tdf.mean(axis=1)
+    return df, metadata
+
+
+def describe_range_feats(df, range_feats_and_range, cc_prefix_max_list):
+    """
+    Calculates sum/avg of given level base features (fnames without lvlN_ prefix) in the level range.
+    May have a bug.
+
+    :rtype: (df, List[str]) where the new df includes sum_ and avg_lvl_A_to_B
+    :param df: dataframe to pull from and append to
+    :param fbase_list: list of feature bases (fnames without lvlN_ prefix)
+    :param lvl_range: range of levels to choose. typically range(min_level, max_level+1)
+    """
+    metadata = []
+    metadata.append(f'*arg* range_feats_and_range = {range_feats_and_range}')
+    metadata.append(f'*arg* cc_prefix_max_list = {cc_prefix_max_list}')
+    if not range_feats_and_range:
+        return df, metadata
+
+    # TODO: Add filter for levels we don't want, like the one from lakeland
+    # query = f'sessDuration > {(level_time - level_overlap) * (lvl_end) + level_time}'
+    # df = df.query(query)
+    # metadata.append(
+    #     f'Describe Level Feats lvls {lvl_start} to {lvl_end}. Assuming WINDOW_SIZE_SECONDS={level_time} and WINDOW_OVERLAP_SECONDS={level_overlap}, filtered by ({query})')
+
+    range_prefix_max_list = [('lvl', None)]+cc_prefix_max_list
+    for i in range(len(range_feats_and_range)):
+        range_feats, rang = range_feats_and_range[i]
+        prefix, _ = range_prefix_max_list[i]
+        fromval, toval = rang[0], rang[-1]
+        sum_prefix = f'sum_{prefix}_{fromval}_to_{toval}_'
+        avg_prefix = f'avg_{prefix}_{fromval}_to_{toval}_'
+        for fn in range_feats:
+            tdf = df[[f'{prefix}{i}_{fn}' for i in rang]].fillna(0)
+            df[sum_prefix + fn] = tdf.sum(axis=1)
+            df[avg_prefix + fn] = tdf.mean(axis=1)
+    return df, metadata
+
+
+def get_feat_selection(df, session_prefix, max_lvl, cc_prefix_max_list=None):
+    """
+    Gets the feature selection widget.
+    :param df:
+    :param max_lvl:
+    :return:
+    """
+
+    cc_prefix_max_list = cc_prefix_max_list or []
+    checkbox_widgets = []
+    slider_widgets = []
+    feats = set()
+
+    for prefix, max_val in [('lvl', max_lvl)] + cc_prefix_max_list:
+        start_val = widgets.IntSlider(value=0, min=0, max=max_val, step=1, description=f'Start {prefix}:',
+                                      disabled=False, continuous_update=False, orientation='horizontal', readout=True,
+                                      readout_format='d')
+        end_val = widgets.IntSlider(value=0, min=0, max=max_val, step=1, description=f'End {prefix}:',
+                                    disabled=False, continuous_update=False, orientation='horizontal', readout=True,
+                                    readout_format='d')
+        val_selection = widgets.GridBox([start_val, end_val])
+        slider_widgets.append(val_selection)
+        val_feats_set = set(['_'.join(f.split('_')[1:])
+                             for f in df.columns if f.startswith(prefix)])
+        feats = feats.union(
+            [f'{prefix}{n}_{v}' for n in range(max_val+1) for v in val_feats_set])
+        val_feats = sorted(val_feats_set)
+        val_feats_checkbox = multi_checkbox_widget(val_feats, prefix)
+        checkbox_widgets.append(val_feats_checkbox)
+
+    other_feats = sorted(set(df.columns).difference(feats))
+    selection_widget = widgets.GridBox(checkbox_widgets+slider_widgets+[multi_checkbox_widget(other_feats, 'other')],
+                                       layout=widgets.Layout(grid_template_columns=f"repeat({len(slider_widgets)}, 500px)"))
+
+    return selection_widget
+
+
+def get_selected_feature_list(selection_widget, session_prefix, cc_prefix_max_list=None):
+    """
+
+    :param selection_widget:
+    :return: list of features selected
+    """
+    cc_prefix_max_list = cc_prefix_max_list or []
+    prefix_list = ['lvl']+[prefix_max[0] for prefix_max in cc_prefix_max_list]
+    other_feats = [
+        s.description for s in selection_widget.children[-1].children[1].children if s.value]
+    range_feats_and_range = get_range_feats_and_range(selection_widget)
+    range_feats_list = []
+    for i in range(len(range_feats_and_range)):
+        prefix = prefix_list[i]
+        feats = range_feats_and_range[i][0]
+        rang = range_feats_and_range[i][1]
+        range_feats_list += [f'{prefix}{n}_{f}' for f in feats for n in rang]
+    return range_feats_list + other_feats
+
+
+def get_range_feats_and_range(selection_widget) -> Union[List[str], Iterable]:
+    """
+
+    :param selection_widget:
+    :return: List of fbases from selection_widget and level range
+    """
+    ret = []
+    widgets = selection_widget.children
+    assert len(widgets) % 2
+    num_range_groups = (len(widgets)-1)//2
+    for i in range(num_range_groups):
+        checkbox = widgets[i]
+        slider = widgets[i+num_range_groups]
+        start_widget = slider.children[0]
+        end_widget = slider.children[1]
+        feat_list = [
+            s.description for s in checkbox.children[1].children if s.value]
+        val_range = range(start_widget.value, end_widget.value + 1)
+        ret.append((feat_list, val_range))
+
+    return ret
+
+
+def multi_checkbox_widget(descriptions, category):
+    """ Widget with a search field and lots of checkboxes """
+    search_widget = widgets.Text(
+        layout={'width': '400px'}, description=f'Search {category}:')
+    options_dict = {description: widgets.Checkbox(description=description, value=False,
+                                                  layout={'overflow-x': 'scroll', 'width': '400px'}, indent=False) for
+                    description in descriptions}
+    options = [options_dict[description] for description in descriptions]
+    options_widget = widgets.VBox(
+        options, layout={'overflow': 'scroll', 'height': '400px'})
+    multi_select = widgets.VBox([search_widget, options_widget])
+
+    # Wire the search field to the checkboxes
+    def on_text_change(change):
+        search_input = change['new']
+        if search_input == '':
+            # Reset search field
+            for d in descriptions:
+                options_dict[d].layout.visibility = 'visible'
+                options_dict[d].layout.height = 'auto'
+        elif search_input[-1] == '$':
+            search_input = search_input[:-1]
+            # Filter by search field using difflib.
+            for d in descriptions:
+                if search_input in d:
+                    options_dict[d].layout.visibility = 'visible'
+                    options_dict[d].layout.height = 'auto'
+                else:
+                    options_dict[d].layout.visibility = 'hidden'
+                    options_dict[d].layout.height = '0px'
+            # close_matches = [d for d in descriptions if search_input in d] #difflib.get_close_matches(search_input, descriptions, cutoff=0.0)
+            # new_options = [options_dict[description] for description in close_matches]
+        # options_widget.children = new_options
+
+    search_widget.observe(on_text_change, names='value')
+    return multi_select
+
+
+def reduce_feats(df, featlist):
+    """
+    Takes in a df and outputs only the given columns in featlist
+    :param df:
+    :param featlist:
+    :return:
+    """
+    return df[featlist].copy(), [f'*arg* finalfeats = {featlist}']
+
+
+def reduce_outliers(df, z_thresh, show_graphs=True, outpath=None):
+    """
+    Takes in df and z_thresh, shows box plots, and outputs graph with points of zscore>z_thresh removed.
+    Does not always work properly. Does not seem to tolerate NaNs.
+    TODO: fix.
+    :param df:
+    :param z_thresh:
+    :param show_graphs:
+    :return:
+    """
+    meta = []
+    meta.append(f"Original Num Rows: {len(df)}")
+    meta.append(f"*arg* zthresh = {z_thresh}")
+    title = f'Raw Boxplot Original Data n={len(df)}'
+    df.plot(kind='box', title=title, figsize=(20, 5))
+    if outpath:
+        savepath = os.path.join(outpath, f'Raw Boxplot Original.png')
+        plt.savefig(savepath)
+    plt.close()
+
+    if z_thresh is None:
+        return df, meta
+
+    z = np.abs(stats.zscore(df))
+    no_outlier_df = df[(z < z_thresh).all(axis=1)]
+    meta.append(
+        f'Removed points with abs(ZScore) >= {z_thresh}. Reduced num rows: {len(no_outlier_df)}')
+    title = f'Raw Boxplot ZThresh={z_thresh} n={len(no_outlier_df)}'
+    no_outlier_df.plot(kind='box', title=title, figsize=(20, 5))
+    if outpath:
+        savepath = os.path.join(outpath, f'Raw Boxplot Zthresh Removed.png')
+        plt.savefig(savepath)
+    plt.close()
+    return no_outlier_df, meta
+
+
+jw_cc_max = [('obj', 80), ('int', 188), ('Q', 18)]
+
+
+def full_filter(df, import_meta, options, outpath) -> Tuple[pd.DataFrame, List[str]]:
+    """
+    Takes in a df, metadata, and options group.
+    Outputs the filtered df and the meta.
+    :param get_df_func:
+    :param options:
+    :return:
+    """
+    # df, import_meta = get_df_func()
+    filtered_df, filter_meta = filter_df(df, **options.filter_args)
+    game = options.game.upper()
+    # if game == 'LAKELAND':
+    #     new_feat_df, new_feat_meta = create_new_base_features_lakeland(filtered_df, **options.new_feat_args)
+    #     aggregate_df, aggregate_meta = describe_lvl_feats_lakeland(new_feat_df, options.lvlfeats, options.lvlrange)
+    # elif game == 'CRYSTAL':
+    #     new_feat_df, new_feat_meta = create_new_base_features_crystal(filtered_df, **options.new_feat_args)
+    #     aggregate_df, aggregate_meta = describe_lvl_feats_crystal(new_feat_df, options.lvlfeats, options.lvlrange)
+    # elif game == 'WAVES':
+    #     new_feat_df, new_feat_meta = create_new_base_features_waves(filtered_df, **options.new_feat_args)
+    #     aggregate_df, aggregate_meta = describe_lvl_feats_waves(new_feat_df, options.lvlfeats, options.lvlrange)
+    # else:
+    #     assert False
+    new_feat_df, new_feat_meta = create_new_base_features(
+        filtered_df, **options.new_feat_args)
+    aggregate_df, aggregate_meta = describe_lvl_feats(
+        new_feat_df, options.lvlfeats, options.lvlrange)
+    reduced_df, reduced_meta = reduce_feats(aggregate_df, options.finalfeats)
+    # hack while NaNs are popping up in aggregate df or newfeatdf TODO: Fix this. It never used to be an issue.
+    reduced_df = reduced_df.fillna(0)
+    final_df, outlier_meta = reduce_outliers(
+        reduced_df, options.zthresh, outpath=outpath)
+    final_meta = import_meta + filter_meta + new_feat_meta + \
+        aggregate_meta + reduced_meta + outlier_meta
+    return final_df, final_meta
+
+
+def save_csv_and_meta(df, meta_list, save_dir, csv_name, meta_name=None, permissions='w+', add_columns=True):
+    if csv_name.endswith(('.tsv', '.csv')):
+        extension = csv_name[-4:]
+        csv_name = csv_name[:-4]
+    else:
+        extension = '.csv'
+    separator = '\t' if extension == '.tsv' else ','
+
+    # hardcopy
+    meta_list = [x for x in meta_list]
+    meta_list.append(f'OUTPUT_SHAPE: {df.shape}')
+    meta_list.append(f'OUTPUT_FILE: {csv_name}')
+    meta_list.append(f'CSV OUTPUT_DATE: {datetime.now()}')
+    if add_columns:
+        meta_list.append(f'OUTPUT_COLUMNS: {sorted(list(df.columns))}')
+
+    meta_name = meta_name or csv_name + '_meta.txt'
+    meta_text = save_meta(meta_list, save_dir, meta_name, permissions=permissions)
+
+    with open(os.path.join(save_dir, csv_name)+extension, permissions) as f:
+        for l in meta_text.splitlines():
+            f.write(f'# {l}\n')
+        f.write('\n')
+        df.to_csv(f, sep=separator)
+
+    return None, []
+
+def save_meta(meta_list, save_dir, meta_name, permissions='w+'):
+    meta_text = 'Metadata:\n'+'\n'.join(meta_list+[
+        f'META OUTPUT_DATE: {datetime.now()}'
+    ])
+    with open(os.path.join(save_dir, meta_name), permissions) as f:
+        f.write(meta_text)
+    return meta_text
+
+
+def open_csv_from_path_with_meta(csv_fpath, index_col=0):
+    metadata = []
+    with open(csv_fpath) as f:
+        for line in f.readlines():
+            if line.startswith('#'):
+                metadata.append(line[2:].strip())
+            else:
+                break
+    df = pd.read_csv(csv_fpath, comment='#', index_col=index_col)
+    return df, metadata
+
+def remove_nan_labels(X, y):
+    nonnull_indices = ~y.isna()
+    ret_X = X.loc[nonnull_indices, :].copy()
+    ret_y = y.loc[nonnull_indices].copy()
+    return ret_X, ret_y
+
+def get_PSPC_pipeline(classifier, preprocessor=None, sampler=None):
+    """
+Returns a Preporcessor Sampler Preprocessor Classifier pipeline
+imblearn.pipeline.make_pipeline(preprocessor, sampler, copy.deepcopy(preprocessor),classifier)
+    :param classifier: sklearn compatible classifier
+    :param preprocessor: sklearn compatible classifier (Make sure it won't change the data if applied iteratively!)
+    :param sampler: sklearn compatible sampler
+    :return:
+    """
+    clf = imblearn.pipeline.make_pipeline(preprocessor, sampler, copy.deepcopy(preprocessor),classifier)
+    return clf
+
+
+
+
+def save_model(savedir, savename, model, X_test, y_test, meta_list=None):
+    name, ext = os.path.splitext(savename)
+    if meta_list:
+        meta_list = [x for x in meta_list]
+        meta_list.append(f'MODEL_USED: {model}')
+        meta_list.append(f'TEST_SHAPE: {X_test.shape}')
+        meta_list.append(f'MODEL_Ytest_Xtest_SAVEPATH: {savename}')
+        meta_list.append(f'OUTPUT_FILE: {savename}')
+        meta_list.append(f'MODEL_OUTPUT_DATE: {datetime.now()}')
+        meta_list.append(f'TEST_COLUMNS: {sorted(list(X_test.columns))}')
+        meta_name = name + '_meta.txt'
+        save_meta(meta_list, savedir, meta_name, permissions='w+')
+    with open(os.path.join(savedir, savename),'wb+') as f:
+        pickle.dump((model, y_test, X_test), f)
+
+def load_model(loadpath):
+    ## Do NOT load ANYTHING that you don't 100% trust! Malicious contents could easily harm your computer.
+    with open(loadpath, 'rb') as f:
+        model, y_test, X_test = pickle.load(f)
+    return model, X_test, y_test, 
+
+def corr_heatmap(df,figsize=(20,20),max_corr=.3, max_rows=3000):
+    corr = fast_corr(df, max_rows)
+    # Generate a mask for the upper triangle
+    mask = np.triu(np.ones_like(corr, dtype=bool))
+
+    # Set up the matplotlib figure
+    f, ax = plt.subplots(figsize=figsize)
+
+    # Generate a custom diverging colormap
+    cmap = sns.diverging_palette(220, 10, as_cmap=True)
+
+    # Draw the heatmap with the mask and correct aspect ratio
+    sns.heatmap(corr, mask=mask, cmap=cmap, vmax=max_corr, vmin=-1*max_corr, center=0,
+                square=True, linewidths=.5, cbar_kws={"shrink": .5})
+def fast_corr(df, max_rows):
+    num_rows = min(max_rows, len(df))
+    corr_matrix = df.iloc[:num_rows,:].corr()
+    return corr_matrix
+
+def get_high_corr_columns(df, thresh=.95,max_rows=3000):
+    corr_matrix = fast_corr(df,max_rows=max_rows).abs()
+    # Select upper triangle of correlation matrix
+    upper = corr_matrix.where(np.triu(np.ones(corr_matrix.shape), k=1).astype(bool))
+
+    # Find index of feature columns with correlation greater or equal to thresh
+    to_drop = [column for column in upper.columns if any(upper[column] >= thresh)]
+    return to_drop
+
+def fb(prec, recall, beta=1):
+    if prec == 0 or recall == 0:
+        return 0
+    numerator = prec*recall
+    denominator = prec*beta*beta + recall
+    return (1+beta*beta)*numerator/denominator
+
+def f1(prec, recall):
+    return fb(prec, recall, beta=1)
+
+def f2(prec, recall):
+    return fb(prec, recall, beta=2)
+
+def binary_metric_list(y_true, y_pred, y_prob, X_shape=None, label_prefix='', majority_class=1):
+    metric_list = []
+
+    baseline_pred = [majority_class]*len(y_true)
+
+    auc = roc_auc_score(y_true=y_true, y_score=y_prob)
+    metric_list.append((auc, f'{label_prefix}AUC'))
+    f1macro = f1_score(y_true=y_true, y_pred=y_pred, average='macro')
+    metric_list.append((f1macro, f'{label_prefix}f1_avg'))
+    acc = accuracy_score(y_true=y_true, y_pred=y_pred)
+    metric_list.append((acc, f'{label_prefix}acc'))
+    baseline_acc = accuracy_score(y_true=y_true, y_pred=baseline_pred)
+    metric_list.append((acc, f'{label_prefix}acc'))
+    metric_list.append((baseline_acc, f'{label_prefix}baseline_acc'))
+    baseline_auc = roc_auc_score(y_true=y_true, y_score=baseline_pred)
+    metric_list.append((baseline_auc, f'{label_prefix}baseline_auc'))
+    dAcc = acc - baseline_acc
+    dAuc = auc - baseline_auc
+    metric_list.append((dAuc, f'{label_prefix}dAuc'))
+    metric_list.append((dAcc, f'{label_prefix}dAcc'))
+
+
+    counter = Counter(y_true)
+    size_0s, size_1s = counter[0], counter[1]
+    if X_shape:
+        num_rows, num_cols = X_shape
+        assert (size_0s + size_1s) == num_rows
+        metric_list.append((num_rows, f'{label_prefix}total_size'))
+        metric_list.append((num_cols, f'{label_prefix}num_feats'))
+
+
+    metric_list.append((size_0s, f'{label_prefix}size_0s'))
+    metric_list.append((size_1s, f'{label_prefix}size_1s'))
+
+    confusion_mat = confusion_matrix(y_true, y_pred)
+    tn, fp, fn, tp = confusion_mat.ravel()        
+    precision_1 = tp/(tp+fp)
+    b_precision_1 = size_1s/(size_1s+size_0s)
+    precision_0 = tn/(tn+fn)
+    b_precision_0 = size_0s/(size_1s+size_0s)
+    recall_1 = tp/(tp+fn)
+    recall_0 = tn/(tn+fp)
+    b_recall = 1
+    f1_1 = f1(precision_1, recall_1)
+    b_f1_1 = f1(b_precision_1, b_recall)
+    f1_0 = f1(precision_0, recall_0)
+    b_f1_0 = f1(b_precision_0, b_recall)
+    f2_1 = f2(precision_1, recall_1)
+    b_f2_1 = f2(b_precision_1, b_recall)
+    f2_0 = f2(precision_0, recall_0)
+    b_f2_0 = f2(b_precision_0, b_recall)
+    f1_avg = (f1_1+f1_0)/2
+
+    metric_list.extend([
+        (tp, f'{label_prefix}tp'),
+        (fp, f'{label_prefix}fp'),
+        (tn, f'{label_prefix}tn'),
+        (fn, f'{label_prefix}fn'),
+        (precision_1, f'{label_prefix}prec_1'),
+        (precision_0, f'{label_prefix}prec_0'),
+        (recall_1, f'{label_prefix}recall_1'),
+        (recall_0, f'{label_prefix}recall_0'),
+        (f1_1, f'{label_prefix}f1_1'),
+        (f1_0, f'{label_prefix}f1_0'),
+        (f2_1, f'{label_prefix}f2_1'),
+        (f2_0, f'{label_prefix}f2_0'),
+
+        (b_precision_1, f'{label_prefix}prec_1_baseline'),
+        (b_precision_0, f'{label_prefix}prec_0_baseline'),
+        (b_f1_1, f'{label_prefix}f1_1_baseline'),
+        (b_f1_0, f'{label_prefix}f1_0_baseline'),
+        (b_f2_1, f'{label_prefix}f2_1_baseline'),
+        (b_f2_0, f'{label_prefix}f2_0_baseline'),
+
+        (precision_1 - b_precision_1, f'{label_prefix}dPrec_1'),
+        (precision_0 - b_precision_0, f'{label_prefix}dPrec_0'),
+        (f1_1 - b_f1_1, f'{label_prefix}dF1_1'),
+        (f1_0 - b_f1_0, f'{label_prefix}dF1_0'),
+        (f2_1 - b_f2_1, f'{label_prefix}dF2_1'),
+        (f2_0 - b_f2_0, f'{label_prefix}dF2_0'),
+    ])
+
+    return metric_list
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils/general/ogd_utils.py` & `OGDUtils-0.1.5/src/OGDUtils/general/ogd_utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-""" First Cell contents:
-#@markdown ###First Cell 
-#@markdown *Please paste this cell into any colab notebook for this project.* <br>
-#@markdown ***
-#@markdown **Contents**: Contents. <br>
-#@markdown ***
-#@markdown Major Edit History: 
-#@markdown - Author, Date: Created as copy of Old Notebook (`Old Title`).
-#@markdown ***
-#@markdown <br> 
-#@markdown Please change `FIELDDAY_DIR` if it is located differently in your drive. This cell will error if `FIELDDAY_DIR` is incorrect.
-# mount drive
-from google.colab import drive
-drive.mount('/content/drive')
-
-# Change working directory
-import os
-FIELDDAY_DIR = '/content/drive/My Drive/Field Day' #@param {type:"string"}
-JUPYTER_DIR = os.path.join(FIELDDAY_DIR,'Research and Writing Projects/2020 CHI Play - Lakeland Clustering/Jupyter')
-os.chdir(JUPYTER_DIR)
-print(f'---\nCWD: {os.getcwd()}')
-
-#@markdown Change pandas `max_rows` and `max_columns`
-import pandas as pd
-pd.options.display.max_columns = 100 #@param {type:"integer"}
-pd.options.display.max_rows = 60 #@param {type:"integer"}
-
-#@markdown *Note: There may be other variables to manually change. Look the "Set Variables" section.*
-
-# import utils
-import sys
-sys.path.append('.')
-import utils
-"""
-
-"""Save Cell contents:
-save = True #@param {type:"boolean"}
-savedir = 'Data/Full Data Tables/' #@param ["/", "Data/", "Data/Full Data Tables"] {allow-input: true}
-savedir = savedir if os.path.isdir(savedir) else 'Data/Full Data Tables'
-savename = '' #@param {type:"string"}
-savename = savename or f'Final CM-Cluster Output {DATE}.csv'
-savepath = os.path.join(savedir,savename)
-if save:
-  print(f'Saving to: {savepath}')
-else:
-  print(f'Not saving.')
-"""
-
-TEST_STR = 'hello'
-
-
-def apply_functions_to_df(df, function_list, verbose=False):
-    ret = df
-    if verbose:
-        print(f'df0 len = {len(ret)}')
-    for i, f in enumerate(function_list):
-        ret = f(ret)
-        if type(ret) is not int and verbose:
-            print(f'df{i + 1} len = {len(ret)}')
-    return ret
-
-
-def equal(col, val):
-    return lambda df: df.loc[df[col] == val, :]
-
-
-def match(col, regex, case=True, flags=0):
-    return lambda df: df.loc[df[col].str.match(regex, case, flags), :]
-
-
-def search(col, regex, case=True, flags=0):
-    return lambda df: df.loc[df[col].str.contains(regex, case, flags), :]
-
-
-def search2colsOR(col1, col2, regex):
-    return lambda df: df.loc[df[col1].str.contains(regex) | df[col2].str.contains(regex), :]
-
-
-def searchPair(col1, col2, regex1, regex2):
-    return lambda df: df.loc[(df[col1].str.contains(regex1) & df[col2].str.contains(regex2)) |
-                             (df[col1].str.contains(regex2) & df[col2].str.contains(regex1)), :]
-
-
-def sum_col(col):
-    return lambda df: df.loc[:, col].sum()
-
-
-def len_df():
-    return lambda df: len(df)
-
-
-def identity():
-    return lambda df: df
-
-
-"""
-Code snippet to add simple file selections to a Jupyter notebook:
-
-base_path = "/content/drive/My Drive/Field Day/Research and Writing Projects/2020 Lakeland EDM/Jupyter/Data/"
-folders = [fdir for fdir in os.listdir(base_path) if os.path.isdir(os.path.join(base_path, fdir))]
-folder_selector = widgets.Select(
-    options = folders,
-    value = folders[0],
-    description = "Folder",
-    layout = widgets.Layout(width='80%')
-)
-file_path = base_path + folder_selector.value
-files = [fdir for fdir in os.listdir(file_path) if os.path.isfile(os.path.join(file_path, fdir))]
-file_selector = widgets.Select(
-    options = files,
-    value = files[0],
-    description = "File",
-    layout = widgets.Layout(width='80%')
-)
-
-def updateFolder(change):
-  file_path = base_path + folder_selector.value
-  files = [fdir for fdir in os.listdir(file_path) if os.path.isfile(os.path.join(file_path, fdir))]
-  file_selector.options = files
-  file_selector.value = files[0]
-folder_selector.observe(updateFolder, names="value")
-
-display(folder_selector, file_selector)
-"""
-
-
-def write_csv_with_meta(df, path, meta_strings, mode='w+'):
-    with open(path, mode=mode) as f:
-        for l in meta_strings:
-            f.write(f'# {l}\n')
-        df.to_csv(f)
-
-
-import os
-
-
-# def init_path():
-#     import src.settings
-#     os.chdir(src.settings.BASE_DIR)
-
-
-# if __name__ == '__main__':
-#     init_path()
+""" First Cell contents:
+#@markdown ###First Cell 
+#@markdown *Please paste this cell into any colab notebook for this project.* <br>
+#@markdown ***
+#@markdown **Contents**: Contents. <br>
+#@markdown ***
+#@markdown Major Edit History: 
+#@markdown - Author, Date: Created as copy of Old Notebook (`Old Title`).
+#@markdown ***
+#@markdown <br> 
+#@markdown Please change `FIELDDAY_DIR` if it is located differently in your drive. This cell will error if `FIELDDAY_DIR` is incorrect.
+# mount drive
+from google.colab import drive
+drive.mount('/content/drive')
+
+# Change working directory
+import os
+FIELDDAY_DIR = '/content/drive/My Drive/Field Day' #@param {type:"string"}
+JUPYTER_DIR = os.path.join(FIELDDAY_DIR,'Research and Writing Projects/2020 CHI Play - Lakeland Clustering/Jupyter')
+os.chdir(JUPYTER_DIR)
+print(f'---\nCWD: {os.getcwd()}')
+
+#@markdown Change pandas `max_rows` and `max_columns`
+import pandas as pd
+pd.options.display.max_columns = 100 #@param {type:"integer"}
+pd.options.display.max_rows = 60 #@param {type:"integer"}
+
+#@markdown *Note: There may be other variables to manually change. Look the "Set Variables" section.*
+
+# import utils
+import sys
+sys.path.append('.')
+import utils
+"""
+
+"""Save Cell contents:
+save = True #@param {type:"boolean"}
+savedir = 'Data/Full Data Tables/' #@param ["/", "Data/", "Data/Full Data Tables"] {allow-input: true}
+savedir = savedir if os.path.isdir(savedir) else 'Data/Full Data Tables'
+savename = '' #@param {type:"string"}
+savename = savename or f'Final CM-Cluster Output {DATE}.csv'
+savepath = os.path.join(savedir,savename)
+if save:
+  print(f'Saving to: {savepath}')
+else:
+  print(f'Not saving.')
+"""
+
+TEST_STR = 'hello'
+
+
+def apply_functions_to_df(df, function_list, verbose=False):
+    ret = df
+    if verbose:
+        print(f'df0 len = {len(ret)}')
+    for i, f in enumerate(function_list):
+        ret = f(ret)
+        if type(ret) is not int and verbose:
+            print(f'df{i + 1} len = {len(ret)}')
+    return ret
+
+
+def equal(col, val):
+    return lambda df: df.loc[df[col] == val, :]
+
+
+def match(col, regex, case=True, flags=0):
+    return lambda df: df.loc[df[col].str.match(regex, case, flags), :]
+
+
+def search(col, regex, case=True, flags=0):
+    return lambda df: df.loc[df[col].str.contains(regex, case, flags), :]
+
+
+def search2colsOR(col1, col2, regex):
+    return lambda df: df.loc[df[col1].str.contains(regex) | df[col2].str.contains(regex), :]
+
+
+def searchPair(col1, col2, regex1, regex2):
+    return lambda df: df.loc[(df[col1].str.contains(regex1) & df[col2].str.contains(regex2)) |
+                             (df[col1].str.contains(regex2) & df[col2].str.contains(regex1)), :]
+
+
+def sum_col(col):
+    return lambda df: df.loc[:, col].sum()
+
+
+def len_df():
+    return lambda df: len(df)
+
+
+def identity():
+    return lambda df: df
+
+
+"""
+Code snippet to add simple file selections to a Jupyter notebook:
+
+base_path = "/content/drive/My Drive/Field Day/Research and Writing Projects/2020 Lakeland EDM/Jupyter/Data/"
+folders = [fdir for fdir in os.listdir(base_path) if os.path.isdir(os.path.join(base_path, fdir))]
+folder_selector = widgets.Select(
+    options = folders,
+    value = folders[0],
+    description = "Folder",
+    layout = widgets.Layout(width='80%')
+)
+file_path = base_path + folder_selector.value
+files = [fdir for fdir in os.listdir(file_path) if os.path.isfile(os.path.join(file_path, fdir))]
+file_selector = widgets.Select(
+    options = files,
+    value = files[0],
+    description = "File",
+    layout = widgets.Layout(width='80%')
+)
+
+def updateFolder(change):
+  file_path = base_path + folder_selector.value
+  files = [fdir for fdir in os.listdir(file_path) if os.path.isfile(os.path.join(file_path, fdir))]
+  file_selector.options = files
+  file_selector.value = files[0]
+folder_selector.observe(updateFolder, names="value")
+
+display(folder_selector, file_selector)
+"""
+
+
+def write_csv_with_meta(df, path, meta_strings, mode='w+'):
+    with open(path, mode=mode) as f:
+        for l in meta_strings:
+            f.write(f'# {l}\n')
+        df.to_csv(f)
+
+
+import os
+
+
+# def init_path():
+#     import src.settings
+#     os.chdir(src.settings.BASE_DIR)
+
+
+# if __name__ == '__main__':
+#     init_path()
```

### Comparing `OGDUtils-0.1.1/src/OGDUtils.egg-info/SOURCES.txt` & `OGDUtils-0.1.5/src/OGDUtils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+src/OGDUtils/__init__.py
 src/OGDUtils.egg-info/PKG-INFO
 src/OGDUtils.egg-info/SOURCES.txt
 src/OGDUtils.egg-info/dependency_links.txt
 src/OGDUtils.egg-info/top_level.txt
 src/OGDUtils/JOWILDER/__init__.py
 src/OGDUtils/JOWILDER/jowilder_utils.py
 src/OGDUtils/LAKELAND/__init__.py
```

