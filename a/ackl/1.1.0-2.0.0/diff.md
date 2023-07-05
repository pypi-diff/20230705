# Comparing `tmp/ackl-1.1.0.tar.gz` & `tmp/ackl-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ackl-1.1.0.tar", last modified: Mon Jul  3 01:26:03 2023, max compression
+gzip compressed data, was "ackl-2.0.0.tar", last modified: Wed Jul  5 10:21:30 2023, max compression
```

## Comparing `ackl-1.1.0.tar` & `ackl-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.403746 ackl-1.1.0/
--rw-rw-rw-   0        0        0     1087 2022-09-05 02:47:29.000000 ackl-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       53 2023-07-01 14:25:20.000000 ackl-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1691 2023-07-03 01:26:03.403746 ackl-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1100 2023-07-01 14:02:39.000000 ackl-1.1.0/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 ackl-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      900 2023-07-03 01:26:03.406744 ackl-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.336745 ackl-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.353742 ackl-1.1.0/src/ackl/
--rw-rw-rw-   0        0        0      160 2023-06-30 14:07:27.000000 ackl-1.1.0/src/ackl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.383741 ackl-1.1.0/src/ackl/gui/
--rw-rw-rw-   0        0        0        0 2023-01-31 05:39:02.000000 ackl-1.1.0/src/ackl/gui/__init__.py
--rw-rw-rw-   0        0        0     2637 2023-07-01 14:04:30.000000 ackl-1.1.0/src/ackl/gui/run.py
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.396748 ackl-1.1.0/src/ackl/gui/static/
--rw-rw-rw-   0        0        0   202389 2023-01-16 12:00:51.000000 ackl-1.1.0/src/ackl/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   136072 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    86929 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0    24228 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17131 2022-11-14 06:36:33.000000 ackl-1.1.0/src/ackl/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0  1477676 2022-12-23 14:00:42.000000 ackl-1.1.0/src/ackl/gui/static/sample.csv
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.401747 ackl-1.1.0/src/ackl/gui/templates/
--rw-rw-rw-   0        0        0    13445 2023-03-31 05:31:00.000000 ackl-1.1.0/src/ackl/gui/templates/home.html
--rw-rw-rw-   0        0        0    38912 2023-07-01 02:44:57.000000 ackl-1.1.0/src/ackl/kernels.py
--rw-rw-rw-   0        0        0    29083 2023-07-03 00:51:01.000000 ackl-1.1.0/src/ackl/metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-03 01:26:03.379738 ackl-1.1.0/src/ackl.egg-info/
--rw-rw-rw-   0        0        0     1691 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-03 01:26:03.000000 ackl-1.1.0/src/ackl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:30.339710 ackl-2.0.0/
+-rw-rw-rw-   0        0        0     1087 2022-09-05 02:47:29.000000 ackl-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-07-01 14:25:20.000000 ackl-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1691 2023-07-05 10:21:30.339710 ackl-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2023-07-01 14:02:39.000000 ackl-2.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 ackl-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      900 2023-07-05 10:21:30.342710 ackl-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:29.913891 ackl-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:30.115046 ackl-2.0.0/src/ackl/
+-rw-rw-rw-   0        0        0      160 2023-07-03 03:16:49.000000 ackl-2.0.0/src/ackl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:30.152589 ackl-2.0.0/src/ackl/gui/
+-rw-rw-rw-   0        0        0        0 2023-01-31 05:39:02.000000 ackl-2.0.0/src/ackl/gui/__init__.py
+-rw-rw-rw-   0        0        0     2670 2023-07-03 10:46:50.000000 ackl-2.0.0/src/ackl/gui/run.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:30.317214 ackl-2.0.0/src/ackl/gui/static/
+-rw-rw-rw-   0        0        0   202389 2023-01-16 12:00:51.000000 ackl-2.0.0/src/ackl/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   136072 2022-11-14 06:36:33.000000 ackl-2.0.0/src/ackl/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    86929 2022-11-14 06:36:33.000000 ackl-2.0.0/src/ackl/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0    24228 2022-11-14 06:36:33.000000 ackl-2.0.0/src/ackl/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17131 2022-11-14 06:36:33.000000 ackl-2.0.0/src/ackl/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0  1477676 2022-12-23 14:00:42.000000 ackl-2.0.0/src/ackl/gui/static/sample.csv
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:30.338711 ackl-2.0.0/src/ackl/gui/templates/
+-rw-rw-rw-   0        0        0    13445 2023-03-31 05:31:00.000000 ackl-2.0.0/src/ackl/gui/templates/home.html
+-rw-rw-rw-   0        0        0    38912 2023-07-01 02:44:57.000000 ackl-2.0.0/src/ackl/kernels.py
+-rw-rw-rw-   0        0        0    29166 2023-07-03 11:05:54.000000 ackl-2.0.0/src/ackl/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:30.148600 ackl-2.0.0/src/ackl.egg-info/
+-rw-rw-rw-   0        0        0     1691 2023-07-05 10:21:29.000000 ackl-2.0.0/src/ackl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-07-05 10:21:29.000000 ackl-2.0.0/src/ackl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:21:29.000000 ackl-2.0.0/src/ackl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-05 10:21:29.000000 ackl-2.0.0/src/ackl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 10:21:29.000000 ackl-2.0.0/src/ackl.egg-info/top_level.txt
```

### Comparing `ackl-1.1.0/LICENSE` & `ackl-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/PKG-INFO` & `ackl-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ackl
-Version: 1.1.0
+Version: 2.0.0
 Summary: A Python library for kernels used in analytical chemistry
 Home-page: https://github.com/zhangys11/ack
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/ack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ackl-1.1.0/README.md` & `ackl-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/setup.cfg` & `ackl-2.0.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 636b 6c0d 0a76 6572 7369 6f6e   = ackl..version
-00000020: 203d 2031 2e31 2e30 0d0a 6175 7468 6f72   = 1.1.0..author
+00000020: 203d 2032 2e30 2e30 0d0a 6175 7468 6f72   = 2.0.0..author
 00000030: 203d 2059 696e 7368 656e 6720 5a68 616e   = Yinsheng Zhan
 00000040: 6720 2850 682e 442e 290d 0a61 7574 686f  g (Ph.D.)..autho
 00000050: 725f 656d 6169 6c20 3d20 6f6f 407a 6a75  r_email = oo@zju
 00000060: 2e65 6475 2e63 6e0d 0a64 6573 6372 6970  .edu.cn..descrip
 00000070: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
 00000080: 6c69 6272 6172 7920 666f 7220 6b65 726e  library for kern
 00000090: 656c 7320 7573 6564 2069 6e20 616e 616c  els used in anal
```

### Comparing `ackl-1.1.0/src/ackl/gui/run.py` & `ackl-2.0.0/src/ackl/gui/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             r += io.scatter_plot(X, y, labels=labels, output_html=True)
 
         r += '<p>' + desc + '</p><hr/>'
         r += '<h6>Kernel Transformation</h6>'
 
         _, dic_test_accs, dic, s = metrics.classify_with_kernels(X, y, scale = True,
                                         do_cla=True,
-                                        run_clfs=True,
+                                        clfs='all', # ['LinearDiscriminantAnalysis()'],
                                         plots=True,
                                         logplot=True,
                                         output_html= True,
                                         selected_kernel_names = kernel_type)
 
         r += s
         r += metrics.visualize_metric_dicts(dic, plot=False)
```

### Comparing `ackl-1.1.0/src/ackl/gui/static/bootstrap.css` & `ackl-2.0.0/src/ackl/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/gui/static/bootstrap.js` & `ackl-2.0.0/src/ackl/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/gui/static/jquery-3.3.1.min.js` & `ackl-2.0.0/src/ackl/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/gui/static/jquery.blockUI.js` & `ackl-2.0.0/src/ackl/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/gui/static/jquery.form.min.js` & `ackl-2.0.0/src/ackl/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/gui/static/sample.csv` & `ackl-2.0.0/src/ackl/gui/static/sample.csv`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/gui/templates/home.html` & `ackl-2.0.0/src/ackl/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/kernels.py` & `ackl-2.0.0/src/ackl/kernels.py`

 * *Files identical despite different names*

### Comparing `ackl-1.1.0/src/ackl/metrics.py` & `ackl-2.0.0/src/ackl/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
     Parameter
     ---------
     cmap : color map scheme
     '''
     X = np.array([0, 1]).reshape(-1, 1)
     _ = classify_with_kernels(X, np.array(
-        [0, 1]), cmap, None, scale=True, run_clfs=False, do_cla=False)
+        [0, 1]), cmap, None, scale=True, clfs=[], do_cla=False)
 
 
 def linear_response_pattern(n=10, dim=1, cmap='gray'):
     '''
     Generates a response pattern of pairwise-point-distances.
     See how each kernel responds to / varies with linearly arranged points.
 
@@ -196,20 +196,20 @@
 
     if dim == 2:
         zeros = np.array([0] * n).reshape(-1, 1)
         X = np.vstack((np.hstack((X, zeros)), np.hstack((zeros, X))))
         y = [0] * n + [1] * n
 
     _ = classify_with_kernels(X, np.array(y), cmap, hyper_param_optimizer = None,
-                        scale = True, run_clfs = False, do_cla = False,
+                        scale = True, clfs = [], do_cla = False,
                         plots = True, embed_title = False, verbose = False)
 
 
 def classify_with_kernels(X, y, cmap=None, hyper_param_optimizer=kes,
-                    scale=False, run_clfs=True, do_cla = False,
+                    scale=False, clfs=['LinearDiscriminantAnalysis()'], do_cla = False,
                     multi_kernels=[1], multi_kernel_topk=-1,
                     logplot=False, plots=True, embed_title=False,
                     output_html=False,
                     selected_kernel_names=None, verbose = True):
     '''
     Try various kernel types for classification task.  
     Each kernel uses their own default/empirical paramters.    
@@ -224,15 +224,15 @@
     y : class labels
     cmap : color map scheme to use. set None to use default, or set another scheme, e.g., 'gray', 'viridis', 'jet', 'rainbow', etc.
         For small dataset, we recommend 'gray'. For complex dataset, we recommend 'viridis'.
     hyper_param_optimizer : which optimizer to optimize the hyper parameters for each kernel. 
         For real-world dataset, use kes by default. For toy dataset, set None to disable optimizer.
         For multi-class dataset (y has more than 5 classes), use acc.
     scale : whether do feature scaling
-    run_clfs : whether run multiple classfiers and show confusion matrices
+    clfs : a list of multi-class classfiers. pass 'all' to use all available classifiers.
     multi_kernels : how many kernels to use. Default is [1].
     multi_kernel_topk : the k best single kernels to use in multi-kernel combinations. Default is 5.
     logplot : whether to output the log-scale plot in parallel.
     plots : whether to ouptut the kernel heatmaps and the scatter plots after PCA / PLS, to check classifiability.
         The PLS tries to maximize the covariance between X and Y.
     embed_title : whether embed the title in the plots. If not, will generate the title in HTML.
     do_cla : whether to do classifiability analysis using the cla package.
@@ -244,17 +244,17 @@
     all_dic_metrics = {}
     html_str = ''
 
     if scale:
         X = MinMaxScaler().fit_transform(X)
         print('perform min-max scaling')
 
-    if run_clfs:
+    if clfs == 'all' or len(clfs) > 0:
         result_html = '<h3>0. no kernel</h3><p>Classification on original dataset</p>'
-        dic, mc_html = run_multiclass_clfs(X, y, clfs=['LinearDiscriminantAnalysis()'], show = False)
+        dic, mc_html = run_multiclass_clfs(X, y, clfs=clfs, show = False)
         dic_test_accs['no kernel'] = dic
         result_html += mc_html
         if output_html:
             html_str += result_html
         if plots:
             IPython.display.display(IPython.display.HTML(result_html))
 
@@ -411,34 +411,34 @@
                     if verbose:
                         print('Exception : ', e)
                     # print('X_pls = ', X_pls)
                     # plt.title('PLS')
                     html_str += '<p>' + str(e) + '</p>'
 
         ###### Classifiction after kernel transformation #######
-        if run_clfs:
+        if clfs == 'all' or len(clfs) > 0:
             # result_html = '<h3>classification</h3>'
-            dic, result_html = run_multiclass_clfs(kns, y, clfs=['LinearDiscriminantAnalysis()'], show = False)
+            dic, result_html = run_multiclass_clfs(kns, y, clfs=clfs, show = False)
             dic_test_accs[key] = dic
             if output_html:
                 html_str += result_html
             if plots:
                 IPython.display.display(IPython.display.HTML(result_html))
 
         ###### cla metrics ######
-        if do_cla: # disable for now
+        if do_cla: # disable for now, keep just for reproduce historical results
             kns = np.nan_to_num(np.hstack((kns, np.array(y).reshape(-1, 1))),   # do nan filtering simultaneously for X and y
                                 nan=0, posinf=kns.max(), neginf=kns.min())
             _, dic_metrics = get_metrics(kns[:, :-1], kns[:, -1].flatten(), verbose = verbose)
             # dic_metrics['NMD'] = metric_nmd
             all_dic_metrics[key] = dic_metrics
 
-    pickle.dump((KX, dic_test_accs), open('single_kernels.pkl', 'wb'))
+    pickle.dump((KX, dic_test_accs, y), open('single_kernels.pkl', 'wb'))
 
-    if run_clfs: # multi-kernel cases
+    if clfs == 'all' or len(clfs) > 0: # multi-kernel cases
 
         # find top k kernels
         best_KX = {}
         best_top1s = {}
         for k,v in dic_test_accs.items():
             if k == 'no kernel':
                 continue
@@ -459,28 +459,28 @@
         for k in sorted_dict: # sorted(best_top1s.items(),  key = lambda kv:(kv[1], kv[0]), reverse=True):
             best_KX[k] = KX[k]
             if multi_kernel_topk != -1 and len(best_KX) >= multi_kernel_topk:
                 break
 
         for multi_kernel in multi_kernels:
 
-            if multi_kernel == 1: # single kernel case, skip
-                continue
+            # if multi_kernel == 1: # single kernel case, skip
+            #     continue
 
             for idx, ks in enumerate(combinations(best_KX, multi_kernel)):
                 combined = np.zeros((len(y),0))
                 mk_title = ''
                 for iidx, k in enumerate(ks):
                     if iidx == 0:
                         mk_title += k
                     else:
                         mk_title += ' + ' + k
                     combined = np.hstack((combined, KX[k]))
                 
-                dic, result_html = run_multiclass_clfs(combined, y, clfs=['LinearDiscriminantAnalysis()'], show = False)
+                dic, result_html = run_multiclass_clfs(combined, y, clfs=clfs, show = False)
                 result_html = '<h3>' + str(multi_kernel) + '-kernel ' + str(idx+1) + '. ' + mk_title + '</h3>' + result_html
                 dic_test_accs[mk_title] = dic
                 if output_html:
                     html_str += result_html
                 if plots:
                     IPython.display.display(IPython.display.HTML(result_html))
 
@@ -492,21 +492,22 @@
     '''
 
     top1_accs = []
     top3_accs = []
     top5_accs = []
     html_str = '<table>'
     for k, v in dic_test_accs.items():
-        accs = [str(round(x,3)) for x in list(v.values())[0]]
-        top1_accs.append(list(v.values())[0][0])
-        top3_accs.append(list(v.values())[0][1])
-        top5_accs.append(list(v.values())[0][2])
-        html_str += '<tr>' + '<td>' + k + '</td>' + '<td>' + accs[0] + '</td>' + '<td>' + accs[1] + '</td>' + '<td>' + accs[2] + '</td></tr>'
+        for kk, vv in v.items():
+            accs = [str(round(x,3)) for x in vv]
+            top1_accs.append(vv[0])
+            top3_accs.append(vv[1])
+            top5_accs.append(vv[2])
+            html_str += '<tr>' + '<td>' + k + '</td>'  + '<td>' + kk + '</td>' + '<td>' + accs[0] + '</td>' + '<td>' + accs[1] + '</td>' + '<td>' + accs[2] + '</td></tr>'
 
-    html_str += '<tr>' + '<td>best</td>' + '<td>' + \
+    html_str += '<tr>' + '<td>best</td>' + '<td></td>' + '<td>' + \
     str(round(np.max(top1_accs),3)) + '</td>' + '<td>' + \
     str(round(np.max(top3_accs),3)) + '</td>' + '<td>' + \
     str(round(np.max(top5_accs),3)) + '</td></tr>'
 
     html_str += '</table>'
     IPython.display.display(IPython.display.HTML(html_str))
```

### Comparing `ackl-1.1.0/src/ackl.egg-info/PKG-INFO` & `ackl-2.0.0/src/ackl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ackl
-Version: 1.1.0
+Version: 2.0.0
 Summary: A Python library for kernels used in analytical chemistry
 Home-page: https://github.com/zhangys11/ack
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/ack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ackl-1.1.0/src/ackl.egg-info/SOURCES.txt` & `ackl-2.0.0/src/ackl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

