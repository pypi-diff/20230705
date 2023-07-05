# Comparing `tmp/pygame_texteditor-0.7.2.tar.gz` & `tmp/pygame_texteditor-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_texteditor-0.7.2.tar", max compression
+gzip compressed data, was "pygame_texteditor-0.7.3.tar", max compression
```

## Comparing `pygame_texteditor-0.7.2.tar` & `pygame_texteditor-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1092 2023-04-21 05:19:33.913074 pygame_texteditor-0.7.2/LICENSE
--rw-r--r--   0        0        0     1541 2023-07-04 06:29:34.882202 pygame_texteditor-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-04-21 05:19:33.919070 pygame_texteditor-0.7.2/README.md
--rw-r--r--   0        0        0       36 2023-04-21 05:19:33.950069 pygame_texteditor-0.7.2/src/pygame_texteditor/__init__.py
--rw-r--r--   0        0        0     3924 2023-04-21 05:19:33.955070 pygame_texteditor-0.7.2/src/pygame_texteditor/_caret.py
--rw-r--r--   0        0        0     5444 2023-04-21 05:19:33.961071 pygame_texteditor-0.7.2/src/pygame_texteditor/_customization.py
--rw-r--r--   0        0        0     1783 2023-04-21 05:19:33.966070 pygame_texteditor-0.7.2/src/pygame_texteditor/_editor_getters.py
--rw-r--r--   0        0        0    17455 2023-04-21 05:19:33.970069 pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard.py
--rw-r--r--   0        0        0     9639 2023-04-21 05:19:33.976071 pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard_highlight.py
--rw-r--r--   0        0        0     8518 2023-04-21 05:19:33.981071 pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_mouse.py
--rw-r--r--   0        0        0     1428 2023-04-21 05:19:33.985071 pygame_texteditor-0.7.2/src/pygame_texteditor/_letter_operations.py
--rw-r--r--   0        0        0     1503 2023-04-21 05:19:33.989069 pygame_texteditor-0.7.2/src/pygame_texteditor/_other.py
--rw-r--r--   0        0        0     8041 2023-04-21 05:19:33.995071 pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering.py
--rw-r--r--   0        0        0     5117 2023-04-21 05:19:34.000069 pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_highlighting.py
--rw-r--r--   0        0        0     1072 2023-04-21 05:19:34.005071 pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_syntax_coloring.py
--rw-r--r--   0        0        0     1852 2023-04-21 05:19:34.011074 pygame_texteditor-0.7.2/src/pygame_texteditor/_scrollbar_vertical.py
--rw-r--r--   0        0        0     2094 2023-04-21 05:19:34.016074 pygame_texteditor-0.7.2/src/pygame_texteditor/_usage.py
--rw-r--r--   0        0        0     3428 2023-04-21 05:19:33.945073 pygame_texteditor-0.7.2/src/pygame_texteditor/ColorFormatter.py
--rw-r--r--   0        0        0      468 2023-04-21 05:19:34.017073 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/colorstyles/bright.yml
--rw-r--r--   0        0        0      469 2023-04-21 05:19:34.017073 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/colorstyles/dark.yml
--rw-r--r--   0        0        0    59516 2023-04-21 05:19:34.018073 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/fonts/Courier.ttf
--rw-r--r--   0        0        0      211 2023-04-21 05:19:34.019070 pygame_texteditor-0.7.2/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
--rw-r--r--   0        0        0    10327 2023-07-04 06:29:01.697222 pygame_texteditor-0.7.2/src/pygame_texteditor/TextEditor.py
--rw-r--r--   0        0        0     7875 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-21 05:19:33.913074 pygame_texteditor-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1541 2023-07-05 06:50:46.709545 pygame_texteditor-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     6965 2023-07-05 06:50:46.705549 pygame_texteditor-0.7.3/README.md
+-rw-r--r--   0        0        0       36 2023-04-21 05:19:33.950069 pygame_texteditor-0.7.3/src/pygame_texteditor/__init__.py
+-rw-r--r--   0        0        0     3924 2023-04-21 05:19:33.955070 pygame_texteditor-0.7.3/src/pygame_texteditor/_caret.py
+-rw-r--r--   0        0        0     5517 2023-07-05 06:50:46.714544 pygame_texteditor-0.7.3/src/pygame_texteditor/_customization.py
+-rw-r--r--   0        0        0     1783 2023-04-21 05:19:33.966070 pygame_texteditor-0.7.3/src/pygame_texteditor/_editor_getters.py
+-rw-r--r--   0        0        0    17455 2023-04-21 05:19:33.970069 pygame_texteditor-0.7.3/src/pygame_texteditor/_input_handling_keyboard.py
+-rw-r--r--   0        0        0     9639 2023-04-21 05:19:33.976071 pygame_texteditor-0.7.3/src/pygame_texteditor/_input_handling_keyboard_highlight.py
+-rw-r--r--   0        0        0     8518 2023-04-21 05:19:33.981071 pygame_texteditor-0.7.3/src/pygame_texteditor/_input_handling_mouse.py
+-rw-r--r--   0        0        0     1428 2023-04-21 05:19:33.985071 pygame_texteditor-0.7.3/src/pygame_texteditor/_letter_operations.py
+-rw-r--r--   0        0        0     1503 2023-04-21 05:19:33.989069 pygame_texteditor-0.7.3/src/pygame_texteditor/_other.py
+-rw-r--r--   0        0        0     8041 2023-04-21 05:19:33.995071 pygame_texteditor-0.7.3/src/pygame_texteditor/_rendering.py
+-rw-r--r--   0        0        0     5117 2023-04-21 05:19:34.000069 pygame_texteditor-0.7.3/src/pygame_texteditor/_rendering_highlighting.py
+-rw-r--r--   0        0        0     1072 2023-04-21 05:19:34.005071 pygame_texteditor-0.7.3/src/pygame_texteditor/_rendering_syntax_coloring.py
+-rw-r--r--   0        0        0     1852 2023-04-21 05:19:34.011074 pygame_texteditor-0.7.3/src/pygame_texteditor/_scrollbar_vertical.py
+-rw-r--r--   0        0        0     2094 2023-04-21 05:19:34.016074 pygame_texteditor-0.7.3/src/pygame_texteditor/_usage.py
+-rw-r--r--   0        0        0     3428 2023-04-21 05:19:33.945073 pygame_texteditor-0.7.3/src/pygame_texteditor/ColorFormatter.py
+-rw-r--r--   0        0        0      497 2023-07-05 06:50:46.719546 pygame_texteditor-0.7.3/src/pygame_texteditor/elements/colorstyles/bright.yml
+-rw-r--r--   0        0        0      498 2023-07-05 06:50:46.723546 pygame_texteditor-0.7.3/src/pygame_texteditor/elements/colorstyles/dark.yml
+-rw-r--r--   0        0        0    59516 2023-04-21 05:19:34.018073 pygame_texteditor-0.7.3/src/pygame_texteditor/elements/fonts/Courier.ttf
+-rw-r--r--   0        0        0      211 2023-04-21 05:19:34.019070 pygame_texteditor-0.7.3/src/pygame_texteditor/elements/graphics/Scroll_Bar.png
+-rw-r--r--   0        0        0    10327 2023-07-04 06:29:01.697222 pygame_texteditor-0.7.3/src/pygame_texteditor/TextEditor.py
+-rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 pygame_texteditor-0.7.3/PKG-INFO
```

### Comparing `pygame_texteditor-0.7.2/LICENSE` & `pygame_texteditor-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/pyproject.toml` & `pygame_texteditor-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygame-texteditor"
-version = "0.7.2"
+version = "0.7.3"
 description = "A WYSIWYG-texteditor based on pygame."
 authors = ["Victor Seifert <seifert.victor@web.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pygame_texteditor", from="src"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `pygame_texteditor-0.7.2/README.md` & `pygame_texteditor-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,17 @@
 **Editor colors** (source: bright.yml)
 
 - `codingBackgroundColor: (255, 255, 255)`
 - `codingScrollBarBackgroundColor: (49, 50, 50)`
 - `lineNumberColor: (255, 255, 255)`
 - `lineNumberBackgroundColor: (60, 61, 61)`
 - `textColor: (255, 255, 255)`
+- `caretColor: (255, 255, 255)`
 
-** Syntax colors** (source: bright.yml)
+**Syntax colors** (source: bright.yml)
 
 - `textColor_normal: (0, 255, 255)`
 - `textColor_comments: (119, 115, 115)`
 - `textColor_quotes: (227, 215, 115)`
 - `textColor_operators: (237, 36, 36)`
 - `textColor_keywords: (237, 36, 36)`
 - `textColor_function: (50, 150, 36)`
```

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_caret.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_caret.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_customization.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_customization.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             color_dict = yaml.load(file, Loader=yaml.FullLoader)
 
             self.color_coding_background = get_rgb_by_key(color_dict, "codingBackgroundColor")
             self.color_scrollbar_background = get_rgb_by_key(color_dict, "codingScrollBarBackgroundColor")
             self.color_line_number_font = get_rgb_by_key(color_dict, "lineNumberColor")
             self.color_line_number_background = get_rgb_by_key(color_dict, "lineNumberBackgroundColor")
             self.color_text = get_rgb_by_key(color_dict, "textColor")
+            self.color_caret = get_rgb_by_key(color_dict, "caretColor")
 
             self.color_formatter.textColor_normal = get_rgb_by_key(color_dict, "textColor_normal")
             self.color_formatter.textColor_comments = get_rgb_by_key(color_dict, "textColor_comments")
             self.color_formatter.textColor_quotes = get_rgb_by_key(color_dict, "textColor_quotes")
             self.color_formatter.textColor_operators = get_rgb_by_key(color_dict, "textColor_operators")
             self.color_formatter.textColor_keywords = get_rgb_by_key(color_dict, "textColor_keywords")
             self.color_formatter.textColor_function = get_rgb_by_key(color_dict, "textColor_function")
```

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_editor_getters.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_editor_getters.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_input_handling_keyboard.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_keyboard_highlight.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_input_handling_keyboard_highlight.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_input_handling_mouse.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_input_handling_mouse.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_letter_operations.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_letter_operations.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_other.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_other.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_rendering.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_highlighting.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_rendering_highlighting.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_rendering_syntax_coloring.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_rendering_syntax_coloring.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_scrollbar_vertical.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_scrollbar_vertical.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/_usage.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/_usage.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/ColorFormatter.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/ColorFormatter.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/elements/fonts/Courier.ttf` & `pygame_texteditor-0.7.3/src/pygame_texteditor/elements/fonts/Courier.ttf`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/src/pygame_texteditor/TextEditor.py` & `pygame_texteditor-0.7.3/src/pygame_texteditor/TextEditor.py`

 * *Files identical despite different names*

### Comparing `pygame_texteditor-0.7.2/PKG-INFO` & `pygame_texteditor-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-texteditor
-Version: 0.7.2
+Version: 0.7.3
 Summary: A WYSIWYG-texteditor based on pygame.
 License: MIT
 Keywords: pygame,texteditor,text,editor
 Author: Victor Seifert
 Author-email: seifert.victor@web.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -198,16 +198,17 @@
 **Editor colors** (source: bright.yml)
 
 - `codingBackgroundColor: (255, 255, 255)`
 - `codingScrollBarBackgroundColor: (49, 50, 50)`
 - `lineNumberColor: (255, 255, 255)`
 - `lineNumberBackgroundColor: (60, 61, 61)`
 - `textColor: (255, 255, 255)`
+- `caretColor: (255, 255, 255)`
 
-** Syntax colors** (source: bright.yml)
+**Syntax colors** (source: bright.yml)
 
 - `textColor_normal: (0, 255, 255)`
 - `textColor_comments: (119, 115, 115)`
 - `textColor_quotes: (227, 215, 115)`
 - `textColor_operators: (237, 36, 36)`
 - `textColor_keywords: (237, 36, 36)`
 - `textColor_function: (50, 150, 36)`
```

