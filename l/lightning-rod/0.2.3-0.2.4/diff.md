# Comparing `tmp/lightning_rod-0.2.3.tar.gz` & `tmp/lightning_rod-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.2.3.tar", max compression
+gzip compressed data, was "lightning_rod-0.2.4.tar", max compression
```

## Comparing `lightning_rod-0.2.3.tar` & `lightning_rod-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1061 2023-06-23 07:04:03.462174 lightning_rod-0.2.3/LICENSE
--rw-r--r--   0        0        0      347 2023-06-23 07:04:03.462174 lightning_rod-0.2.3/README.md
--rw-r--r--   0        0        0      307 2023-06-23 07:05:07.371057 lightning_rod-0.2.3/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      566 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4574 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       38 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0       85 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/comment.bolt
--rw-r--r--   0        0        0      144 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     1593 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      581 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     2418 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0       35 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0       86 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1047 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2142 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/py.typed
--rw-r--r--   0        0        0     1242 2023-06-23 07:05:07.391058 lightning_rod-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 lightning_rod-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1389 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/README.md
+-rw-r--r--   0        0        0      307 2023-07-05 19:29:24.543454 lightning_rod-0.2.4/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      566 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4562 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       38 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      144 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     1593 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      569 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     2521 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0       35 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0       86 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1029 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2175 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-07-05 19:28:21.778877 lightning_rod-0.2.4/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1242 2023-07-05 19:29:24.559454 lightning_rod-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.2.4/PKG-INFO
```

### Comparing `lightning_rod-0.2.3/LICENSE` & `lightning_rod-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/api.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/bossbar.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import ClassVar
 from dataclasses import dataclass
 
-from wicked_expressions:api import StaticVar, Int, ExpressionNode, Rebindable
+from wicked_expressions:api import Var, Int, ExpressionNode, Rebindable
 from ./utils import logger
 from ./raw_cmd import raw_cmd
 from ./tag import tag, untag
 from ./config import Config
 
 import inspect
 
 
 @dataclass
 class Bossbar(Rebindable):
     _bossbar_index: ClassVar[int] = 0
 
     def __post_init__(self):
-        self._temp = StaticVar(Int)
+        self._temp = Var(Int)
 
         self._id = self._generate_unique_id()
         self._name = self._id
         self._color = 'white'
         self._style = 'progress'
         self._visible = True
         self._last_value = None
```

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/effect.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/math.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/math.bolt`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from wicked_expressions:api import StaticVar, Int, ExpressionNode
+from wicked_expressions:api import Var, StaticVar, Int, ExpressionNode
 from ./config import Config
 
 
 _WORKING_DIR = f"{Config.ROOT}/math"
 
 
 def random(value_min: int | ExpressionNode, value_max: int | ExpressionNode) -> ExpressionNode:
     min = StaticVar(Int)
     max = StaticVar(Int)
     size = StaticVar(Int)
     lcg = StaticVar(Int)
-    output = StaticVar(Int)
+    temp = StaticVar(Int)
+    output = Var(Int)
 
     lcg_a = 1630111353
     lcg_c = 1623164762
     lcg_m = 2147483647
     setup_path = f"{_WORKING_DIR}/random/setup"
     run_path = f"{_WORKING_DIR}/random/run"
 
@@ -26,66 +27,71 @@
         if not lcg.exists():
             with lcg.store():
                 seed
 
     execute function run_path:
         size = max - min + 1
         lcg = (lcg * lcg_a + lcg_c) % lcg_m
-        output = lcg / 8 % size + min
+        temp = lcg / 8 % size + min
 
+    output = temp
     return output
 
 
 def pow(val: int | ExpressionNode, exp: int | ExpressionNode) -> ExpressionNode:
     value = StaticVar(Int)
     exponent = StaticVar(Int)
-    output = StaticVar(Int)
+    temp = StaticVar(Int)
+    output = Var(Int)
 
     run_path = f"{_WORKING_DIR}/pow/run"
 
     value = val
     exponent = exp
 
     execute function run_path:
-        output *= value
+        temp *= value
         exponent -= 1
 
         if exponent > 1:
             function run_path
 
+    output = temp
     return output
 
 
 def sqrt(val: int | ExpressionNode) -> ExpressionNode:
     a = StaticVar(Int)
     b = StaticVar(Int)
     value = StaticVar(Int)
-    output = StaticVar(Int)
+    temp = StaticVar(Int)
+    output = Var(Int)
 
     run_path = '{_WORKING_DIR}/sqrt/run'
 
     value = val
 
     if value >= 214748:
         tellraw @a [{"text":f"\n{Config.LIBRARY_NAME} ","color":"gray"},{"text":" ERROR 'sqrt()' overflow. Input value of ","color":"red"},{"score":{"name": value.holder, "objective": value.obj},"color":"red"},{"text":" is too large.","color":"red"}]
     if value < 0:
         tellraw @a [{"text":f"\n{Config.LIBRARY_NAME} ","color":"gray"},{"text":" ERROR 'sqrt()' received input value ","color":"red"},{"score":{"name": value.holder, "objective": value.obj},"color":"red"},{"text":". Negative input values not supported.","color":"red"}]
 
     b = value
     value *= 10000
-    output = 1255
+    temp = 1255
 
     for _ in range(4):
         execute function run_path:
-            a = value / output
-            output += a
-            output /= 2
+            a = value / temp
+            temp += a
+            temp /= 2
 
     if b >= 10000:
         function run_path
     if b >= 100000:
         function run_path
 
-    if output <= 0:
-        output *= -1
+    if temp <= 0:
+        temp *= -1
 
+    output = temp
     return output
```

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/time.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/time.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wicked_expressions:api import StaticVar, Int, ExpressionNode
+from wicked_expressions:api import Var, Int, ExpressionNode
 from ./raw_cmd import raw_cmd
 from ./utils import binary_progression
 from ./config import Config
 
 
 _WORKING_DIR = f"{Config.ROOT}/time"
 
@@ -13,15 +13,15 @@
 def get_time() -> ExpressionNode:
     return _get('daytime')
 
 def get_day() -> ExpressionNode:
     return _get('day')
 
 def set_time(value: int | ExpressionNode):
-    output = StaticVar(Int)
+    output = Var(Int)
 
     if not isinstance(value, ExpressionNode):
         time set value
         return 0
 
     output = value
     bin_prog = binary_progression(16)
@@ -34,13 +34,13 @@
         for n in bin_prog:
             if output >= n:
                 execute function f"{run_path}_{n}":
                     output -= n
                     time add n
 
 def _get(mode: str) -> ExpressionNode:
-    output = StaticVar(Int)
+    output = Var(Int)
 
     with output.store():
         raw_cmd(f"time query {mode}")
 
     return output
```

### Comparing `lightning_rod-0.2.3/lightning_rod/modules/xp.bolt` & `lightning_rod-0.2.4/lightning_rod/modules/xp.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wicked_expressions:api import StaticVar, Int, ExpressionNode
+from wicked_expressions:api import Var, StaticVar, Int, ExpressionNode
 from ./raw_cmd import raw_cmd
 from ./utils import binary_progression
 from ./config import Config
 
 
 _WORKING_DIR = f"{Config.ROOT}/xp"
 
@@ -25,18 +25,18 @@
 
 def set_xp_percent(amount: int | ExpressionNode):
     amt = StaticVar(Int)
     previous_level = StaticVar(Int)
 
     amt = amount
 
-    execute function f"{_WORKING_DIR}/set_percent":
-        # save previous level
-        previous_level = get_level()
+    # save previous level
+    previous_level = get_level()
 
+    execute function f"{_WORKING_DIR}/set_percent":
         set_level(8772)
         set_xp(0)
 
         for n in binary_progression(7, reversed=True):
             if amt >= n:
                 increment = n * 778      # (lvl 8872) 778 xp = 1% of bar
 
@@ -48,22 +48,24 @@
                     amt -= n
                     xp add @s increment
 
         # restore level
         set_level(previous_level)
 
 def _get_xp(mode: str) -> ExpressionNode:
-    output = StaticVar(Int)
+    temp = StaticVar(Int)
+    output = Var(Int)
 
-    with output.store():
+    with temp.store():
         if mode in ('p', 'points'):
             xp query @s points
         elif mode in ('l', 'levels'):
             xp query @s levels
 
+    output = temp
     return output
 
 def _set_xp_from_expression(amount: ExpressionNode, mode: str):
     amt = StaticVar(Int)
 
     raw_cmd(f"xp set @s 0 {mode}")
     amt = amount
```

### Comparing `lightning_rod-0.2.3/pyproject.toml` & `lightning_rod-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.2.3"
+version = "0.2.4"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
```

