# Comparing `tmp/marquedown-0.8.0.tar.gz` & `tmp/marquedown-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marquedown-0.8.0.tar", max compression
+gzip compressed data, was "marquedown-0.9.0.tar", max compression
```

## Comparing `marquedown-0.8.0.tar` & `marquedown-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35088 2022-03-11 23:25:27.035634 marquedown-0.8.0/LICENSE
--rw-r--r--   0        0        0     2998 2022-04-18 23:47:46.352613 marquedown-0.8.0/README.md
--rw-r--r--   0        0        0      640 2022-08-05 21:55:39.172325 marquedown-0.8.0/marquedown/__init__.py
--rw-r--r--   0        0        0     1067 2022-04-01 19:57:07.097960 marquedown-0.8.0/marquedown/__main__.py
--rw-r--r--   0        0        0     2165 2022-04-18 16:48:40.774410 marquedown-0.8.0/marquedown/bblike.py
--rw-r--r--   0        0        0     1553 2022-04-18 20:53:47.387267 marquedown-0.8.0/marquedown/citation.py
--rw-r--r--   0        0        0        0 2022-04-01 17:48:36.114371 marquedown-0.8.0/marquedown/commands/__init__.py
--rw-r--r--   0        0        0     3351 2022-04-03 14:36:09.005532 marquedown-0.8.0/marquedown/commands/render.py
--rw-r--r--   0        0        0     2208 2022-08-05 21:55:06.592878 marquedown-0.8.0/marquedown/labellist.py
--rw-r--r--   0        0        0      597 2022-04-18 20:39:35.305684 marquedown-0.8.0/marquedown/tagtools.py
--rw-r--r--   0        0        0     1346 2022-04-03 18:02:28.590892 marquedown-0.8.0/marquedown/video.py
--rw-r--r--   0        0        0      529 2022-08-05 21:55:31.285792 marquedown-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3935 2022-08-05 21:56:04.120822 marquedown-0.8.0/setup.py
--rw-r--r--   0        0        0     3677 2022-08-05 21:56:04.121389 marquedown-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35088 2022-03-11 23:25:27.035634 marquedown-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3967 2022-08-07 18:14:24.039167 marquedown-0.9.0/README.md
+-rw-r--r--   0        0        0      985 2022-08-07 17:39:40.034453 marquedown-0.9.0/marquedown/__init__.py
+-rw-r--r--   0        0        0     1114 2022-08-07 16:23:42.343900 marquedown-0.9.0/marquedown/__main__.py
+-rw-r--r--   0        0        0     2165 2022-04-18 16:48:40.774410 marquedown-0.9.0/marquedown/bblike.py
+-rw-r--r--   0        0        0     1553 2022-04-18 20:53:47.387267 marquedown-0.9.0/marquedown/citation.py
+-rw-r--r--   0        0        0        0 2022-04-01 17:48:36.114371 marquedown-0.9.0/marquedown/commands/__init__.py
+-rw-r--r--   0        0        0     3750 2022-08-07 17:44:20.076597 marquedown-0.9.0/marquedown/commands/render.py
+-rw-r--r--   0        0        0     2208 2022-08-05 21:55:06.592878 marquedown-0.9.0/marquedown/labellist.py
+-rw-r--r--   0        0        0     1987 2022-08-07 18:04:26.279640 marquedown-0.9.0/marquedown/qr.py
+-rw-r--r--   0        0        0      597 2022-04-18 20:39:35.305684 marquedown-0.9.0/marquedown/tagtools.py
+-rw-r--r--   0        0        0     1346 2022-04-03 18:02:28.590892 marquedown-0.9.0/marquedown/video.py
+-rw-r--r--   0        0        0      529 2022-08-07 14:49:57.053305 marquedown-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4972 2022-08-07 18:15:13.367354 marquedown-0.9.0/setup.py
+-rw-r--r--   0        0        0     4646 2022-08-07 18:15:13.367680 marquedown-0.9.0/PKG-INFO
```

### Comparing `marquedown-0.8.0/LICENSE` & `marquedown-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marquedown-0.8.0/README.md` & `marquedown-0.9.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,40 +6,50 @@
 ## Examples
 
 ### Blockquote with citation
 
 This is currently limited to the top scope with no indentation.
 Surrounding dotted lines are optional.
 
+#### Example
+
+##### Marquedown
+
 ```md
 ......................................................
 > You have enemies? Good. That means you've stood up
 > for something, sometime in your life.
 -- Winston Churchill
 ''''''''''''''''''''''''''''''''''''''''''''''''''''''
 ```
 
+##### HTML
+
 ```html
 <blockquote>
     <p>
         You have enemies? Good. That means you've stood up
         for something, sometime in your life.
     </p>
     <cite>Winston Churchill</cite>
 </blockquote>
 ```
 
 ### Embed video
 
 #### YouTube
 
+##### Marquedown
+
 ```md
 ![dimweb](https://youtu.be/VmAEkV5AYSQ "An embedded YouTube video")
 ```
 
+##### HTML
+
 ```html
 <iframe
     src="https://www.youtube.com/embed/VmAEkV5AYSQ"
     title="An embedded YouTube video" frameborder="0"
     allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
     allowfullscreen>
 </iframe>
@@ -54,42 +64,54 @@
 The naming scheme is the same as in CSS, e.g. `tag.class1.class2`
 If `tag` is omitted, it is treated to be `div`
 
 #### ID:s
 
 ID:s are supported using `#beans` at the end of the tag, ex. `[p#beans]`
 
+#### Example
+
+##### Marquedown
+
 ```md
 [section]
 [.bingo]
 A regular **paragraph** written in Marquedown, but *within* other HTML tags.
 [//]
 
 [tag.class1.class2] [/tag]
 ```
 
+##### HTML
+
 ```html
 <section>
 <div class="bingo">
     <p>
         A regular <strong>paragraph</strong> written in Marquedown, but <em>within</em> other HTML tags.
     </p>
 </div></section>
 
 <tag class="class1 class2"> </tag>
 ```
 
 ### Label list
 
+#### Example
+
+##### Marquedown
+
 ```md
 (| email: [jon@webby.net](mailto:jon@webby.net)
 (| matrix: [@jon:webby.net](https://matrix.to/#/@jon:webby.net)
 (| runescape: jonathan_superstar1777
 ```
 
+##### HTML
+
 ```html
 <ul class="labels">
     <li class="label label-email">
         <a href="mailto:jon@webby.net">
             jon@webby.net
         </a>
     </li>
@@ -100,28 +122,64 @@
     </li>
     <li class="label label-runescape">
         jonathan_superstar1777
     </li>
 </ul>
 ```
 
+### QR codes
+
+QR codes can be generated and referenced automatically via the `render` command. If you want to generate QR codes with `marquedown.marquedown`, you can follow the example below.
+
+#### Example
+
+##### Marquedown
+
+```md
+![qr:monero-wallet](monero:abcdefghijklmnopqrstuvwxyz)
+```
+
+##### Python
+
+```py
+from marquedown import marquedown
+
+with open('document.mqd', 'r') as f:
+    document = f.read()
+
+with open('public/document.html', 'w') as f:
+    rendered = marquedown(document, qrgen='public/qr:qr')
+    f.write(rendered)
+```
+
+The string provided to `qrgen` is two paths separated by a colon.
+
+1. Where to save the generated images
+2. What directory to reference in the HTML `src` parameter
+
+##### The generated HTML
+
+```html
+<img src="qr/qr-0-monero-wallet.png" alt="monero-wallet">
+```
+
 ## Commands
 
 ### `render`: Render documents
 
 You can render an entire directory and its subdirectories of Markdown or Marquedown documents. This can be used to automate rendering pages for your website.
 
 Do `python -m marquedown render --help` for list of options.
 
 #### Example
 
 For a few of my websites hosted on GitLab, I have it set up to run *this* on push:
 
 ```sh
 # Render document
-python -m marquedown render -i ./md -o ./public -t ./templates/page.html
+python -m marquedown render -i "./mqd" -o "./public" -t "./templates/page.html"
 
 # This is for the GitLab Pages publication
 mkdir .public
 cp -r public .public
 mv .public public  
 ```
```

#### html2text {}

```diff
@@ -1,35 +1,46 @@
 # Marquedown Extending Markdown further by adding a few more useful notations.
 It can be used in place of `markdown` as it also uses and applies it. ##
 Examples ### Blockquote with citation This is currently limited to the top
-scope with no indentation. Surrounding dotted lines are optional. ```md
-...................................................... > You have enemies?
-Good. That means you've stood up > for something, sometime in your life. -
-- Winston Churchill '''''''''''''''''''''''''''''''''''''''''''''''''''''' ```
-```html
+scope with no indentation. Surrounding dotted lines are optional. #### Example
+##### Marquedown ```md ...................................................... >
+You have enemies? Good. That means you've stood up > for something, sometime in
+your life. -- Winston Churchill
+'''''''''''''''''''''''''''''''''''''''''''''''''''''' ``` ##### HTML ```html
      You have enemies? Good. That means you've stood up for something,
      sometime in your life.
      Winston Churchill
-``` ### Embed video #### YouTube ```md ![dimweb](https://youtu.be/VmAEkV5AYSQ
-"An embedded YouTube video") ``` ```html   ``` ### BBCode HTML tags These tags
-allow you to put Marquedown inside HTML tags. This is done by finding and
-replacing them with their represented HTML after all other Marquedown has been
-rendered. #### Tags and classes The naming scheme is the same as in CSS, e.g.
-`tag.class1.class2` If `tag` is omitted, it is treated to be `div` #### ID:
-s ID:s are supported using `#beans` at the end of the tag, ex. `[p#beans]`
-```md [section] [.bingo] A regular **paragraph** written in Marquedown, but
-*within* other HTML tags. [//] [tag.class1.class2] [/tag] ``` ```html
+``` ### Embed video #### YouTube ##### Marquedown ```md ![dimweb](https://
+youtu.be/VmAEkV5AYSQ "An embedded YouTube video") ``` ##### HTML ```html   ```
+### BBCode HTML tags These tags allow you to put Marquedown inside HTML tags.
+This is done by finding and replacing them with their represented HTML after
+all other Marquedown has been rendered. #### Tags and classes The naming scheme
+is the same as in CSS, e.g. `tag.class1.class2` If `tag` is omitted, it is
+treated to be `div` #### ID:s ID:s are supported using `#beans` at the end of
+the tag, ex. `[p#beans]` #### Example ##### Marquedown ```md [section] [.bingo]
+A regular **paragraph** written in Marquedown, but *within* other HTML tags. [/
+/] [tag.class1.class2] [/tag] ``` ##### HTML ```html
 A regular paragraph written in Marquedown, but within other HTML tags.
-  ``` ### Label list ```md (| email: [jon@webby.net](mailto:jon@webby.net) (|
-matrix: [@jon:webby.net](https://matrix.to/#/@jon:webby.net) (| runescape:
-jonathan_superstar1777 ``` ```html
+  ``` ### Label list #### Example ##### Marquedown ```md (| email:
+[jon@webby.net](mailto:jon@webby.net) (| matrix: [@jon:webby.net](https://
+matrix.to/#/@jon:webby.net) (| runescape: jonathan_superstar1777 ``` ##### HTML
+```html
     * jon@webby.net
     * @jon:webby.net
     * jonathan_superstar1777
-``` ## Commands ### `render`: Render documents You can render an entire
-directory and its subdirectories of Markdown or Marquedown documents. This can
-be used to automate rendering pages for your website. Do `python -m marquedown
-render --help` for list of options. #### Example For a few of my websites
-hosted on GitLab, I have it set up to run *this* on push: ```sh # Render
-document python -m marquedown render -i ./md -o ./public -t ./templates/
-page.html # This is for the GitLab Pages publication mkdir .public cp -r public
-.public mv .public public ```
+``` ### QR codes QR codes can be generated and referenced automatically via the
+`render` command. If you want to generate QR codes with
+`marquedown.marquedown`, you can follow the example below. #### Example #####
+Marquedown ```md ![qr:monero-wallet](monero:abcdefghijklmnopqrstuvwxyz) ```
+##### Python ```py from marquedown import marquedown with open('document.mqd',
+'r') as f: document = f.read() with open('public/document.html', 'w') as f:
+rendered = marquedown(document, qrgen='public/qr:qr') f.write(rendered) ``` The
+string provided to `qrgen` is two paths separated by a colon. 1. Where to save
+the generated images 2. What directory to reference in the HTML `src` parameter
+##### The generated HTML ```html [monero-wallet] ``` ## Commands ### `render`:
+Render documents You can render an entire directory and its subdirectories of
+Markdown or Marquedown documents. This can be used to automate rendering pages
+for your website. Do `python -m marquedown render --help` for list of options.
+#### Example For a few of my websites hosted on GitLab, I have it set up to run
+*this* on push: ```sh # Render document python -m marquedown render -i "./mqd"
+-o "./public" -t "./templates/page.html" # This is for the GitLab Pages
+publication mkdir .public cp -r public .public mv .public public ```
```

### Comparing `marquedown-0.8.0/marquedown/__main__.py` & `marquedown-0.9.0/marquedown/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,12 @@
 
 if __name__ == '__main__':
     args = parser.parse_args()
     
     # `render`: Render Marquedown documents
     if args.command == 'render':
         from .commands.render import render_documents
-        render_documents(args.source, args.destination, args.template)
+        render_documents(
+            args.source,
+            args.destination,
+            args.template,
+        )
```

### Comparing `marquedown-0.8.0/marquedown/bblike.py` & `marquedown-0.9.0/marquedown/bblike.py`

 * *Files identical despite different names*

### Comparing `marquedown-0.8.0/marquedown/citation.py` & `marquedown-0.9.0/marquedown/citation.py`

 * *Files identical despite different names*

### Comparing `marquedown-0.8.0/marquedown/commands/render.py` & `marquedown-0.9.0/marquedown/commands/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # 
 # Provide a template for embedding the rendered content.
 
 import re
 import os
 import yaml
 
-from typing import Any
 from pathlib import Path
 from collections import defaultdict
 
 from .. import marquedown
+from ..qr import QRGenerator
 
 
 def extract_metadata(document: str):
     """Extract metadata from a YAML code block at the top of the document.
     
     Example:
         ```yml
@@ -66,15 +66,16 @@
             if file_source.name in ('index.md', 'index.mqd'):
                 yield file_source, file_destination.parent / 'index.html'
             else:
                 yield file_source, file_destination / 'index.html'
 
 
 def render_documents(source: Path, destination: Path, template: Path = None):
-    """Load all documents from within the source directory
+    """
+    Load all documents from within the source directory
     and its subdirectories and render them onto a template file.
     Save all renders in the destination directory.
     """
 
     # Load template
     if template is not None:
         with open(template, 'r') as f:
@@ -84,19 +85,28 @@
     for fsource, fdestination in find_documents(source, destination):
         # Load document
         with open(fsource, 'r') as f:
             document = f.read()
 
         # Prepare document and render it
         metadata, document = extract_metadata(document)
-        rendered = marquedown(document)
 
         # Ensure destination directory
         os.makedirs(fdestination.parent, exist_ok=True)
 
+        # Save QR codes differently depending on whether source file is index
+        if fsource.name in ('index.md', 'index.mqd'):
+            qrgen = QRGenerator(fdestination.parent / 'qr', Path('qr'))
+        else:
+            qrgen = QRGenerator(fdestination.parent / 'qr', Path(fsource.stem, 'qr'))
+
+
+        # Render Marquedown, optionally template, and write to file
+        rendered = marquedown(document, qrgen=qrgen)
+
         with open(fdestination, 'w') as f:
             # Format to template if provided
             if template is not None:
                 rendered = template.format_map(defaultdict(str, **metadata, document=rendered))
             # Write to destination
             f.write(rendered)
             print(f'Rendered document: {fsource.relative_to(source)}')
```

### Comparing `marquedown-0.8.0/marquedown/labellist.py` & `marquedown-0.9.0/marquedown/labellist.py`

 * *Files identical despite different names*

### Comparing `marquedown-0.8.0/marquedown/tagtools.py` & `marquedown-0.9.0/marquedown/tagtools.py`

 * *Files identical despite different names*

### Comparing `marquedown-0.8.0/marquedown/video.py` & `marquedown-0.9.0/marquedown/video.py`

 * *Files identical despite different names*

### Comparing `marquedown-0.8.0/pyproject.toml` & `marquedown-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marquedown"
-version = "0.8.0"
+version = "0.9.0"
 description = "Extending Markdown further by adding a few more useful notations."
 readme = "README.md"
 authors = ["Maximillian Strand <maximillian.strand@protonmail.com>"]
 repository = "https://gitlab.com/deepadmax/marquedown"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
```

### Comparing `marquedown-0.8.0/setup.py` & `marquedown-0.9.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['Markdown>=3.3.6,<4.0.0', 'PyYAML>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'marquedown',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Extending Markdown further by adding a few more useful notations.',
-    'long_description': '# Marquedown\n\nExtending Markdown further by adding a few more useful notations.\nIt can be used in place of `markdown` as it also uses and applies it.\n\n## Examples\n\n### Blockquote with citation\n\nThis is currently limited to the top scope with no indentation.\nSurrounding dotted lines are optional.\n\n```md\n......................................................\n> You have enemies? Good. That means you\'ve stood up\n> for something, sometime in your life.\n-- Winston Churchill\n\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\n```\n\n```html\n<blockquote>\n    <p>\n        You have enemies? Good. That means you\'ve stood up\n        for something, sometime in your life.\n    </p>\n    <cite>Winston Churchill</cite>\n</blockquote>\n```\n\n### Embed video\n\n#### YouTube\n\n```md\n![dimweb](https://youtu.be/VmAEkV5AYSQ "An embedded YouTube video")\n```\n\n```html\n<iframe\n    src="https://www.youtube.com/embed/VmAEkV5AYSQ"\n    title="An embedded YouTube video" frameborder="0"\n    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"\n    allowfullscreen>\n</iframe>\n```\n\n### BBCode HTML tags\n\nThese tags allow you to put Marquedown inside HTML tags. This is done by finding and replacing them with their represented HTML after all other Marquedown has been rendered.\n\n#### Tags and classes\n\nThe naming scheme is the same as in CSS, e.g. `tag.class1.class2`\nIf `tag` is omitted, it is treated to be `div`\n\n#### ID:s\n\nID:s are supported using `#beans` at the end of the tag, ex. `[p#beans]`\n\n```md\n[section]\n[.bingo]\nA regular **paragraph** written in Marquedown, but *within* other HTML tags.\n[//]\n\n[tag.class1.class2] [/tag]\n```\n\n```html\n<section>\n<div class="bingo">\n    <p>\n        A regular <strong>paragraph</strong> written in Marquedown, but <em>within</em> other HTML tags.\n    </p>\n</div></section>\n\n<tag class="class1 class2"> </tag>\n```\n\n### Label list\n\n```md\n(| email: [jon@webby.net](mailto:jon@webby.net)\n(| matrix: [@jon:webby.net](https://matrix.to/#/@jon:webby.net)\n(| runescape: jonathan_superstar1777\n```\n\n```html\n<ul class="labels">\n    <li class="label label-email">\n        <a href="mailto:jon@webby.net">\n            jon@webby.net\n        </a>\n    </li>\n    <li class="label label-matrix">\n        <a href="https://matrix.to/#/@jon:webby.net">\n            @jon:webby.net\n        </a>\n    </li>\n    <li class="label label-runescape">\n        jonathan_superstar1777\n    </li>\n</ul>\n```\n\n## Commands\n\n### `render`: Render documents\n\nYou can render an entire directory and its subdirectories of Markdown or Marquedown documents. This can be used to automate rendering pages for your website.\n\nDo `python -m marquedown render --help` for list of options.\n\n#### Example\n\nFor a few of my websites hosted on GitLab, I have it set up to run *this* on push:\n\n```sh\n# Render document\npython -m marquedown render -i ./md -o ./public -t ./templates/page.html\n\n# This is for the GitLab Pages publication\nmkdir .public\ncp -r public .public\nmv .public public  \n```',
+    'long_description': '# Marquedown\n\nExtending Markdown further by adding a few more useful notations.\nIt can be used in place of `markdown` as it also uses and applies it.\n\n## Examples\n\n### Blockquote with citation\n\nThis is currently limited to the top scope with no indentation.\nSurrounding dotted lines are optional.\n\n#### Example\n\n##### Marquedown\n\n```md\n......................................................\n> You have enemies? Good. That means you\'ve stood up\n> for something, sometime in your life.\n-- Winston Churchill\n\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\n```\n\n##### HTML\n\n```html\n<blockquote>\n    <p>\n        You have enemies? Good. That means you\'ve stood up\n        for something, sometime in your life.\n    </p>\n    <cite>Winston Churchill</cite>\n</blockquote>\n```\n\n### Embed video\n\n#### YouTube\n\n##### Marquedown\n\n```md\n![dimweb](https://youtu.be/VmAEkV5AYSQ "An embedded YouTube video")\n```\n\n##### HTML\n\n```html\n<iframe\n    src="https://www.youtube.com/embed/VmAEkV5AYSQ"\n    title="An embedded YouTube video" frameborder="0"\n    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"\n    allowfullscreen>\n</iframe>\n```\n\n### BBCode HTML tags\n\nThese tags allow you to put Marquedown inside HTML tags. This is done by finding and replacing them with their represented HTML after all other Marquedown has been rendered.\n\n#### Tags and classes\n\nThe naming scheme is the same as in CSS, e.g. `tag.class1.class2`\nIf `tag` is omitted, it is treated to be `div`\n\n#### ID:s\n\nID:s are supported using `#beans` at the end of the tag, ex. `[p#beans]`\n\n#### Example\n\n##### Marquedown\n\n```md\n[section]\n[.bingo]\nA regular **paragraph** written in Marquedown, but *within* other HTML tags.\n[//]\n\n[tag.class1.class2] [/tag]\n```\n\n##### HTML\n\n```html\n<section>\n<div class="bingo">\n    <p>\n        A regular <strong>paragraph</strong> written in Marquedown, but <em>within</em> other HTML tags.\n    </p>\n</div></section>\n\n<tag class="class1 class2"> </tag>\n```\n\n### Label list\n\n#### Example\n\n##### Marquedown\n\n```md\n(| email: [jon@webby.net](mailto:jon@webby.net)\n(| matrix: [@jon:webby.net](https://matrix.to/#/@jon:webby.net)\n(| runescape: jonathan_superstar1777\n```\n\n##### HTML\n\n```html\n<ul class="labels">\n    <li class="label label-email">\n        <a href="mailto:jon@webby.net">\n            jon@webby.net\n        </a>\n    </li>\n    <li class="label label-matrix">\n        <a href="https://matrix.to/#/@jon:webby.net">\n            @jon:webby.net\n        </a>\n    </li>\n    <li class="label label-runescape">\n        jonathan_superstar1777\n    </li>\n</ul>\n```\n\n### QR codes\n\nQR codes can be generated and referenced automatically via the `render` command. If you want to generate QR codes with `marquedown.marquedown`, you can follow the example below.\n\n#### Example\n\n##### Marquedown\n\n```md\n![qr:monero-wallet](monero:abcdefghijklmnopqrstuvwxyz)\n```\n\n##### Python\n\n```py\nfrom marquedown import marquedown\n\nwith open(\'document.mqd\', \'r\') as f:\n    document = f.read()\n\nwith open(\'public/document.html\', \'w\') as f:\n    rendered = marquedown(document, qrgen=\'public/qr:qr\')\n    f.write(rendered)\n```\n\nThe string provided to `qrgen` is two paths separated by a colon.\n\n1. Where to save the generated images\n2. What directory to reference in the HTML `src` parameter\n\n##### The generated HTML\n\n```html\n<img src="qr/qr-0-monero-wallet.png" alt="monero-wallet">\n```\n\n## Commands\n\n### `render`: Render documents\n\nYou can render an entire directory and its subdirectories of Markdown or Marquedown documents. This can be used to automate rendering pages for your website.\n\nDo `python -m marquedown render --help` for list of options.\n\n#### Example\n\nFor a few of my websites hosted on GitLab, I have it set up to run *this* on push:\n\n```sh\n# Render document\npython -m marquedown render -i "./mqd" -o "./public" -t "./templates/page.html"\n\n# This is for the GitLab Pages publication\nmkdir .public\ncp -r public .public\nmv .public public  \n```',
     'author': 'Maximillian Strand',
     'author_email': 'maximillian.strand@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/deepadmax/marquedown',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,58 +1,72 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['marquedown', 'marquedown.commands'] package_data = \ {'': ['*']}
 install_requires = \ ['Markdown>=3.3.6,<4.0.0', 'PyYAML>=6.0,<7.0']
-setup_kwargs = { 'name': 'marquedown', 'version': '0.8.0', 'description':
+setup_kwargs = { 'name': 'marquedown', 'version': '0.9.0', 'description':
 'Extending Markdown further by adding a few more useful notations.',
 'long_description': '# Marquedown\n\nExtending Markdown further by adding a few
 more useful notations.\nIt can be used in place of `markdown` as it also uses
 and applies it.\n\n## Examples\n\n### Blockquote with citation\n\nThis is
 currently limited to the top scope with no indentation.\nSurrounding dotted
-lines are
-optional.\n\n```md\n......................................................\n>
+lines are optional.\n\n#### Example\n\n#####
+Marquedown\n\n```md\n......................................................\n>
 You have enemies? Good. That means you\'ve stood up\n> for something, sometime
 in your life.\n-- Winston
-Churchill\n\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\n```\n\n```html\n
+Churchill\n\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\'\n```\n\n#####
+HTML\n\n```html\n
      \n
      \n You have enemies? Good. That means you\'ve stood up\n for
      something, sometime in your life.\n
      \nWinston Churchill\n
-\n```\n\n### Embed video\n\n#### YouTube\n\n```md\n![dimweb](https://youtu.be/
-VmAEkV5AYSQ "An embedded YouTube video")\n```\n\n```html\n
+\n```\n\n### Embed video\n\n#### YouTube\n\n##### Marquedown\n\n```md\n!
+[dimweb](https://youtu.be/VmAEkV5AYSQ "An embedded YouTube
+video")\n```\n\n##### HTML\n\n```html\n
 n src="https://www.youtube.com/embed/VmAEkV5AYSQ"\n title="An embedded YouTube
 video" frameborder="0"\n allow="accelerometer; autoplay; clipboard-write;
 encrypted-media; gyroscope; picture-in-picture"\n
 allowfullscreen>\n\n```\n\n### BBCode HTML tags\n\nThese tags allow you to put
 Marquedown inside HTML tags. This is done by finding and replacing them with
 their represented HTML after all other Marquedown has been rendered.\n\n####
 Tags and classes\n\nThe naming scheme is the same as in CSS, e.g.
 `tag.class1.class2`\nIf `tag` is omitted, it is treated to be `div`\n\n#### ID:
 s\n\nID:s are supported using `#beans` at the end of the tag, ex. `
-[p#beans]`\n\n```md\n[section]\n[.bingo]\nA regular **paragraph** written in
-Marquedown, but *within* other HTML tags.\n[//]\n\n[tag.class1.class2] [/
-tag]\n```\n\n```html\n\n
+[p#beans]`\n\n#### Example\n\n##### Marquedown\n\n```md\n[section]\n[.bingo]\nA
+regular **paragraph** written in Marquedown, but *within* other HTML tags.\n[//
+]\n\n[tag.class1.class2] [/tag]\n```\n\n##### HTML\n\n```html\n\n
 \n
 \n A regular paragraph written in Marquedown, but within other HTML tags.\n
 \n
-\n\n \n```\n\n### Label list\n\n```md\n(| email: [jon@webby.net](mailto:
-jon@webby.net)\n(| matrix: [@jon:webby.net](https://matrix.to/#/@jon:
-webby.net)\n(| runescape: jonathan_superstar1777\n```\n\n```html\n
+\n\n \n```\n\n### Label list\n\n#### Example\n\n##### Marquedown\n\n```md\n(|
+email: [jon@webby.net](mailto:jon@webby.net)\n(| matrix: [@jon:webby.net]
+(https://matrix.to/#/@jon:webby.net)\n(| runescape:
+jonathan_superstar1777\n```\n\n##### HTML\n\n```html\n
     * \n
     * \n \n_jon@webby.net\n\n
     * \n
     * \n \n_@jon:webby.net\n\n
     * \n
     * \n jonathan_superstar1777\n
     * \n
-\n```\n\n## Commands\n\n### `render`: Render documents\n\nYou can render an
-entire directory and its subdirectories of Markdown or Marquedown documents.
-This can be used to automate rendering pages for your website.\n\nDo `python -
+\n```\n\n### QR codes\n\nQR codes can be generated and referenced automatically
+via the `render` command. If you want to generate QR codes with
+`marquedown.marquedown`, you can follow the example below.\n\n####
+Example\n\n##### Marquedown\n\n```md\n![qr:monero-wallet](monero:
+abcdefghijklmnopqrstuvwxyz)\n```\n\n##### Python\n\n```py\nfrom marquedown
+import marquedown\n\nwith open(\'document.mqd\', \'r\') as f:\n document =
+f.read()\n\nwith open(\'public/document.html\', \'w\') as f:\n rendered =
+marquedown(document, qrgen=\'public/qr:qr\')\n f.write(rendered)\n```\n\nThe
+string provided to `qrgen` is two paths separated by a colon.\n\n1. Where to
+save the generated images\n2. What directory to reference in the HTML `src`
+parameter\n\n##### The generated HTML\n\n```html\n[monero-wallet]\n```\n\n##
+Commands\n\n### `render`: Render documents\n\nYou can render an entire
+directory and its subdirectories of Markdown or Marquedown documents. This can
+be used to automate rendering pages for your website.\n\nDo `python -
 m marquedown render --help` for list of options.\n\n#### Example\n\nFor a few
 of my websites hosted on GitLab, I have it set up to run *this* on push:
-\n\n```sh\n# Render document\npython -m marquedown render -i ./md -o ./public -
-t ./templates/page.html\n\n# This is for the GitLab Pages publication\nmkdir
-.public\ncp -r public .public\nmv .public public \n```', 'author': 'Maximillian
-Strand', 'author_email': 'maximillian.strand@protonmail.com', 'maintainer':
-None, 'maintainer_email': None, 'url': 'https://gitlab.com/deepadmax/
-marquedown', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.10,<4.0', } setup
-(**setup_kwargs)
+\n\n```sh\n# Render document\npython -m marquedown render -i "./mqd" -o "./
+public" -t "./templates/page.html"\n\n# This is for the GitLab Pages
+publication\nmkdir .public\ncp -r public .public\nmv .public public \n```',
+'author': 'Maximillian Strand', 'author_email':
+'maximillian.strand@protonmail.com', 'maintainer': None, 'maintainer_email':
+None, 'url': 'https://gitlab.com/deepadmax/marquedown', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `marquedown-0.8.0/PKG-INFO` & `marquedown-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marquedown
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extending Markdown further by adding a few more useful notations.
 Home-page: https://gitlab.com/deepadmax/marquedown
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maximillian.strand@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -23,40 +23,50 @@
 ## Examples
 
 ### Blockquote with citation
 
 This is currently limited to the top scope with no indentation.
 Surrounding dotted lines are optional.
 
+#### Example
+
+##### Marquedown
+
 ```md
 ......................................................
 > You have enemies? Good. That means you've stood up
 > for something, sometime in your life.
 -- Winston Churchill
 ''''''''''''''''''''''''''''''''''''''''''''''''''''''
 ```
 
+##### HTML
+
 ```html
 <blockquote>
     <p>
         You have enemies? Good. That means you've stood up
         for something, sometime in your life.
     </p>
     <cite>Winston Churchill</cite>
 </blockquote>
 ```
 
 ### Embed video
 
 #### YouTube
 
+##### Marquedown
+
 ```md
 ![dimweb](https://youtu.be/VmAEkV5AYSQ "An embedded YouTube video")
 ```
 
+##### HTML
+
 ```html
 <iframe
     src="https://www.youtube.com/embed/VmAEkV5AYSQ"
     title="An embedded YouTube video" frameborder="0"
     allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
     allowfullscreen>
 </iframe>
@@ -71,42 +81,54 @@
 The naming scheme is the same as in CSS, e.g. `tag.class1.class2`
 If `tag` is omitted, it is treated to be `div`
 
 #### ID:s
 
 ID:s are supported using `#beans` at the end of the tag, ex. `[p#beans]`
 
+#### Example
+
+##### Marquedown
+
 ```md
 [section]
 [.bingo]
 A regular **paragraph** written in Marquedown, but *within* other HTML tags.
 [//]
 
 [tag.class1.class2] [/tag]
 ```
 
+##### HTML
+
 ```html
 <section>
 <div class="bingo">
     <p>
         A regular <strong>paragraph</strong> written in Marquedown, but <em>within</em> other HTML tags.
     </p>
 </div></section>
 
 <tag class="class1 class2"> </tag>
 ```
 
 ### Label list
 
+#### Example
+
+##### Marquedown
+
 ```md
 (| email: [jon@webby.net](mailto:jon@webby.net)
 (| matrix: [@jon:webby.net](https://matrix.to/#/@jon:webby.net)
 (| runescape: jonathan_superstar1777
 ```
 
+##### HTML
+
 ```html
 <ul class="labels">
     <li class="label label-email">
         <a href="mailto:jon@webby.net">
             jon@webby.net
         </a>
     </li>
@@ -117,28 +139,64 @@
     </li>
     <li class="label label-runescape">
         jonathan_superstar1777
     </li>
 </ul>
 ```
 
+### QR codes
+
+QR codes can be generated and referenced automatically via the `render` command. If you want to generate QR codes with `marquedown.marquedown`, you can follow the example below.
+
+#### Example
+
+##### Marquedown
+
+```md
+![qr:monero-wallet](monero:abcdefghijklmnopqrstuvwxyz)
+```
+
+##### Python
+
+```py
+from marquedown import marquedown
+
+with open('document.mqd', 'r') as f:
+    document = f.read()
+
+with open('public/document.html', 'w') as f:
+    rendered = marquedown(document, qrgen='public/qr:qr')
+    f.write(rendered)
+```
+
+The string provided to `qrgen` is two paths separated by a colon.
+
+1. Where to save the generated images
+2. What directory to reference in the HTML `src` parameter
+
+##### The generated HTML
+
+```html
+<img src="qr/qr-0-monero-wallet.png" alt="monero-wallet">
+```
+
 ## Commands
 
 ### `render`: Render documents
 
 You can render an entire directory and its subdirectories of Markdown or Marquedown documents. This can be used to automate rendering pages for your website.
 
 Do `python -m marquedown render --help` for list of options.
 
 #### Example
 
 For a few of my websites hosted on GitLab, I have it set up to run *this* on push:
 
 ```sh
 # Render document
-python -m marquedown render -i ./md -o ./public -t ./templates/page.html
+python -m marquedown render -i "./mqd" -o "./public" -t "./templates/page.html"
 
 # This is for the GitLab Pages publication
 mkdir .public
 cp -r public .public
 mv .public public  
 ```
```

#### html2text {}

```diff
@@ -1,44 +1,55 @@
-Metadata-Version: 2.1 Name: marquedown Version: 0.8.0 Summary: Extending
+Metadata-Version: 2.1 Name: marquedown Version: 0.9.0 Summary: Extending
 Markdown further by adding a few more useful notations. Home-page: https://
 gitlab.com/deepadmax/marquedown License: GPL-3.0-or-later Author: Maximillian
 Strand Author-email: maximillian.strand@protonmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU General Public License
 v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Markdown
 (>=3.3.6,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Project-URL: Repository,
 https://gitlab.com/deepadmax/marquedown Description-Content-Type: text/markdown
 # Marquedown Extending Markdown further by adding a few more useful notations.
 It can be used in place of `markdown` as it also uses and applies it. ##
 Examples ### Blockquote with citation This is currently limited to the top
-scope with no indentation. Surrounding dotted lines are optional. ```md
-...................................................... > You have enemies?
-Good. That means you've stood up > for something, sometime in your life. -
-- Winston Churchill '''''''''''''''''''''''''''''''''''''''''''''''''''''' ```
-```html
+scope with no indentation. Surrounding dotted lines are optional. #### Example
+##### Marquedown ```md ...................................................... >
+You have enemies? Good. That means you've stood up > for something, sometime in
+your life. -- Winston Churchill
+'''''''''''''''''''''''''''''''''''''''''''''''''''''' ``` ##### HTML ```html
      You have enemies? Good. That means you've stood up for something,
      sometime in your life.
      Winston Churchill
-``` ### Embed video #### YouTube ```md ![dimweb](https://youtu.be/VmAEkV5AYSQ
-"An embedded YouTube video") ``` ```html   ``` ### BBCode HTML tags These tags
-allow you to put Marquedown inside HTML tags. This is done by finding and
-replacing them with their represented HTML after all other Marquedown has been
-rendered. #### Tags and classes The naming scheme is the same as in CSS, e.g.
-`tag.class1.class2` If `tag` is omitted, it is treated to be `div` #### ID:
-s ID:s are supported using `#beans` at the end of the tag, ex. `[p#beans]`
-```md [section] [.bingo] A regular **paragraph** written in Marquedown, but
-*within* other HTML tags. [//] [tag.class1.class2] [/tag] ``` ```html
+``` ### Embed video #### YouTube ##### Marquedown ```md ![dimweb](https://
+youtu.be/VmAEkV5AYSQ "An embedded YouTube video") ``` ##### HTML ```html   ```
+### BBCode HTML tags These tags allow you to put Marquedown inside HTML tags.
+This is done by finding and replacing them with their represented HTML after
+all other Marquedown has been rendered. #### Tags and classes The naming scheme
+is the same as in CSS, e.g. `tag.class1.class2` If `tag` is omitted, it is
+treated to be `div` #### ID:s ID:s are supported using `#beans` at the end of
+the tag, ex. `[p#beans]` #### Example ##### Marquedown ```md [section] [.bingo]
+A regular **paragraph** written in Marquedown, but *within* other HTML tags. [/
+/] [tag.class1.class2] [/tag] ``` ##### HTML ```html
 A regular paragraph written in Marquedown, but within other HTML tags.
-  ``` ### Label list ```md (| email: [jon@webby.net](mailto:jon@webby.net) (|
-matrix: [@jon:webby.net](https://matrix.to/#/@jon:webby.net) (| runescape:
-jonathan_superstar1777 ``` ```html
+  ``` ### Label list #### Example ##### Marquedown ```md (| email:
+[jon@webby.net](mailto:jon@webby.net) (| matrix: [@jon:webby.net](https://
+matrix.to/#/@jon:webby.net) (| runescape: jonathan_superstar1777 ``` ##### HTML
+```html
     * jon@webby.net
     * @jon:webby.net
     * jonathan_superstar1777
-``` ## Commands ### `render`: Render documents You can render an entire
-directory and its subdirectories of Markdown or Marquedown documents. This can
-be used to automate rendering pages for your website. Do `python -m marquedown
-render --help` for list of options. #### Example For a few of my websites
-hosted on GitLab, I have it set up to run *this* on push: ```sh # Render
-document python -m marquedown render -i ./md -o ./public -t ./templates/
-page.html # This is for the GitLab Pages publication mkdir .public cp -r public
-.public mv .public public ```
+``` ### QR codes QR codes can be generated and referenced automatically via the
+`render` command. If you want to generate QR codes with
+`marquedown.marquedown`, you can follow the example below. #### Example #####
+Marquedown ```md ![qr:monero-wallet](monero:abcdefghijklmnopqrstuvwxyz) ```
+##### Python ```py from marquedown import marquedown with open('document.mqd',
+'r') as f: document = f.read() with open('public/document.html', 'w') as f:
+rendered = marquedown(document, qrgen='public/qr:qr') f.write(rendered) ``` The
+string provided to `qrgen` is two paths separated by a colon. 1. Where to save
+the generated images 2. What directory to reference in the HTML `src` parameter
+##### The generated HTML ```html [monero-wallet] ``` ## Commands ### `render`:
+Render documents You can render an entire directory and its subdirectories of
+Markdown or Marquedown documents. This can be used to automate rendering pages
+for your website. Do `python -m marquedown render --help` for list of options.
+#### Example For a few of my websites hosted on GitLab, I have it set up to run
+*this* on push: ```sh # Render document python -m marquedown render -i "./mqd"
+-o "./public" -t "./templates/page.html" # This is for the GitLab Pages
+publication mkdir .public cp -r public .public mv .public public ```
```

