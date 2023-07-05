# Comparing `tmp/grassmanntn-1.1.2.tar.gz` & `tmp/grassmanntn-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.1.2.tar", last modified: Tue Jul  4 06:52:32 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.3.tar", last modified: Wed Jul  5 06:59:36 2023, max compression
```

## Comparing `grassmanntn-1.1.2.tar` & `grassmanntn-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:52:32.935953 grassmanntn-1.1.2/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.2/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-04 06:52:32.935953 grassmanntn-1.1.2/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.2/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:52:32.935953 grassmanntn-1.1.2/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109338 2023-07-04 06:41:05.000000 grassmanntn-1.1.2/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.2/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132595 2023-07-04 06:45:41.000000 grassmanntn-1.1.2/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.2/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-04 06:52:32.935953 grassmanntn-1.1.2/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-04 06:52:32.000000 grassmanntn-1.1.2/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-04 06:52:32.000000 grassmanntn-1.1.2/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-04 06:52:32.000000 grassmanntn-1.1.2/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-04 06:52:32.000000 grassmanntn-1.1.2/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-04 06:52:32.000000 grassmanntn-1.1.2/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-04 06:52:32.935953 grassmanntn-1.1.2/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-04 06:48:43.000000 grassmanntn-1.1.2/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 06:59:36.390622 grassmanntn-1.1.3/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1.3/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 06:59:36.390622 grassmanntn-1.1.3/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.1.3/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 06:59:36.390622 grassmanntn-1.1.3/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109463 2023-07-05 06:55:21.000000 grassmanntn-1.1.3/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.1.3/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-05 06:56:28.000000 grassmanntn-1.1.3/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1.3/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-05 06:59:36.390622 grassmanntn-1.1.3/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-05 06:59:36.000000 grassmanntn-1.1.3/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-05 06:59:36.000000 grassmanntn-1.1.3/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-05 06:59:36.000000 grassmanntn-1.1.3/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-05 06:59:36.000000 grassmanntn-1.1.3/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-05 06:59:36.000000 grassmanntn-1.1.3/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-05 06:59:36.390622 grassmanntn-1.1.3/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-05 06:59:24.000000 grassmanntn-1.1.3/setup.py
```

### Comparing `grassmanntn-1.1.2/LICENSE.txt` & `grassmanntn-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.2/PKG-INFO` & `grassmanntn-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.2
+Version: 1.1.3
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_112.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_113.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.2/README.md` & `grassmanntn-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.2/grassmanntn/__init__.py` & `grassmanntn-1.1.3/grassmanntn/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,19 +217,19 @@
     return ret
 
 ####################################################
 ##             Densed Grassmann Array             ##
 ####################################################
 
 class dense:
-    def __init__(self, data=None, encoder = "canonical", format = "standard", statistic=None):
+    def __init__(self, data=None, encoder = "canonical", format = "standard", statistics=None):
     
         #copy dense properties
         self.data = None
-        self.statistic = None
+        self.statistics = None
         self.format = format
         self.encoder = encoder
     
         default = True
     
         if(encoder not in encoder_type):
             error("Error[dense]: Unknown encoder.")
@@ -242,41 +242,41 @@
             default = False
         elif(type(data)==sp.COO):
             self.data  = data.todense()
             default = False
         elif(type(data)==sparse):
             #copy dense properties
             self.data = data.data.todense()
-            self.statistic = data.statistic
+            self.statistics = data.statistics
             self.format = data.format
             self.encoder = data.encoder
             default = False
         elif(type(data)==dense):
             #copy dense properties
             self.data = data.data.copy()
-            self.statistic = data.statistic
+            self.statistics = data.statistics
             self.format = data.format
             self.encoder = data.encoder
             default = False
         elif(np.isscalar(data)):
             self.data = np.array(list([data]))
             default = False
         elif(data==None):
             "nothing to see here"
         else:
             error("Error[dense]: Invalid initialized data.")
             
         
-        if statistic != None:
-            self.statistic = make_tuple(statistic)
+        if statistics != None:
+            self.statistics = make_tuple(statistics)
             
         if not default and not skip_power_of_two_check:
             for i,dim in enumerate(self.data.shape):
-                if self.statistic[i] in fermi_type and dim != int(2**math.floor(np.log2(dim))):
-                    error("Error[dense]: Some of the fermionic tensor shapes are not a power of two.\n              Have you added the <statistic> argument when calling this function?")
+                if self.statistics[i] in fermi_type and dim != int(2**math.floor(np.log2(dim))):
+                    error("Error[dense]: Some of the fermionic tensor shapes are not a power of two.\n              Have you added the <statistics> argument when calling this function?")
                 
     def __getitem__(self, index):
         return self.data[index]
     
     def __setitem__(self, index, value):
         self.data[index] = value
         
@@ -315,15 +315,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: dense")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistic:",self.statistic)
+        print(indent+"   statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print(indent+"     entries:")
         iterator = np.nditer(self, flags=['multi_index'])
         for element in iterator:
@@ -340,44 +340,44 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: dense")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistic:",self.statistic)
+        print(indent+"   statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print()
 
     def copy(self):
         #copy dense properties
         ret = dense()
         ret.data = self.data.copy()
-        ret.statistic = self.statistic
+        ret.statistics = self.statistics
         ret.format = self.format
         ret.encoder = self.encoder
         return ret
     
     def __add__(self, other):
         if(self.shape!=other.shape
-            or self.statistic!=other.statistic
+            or self.statistics!=other.statistics
              or self.format!=other.format
               or self.encoder!=other.encoder):
             error("Error[dense.+]: Inconsistent object properties")
             
         ret = self.copy()
         ret.data = ret.data+other.data
         return ret
         
     def __sub__(self, other):
         if(self.shape!=other.shape
-            or self.statistic!=other.statistic
+            or self.statistics!=other.statistics
              or self.format!=other.format
               or self.encoder!=other.encoder):
             error("Error[dense.-]: Inconsistent object properties")
             
         ret = self.copy()
         ret.data = ret.data-other.data
         return ret
@@ -412,16 +412,16 @@
             ret = self
         else:
             ret = self.copy()
         if(self.encoder=='parity-preserving'):
             ret = ret.switch_encoder(save_memory=True)
         to_calc = []
         for i in range(self.ndim):
-            to_calc += (ret.statistic[i]==-1),
-            if(ret.statistic[i]==hybrid_symbol):
+            to_calc += (ret.statistics[i]==-1),
+            if(ret.statistics[i]==hybrid_symbol):
                 error("Error[switch_format]: Cannot switch format with a hybrid index.\n                      Split them into bosonic and fermionic ones first!")
         
         k=0
         kmax = ret.ndim
         s0 = time.time()
         s00 = s0
         progress_space()
@@ -470,15 +470,15 @@
         s0 = time.time()
         s00 = s0
         progress_space()
 
         dat = ret.data
         for axis in range(ret.ndim):
             d = ret.shape[axis]
-            if ret.statistic[axis] in fermi_type :
+            if ret.statistics[axis] in fermi_type :
                 dat = dat.take(indices=np.array([param.encoder(i) for i in range(d)]),axis=axis)
 
             if time.time()-s0 > 2 :
                 show_progress(axis,kmax,process_name = "switch_encoder",ratio = False,color="cyan",time=time.time()-s00)
                 s0 = time.time()
             
         clear_progress()
@@ -524,19 +524,19 @@
         return eig(self,string_inp,cutoff,debug_mode,save_memory)
 
 ####################################################
 ##            Sparse Grassmann arrays             ##
 ####################################################
 
 class sparse:
-    def __init__(self, data=None, encoder = "canonical", format = "standard", statistic = None):
+    def __init__(self, data=None, encoder = "canonical", format = "standard", statistics = None):
     
         #copy sparse properties
         self.data = None
-        self.statistic = None
+        self.statistics = None
         self.format = format
         self.encoder = encoder
 
         default = True
     
         if(encoder not in encoder_type):
             error("Error[sparse]: Unknown encoder.")
@@ -549,38 +549,38 @@
             default = False
         elif(type(data)==sp.COO):
             self.data  = data.copy()
             default = False
         elif(type(data)==dense):
             #copy sparse properties
             self.data  = sp.COO.from_numpy(data.data)
-            self.statistic = data.statistic
+            self.statistics = data.statistics
             self.format = data.format
             self.encoder = data.encoder
             default = False
         elif(type(data)==sparse):
             #copy sparse properties
             self.data = data.data.copy()
-            self.statistic = data.statistic
+            self.statistics = data.statistics
             self.format = data.format
             self.encoder = data.encoder
             default = False
         elif data==None:
             "nothing to see here"
         else:
             error("Error[sparse]: Invalid initialized data")
             
         
-        if statistic != None:
-            self.statistic = make_tuple(statistic)
+        if statistics != None:
+            self.statistics = make_tuple(statistics)
         
         if not default and not skip_power_of_two_check:
             for i,dim in enumerate(self.data.shape):
-                if self.statistic[i] in fermi_type and dim != int(2**math.floor(np.log2(dim))):
-                    error("Error[sparse]: Some of the fermionic tensor shapes are not a power of two.\n               Have you added the <statistic> argument when calling this function?")
+                if self.statistics[i] in fermi_type and dim != int(2**math.floor(np.log2(dim))):
+                    error("Error[sparse]: Some of the fermionic tensor shapes are not a power of two.\n               Have you added the <statistics> argument when calling this function?")
                
     @property
     def nnz(self):
         return self.data.nnz
 
     @property
     def shape(self):
@@ -624,15 +624,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: sparse")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistic:",self.statistic)
+        print(indent+"   statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print(indent+"     entries:")
 
         C = self.coords
@@ -650,15 +650,15 @@
 
         print()
         if name != None:
             print(indent+"        name:",name)
         print(indent+"  array type: sparse")
         print(indent+"       shape:",self.shape)
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
-        print(indent+"   statistic:",self.statistic)
+        print(indent+"   statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print()
 
     def set_value(self,entry,value):
@@ -695,33 +695,33 @@
             ret.remove_entry(zero_entry-i)
         return ret
 
     def copy(self):
         #copy sparse properties
         ret = sparse()
         ret.data = self.data.copy()
-        ret.statistic = self.statistic
+        ret.statistics = self.statistics
         ret.format = self.format
         ret.encoder = self.encoder
         return ret
     
     def __add__(self, other):
         if(self.shape!=other.shape
-            or self.statistic!=other.statistic
+            or self.statistics!=other.statistics
              or self.format!=other.format
               or self.encoder!=other.encoder):
             error("Error[sparse.+]: Inconsistent object properties")
             
         ret = self.copy()
         ret.data = ret.data+other.data
         return ret
         
     def __sub__(self, other):
         if(self.shape!=other.shape
-            or self.statistic!=other.statistic
+            or self.statistics!=other.statistics
              or self.format!=other.format
               or self.encoder!=other.encoder):
             error("Error[sparse.-]: Inconsistent object properties")
             
         ret = self.copy()
         ret.data = ret.data-other.data
         return ret
@@ -998,15 +998,15 @@
 
     summand = input_string.replace(",","")
 
     obj_index_list = input_string.split(",")
     nobj = len(obj_index_list)
 
     obj_list = make_list(args[1:1+nobj])
-    stats_list = sum([ make_list(obj.statistic) for obj in obj_list ],[])
+    stats_list = sum([ make_list(obj.statistics) for obj in obj_list ],[])
     shape_list = sum([ make_list(obj.shape) for obj in obj_list ],[])
 
     # force everything to be canonical and standard -------------------------------------------------
     # also force everything to be of the same type
 
     this_type = type(obj_list[0])
     this_encoder = obj_list[0].encoder
@@ -1062,15 +1062,15 @@
         elif [stat1,stat2] == [hybrid_symbol,hybrid_symbol]:
             return False
         else:
             return True
 
     for [char,location,stats] in summed_index_info:
         if len(stats)==2 and is_statwise_inconsistent(stats[0],stats[1]):
-            error("Error[einsum]: The contracted indices have inconsistent statistic!")
+            error("Error[einsum]: The contracted indices have inconsistent statistics!")
     
     if debug_mode :
         print()
         print("input:",instruction_string)
         print("obj indices:")
         for elem in obj_index_list:
             print(" ",elem)
@@ -1614,15 +1614,15 @@
         for obj in einsum_obj_list:
             print(" ",[obj.shape,type(obj)])
 
             
     ret = oe.contract(*tuple([einsum_string]+einsum_obj_list))
 
     if has_output :
-        return this_type(ret,statistic=final_stats).force_encoder(this_encoder).force_format(this_format)
+        return this_type(ret,statistics=final_stats).force_encoder(this_encoder).force_format(this_format)
     else:
         if this_type == sparse :
             if type(ret.data)==memoryview:
                 return ret
             else:
                 return ret.data[0]
         else:
@@ -1651,15 +1651,15 @@
     #   Step 0: Preconditioning the initial Object to standard & canonical          #
     #===============================================================================#
     
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
-    XObj_stats = Obj.statistic
+    XObj_stats = Obj.statistics
     XObj_shape = Obj.shape
 
     if save_memory :
         del InpObj.data
         del InpObj
         gc.collect()
         
@@ -1674,15 +1674,15 @@
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 1: Move bosonic indices to the left of each group                      #
     #===============================================================================#
     
     # get the grouping info first
-    group_info, sorted_group_info = get_group_info(string_inp, Obj.statistic, Obj.shape)
+    group_info, sorted_group_info = get_group_info(string_inp, Obj.statistics, Obj.shape)
     #group_info contains the index_string, statistics, and shape of each group
     #sorted_group_info is the same, but with bosonic indices sorted to the left
     
     n_indices = sum([ len(indices) for [indices,stats,shape] in group_info ])
     
     if n_indices != Obj.ndim :
         error("Error[join_legs]: The number of indices is not consistent with the object's shape.")
@@ -1696,27 +1696,27 @@
     
     sorted_stat = make_tuple(sum(
             [ make_list(stats) for [indices, stats, shape] in sorted_group_info ] ,[]
         ))
     
     #sorted tensor
     Obj.data = oe.contract(*make_tuple( [npeinsum_string] + npeinsum_obj ))
-    Obj.statistic = sorted_stat
+    Obj.statistics = sorted_stat
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     
     #===============================================================================#
     #   Step 2: Join fermionic indices with np.reshape                              #
     #===============================================================================#
     
     new_stats, new_shape, final_stats, final_shape = get_intermediate_info(sorted_group_info,intermediate_stat)
     #intermediate_tensor
     
     Obj.data = np.reshape(Obj.data,new_shape)
-    Obj.statistic = new_stats
+    Obj.statistics = new_stats
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 3: Switch format if make_format='matrix'                               #
     #===============================================================================#
     
     if make_format == 'matrix':
@@ -1731,15 +1731,15 @@
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 5: Merge bosons and fermions                                           #
     #===============================================================================#
     
     Obj.data = np.reshape(Obj.data,final_shape)
-    Obj.statistic = final_stats
+    Obj.statistics = final_stats
     
     clear_progress()
     tab_up()
 
     return Obj
     
 def split_legs(InpObj,string_inp,final_stat,final_shape,intermediate_stat=(-1,1),save_memory=False):
@@ -1762,15 +1762,15 @@
     #   Step 0: Preparation                                                         #
     #===============================================================================#
     
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
-    XObj_stats = Obj.statistic
+    XObj_stats = Obj.statistics
     XObj_shape = Obj.shape
 
     if save_memory :
         del InpObj.data
         del InpObj
         gc.collect()
 
@@ -1780,15 +1780,15 @@
     #===============================================================================#
     
     group_info, sorted_group_info = get_group_info(string_inp, final_stat, final_shape)
     new_stats, new_shape, _, _ = get_intermediate_info(sorted_group_info,intermediate_stat)
     sign_factors_list = get_grouping_sign_factors(sorted_group_info, intermediate_stat)
     
     Obj.data = np.reshape(Obj.data,new_shape)
-    Obj.statistic = new_stats
+    Obj.statistics = new_stats
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 4: Switch encoder                                                      #
     #===============================================================================#
     
     Obj = Obj.switch_encoder(save_memory=True)
@@ -1811,27 +1811,27 @@
     for [indices,stats,shape] in sorted_group_info:
         new_stats += make_list(stats)
         new_shape += make_list(shape)
     new_stats = make_tuple(new_stats)
     new_shape = make_tuple(new_shape)
     
     Obj.data = np.reshape(Obj.data,new_shape)
-    Obj.statistic = new_stats
+    Obj.statistics = new_stats
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #===============================================================================#
     #   Step 1: Move bosonic indices to the left of each group                      #
     #===============================================================================#
     
     unsorted_string = ''.join( [ indices for [indices, stats, shape] in group_info ] )
     sorted_string = ''.join( [ indices for [indices, stats, shape] in sorted_group_info ] )
     npeinsum_string = sorted_string+sign_factors_list[0]+"->"+unsorted_string
     npeinsum_obj = [Obj.data] + sign_factors_list[1]
     Obj.data = oe.contract(*make_tuple( [npeinsum_string] + npeinsum_obj ))
-    Obj.statistic = final_stat
+    Obj.statistics = final_stat
     
     clear_progress()
     tab_up()
 
     if this_format=='matrix':
         return Obj.switch_format(save_memory=True)
     
@@ -1852,15 +1852,15 @@
         for separator in separator_list:
             separator_count += formatted_string.count(separator)
         if separator_count > 0 :
             error("Error[get_grouping_info]: Do not mix the string format.")
     #print("formatted string:",formatted_string)
     
     # parse the string ---------------------------------------------------------------
-    group_info = [] # [string text, statistic, shape]
+    group_info = [] # [string text, statistics, shape]
     is_outside = True
     location = 0
     for char in formatted_string:
         if char == "(" and is_outside :
             is_outside = False
             group_info += [
                 [ "", [], [] ] #make a blank template for this group
@@ -1998,15 +1998,15 @@
         Obj = sparse(Obj)
     C = Obj.coords
     s0 = time.time()
     s00 = s0
     progress_space() # << Don't remove this. This is for the show_progress!
 
     for i in range(Obj.nnz):
-        fcoords = [ ind for j,ind in enumerate(C[i]) if (Obj.statistic[j] in fermi_type)]
+        fcoords = [ ind for j,ind in enumerate(C[i]) if (Obj.statistics[j] in fermi_type)]
         if(sum(fcoords)%2 == 1):
             Obj.data.data[i] = 0
 
         if time.time()-s0 > 0.5 :
             show_progress(i,Obj.nnz,"trim_grassmann_odd",time=time.time()-s00)
 
     clear_progress()
@@ -2025,15 +2025,15 @@
     if Obj.encoder == 'canonical':
         Obj = Obj.switch_encoder(save_memory=True)
     if type(Obj) == dense:
         Obj = sparse(Obj)
 
     C = Obj.coords
     for x in C:
-        parity = sum([ ind for i,ind in enumerate(x) if Obj.statistic[i] in fermi_type ])
+        parity = sum([ ind for i,ind in enumerate(x) if Obj.statistics[i] in fermi_type ])
         if parity%2!=0 :
             return False
     return True
 
 ####################################################
 ##          Singular value decomposition          ##
 ####################################################
@@ -2156,32 +2156,32 @@
     string = denumerate(string)
 
     
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
-    XObj_stats = Obj.statistic
+    XObj_stats = Obj.statistics
     XObj_shape = Obj.shape
 
     if save_memory :
         del InpObj.data
         del InpObj
         gc.collect()
         
         
     if(this_type==sparse):
         Obj = dense(Obj)
     if(this_type not in [dense,sparse]):
         error("Error[svd]: Object type must only be dense or sparse!")
         
-    # check if Obj.statistic or final_statistic is weird or not
-    for stat in Obj.statistic:
+    # check if Obj.statistics or final_statistics is weird or not
+    for stat in Obj.statistics:
         if(stat not in allowed_stat):
-            error("Error[svd]: The input object contains illegal statistic. (0, 1, -1, or "+hybrid_symbol+" only)")
+            error("Error[svd]: The input object contains illegal statistics. (0, 1, -1, or "+hybrid_symbol+" only)")
 
     if string.count("(")==string.count(")") and string.count("(")>0:
         string = string.replace(" ","")
         string = string.replace(")("," ")
         if string.count("(")>1 or string.count(")")<1:
             error("Error[svd]: Parentheses don't match")
         string = string.replace(")","")
@@ -2227,17 +2227,17 @@
 
     join_legs_string_input = string
     for partition in separator_list:
         join_legs_string_input = join_legs_string_input.replace(partition,")(")
     join_legs_string_input = "("+join_legs_string_input+")"
 
     shape_left  = Obj.shape[:n_left]
-    stats_left  = Obj.statistic[:n_left]
+    stats_left  = Obj.statistics[:n_left]
     shape_right = Obj.shape[n_left:]
-    stats_right = Obj.statistic[n_left:]
+    stats_right = Obj.statistics[n_left:]
 
     def zero_or_else(vector,value):
         for elem in vector:
             if elem!=0:
                 return value
         return 0
     def get_stat(vector,prefer=None):
@@ -2268,15 +2268,15 @@
     Obj = Obj.join_legs(join_legs_string_input,"matrix",intermediate_stat=intermediate_stat,save_memory=True)
 
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 2 - BLOCK SVD (MAKE SURE IT'S PARITY-PRESERVING!)                          :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #3
-    if Obj.statistic[0]==0 or Obj.statistic[1]==0:
+    if Obj.statistics[0]==0 or Obj.statistics[1]==0:
         U, Λ, V = SortedSVD(Obj.data,cutoff)
         Λ = np.diag(Λ)
     else:
         U, Λ, V = BlockSVD(Obj.data,cutoff)
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #4
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
@@ -2285,30 +2285,30 @@
 
     skip_power_of_two_check = True
 
     #the first way is to form the tensor first, then split
     Λstatleft = -1
     Λstatright = +1
     
-    if Obj.statistic[0]==0:
-        U = dense(U,encoder="parity-preserving",format="matrix",statistic=(0,0))
-        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistic=(0,0))
-        V = dense(V,encoder="parity-preserving",format="matrix",statistic=(0,Obj.statistic[1]))
+    if Obj.statistics[0]==0:
+        U = dense(U,encoder="parity-preserving",format="matrix",statistics=(0,0))
+        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistics=(0,0))
+        V = dense(V,encoder="parity-preserving",format="matrix",statistics=(0,Obj.statistics[1]))
         Λstatleft = 0
         Λstatright = 0
-    elif Obj.statistic[1]==0:
-        U = dense(U,encoder="parity-preserving",format="matrix",statistic=(Obj.statistic[0],0))
-        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistic=(0,0))
-        V = dense(V,encoder="parity-preserving",format="matrix",statistic=(0,0))
+    elif Obj.statistics[1]==0:
+        U = dense(U,encoder="parity-preserving",format="matrix",statistics=(Obj.statistics[0],0))
+        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistics=(0,0))
+        V = dense(V,encoder="parity-preserving",format="matrix",statistics=(0,0))
         Λstatleft = 0
         Λstatright = 0
     else:
-        U = dense(U,encoder="parity-preserving",format="matrix",statistic=(Obj.statistic[0],1))
-        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistic=(-1,1))
-        V = dense(V,encoder="parity-preserving",format="matrix",statistic=(-1,Obj.statistic[1]))
+        U = dense(U,encoder="parity-preserving",format="matrix",statistics=(Obj.statistics[0],1))
+        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistics=(-1,1))
+        V = dense(V,encoder="parity-preserving",format="matrix",statistics=(-1,Obj.statistics[1]))
     dΛ = Λ.shape[0]
 
     skip_power_of_two_check = False
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #5
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 4 - Split the legs                                                         :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
@@ -2500,32 +2500,32 @@
     string = denumerate(string)
 
     
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
-    XObj_stats = Obj.statistic
+    XObj_stats = Obj.statistics
     XObj_shape = Obj.shape
 
     if save_memory :
         del InpObj.data
         del InpObj
         gc.collect()
         
         
     if(this_type==sparse):
         Obj = dense(Obj)
     if(this_type not in [dense,sparse]):
         error("Error[eig]: Object type must only be dense or sparse!")
         
-    # check if Obj.statistic or final_statistic is weird or not
-    for stat in Obj.statistic:
+    # check if Obj.statistics or final_statistics is weird or not
+    for stat in Obj.statistics:
         if(stat not in allowed_stat):
-            error("Error[eig]: The input object contains illegal statistic. (0, 1, -1, or "+hybrid_symbol+" only)")
+            error("Error[eig]: The input object contains illegal statistics. (0, 1, -1, or "+hybrid_symbol+" only)")
 
     if string.count("(")==string.count(")") and string.count("(")>0:
         string = string.replace(" ","")
         string = string.replace(")("," ")
         if string.count("(")>1 or string.count(")")<1:
             error("Error[eig]: Parentheses don't match")
         string = string.replace(")","")
@@ -2571,17 +2571,17 @@
 
     join_legs_string_input = string
     for partition in separator_list:
         join_legs_string_input = join_legs_string_input.replace(partition,")(")
     join_legs_string_input = "("+join_legs_string_input+")"
 
     shape_left  = Obj.shape[:n_left]
-    stats_left  = Obj.statistic[:n_left]
+    stats_left  = Obj.statistics[:n_left]
     shape_right = Obj.shape[n_left:]
-    stats_right = Obj.statistic[n_left:]
+    stats_right = Obj.statistics[n_left:]
 
     def zero_or_else(vector,value):
         for elem in vector:
             if elem!=0:
                 return value
         return 0
     def get_stat(vector,prefer=None):
@@ -2611,15 +2611,15 @@
     Obj = Obj.join_legs(join_legs_string_input,"matrix",intermediate_stat=intermediate_stat,save_memory=True)
 
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 2 - BLOCK SVD (MAKE SURE IT'S PARITY-PRESERVING!)                          :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #3
-    if Obj.statistic[0]==0 or Obj.statistic[1]==0:
+    if Obj.statistics[0]==0 or Obj.statistics[1]==0:
         U, Λ, V = SortedEig(Obj.data,cutoff,debug_mode)
         Λ = np.diag(Λ)
     else:
         U, Λ, V = BlockEig(Obj.data,cutoff,debug_mode)
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #4
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
@@ -2628,30 +2628,30 @@
 
     skip_power_of_two_check = True
 
     #the first way is to form the tensor first, then split
     Λstatleft = -1
     Λstatright = +1
     
-    if Obj.statistic[0]==0:
-        U = dense(U,encoder="parity-preserving",format="matrix",statistic=(0,0))
-        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistic=(0,0))
-        V = dense(V,encoder="parity-preserving",format="matrix",statistic=(0,Obj.statistic[1]))
+    if Obj.statistics[0]==0:
+        U = dense(U,encoder="parity-preserving",format="matrix",statistics=(0,0))
+        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistics=(0,0))
+        V = dense(V,encoder="parity-preserving",format="matrix",statistics=(0,Obj.statistics[1]))
         Λstatleft = 0
         Λstatright = 0
-    elif Obj.statistic[1]==0:
-        U = dense(U,encoder="parity-preserving",format="matrix",statistic=(Obj.statistic[0],0))
-        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistic=(0,0))
-        V = dense(V,encoder="parity-preserving",format="matrix",statistic=(0,0))
+    elif Obj.statistics[1]==0:
+        U = dense(U,encoder="parity-preserving",format="matrix",statistics=(Obj.statistics[0],0))
+        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistics=(0,0))
+        V = dense(V,encoder="parity-preserving",format="matrix",statistics=(0,0))
         Λstatleft = 0
         Λstatright = 0
     else:
-        U = dense(U,encoder="parity-preserving",format="matrix",statistic=(Obj.statistic[0],1))
-        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistic=(-1,1))
-        V = dense(V,encoder="parity-preserving",format="matrix",statistic=(-1,Obj.statistic[1]))
+        U = dense(U,encoder="parity-preserving",format="matrix",statistics=(Obj.statistics[0],1))
+        Λ = dense(Λ,encoder="parity-preserving",format="matrix",statistics=(-1,1))
+        V = dense(V,encoder="parity-preserving",format="matrix",statistics=(-1,Obj.statistics[1]))
     dΛ = Λ.shape[0]
 
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00) #5
     skip_power_of_two_check = False
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 4 - Split the legs                                                         :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
@@ -2741,31 +2741,31 @@
 
     # the string is of the form aaaa|bbb
 
     Obj = InpObj.copy()
     this_type = type(Obj)
     this_format = Obj.format
     this_encoder = Obj.encoder
-    XObj_stats = Obj.statistic
+    XObj_stats = Obj.statistics
     XObj_shape = Obj.shape
 
     if save_memory :
         del InpObj.data
         del InpObj
         gc.collect()
 
     #if this_type==sparse :
     #    Obj = dense(Obj)
     if this_type not in [dense,sparse] :
         error("Error[hconjugate]: Object type must only be dense or sparse!")
         
-    # check if Obj.statistic or final_statistic is weird or not
-    for stat in Obj.statistic:
+    # check if Obj.statistics or final_statistics is weird or not
+    for stat in Obj.statistics:
         if(stat not in allowed_stat):
-            error("Error[hconjugate]: The input object contains illegal statistic. (0, 1, -1, or "+hybrid_symbol+" only)")
+            error("Error[hconjugate]: The input object contains illegal statistics. (0, 1, -1, or "+hybrid_symbol+" only)")
             
     partition_count = 0
     for partition in separator_list:
         partition_count += string.count(partition)
     if(partition_count!=1):
         partition_string = ""
         for i, partition in enumerate(separator_list):
@@ -2803,17 +2803,17 @@
 
     join_legs_string_input = string
     for partition in separator_list:
         join_legs_string_input = join_legs_string_input.replace(partition,")(")
     join_legs_string_input = "("+join_legs_string_input+")"
 
     shape_left  = Obj.shape[:n_left]
-    stats_left  = Obj.statistic[:n_left]
+    stats_left  = Obj.statistics[:n_left]
     shape_right = Obj.shape[n_left:]
-    stats_right = Obj.statistic[n_left:]
+    stats_right = Obj.statistics[n_left:]
     def prod(vector):
         ret = 1
         for elem in vector:
             ret *= elem
         return ret
     def get_stat(vector,prefer=None):
         boson_count = 0
@@ -2844,27 +2844,27 @@
     #:::::      STEP 2 - Perform Hermitian Conjugation                                          :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
     Obj.data = np.conjugate(oe.contract('ij->ji',Obj.data))
     
     new_stat = [1,1]
     
-    if Obj.statistic[0] in fermi_type :
-        new_stat[1] = -Obj.statistic[0]
+    if Obj.statistics[0] in fermi_type :
+        new_stat[1] = -Obj.statistics[0]
     else:
-        new_stat[1] = Obj.statistic[0]
+        new_stat[1] = Obj.statistics[0]
         
-    if Obj.statistic[1] in fermi_type :
-        new_stat[0] = -Obj.statistic[1]
+    if Obj.statistics[1] in fermi_type :
+        new_stat[0] = -Obj.statistics[1]
     else:
-        new_stat[0] = Obj.statistic[1]
+        new_stat[0] = Obj.statistics[1]
     
     new_stat = make_tuple(new_stat)
     
-    Obj.statistic = new_stat
+    Obj.statistics = new_stat
     
     step = show_progress(step,process_length,process_name+" "+"<"+current_memory_display()+">",color=process_color,time=time.time()-s00)
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     #:::::      STEP 3 - Split legs                                                             :::::
     #::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
     
     
@@ -2911,19 +2911,19 @@
 
     return Obj
 
 ####################################################
 ##                    Utilities                   ##
 ####################################################
 
-def random(shape,statistic,tensor_format=dense,dtype=float,skip_trimming=False):
+def random(shape,statistics,tensor_format=dense,dtype=float,skip_trimming=False):
     X = np.random.rand(*shape)
     if dtype == complex :
         X = complex(1,0)*X + complex(0,1)*np.random.rand(*shape)
-    A = dense(X, statistic = statistic)
+    A = dense(X, statistics = statistics)
     if not skip_trimming:
         A = trim_grassmann_odd(A)
     if tensor_format==sparse:
         A = sparse(A)
         A = A.remove_zeros()
     return A
```

### Comparing `grassmanntn-1.1.2/grassmanntn/example.py` & `grassmanntn-1.1.3/grassmanntn/example.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.2/grassmanntn/gauge2d.py` & `grassmanntn-1.1.3/grassmanntn/gauge2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if not mute:
         print("                             T formation: "+gtn.time_display(time.time()-t0))
 
     t0 = time.time()
     T = compress_T(T)
     if not mute:
         print("                           T compression: "+gtn.time_display(time.time()-t0))
-    z4 = gtn.einsum("IJIJij,ij",T,gtn.sparse(np.full((Nphi,Nphi),1),statistic=(0,0)))
+    z4 = gtn.einsum("IJIJij,ij",T,gtn.sparse(np.full((Nphi,Nphi),1),statistics=(0,0)))
 
     trace_error = np.abs(1-z4/z1)
     if not mute:
         print("                       Compression error:",trace_error)
         T.info("Compressed tensor T",21)
 
     T = gtn.dense(T)
@@ -998,17 +998,17 @@
                     B+=[(-1/4 + cI/4)*np.exp((-cI)*p1*charge - cI*q1*charge - spacing*mu)]  #446
                     psi1+=[9]; psi2+=[10]; psi3+=[0]; psi4+=[0]; phi1+=[i]; phi2+=[j]; phi3+=[k]; phi4+=[l]
                     B+=[(1/4 - cI/4)*np.exp((-cI)*p1*charge - cI*q1*charge - spacing*mu)]  #447
                     psi1+=[10]; psi2+=[9]; psi3+=[0]; psi4+=[0]; phi1+=[i]; phi2+=[j]; phi3+=[k]; phi4+=[l]
                     B+=[(-1/4 + cI/4)*np.exp((-cI)*p1*charge - cI*q1*charge - spacing*mu)]  #448
                     psi1+=[8]; psi2+=[11]; psi3+=[0]; psi4+=[0]; phi1+=[i]; phi2+=[j]; phi3+=[k]; phi4+=[l]
                     B+=[(-1/4 + cI/4)*np.exp((-cI)*p1*charge - cI*q1*charge - spacing*mu)]  #449
-    A = gtn.sparse(A, statistic=(0,0,0,0))
+    A = gtn.sparse(A, statistics=(0,0,0,0))
     B = sp.COO([psi1,psi2,psi3,psi4,phi1,phi2,phi3,phi4], B, shape=(Npsi,Npsi,Npsi,Npsi,Nphi,Nphi,Nphi,Nphi))
-    B = gtn.sparse(B, statistic=(1,1,-1,-1,0,0,0,0))
+    B = gtn.sparse(B, statistics=(1,1,-1,-1,0,0,0,0))
 
     return A, B
 
 def fcompress_B(B,cutoff=64,mute=True):
 
     process_name = "B compression (1)"
     process_length = 16
@@ -1111,15 +1111,15 @@
     gtn.progress_space()
 
     Npsi = B.shape[0]
     Nphi = B.shape[4]
     δ = np.zeros([Nphi,Nphi],dtype=int)
     for i in range(Nphi):
         δ[i,i] = 1
-    δ = gtn.sparse(δ,statistic=(0,0))
+    δ = gtn.sparse(δ,statistics=(0,0))
 
     if not mute:
         B.info("B (uncompressed)")
 
     # μ = 1 ===========================================================================
 
     step = 1
@@ -1288,15 +1288,15 @@
     s00 = time.time()
     gtn.progress_space()
 
     Nphi = A.shape[0]
     δ = np.zeros([Nphi,Nphi],dtype=int)
     for i in range(Nphi):
         δ[i,i] = 1
-    δ = gtn.sparse(δ,statistic=(0,0))
+    δ = gtn.sparse(δ,statistics=(0,0))
 
     if not mute:
         A.info("A (uncompressed)")
 
     step = 1
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Ix = gtn.einsum('KXj,XjI->KIj',U1.hconjugate('ij k'),U3)
@@ -1400,17 +1400,17 @@
 ####################################################
 ##               2D Coarse graining               ##
 ####################################################
 
 def zcap(T):
     Nphi = T.shape[4]
     if type(T)==gtn.dense :
-        capper = gtn.dense(np.full((Nphi,Nphi),1),statistic=(0,0))
+        capper = gtn.dense(np.full((Nphi,Nphi),1),statistics=(0,0))
     else :
-        capper = gtn.sparse(np.full((Nphi,Nphi),1),statistic=(0,0))
+        capper = gtn.sparse(np.full((Nphi,Nphi),1),statistics=(0,0))
     return gtn.einsum("IJKLij,ij->IJKL",T,capper)
 
 def logZ(T,boundary_conditions='periodic'):
     
     if type(T) == gtn.sparse:
         T = gtn.dense(T)
         if T.encoder == 'parity-preserving':
@@ -1457,21 +1457,21 @@
 ##                       TRG                      ##
 ####################################################
 
 def trg(T,dcut=16):
 
     # mandatory properties of T:
     #    - shape = (nx,ny,nx,ny)
-    #    - statistic = (1,1,-1,-1)
+    #    - statistics = (1,1,-1,-1)
 
     if [T.shape[0],T.shape[1]] != [T.shape[2],T.shape[3]] :
         error("Error[trg]: The shape must be of the form (m,n,m,n)!")
 
-    if make_list(T.statistic) != [1,1,-1,-1] :
-        error("Error[trg]: The statistic must be (1,1,-1,-1)!")
+    if make_list(T.statistics) != [1,1,-1,-1] :
+        error("Error[trg]: The statistics must be (1,1,-1,-1)!")
 
     #===============================================================================#
     #   Step 1: Rearrange the tensor legs in two ways                               #
     #===============================================================================#
     
     T1 = gtn.einsum('ijkl->jkli',T)
     T2 = gtn.einsum('ijkl->klij',T)
```

### Comparing `grassmanntn-1.1.2/grassmanntn/param.py` & `grassmanntn-1.1.3/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.1.2/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1.3/grassmanntn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.1.2
+Version: 1.1.3
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_112.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_113.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.1.2/setup.py` & `grassmanntn-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.1.2',      # Start with a small number and increase it with every change you make
+  version = '1.1.3',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_112.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_113.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

