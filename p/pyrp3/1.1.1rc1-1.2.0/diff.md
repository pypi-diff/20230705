# Comparing `tmp/pyrp3-1.1.1rc1.tar.gz` & `tmp/pyrp3-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrp3-1.1.1rc1.tar", last modified: Wed Mar 29 12:06:35 2023, max compression
+gzip compressed data, was "pyrp3-1.2.0.tar", last modified: Wed Jul  5 11:41:27 2023, max compression
```

## Comparing `pyrp3-1.1.1rc1.tar` & `pyrp3-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/monitor/monitor.c
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/pyrp3/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/board.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/client_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/pyrp3/enum/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/enum/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    18871 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/pc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/raw_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/pyrp3/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/pyrp3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-29 12:06:35.000000 pyrp3-1.1.1rc1/pyrp3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-29 12:06:35.000000 pyrp3-1.1.1rc1/pyrp3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:06:35.000000 pyrp3-1.1.1rc1/pyrp3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-29 12:06:35.000000 pyrp3-1.1.1rc1/pyrp3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 12:06:35.000000 pyrp3-1.1.1rc1/pyrp3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 12:06:35.141113 pyrp3-1.1.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-29 12:06:29.000000 pyrp3-1.1.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:41:27.657936 pyrp3-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-05 11:41:21.000000 pyrp3-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-05 11:41:27.657936 pyrp3-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-05 11:41:21.000000 pyrp3-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:41:27.657936 pyrp3-1.2.0/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-05 11:41:21.000000 pyrp3-1.2.0/monitor/monitor.c
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:41:27.657936 pyrp3-1.2.0/pyrp3/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/client_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18272 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/raw_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 11:41:21.000000 pyrp3-1.2.0/pyrp3/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:41:27.657936 pyrp3-1.2.0/pyrp3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-05 11:41:27.000000 pyrp3-1.2.0/pyrp3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-05 11:41:27.000000 pyrp3-1.2.0/pyrp3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:41:27.000000 pyrp3-1.2.0/pyrp3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 11:41:27.000000 pyrp3-1.2.0/pyrp3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 11:41:27.000000 pyrp3-1.2.0/pyrp3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:41:27.657936 pyrp3-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-05 11:41:21.000000 pyrp3-1.2.0/setup.py
```

### Comparing `pyrp3-1.1.1rc1/LICENSE` & `pyrp3-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrp3-1.1.1rc1/PKG-INFO` & `pyrp3-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrp3
-Version: 1.1.1rc1
+Version: 1.2.0
 Summary: Python utilities for redpitaya
 Author: Pierre Cladé
 Author-email: pierre.clade@upmc.fr
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Keywords: redpitaya,FPGA,zynq
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pyrp3
 =======
 Python 3 port (using 2to3) of `PyRedPitaya <https://github.com/clade/PyRedPitaya>`_ library in the `pyrp3` namespace.
```

### Comparing `pyrp3-1.1.1rc1/README.rst` & `pyrp3-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyrp3-1.1.1rc1/monitor/monitor.c` & `pyrp3-1.2.0/monitor/monitor.c`

 * *Files identical despite different names*

### Comparing `pyrp3-1.1.1rc1/pyrp3/client_memory.py` & `pyrp3-1.2.0/pyrp3/client_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-class ClientMemory(object):
+class ClientMemory:
     def __init__(self, remote_connection):
         self.remote_connection = remote_connection
         self.remote_interface = remote_connection.root.mem()
 
     def read(self, addr):
         return self.remote_interface.read(addr)
```

### Comparing `pyrp3-1.1.1rc1/pyrp3/instrument.py` & `pyrp3-1.2.0/pyrp3/instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import numpy as np
 from myhdl import intbv
 
 from .enum import Enum
 from .memory import MemoryInterface
 
 
-class UnsignedInteger(object):
+class UnsignedInteger:
     def __init__(self, size):
         self.size = size
 
     def to_python(self, val):
         return int(val & (2**self.size - 1))
 
     def to_binary(self, val):
         return intbv(val, max=2**self.size, min=0)._val
 
 
-class SignedInteger(object):
+class SignedInteger:
     def __init__(self, size):
         self.size = size
 
     def to_python(self, val):
         return int(
             intbv(val & (2**self.size - 1), min=0, max=2**self.size).signed()
         )
@@ -32,15 +32,14 @@
             self.size :
         ]._val
 
 
 class EnumTypeWrapper(UnsignedInteger):
     def __init__(self, enum_type):
         self._enum_type = enum_type
-        maximum = max(self._enum_type._reverse_dct.keys())
         size = int(ceil(log(16, 2)))
         super(EnumTypeWrapper, self).__init__(size=size)
 
     def to_python(self, val):
         raw = super(EnumTypeWrapper, self).to_python(val)
         return self._enum_type(raw)
 
@@ -86,15 +85,15 @@
         out = intbv(0, min=0, max=2**32)
         tmp = np.long(np.round(val * (17 * 157 - 1)))
         out[32:16] = tmp // 17
         out[16:0] = 2**tmp % 17 - 1
         return out[32:]._val
 
 
-class RegisterProperty(object):
+class RegisterProperty:
     def __init__(self, addr, register_type, size=None):
         if isinstance(register_type, type) and issubclass(register_type, Enum):
             register_type = EnumTypeWrapper(register_type)
         self.register_type = register_type
         self.addr = addr
         self.size = size
 
@@ -117,15 +116,15 @@
         return instance.write(self.addr, self.register_type.to_binary(value))
 
 
 class GetSetRegister(SetRegister, GetRegister):
     pass
 
 
-class GetSetBit(object):
+class GetSetBit:
     def __init__(self, addr, pos, bit_type=None):
         self._bit_type = bit_type
         self.addr = addr
         self.pos = pos
 
     def __get__(self, instance, owner):
         if instance is None:
@@ -137,21 +136,14 @@
     def __set__(self, instance, value):
         current = instance.read(self.addr)
         new_value = intbv(current)
         new_value[self.pos] = value
         return instance.write(self.addr, int(new_value))
 
 
-# class EnumRegister(GetSetRegister):
-#    def __init__(self, addr, enum_type):
-#        assert issubclass(enum_type, Enum)
-#        register_type = EnumType(enum_type)
-#        super(EnumRegister, self).__init__(addr, register_type)
-
-
 class HK(MemoryInterface):
     def __init__(self, addr_base=0x40000000, **kwd):
         kwd["addr_base"] = addr_base
         super(HK, self).__init__(**kwd)
 
     id = GetRegister(0x0, UnsignedInteger(size=4))
     dna_part1 = GetRegister(0x4, UnsignedInteger(size=32))
@@ -196,18 +188,18 @@
     vccaux = GetRegister(addr=0x44, register_type=XADC())
     vccddr = GetRegister(addr=0x48, register_type=XADC())
 
 
 class TriggerSource(Enum):
     none = 0
     immediately = 1
-    chA_posedge = 2
-    chA_negedge = 3
-    chB_posedge = 4
-    chB_negedge = 5
+    cha_posedge = 2
+    cha_negedge = 3
+    chb_posedge = 4
+    chb_negedge = 5
     ext_posedge = 6
     ext_negedge = 7
     awg_posedge = 8
     awg_negedge = 9
 
 
 class Decimation(UnsignedInteger):
@@ -244,15 +236,15 @@
     hysteresis_ch1 = GetSetRegister(0x20, SignedInteger(size=14))
     hysteresis_ch2 = GetSetRegister(0x24, SignedInteger(size=14))
     average = GetSetBit(addr=0x28, pos=0)
     # equalization filter not implemented here
     dac2_on_ch1 = GetSetBit(0x50, pos=0)
     dac1_on_ch2 = GetSetBit(0x50, pos=1)
 
-    ## Function specific to read the array of data
+    # Function specific to read the array of data
     def get_rawdata(self, addr):
         x = self.reads(addr, self.data_length)
         y = x.copy()
         y.dtype = np.int32
         y[y > 2**13] -= 2**14
         return y
 
@@ -291,15 +283,15 @@
         self.average = True
         self.frequency = frequency
         self.trigger_source = trigger_source
         self.reset_writestate_machine(v=False)
         self.arm_trigger()
 
     def rearm(self, frequency=None, trigger_source=8):
-        if not frequency is None:
+        if frequency is not None:
             self.frequency = frequency
         self.trigger_delay = self.data_length
         self.trigger_source = trigger_source
         self.arm_trigger()
 
     @property
     def frequency(self):
@@ -511,15 +503,15 @@
 
         self.sm_onetimetrigger = True
         self.sm_wrappointer = False
         self.output_zero = False
         self.sm_reset = False
 
     def trig(self, frequency=None):
-        if not frequency is None:
+        if frequency is not None:
             self.frequency = frequency
         self.start_offset = 0
         self.trig_selector = 1
         self.trig_selector = 0
 
 
 class Pid(MemoryInterface):
@@ -578,59 +570,48 @@
 
     @derivative.setter
     def derivative(self, val):
         self.write(self.pidnumber * 0x10 + 0x1C, self.from_pyint(val, bitlength=14))
 
     def initialize(self, setpoint=None, integral=0, proportional=0, derivative=0):
         self.reset = True
-        if not setpoint is None:
+        if setpoint is not None:
             self.setpoint = setpoint
         self.integral = integral
         self.proportional = proportional
         self.derivative = derivative
         self.reset = False
 
 
-class InterfaceDescriptor(object):
+class InterfaceDescriptor:
     def __init__(self, cls, **kwd):
         self._cls = cls
         self.kwd = kwd
 
     def __get__(self, instance, owner):
         if instance is None:
             return self._cls
         return self._cls(parent_memory=instance, **self.kwd)
 
 
-class RedPitaya(object):
+class RedPitaya:
     hk = InterfaceDescriptor(HK)
     ams = InterfaceDescriptor(AMS)
     scope = InterfaceDescriptor(Scope)
     pid11 = InterfaceDescriptor(Pid, number="11")
     pid12 = InterfaceDescriptor(Pid, number="12")
     pid21 = InterfaceDescriptor(Pid, number="21")
     pid22 = InterfaceDescriptor(Pid, number="22")
     asga = InterfaceDescriptor(ASG, channel="A")
     asgb = InterfaceDescriptor(ASG, channel="B")
 
 
-# class BoardRedPitaya(RedPitaya, BoardRawMemory):
-#    pass
-
-
-# class PCRedPitaya(RedPitaya, ClientMemory):
-#    pass
-
 if __name__ == "__main__":
     from time import sleep, time
 
-    import rpyc
-
-    #    conn = rpyc.connect('134.157.6.206', 18861)
-    #    red_pitaya = PCRedPitaya(remote_connection = conn)
-    red_pitaya = BoardRedPitaya()
+    red_pitaya = RedPitaya()
     red_pitaya.scope.arm_trigger()
     red_pitaya.scope.trigger_source = 1
     sleep(1)
     t0 = time()
     red_pitaya.scope.data_ch1
     print(time() - t0)
```

### Comparing `pyrp3-1.1.1rc1/pyrp3/memory.py` & `pyrp3-1.2.0/pyrp3/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class MemoryInterface(object):
+class MemoryInterface:
     def __init__(self, addr_base=0x00000000, parent_memory=None):
         self.addr_base = addr_base
         self._parent = parent_memory
 
     def read(self, addr):
         """Read one register"""
         return self._parent.read(self.addr_base + addr)
```

### Comparing `pyrp3-1.1.1rc1/pyrp3/raw_memory.py` & `pyrp3-1.2.0/pyrp3/raw_memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 libmonitor = cdll.LoadLibrary(libmonitor_file)
 libmonitor.read_value.restype = c_uint32
 
 # TODO
 # Specify output types of read_value to uint32
 
 
-class BoardRawMemory(object):
+class BoardRawMemory:
     """Classes uses to interface de RedPitaya memory
 
     This is a one to one match to the libmonitor.so library"""
 
     a = libmonitor
 
     def read(self, addr):
```

### Comparing `pyrp3-1.1.1rc1/pyrp3/service.py` & `pyrp3-1.2.0/pyrp3/service.py`

 * *Files identical despite different names*

### Comparing `pyrp3-1.1.1rc1/pyrp3.egg-info/PKG-INFO` & `pyrp3-1.2.0/pyrp3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrp3
-Version: 1.1.1rc1
+Version: 1.2.0
 Summary: Python utilities for redpitaya
 Author: Pierre Cladé
 Author-email: pierre.clade@upmc.fr
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Keywords: redpitaya,FPGA,zynq
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pyrp3
 =======
 Python 3 port (using 2to3) of `PyRedPitaya <https://github.com/clade/PyRedPitaya>`_ library in the `pyrp3` namespace.
```

