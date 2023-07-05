# Comparing `tmp/almoststatic-1.0.2.tar.gz` & `tmp/almoststatic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almoststatic-1.0.2.tar", last modified: Sat May  6 15:48:53 2023, max compression
+gzip compressed data, was "almoststatic-1.0.3.tar", last modified: Wed Jul  5 11:54:05 2023, max compression
```

## Comparing `almoststatic-1.0.2.tar` & `almoststatic-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-05-06 15:48:53.446243 almoststatic-1.0.2/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-07-11 08:32:04.000000 almoststatic-1.0.2/LICENSE
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6227 2023-05-06 15:48:53.446243 almoststatic-1.0.2/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5299 2023-05-06 13:04:22.000000 almoststatic-1.0.2/README.md
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-05-06 15:48:53.446243 almoststatic-1.0.2/almoststatic/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    29838 2023-05-06 13:05:10.000000 almoststatic-1.0.2/almoststatic/__init__.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-05-06 15:48:53.446243 almoststatic-1.0.2/almoststatic.egg-info/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6227 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      246 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/SOURCES.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/dependency_links.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       22 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/requires.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       13 2023-05-06 15:48:53.000000 almoststatic-1.0.2/almoststatic.egg-info/top_level.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       90 2021-07-11 07:09:18.000000 almoststatic-1.0.2/pyproject.toml
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      972 2023-05-06 15:48:53.446243 almoststatic-1.0.2/setup.cfg
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-05 11:54:05.106436 almoststatic-1.0.3/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-07-11 08:32:04.000000 almoststatic-1.0.3/LICENSE
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6227 2023-07-05 11:54:05.106436 almoststatic-1.0.3/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5299 2023-05-06 13:04:22.000000 almoststatic-1.0.3/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-05 11:54:05.106436 almoststatic-1.0.3/almoststatic/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    29625 2023-07-05 10:52:53.000000 almoststatic-1.0.3/almoststatic/__init__.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-05 11:54:05.106436 almoststatic-1.0.3/almoststatic.egg-info/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6227 2023-07-05 11:54:05.000000 almoststatic-1.0.3/almoststatic.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      246 2023-07-05 11:54:05.000000 almoststatic-1.0.3/almoststatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-07-05 11:54:05.000000 almoststatic-1.0.3/almoststatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       22 2023-07-05 11:54:05.000000 almoststatic-1.0.3/almoststatic.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       13 2023-07-05 11:54:05.000000 almoststatic-1.0.3/almoststatic.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       90 2021-07-11 07:09:18.000000 almoststatic-1.0.3/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      972 2023-07-05 11:54:05.106436 almoststatic-1.0.3/setup.cfg
```

### Comparing `almoststatic-1.0.2/LICENSE` & `almoststatic-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `almoststatic-1.0.2/PKG-INFO` & `almoststatic-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almoststatic
-Version: 1.0.2
+Version: 1.0.3
 Summary: Use Jinja2 template system to build static pages with Flask integration
 Home-page: https://gitlab.com/claudio.driussi/almoststatic
 Author: Claudio driussi
 Author-email: claudio.driussi@gmail.com
 License: LGPL
 Keywords: Flask,static,web,"static pages","static sites",html
 Platform: any
```

### Comparing `almoststatic-1.0.2/README.md` & `almoststatic-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `almoststatic-1.0.2/almoststatic/__init__.py` & `almoststatic-1.0.3/almoststatic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,19 +211,17 @@
             content = self.render_content(
                 page['content'], page.get('widgets_envelope'))
             content = self.render_template(
                 templ_name=templ_name, content=content)
             # substitute macros keys with values, first are evaluated page
             # macros and the the global macros declared in config file.
             for k, v in self.page.get('macros', {}).items():
-                content = content.replace(k,
-                                          self.get_markdown(v, strip_p=True))
+                content = content.replace(k, self.get_markdown(v))
             for k, v in self.macros.items():
-                content = content.replace(k,
-                                          self.get_markdown(v, strip_p=True))
+                content = content.replace(k, self.get_markdown(v))
             # template commands can be embedded within html and md and this is
             # the last rendering which evaluate them
             template = self.env.from_string(content)
             content = template.render(page=page, **kwargs)
             if self.cache and page.get('cacheable', True):
                 self.cached[pagename] = (time.time(), content)
         return content
@@ -353,46 +351,43 @@
             anchor = page[i:]
             page = page[:i]
         except ValueError:
             anchor = ''
         suffix = self.vars['url_suffix']
         return f"{self._relative_url()}{page}{suffix}{anchor}"
 
-    def get_markdown(self, text, strip_p=False):
+    def get_markdown(self, text):
         """convert markdown to html with tables extension.
 
         Double quote and single quotes by default can be escaped with "^^"
         sequence, this let to insert Jinja2 commands within links.
         In markdown `[My Page]({{get_url("mylink")}})` produce an error because
         markdown uses quotes to identify title attribute. So it can be
         substituted with `[My Page]({{get_url(^^mylink^^)}})`. This mean that
         you can use the sequence "^^" only for links.
 
-        Usually markdown surround text within a paragraph tag <p></p> this is
-        not desired in macros because usually they are inline, so we have a
-        parameter to strip them out.
-
         Args:
             text (str): the text in markdown format
             strip_p (bool): strip paragraph tag from evaluated markdown
 
         Returns:
             str: the converted text
         """
         quote_marker = '\\:'
         text = text.replace(self.quote_escape, quote_marker)
         text = markdown.markdown(text, extensions=self.md_extensions)
 
-        if strip_p:
-            try:
-                if text.index('<p>') == 0:
-                    end = text.rindex('</p>')
-                    text = text[3:end]
-            except Exception:
-                pass
+        # Usually markdown surround text within a paragraph tag <p></p> this is
+        # not desired because we like to have control of on our text.
+        try:
+            if text.index('<p>') == 0:
+                end = text.rindex('</p>')
+                text = text[3:end]
+        except Exception:
+            pass
 
         return text.replace(quote_marker, "'")
 
     def _relative_url(self):
         """"""
         if self.vars['url_prefix']:
             return self.vars['url_prefix']
```

### Comparing `almoststatic-1.0.2/almoststatic.egg-info/PKG-INFO` & `almoststatic-1.0.3/almoststatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almoststatic
-Version: 1.0.2
+Version: 1.0.3
 Summary: Use Jinja2 template system to build static pages with Flask integration
 Home-page: https://gitlab.com/claudio.driussi/almoststatic
 Author: Claudio driussi
 Author-email: claudio.driussi@gmail.com
 License: LGPL
 Keywords: Flask,static,web,"static pages","static sites",html
 Platform: any
```

### Comparing `almoststatic-1.0.2/setup.cfg` & `almoststatic-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = almoststatic
-version = 1.0.2
+version = 1.0.3
 author = Claudio driussi
 author_email = claudio.driussi@gmail.com
 description = Use Jinja2 template system to build static pages with Flask integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/claudio.driussi/almoststatic
 license = LGPL
```

