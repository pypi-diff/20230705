# Comparing `tmp/nlpia2_wikipedia-1.5.3.tar.gz` & `tmp/nlpia2_wikipedia-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpia2_wikipedia-1.5.3.tar", max compression
+gzip compressed data, was "nlpia2_wikipedia-1.5.4.tar", max compression
```

## Comparing `nlpia2_wikipedia-1.5.3.tar` & `nlpia2_wikipedia-1.5.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1057 2022-02-24 21:47:29.044908 nlpia2_wikipedia-1.5.3/LICENSE
--rw-r--r--   0        0        0     3798 2022-05-04 23:25:18.637807 nlpia2_wikipedia-1.5.3/README.md
--rw-r--r--   0        0        0     1616 2023-07-01 00:19:11.797373 nlpia2_wikipedia-1.5.3/pyproject.toml
--rw-r--r--   0        0        0       99 2023-07-01 00:11:01.060006 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/__init__.py
--rw-r--r--   0        0        0     2420 2023-06-30 23:36:01.865166 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/exceptions.py
--rw-r--r--   0        0        0     1623 2023-07-01 00:11:05.932013 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/parsers.py
--rw-r--r--   0        0        0     1069 2023-06-30 23:31:53.674041 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/util.py
--rw-r--r--   0        0        0    23481 2022-02-24 22:35:10.763977 nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/wikipedia.py
--rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.3/setup.py
--rw-r--r--   0        0        0     5250 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-24 21:47:29.044908 nlpia2_wikipedia-1.5.4/LICENSE
+-rw-r--r--   0        0        0     3798 2022-05-04 23:25:18.637807 nlpia2_wikipedia-1.5.4/README.md
+-rw-r--r--   0        0        0     1633 2023-07-04 22:26:53.425674 nlpia2_wikipedia-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-07-01 00:11:01.060006 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-30 23:36:01.865166 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/exceptions.py
+-rw-r--r--   0        0        0      184 2023-07-04 20:01:10.064999 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/parsers.py
+-rw-r--r--   0        0        0     2873 2023-07-04 22:12:15.959850 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/util.py
+-rw-r--r--   0        0        0    26553 2023-07-04 21:56:30.536368 nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/wikipedia.py
+-rw-r--r--   0        0        0     4788 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.4/setup.py
+-rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 nlpia2_wikipedia-1.5.4/PKG-INFO
```

### Comparing `nlpia2_wikipedia-1.5.3/LICENSE` & `nlpia2_wikipedia-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.3/README.md` & `nlpia2_wikipedia-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.3/pyproject.toml` & `nlpia2_wikipedia-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nlpia2_wikipedia"
-version = "1.5.3"
+version = "1.5.4"
 description = "Updated version of `wikipedia` package because original repo has been abandoned since 2014."
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 authors = [
     "Hobson Lane <hobson@tangibleai.com>",
     ]
 homepage = "https://gitlab.com/tangibleai/community/nlpia2_wikipedia"
@@ -49,14 +49,15 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.1"
 beautifulsoup4 = ">=4.11"
 requests = ">=2.0,<3.0.0"
+pandas = ">=2.0"
 
 [tool.poetry.dev-dependencies]
 tox = ">=3.18"
 pytest = ">=6.2.0"
 pytest-cov = ">=3.0.0"
 pydocstyle = ">=5.1.1"
 Sphinx = ">=4.4.0"
```

### Comparing `nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/exceptions.py` & `nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/exceptions.py`

 * *Files identical despite different names*

### Comparing `nlpia2_wikipedia-1.5.3/src/nlpia2_wikipedia/wikipedia.py` & `nlpia2_wikipedia-1.5.4/src/nlpia2_wikipedia/wikipedia.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from .exceptions import (
     PageError, DisambiguationError, RedirectError, HTTPTimeoutError,
     WikipediaException, ODD_ERROR_MESSAGE
 )
 from .util import cache, stdout_encode
 from .util import debug  # noqa
+import pandas as pd
 import re
 
 log = logging.getLogger(__name__)
 
 API_URL = 'http://en.wikipedia.org/w/api.php'
 RATE_LIMIT = False
 RATE_LIMIT_MIN_WAIT = None
@@ -265,45 +266,64 @@
 
     * title - the title of the page to load
     * pageid - the numeric pageid of the page to load
     * auto_suggest - let Wikipedia find a valid page title for the query
     * redirect - allow redirection without raising RedirectError
     * preload - load content, summary, images, references, and links during initialization
     '''
-
+    if title and not pageid and isinstance(title, int):
+        pageid = title
+        title = None
     if title is not None:
         suggestion = title
         if auto_suggest:
             results, suggestion = search(title, results=1, suggestion=True)
             try:
                 suggestion = suggestion or results[0]
             except IndexError:
-                # if there is no suggestion or search results, the page doesn't exist
-                raise PageError(title)
+                log.info('Unable to automatically suggest a title')
+                # FIXME: If the suggestion or search results, does the page really not exist?
+                # raise PageError(title)
+        try:
+            # search for exact match first, even if alternative suggestions found
+            return WikipediaPage(
+                title.strip().replace(' ', '_').title(),
+                redirect=redirect, preload=preload
+                )
+        except (PageError, DisambiguationError):
+            try:
+                return WikipediaPage(suggestion, redirect=redirect, preload=preload)
+            except (PageError, DisambiguationError) as e:
+                log.warning(f'BAD SUGGESTION: {e}')
+                log.warning(f'BAD SUGGESTION: {__name__}.suggest({title}) => {suggestion}')
+                if suggestion != title:
+                    return WikipediaPage(title, redirect=redirect, preload=preload)
+                raise e
+    if pageid:
         try:
-            return WikipediaPage(suggestion, redirect=redirect, preload=preload)
+            return WikipediaPage(pageid=pageid, preload=preload)
         except (PageError, DisambiguationError) as e:
-            log.warning(f'BAD SUGGESTION: {e}')
-            log.warning(f'BAD SUGGESTION: {__name__}.suggest({title}) => {suggestion}')
-            if suggestion != title:
-                return WikipediaPage(title, redirect=redirect, preload=preload)
+            log.exception()
+            for i in range(2):
+                if suggestion != title:
+                    return WikipediaPage(title, redirect=redirect, preload=preload)
+                title = title.strip().replace(' ', '_').title()
             raise e
-    elif pageid is not None:
-        return WikipediaPage(pageid=pageid, preload=preload)
     else:
         raise ValueError("Either a title or a pageid must be specified")
 
 
 class WikipediaPage(object):
     '''
     Contains data from a Wikipedia page.
     Uses property methods to filter data from the raw HTML.
     '''
 
-    def __init__(self, title=None, pageid=None, redirect=True, preload=False, original_title=''):
+    def __init__(self, title=None, pageid=None, redirect=True, preload=False, original_title='', markdown=False):
+        # FIXME: parse page.content as markdown (headings with ## instead of ==
         if title is not None:
             self.title = title
             self.original_title = original_title or title
         elif pageid is not None:
             self.pageid = pageid
         else:
             raise ValueError("Either a title or a pageid must be specified")
@@ -535,14 +555,16 @@
                 'exintro': '',
             }
             if not getattr(self, 'title', None) is None:
                 query_params['titles'] = self.title
             else:
                 query_params['pageids'] = self.pageid
 
+            # FIXME: insert spaces at end of sentences (or don't strip them)
+            # FIXME: add double newlines between paragraphs
             request = _wiki_request(query_params)
             self._summary = request['query']['pages'][self.pageid]['extract']
 
         return self._summary
 
     @property
     def images(self):
@@ -658,26 +680,30 @@
             if not getattr(self, 'title', None) is None:
                 query_params["page"] = self.title
 
             request = _wiki_request(query_params)
             self._sections = [section['line'] for section in request['parse']['sections']]
 
         return self._sections
+        # FIXME:
+        return dict(zip(self._section_names, self._section_texts))
 
     def section(self, section_title):
         '''
         Get the plain text content of a section from `self.sections`.
         Returns None if `section_title` isn't found, otherwise returns a whitespace stripped string.
 
         This is a convenience method that wraps self.content.
 
         .. warning:: Calling `section` on a section that has subheadings will NOT return
                the full text of all of the subsections. It only gets the text between
                `section_title` and the next subheading, which is often empty.
         '''
+        if isinstance(section_title, int):
+            section_title = self.sections[0]
 
         section = u"== {} ==".format(section_title)
         try:
             index = self.content.index(section) + len(section)
         except ValueError:
             return None
 
@@ -685,14 +711,55 @@
             next_index = self.content.index("==", index)
         except ValueError:
             next_index = len(self.content)
 
         return self.content[index:next_index].lstrip("=").strip()
 
 
+    def to_dataframe(self, re_heading=r'^\s*[=]+ [^=]+ [=]+\s*'):
+        """ Split wikitext into paragraphs and return a dataframe with columns for headings (title, h1, h2, h3, ...)
+
+        TODO: create a method or property within a wikipedia.Page class with this function
+
+        >>> from nlpia2_wikipedia.wikipedia import wikipedia as wiki
+        >>> page = wiki.page('Large language model')
+        >>> df = paragraphs_dataframe(page)
+        >>> df.head(2)
+
+        """
+        paragraphs = [p for p in page.content.split('\n\n')]
+        headings = [page.title]
+        df_paragraphs = []
+        for p in paragraphs:
+            p = p.strip()
+            p_headings = re.findall(re_heading, p)
+            # TODO strip headings from front of p
+            # TODO use match instead of findall (only need 1)
+            while p_headings:
+                    h = p_headings[0]
+                    p = p[len(h):].strip()
+                    h = h.strip()
+                    level = len([c for c in h if c == '=']) + 1
+                    h = h.strip('=').strip()
+                    headings = headings[:level]
+                    if len(headings) <= level:
+                        headings = headings + [''] * (level - len(headings))
+                        headings[level - 1] = h
+                    p_headings = re.findall(re_heading, p)
+            if p:
+                p_record = dict(text=p, title=page.title)
+                p_record.update({f'h{i}': h for (i, h) in enumerate(headings)}) 
+                df_paragraphs.append(p_record)
+        
+        df = pd.DataFrame(df_paragraphs).fillna('')
+        df['h_all'] = [
+            ': '.join(h for h in row.loc['h0':] if h) for i, row in df.iterrows()]
+        return df
+    
+
 @cache
 def languages():
     '''
     List all the currently supported language prefixes (usually ISO language code).
 
     Can be inputted to `set_lang` to change the Mediawiki that `wikipedia` requests
     results from.
@@ -748,8 +815,9 @@
         time.sleep(int(wait_time.total_seconds()))
 
     r = requests.get(API_URL, params=params, headers=headers)
 
     if RATE_LIMIT:
         RATE_LIMIT_LAST_CALL = datetime.now()
 
+    # FIXME: find out if json contains spaces at end of sentence
     return r.json()
```

### Comparing `nlpia2_wikipedia-1.5.3/setup.py` & `nlpia2_wikipedia-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['nlpia2_wikipedia']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beautifulsoup4>=4.11', 'poetry>=1.1', 'requests>=2.0,<3.0.0']
+['beautifulsoup4>=4.11', 'pandas>=2.0', 'poetry>=1.1', 'requests>=2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'nlpia2-wikipedia',
-    'version': '1.5.3',
+    'version': '1.5.4',
     'description': 'Updated version of `wikipedia` package because original repo has been abandoned since 2014.',
     'long_description': '# Wikipedia\n\n[![image](https://travis-ci.org/goldsmith/Wikipedia.png?branch=master)](https://travis-ci.org/goldsmith/Wikipedia)\n\n[![image](https://pypip.in/d/wikipedia/badge.png)](https://crate.io/packages/wikipedia)\n\n[![image](https://pypip.in/v/wikipedia/badge.png)](https://crate.io/packages/wikipedia)\n\n[![License](https://pypip.in/license/wikipedia/badge.png)](https://pypi.python.org/pypi/wikipedia/)\n\n**Wikipedia** is a Python library that makes it easy to access and parse\ndata from Wikipedia.\n\nSearch Wikipedia, get article summaries, get data like links and images\nfrom a page, and more. Wikipedia wraps the [MediaWiki\nAPI](https://www.mediawiki.org/wiki/API) so you can focus on using\nWikipedia data, not getting it.\n\n``` {.python}\n>>> import wikipedia\n>>> print wikipedia.summary("Wikipedia")\n# Wikipedia (/ˌwɪkɨˈpiːdiə/ or /ˌwɪkiˈpiːdiə/ WIK-i-PEE-dee-ə) is a collaboratively edited, multilingual, free Internet encyclopedia supported by the non-profit Wikimedia Foundation...\n\n>>> wikipedia.search("Barack")\n# [u\'Barak (given name)\', u\'Barack Obama\', u\'Barack (brandy)\', u\'Presidency of Barack Obama\', u\'Family of Barack Obama\', u\'First inauguration of Barack Obama\', u\'Barack Obama presidential campaign, 2008\', u\'Barack Obama, Sr.\', u\'Barack Obama citizenship conspiracy theories\', u\'Presidential transition of Barack Obama\']\n\n>>> ny = wikipedia.page("New York")\n>>> ny.title\n# u\'New York\'\n>>> ny.url\n# u\'http://en.wikipedia.org/wiki/New_York\'\n>>> ny.content\n# u\'New York is a state in the Northeastern region of the United States. New York is the 27th-most exten\'...\n>>> ny.links[0]\n# u\'1790 United States Census\'\n\n>>> wikipedia.set_lang("fr")\n>>> wikipedia.summary("Facebook", sentences=1)\n# Facebook est un service de réseautage social en ligne sur Internet permettant d\'y publier des informations (photographies, liens, textes, etc.) en contrôlant leur visibilité par différentes catégories de personnes.\n```\n\nNote: this library was designed for ease of use and simplicity, not for\nadvanced use. If you plan on doing serious scraping or automated\nrequests, please use\n[Pywikipediabot](http://www.mediawiki.org/wiki/Manual:Pywikipediabot)\n(or one of the other more advanced [Python MediaWiki API\nwrappers](http://en.wikipedia.org/wiki/Wikipedia:Creating_a_bot#Python)),\nwhich has a larger API, rate limiting, and other features so we can be\nconsiderate of the MediaWiki infrastructure.\n\n## Installation\n\nTo install Wikipedia, simply run:\n\n    $ pip install wikipedia\n\nWikipedia is compatible with Python 2.6+ (2.7+ to run unittest discover)\nand Python 3.3+.\n\n## Documentation\n\nRead the docs at <https://wikipedia.readthedocs.org/en/latest/>.\n\n-   [Quickstart](https://wikipedia.readthedocs.org/en/latest/quickstart.html)\n-   [Full API](https://wikipedia.readthedocs.org/en/latest/code.html)\n\nTo run tests, clone the [repository on\nGitHub](https://github.com/goldsmith/Wikipedia), then run:\n\n    $ pip install -r requirements.txt\n    $ bash runtests  # will run tests for python and python3\n    $ python -m unittest discover tests/ \'*test.py\'  # manual style\n\nin the root project directory.\n\nTo build the documentation yourself, after installing requirements.txt,\nrun:\n\n    $ pip install sphinx\n    $ cd docs/\n    $ make html\n\n## License\n\nMIT licensed. See the [LICENSE\nfile](https://github.com/goldsmith/Wikipedia/blob/master/LICENSE) for\nfull details.\n\n## Credits\n\n-   [wiki-api](https://github.com/richardasaurus/wiki-api) by\n    \\@richardasaurus for inspiration\n-   \\@nmoroze and \\@themichaelyang for feedback and suggestions\n-   The [Wikimedia Foundation](http://wikimediafoundation.org/wiki/Home)\n    for giving the world free access to data\n\n[![Bitdeli badge](https://d2weczhvl823v0.cloudfront.net/goldsmith/wikipedia/trend.png)](https://bitdeli.com/free)\n',
     'author': 'Hobson Lane',
     'author_email': 'hobson@tangibleai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tangibleai/community/nlpia2_wikipedia',
```

### Comparing `nlpia2_wikipedia-1.5.3/PKG-INFO` & `nlpia2_wikipedia-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpia2-wikipedia
-Version: 1.5.3
+Version: 1.5.4
 Summary: Updated version of `wikipedia` package because original repo has been abandoned since 2014.
 Home-page: https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 License: AGPL-3.0-or-later
 Keywords: wiki,Wikipedia,scraping,api,wrapper,crawler,markdown,html,parser
 Author: Hobson Lane
 Author-email: hobson@tangibleai.com
 Requires-Python: >=3.8
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: beautifulsoup4 (>=4.11)
+Requires-Dist: pandas (>=2.0)
 Requires-Dist: poetry (>=1.1)
 Requires-Dist: requests (>=2.0,<3.0.0)
 Project-URL: Documentation, https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 Project-URL: Repository, https://gitlab.com/tangibleai/community/nlpia2_wikipedia
 Description-Content-Type: text/markdown
 
 # Wikipedia
```

