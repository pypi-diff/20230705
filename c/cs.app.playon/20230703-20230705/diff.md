# Comparing `tmp/cs.app.playon-20230703.tar.gz` & `tmp/cs.app.playon-20230705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.app.playon-20230703.tar", last modified: Mon Jul  3 10:17:17 2023, max compression
+gzip compressed data, was "cs.app.playon-20230705.tar", last modified: Wed Jul  5 00:19:04 2023, max compression
```

## Comparing `cs.app.playon-20230703.tar` & `cs.app.playon-20230705.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.080803 cs.app.playon-20230703/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-03 10:17:01.000000 cs.app.playon-20230703/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6847 2023-07-03 10:17:17.080931 cs.app.playon-20230703/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    13326 2023-07-03 10:17:03.000000 cs.app.playon-20230703/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.075575 cs.app.playon-20230703/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.075927 cs.app.playon-20230703/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.076059 cs.app.playon-20230703/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.080431 cs.app.playon-20230703/lib/python/cs/app/
--rw-r--r--   0 cameron    (501) cameron    (502)    32942 2023-07-03 10:16:46.000000 cs.app.playon-20230703/lib/python/cs/app/playon.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-03 10:17:17.080067 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6847 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      373 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       46 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      327 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-03 10:17:17.000000 cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     7444 2023-07-03 10:17:07.000000 cs.app.playon-20230703/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1263 2023-07-03 10:17:17.081639 cs.app.playon-20230703/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-03 10:17:03.000000 cs.app.playon-20230703/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-05 00:19:04.027426 cs.app.playon-20230705/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-05 00:18:48.000000 cs.app.playon-20230705/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6758 2023-07-05 00:19:04.027537 cs.app.playon-20230705/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    13237 2023-07-05 00:18:50.000000 cs.app.playon-20230705/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-05 00:19:04.022775 cs.app.playon-20230705/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-05 00:19:04.023114 cs.app.playon-20230705/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-05 00:19:04.023244 cs.app.playon-20230705/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-05 00:19:04.027062 cs.app.playon-20230705/lib/python/cs/app/
+-rw-r--r--   0 cameron    (501) cameron    (502)    33744 2023-07-05 00:18:40.000000 cs.app.playon-20230705/lib/python/cs/app/playon.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-05 00:19:04.026708 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6758 2023-07-05 00:19:04.000000 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      373 2023-07-05 00:19:04.000000 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-05 00:19:04.000000 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       46 2023-07-05 00:19:04.000000 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      327 2023-07-05 00:19:04.000000 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-05 00:19:04.000000 cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7358 2023-07-05 00:18:55.000000 cs.app.playon-20230705/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1263 2023-07-05 00:19:04.028115 cs.app.playon-20230705/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-05 00:18:50.000000 cs.app.playon-20230705/setup.py
```

### Comparing `cs.app.playon-20230703/PKG-INFO` & `cs.app.playon-20230705/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.app.playon
-Version: 20230703
+Version: 20230705
 Summary: PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -17,20 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230703*:
-* PlayOnAPI: features, feature, featured_image_url, service_image_url.
-* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
-* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
-* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
-* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
+*Latest release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in "playon dl".
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -46,15 +42,15 @@
     Usage: playon subcommand [args...]
 
         Environment:
           PLAYON_USER               PlayOn login name, default from $EMAIL.
           PLAYON_PASSWORD           PlayOn password.
                                     This is obtained from .netrc if omitted.
           PLAYON_FILENAME_FORMAT  Format string for downloaded filenames.
-                                    Default: {series_prefix}{playon.Name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
+                                    Default: {series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
           PLAYON_TAGS_DBURL         Location of state tags database.
                                     Default: ~/var/playon.sqlite
 
         Recording specification:
           an int        The specific recording id.
           all           All known recordings.
           downloaded    Recordings already downloaded.
@@ -117,14 +113,17 @@
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 # Release Log
 
 
 
+*Release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in "playon dl".
+
 *Release 20230703*:
 * PlayOnAPI: features, feature, featured_image_url, service_image_url.
 * PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
 * PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
 * Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
 * PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
```

### Comparing `cs.app.playon-20230703/README.md` & `cs.app.playon-20230705/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230703*:
-* PlayOnAPI: features, feature, featured_image_url, service_image_url.
-* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
-* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
-* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
-* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
+*Latest release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in "playon dl".
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -121,15 +117,15 @@
     Usage: playon subcommand [args...]
 
         Environment:
           PLAYON_USER               PlayOn login name, default from $EMAIL.
           PLAYON_PASSWORD           PlayOn password.
                                     This is obtained from .netrc if omitted.
           PLAYON_FILENAME_FORMAT  Format string for downloaded filenames.
-                                    Default: {series_prefix}{playon.Name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
+                                    Default: {series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
           PLAYON_TAGS_DBURL         Location of state tags database.
                                     Default: ~/var/playon.sqlite
 
         Recording specification:
           an int        The specific recording id.
           all           All known recordings.
           downloaded    Recordings already downloaded.
@@ -324,14 +320,17 @@
 *Method `Recording.status(self)`*:
 Return a short status string.
 
 # Release Log
 
 
 
+*Release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in "playon dl".
+
 *Release 20230703*:
 * PlayOnAPI: features, feature, featured_image_url, service_image_url.
 * PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
 * PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
 * Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
 * PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
```

### Comparing `cs.app.playon-20230703/lib/python/cs/app/playon.py` & `cs.app.playon-20230705/lib/python/cs/app/playon.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from cs.result import bg as bg_result, report as report_results, CancellationError
 from cs.service_api import HTTPServiceAPI, RequestsNoAuth
 from cs.sqltags import SQLTags, SQLTagSet
 from cs.threads import monitor, bg as bg_thread
 from cs.units import BINARY_BYTES_SCALE
 from cs.upd import print  # pylint: disable=redefined-builtin
 
-__version__ = '20230703'
+__version__ = '20230705'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Programming Language :: Python",
@@ -82,15 +82,15 @@
 }
 
 DBURL_ENVVAR = 'PLAYON_TAGS_DBURL'
 DBURL_DEFAULT = '~/var/playon.sqlite'
 
 FILENAME_FORMAT_ENVVAR = 'PLAYON_FILENAME_FORMAT'
 DEFAULT_FILENAME_FORMAT = (
-    '{series_prefix}{playon.Name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}'
+    '{series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}'
 )
 
 # download parallelism
 DEFAULT_DL_PARALLELISM = 2
 
 def main(argv=None):
   ''' Playon command line mode;
@@ -247,16 +247,16 @@
 
     @typechecked
     def _dl(dl_id: int, sem):
       try:
         with sqltags:
           filename = api[dl_id].format_as(filename_format)
           filename = (
-              filename.lower().replace(' - ', '--').replace('_', ':')
-              .replace(' ', '-').replace(os.sep, ':') + '.'
+              filename.lower().replace(' - ', '--').replace('----', '--')
+              .replace('_', ':').replace(' ', '-').replace(os.sep, ':') + '.'
           )
           try:
             api.download(dl_id, filename=filename)
           except ValueError as e:
             warning("download fails: %s", e)
             return None
           return filename
@@ -552,14 +552,36 @@
     if se_parts:
       parts.append(''.join(se_parts))
     if not parts:
       return ''
     return sep.join(parts) + sep
 
   @format_attribute
+  def series_episode_name(self):
+    name = self.playon.Name
+    name = name.strip()
+    if self.playon.Season is not None:
+      spfx, n, offset = get_prefix_n(name, 's', n=self.playon.Season)
+      if spfx is not None:
+        assert name.startswith(f's{self.playon.Season:02d}')
+        name = name[offset:]
+    if self.playon.Episode is not None:
+      epfx, n, offset = get_prefix_n(name, 'e', n=self.playon.Episode)
+      if epfx is not None:
+        assert name.startswith(f'e{self.playon.Episode:02d}')
+        name = name[offset:]
+      name = name.lstrip()
+      epfx, n, offset = get_prefix_n(
+          name.lower(), 'episode ', n=self.playon.Episode
+      )
+      if epfx is not None:
+        name = name[offset:]
+    return name.strip()
+
+  @format_attribute
   def is_available(self):
     ''' Is a recording available for download?
     '''
     return not self.is_expired() and not self.is_queued()
 
   @format_attribute
   def is_queued(self):
```

### Comparing `cs.app.playon-20230703/lib/python/cs.app.playon.egg-info/PKG-INFO` & `cs.app.playon-20230705/lib/python/cs.app.playon.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.app.playon
-Version: 20230703
+Version: 20230705
 Summary: PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -17,20 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230703*:
-* PlayOnAPI: features, feature, featured_image_url, service_image_url.
-* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
-* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
-* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
-* PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
+*Latest release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in "playon dl".
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -46,15 +42,15 @@
     Usage: playon subcommand [args...]
 
         Environment:
           PLAYON_USER               PlayOn login name, default from $EMAIL.
           PLAYON_PASSWORD           PlayOn password.
                                     This is obtained from .netrc if omitted.
           PLAYON_FILENAME_FORMAT  Format string for downloaded filenames.
-                                    Default: {series_prefix}{playon.Name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
+                                    Default: {series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
           PLAYON_TAGS_DBURL         Location of state tags database.
                                     Default: ~/var/playon.sqlite
 
         Recording specification:
           an int        The specific recording id.
           all           All known recordings.
           downloaded    Recordings already downloaded.
@@ -117,14 +113,17 @@
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 # Release Log
 
 
 
+*Release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in "playon dl".
+
 *Release 20230703*:
 * PlayOnAPI: features, feature, featured_image_url, service_image_url.
 * PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
 * PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
 * Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
 * PlayOnCommand.cmd_downloaded: add 'downloaded" tag to specified recordings.
```

### Comparing `cs.app.playon-20230703/pyproject.toml` & `cs.app.playon-20230705/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -33,33 +33,29 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230703"
+version = "20230705"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 PlayOn facilities, primarily access to the download API.
 Includes a nice command line tool.
 
-*Latest release 20230703*:
-* PlayOnAPI: features, feature, featured_image_url, service_image_url.
-* PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
-* PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
-* Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
-* PlayOnCommand.cmd_downloaded: add 'downloaded\" tag to specified recordings.
+*Latest release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in \"playon dl\".
 
 ## Function `main(argv=None)`
 
 Playon command line mode;
 see the `PlayOnCommand` class below.
 
 ## Class `PlayOnAPI(cs.service_api.HTTPServiceAPI, cs.service_api.ServiceAPI, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -75,15 +71,15 @@
     Usage: playon subcommand [args...]
 
         Environment:
           PLAYON_USER               PlayOn login name, default from $EMAIL.
           PLAYON_PASSWORD           PlayOn password.
                                     This is obtained from .netrc if omitted.
           PLAYON_FILENAME_FORMAT  Format string for downloaded filenames.
-                                    Default: {series_prefix}{playon.Name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
+                                    Default: {series_prefix}{series_episode_name}--{resolution}--{playon.ProviderID}--playon--{playon.ID}
           PLAYON_TAGS_DBURL         Location of state tags database.
                                     Default: ~/var/playon.sqlite
 
         Recording specification:
           an int        The specific recording id.
           all           All known recordings.
           downloaded    Recordings already downloaded.
@@ -146,14 +142,17 @@
 
 An `SQLTagSet` with knowledge about PlayOn recordings.
 
 # Release Log
 
 
 
+*Release 20230705*:
+DEFAULT_FILENAME_FORMAT: replace naive playon.Name with series_episode_name which is the name with leading series/episode info removed, honour in \"playon dl\".
+
 *Release 20230703*:
 * PlayOnAPI: features, feature, featured_image_url, service_image_url.
 * PlayOnCommand: new cmd_feature like cmd_service but for featured shows.
 * PlayOnAPI.suburl: infer _base_url from api_version if _base_url is None and api_version is provided.
 * Recording.is_downloaded: also check for a 'downloaded' tag, fallback for when the downloaded_path is empty.
 * PlayOnCommand.cmd_downloaded: add 'downloaded\" tag to specified recordings.
 
@@ -175,13 +174,13 @@
 Bugfix criteria for refreshing the PlayOn state.
 
 *Release 20211212*:
 Initial release."""
 content-type = "text/markdown"
 
 [build-system]
+build-backend = "setuptools.build_meta"
 requires = [
     "setuptools >= 61.2",
     "trove-classifiers",
     "wheel",
 ]
-build-backend = "setuptools.build_meta"
```

### Comparing `cs.app.playon-20230703/setup.cfg` & `cs.app.playon-20230705/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.app.playon
-version = 20230703
+version = 20230705
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = PlayOn facilities, primarily access to the download API. Includes a nice command line tool.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

