# Comparing `tmp/KnowledgeCore-2.8.0.tar.gz` & `tmp/KnowledgeCore-2.8.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KnowledgeCore-2.8.0.tar", last modified: Fri Sep 16 07:44:02 2022, max compression
+gzip compressed data, was "KnowledgeCore-2.8.10.tar", last modified: Wed Jul  5 16:34:05 2023, max compression
```

## Comparing `KnowledgeCore-2.8.0.tar` & `KnowledgeCore-2.8.10.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     1556 2022-05-04 13:22:39.918314 KnowledgeCore-2.8.0/LICENSE
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     7076 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/PKG-INFO
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      295 2022-05-04 13:22:39.918314 KnowledgeCore-2.8.0/README-debian.md
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     5073 2022-06-13 07:31:57.063403 KnowledgeCore-2.8.0/README-pypi.rst
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     6422 2022-07-20 09:04:37.248145 KnowledgeCore-2.8.0/README.md
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/bin/
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     5312 2022-07-26 09:44:01.092153 KnowledgeCore-2.8.0/bin/knowledge_core
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      980 2022-06-13 06:59:45.426105 KnowledgeCore-2.8.0/setup.py
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/src/
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/src/knowledge_core/
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)       22 2022-08-17 09:38:56.712973 KnowledgeCore-2.8.0/src/knowledge_core/__init__.py
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     6174 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.0/src/knowledge_core/ansistrm.py
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/src/knowledge_core/api/
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    10485 2022-07-20 09:04:37.264146 KnowledgeCore-2.8.0/src/knowledge_core/api/__init__.py
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      146 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.0/src/knowledge_core/exceptions.py
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      552 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.0/src/knowledge_core/helpers.py
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)    36065 2022-08-17 09:35:06.894252 KnowledgeCore-2.8.0/src/knowledge_core/kb.py
--rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     8075 2022-08-17 09:16:53.164924 KnowledgeCore-2.8.0/src/knowledge_core/knowledge_core_ros.py
-drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2022-09-16 07:44:02.459476 KnowledgeCore-2.8.0/test/
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    16229 2022-05-20 13:16:21.928319 KnowledgeCore-2.8.0/test/test.py
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    13369 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.0/test/test_embedded.py
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    13223 2022-06-13 06:59:45.430105 KnowledgeCore-2.8.0/test/test_pythonic_api_ros.py
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     4572 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.0/test/test_reasoner.py
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     8924 2022-06-07 09:39:44.184273 KnowledgeCore-2.8.0/test/test_ros.py
--rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     7898 2022-06-07 09:39:44.184273 KnowledgeCore-2.8.0/test/test_ros_events.py
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     1556 2022-05-04 13:22:39.918314 KnowledgeCore-2.8.10/LICENSE
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     8182 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/PKG-INFO
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      295 2022-05-04 13:22:39.918314 KnowledgeCore-2.8.10/README-debian.md
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     5890 2022-09-16 07:46:33.168815 KnowledgeCore-2.8.10/README-pypi.rst
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     6422 2022-07-20 09:04:37.248145 KnowledgeCore-2.8.10/README.md
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     6903 2022-12-22 12:10:18.969731 KnowledgeCore-2.8.10/README.rst
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/bin/
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     5336 2023-05-08 12:02:57.979413 KnowledgeCore-2.8.10/bin/knowledge_core
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      980 2022-06-13 06:59:45.426105 KnowledgeCore-2.8.10/setup.py
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/src/
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/src/knowledge_core/
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)       23 2023-07-05 16:32:21.743220 KnowledgeCore-2.8.10/src/knowledge_core/__init__.py
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     6174 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.10/src/knowledge_core/ansistrm.py
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/src/knowledge_core/api/
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    10485 2022-07-20 09:04:37.264146 KnowledgeCore-2.8.10/src/knowledge_core/api/__init__.py
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      146 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.10/src/knowledge_core/exceptions.py
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)      552 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.10/src/knowledge_core/helpers.py
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)    37984 2023-07-05 15:59:09.345346 KnowledgeCore-2.8.10/src/knowledge_core/kb.py
+-rw-rw-r--   0 severinlemaignan  (1001) severinlemaignan  (1001)     9231 2023-05-08 12:17:04.188612 KnowledgeCore-2.8.10/src/knowledge_core/knowledge_core_ros.py
+drwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)        0 2023-07-05 16:34:05.474897 KnowledgeCore-2.8.10/test/
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    16229 2022-05-20 13:16:21.928319 KnowledgeCore-2.8.10/test/test.py
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    13369 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.10/test/test_embedded.py
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    13335 2023-07-05 15:53:14.476794 KnowledgeCore-2.8.10/test/test_pythonic_api_ros.py
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     4572 2022-05-04 13:22:39.922314 KnowledgeCore-2.8.10/test/test_reasoner.py
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)    10862 2023-07-05 15:31:32.466860 KnowledgeCore-2.8.10/test/test_ros.py
+-rwxrwxr-x   0 severinlemaignan  (1001) severinlemaignan  (1001)     7898 2022-06-07 09:39:44.184273 KnowledgeCore-2.8.10/test/test_ros_events.py
```

### Comparing `KnowledgeCore-2.8.0/LICENSE` & `KnowledgeCore-2.8.10/LICENSE`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/PKG-INFO` & `KnowledgeCore-2.8.10/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: KnowledgeCore
-Version: 2.8.0
+Version: 2.8.10
 Summary: A RDFlib-backed minimalistic knowledge based for robotic application
 Home-page: https://github.com/severin-lemaignan/knowledge_core
 Author: Séverin Lemaignan
 Author-email: severin.lemaignan@pal-robotics.com
 License: BSD
 Description: KnowledgeCore
         ==============
@@ -20,14 +20,50 @@
         idiomatic Python binding, making easy to integrate the knowledge base in
         your applications.
         
         It integrates with the `reasonable <https://github.com/gtfierro/reasonable>`__ OWL2
         RL reasoner to provide OWL2 semantics and fast knowledge materialisation.
         
         
+        Example
+        -------
+        
+        This example uses the ROS API (see below), with some Pythonic syntatic sugar:
+        
+        .. code:: python
+        
+           from knowledge_core.api import KB
+           
+           rospy.init_node("test_knowledge_base")
+           
+           kb = KB()
+           
+           def on_robot_entering_antonio_property(evt):
+             print("A robot entered Antonio's %s: %s" (evt[0]["place"], evt[0]["robot"]))
+           
+           kb += "ari rdf:type Robot"  
+           kb += ["antonio looksAt ari", "ari isIn kitchen"]
+           
+           kb.subscribe(["?robot isIn ?place", "?place belongsTo antonio", "?robot rdf:type Robot"], onRobotEnteringAntonioProperty)
+           
+           kb += "kitchen belongsTo antonio"
+           
+           # try as well:
+           # kb -= "antonio looksAt ari" to remove facts
+           # kb["* rdf:type Robot"] to query the knowledge base
+           
+           rospy.spin()
+        
+        
+        will print:
+        
+        ```
+        A robot entered Antonio's kitchen: ari
+        ```
+        
         Installation
         ------------
         
         **KnowledgeCore only supports Python 3**
         
         Prerequisite
         ~~~~~~~~~~~~
```

### Comparing `KnowledgeCore-2.8.0/README-pypi.rst` & `KnowledgeCore-2.8.10/README-pypi.rst`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,50 @@
 idiomatic Python binding, making easy to integrate the knowledge base in
 your applications.
 
 It integrates with the `reasonable <https://github.com/gtfierro/reasonable>`__ OWL2
 RL reasoner to provide OWL2 semantics and fast knowledge materialisation.
 
 
+Example
+-------
+
+This example uses the ROS API (see below), with some Pythonic syntatic sugar:
+
+.. code:: python
+
+   from knowledge_core.api import KB
+   
+   rospy.init_node("test_knowledge_base")
+   
+   kb = KB()
+   
+   def on_robot_entering_antonio_property(evt):
+     print("A robot entered Antonio's %s: %s" (evt[0]["place"], evt[0]["robot"]))
+   
+   kb += "ari rdf:type Robot"  
+   kb += ["antonio looksAt ari", "ari isIn kitchen"]
+   
+   kb.subscribe(["?robot isIn ?place", "?place belongsTo antonio", "?robot rdf:type Robot"], onRobotEnteringAntonioProperty)
+   
+   kb += "kitchen belongsTo antonio"
+   
+   # try as well:
+   # kb -= "antonio looksAt ari" to remove facts
+   # kb["* rdf:type Robot"] to query the knowledge base
+   
+   rospy.spin()
+
+
+will print:
+
+```
+A robot entered Antonio's kitchen: ari
+```
+
 Installation
 ------------
 
 **KnowledgeCore only supports Python 3**
 
 Prerequisite
 ~~~~~~~~~~~~
```

### Comparing `KnowledgeCore-2.8.0/README.md` & `KnowledgeCore-2.8.10/README.md`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/bin/knowledge_core` & `KnowledgeCore-2.8.10/bin/knowledge_core`

 * *Files 2% similar despite different names*

```diff
@@ -179,12 +179,14 @@
 
     try:
         while True:
             asyncore.loop(
                 timeout=0.02, count=1
             )  # event will be notified at worst 20ms after they are triggered
             kb.process()
+            ros.step()
+
     except KeyboardInterrupt:
         if args.no_ros:
             ros.shutdown()
         kb.stop_services()
         logger.info("Bye bye")
```

### Comparing `KnowledgeCore-2.8.0/setup.py` & `KnowledgeCore-2.8.10/setup.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/src/knowledge_core/ansistrm.py` & `KnowledgeCore-2.8.10/src/knowledge_core/ansistrm.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/src/knowledge_core/api/__init__.py` & `KnowledgeCore-2.8.10/src/knowledge_core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/src/knowledge_core/helpers.py` & `KnowledgeCore-2.8.10/src/knowledge_core/helpers.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/src/knowledge_core/kb.py` & `KnowledgeCore-2.8.10/src/knowledge_core/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 "invalid syntax for statement %s: it should be formed of 3 terms."
                 % stmt
             )
         data += " %s . " % stmt
 
     try:
         return Graph().parse(data=data, format="n3")
-    except rdflib.plugins.parsers.notation3.BadSyntax:
+    except rdflib.plugins.parsers.notation3.BadSyntax as bs:
         raise KbServerError("invalid syntax for statements %s" % stmts)
 
 
 # @memoize
 def parse_stmts(stmts):
 
     return list(parse_stmts_to_graph(stmts))
@@ -127,14 +127,17 @@
     except IndexError:
         raise KbServerError("invalid syntax for statement <%s>" % stmt)
 
 
 # @memoize
 def parse_term(term):
 
+    if type(term) in [bool, int, float]:
+        return Literal(term)
+
     try:
         # TODO: correct, but not super effective!
         return list(
             Graph().parse(data=N3_PROLOGUE + " <s> <p> %s ." % term, format="n3")
         )[0][2]
     except rdflib.plugins.parsers.notation3.BadSyntax:
         raise KbServerError("invalid syntax for term <%s>" % term)
@@ -153,15 +156,18 @@
 def shorten(graph, stmt):
 
     res = []
     for t in stmt:
         if isinstance(t, URIRef):
             res.append(graph.qname(t))
         elif isinstance(t, Literal):
-            res.append(t.value)
+            lit = t.toPython()
+            if isinstance(lit, str):
+                lit = '"%s"' % lit
+            res.append(lit)
         else:
             res.append(t.n3())
     return res
 
 
 def shortenN(graph, stmts):
     return [shorten(graph, s) for s in stmts]
@@ -405,15 +411,15 @@
             return []
 
         matching_concepts = set()
 
         for s, p, o in about:
             if s == resource or p == resource or o == resource:
                 matching_concepts.add(resource)
-            elif p == shorten_term(self.models[DEFAULT_MODEL].graph, RDFS.label):
+            elif p == shorten_term(self.models[DEFAULT_MODEL].graph, RDFS.label) and o == '"%s"' % resource:
                 matching_concepts.add(s)
 
         res = [(concept, self.typeof(concept, models)) for concept in matching_concepts]
         logger.info("Found: " + str(res))
         return res
 
     def _instancesof(self, term, direct=False, models=[]):
@@ -677,23 +683,28 @@
 
         if type(policy) != dict:
             raise KbServerError("Expected a dictionary as policy")
 
         if isinstance(stmts, str):
             raise KbServerError("A list of statements is expected")
 
+        vars = get_all_variables(stmts)
+
         subgraph = parse_stmts_to_graph(stmts)
         parsed_stmts = "\n\t- ".join(
             [" ".join([str(t) for t in s]) for s in shorten_graph(subgraph)]
         )
 
         models = self.normalize_models(policy.get("models", []))
 
         if policy["method"] in ["update", "safe_update", "add", "safe_add", "revision"]:
 
+            if len(vars) > 0:
+                raise KbServerError("You can not add/update statements containing variables: %s" % stmts)
+
             if policy["method"].startswith("safe"):
                 logger.warn(
                     "Warning: %s is not implemented. Performing %s instead."
                     % (policy["method"], policy["method"][5:])
                 )
             if policy["method"].endswith("add"):
                 logger.warn(
@@ -716,14 +727,49 @@
                     if p in self._functionalproperties:
                         self.models[model].graph.set((s, p, o))  # TODO: lifespan
                     else:
                         self.models[model].graph.add((s, p, o))  # TODO: lifespan
                 self.models[model].is_dirty = True
 
         elif policy["method"] == "retract":
+
+            if len(vars) > 0:
+
+                if len(stmts) > 1:
+                    raise KbServerError("Removing multiple statements that \
+                            include variables or wildcards is not supported. \
+                            Wildcards are only permitted with a single \
+                            pattern.")
+
+                # we've been provided with a pattern that contains at least one variable.
+                # find() all matching values for the varaible(s), and reconstruct the final
+                # list of statements to retract that match that pattern.
+
+                res = self.find(stmts)
+
+                for tok in stmts[0].split():
+                    # if the token is *not* a variable, add it to the find() results 'as it'
+                    if not tok.startswith("?"):
+                        for e in res:
+                            e[tok] = tok
+
+                # tok_order is a copy of the pattern, without the leading '?'
+                tok_order = [tok[1:] if tok.startswith("?") else tok for tok in stmts[0].split()]
+
+                # final list of statments to remove
+                new_stmts = []
+                for e in res:
+                    new_stmts.append(" ".join([str(e[tok_order[0]]), str(e[tok_order[1]]), parse_term(e[tok_order[2]]).n3()]))
+                
+                subgraph = parse_stmts_to_graph(new_stmts)
+                parsed_stmts = "\n\t- ".join(
+                [" ".join([str(t) for t in s]) for s in shorten_graph(subgraph)]
+                )
+
+
             logger.info("Deleting from " + str(list(models)) + ":\n\t- " + parsed_stmts)
             for model in models:
                 self.models[model].graph -= subgraph
                 self.models[model].is_dirty = True
 
         else:
             raise KbServerError("Unknown method in revise: %s" % policy["method"])
```

### Comparing `KnowledgeCore-2.8.0/src/knowledge_core/knowledge_core_ros.py` & `KnowledgeCore-2.8.10/src/knowledge_core/knowledge_core_ros.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,28 +7,36 @@
         "Unable to load the ROS support. You might want to run with --no-ros"
         " to use KnowledgeCore without ROS support enabled."
     )
     sys.exit(1)
 
 import json
 
+from diagnostic_msgs.msg import DiagnosticArray, DiagnosticStatus
 from knowledge_core.exceptions import KbServerError
 
 from knowledge_core.srv import Manage, Revise, Query, About, Lookup, Sparql, Event
 from std_msgs.msg import String
 
 EVENTS_TOPIC_NS = "/kb/events/"
 
+DIAGNOSTICS_FREQUENCY = 1  # Hz
+
 
 class KnowledgeCoreROS:
     def __init__(self, kb):
         self.kb = kb
 
         rospy.init_node("knowledge_core", disable_signals=True)
 
+        self.diagnostics_pub = rospy.Publisher(
+            "/diagnostics", DiagnosticArray, queue_size=1
+        )
+        self.last_diagnostics_ts = rospy.Time()
+
         self.update_sub = rospy.Subscriber("/kb/add_fact", String, self.on_update_fact)
         self.retract_sub = rospy.Subscriber(
             "/kb/remove_fact", String, self.on_retract_fact
         )
 
         self.services = {
             "manage": rospy.Service("kb/manage", Manage, self.handle_manage),
@@ -223,10 +231,33 @@
 
         rospy.logwarn("Subscribed to event " + evt)
 
         self.kb.eventsubscriptions.setdefault(evt, []).append(evt_relay)
 
         return EventResponse(id=evt, topic=EVENTS_TOPIC_NS + evt)
 
+    def step(self):
+        now = rospy.Time.now()
+
+        if (now - self.last_diagnostics_ts).to_sec() > 1 / DIAGNOSTICS_FREQUENCY:
+            if self.kb.reasoner_enabled:
+                msg = DiagnosticStatus(
+                    level=DiagnosticStatus.OK,
+                    name="Reasoning: Knowledge base",
+                    message="Knowledge base running, with OWL/RDF reasoner enabled",
+                )
+            else:
+                msg = DiagnosticStatus(
+                    level=DiagnosticStatus.WARN,
+                    name="Reasoning: Knowledge base",
+                    message="Knowledge base running, but OWL/RDF reasoner not enabled",
+                )
+            arr = DiagnosticArray()
+            arr.header.stamp = rospy.Time.now()
+            arr.status = [msg]
+            self.diagnostics_pub.publish(arr)
+
+            self.last_diagnostics_ts = now
+
     def shutdown(self):
 
         rospy.signal_shutdown("KnowledgeCore closing")
```

### Comparing `KnowledgeCore-2.8.0/test/test.py` & `KnowledgeCore-2.8.10/test/test.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/test/test_embedded.py` & `KnowledgeCore-2.8.10/test/test_embedded.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/test/test_pythonic_api_ros.py` & `KnowledgeCore-2.8.10/test/test_pythonic_api_ros.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,18 @@
         )
 
         self.kb += ["alfred likes icecream"]
         self.assertCountEqual(self.kb.lookup("likes"), [["likes", "object_property"]])
         self.assertCountEqual(self.kb.lookup("alfred"), [["alfred", "instance"]])
 
         self.kb += ['nono rdfs:label "alfred"']
+        self.kb += ['sentence rdfs:label "alfred is a charming person"']
         self.assertCountEqual(
             self.kb.lookup("alfred"), [["alfred", "instance"], ["nono", "undecided"]]
-        )
+        )  # 'sentence' should *not* be included
 
         self.kb += ['gerard rdfs:label "likes"']
         self.assertCountEqual(
             self.kb.lookup('"likes"'),
             [['"likes"', "literal"]],
         )
```

### Comparing `KnowledgeCore-2.8.0/test/test_reasoner.py` & `KnowledgeCore-2.8.10/test/test_reasoner.py`

 * *Files identical despite different names*

### Comparing `KnowledgeCore-2.8.0/test/test_ros.py` & `KnowledgeCore-2.8.10/test/test_ros.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,14 +84,81 @@
         self.assertCountEqual(
             json.loads(res.json),
             [
                 {"s": "stockbot"},
             ],
         )
 
+    def test_retract_wildcards(self):
+
+        self.assertTrue(
+            self.revise(
+                statements=[
+                    "ari rdf:type Robot",
+                    "ari isIn kitchen",
+                    "tiago rdf:type Robot",
+                    "tiago isIn living_room",
+                ],
+                method=ReviseRequest.ADD,
+            )
+        )
+
+        self.assertTrue(
+            self.revise(
+                statements=["ari ?p ?o"],
+                method=ReviseRequest.DELETE,
+            )
+        )
+
+        res = self.query(["ari ?p ?o"], None, None)
+        self.assertFalse(json.loads(res.json))
+
+        self.assertTrue(
+            self.revise(
+                statements=["tiago isIn ?loc"],
+                method=ReviseRequest.DELETE,
+            )
+        )
+
+        res = self.query(["tiago ?p ?o"], None, None)
+        self.assertCountEqual(
+            json.loads(res.json),
+            [{"p": "rdf:type", "o": "Robot"}, {"p": "rdf:type", "o": "owl:Thing"}],
+        )
+
+        self.assertTrue(
+            self.revise(
+                statements=["?robot rdf:type Robot"],
+                method=ReviseRequest.DELETE,
+            )
+        )
+
+        res = self.query(["?s rdf:type Robot"], None, None)
+        self.assertFalse(json.loads(res.json))
+
+        # TODO:
+        # as of knowledge_core 2.8.9, retracting with wildcard is only support
+        # for a single statement.
+        # self.assertTrue(
+        #    self.revise(
+        #        statements=["stockbot rdf:type Robot", "talos rdf:type Robot"],
+        #        method=ReviseRequest.ADD,
+        #    )
+        # )
+
+        # self.assertTrue(
+        #    self.revise(
+        #        statements=["stockbot ?p ?o", "talos ?a ?b"],
+        #        method=ReviseRequest.DELETE,
+        #    )
+        # )
+
+        # res = self.query(["?s rdf:type Robot"], None, None)
+        # self.assertFalse(json.loads(res.json))
+
     def test_errors(self):
 
         self.assertFalse(
             self.revise(statements=["term"], method=ReviseRequest.ADD).success
         )
         self.assertFalse(
             self.revise(statements=["term term"], method=ReviseRequest.ADD).success
```

### Comparing `KnowledgeCore-2.8.0/test/test_ros_events.py` & `KnowledgeCore-2.8.10/test/test_ros_events.py`

 * *Files identical despite different names*

