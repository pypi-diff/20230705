# Comparing `tmp/vcarhilclient-1.0.608.tar.gz` & `tmp/vcarhilclient-1.0.705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.608.tar", last modified: Thu Jun  8 03:17:39 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.705.tar", last modified: Wed Jul  5 09:44:35 2023, max compression
```

## Comparing `vcarhilclient-1.0.608.tar` & `vcarhilclient-1.0.705.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 03:17:39.068292 vcarhilclient-1.0.608/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.608/LICENSE
--rw-rw-rw-   0        0        0     2596 2023-06-08 03:17:39.068292 vcarhilclient-1.0.608/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.608/README.md
--rw-rw-rw-   0        0        0       86 2023-06-08 03:17:39.070294 vcarhilclient-1.0.608/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-06-08 03:15:35.000000 vcarhilclient-1.0.608/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:17:39.053451 vcarhilclient-1.0.608/vcarhilclient/
--rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.608/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.608/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.608/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.608/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    50876 2023-05-31 10:22:11.000000 vcarhilclient-1.0.608/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.608/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    12059 2023-05-31 10:22:11.000000 vcarhilclient-1.0.608/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.608/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.608/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.608/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:17:39.065293 vcarhilclient-1.0.608/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2596 2023-06-08 03:17:38.000000 vcarhilclient-1.0.608/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-08 03:17:38.000000 vcarhilclient-1.0.608/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 03:17:38.000000 vcarhilclient-1.0.608/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 03:17:38.000000 vcarhilclient-1.0.608/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 03:17:38.000000 vcarhilclient-1.0.608/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 09:44:35.230883 vcarhilclient-1.0.705/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.705/LICENSE
+-rw-rw-rw-   0        0        0     2596 2023-07-05 09:44:35.231878 vcarhilclient-1.0.705/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.705/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-05 09:44:35.232875 vcarhilclient-1.0.705/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-07-05 09:40:42.000000 vcarhilclient-1.0.705/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 09:44:35.208185 vcarhilclient-1.0.705/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.705/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.705/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.705/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50918 2023-07-05 09:39:43.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    14192 2023-07-05 09:39:43.000000 vcarhilclient-1.0.705/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.705/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2383 2023-07-05 09:39:43.000000 vcarhilclient-1.0.705/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.705/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-07-05 09:44:35.228887 vcarhilclient-1.0.705/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2596 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-05 09:44:35.000000 vcarhilclient-1.0.705/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.608/LICENSE` & `vcarhilclient-1.0.705/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/PKG-INFO` & `vcarhilclient-1.0.705/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.608
+Version: 1.0.705
 Summary: vcarhilclient
 Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vcarhilclient-1.0.608/README.md` & `vcarhilclient-1.0.705/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/setup.py` & `vcarhilclient-1.0.705/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.608",
+    version="1.0.705",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `vcarhilclient-1.0.608/vcarhilclient/Enums.py` & `vcarhilclient-1.0.705/vcarhilclient/Enums.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/vcarhilclient/kunyi_ma.py` & `vcarhilclient-1.0.705/vcarhilclient/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.705/vcarhilclient/kunyi_mrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,28 +450,28 @@
         en_pointer = c_char_p(bs)
         mrt_lib.mrt_daq_set_trigger_period.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32, c_uint32]
         mrt_lib.mrt_daq_set_trigger_period.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_set_trigger_period(self.context, en_pointer, c_uint64(daq_handle),
                                                         period_ms, offset_ms)
         return error_code
 
-    def daq_set_port(self, env_name, daq_handle, port_index, model_instance_name, port_name, port_type, port_datatype):
+    def daq_set_port(self, env_name, daq_handle, port_index, model_instance_name, port_name, port_type):
 
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         modelName = model_instance_name.encode('utf-8')
         mn_pointer = c_char_p(modelName)
         portName = port_name.encode('utf-8')
         pn_pointer = c_char_p(portName)
         mrt_lib.mrt_daq_set_port.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32, c_char_p, c_char_p, c_int32]
         mrt_lib.mrt_daq_set_port.restype = mrt_status_t
         error_code = mrt_lib.mrt_daq_set_port(self.context, en_pointer, c_uint64(daq_handle), c_uint32(port_index),
                                               mn_pointer, pn_pointer, port_type[0])
         if error_code.value == 0:
-            self.daqs[(daq_handle,env_name)][port_index] = (model_instance_name, port_name, port_type[0], port_datatype)
+            self.daqs[(daq_handle,env_name)][port_index] = (model_instance_name, port_name, port_type[0])
         return error_code
 
     def daq_set_multiple_ports(self, env_name, daq_handle, port_index, port_info_list, port_num):
 
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         tt = (mrt_daq_port_cfg_t*port_num)()
@@ -664,15 +664,15 @@
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         mrt_lib.mrt_stop_daq.argtypes = [c_void_p, c_char_p, c_uint64]
         mrt_lib.mrt_stop_daq.restype = mrt_status_t
         error_code = mrt_lib.mrt_stop_daq(self.context, en_pointer, c_uint64(daq_handle))
         return error_code
 
-    def daq_read(self, env_name, daq_handle, item_count, sub_struct_detail):
+    def daq_read(self, env_name, daq_handle, port_metas):
         info_dir = r'./record_infoFile'
         if not os.path.exists(info_dir):
             os.mkdir(info_dir)
         with open(f"{info_dir}/PortConfig.json", "w") as f:
             f.write(str(self.daqs))
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
@@ -718,17 +718,18 @@
                 data_pba = bytearray(data_byte_arr)
                 p_idx = 0
                 buf_read_idx = 0
                 data_list = []
                 for item in ports:
                     if item is None:
                         continue
-                    item_size = kunyi_util.get_signal_bytes_length(item[3],item_count,sub_struct_detail)
+                    meta = port_metas[item]
+                    item_size = kunyi_util.get_signal_bytes_length(meta["datatype"], meta["item_count"], meta["struct_detail"])
                     item_data_buf = data_pba[buf_read_idx: buf_read_idx+item_size]
-                    item_data_value = kunyi_util.bytes_to_data(item[3], item_data_buf,item_count,sub_struct_detail)
+                    item_data_value = kunyi_util.bytes_to_data(meta["datatype"], item_data_buf, meta["item_count"], meta["struct_detail"])
                     data_list.append((item[0], item[1], item[2], item_data_value, msg.time_stamp_us))
                     buf_read_idx = buf_read_idx + item_size
                     p_idx = p_idx + 1
                 self.data_listTemp = data_list
                 t = msg.time_stamp_us
                 t_bytes = kunyi_util.data_to_bytes("UInt64", t, 1, struct_detail=None)
                 if self.isrecord:
```

### Comparing `vcarhilclient-1.0.608/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.705/vcarhilclient/kunyi_project.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.705/vcarhilclient/kunyi_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,28 @@
 import subprocess
 r=os.path.abspath(os.path.dirname(__file__))
 rootpath= os.path.split(r)[0]
 sys.path.append(rootpath)
 
 from vcarhilclient.Enums import *
 import collections.abc
+from bitstring import BitArray
+
+class can_detail():
+    def __init__(self):
+        self.dlc = 0
+        self.rtr = 0
+        self.fdf = 0
+        self.brs = 0
+        self.ef = 0
+        self.dir = 0
+        self.protocol_id = 0
+        self.id = 0
+        self.extend = 0
+        self.data = b''
 
 class kunyi_util():
     @staticmethod
     def get_signal_bytes_length(signal_type, item_count=1, struct_detail=None, **sub_struct_detail):
         type_dict = {"Int8": 1,
                      "Int16": 2,
                      "Int32": 4,
@@ -41,15 +55,15 @@
                                                                     member["ItemCount"],
                                                                     sub_struct_detail[member["RefStruct"]],
                                                                     **sub_struct_detail)
                     total_length = total_length + sub_length
                 else:
                     sub_length = kunyi_util.get_signal_bytes_length(member["Type"], member["ItemCount"], None)
                     total_length = total_length + sub_length
-            return total_length
+            return total_length * item_count
 
         elif signal_type in type_dict:
             return type_dict[signal_type] * item_count
 
         else:
             raise Exception("Unsupport datatype pass in")
 
@@ -133,15 +147,15 @@
             start_idx = start_idx+move_steps
             value = kunyi_util.bytes_to_data(datatype, temp_array, 1)
             item_data.append(value)
         return item_data
 
 
     @staticmethod
-    def data_to_bytes(datatype, data_value, item_count=1, struct_detail=None, **sub_struct_detail):
+    def data_to_bytes(datatype, data_value, item_count=1, struct_detail=None, bit_order=None, **sub_struct_detail):
         bytes_result = b''
         decode_charactor = {
             "Int8": "b",
             "Int16": "h",
             "Int32": "i",
             "Int64": "q",
             "UInt8": "B",
@@ -198,26 +212,64 @@
                     elif datatype == "UTF8":
                         bytes_result = bytes_result + data_value[mi].encode("utf-8")
                         break
                     else:
                         raise Exception("Unsupportted type for counting the bytes")
             else:
                 value = data_value
-
                 if datatype in decode_charactor:
-                    bytes_result = bytes_result + struct.pack(decode_charactor[datatype], value)
+                    ff_str = decode_charactor[datatype]
+                    if bit_order != None:
+                        format_str = bit_order + decode_charactor[datatype]
+                    bytes_result = bytes_result + struct.pack(ff_str, value)
                 elif datatype == "ASCII":
                     bytes_result = bytes_result + value.encode("ascii")
                 elif datatype == "UTF8":
                     bytes_result = bytes_result + value.encode("utf-8")
                 else:
                     raise Exception("Unsupportted type for counting the bytes")
 
         return bytes_result
 
+    @staticmethod
+    def msg_to_can_detail(data):
+        result = can_detail()
+        flag_bytes = kunyi_util.data_to_bytes("UInt32", data["flags"], 1)
+        aaa = str(flag_bytes.hex())
+        first_byte = BitArray('0x'+ aaa[0:2])
+        dlc_bit = '0000' + first_byte.b[::-1][0:4][::-1]
+        result.dlc = int(dlc_bit, base=2)
+        third_byte = BitArray('0x'+ aaa[4:6])
+        rtr_bit = '0000000' + third_byte.b[::-1][0:1]
+        fdf_bit = '0000000' + third_byte.b[::-1][1:2]
+        brs_bit = '0000000' + third_byte.b[::-1][2:3]
+        ef_bit = '0000000' + third_byte.b[::-1][5:6]
+        dir_bit = '0000000' + third_byte.b[::-1][-1]
+        last_byte = BitArray('0x' + aaa[-2:])
+        pro_id_bit = '0000' + last_byte.b[::-1][-4:]
+        result.rtr = int(rtr_bit, base=2)
+        result.fdf = int(fdf_bit, base=2)
+        result.brs = int(brs_bit, base=2)
+        result.ef = int(ef_bit, base=2)
+        result.dir = int(dir_bit, base=2)
+        result.protocol_id = int(pro_id_bit, base=2)
+
+        id_bytes = kunyi_util.data_to_bytes("UInt32", data["id"], 1, bit_order='>')
+        all_bytes = BitArray('0x'+ str(id_bytes.hex()))
+        id_bit = '000'+ all_bytes.b[-29:]
+        result.id = int(id_bit, base=2)
+        extend_bit = '0000000' + all_bytes.b[-32:31][-1]
+        result.extend = int(extend_bit, base=2)
+        data_sub = data['data'][0:result.dlc]
+        data_bytes = b''
+        for dd in data_sub:
+            data_bytes = data_bytes + kunyi_util.data_to_bytes("UInt8", dd, 1, struct=None, bit_order=None)
+
+        result.data = data_bytes
+        return result
 
 
     @staticmethod
     def file_compress(root_path, out_zip_file):
         import shutil
         shutil.make_archive(out_zip_file, 'zip', root_path)
         return out_zip_file + ".zip"
```

### Comparing `vcarhilclient-1.0.608/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.705/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.705/vcarhilclient/mrt_strunctures.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,8 +50,14 @@
 
 class mrt_gen_port_info_t(Structure):
     _fields_ = [("port_model", c_char*mrt_name_size),
                 ("port_name", c_char*mrt_name_size),
                 ("event_model", c_char*mrt_name_size),
                 ("event_name", c_char*mrt_name_size),
                 ("event_type", c_uint32),
-                ("period_ms", c_uint32)]
+                ("period_ms", c_uint32)]
+
+class drt_can_msg_t(Structure):
+    _fields_ = [("flags", c_uint32), ("id", c_uint32), ("data", c_uint8*64)]
+
+class drt_lin_msg_t(Structure):
+    _fields_ = [("flags", c_uint32), ("id", c_uint32), ("data", c_uint8*8)]
```

### Comparing `vcarhilclient-1.0.608/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.705/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.608/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.705/vcarhilclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.608
+Version: 1.0.705
 Summary: vcarhilclient
 Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

