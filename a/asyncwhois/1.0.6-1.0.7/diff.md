# Comparing `tmp/asyncwhois-1.0.6.tar.gz` & `tmp/asyncwhois-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/josepho/Desktop/workspace-py/asyncwhois/dist/.tmp-7_y4nv7r/asyncwhois-1.0.6.tar", last modified: Fri Jun  2 17:46:45 2023, max compression
+gzip compressed data, was "/Users/josepho/Desktop/workspace-py/asyncwhois/dist/.tmp-9lgzjyyv/asyncwhois-1.0.7.tar", last modified: Wed Jul  5 20:52:26 2023, max compression
```

## Comparing `asyncwhois-1.0.6.tar` & `asyncwhois-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/
--rw-r--r--   0 josepho    (502) staff       (20)     1088 2022-01-20 03:14:56.000000 asyncwhois-1.0.6/LICENSE
--rw-r--r--   0 josepho    (502) staff       (20)       68 2022-01-20 03:14:56.000000 asyncwhois-1.0.6/MANIFEST.in
--rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/PKG-INFO
--rw-r--r--   0 josepho    (502) staff       (20)     6649 2023-03-01 02:03:52.000000 asyncwhois-1.0.6/README.md
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois/
--rw-r--r--   0 josepho    (502) staff       (20)     9039 2023-06-02 17:46:32.000000 asyncwhois-1.0.6/asyncwhois/__init__.py
--rw-r--r--   0 josepho    (502) staff       (20)      166 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/asyncwhois/errors.py
--rw-r--r--   0 josepho    (502) staff       (20)    10440 2023-04-05 14:03:21.000000 asyncwhois-1.0.6/asyncwhois/parse.py
--rw-r--r--   0 josepho    (502) staff       (20)    14205 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/asyncwhois/parse_rir.py
--rw-r--r--   0 josepho    (502) staff       (20)    66855 2023-04-05 14:03:21.000000 asyncwhois-1.0.6/asyncwhois/parse_tld.py
--rw-r--r--   0 josepho    (502) staff       (20)    11885 2023-03-01 02:03:52.000000 asyncwhois-1.0.6/asyncwhois/pywhois.py
--rw-r--r--   0 josepho    (502) staff       (20)     9906 2023-06-02 17:46:32.000000 asyncwhois-1.0.6/asyncwhois/query.py
--rw-r--r--   0 josepho    (502) staff       (20)    72921 2023-03-01 02:03:52.000000 asyncwhois-1.0.6/asyncwhois/servers.py
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/
--rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/PKG-INFO
--rw-r--r--   0 josepho    (502) staff       (20)      561 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/SOURCES.txt
--rw-r--r--   0 josepho    (502) staff       (20)        1 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/dependency_links.txt
--rw-r--r--   0 josepho    (502) staff       (20)       61 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/requires.txt
--rw-r--r--   0 josepho    (502) staff       (20)       11 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/top_level.txt
--rw-r--r--   0 josepho    (502) staff       (20)      239 2022-01-20 03:14:56.000000 asyncwhois-1.0.6/pyproject.toml
--rw-r--r--   0 josepho    (502) staff       (20)     1017 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/setup.cfg
--rw-r--r--   0 josepho    (502) staff       (20)     1787 2023-03-03 02:48:10.000000 asyncwhois-1.0.6/setup.py
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/tests/
--rw-r--r--   0 josepho    (502) staff       (20)      609 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/tests/test_not_found.py
--rw-r--r--   0 josepho    (502) staff       (20)     2610 2023-02-28 22:25:51.000000 asyncwhois-1.0.6/tests/test_package_methods.py
--rw-r--r--   0 josepho    (502) staff       (20)     1668 2022-04-26 19:29:46.000000 asyncwhois-1.0.6/tests/test_parser_methods.py
--rw-r--r--   0 josepho    (502) staff       (20)    60537 2023-04-05 14:03:21.000000 asyncwhois-1.0.6/tests/test_parser_output.py
--rw-r--r--   0 josepho    (502) staff       (20)     1261 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/tests/test_pywhois.py
--rw-r--r--   0 josepho    (502) staff       (20)     1309 2022-04-26 20:37:44.000000 asyncwhois-1.0.6/tests/test_query.py
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/
+-rw-r--r--   0 josepho    (502) staff       (20)     1088 2022-01-20 03:14:56.000000 asyncwhois-1.0.7/LICENSE
+-rw-r--r--   0 josepho    (502) staff       (20)       68 2022-01-20 03:14:56.000000 asyncwhois-1.0.7/MANIFEST.in
+-rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/PKG-INFO
+-rw-r--r--   0 josepho    (502) staff       (20)     6649 2023-03-01 02:03:52.000000 asyncwhois-1.0.7/README.md
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois/
+-rw-r--r--   0 josepho    (502) staff       (20)     9039 2023-07-05 20:51:37.000000 asyncwhois-1.0.7/asyncwhois/__init__.py
+-rw-r--r--   0 josepho    (502) staff       (20)      166 2023-02-20 17:06:00.000000 asyncwhois-1.0.7/asyncwhois/errors.py
+-rw-r--r--   0 josepho    (502) staff       (20)    10580 2023-07-05 20:51:37.000000 asyncwhois-1.0.7/asyncwhois/parse.py
+-rw-r--r--   0 josepho    (502) staff       (20)    14205 2023-02-20 17:06:00.000000 asyncwhois-1.0.7/asyncwhois/parse_rir.py
+-rw-r--r--   0 josepho    (502) staff       (20)    67228 2023-07-05 20:51:37.000000 asyncwhois-1.0.7/asyncwhois/parse_tld.py
+-rw-r--r--   0 josepho    (502) staff       (20)    12576 2023-07-05 20:51:37.000000 asyncwhois-1.0.7/asyncwhois/pywhois.py
+-rw-r--r--   0 josepho    (502) staff       (20)     9906 2023-06-02 17:46:32.000000 asyncwhois-1.0.7/asyncwhois/query.py
+-rw-r--r--   0 josepho    (502) staff       (20)    72921 2023-03-01 02:03:52.000000 asyncwhois-1.0.7/asyncwhois/servers.py
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois.egg-info/
+-rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois.egg-info/PKG-INFO
+-rw-r--r--   0 josepho    (502) staff       (20)      561 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois.egg-info/SOURCES.txt
+-rw-r--r--   0 josepho    (502) staff       (20)        1 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois.egg-info/dependency_links.txt
+-rw-r--r--   0 josepho    (502) staff       (20)       61 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois.egg-info/requires.txt
+-rw-r--r--   0 josepho    (502) staff       (20)       11 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/asyncwhois.egg-info/top_level.txt
+-rw-r--r--   0 josepho    (502) staff       (20)      239 2022-01-20 03:14:56.000000 asyncwhois-1.0.7/pyproject.toml
+-rw-r--r--   0 josepho    (502) staff       (20)     1017 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/setup.cfg
+-rw-r--r--   0 josepho    (502) staff       (20)     1787 2023-03-03 02:48:10.000000 asyncwhois-1.0.7/setup.py
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-07-05 20:52:26.000000 asyncwhois-1.0.7/tests/
+-rw-r--r--   0 josepho    (502) staff       (20)      609 2023-02-20 17:06:00.000000 asyncwhois-1.0.7/tests/test_not_found.py
+-rw-r--r--   0 josepho    (502) staff       (20)     2610 2023-02-28 22:25:51.000000 asyncwhois-1.0.7/tests/test_package_methods.py
+-rw-r--r--   0 josepho    (502) staff       (20)     1668 2022-04-26 19:29:46.000000 asyncwhois-1.0.7/tests/test_parser_methods.py
+-rw-r--r--   0 josepho    (502) staff       (20)    61009 2023-07-05 20:51:37.000000 asyncwhois-1.0.7/tests/test_parser_output.py
+-rw-r--r--   0 josepho    (502) staff       (20)     1261 2023-02-20 17:06:00.000000 asyncwhois-1.0.7/tests/test_pywhois.py
+-rw-r--r--   0 josepho    (502) staff       (20)     1309 2022-04-26 20:37:44.000000 asyncwhois-1.0.7/tests/test_query.py
```

### Comparing `asyncwhois-1.0.6/LICENSE` & `asyncwhois-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/PKG-INFO` & `asyncwhois-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.0.6
+Version: 1.0.7
 Summary: asyncio-friendly Python module for WHOIS and RDAP queries.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.0.6/README.md` & `asyncwhois-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/asyncwhois/__init__.py` & `asyncwhois-1.0.7/asyncwhois/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "rdap_ipv4",
     "rdap_ipv6",
     "rdap_asn",
     "whois_domain",
     "whois_ipv4",
     "whois_ipv6",
 ]
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 
 def whois_domain(
     domain: str,
     authoritative_only: bool = False,
     proxy_url: str = None,
     timeout: int = 10,
```

### Comparing `asyncwhois-1.0.6/asyncwhois/parse.py` & `asyncwhois-1.0.7/asyncwhois/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
     CREATED = "created"
     UPDATED = "updated"
     EXPIRES = "expires"
 
     REGISTRAR = "registrar"
     REGISTRAR_IANA_ID = "registrar_iana_id"
+    REGISTRAR_URL = "registrar_url"
+    REGISTRAR_ABUSE_EMAIL = "registrar_abuse_email"
+    REGISTRAR_ABUSE_PHONE = "registrar_abuse_phone"
 
     REGISTRANT_NAME = "registrant_name"
     REGISTRANT_ORGANIZATION = "registrant_organization"
     REGISTRANT_ADDRESS = "registrant_address"
     REGISTRANT_CITY = "registrant_city"
     REGISTRANT_STATE = "registrant_state"
     REGISTRANT_COUNTRY = "registrant_country"
```

### Comparing `asyncwhois-1.0.6/asyncwhois/parse_rir.py` & `asyncwhois-1.0.7/asyncwhois/parse_rir.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/asyncwhois/parse_tld.py` & `asyncwhois-1.0.7/asyncwhois/parse_tld.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     base_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name: *(.+)",
         TLDBaseKeys.CREATED: r"Creation Date: *(.+)",
         TLDBaseKeys.UPDATED: r"Updated Date: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expir\w+\sDate: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar: *(.+)",
         TLDBaseKeys.REGISTRAR_IANA_ID: r"Registrar IANA ID: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"Registrar URL: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Registrar Abuse Contact Email: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"Registrar Abuse Contact Phone: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Name: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Registrant Organization: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant Street: *(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"Registrant City: *(.+)",
         TLDBaseKeys.REGISTRANT_STATE: r"Registrant State/Province: *(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"Registrant Postal Code: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"Registrant Country: *(.+)",
@@ -112,15 +115,14 @@
             "aw": RegexAW(),
             "ax": RegexAX(),
             "be": RegexBE(),
             "br": RegexBR(),
             "by": RegexBY(),
             "cc": RegexCC(),
             "ch": RegexCH(),
-            "ci": RegexCI(),
             "cl": RegexCL(),
             "cn": RegexCN(),
             "cr": RegexCR(),
             "cz": RegexCZ(),
             "de": RegexDE(),
             "dk": RegexDK(),
             "edu": RegexEDU(),
@@ -189,14 +191,15 @@
     _ru_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.CREATED: r"created: *(.+)",
         TLDBaseKeys.EXPIRES: r"paid-till: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org: *(.+)",
         TLDBaseKeys.STATUS: r"state: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
+        TLDBaseKeys.ADMIN_EMAIL: r"admin-contact: *(.+)"
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._ru_expressions)
 
 
@@ -244,25 +247,27 @@
 class RegexRO(TLDParser):
     # % The ROTLD WHOIS service on port 43 never discloses any information concerning the registrant.
 
     _ro_expressions = {
         TLDBaseKeys.CREATED: r"Registered On: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expires On: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Nameserver: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"Referral URL: *(.+)"
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._ro_expressions)
 
 
 class RegexPE(TLDParser):
     _pe_expressions = {
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant name: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar: *(.+)",
+        TLDBaseKeys.ADMIN_EMAIL: r"Admin Email: *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name server: *(.+)",
         TLDBaseKeys.STATUS: r"Domain Status: *(.+)",
     }
 
     def __init__(self):
         super().__init__()
@@ -272,15 +277,17 @@
 class RegexEE(TLDParser):
     _ee_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *[\n\r]+\s*name: *([^\n\r]+)",
         TLDBaseKeys.STATUS: r"status: *([^\n\r]+)",
         TLDBaseKeys.CREATED: r"registered: *([^\n\r]+)",
         TLDBaseKeys.UPDATED: r"changed: *([^\n\r]+)",
         TLDBaseKeys.EXPIRES: r"expire: *([^\n\r]+)",
-        TLDBaseKeys.REGISTRAR: r"Registrar: *[\n\r]+\s*name: *([^\n\r]+)",
+        TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?name: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?url: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"(?<=Registrar)[\s\S]*?phone: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"country: *(.+)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._ee_expressions)
@@ -289,14 +296,15 @@
 class RegexFR(TLDParser):
     _fr_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.CREATED: r"created: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.UPDATED: r"last-update: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.EXPIRES: r"Expiry Date: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
+        TLDBaseKeys.REGISTRAR: r"registrar: *(.+)"
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._fr_expressions)
 
 
@@ -317,14 +325,16 @@
 
 class RegexKR(TLDParser):
     _kr_expressions = {
         TLDBaseKeys.CREATED: r"Registered Date *: (\d{4}\.\s\d{2}\.\s\d{2}\.)",
         TLDBaseKeys.UPDATED: r"Last Updated Date *: (\d{4}\.\s\d{2}\.\s\d{2}\.)",
         TLDBaseKeys.EXPIRES: r"Expiration Date *: (\d{4}\.\s\d{2}\.\s\d{2}\.)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant *: (.+)",
+        TLDBaseKeys.ADMIN_EMAIL: r"Administrative Contact(AC) *: *(.+)",
+        TLDBaseKeys.ADMIN_NAME: r"AC E-Mail *: *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC *: ([a-zA-Z]+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"Registrant Zip Code: *: (.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant Address *: (.+)",
         TLDBaseKeys.DOMAIN_NAME: r"Domain *: (.+)",
         TLDBaseKeys.NAME_SERVERS: r"Host Name *: (.+)",
     }
 
@@ -336,14 +346,15 @@
 class RegexEU(TLDParser):
     # .EU whois server disclaimer:
     # % The EURid WHOIS service on port 43 (textual whois) never
     # % discloses any information concerning the registrant.
 
     _eu_expressions = {
         TLDBaseKeys.REGISTRAR: r"Registrar:\n.*Name: (.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"Registrar:\n.*Name:.+\n.*Website: *(.+)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._eu_expressions)
 
     def parse(self, blob: str) -> Dict[str, Any]:
@@ -378,14 +389,15 @@
 class RegexUK(TLDParser):
     _uk_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain name:\r\n*(.+)",
         TLDBaseKeys.CREATED: r"Registered on:\s*(\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.UPDATED: r"Last updated:\s*(\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.EXPIRES: r"Expiry date:\s*(\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.REGISTRAR: r"Registrar:\s*(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?URL: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\n *(.+)",
         TLDBaseKeys.STATUS: r"Registration status:\n *(.+)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._uk_expressions)
@@ -460,21 +472,18 @@
         self.update_reg_expressions(self._au_expressions)
 
 
 class RegexAT(TLDParser):
     _at_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
-        TLDBaseKeys.UPDATED: r"changed on: *(.+)",
+        TLDBaseKeys.UPDATED: r"changed: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
-        TLDBaseKeys.REGISTRANT_NAME: r"",
-        TLDBaseKeys.REGISTRANT_ADDRESS: r"",
-        TLDBaseKeys.REGISTRANT_ZIPCODE: r"",
-        TLDBaseKeys.REGISTRANT_CITY: r"",
-        TLDBaseKeys.REGISTRANT_COUNTRY: r"",
+        TLDBaseKeys.REGISTRANT_NAME: r"registrant: *(.+)",
+        TLDBaseKeys.TECH_NAME: r"tech-c: *(.+)",
     }
 
     _contact_fields = {
         "name": r"personname: *(.+)",
         "address": r"street address: *(.+)",
         "city": r"city: *(.+)",
         "country": r"country: *(.+)",
@@ -518,14 +527,15 @@
 
 
 class RegexBE(TLDParser):
     _be_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"Registered: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\n.+Name: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"Registrar:\n.+Name:.+\n.+Website:*(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\n *(.+)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._be_expressions)
 
@@ -595,14 +605,17 @@
 class RegexID(TLDParser):
     _id_expressions = {
         TLDBaseKeys.CREATED: r"Created On:(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Date:(.+)",
         TLDBaseKeys.UPDATED: r"Last Updated On:(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC:(.+)",
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar Organization:(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"Sponsoring Registrar Phone: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Sponsoring Registrar Email: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"Sponsoring Registrar URL: *(.+)",
         TLDBaseKeys.STATUS: r"Status:(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Name:(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant Street1:(.+)",
     }
 
     def __init__(self):
         super().__init__()
@@ -631,15 +644,16 @@
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"(?<! )Created: *(.+)",
         TLDBaseKeys.UPDATED: r"(?<! )Last Update: *(.+)",
         TLDBaseKeys.EXPIRES: r"(?<! )Expire Date: *(.+)",
         TLDBaseKeys.STATUS: r"Status: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant)[\s\S]*?Organization:(.*)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant)[\s\S]*?Address:(.*)",
-        TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?Name:(.*)",
+        TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?Name: *(.*)",
+        TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?Web: *(.*)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._it_expressions)
 
 
@@ -660,14 +674,16 @@
     _sk_expressions = {
         TLDBaseKeys.CREATED: r"(?<=Domain:)[\s\w\W]*?Created: *(.+)",
         TLDBaseKeys.UPDATED: r"(?<=Domain:)[\s\w\W]*?Updated: *(.+)",
         TLDBaseKeys.EXPIRES: r"Valid Until: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Name:\s*(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Street:\s*(.+)",
         TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?Organization:(.*)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"(?<=Registrar)[\s\S]*?Email: *(.*)",
+        TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"(?<=Registrar)[\s\S]*?Phone: *(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=^Contact)[\s\S]*?City:(.*)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"(?<=^Contact)[\s\S]*?Postal Code:(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=^Contact)[\s\S]*?Country Code:(.*)",
     }
 
     def __init__(self):
         super().__init__()
@@ -676,14 +692,15 @@
 
 class RegexMX(TLDParser):
     _mx_expressions = {
         TLDBaseKeys.CREATED: r"Created On: *(.+)",
         TLDBaseKeys.UPDATED: r"Last Updated On: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Date: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\s*(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"URL: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant)[\s\S]*?Name:(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=Registrant)[\s\S]*?City:(.*)",
         TLDBaseKeys.REGISTRANT_STATE: r"(?<=Registrant)[\s\S]*?State:(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=Registrant)[\s\S]*?Country:(.*)",
     }
 
     def __init__(self):
@@ -692,14 +709,15 @@
 
 
 class RegexTW(TLDParser):
     _tw_expressions = {
         TLDBaseKeys.CREATED: r"Record created on (.+) ",
         TLDBaseKeys.EXPIRES: r"Record expires on (.+) ",
         TLDBaseKeys.REGISTRAR: r"Registration Service Provider: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"Registration Service URL: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant:)\s+(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=Registrant:)\s*(?:.*\n){5}\s+(.*),",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant:)\s*(?:.*\n){4}\s+(.*)",
         TLDBaseKeys.REGISTRANT_STATE: r"(?<=Registrant:)\s*(?:.*\n){5}.*, (.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=Registrant:)\s*(?:.*\n){6}\s+(.*)",
     }
 
@@ -885,14 +903,16 @@
 
 class RegexLU(TLDParser):
     _lu_expressions = {
         TLDBaseKeys.CREATED: r"registered: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.STATUS: r"domaintype: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar-name: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"registrar-email: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"registrar-url: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org-name: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"org-address: *(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"org-zipcode:*(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"org-city: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"org-country: *(.+)",
     }
 
@@ -958,14 +978,16 @@
 
 
 class RegexHK(TLDParser):
     _hk_expressions = {
         TLDBaseKeys.STATUS: r"Domain Status: *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar Name: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Registrar Contact Information: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"Registrar Contact Information: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Contact Information:\s*Company English Name.*:(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant Contact Information:)[\s\S]*?Address: (.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"[Registrant Contact Information\w\W]+Country: ([\S\ ]+)",
         # 'registrant_email': r'[Registrant Contact Information\w\W]+Email: ([\S\ ]+)',
         TLDBaseKeys.UPDATED: r"Updated Date: *(.+)",
         TLDBaseKeys.CREATED: r"[Registrant Contact Information\w\W]+Domain Name Commencement Date: (.+)",
         TLDBaseKeys.EXPIRES: r"[Registrant Contact Information\w\W]+Expiry Date: (.+)",
@@ -978,14 +1000,17 @@
 
 
 class RegexUA(TLDParser):
     _ua_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.STATUS: r"status: *(.+)",
         TLDBaseKeys.REGISTRAR: r"(?:Registrar: |(?<=Registrar:)[\s\W\w]*?organization-loc: )(.*)",
+        TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?url: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"(?<=Registrar)[\s\S]*?abuse-phone: *(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"(?<=Registrar)[\s\S]*?abuse-email: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant:)[\s\W\w]*?organization-loc:(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=Registrant:)[\s\W\w]*?country-loc:(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=Registrant:)[\s\W\w]*?(?:address\-loc:\s+.*\n){2}address-loc:\s+(.*)\n",
         TLDBaseKeys.REGISTRANT_STATE: r"(?<=Registrant:)[\s\W\w]*?(?:address\-loc:\s+.*\n){1}address-loc:\s+(.*)\n",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant:)[\s\W\w]*?address-loc:\s+(.*)\n",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"(?<=Registrant:)[\s\W\w]*?postal-code-loc:(.*)",
         TLDBaseKeys.UPDATED: "(?:Updated Date: |modified: )(.+)",
@@ -1047,14 +1072,15 @@
 
 class RegexCN(TLDParser):
     _cn_expressions = {
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar: *(.+)",
         TLDBaseKeys.CREATED: r"Registration Time: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Time: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant: *(.+)",
+        TLDBaseKeys.REGISTRANT_EMAIL: r"Registrant Contact Email: *(.+)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._cn_expressions)
 
 
@@ -1075,14 +1101,15 @@
 
 
 class RegexBY(TLDParser):
     _by_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Person: *(.+)",
+        TLDBaseKeys.REGISTRANT_EMAIL: r"Email: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Org: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"Country: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Address: *(.+)",
     }
 
     def __init__(self):
         super().__init__()
@@ -1133,25 +1160,30 @@
 
 
 class RegexAE(TLDParser):
     _ae_expressions = {
         TLDBaseKeys.STATUS: r"Status: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Contact Name: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Registrant Contact Organisation: *(.+)",
+        TLDBaseKeys.REGISTRANT_EMAIL: r"Registrant Contact Email: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar Name: *(.+)",
+        TLDBaseKeys.TECH_NAME: r"Tech Contact Name: *(.+)",
+        TLDBaseKeys.TECH_EMAIL: r"Tech Contact Email: *(.+)",
+        TLDBaseKeys.TECH_ORGANIZATION: r"Tech Contact Organisation: *(.+)",
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._ae_expressions)
 
 
 class RegexSI(TLDParser):
     _si_expressions = {
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"registrar-url: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nameserver: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"registrant: *(.+)",
         TLDBaseKeys.CREATED: r"created: *(.+)",
         TLDBaseKeys.EXPIRES: r"expire: *(.+)",
         TLDBaseKeys.DOMAIN_NAME: "domain: *(.+)",
         TLDBaseKeys.STATUS: "status: *(.+)",
     }
@@ -1382,15 +1414,18 @@
 
     def parse(self, blob: str) -> Dict[str, Any]:
         # GQ server has the same format as TK
         return RegexTK().parse(blob)
 
 
 class RegexNL(TLDParser):
-    _nl_expressions = {TLDBaseKeys.REGISTRAR: r"Registrar:\n(.+)"}
+    _nl_expressions = {
+        TLDBaseKeys.REGISTRAR: r"Registrar:\n(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Abuse Contact:\n(.+)"
+    }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._nl_expressions)
 
     def parse(self, blob: str) -> Dict[str, Any]:
         parsed_output = super().parse(blob)
@@ -1453,14 +1488,15 @@
         )
         return parsed_output
 
 
 class RegexAW(TLDParser):
     _aw_expressions = {
         TLDBaseKeys.REGISTRAR: r"Registrar:\n*(.+)",
+        TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Abuse Contact:\n*(.+)"
     }
 
     def __init__(self):
         super().__init__()
         self.update_reg_expressions(self._aw_expressions)
 
     def parse(self, blob: str) -> Dict[str, Any]:
@@ -1471,14 +1507,15 @@
         return parsed_output
 
 
 class RegexAX(TLDParser):
     _ax_expressions = {
         TLDBaseKeys.DOMAIN_NAME: r"domain\.+: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar\.+: *(.+)",
+        TLDBaseKeys.REGISTRAR_URL: r"www\.+: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"name\.+: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"country\.+: *(.+)",
         TLDBaseKeys.CREATED: r"created\.+: *(.+)",
         TLDBaseKeys.EXPIRES: r"expires\.+: *(.+)",
         TLDBaseKeys.UPDATED: r"modified\.+: *(.+)",
         TLDBaseKeys.STATUS: r"status\.+: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver\.+: *(.+)",
@@ -1657,52 +1694,7 @@
             output[TLDBaseKeys.CREATED] = self._parse_date_mdY(created)
 
         expires = output.get(TLDBaseKeys.EXPIRES)
         if expires:
             output[TLDBaseKeys.EXPIRES] = self._parse_date_mdY(expires)
 
         return output
-
-
-class RegexCI(TLDParser):
-
-    _ci_expressions = {
-        TLDBaseKeys.REGISTRANT_NAME: r"RegistrantName: *(.+)",
-        TLDBaseKeys.REGISTRANT_ORGANIZATION: r"RegistrantOrganization: *(.+)",
-        TLDBaseKeys.REGISTRANT_ADDRESS: r"RegistrantStreet: *(.+)",
-        TLDBaseKeys.REGISTRANT_CITY: r"RegistrantCity: *(.+)",
-        TLDBaseKeys.REGISTRANT_ZIPCODE: r"RegistrantPostal Code: *(.+)",
-        TLDBaseKeys.REGISTRANT_COUNTRY: r"RegistrantCountry: *(.+)",
-        TLDBaseKeys.REGISTRANT_EMAIL: r"RegistrantEmail: *(.+)",
-        TLDBaseKeys.STATUS: r"Domain status: *(.+)",
-        TLDBaseKeys.ADMIN_NAME: r"AdminName: (.+)",
-        TLDBaseKeys.ADMIN_ORGANIZATION: r"AdminOrganization: (.+)",
-        TLDBaseKeys.ADMIN_CITY: r"AdminCity: (.*)",
-        TLDBaseKeys.ADMIN_ADDRESS: r"AdminStreet: (.*)",
-        TLDBaseKeys.ADMIN_ZIPCODE: r"AdminPostal Code: (.*)",
-        TLDBaseKeys.ADMIN_COUNTRY: r"AdminCountry: (.+)",
-        TLDBaseKeys.ADMIN_PHONE: r"AdminPhone: (.+)",
-        TLDBaseKeys.ADMIN_FAX: r"AdminFax: (.+)",
-        TLDBaseKeys.ADMIN_EMAIL: r"AdminEmail: (.+)",
-        TLDBaseKeys.BILLING_NAME: r"BillingName: (.+)",
-        TLDBaseKeys.BILLING_ORGANIZATION: r"BillingOrganization: (.+)",
-        TLDBaseKeys.BILLING_CITY: r"BillingCity: (.*)",
-        TLDBaseKeys.BILLING_ADDRESS: r"BillingStreet: (.*)",
-        TLDBaseKeys.BILLING_ZIPCODE: r"BillingPostal Code: (.*)",
-        TLDBaseKeys.BILLING_COUNTRY: r"BillingCountry: (.+)",
-        TLDBaseKeys.BILLING_PHONE: r"BillingPhone: (.+)",
-        TLDBaseKeys.BILLING_FAX: r"BillingFax: (.+)",
-        TLDBaseKeys.BILLING_EMAIL: r"BillingEmail: (.+)",
-        TLDBaseKeys.TECH_NAME: r"TechName: (.+)",
-        TLDBaseKeys.TECH_ORGANIZATION: r"TechOrganization: (.+)",
-        TLDBaseKeys.TECH_CITY: r"TechCity: (.*)",
-        TLDBaseKeys.TECH_ADDRESS: r"TechStreet: (.*)",
-        TLDBaseKeys.TECH_ZIPCODE: r"TechPostal Code: (.*)",
-        TLDBaseKeys.TECH_COUNTRY: r"TechCountry: (.+)",
-        TLDBaseKeys.TECH_PHONE: r"TechPhone: (.+)",
-        TLDBaseKeys.TECH_FAX: r"TechFax: (.+)",
-        TLDBaseKeys.TECH_EMAIL: r"TechEmail: (.+)",
-    }
-
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ci_expressions)
```

### Comparing `asyncwhois-1.0.6/asyncwhois/pywhois.py` & `asyncwhois-1.0.7/asyncwhois/pywhois.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,17 +124,21 @@
         )
         _self._query = response.to_dict()
         # date keys are mismatched between projects; change these keys to the asyncwhois set.
         whois_dict = response.to_whois_dict()
         for a_key, b_key in [
             (TLDBaseKeys.EXPIRES, "expires_date"),
             (TLDBaseKeys.UPDATED, "updated_date"),
-            (TLDBaseKeys.CREATED, "created_date"),
+            (TLDBaseKeys.CREATED, "created_date")
         ]:
             whois_dict[a_key] = whois_dict.pop(b_key)
+        # reconcile abuse keys, but don't remove existing key as to not cause issues
+        # with apps currently depending on them. todo: re-standardize keys in next major release
+        whois_dict[TLDBaseKeys.REGISTRAR_ABUSE_EMAIL] = whois_dict["abuse_email"]
+        whois_dict[TLDBaseKeys.REGISTRAR_ABUSE_PHONE] = whois_dict["abuse_phone"]
         _self._parser = whois_dict
         return _self
 
     @classmethod
     async def aio_rdap_domain(cls, domain: str, httpx_client: Any = None):
         """
         Performs an async RDAP query using the `whodap` project.
@@ -157,14 +161,18 @@
         # date keys are mismatched between projects; change these keys to the asyncwhois set.
         for a_key, b_key in [
             (TLDBaseKeys.EXPIRES, "expires_date"),
             (TLDBaseKeys.UPDATED, "updated_date"),
             (TLDBaseKeys.CREATED, "created_date"),
         ]:
             whois_dict[a_key] = whois_dict.pop(b_key)
+        # reconcile abuse keys, but don't remove existing key as to not cause issues
+        # with apps currently depending on them. todo: re-standardize keys in next major release
+        whois_dict[TLDBaseKeys.REGISTRAR_ABUSE_EMAIL] = whois_dict["abuse_email"]
+        whois_dict[TLDBaseKeys.REGISTRAR_ABUSE_PHONE] = whois_dict["abuse_phone"]
         _self._parser = whois_dict
         return _self
 
 
 class NumberLookup(Lookup):
     def __init__(self):
         super().__init__()
```

### Comparing `asyncwhois-1.0.6/asyncwhois/query.py` & `asyncwhois-1.0.7/asyncwhois/query.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/asyncwhois/servers.py` & `asyncwhois-1.0.7/asyncwhois/servers.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/asyncwhois.egg-info/PKG-INFO` & `asyncwhois-1.0.7/asyncwhois.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.0.6
+Version: 1.0.7
 Summary: asyncio-friendly Python module for WHOIS and RDAP queries.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.0.6/asyncwhois.egg-info/SOURCES.txt` & `asyncwhois-1.0.7/asyncwhois.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/setup.cfg` & `asyncwhois-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/setup.py` & `asyncwhois-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/tests/test_not_found.py` & `asyncwhois-1.0.7/tests/test_not_found.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/tests/test_package_methods.py` & `asyncwhois-1.0.7/tests/test_package_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/tests/test_parser_methods.py` & `asyncwhois-1.0.7/tests/test_parser_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/tests/test_parser_output.py` & `asyncwhois-1.0.7/tests/test_parser_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,16 @@
         self.assertEqual(parser.parser_output.get("registrant_state"), "CA")
         self.assertEqual(parser.parser_output.get("registrant_city"), "Mountain View")
         self.assertEqual(parser.parser_output.get("registrant_country"), "US")
         self.assertEqual(parser.parser_output.get("registrant_zipcode"), "94043")
         self.assertEqual(parser.parser_output.get("registrant_address"), "1600 Amphitheatre Parkway")
         # registrar
         self.assertEqual(parser.parser_output.get("registrar"), "MarkMonitor Inc.")
+        self.assertEqual(parser.parser_output.get("registrar_url"), "http://markmonitor.com")
+        self.assertEqual(parser.parser_output.get("registrar_abuse_email"), "abusecomplaints@markmonitor.com")
         # registrant
         self.assertEqual(parser.parser_output.get("registrant_organization"), None)
         self.assertEqual(parser.parser_output.get("registrant_name"), "Google LLC")
         # misc
         self.assertEqual(parser.parser_output.get("dnssec"), None)
         self.assertEqual(len(parser.parser_output.get("name_servers")), 4)
         self.assertEqual(len(parser.parser_output.get("status")), 7)
@@ -518,14 +520,15 @@
         self.assertEqual(expires_date.year, 2021)
         self.assertEqual(created_date.month, 3)
         self.assertEqual(expires_date.month, 3)
         self.assertEqual(created_date.day, 3)
         self.assertEqual(expires_date.day, 4)
         # registrant
         self.assertEqual(parser.parser_output.get("registrant_organization"), "Google LLC")
+        self.assertEqual(parser.parser_output.get("admin_email"), "https://www.nic.ru/whois")
 
     def test_parser_edu(self):
         query_output = self.get_txt('edu')
         parser = DomainParser('edu')
         parser.parse(query_output)
         # confirm dates
         created_date = parser.parser_output.get("created")
@@ -987,14 +990,15 @@
         self.assertEqual(updated_date.year, 2015)
         self.assertEqual(created_date.month, 5)
         self.assertEqual(updated_date.month, 12)
         self.assertEqual(created_date.day, 27)
         self.assertEqual(updated_date.day, 30)
         # registrar
         self.assertEqual(parser.parser_output.get("registrar"), "MarkMonitor Inc.")
+        self.assertEqual(parser.parser_output.get("registrar"), "MarkMonitor Inc.")
         self.assertEqual(len(parser.parser_output.get("name_servers")), 4)
         self.assertEqual(len(parser.parser_output.get("status")), 1)
 
     def test_parser_gq(self):
         query_output = self.get_txt('gq')
         parser = DomainParser('gq')
         parser.parse(query_output)
@@ -1184,14 +1188,15 @@
         self.assertEqual(updated_date.day, 5)
         # registrant
         self.assertEqual(parser.parser_output.get("registrant_name"), "xTom GmbH")
         self.assertEqual(parser.parser_output.get("registrant_country"), "Tyskland")
         self.assertEqual(parser.parser_output.get("registrant_address"), "Kreuzstr.60, 40210, Duesseldorf")
         # registrar
         self.assertEqual(parser.parser_output.get("registrar"), "xTom")
+        self.assertEqual(parser.parser_output.get("registrar_url"), "https://xtom.com/")
         # misc
         self.assertEqual(len(parser.parser_output.get("name_servers")), 2)
         self.assertEqual(len(parser.parser_output.get("status")), 1)
         self.assertEqual(parser.parser_output.get("domain_name"), "google.ax")
 
     def test_tld_aw(self):
         query_output = self.get_txt('aw')
```

### Comparing `asyncwhois-1.0.6/tests/test_pywhois.py` & `asyncwhois-1.0.7/tests/test_pywhois.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.6/tests/test_query.py` & `asyncwhois-1.0.7/tests/test_query.py`

 * *Files identical despite different names*

