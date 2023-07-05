# Comparing `tmp/ds_caselaw_utils-1.0.1.tar.gz` & `tmp/ds_caselaw_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_utils-1.0.1.tar", max compression
+gzip compressed data, was "ds_caselaw_utils-1.0.2.tar", max compression
```

## Comparing `ds_caselaw_utils-1.0.1.tar` & `ds_caselaw_utils-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1108 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     4132 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/README.md
--rw-r--r--   0        0        0      617 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/.gitignore
--rw-r--r--   0        0        0       75 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/__init__.py
--rw-r--r--   0        0        0     3062 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/courts.py
--rw-r--r--   0        0        0      709 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/README.md
--rw-r--r--   0        0        0    15200 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/court_names.yaml
--rw-r--r--   0        0        0      615 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/neutral_citation_regex.yaml
--rw-r--r--   0        0        0      656 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/neutral.py
--rw-r--r--   0        0        0     6899 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_courts.py
--rw-r--r--   0        0        0     1395 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_neutral.py
--rw-r--r--   0        0        0     4782 1970-01-01 00:00:00.000000 ds_caselaw_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     4132 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/README.md
+-rw-r--r--   0        0        0      617 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/.gitignore
+-rw-r--r--   0        0        0       75 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/__init__.py
+-rw-r--r--   0        0        0     3112 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/courts.py
+-rw-r--r--   0        0        0      709 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/README.md
+-rw-r--r--   0        0        0    14234 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/court_names.yaml
+-rw-r--r--   0        0        0      628 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/neutral_citation_regex.yaml
+-rw-r--r--   0        0        0     1911 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/schema/courts.schema.json
+-rw-r--r--   0        0        0      656 2023-07-05 10:04:11.711152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/neutral.py
+-rw-r--r--   0        0        0     7081 2023-07-05 10:04:11.715152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/test_courts.py
+-rw-r--r--   0        0        0     1395 2023-07-05 10:04:11.715152 ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/test_neutral.py
+-rw-r--r--   0        0        0     4782 1970-01-01 00:00:00.000000 ds_caselaw_utils-1.0.2/PKG-INFO
```

### Comparing `ds_caselaw_utils-1.0.1/LICENSE.md` & `ds_caselaw_utils-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.1/README.md` & `ds_caselaw_utils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.1/pyproject.toml` & `ds_caselaw_utils-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ds_caselaw_utils"
-version = "1.0.1"
+version = "1.0.2"
 description = "Utilities for the National Archives Caselaw project"
 authors = ["Nick Jackson <nick@dxw.com>", "David McKee <dragon@dxw.com>", "Tim Cowlishaw <tim@timcowlishaw.co.uk>", "Laura Porter <laura@dxw.com>"]
 license = "MIT"
 homepage = "https://github.com/nationalarchives/ds-caselaw-utils"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
```

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/courts.py` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/courts.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         self.link = data.get("link")
         self.ncn = data.get("ncn")
         self.canonical_param = data.get("param")
         self.param_aliases = [data.get("param")] + (data.get("extra_params") or [])
         self.start_year = data.get("start_year")
         self.end_year = data.get("end_year") or date.today().year
 
+    def __repr__(self):
+        return self.name
+
 
 class CourtGroup:
     def __init__(self, name, courts):
         self.name = name
         self.courts = courts
```

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/README.md` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/court_names.yaml` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/court_names.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,459 +1,415 @@
 - name: supreme_court
   display_name: ~
   is_tribunal: false
   courts:
-    -
-        code: UKSC
-        name: United Kingdom Supreme Court
-        link: https://www.supremecourt.uk/
-        ncn: \[(\d{4})\] (UKSC) (\d+)
-        param: 'uksc'
-        start_year: 2014
-        end_year: 2022
-        selectable: true
-        listable: true
+    - code: UKSC
+      name: United Kingdom Supreme Court
+      link: https://www.supremecourt.uk/
+      ncn: \[(\d{4})\] (UKSC) (\d+)
+      param: "uksc"
+      start_year: 2014
+      end_year: 2022
+      selectable: true
+      listable: true
 - name: privy_council
   display_name: ~
   is_tribunal: false
   courts:
-    -
-        code: UKPC
-        name: Privy Council
-        link: https://www.jcpc.uk/
-        ncn: \[(\d{4})\] (UKPC) \d+
-        param: 'ukpc'
-        start_year: 2014
-        end_year: 2022
-        selectable: true
-        listable: true
+    - code: UKPC
+      name: Privy Council
+      link: https://www.jcpc.uk/
+      ncn: \[(\d{4})\] (UKPC) \d+
+      param: "ukpc"
+      start_year: 2014
+      end_year: 2022
+      selectable: true
+      listable: true
 - name: court_of_appeal
   display_name: "Court of Appeal"
   is_tribunal: false
   courts:
-    -
-        code: EWCA-Civil
-        name: Court of Appeal Civil Division
-        list_name: "Court of Appeal (Civil Division)"
-        link: https://www.gov.uk/courts-tribunals/court-of-appeal-civil-division
-        ncn: \[(\d{4})\] (EWCA) (Civ) (\d+)
-        param: 'ewca/civ'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWCA-Criminal
-        name: Court of Appeal Criminal Division
-        list_name: Court of Appeal (Criminal Division)
-        link: https://www.gov.uk/courts-tribunals/court-of-appeal-criminal-division
-        ncn: \[(\d{4})\] (EWCA) (Crim) (\d+)
-        param: 'ewca/crim'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
+    - code: EWCA-Civil
+      name: Court of Appeal Civil Division
+      list_name: "Court of Appeal (Civil Division)"
+      link: https://www.gov.uk/courts-tribunals/court-of-appeal-civil-division
+      ncn: \[(\d{4})\] (EWCA) (Civ) (\d+)
+      param: "ewca/civ"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWCA-Criminal
+      name: Court of Appeal Criminal Division
+      list_name: Court of Appeal (Criminal Division)
+      link: https://www.gov.uk/courts-tribunals/court-of-appeal-criminal-division
+      ncn: \[(\d{4})\] (EWCA) (Crim) (\d+)
+      param: "ewca/crim"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
 - name: high_court
   display_name: "High Court"
   is_tribunal: false
   courts:
-    -
-        code: EWHC-QBD-Admin
-        name: Administrative Court
-        list_name: High Court (Administrative Court)
-        link: https://www.gov.uk/courts-tribunals/administrative-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Admin)\)
-        param: 'ewhc/admin'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-KBD-Admin
-        name: Administrative Court
-        list_name: High Court (Administrative Court)
-        link: https://www.gov.uk/courts-tribunals/administrative-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Admin)\)
-        param: 'ewhc/admin'
-        start_year: 2022
-        end_year: 2022
-        selectable: false
-        listable: false
-    -
-        code: EWHC-QBD-Admiralty
-        name: Admiralty Court
-        list_name: High Court (Admiralty Division)
-        link: https://www.gov.uk/courts-tribunals/admiralty-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Admlty)\)
-        param: 'ewhc/admlty'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-KBD-Admiralty
-        name: Admiralty Court
-        list_name: High Court (Admiralty Division)
-        link: https://www.gov.uk/courts-tribunals/admiralty-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Admlty)\)
-        param: 'ewhc/admlty'
-        start_year: 2022
-        end_year: 2022
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery
-        name: Chancery Division of the High Court
-        list_name: High Court (Chancery Division)
-        link: https://www.gov.uk/courts-tribunals/chancery-division-of-the-high-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Ch)\)
-        param: 'ewhc/ch'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-QBD-Commercial
-        name: Commercial Court
-        list_name: High Court (Commercial Court)
-        link: https://www.gov.uk/courts-tribunals/commercial-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
-        param: 'ewhc/comm'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-KBD-Commercial
-        name: Commercial Court
-        list_name: High Court (Commercial Court)
-        link: https://www.gov.uk/courts-tribunals/commercial-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
-        param: 'ewhc/comm'
-        start_year: 2022
-        end_year: 2022
-        selectable: false
-        listable: false
-    -
-        code: EWHC-SeniorCourtsCosts
-        name: Senior Courts Costs Office
-        list_name: High Court (Senior Court Costs Office)
-        link: https://www.gov.uk/courts-tribunals/senior-courts-costs-office
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((SCCO)\)
-        param: 'ewhc/scco'
-        extra_params: ['ewhc/costs']
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-Family
-        name: Family Division of the High Court
-        list_name: High Court (Family Division)
-        link: https://www.gov.uk/courts-tribunals/family-division-of-the-high-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Fam)\)
-        param: 'ewhc/fam'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-Chancery-IPEC
-        name: Intellectual Property Enterprise Court
-        link: https://www.gov.uk/courts-tribunals/intellectual-property-enterprise-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((IPEC)\)
-        param: 'ewhc/ipec'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-Mercantile
-        name: Mercantile Court
-        list_name: High Court (Mercantile Court)
-        link: https://www.gov.uk/courts-tribunals/intellectual-property-enterprise-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((IPEC)\)
-        param: 'ewhc/mercantile'
-        start_year: 2008
-        end_year: 2014
-        selectable: true
-        listable: true
-    -
-        code: EWHC-Chancery-Patents
-        name: Patents Court
-        list_name: High Court (Patents Court)
-        link: https://www.gov.uk/courts-tribunals/patents-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Pat)\)
-        param: 'ewhc/pat'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-KBD
-        name: King's / Queen's Bench Division of the High Court
-        link: https://www.gov.uk/courts-tribunals/kings-bench-division-of-the-high-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((KB)\)
-        param: "ewhc/kb"
-        extra_params: ["ewhc/qb"]
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: false
-    -
-        code: EWHC-QBD
-        name: High Court (Queen's Bench Division)
-        link: https://www.gov.uk/courts-tribunals/queens-bench-division-of-the-high-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((QB)\)
-        param: 'ewhc/qb'
-        start_year: 2003
-        end_year: 2022
-        selectable: false
-        listable: true
-    -
-        code: EWHC-KBD
-        name: High Court (King's Bench Division)
-        link: https://www.gov.uk/courts-tribunals/kings-bench-division-of-the-high-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((KB)\)
-        param: "ewhc/kb"
-        start_year: 2022
-        end_year: 2022
-        selectable: false
-        listable: true
-    -
-        code: EWHC-QBD-TCC
-        name: Technology and Construction Court
-        list_name: High Court (Technology and Construction Court)
-        link: https://www.gov.uk/courts-tribunals/technology-and-construction-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((TCC)\)
-        param: 'ewhc/tcc'
-        start_year: 2003
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-KBD-TCC
-        name: Technology and Construction Court
-        list_name: High Court (Technology and Construction Court)
-        link: https://www.gov.uk/courts-tribunals/technology-and-construction-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((TCC)\)
-        param: 'ewhc/tcc'
-        start_year: 2022
-        end_year: 2022
-        selectable: false
-        listable: false
-    -
-        code: EWCOP
-        name: Court of Protection
-        link: https://www.gov.uk/courts-tribunals/court-of-protection
-        ncn: \[(\d{4})\] (EWCOP) (\d+)
-        param: 'ewcop'
-        start_year: 2009
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWFC
-        name: Family Court
-        link: https://www.judiciary.uk/you-and-the-judiciary/going-to-court/family-law-courts/
-        ncn: \[(\d{4})\] (EWFC) (\d+)
-        param: 'ewfc'
-        start_year: 2009
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: EWHC-QBD-Planning
-        name: Planning Court
-        link: https://www.gov.uk/courts-tribunals/planning-court
-        selectable: false
-        listable: false
-    -
-        code: EWHC-KBD-Planning
-        name: Planning Court
-        link: https://www.gov.uk/courts-tribunals/planning-court
-        selectable: false
-        listable: false
-    -
-        code: EWHC-QBD-BusinessAndProperty
-        name: The Business and Property Courts
-        link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
-        selectable: false
-        listable: false
-    -
-        code: EWHC-KBD-BusinessAndProperty
-        name: The Business and Property Courts
-        link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
-        selectable: false
-        listable: false
-    -
-        code: EWHC-QBD-Commercial-Financial
-        name: The Financial List
-        link: https://www.gov.uk/courts-tribunals/the-financial-list
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
-        selectable: false
-        listable: false
-    -
-        code: EWHC-KBD-Commercial-Financial
-        name: The Financial List
-        link: https://www.gov.uk/courts-tribunals/the-financial-list
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
-        selectable: false
-        listable: false
-    -
-        code: EWHC-QBD-Commercial-Circuit
-        name: Circuit Commercial Court
-        link: https://www.gov.uk/courts-tribunals/commercial-circuit-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
-        selectable: false
-        listable: false
-    -
-        code: EWHC-KBD-Commercial-Circuit
-        name: Circuit Commercial Court
-        link: https://www.gov.uk/courts-tribunals/commercial-circuit-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-BusinessAndProperty
-        name: The Business and Property Courts
-        link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-Business
-        name: The Business List
-        link: https://www.gov.uk/courts-tribunals/the-business-list
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-InsolvencyAndCompanies
-        name: Insolvency and Companies List
-        link: https://www.gov.uk/courts-tribunals/insolvency-list
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-Financial
-        name: The Financial List
-        link: https://www.gov.uk/courts-tribunals/the-financial-list
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-IntellectualProperty
-        name: The Intellectual Property List
-        link: https://www.gov.uk/courts-tribunals/the-intellectual-property-list
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-Patents
-        name: Patents Court
-        link: https://www.gov.uk/courts-tribunals/patents-court
-        ncn: \[(\d{4})\] (EWHC) (\d+) \((Pat)\)
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-PropertyTrustsProbate
-        name: The Property, Trusts and Probate List
-        link: https://www.gov.uk/courts-tribunals/the-property-trusts-and-probate-list
-        selectable: false
-        listable: false
-    -
-        code: EWHC-Chancery-Appeals
-        name: Chancery Appeals
-        link: https://www.gov.uk/courts-tribunals/chancery-division-of-the-high-court
-        selectable: false
-        listable: false
+    - code: EWHC-QBD-Admin
+      name: Administrative Court
+      list_name: High Court (Administrative Court)
+      link: https://www.gov.uk/courts-tribunals/administrative-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Admin)\)
+      param: "ewhc/admin"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-KBD-Admin
+      name: Administrative Court
+      list_name: High Court (Administrative Court)
+      link: https://www.gov.uk/courts-tribunals/administrative-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Admin)\)
+      param: "ewhc/admin"
+      start_year: 2022
+      end_year: 2022
+      selectable: false
+      listable: false
+    - code: EWHC-QBD-Admiralty
+      name: Admiralty Court
+      list_name: High Court (Admiralty Division)
+      link: https://www.gov.uk/courts-tribunals/admiralty-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Admlty)\)
+      param: "ewhc/admlty"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-KBD-Admiralty
+      name: Admiralty Court
+      list_name: High Court (Admiralty Division)
+      link: https://www.gov.uk/courts-tribunals/admiralty-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Admlty)\)
+      param: "ewhc/admlty"
+      start_year: 2022
+      end_year: 2022
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery
+      name: Chancery Division of the High Court
+      list_name: High Court (Chancery Division)
+      link: https://www.gov.uk/courts-tribunals/chancery-division-of-the-high-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Ch)\)
+      param: "ewhc/ch"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-QBD-Commercial
+      name: Commercial Court
+      list_name: High Court (Commercial Court)
+      link: https://www.gov.uk/courts-tribunals/commercial-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+      param: "ewhc/comm"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-KBD-Commercial
+      name: Commercial Court
+      list_name: High Court (Commercial Court)
+      link: https://www.gov.uk/courts-tribunals/commercial-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+      param: "ewhc/comm"
+      start_year: 2022
+      end_year: 2022
+      selectable: false
+      listable: false
+    - code: EWHC-Family
+      name: Family Division of the High Court
+      list_name: High Court (Family Division)
+      link: https://www.gov.uk/courts-tribunals/family-division-of-the-high-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Fam)\)
+      param: "ewhc/fam"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-KBD
+      name: King's / Queen's Bench Division of the High Court
+      link: https://www.gov.uk/courts-tribunals/kings-bench-division-of-the-high-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((KB)\)
+      param: "ewhc/kb"
+      extra_params: ["ewhc/qb"]
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: false
+    - code: EWHC-Chancery-IPEC
+      name: Intellectual Property Enterprise Court
+      link: https://www.gov.uk/courts-tribunals/intellectual-property-enterprise-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((IPEC)\)
+      param: "ewhc/ipec"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-Mercantile
+      name: Mercantile Court
+      list_name: High Court (Mercantile Court)
+      link: https://www.gov.uk/courts-tribunals/intellectual-property-enterprise-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((IPEC)\)
+      param: "ewhc/mercantile"
+      start_year: 2008
+      end_year: 2014
+      selectable: true
+      listable: true
+    - code: EWHC-Chancery-Patents
+      name: Patents Court
+      list_name: High Court (Patents Court)
+      link: https://www.gov.uk/courts-tribunals/patents-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Pat)\)
+      param: "ewhc/pat"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-QBD
+      name: High Court (Queen's Bench Division)
+      link: https://www.gov.uk/courts-tribunals/queens-bench-division-of-the-high-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((QB)\)
+      param: "ewhc/qb"
+      start_year: 2003
+      end_year: 2022
+      selectable: false
+      listable: true
+    - code: EWHC-KBD
+      name: High Court (King's Bench Division)
+      link: https://www.gov.uk/courts-tribunals/kings-bench-division-of-the-high-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((KB)\)
+      param: "ewhc/kb"
+      start_year: 2022
+      end_year: 2022
+      selectable: false
+      listable: true
+    - code: EWHC-SeniorCourtsCosts
+      name: Senior Courts Costs Office
+      list_name: High Court (Senior Court Costs Office)
+      link: https://www.gov.uk/courts-tribunals/senior-courts-costs-office
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((SCCO)\)
+      param: "ewhc/scco"
+      extra_params: ["ewhc/costs"]
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-QBD-TCC
+      name: Technology and Construction Court
+      list_name: High Court (Technology and Construction Court)
+      link: https://www.gov.uk/courts-tribunals/technology-and-construction-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((TCC)\)
+      param: "ewhc/tcc"
+      start_year: 2003
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWHC-KBD-TCC
+      name: Technology and Construction Court
+      list_name: High Court (Technology and Construction Court)
+      link: https://www.gov.uk/courts-tribunals/technology-and-construction-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((TCC)\)
+      param: "ewhc/tcc"
+      start_year: 2022
+      end_year: 2022
+      selectable: false
+      listable: false
+    - code: EWHC-QBD-Planning
+      name: Planning Court
+      link: https://www.gov.uk/courts-tribunals/planning-court
+      selectable: false
+      listable: false
+    - code: EWHC-KBD-Planning
+      name: Planning Court
+      link: https://www.gov.uk/courts-tribunals/planning-court
+      selectable: false
+      listable: false
+    - code: EWHC-QBD-BusinessAndProperty
+      name: The Business and Property Courts
+      link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
+      selectable: false
+      listable: false
+    - code: EWHC-KBD-BusinessAndProperty
+      name: The Business and Property Courts
+      link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
+      selectable: false
+      listable: false
+    - code: EWHC-QBD-Commercial-Financial
+      name: The Financial List
+      link: https://www.gov.uk/courts-tribunals/the-financial-list
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+      selectable: false
+      listable: false
+    - code: EWHC-KBD-Commercial-Financial
+      name: The Financial List
+      link: https://www.gov.uk/courts-tribunals/the-financial-list
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+      selectable: false
+      listable: false
+    - code: EWHC-QBD-Commercial-Circuit
+      name: Circuit Commercial Court
+      link: https://www.gov.uk/courts-tribunals/commercial-circuit-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+      selectable: false
+      listable: false
+    - code: EWHC-KBD-Commercial-Circuit
+      name: Circuit Commercial Court
+      link: https://www.gov.uk/courts-tribunals/commercial-circuit-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-BusinessAndProperty
+      name: The Business and Property Courts
+      link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-Business
+      name: The Business List
+      link: https://www.gov.uk/courts-tribunals/the-business-list
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-InsolvencyAndCompanies
+      name: Insolvency and Companies List
+      link: https://www.gov.uk/courts-tribunals/insolvency-list
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-Financial
+      name: The Financial List
+      link: https://www.gov.uk/courts-tribunals/the-financial-list
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-IntellectualProperty
+      name: The Intellectual Property List
+      link: https://www.gov.uk/courts-tribunals/the-intellectual-property-list
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-Patents
+      name: Patents Court
+      link: https://www.gov.uk/courts-tribunals/patents-court
+      ncn: \[(\d{4})\] (EWHC) (\d+) \((Pat)\)
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-PropertyTrustsProbate
+      name: The Property, Trusts and Probate List
+      link: https://www.gov.uk/courts-tribunals/the-property-trusts-and-probate-list
+      selectable: false
+      listable: false
+    - code: EWHC-Chancery-Appeals
+      name: Chancery Appeals
+      link: https://www.gov.uk/courts-tribunals/chancery-division-of-the-high-court
+      selectable: false
+      listable: false
+- name: lower_courts
+  display_name: "Lower Courts"
+  is_tribunal: false
+  courts:
+    - code: EWCOP
+      name: Court of Protection
+      link: https://www.gov.uk/courts-tribunals/court-of-protection
+      ncn: \[(\d{4})\] (EWCOP) (\d+)
+      param: "ewcop"
+      start_year: 2009
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: EWFC
+      name: Family Court
+      link: https://www.judiciary.uk/you-and-the-judiciary/going-to-court/family-law-courts/
+      ncn: \[(\d{4})\] (EWFC) (\d+)
+      param: "ewfc"
+      start_year: 2009
+      end_year: 2022
+      selectable: true
+      listable: true
 - name: upper_tribunals
   display_name: "Upper Tribunals"
   is_tribunal: true
   courts:
-    -
-        code: UKUT-IAC
-        name: Upper Tribunal Immigration and Asylum Chamber
-        list_name: Upper Tribunal (Immigration and Asylum Chamber)
-        link: https://www.gov.uk/courts-tribunals/upper-tribunal-immigration-and-asylum-chamber
-        ncn: \[(\d{4})\] (UKUT) (\d+) \((IAC)\)
-        selectable: true
-        listable: true
-        param: 'ukut/iac'
-        start_year: 2010
-        end_year: 2022
-
-    -
-        code: UKUT-LC
-        name: Upper Tribunal Lands Chamber
-        list_name: Upper Tribunal (Lands Chamber)
-        link: https://www.gov.uk/courts-tribunals/upper-tribunal-lands-chamber
-        ncn: \[(\d{4})\] (UKUT) (\d+) \((LC)\)
-        selectable: true
-        listable: true
-        param: 'ukut/lc'
-        start_year: 2015
-        end_year: 2022
-    -
-        code: UKUT-TCC
-        name: Upper Tribunal Tax and Chancery Chamber
-        list_name: Upper Tribunal (Tax and Chancery Chamber)
-        link: https://www.gov.uk/courts-tribunals/upper-tribunal-tax-and-chancery-chamber
-        ncn: \[(\d{4})\] (UKUT) (\d+) \((TCC)\)
-        selectable: true
-        listable: true
-        param: 'ukut/tcc'
-        start_year: 2017
-        end_year: 2022
-    -
-        code: UKUT-AAC
-        name: Upper Tribunal Administrative Appeals Chamber
-        list_name: Upper Tribunal (Administrative Appeals Chamber)
-        link: https://www.gov.uk/courts-tribunals/upper-tribunal-administrative-appeals-chamber
-        ncn: \[(\d{4})\] (UKUT) (\d+) \((AAC)\)
-        selectable: true
-        listable: true
-        param: 'ukut/aac'
-        start_year: 2022
-        end_year: 2022
+    - code: UKUT-AAC
+      name: Upper Tribunal Administrative Appeals Chamber
+      list_name: Upper Tribunal (Administrative Appeals Chamber)
+      link: https://www.gov.uk/courts-tribunals/upper-tribunal-administrative-appeals-chamber
+      ncn: \[(\d{4})\] (UKUT) (\d+) \((AAC)\)
+      selectable: true
+      listable: true
+      param: "ukut/aac"
+      start_year: 2022
+      end_year: 2022
+    - code: UKUT-LC
+      name: Upper Tribunal Lands Chamber
+      list_name: Upper Tribunal (Lands Chamber)
+      link: https://www.gov.uk/courts-tribunals/upper-tribunal-lands-chamber
+      ncn: \[(\d{4})\] (UKUT) (\d+) \((LC)\)
+      selectable: true
+      listable: true
+      param: "ukut/lc"
+      start_year: 2015
+      end_year: 2022
+    - code: UKUT-IAC
+      name: Upper Tribunal Immigration and Asylum Chamber
+      list_name: Upper Tribunal (Immigration and Asylum Chamber)
+      link: https://www.gov.uk/courts-tribunals/upper-tribunal-immigration-and-asylum-chamber
+      ncn: \[(\d{4})\] (UKUT) (\d+) \((IAC)\)
+      selectable: true
+      listable: true
+      param: "ukut/iac"
+      start_year: 2010
+      end_year: 2022
+    - code: UKUT-TCC
+      name: Upper Tribunal Tax and Chancery Chamber
+      list_name: Upper Tribunal (Tax and Chancery Chamber)
+      link: https://www.gov.uk/courts-tribunals/upper-tribunal-tax-and-chancery-chamber
+      ncn: \[(\d{4})\] (UKUT) (\d+) \((TCC)\)
+      selectable: true
+      listable: true
+      param: "ukut/tcc"
+      start_year: 2017
+      end_year: 2022
 - name: employment_appeal_tribunal
   display_name: ~
   is_tribunal: true
   courts:
-    -
-        code: EAT
-        name: Employment Appeal Tribunal
-        link: https://www.gov.uk/courts-tribunals/employment-appeal-tribunal
-        ncn: \[(\d{4})\] (EAT) (\d+)
-        selectable: true
-        listable: true
-        param: 'eat'
-        start_year: 2021
-        end_year: 2022
+    - code: EAT
+      name: Employment Appeal Tribunal
+      link: https://www.gov.uk/courts-tribunals/employment-appeal-tribunal
+      ncn: \[(\d{4})\] (EAT) (\d+)
+      selectable: true
+      listable: true
+      param: "eat"
+      start_year: 2021
+      end_year: 2022
 - name: first_tier_tribunals
   display_name: "First-tier Tribunals"
   is_tribunal: true
   courts:
-    -
-        code: UKFTT-TC
-        name: First-tier Tribunal (Tax Chamber)
-        link: https://www.gov.uk/courts-tribunals/first-tier-tribunal-tax
-        ncn: \[(\d{4})\] (UKFTT) (\d+) \((TC)\)
-        param: 'ukftt/tc'
-        start_year: 2022
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: UKFTT-GRC
-        name: First-tier Tribunal (General Regulatory Chamber)
-        param: 'ukftt/grc'
-        link: https://www.gov.uk/courts-tribunals/first-tier-tribunal-general-regulatory-chamber
-        ncn: \[(\d{4})\] (UKFTT) (\d+) \((GRC)\)
-        start_year: 2022
-        end_year: 2022
-        selectable: true
-        listable: true
-    -
-        code: ET
-        name: Employment Tribunal
-        link: https://www.gov.uk/courts-tribunals/employment-tribunal
-        start_year: 2022
-        end_year: 2022
-        selectable: false
-        listable: false
+    - code: ET
+      name: Employment Tribunal
+      link: https://www.gov.uk/courts-tribunals/employment-tribunal
+      start_year: 2022
+      end_year: 2022
+      selectable: false
+      listable: false
+    - code: UKFTT-GRC
+      name: First-tier Tribunal (General Regulatory Chamber)
+      param: "ukftt/grc"
+      link: https://www.gov.uk/courts-tribunals/first-tier-tribunal-general-regulatory-chamber
+      ncn: \[(\d{4})\] (UKFTT) (\d+) \((GRC)\)
+      start_year: 2022
+      end_year: 2022
+      selectable: true
+      listable: true
+    - code: UKFTT-TC
+      name: First-tier Tribunal (Tax Chamber)
+      link: https://www.gov.uk/courts-tribunals/first-tier-tribunal-tax
+      ncn: \[(\d{4})\] (UKFTT) (\d+) \((TC)\)
+      param: "ukftt/tc"
+      start_year: 2022
+      end_year: 2022
+      selectable: true
+      listable: true
```

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/neutral_citation_regex.yaml` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/data/neutral_citation_regex.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Reading the match_data:
 # the components of the URL for [2022] EAT 1 are the
 # 2nd, 1st and 3rd components of the neutral citation,
 # so the URL becomes eat/2022/1
 
 [
-  ['^\[(\d{4})\] (UKSC|UKPC) (\d+)$',  [2, 1, 3]],
+  ['^\[(\d{4})\] (UKSC|UKPC) (\d+)$', [2, 1, 3]],
   ['^\[(\d{4})\] (EWCA) (Civ|Crim) (\d+)$', [2, 3, 1, 4]],
-  ['^\[(\d{4})\] (EWHC) (\d+) \((Admin|Admlty|Ch|Comm|Costs|Fam|IPEC|Pat|QB|KB|SCCO|TCC)\)$', [2, 4, 1, 3]],
+  [
+    '^\[(\d{4})\] (EWHC) (\d+) \((Admin|Admlty|Ch|Comm|Costs|Fam|IPEC|Pat|QB|KB|SCCO|TCC)\)$',
+    [2, 4, 1, 3],
+  ],
   ['^\[(\d{4})\] (EWFC|EWCOP) (\d+)$', [2, 1, 3]],
   ['^\[(\d{4})\] (UKUT) (\d+) \((AAC|IAC|LC|TCC)\)$', [2, 4, 1, 3]],
   ['^\[(\d{4})\] (EAT) (\d+)$', [2, 1, 3]],
-  ['^\[(\d{4})\] (UKFTT) (\d+) \((TC|GRC)\)$', [2, 4, 1, 3]]
+  ['^\[(\d{4})\] (UKFTT) (\d+) \((TC|GRC)\)$', [2, 4, 1, 3]],
 ]
```

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/neutral.py` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/neutral.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_courts.py` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/test_courts.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,14 +161,19 @@
         )
         self.assertIn(
             "court3", [c.canonical_param for c in repo.get_listable_tribunals()]
         )
 
 
 class TestCourt(unittest.TestCase):
+    def test_repr_string(self):
+        court = Court({"name": "court_name"})
+        self.assertEqual("court_name", str(court))
+        self.assertEqual("court_name", repr(court))
+
     def test_list_name_explicit(self):
         court = Court({"list_name": "court_name"})
         self.assertEqual("court_name", court.list_name)
 
     def test_list_name_default(self):
         court = Court({"name": "court_name"})
         self.assertEqual("court_name", court.list_name)
```

### Comparing `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_neutral.py` & `ds_caselaw_utils-1.0.2/src/ds_caselaw_utils/test_neutral.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.1/PKG-INFO` & `ds_caselaw_utils-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for the National Archives Caselaw project
 Home-page: https://github.com/nationalarchives/ds-caselaw-utils
 License: MIT
 Keywords: national archives,caselaw
 Author: Nick Jackson
 Author-email: nick@dxw.com
 Requires-Python: >=3.9,<4.0
```

