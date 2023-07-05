# Comparing `tmp/curcheck-1.1.3b0.tar.gz` & `tmp/curcheck-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck-1.1.3b0.tar", last modified: Wed Jun 21 20:23:20 2023, max compression
+gzip compressed data, was "curcheck-1.1.4.tar", max compression
```

## Comparing `curcheck-1.1.3b0.tar` & `curcheck-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:23:20.350671 curcheck-1.1.3b0/
--rw-rw-rw-   0        0        0     1086 2023-01-06 12:52:22.000000 curcheck-1.1.3b0/LICENSE.md
--rw-rw-rw-   0        0        0      248 2023-06-21 20:23:20.350671 curcheck-1.1.3b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 20:23:20.334666 curcheck-1.1.3b0/curcheck/
--rw-rw-rw-   0        0        0      473 2023-06-07 10:59:42.000000 curcheck-1.1.3b0/curcheck/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-20 20:06:51.000000 curcheck-1.1.3b0/curcheck/config.py
--rw-rw-rw-   0        0        0     1061 2023-06-21 19:55:22.000000 curcheck-1.1.3b0/curcheck/dispatcher.py
--rw-rw-rw-   0        0        0     6731 2023-06-20 20:06:31.000000 curcheck-1.1.3b0/curcheck/events.py
--rw-rw-rw-   0        0        0      766 2023-06-21 19:56:05.000000 curcheck-1.1.3b0/curcheck/gui.py
--rw-rw-rw-   0        0        0     3028 2023-06-21 20:20:54.000000 curcheck-1.1.3b0/curcheck/router.py
--rw-rw-rw-   0        0        0       73 2023-06-20 20:06:13.000000 curcheck-1.1.3b0/curcheck/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:23:20.349670 curcheck-1.1.3b0/curcheck.egg-info/
--rw-rw-rw-   0        0        0      248 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-21 20:23:20.000000 curcheck-1.1.3b0/curcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 20:23:20.352671 curcheck-1.1.3b0/setup.cfg
--rw-rw-rw-   0        0        0      529 2023-06-21 20:23:15.000000 curcheck-1.1.3b0/setup.py
+-rw-r--r--   0        0        0      473 2023-06-07 10:59:42.004006 curcheck-1.1.4/curcheck/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 11:30:37.676819 curcheck-1.1.4/curcheck/bot.py
+-rw-r--r--   0        0        0       61 2023-06-20 20:06:51.342155 curcheck-1.1.4/curcheck/config.py
+-rw-r--r--   0        0        0     1061 2023-06-21 19:55:22.368193 curcheck-1.1.4/curcheck/dispatcher.py
+-rw-r--r--   0        0        0     6757 2023-06-30 09:48:58.967164 curcheck-1.1.4/curcheck/events.py
+-rw-r--r--   0        0        0      810 2023-06-28 08:21:32.835014 curcheck-1.1.4/curcheck/gui.py
+-rw-r--r--   0        0        0       47 2023-06-30 09:22:31.315113 curcheck-1.1.4/curcheck/middlewares.py
+-rw-r--r--   0        0        0     3106 2023-06-28 08:36:11.961399 curcheck-1.1.4/curcheck/router.py
+-rw-r--r--   0        0        0       73 2023-06-20 20:06:13.035766 curcheck-1.1.4/curcheck/utils.py
+-rw-r--r--   0        0        0     1086 2023-01-06 12:52:22.705303 curcheck-1.1.4/LICENSE.md
+-rw-r--r--   0        0        0      452 2023-07-05 15:46:48.750997 curcheck-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-06-21 20:22:04.879283 curcheck-1.1.4/README.md
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 curcheck-1.1.4/PKG-INFO
```

### Comparing `curcheck-1.1.3b0/LICENSE.md` & `curcheck-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.3b0/curcheck/dispatcher.py` & `curcheck-1.1.4/curcheck/dispatcher.py`

 * *Files identical despite different names*

### Comparing `curcheck-1.1.3b0/curcheck/events.py` & `curcheck-1.1.4/curcheck/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             self.link: str = self.domain + self.url
 
 
 class EventPage(AbstractEvent):
     def __init__(self, domain: str, url: str, is_browser: bool = False):
         super().__init__(domain=domain, url=url, is_browser=is_browser)
 
-    def __call__(self, func):
+    def __call__(self, func: Awaitable):
         @functools.wraps(func) 
         async def spa_task(browser: Browser):
             page = await browser.newPage()
             await page.goto(url=self.link)
             await func(page)
             await page.close()
 
@@ -68,15 +68,15 @@
         super().__init__(domain=domain, url=url, is_browser=is_browser)
 
         self.pages_links_xpath = pages_links_xpath
         self.count_in_approach = count_in_approach
 
         self.pages: List[EventPage] = []
 
-    def __call__(self, func):
+    def __call__(self, func: Awaitable):
         @functools.wraps(func) 
         async def spa_task(browser: Browser):
             base_page = await browser.newPage()
             await base_page.goto(url=self.domain+self.url)
             
             if self.pages_links_xpath.split("/")[-1][0] == "@":
                 html_attr = f'.getAttribute("{self.pages_links_xpath.split("/")[-1][1:]}")'
@@ -165,15 +165,15 @@
     ) -> None:
         super().__init__(domain=domain, url=url, is_browser=is_browser)
 
         self.count = count
         self.timeout = timeout
         self.i = 0
 
-    def __call__(self, func) -> Any:
+    def __call__(self, func: Awaitable):
         @functools.wraps(func)
         async def spa_task(browser: Browser):
             self.browser = browser
             page = await self.browser.newPage()
             await self.page.goto(self.link)
             while self.i <= self.count or self.count == None:
                 self.i += 1
```

### Comparing `curcheck-1.1.3b0/curcheck/router.py` & `curcheck-1.1.4/curcheck/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
         self.browser: Browser = None
 
         self.pages: List[EventPage] = []
         self.paginators: List[EventPaginator] = []
         self.longpolls: List[EventLongpoll] = []
 
+    def register_middleware(
+        self, middleware
+    ):
+        pass
 
     def paginate_page(
         self, url: str, pages_links_xpath: str, count_in_approach: int = 10
     ) -> EventPaginator:
         paginator = EventPaginator(
             domain=self.domain, 
             url=url,
```

