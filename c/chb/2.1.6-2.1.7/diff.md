# Comparing `tmp/chb-2.1.6.tar.gz` & `tmp/chb-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chb-2.1.6.tar", last modified: Mon May 22 06:30:11 2023, max compression
+gzip compressed data, was "chb-2.1.7.tar", last modified: Wed Jul  5 06:58:53 2023, max compression
```

## Comparing `chb-2.1.6.tar` & `chb-2.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 06:30:11.433036 chb-2.1.6/
--rw-rw-rw-   0        0        0     1091 2023-04-07 05:55:28.000000 chb-2.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0      637 2023-05-22 06:30:11.433036 chb-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-07 05:55:28.000000 chb-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 06:30:11.428049 chb-2.1.6/chb/
--rw-rw-rw-   0        0        0     5506 2023-05-22 06:29:52.000000 chb-2.1.6/chb/__init__.py
--rw-rw-rw-   0        0        0     8851 2023-04-20 15:09:42.000000 chb-2.1.6/chb/_dao.py
--rw-rw-rw-   0        0        0     3424 2023-04-07 05:55:28.000000 chb-2.1.6/chb/_importable.py
--rw-rw-rw-   0        0        0     4038 2023-05-22 06:17:54.000000 chb-2.1.6/chb/_imports.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 05:55:28.000000 chb-2.1.6/chb/_log.py
--rw-rw-rw-   0        0        0    26819 2023-05-22 06:20:18.000000 chb-2.1.6/chb/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:30:11.431041 chb-2.1.6/chb.egg-info/
--rw-rw-rw-   0        0        0      637 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-22 06:30:11.433442 chb-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-05-22 06:27:10.000000 chb-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:58:53.136761 chb-2.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-04-07 05:55:28.000000 chb-2.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      637 2023-07-05 06:58:53.136761 chb-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-07 05:55:28.000000 chb-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 06:58:53.131263 chb-2.1.7/chb/
+-rw-rw-rw-   0        0        0     5506 2023-05-22 06:29:52.000000 chb-2.1.7/chb/__init__.py
+-rw-rw-rw-   0        0        0     8851 2023-04-20 15:09:42.000000 chb-2.1.7/chb/_dao.py
+-rw-rw-rw-   0        0        0     3424 2023-04-07 05:55:28.000000 chb-2.1.7/chb/_importable.py
+-rw-rw-rw-   0        0        0     4038 2023-05-22 06:17:54.000000 chb-2.1.7/chb/_imports.py
+-rw-rw-rw-   0        0        0     4640 2023-06-02 03:44:03.000000 chb-2.1.7/chb/_log.py
+-rw-rw-rw-   0        0        0    29780 2023-07-03 08:36:06.000000 chb-2.1.7/chb/_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 06:58:53.135324 chb-2.1.7/chb.egg-info/
+-rw-rw-rw-   0        0        0      637 2023-07-05 06:58:53.000000 chb-2.1.7/chb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-05 06:58:53.000000 chb-2.1.7/chb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 06:58:53.000000 chb-2.1.7/chb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-05 06:58:53.000000 chb-2.1.7/chb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-05 06:58:53.136761 chb-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-07-05 06:58:49.000000 chb-2.1.7/setup.py
```

### Comparing `chb-2.1.6/LICENSE.txt` & `chb-2.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chb-2.1.6/PKG-INFO` & `chb-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chb
-Version: 2.1.6
+Version: 2.1.7
 Summary: chb常用代码库
 Home-page: https://github.com/ChenHuabin321/pypi
 Author: chenhuabin
 Author-email: chenhuabin321@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chb-2.1.6/chb/__init__.py` & `chb-2.1.7/chb/__init__.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.6/chb/_dao.py` & `chb-2.1.7/chb/_dao.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.6/chb/_importable.py` & `chb-2.1.7/chb/_importable.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.6/chb/_imports.py` & `chb-2.1.7/chb/_imports.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.6/chb/_log.py` & `chb-2.1.7/chb/_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,26 +87,26 @@
                         break
             else:
                 log_file = os.path.join(log_dir, f'{self.logger_name}.log')
                 file_handler = logging.FileHandler(log_file, encoding='UTF-8')
                 file_handler.setFormatter(file_logging_format)
                 self.logger.addHandler(file_handler)
 
-    def __call__(self, level='info'):
+    def __call__(self, level=None):
         """
         如果level为None，则返回日志器，否则返回对应等级的输出函数：debug、info等
         :param level:
         :return:
         """
         if level:
             return getattr(self.logger, level)
         else:
             return self.logger
 
-    def getLogger(self, level='info'):
+    def getLogger(self, level=None):
         """
         如果level为None，则返回日志器，否则返回对应等级的输出函数：debug、info等
         :param level:
         :return:
         """
         return self.__call__(level)
```

### Comparing `chb-2.1.6/chb/_utils.py` & `chb-2.1.7/chb/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -636,15 +636,15 @@
         """
         逐行读取文件内容，返回一个生成器。
         """
         while True:
             line = self.f.readline()
             if not line:
                 break
-            yield line
+            yield line.rstrip('\n')
 
     def readlines(self, num_lines=100000):
         """
         按指定数量的行数读取文件内容，返回一个生成器。
 
         参数:
         num_lines: 每次读取的行数，默认为100000行
@@ -668,10 +668,64 @@
         if isinstance(img, torch.Tensor):  # 如果是torch.Tensor类型，就必须转换成Pillow.Image类型，才能进行展示
             img = transforms.ToPILImage()(img)
         axs[0, i].imshow(np.asarray(img), **imshow_kwargs)
         # axs[0, i].set(xticklabels=[], yticklabels=[], xticks=[], yticks=[])
         axs[0, i].set_title(title)
     plt.show()
 
+class EarlyStopping:
+    """
+    如果验证性能（损失或者准确率）在连续指定个轮次后没有得到改善，则提前停止训练。
+    """
+    def __init__(self,
+                 patience=7,
+                 delta=0,
+                 full_model_name='./models/model.pth',
+                 loss_or_accuracy='loss'):
+        """
+        Args:
+            patience (int): 上次验证集损失值改善后等待多少个epoch，如果在这期间没有进一步改善，则进行提前停止。
+                            默认值: 7
+            delta (float): 监测数量的最小变化，只有高于这个值的变化才被认定为实质改进。
+                            默认值: 0
+            full_model_name (str): 最佳模型的保存路径。
+                            默认值: './models/model.pth'
+            loss_or_accuracy (str): 选择基于哪个指标进行早停，可以选择"loss"或者"accuracy"。
+                            默认值: 'loss'
+        """
+        self.patience = patience
+        self.counter = 0  # 计数器，用于记录从上次最佳分数后经过了多少个epoch
+        self.best_score = None  # 记录最佳分数
+        self.best_epoch = False  # 标记当前epoch是否为最佳epoch
+        self.early_stop = False  # 标记是否提前停止
+        self.delta = delta  # 最小改进值
+        self.loss_or_accuracy = loss_or_accuracy  # 基于哪个指标进行早停
+        self.full_model_name = full_model_name  # 最佳模型的保存路径
+
+    def __call__(self, model, score):
+        # 如果选择的是损失值作为早停的依据，则为了方便比较，转为负数
+        if self.loss_or_accuracy == 'loss':
+            score = -score
+        # 如果尚未记录过最佳分数，将当前分数设为最佳分数，并保存当前模型
+        if self.best_score is None:
+            self.best_score = score
+            self.best_epoch = True
+            torch.save(model, self.full_model_name)
+        # 如果当前分数小于或等于最佳分数（如果选择的是损失值作为早停的依据，这里的小于实际上是大于）
+        # 计数器加一，表示没有进一步改进
+        elif score <= self.best_score + self.delta:
+            self.counter += 1
+            self.best_epoch = False
+            # 如果没有进一步改进的epoch数量达到了设定的耐心值，进行提前停止
+            if self.counter >= self.patience:
+                self.early_stop = True
+        # 如果当前分数大于最佳分数（如果选择的是损失值作为早停的依据，这里的大于实际上是小于）
+        # 更新最佳分数，并保存当前模型，计数器重置为0
+        else:
+            self.best_score = score
+            self.best_epoch = True
+            torch.save(model, self.full_model_name)
+            self.counter = 0
+
 
 if __name__=='__main__':
     print(Timer.datebetween('2022-01-01 00:00:00', '2022-01-04 00:00:00'))
```

### Comparing `chb-2.1.6/chb.egg-info/PKG-INFO` & `chb-2.1.7/chb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chb
-Version: 2.1.6
+Version: 2.1.7
 Summary: chb常用代码库
 Home-page: https://github.com/ChenHuabin321/pypi
 Author: chenhuabin
 Author-email: chenhuabin321@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chb-2.1.6/setup.py` & `chb-2.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chb",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="2.1.6",  # 包版本号，便于维护版本
+    version="2.1.7",  # 包版本号，便于维护版本
     author="chenhuabin",  # 作者，可以写自己的姓名
     author_email="chenhuabin321@163.com",  # 作者联系方式，可写自己的邮箱地址
     description="chb常用代码库",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/ChenHuabin321/pypi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

