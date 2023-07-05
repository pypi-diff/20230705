# Comparing `tmp/wasc-0.2.0.tar.gz` & `tmp/wasc-0.3.0.tar.gz`

## Comparing `wasc-0.2.0.tar` & `wasc-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 wasc-0.2.0/data/agro_alim.csv
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wasc-0.2.0/data/criteria.yml
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wasc-0.2.0/data/example_websites.csv
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/__main__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/abstract_checker.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/checker_factory.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/criterion.py
--rw-r--r--   0        0        0    15835 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/default_checkers.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/report.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/utils.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 wasc-0.2.0/src/wasc/cli/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/test_checker.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/data/crit_example.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.2.0/tests/data/url_example.csv
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wasc-0.2.0/.gitignore
--rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wasc-0.2.0/README.md
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 wasc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 wasc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 wasc-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 wasc-0.3.0/requirements_dev.txt
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wasc-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wasc-0.3.0/data/checkers.csv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.3.0/data/example_websites.csv
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 wasc-0.3.0/data/sub_list.csv
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/checkers.md
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/license.md
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 wasc-0.3.0/docs/releases.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/__about__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/__main__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/abstract_checker.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/checker_factory.py
+-rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/default_checkers.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/utils.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 wasc-0.3.0/src/wasc/cli/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/test_checker.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/test_checker_factory.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/data/checkers_example.csv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 wasc-0.3.0/tests/data/url_example.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 wasc-0.3.0/.gitignore
+-rw-r--r--   0        0        0    21439 2020-02-02 00:00:00.000000 wasc-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 wasc-0.3.0/README.md
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 wasc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 wasc-0.3.0/PKG-INFO
```

### Comparing `wasc-0.2.0/src/wasc/abstract_checker.py` & `wasc-0.3.0/src/wasc/abstract_checker.py`

 * *Files identical despite different names*

### Comparing `wasc-0.2.0/src/wasc/checker_factory.py` & `wasc-0.3.0/src/wasc/checker_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,45 @@
 
         Returns
         -------
         The checker object corresponding to the checker name
         """
         return self.__checker_dict[checker_name]()
 
+    def available(self):
+        """
+        Returns the list of checkers names
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        : list
+        The list of checkers names
+        """
+        return list(self.__checker_dict.keys())
+
+    def is_registered(self, checker_name : str):
+        """
+        Returns the list of checkers as pair (checker.name, checker.description)
+
+        Parameters
+        ----------
+        checker_name : str
+            A checker name
+        Returns
+        -------
+        : bool
+        True is the checker name is known
+        """
+        return checker_name in self.__checker_dict
+
 checker_factory = CheckerFactory()
 checker_factory.register("DFTT01", dft.DFTT01)
 checker_factory.register("DFTT02", dft.DFTT02)
-checker_factory.register("DFTT05", dft.DFTT05)
+checker_factory.register("AccessRateChecker", dft.AccessRateChecker)
 checker_factory.register("LangChecker", dft.LangChecker)
 checker_factory.register("DoctypeChecker", dft.DoctypeChecker)
 checker_factory.register("AccessChecker", dft.AccessChecker)
 checker_factory.register("AccessLinkChecker", dft.AccessLinkChecker)
-checker_factory.register("MentionsLegalesChecker", dft.MentionsLegalesChecker)
+checker_factory.register("LegalChecker", dft.LegalChecker)
```

### Comparing `wasc-0.2.0/src/wasc/default_checkers.py` & `wasc-0.3.0/src/wasc/default_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,43 +10,37 @@
 
 Classes
 -------
 DFTT01(AbstractChecker) :
     Test the presence of tags <HEAD>
 DFTT02(AbstractChecker) :
     Test the depth of tags <HEAD>
-DFTT05(AbstractChecker) :
-    Test the presence of a compliance rate (%) on the accessibility statement
-LangChecker(AbstractChecker) :
-    Test the presence of the language in the header of the HTML page
-DoctypeChecker(AbstractChecker) :
-    Test the presence of Doctype in the web page
 AccessChecker(AbstractChecker) :
     Test the presence of "Accessibilité" in the page
 AccessLinkChecker(AbstractChecker) :
     Test if a link exist to the accessibility page
-MentionsLegalesChecker(AbstractChecker) :
+AccessRateChecker(AbstractChecker) :
+    Test the presence of a compliance rate (%) on the accessibility statement
+LegalChecker(AbstractChecker) :
     Test the presence of "mention légales" link on the web page
+LangChecker(AbstractChecker) :
+    Test the presence of the language in the header of the HTML page
+DoctypeChecker(AbstractChecker) :
+    Test the presence of Doctype in the web page
 """
 import functools
 import re
 
 import bs4
 import requests
 
 from wasc.abstract_checker import AbstractChecker
-from wasc.utils import check_and_correct_url, find_link
+from wasc.utils import HEADER, check_and_correct_url, find_link
 
 FAIL = "échec"
-
-HEADER = {
-    "user-agent" : "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 \
-        (KHTML, like Gecko) Chrome/74.0.3729.169 Safari/537.36" ,
-    "referer" : "https://www.google.com/"
-    }
 mentions = "non|partiellement|totalement"
 ACCESS_PATTERN = re.compile("Accessibilité[ \xa0]:[ \xa0](" + mentions + ")[ \xa0]conforme", re.IGNORECASE)
 
 class DFTT01(AbstractChecker) :
     """DFTT01
     A class to test the presence of <head> tags.
     This class inherits from the AbstrastChecker.
@@ -124,375 +118,379 @@
         -------
          : list
             The list of depth of head tags
         """
         head_tag = web_page.find_all("head")
         return [len(list(tag.parents)) - 1 for tag in head_tag] if head_tag else []
 
-class DFTT05(AbstractChecker) :
-    """DFTT05
-    A class to represent the test of presence of compliance rate (%) on the accessibility statement
-    web page. This class inherits from the AbstrastChecker class.
+class AccessChecker(AbstractChecker) :
+    """AccessChecker
+    Check the presence of "Accessibilité" mention on the web page.
 
     Attributes
     ----------
     name : str
         The name of the checker
+    description : str
+        Description of the checker
 
     Methods
     -------
     execute(self, web_page, url) :
-        return the result of the checker
+        return the level string or "non conforme"
     """
     def __init__(self) :
         """
-        It constructs all the necessary attributes for the DFTT05 class
+        Sets the name and description of AccessChecker
 
         Parameters
         ----------
         None
         """
-        super().__init__("DFTT05", "Taux d'accessibilité")
+        super().__init__("AccessChecker", "Mention accessibilité")
 
-    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
-        This method performs the test on the beautifulsoup object passed in parameter and determines
-        if there is a compliance rate (%) on the accessibility statement web page or not
+        If there is a mention "Accessibilité", returns the level of accessibility,
+        else "non conforme"
 
         Parameters
         ----------
         web_page : bs4.BeautifulSoup
             The BeautifulSoup object created from url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        dict :
-            The name of the checker is the key and the value is either False if there is no
-            compliance rate (%), or the compliance rate (%)
+        str :
+            The level of accessibility or "non conforme"
         """
-        checker_04 = AccessLinkChecker()
-        access_url = checker_04.execute(web_page, root_url)
-        if not access_url :
-            return False
-        response = requests.get(access_url, headers=HEADER, timeout = 1)
-        if response.status_code == requests.codes.ok :
-            access_page = bs4.BeautifulSoup(response.content, "html.parser")
-        else :
-            msg = f"The status_code is {response.status_code}, check the URL : {access_url}"
-            raise ValueError(msg)
-        for access_string in access_page.stripped_strings :
-            match_string = re.search(r"Résultats des tests.*",access_string, \
-                                     flags = re.IGNORECASE)
-            if not match_string :
-                continue
-            access_tag = access_page.find(string = re.compile("Résultats des tests",\
-                                                                   re.IGNORECASE)).parent
-            iter_limit = 10
-            while iter_limit :
-                for tag in access_tag.next_siblings :
-                    if tag.name :
-                        statement = tag.find(string = re.compile("%"))
-                        if statement :
-                            statement_str = str(statement)
-                            try:
-                                index = statement_str.index("%")
-                                counter = 0
-                                for j in range(index-1, index-10, -1) :
-                                    if statement_str[j] in "0123456789 ,." :
-                                        counter += 1
-                                    else :
-                                        break
-                                compliance_tmp = statement_str[index - counter:index + 1].split(" ")
-                                compliance = functools.reduce(lambda x, y : x + y, compliance_tmp)
-                                return compliance
-                            except ValueError:
-                                continue
-                access_tag = access_tag.parent
-                iter_limit -= 1
-        return False
+        mention = web_page.find_all(string = ACCESS_PATTERN)
+        if mention :
+            return mention[0].split(":")[1].strip()
+        return FAIL
 
-class LangChecker(AbstractChecker) :
-    """LangChecker
-    Check the presence of attribute lang in the html tag of the website
+class AccessLinkChecker(AbstractChecker) :
+    """AccessLinkChecker
+    Check that "Accessibilité" present on the web page is a link.
 
     Attributes
     ----------
     name : str
         The name of the checker
     description : str
         Description of the checker
 
     Methods
     -------
     execute(self, web_page, url) :
-        return the lang string or "non conforme"
+        return the link URL
     """
     def __init__(self) :
         """
-        Sets the name and description of LangChecker
+        It constructs all the necessary attributes for the AccessLinkChecker class
 
         Parameters
         ----------
         None
         """
-        super().__init__("LangChecker", "Lang")
+        super().__init__("AccessLinkChecker", "Lien accessibilité")
 
-    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
         """
-        If the language is specified in the html tag, returns a string
-        corresponding to the language of the web page, else "non conforme"
+        Search for a link to the accessibility page, either :
+        * if the mention "Accessibilité" is a link
+        * if there exists a link to root_url/accessibilite
 
         Parameters
         ----------
         web_page : bs4.BeautifulSoup
-            The BeautifulSoup object created url
+            The BeautifulSoup object created from url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        str :
-            the string of language or "non conforme"
+        dict :
+            The name of the checker is the key and the value is either False if the mention
+            "Accessibilité" / "Accessibility" is not a link, or it returns the URL of the link (str)
         """
-        try :
-            return web_page.html.attrs["lang"]
-        except KeyError :
-            return FAIL
+        # 1- Check the link in the mention
+        access_tag = web_page.find(string = ACCESS_PATTERN)
+        if access_tag :
+            link = find_link(access_tag, root_url)
+            if link :
+                return link
+        # 2 - Find text "Déclaration d'accessibilité" and check if it's a link
+        access_tag = web_page.find(string = "Déclaration d'accessibilité")
+        if access_tag :
+            link = find_link(access_tag, root_url)
+            if link :
+                return link
+        # 3 - Check if there exists a link to a standard adresse root_url/accessibilite
+        standard_link = check_and_correct_url("accessibilite", root_url)
+        link_tags = web_page.find_all("a")
+        for tag in link_tags:
+            try :
+                if check_and_correct_url(tag.attrs["href"], root_url) == standard_link:
+                    return standard_link
+            except KeyError :
+                pass
+        return FAIL
 
-class DoctypeChecker(AbstractChecker) :
-    """DoctypeChecker
-    Check the presence of DOCTYPE at the beginning of HTML document
-    (before <html>) + the type is html
+class AccessRateChecker(AbstractChecker) :
+    """AccessRateChecker
+    A class to represent the test of presence of compliance rate (%) on the accessibility statement
+    web page. This class inherits from the AbstrastChecker class.
 
     Attributes
     ----------
     name : str
         The name of the checker
     description : str
         Description of the checker
 
     Methods
     -------
     execute(self, web_page, url) :
-        return "html" or "non conforme"
+        return the result of the checker
     """
     def __init__(self) :
         """
-        Sets the name and description of DoctypeChecker
+        It constructs all the necessary attributes for the AccessRateChecker class
 
         Parameters
         ----------
         None
         """
-        super().__init__("DoctypeChecker", "Doctype")
+        super().__init__("AccessRateChecker", "Taux d'accessibilité")
 
-    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
         """
-        Check the presence of doctype in html document
+        This method performs the test on the beautifulsoup object passed in parameter and determines
+        if there is a compliance rate (%) on the accessibility statement web page or not
 
         Parameters
         ----------
         web_page : bs4.BeautifulSoup
-            The BeautifulSoup object created url
+            The BeautifulSoup object created from url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        bool :
-            True if Doctype is present, before <html> and has "html" value
+        dict :
+            The name of the checker is the key and the value is either False if there is no
+            compliance rate (%), or the compliance rate (%)
         """
-        current_pos = 0
-        doctype_pos = 1
-        html_pos = 0
-        doctype_found = False
-        for item in web_page.contents:
-            if isinstance(item, bs4.Doctype):
-                doctype_pos = current_pos
-                doctype_found = True
-                if item != "html":
-                    return FAIL
-            elif isinstance(item, bs4.Tag) and item.name == "html":
-                html_pos = current_pos
-            current_pos += 1
-        if doctype_found and doctype_pos < html_pos:
-            return "html"
-        return FAIL
+        checker_04 = AccessLinkChecker()
+        access_url = checker_04.execute(web_page, root_url)
+        if not access_url :
+            return False
+        response = requests.get(access_url, headers=HEADER, timeout = 1)
+        if response.status_code == requests.codes.ok :
+            access_page = bs4.BeautifulSoup(response.content, "html.parser")
+        else :
+            msg = f"The status_code is {response.status_code}, check the URL : {access_url}"
+            raise ValueError(msg)
+        for access_string in access_page.stripped_strings :
+            match_string = re.search(r"Résultats des tests.*",access_string, \
+                                     flags = re.IGNORECASE)
+            if not match_string :
+                continue
+            if isinstance(access_page, bs4.NavigableString):
+                access_tag = access_page.find(string = re.compile("Résultats des tests",\
+                                                                   re.IGNORECASE)).parent
+            iter_limit = 10
+            while iter_limit and isinstance(access_tag, bs4.Tag) :
+                for tag in access_tag.next_siblings :
+                    if isinstance(tag, bs4.Tag) and tag.name :
+                        statement = tag.find(string = re.compile("%"))
+                        if statement :
+                            statement_str = str(statement)
+                            try:
+                                index = statement_str.index("%")
+                                counter = 0
+                                for j in range(index-1, index-10, -1) :
+                                    if statement_str[j] in "0123456789 ,." :
+                                        counter += 1
+                                    else :
+                                        break
+                                compliance_tmp = statement_str[index - counter:index + 1].split(" ")
+                                compliance = functools.reduce(lambda x, y : x + y, compliance_tmp)
+                                return compliance
+                            except ValueError:
+                                continue
+                access_tag = access_tag.parent
+                iter_limit -= 1
+        return False
 
-class AccessChecker(AbstractChecker) :
-    """AccessChecker
-    Check the presence of "Accessibilité" mention on the web page.
+class LegalChecker(AbstractChecker) :
+    """LegalChecker
+    Test the presence of "Mentions légales" link on the web page.
 
     Attributes
     ----------
     name : str
         The name of the checker
     description : str
         Description of the checker
 
     Methods
     -------
     execute(self, web_page, url) :
-        return the level string or "non conforme"
+        return the link to the page or fail
     """
     def __init__(self) :
         """
-        Sets the name and description of AccessChecker
+        It constructs all the necessary attributes for the LegalChecker class
 
         Parameters
         ----------
         None
         """
-        super().__init__("AccessChecker", "Mention accessibilité")
+        super().__init__("LegalChecker", "Mentions légales")
 
-    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
         """
-        If there is a mention "Accessibilité", returns the level of accessibility,
-        else "non conforme"
+        Try to find :
+        * text "Mentions légales" (case insensitive) and check if a link exists
+        * try the url root_url + "/mentions-legales" and check if a link exists
+        Return the link to "Mentions légales" page if it exists, else fail
 
         Parameters
         ----------
         web_page : bs4.BeautifulSoup
             The BeautifulSoup object created from url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
         str :
-            The level of accessibility or "non conforme"
+            The link to "Mentions légales" page if it exists, else fail
         """
-        mention = web_page.find_all(string = ACCESS_PATTERN)
-        if mention :
-            return mention[0].split(":")[1].strip()
+        motif = re.compile("Mentions* l[eé]gales*", re.IGNORECASE)
+        legal_tags = web_page.find_all(string = motif)
+        for tag in legal_tags:
+            legal_tag = tag
+            while legal_tag and legal_tag.name != "a" and legal_tag.name != "html":
+                legal_tag = legal_tag.parent
+            try :
+                return check_and_correct_url(legal_tag.attrs["href"], root_url)
+            except KeyError :
+                pass
+        legal_link = check_and_correct_url("mentions-legales", root_url)
+        response = requests.get(legal_link, headers=HEADER, timeout = 1)
+        if response.status_code == requests.codes.ok :
+            return legal_link
         return FAIL
 
-class AccessLinkChecker(AbstractChecker) :
-    """AccessLinkChecker
-    Check that "Accessibilité" present on the web page is a link.
+class LangChecker(AbstractChecker) :
+    """LangChecker
+    Check the presence of attribute lang in the html tag of the website
 
     Attributes
     ----------
     name : str
         The name of the checker
     description : str
         Description of the checker
 
     Methods
     -------
     execute(self, web_page, url) :
-        return the link URL
+        return the lang string or "non conforme"
     """
     def __init__(self) :
         """
-        It constructs all the necessary attributes for the AccessLinkChecker class
+        Sets the name and description of LangChecker
 
         Parameters
         ----------
         None
         """
-        super().__init__("AccessLinkChecker", "Lien accessibilité")
+        super().__init__("LangChecker", "Lang")
 
-    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
-        Search for a link to the accessibility page, either :
-        * if the mention "Accessibilité" is a link
-        * if there exists a link to root_url/accessibilite
+        If the language is specified in the html tag, returns a string
+        corresponding to the language of the web page, else "non conforme"
 
         Parameters
         ----------
         web_page : bs4.BeautifulSoup
-            The BeautifulSoup object created from url
+            The BeautifulSoup object created url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        dict :
-            The name of the checker is the key and the value is either False if the mention
-            "Accessibilité" / "Accessibility" is not a link, or it returns the URL of the link (str)
+        str :
+            the string of language or "non conforme"
         """
-        # 1- Check the link in the mention
-        access_tag = web_page.find(string = ACCESS_PATTERN)
-        if access_tag :
-            link = find_link(access_tag, root_url)
-            if link :
-                return link
-        # 2 - Find text "Déclaration d'accessibilité" and check if it's a link
-        access_tag = web_page.find(string = "Déclaration d'accessibilité")
-        if access_tag :
-            link = find_link(access_tag, root_url)
-            if link :
-                return link
-        # 3 - Check if there exists a link to a standard adresse root_url/accessibilite
-        standard_link = check_and_correct_url("accessibilite", root_url)
-        link_tags = web_page.find_all("a")
-        for tag in link_tags:
-            try :
-                if check_and_correct_url(tag.attrs["href"], root_url) == standard_link:
-                    return standard_link
-            except KeyError :
-                pass
-        return FAIL
+        try :
+            if isinstance(web_page.html, bs4.Tag):
+                return web_page.html.attrs["lang"]
+        except KeyError :
+            return FAIL
 
-class MentionsLegalesChecker(AbstractChecker) :
-    """MentionsLegalesChecker
-    Test the presence of "Mentions légales" link on the web page.
+class DoctypeChecker(AbstractChecker) :
+    """DoctypeChecker
+    Check the presence of DOCTYPE at the beginning of HTML document
+    (before <html>) + the type is html
 
     Attributes
     ----------
     name : str
         The name of the checker
     description : str
         Description of the checker
 
     Methods
     -------
     execute(self, web_page, url) :
-        return the link to the page or fail
+        return "html" or "non conforme"
     """
     def __init__(self) :
         """
-        It constructs all the necessary attributes for the MentionsLegalesChecker class
+        Sets the name and description of DoctypeChecker
 
         Parameters
         ----------
         None
         """
-        super().__init__("MentionsLegalesChecker", "Mentions légales")
+        super().__init__("DoctypeChecker", "Doctype")
 
-    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):
+    def execute(self, web_page : bs4.BeautifulSoup, root_url : str):  # noqa: ARG002
         """
-        Try to find :
-        * text "Mentions légales" (case insensitive) and check if a link exists
-        * try the url root_url + "/mentions-legales" and check if a link exists
-        Return the link to "Mentions légales" page if it exists, else fail
+        Check the presence of doctype in html document
 
         Parameters
         ----------
         web_page : bs4.BeautifulSoup
-            The BeautifulSoup object created from url
+            The BeautifulSoup object created url
         root_url : str
             The root URL of the analyzed web page
 
         Returns
         -------
-        str :
-            The link to "Mentions légales" page if it exists, else fail
+        bool :
+            True if Doctype is present, before <html> and has "html" value
         """
-        motif = re.compile("Mentions* l[eé]gales*", re.IGNORECASE)
-        legal_tags = web_page.find_all(string = motif)
-        for tag in legal_tags:
-            legal_tag = tag
-            while legal_tag and legal_tag.name != "a" and legal_tag.name != "html":
-                legal_tag = legal_tag.parent
-            try :
-                return check_and_correct_url(legal_tag.attrs["href"], root_url)
-            except KeyError :
-                pass
-        legal_link = check_and_correct_url("mentions-legales", root_url)
-        response = requests.get(legal_link, headers=HEADER, timeout = 1)
-        if response.status_code == requests.codes.ok :
-            return legal_link
+        current_pos = 0
+        doctype_pos = 1
+        html_pos = 0
+        doctype_found = False
+        for item in web_page.contents:
+            if isinstance(item, bs4.Doctype):
+                doctype_pos = current_pos
+                doctype_found = True
+                if item != "html":
+                    return FAIL
+            elif isinstance(item, bs4.Tag) and item.name == "html":
+                html_pos = current_pos
+            current_pos += 1
+        if doctype_found and doctype_pos < html_pos:
+            return "html"
         return FAIL
```

### Comparing `wasc-0.2.0/src/wasc/utils.py` & `wasc-0.3.0/src/wasc/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # SPDX-FileCopyrightText: 2023-present Guillaume Collet <bilouweb@free.fr>
 #
 # SPDX-License-Identifier: CECILL-2.1
 """
 This module provides some reading functions
 """
 import pandas as pd
-import yaml
 
+HEADER = {
+    "user-agent" : "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 \
+        (KHTML, like Gecko) Chrome/74.0.3729.169 Safari/537.36" ,
+    "referer" : "https://www.google.com/"
+    }
 
-def read_criteria_config(filename) :
+def read_checkers(filename) :
     """
-    Reads the list of criteria.
-    Each criterion is associated with a list of checkers
-    The file must be in YAML format.
+    Reads the list of checkers.
 
     Parameters
     ----------
     filename : str
-        File name containing list of criteria
+        File name containing list of checkers
 
     Returns
     -------
-    config_data : dict
-        A dictionary of criteria associated with the list of checkers
+    : list
+        A list of checker names
     """
     with open(filename, encoding = "utf-8") as config_file :
-        return yaml.safe_load(config_file)
+        return [line.strip() for line in config_file]
 
 def read_websites(filename) :
     """
     Reads the websites list, each website is a couple (label, URL)
 
     Parameters
     ----------
@@ -83,17 +85,10 @@
     while access_tag and access_tag.name != "a" and access_tag.name != "html":
         access_tag = access_tag.parent
     try :
         return check_and_correct_url(access_tag.attrs["href"], root_url)
     except KeyError :
         pass
 
-def dict_to_csv(indict):
-    res = {"Organisation" : []}
-    for org, subdict in indict.items():
-        res["Organisation"].append(org)
-        for checkdict in subdict.values():
-            for key, val in checkdict.items():
-                if key not in res:
-                    res[key] = []
-                res[key].append(val)
+def report_to_csv(reports, checkers_list):
+    res = []
     return res
```

### Comparing `wasc-0.2.0/tests/test_checker.py` & `wasc-0.3.0/tests/test_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,39 +121,39 @@
 
     def test_access_link_checker_fail_href(self):
         test_html = DEFAULT_HTML_HEAD + "<a>Accessibilité</a>" + DEFAULT_HTML_TAIL
         access_link_checker = dft.AccessLinkChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert access_link_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
-class TestMentionsLegalesChecker:
+class TestLegalChecker:
     def test_mention_legales_checker_init(self):
-        mention_legales_checker = dft.MentionsLegalesChecker()
-        assert mention_legales_checker.name == "MentionsLegalesChecker"
+        mention_legales_checker = dft.LegalChecker()
+        assert mention_legales_checker.name == "LegalChecker"
         assert mention_legales_checker.description == "Mentions légales"
 
     def test_mention_legales_valid_mention1(self):
         test_html = DEFAULT_HTML_HEAD + '<a href="/misc/mentions-legales/">Mentions légales</a>' + DEFAULT_HTML_TAIL
-        mention_legales_checker = dft.MentionsLegalesChecker()
+        mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = DEFAULT_HTML_ROOT + "/misc/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_mention_legales_valid_mention2(self):
         test_html = DEFAULT_HTML_HEAD + '<a href="/misc/mentions-legales/">mention legale</a>' + DEFAULT_HTML_TAIL
-        mention_legales_checker = dft.MentionsLegalesChecker()
+        mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = DEFAULT_HTML_ROOT + "/misc/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == answer
 
     def test_mention_legales_fail_mention(self):
         test_html = DEFAULT_HTML_HEAD + "Mentions légales" + DEFAULT_HTML_TAIL
-        mention_legales_checker = dft.MentionsLegalesChecker()
+        mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         assert mention_legales_checker.execute(basic_webpage, DEFAULT_HTML_ROOT) == FAIL
 
     def test_mention_legales_valid_dftlink(self):
         test_html = DEFAULT_HTML_HEAD + "foo" + DEFAULT_HTML_TAIL
-        mention_legales_checker = dft.MentionsLegalesChecker()
+        mention_legales_checker = dft.LegalChecker()
         basic_webpage = BeautifulSoup(test_html, BS_PARSER)
         answer = "https://www.gouvernement.fr/mentions-legales"
         assert mention_legales_checker.execute(basic_webpage, "https://www.gouvernement.fr/") == answer
```

### Comparing `wasc-0.2.0/tests/test_utils.py` & `wasc-0.3.0/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 import pytest
 
 from wasc import utils
 
 
-class TestReadCriteria:
+class TestReadCheckers:
     def test_no_file(self):
         with pytest.raises(FileNotFoundError):
-            utils.read_criteria_config("foo.txt")
-    def test_not_yaml(self):
-        utils.read_criteria_config("tests/data/url_example.csv")
+            utils.read_checkers("foo.txt")
     def test_read_crit_example(self):
-        expected_criteria = {
-            "Balise head" : ["DFTT01", "DFTT02"],
-            "Mention Accessibilité" : ["DFTT03", "DFTT04", "DFTT05"],
-            "Mention légale" : ["DFTT06"],
-            "Langage" : ["DFTT07"]
+        expected_checkers = {
+            "DFTT01", "DFTT02",
+            "AccessChecker", "AccessLinkChecker", "AccessRateChecker",
+            "LegalChecker", "LangChecker", "DoctypeChecker"
         }
-        crit_example = utils.read_criteria_config("tests/data/crit_example.yml")
-        assert isinstance(crit_example, dict)
-        for key, value in crit_example.items():
-            assert key in expected_criteria.keys()
-            assert value in expected_criteria.values()
+        read_checkers = utils.read_checkers("tests/data/checkers_example.csv")
+        assert isinstance(read_checkers, list)
+        assert set(read_checkers) == expected_checkers
 
 class TestReadWebsites:
     def test_no_file(self):
         with pytest.raises(FileNotFoundError):
-            utils.read_criteria_config("foo.txt")
+            utils.read_websites("foo.txt")
     def test_read_url_example(self):
         expected_url = [
             ("Design Gouv", "https://design.numerique.gouv.fr/"),
             ("Example", "http://example.com")
         ]
         url_example = utils.read_websites("tests/data/url_example.csv")
         assert isinstance(url_example, list)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wasc-0.2.0/LICENSE.txt` & `wasc-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wasc-0.2.0/pyproject.toml` & `wasc-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wasc"
 dynamic = ["version"]
-description = 'wasc, for Web Accessibility Simple Checker, helps to evaluate accessibility criteria on a list of websites'
+description = 'Web Accessibility Simple Checker'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "CECILL-2.1"
 keywords = ["Web", "Accessibility", "Criteria", "Checker"]
 authors = [
   { name = "Guillaume Collet", email = "bilouweb@free.fr" },
   { name = "Juliette Francis", email = "juliette.francis@etudiant.univ-rennes.fr" },
@@ -25,15 +25,14 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
   "click",
-  "pyyaml",
   "beautifulsoup4",
   "requests",
   "tqdm",
   "pandas"
 ]
 
 [project.urls]
@@ -57,26 +56,25 @@
 WASC_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.build.env-vars]
 WACS_CRITERIA_DEFAULT_PATH = "./data/default_criteria.yml"
 
 [tool.hatch.envs.default.scripts]
 test = "pytest -v {args:tests}"
-all_test = "pytest tests/__init__.py"
 test-cov = "coverage run -m pytest {args:tests}"
 lcov = "coverage lcov"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
-all_cov = [
+test_all = [
   "test-cov tests/__init__.py",
   "cov-report",
   "lcov",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
```

