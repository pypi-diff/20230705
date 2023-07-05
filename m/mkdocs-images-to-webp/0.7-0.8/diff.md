# Comparing `tmp/mkdocs-images-to-webp-0.7.tar.gz` & `tmp/mkdocs-images-to-webp-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-images-to-webp-0.7.tar", last modified: Tue Jun 13 12:06:11 2023, max compression
+gzip compressed data, was "mkdocs-images-to-webp-0.8.tar", last modified: Wed Jul  5 10:45:14 2023, max compression
```

## Comparing `mkdocs-images-to-webp-0.7.tar` & `mkdocs-images-to-webp-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:06:11.427646 mkdocs-images-to-webp-0.7/
--rw-rw-rw-   0        0        0     1089 2023-01-23 18:45:26.000000 mkdocs-images-to-webp-0.7/LICENSE
--rw-rw-rw-   0        0        0      417 2023-06-13 12:06:11.427646 mkdocs-images-to-webp-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-06-13 06:01:42.000000 mkdocs-images-to-webp-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 12:06:11.409645 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp/
--rw-rw-rw-   0        0        0        0 2023-01-29 17:09:12.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-06-13 11:52:36.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp/plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:06:11.427646 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/
--rw-rw-rw-   0        0        0      417 2023-06-13 12:06:11.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-06-13 12:06:11.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:06:11.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-13 12:06:11.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-13 12:06:11.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-13 12:06:11.000000 mkdocs-images-to-webp-0.7/mkdocs_images_to_webp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      445 2023-06-13 11:53:05.000000 mkdocs-images-to-webp-0.7/pyproject.toml
--rw-rw-rw-   0        0        0      397 2023-06-13 12:06:11.429645 mkdocs-images-to-webp-0.7/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-06-13 12:05:09.000000 mkdocs-images-to-webp-0.7/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-01-25 09:31:29.000000 mkdocs-images-to-webp-0.8/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      407 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      648 2023-02-07 12:01:18.000000 mkdocs-images-to-webp-0.8/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-30 06:39:53.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1841 2023-07-05 10:40:35.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/plugin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      407 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      389 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       89 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      114 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      430 2023-07-05 10:45:03.000000 mkdocs-images-to-webp-0.8/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      597 2023-07-05 10:44:59.000000 mkdocs-images-to-webp-0.8/setup.py
```

### Comparing `mkdocs-images-to-webp-0.7/LICENSE` & `mkdocs-images-to-webp-0.8/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 mur4d1n-lib
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
+Copyright (c) 2023 mur4d1n-lib
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

### Comparing `mkdocs-images-to-webp-0.7/mkdocs_images_to_webp/plugin.py` & `mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from mkdocs.plugins import BasePlugin
-from mkdocs.config import base, config_options as c
-from PIL import Image
-import os
-
-
-class ConvertImagesToWebpPluginConfig(base.Config):
-    extensions = c.ListOfItems(c.Choice(('png', 'jpeg', 'jpg', 'bmp'), default='png'))
-    img_dir = c.Dir(default='docs/img')
-
-
-class ConvertImagesToWebpPlugin(BasePlugin[ConvertImagesToWebpPluginConfig]):
-    def clean(self, target_dir):
-        paths = os.listdir(target_dir)
-        for path in paths:
-            full_path = '/'.join([target_dir, path])
-            if os.path.isdir(full_path):
-                self.clean(full_path)
-            else:
-                if path.endswith('.webp'):
-                    os.remove(full_path)
-
-    def on_files(self, files, config):
-        extensions_local = list([extension for extension in self.config.extensions])
-        for file in files:
-            for extension in extensions_local:
-                if file.abs_src_path.endswith(extension) and file.abs_src_path.find(self.config.img_dir) + 1:
-                    image = Image.open(file.abs_src_path)
-                    file.abs_src_path = file.abs_src_path[:len(file.abs_src_path) - 4] + ".webp"
-                    image.save(file.abs_src_path, format='webp')
-                    file.abs_dest_path = file.abs_dest_path[:len(file.abs_src_path) - 4] + ".webp"
-                    break
-        print("INFO     -  [images-to-webp] Formats", ', '.join(extensions_local), 'successfully changed to webp')
-        return files
-
-    def on_page_content(self, html, page, config, files):
-        extensions_local = list([extension for extension in self.config.extensions])
-        for extension in extensions_local:
-            html = html.replace(extension, "webp")
-        return html
-
-    # def on_post_build(self, config):
-    #     target_dir = self.config.img_dir
-    #     self.clean(target_dir)
+from mkdocs.plugins import BasePlugin
+from mkdocs.config import base, config_options as c
+from PIL import Image
+import os
+
+
+class ConvertImagesToWebpPluginConfig(base.Config):
+    extensions = c.ListOfItems(c.Choice(('png', 'jpeg', 'jpg', 'bmp'), default='png'))
+    img_dir = c.Dir(default='docs/img')
+
+
+class ConvertImagesToWebpPlugin(BasePlugin[ConvertImagesToWebpPluginConfig]):
+    def clean(self, target_dir):
+        paths = os.listdir(target_dir)
+        for path in paths:
+            full_path = '/'.join([target_dir, path])
+            if os.path.isdir(full_path):
+                self.clean(full_path)
+            else:
+                if path.endswith('.webp'):
+                    os.remove(full_path)
+
+    def on_files(self, files, config):
+        extensions_local = list([extension for extension in self.config.extensions])
+        for file in files:
+            for extension in extensions_local:
+                if file.abs_src_path.endswith(extension):
+                    image = Image.open(file.abs_src_path)
+                    file.abs_src_path = file.abs_src_path[:len(file.abs_src_path) - 4] + ".webp"
+                    image.save(file.abs_src_path, format='webp')
+                    file.abs_dest_path = file.abs_dest_path[:len(file.abs_src_path) - 4] + ".webp"
+                    break
+        print("INFO     -  [images-to-webp] Formats", ', '.join(extensions_local), 'successfully changed to webp')
+        return files
+
+    def on_page_content(self, html, page, config, files):
+        extensions_local = list([extension for extension in self.config.extensions])
+        for extension in extensions_local:
+            html = html.replace(extension, extension + ".webp")
+        return html
+
+    # def on_post_build(self, config):
+    #     target_dir = self.config.img_dir
+    #     self.clean(target_dir)
```

