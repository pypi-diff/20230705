# Comparing `tmp/pyperf2-0.4.5-py3-none-any.whl.zip` & `tmp/pyperf2-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11552 bytes, number of entries: 6
--rw-r--r--  2.0 unx    26905 b- defN 23-Jul-04 10:45 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3340 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-04 10:46 pyperf2-0.4.5.dist-info/RECORD
-6 files, 42165 bytes uncompressed, 10718 bytes compressed:  74.6%
+Zip file size: 11548 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    26898 b- defN 23-Jul-05 09:46 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jul-05 09:48 pyperf2-0.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3340 b- defN 23-Jul-05 09:48 pyperf2-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 09:48 pyperf2-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-05 09:48 pyperf2-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      463 b- defN 23-Jul-05 09:48 pyperf2-0.4.6.dist-info/RECORD
+6 files, 42158 bytes uncompressed, 10714 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.4.5.dist-info/LICENSE
+Filename: pyperf2-0.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.4.5.dist-info/METADATA
+Filename: pyperf2-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.4.5.dist-info/WHEEL
+Filename: pyperf2-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.4.5.dist-info/top_level.txt
+Filename: pyperf2-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.4.5.dist-info/RECORD
+Filename: pyperf2-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -453,23 +453,21 @@
             if self.use_linux_namespace not in list(netns.listnetns()):
                 raise NameSpaceNotFoundError(
                     f"Namespace {self.use_linux_namespace} cannot be found."
                 )
             _cli.extend("ip netns exec {0}".format(self.use_linux_namespace).split(" "))
         _cli.append(self.iperf_binary_path)
         _cli.append("-e")
-        if int(self.test_duration) and self.type == "client":
-            _cli.append("-t")
-            _cli.append(self.test_duration)
-        elif int(self.test_duration) > 0:
-            _cli.append("-t")
-            _cli.append(self.test_duration)
 
         if self.type == "server":
             _cli.append("-s")
+            if int(self.test_duration) > 0:
+                _cli.append("-t")
+                _cli.append(self.test_duration)
+
             if self.bind_ip:
                 _cli.append("-B")
                 _cli.append(self.bind_ip)
             ####Ü
             if self.protocol == "tcp":
                 self._result_regex = re.compile(
                     r"^\[\s*(?P<stream_id>\d+)\]\s+(?P<interval_begin>\d+\.\d+)-(?P<interval_end>\d+\.\d+)\s+(?P<interval_unit>\S+)\s+(?P<received>\S+)\s+(?P<received_unit>\S+)\s+(?P<bandwidth>\S+)\s+(?P<bandwidth_unit>\S+)?"
@@ -484,14 +482,18 @@
                 )
 
         elif self.type == "client":
             _cli.append("-c")
             if not self.server_ip:
                 raise ValueError("Client needs server_ip to be set")
             _cli.append(self.server_ip)
+            if self.test_duration:
+                _cli.append("-t")
+                _cli.append(self.test_duration)
+
             if self.bind_ip and self.client_source_port:
                 _cli.append("-B")
                 _cli.append("{0}:{1}".format(self.bind_ip, self.client_source_port))
             elif self.bind_ip:
                 _cli.append("-B")
                 _cli.append(self.bind_ip)
             if self.protocol == "udp":
```

## Comparing `pyperf2-0.4.5.dist-info/LICENSE` & `pyperf2-0.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.4.5.dist-info/METADATA` & `pyperf2-0.4.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.4.5
+Version: 0.4.6
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

