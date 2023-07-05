# Comparing `tmp/ontobot_change_agent-0.4.0.tar.gz` & `tmp/ontobot_change_agent-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontobot_change_agent-0.4.0.tar", max compression
+gzip compressed data, was "ontobot_change_agent-0.4.1.tar", max compression
```

## Comparing `ontobot_change_agent-0.4.0.tar` & `ontobot_change_agent-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-04-06 16:23:00.355237 ontobot_change_agent-0.4.0/LICENSE
--rw-r--r--   0        0        0     1025 2023-04-06 16:23:00.355237 ontobot_change_agent-0.4.0/README.md
--rw-r--r--   0        0        0     1056 2023-04-06 16:23:16.603288 ontobot_change_agent-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      349 2023-04-06 16:23:00.359237 ontobot_change_agent-0.4.0/src/ontobot_change_agent/__init__.py
--rw-r--r--   0        0        0      337 2023-04-06 16:23:00.359237 ontobot_change_agent-0.4.0/src/ontobot_change_agent/__main__.py
--rw-r--r--   0        0        0     6854 2023-04-06 16:23:00.359237 ontobot_change_agent-0.4.0/src/ontobot_change_agent/api.py
--rw-r--r--   0        0        0     6430 2023-04-06 16:23:00.359237 ontobot_change_agent-0.4.0/src/ontobot_change_agent/cli.py
--rw-r--r--   0        0        0      188 2023-04-06 16:23:00.359237 ontobot_change_agent-0.4.0/src/ontobot_change_agent/constants.py
--rw-r--r--   0        0        0     1189 2023-04-06 16:23:00.359237 ontobot_change_agent-0.4.0/src/ontobot_change_agent/version.py
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 ontobot_change_agent-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-05 21:49:01.617619 ontobot_change_agent-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1025 2023-07-05 21:49:01.617619 ontobot_change_agent-0.4.1/README.md
+-rw-r--r--   0        0        0     1056 2023-07-05 21:49:22.802214 ontobot_change_agent-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      349 2023-07-05 21:49:01.621619 ontobot_change_agent-0.4.1/src/ontobot_change_agent/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-05 21:49:01.621619 ontobot_change_agent-0.4.1/src/ontobot_change_agent/__main__.py
+-rw-r--r--   0        0        0     8593 2023-07-05 21:49:01.621619 ontobot_change_agent-0.4.1/src/ontobot_change_agent/api.py
+-rw-r--r--   0        0        0     6678 2023-07-05 21:49:01.621619 ontobot_change_agent-0.4.1/src/ontobot_change_agent/cli.py
+-rw-r--r--   0        0        0      188 2023-07-05 21:49:01.621619 ontobot_change_agent-0.4.1/src/ontobot_change_agent/constants.py
+-rw-r--r--   0        0        0     1189 2023-07-05 21:49:01.621619 ontobot_change_agent-0.4.1/src/ontobot_change_agent/version.py
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 ontobot_change_agent-0.4.1/PKG-INFO
```

### Comparing `ontobot_change_agent-0.4.0/LICENSE` & `ontobot_change_agent-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ontobot_change_agent-0.4.0/README.md` & `ontobot_change_agent-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ontobot_change_agent-0.4.0/pyproject.toml` & `ontobot_change_agent-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 
 name = "ontobot-change-agent"
-version = "0.4.0"
+version = "0.4.1"
 description = "Update ontologies using change language."
 
 authors = ["Harshad Hegde <hhegde@lbl.gov>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-oaklib = "^0.4.0"
+oaklib = "^0.5.0"
 PyGithub = "^1.55"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 Sphinx = "^5.2.3"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autodoc-typehints = "^1.19.4"
```

### Comparing `ontobot_change_agent-0.4.0/src/ontobot_change_agent/api.py` & `ontobot_change_agent-0.4.1/src/ontobot_change_agent/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # -*- coding: utf-8 -*-
 """API section."""
 
+import json
 import re
 from os.path import join, splitext
 from pathlib import Path
 from typing import Generator, Optional
 
 import kgcl_schema.grammar.parser as kgcl_parser
+import requests
+import yaml
 from github import Github
 from github.Issue import Issue
 from oaklib.cli import query_terms_iterator
 from oaklib.implementations import ProntoImplementation, SimpleOboImplementation
 from oaklib.interfaces.patcher_interface import PatcherInterface
 from oaklib.selector import get_resource_from_shorthand
 
@@ -27,15 +30,17 @@
 
 # Token.txt unique to every user.
 # For more information:
 #   https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
 # Save the token in a txt file as named below.
 SRC = Path(__file__).parent
 TOKEN_FILE = join(SRC, "token.txt")
-
+ISSUE_TEMPLATE_DIR = ".github/ISSUE_TEMPLATE"
+# TODO: This variable below needs to be standard across the board.
+NEW_TERM_TEMPLATE_YAML = "/add-term.yml"
 # Example for API: https://pygithub.readthedocs.io/en/latest/examples.html
 
 RAW_DATA = "_rawData"
 ISSUE_KEYS = [
     # 'repository_url',
     # 'html_url',
     "number",
@@ -72,14 +77,16 @@
     if token is None:
         token_file = TOKEN_FILE
         with open(token_file, "r") as t:
             token = t.read().rstrip()
 
     g = Github(token)
     repo = g.get_repo(repository_name)
+    global ISSUE_TEMPLATE_DIR
+    ISSUE_TEMPLATE_DIR = repo.contents_url.replace("{+path}", ISSUE_TEMPLATE_DIR)
     label_object = None
     if label:
         label_object = repo.get_label(label)
     if number and number > 0:
         yield _extract_info_from_issue_object(repo.get_issue(number))
     else:
         issues = repo.get_issues(state=state)
@@ -165,32 +172,61 @@
 
         impl_obj.apply_patch(change)
 
     impl_obj.dump(output, output_format)
 
 
 def process_new_term_template(body, prefix):
-    """Process an issue generated via new term request template."""
+    """Process an issue generated via new term request template.
+
+    :param body: Body of the issue.
+    :param prefix: Prefix of the ontology corresponding to the repository.
+    :return: Command list and body as a dict. If Issue does not match template: (None, None)
+    :raises ValueError: If prefix is absent.
+    """
     split_body = body.replace("\r", "").strip("#").split("\n\n###")
-    CURIE = prefix + ":XXXXXX"
+    reason = None
+    if prefix:
+        CURIE = prefix + ":XXXXXX"
+    else:
+        raise (ValueError("Prefix must be provided in the command."))
+
     body_as_dict = {}
 
     for line in split_body:
         if line.split("\n\n")[1].strip() not in ["_No response_", "None"]:
             body_as_dict[line.split("\n\n")[0].strip()] = line.split("\n\n")[1].strip()
+    response_1 = requests.get(
+        ISSUE_TEMPLATE_DIR + NEW_TERM_TEMPLATE_YAML, allow_redirects=True, timeout=5
+    )
+    metadata = json.loads(response_1.content.decode("utf-8"))
+    if "message" in metadata and metadata["message"] == "Not Found":
+        reason = "the 'New Term request' template yml does not exist."
+        return (None, None, reason)
+    else:
+        download_url = metadata["download_url"]
+        response_2 = requests.get(download_url, allow_redirects=True, timeout=5)
+        content = response_2.content.decode("utf8")
+        template = yaml.safe_load(content)
+        list_of_template_keys = [x["attributes"]["label"] for x in template["body"] if "id" in x]
+        if all(key in list_of_template_keys for key in body_as_dict.keys()):
+            kgcl_command_list = [f"create node {CURIE} '{body_as_dict['Label']}'"]
+
+            if SYNONYMS in body_as_dict:
+                body_as_dict[SYNONYMS] = body_as_dict[SYNONYMS].split(",")
+                for synonym in body_as_dict[SYNONYMS]:
+                    if SYNONYM_TYPE in body_as_dict:
+                        kgcl_command_list.append(
+                            f"create {body_as_dict[SYNONYM_TYPE]} synonym '{synonym.strip()}' for {CURIE}"  # noqa
+                        )
+                    else:
+                        kgcl_command_list.append(f"create synonym {synonym.strip()} for {CURIE}")
 
-    kgcl_command_list = [f"create node {CURIE} '{body_as_dict['Label']}'"]
-
-    if SYNONYMS in body_as_dict:
-        body_as_dict[SYNONYMS] = body_as_dict[SYNONYMS].split(",")
-        for synonym in body_as_dict[SYNONYMS]:
-            if SYNONYM_TYPE in body_as_dict:
+            if DEFINITION in body_as_dict:
                 kgcl_command_list.append(
-                    f"create {body_as_dict[SYNONYM_TYPE]} synonym '{synonym.strip()}' for {CURIE}"
+                    f"add definition '{body_as_dict[DEFINITION].strip()}' to {CURIE}"
                 )
-            else:
-                kgcl_command_list.append(f"create synonym {synonym.strip()} for {CURIE}")
-
-    if DEFINITION in body_as_dict:
-        kgcl_command_list.append(f"add definition '{body_as_dict[DEFINITION].strip()}' to {CURIE}")
 
-    return (kgcl_command_list, body_as_dict)
+            return (kgcl_command_list, body_as_dict, reason)
+        else:
+            reason = "the issue does not match the 'New Term request' template."
+            return (None, None, reason)
```

### Comparing `ontobot_change_agent-0.4.0/src/ontobot_change_agent/cli.py` & `ontobot_change_agent-0.4.1/src/ontobot_change_agent/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,17 +166,25 @@
         repository_name=repo, token=token, label=label, number=number, state=state
     ):
         # Make sure ontobot_change_agent needs to be triggered or no.
         if issue:
             KGCL_COMMANDS = []
             if NEW_TERM_LABEL in issue["labels"]:
                 formatted_body = "The following input was provided: </br> "
-                KGCL_COMMANDS, body_as_dict = process_new_term_template(issue["body"], prefix)
-                formatted_body += _convert_to_markdown(body_as_dict)
-                formatted_body += "</br> The following commands were executed: </br> "
+                KGCL_COMMANDS, body_as_dict, reason = process_new_term_template(
+                    issue["body"], prefix
+                )
+                if reason is None:
+                    formatted_body += _convert_to_markdown(body_as_dict)
+                    formatted_body += "</br> The following commands were executed: </br> "
+                else:
+                    click.echo(
+                        f"""{issue[TITLE]} does not need ontobot's attention since {reason}""",  # noqa
+                    )
+                    break
 
             elif re.match(r"(.*)ontobot(.*)apply(.*):(.*)", issue[BODY]):
                 formatted_body = "The following commands were executed: </br> "
                 bullet_starters = ["* ", "- "]
                 for bullet in bullet_starters:
                     KGCL_COMMANDS.extend(
                         [
@@ -190,18 +198,15 @@
 
             else:
                 click.echo(f"""{issue[TITLE]} does not need ontobot's attention.""")
         else:
             click.echo(f"""Issue number:{number} is either closed or does not exist.""")
             break
 
-        if output:
-            new_output = output
-        else:
-            new_output = input
+        new_output = output if output else input
 
         if issue["number"] == number and len(KGCL_COMMANDS) > 0:  # noqa W503  # noqa W503
             process_issue_via_oak(
                 input=input,
                 commands=KGCL_COMMANDS,
                 output=new_output,
             )
```

### Comparing `ontobot_change_agent-0.4.0/src/ontobot_change_agent/version.py` & `ontobot_change_agent-0.4.1/src/ontobot_change_agent/version.py`

 * *Files identical despite different names*

### Comparing `ontobot_change_agent-0.4.0/PKG-INFO` & `ontobot_change_agent-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ontobot-change-agent
-Version: 0.4.0
+Version: 0.4.1
 Summary: Update ontologies using change language.
 License: MIT
 Author: Harshad Hegde
 Author-email: hhegde@lbl.gov
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: PyGithub (>=1.55,<2.0)
-Requires-Dist: oaklib (>=0.4.0,<0.5.0)
+Requires-Dist: oaklib (>=0.5.0,<0.6.0)
 Description-Content-Type: text/markdown
 
 <!--
 <p align="center">
   <img src="https://github.com/hrshdhgd/ontobot-change-agent/raw/main/docs/source/logo.png" height="150">
 </p>
 -->
```

