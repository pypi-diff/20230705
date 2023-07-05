# Comparing `tmp/fatld-0.1.6.tar.gz` & `tmp/fatld-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fatld-0.1.6.tar", max compression
+gzip compressed data, was "fatld-0.1.7.tar", max compression
```

## Comparing `fatld-0.1.6.tar` & `fatld-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     3239 2023-03-10 20:43:01.274937 fatld-0.1.6/README.md
--rwxr-xr-x   0        0        0      147 2023-04-18 13:22:51.567061 fatld-0.1.6/fatld/__init__.py
--rwxr-xr-x   0        0        0    33809 2023-04-18 13:22:16.768689 fatld-0.1.6/fatld/design.py
--rwxr-xr-x   0        0        0     6794 2023-03-10 14:53:29.404853 fatld-0.1.6/fatld/main.py
--rwxr-xr-x   0        0        0     8448 2023-03-10 14:53:29.419886 fatld-0.1.6/fatld/relation.py
--rwxr-xr-x   0        0        0     1040 2023-04-18 13:22:46.910889 fatld-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 fatld-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     3238 2023-07-03 09:25:25.776302 fatld-0.1.7/README.md
+-rwxr-xr-x   0        0        0      147 2023-04-18 13:22:51.567061 fatld-0.1.7/fatld/__init__.py
+-rwxr-xr-x   0        0        0    37463 2023-07-05 14:24:40.991279 fatld-0.1.7/fatld/design.py
+-rwxr-xr-x   0        0        0     6794 2023-03-10 14:53:29.404853 fatld-0.1.7/fatld/main.py
+-rwxr-xr-x   0        0        0     8448 2023-03-10 14:53:29.419886 fatld-0.1.7/fatld/relation.py
+-rwxr-xr-x   0        0        0     1040 2023-07-05 13:00:57.622808 fatld-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 fatld-0.1.7/PKG-INFO
```

### Comparing `fatld-0.1.6/README.md` & `fatld-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 ```python
 >>> import fatld
 >>> D = fatld.Design(runsize=32, m=1, cols=[21, 27, 29])
 >>> D.wlp()
 [1, 3, 3, 0, 0]
 >>> D.defining_relation()
 ['A1cef', 'A3deg', 'A1cdeh']
->>> print("There are %s 2-2 interactions totally clear from any main effect or other interaction." % D.clear('2-2', 'all'))
-There are 6 2-2 interactions totally clear from any main effect or other interaction.
+>>> print("There are %s 2-2 interactions clear from any main effect or other two-factor interaction." % D.clear('2-2'))
+There are 6 2-2 interactions clear from any main effect or other two-factor interaction.
 >>> print("The design contains %s four-level factors and %s two-level factors" % (D.m, D.n))
 The design contains 1 four-level factors and 6 two-level factors
 ```
 
 For more examples see the documentation.
 
 ## Installation
```

### Comparing `fatld-0.1.6/fatld/design.py` & `fatld-0.1.7/fatld/design.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             warnings.warn("Wrong max_length value, ignoring")
             return wlp_list
         elif max_length is None:
             return wlp_list
         else:
             return wlp_list[0 : (max_length - 2)]
 
-    def qwlp(self, max_length: int | None = None) -> tuple[list[float], list[int]]:
+    def beta_wlp(self, max_length: int | None = None) -> tuple[list[float], list[int]]:
         """
         Find the permutation of the levels of the m four-level factors that minimize
         the qWLP for the design.
 
         Parameters
         ----------
         max_length : int, optional
@@ -239,29 +239,101 @@
 
         # Compute all possible permutations for m factors
         all_perms = []
         for _, p in enumerate(product(range(12), repeat=self.m)):
             all_perms.append([perms[i] for i in p])
 
         # Compute beta wlp for all permutations
-        a_vector_list = beta_wlp(
+        a_vector_list = qwlp(
             design=self, permutation_list=all_perms, max_length=max_length
         )
 
         # Find the best Beta vector and the corresponding permutation
         best_vector = a_vector_list[0]
         best_perm = all_perms[0]
 
         for i, v in enumerate(a_vector_list[1:]):
             if best_vector > v:
                 best_vector = v
                 best_perm = all_perms[i]
 
         return best_vector, best_perm
 
+    def w2_wlp(self) -> tuple[list[float], str]:
+        """
+        Compute the W_2 word length pattern of the design.
+        The structure of the W_2 vector is:
+        A3.0, A2.1, A4.0, A5.0, A3.1, A6.0, A7.0, ...
+
+        Returns
+        -------
+        W2_vector: list[float]
+            The vector containing the A_x.i values of the W_2 word length pattern
+        factor: str
+            A string indicating which factor must be used to obtain W_2 optimal
+            blocking. Can either be 'A', 'B', or 'C'.
+            
+        """
+        design_oa = oa.array_link(self.array)
+        design_wlp = list(map(int, design_oa.GWLP()))
+
+        best_factor = "A"
+        best_w2_vector = []
+        for factor_index in range(self.m):
+            # Remove the blocking factor and evaluate the WLP of the design
+            trmt_wlp = list(map(int, design_oa.deleteColumn(factor_index).GWLP()))
+            block_wlp = [design_wlp[i] - x for i, x in enumerate(trmt_wlp)]
+            w2_vector = build_w2_vector(block_wlp, trmt_wlp)
+            # Set as default if it is the first factor we evaluate
+            if factor_index == 0:
+                best_w2_vector = w2_vector
+            else:
+                if w2_vector < best_w2_vector:
+                    best_w2_vector = w2_vector
+                    best_factor = chr(65 + factor_index)
+        return best_w2_vector, best_factor
+
+    def alpha_wlp(self, rounding: bool = True) -> list[float]:
+        """
+        Compute the alpha word length pattern of the design.
+        The alpha wlp contains 5 values ordered in the following way:
+        ω4, ω2, ω42, ω22, ω44
+
+        Parameters
+        ----------
+        rounding : bool, optional
+            Round the ω values to 2 decimals, by default True
+
+        Returns
+        -------
+        list[float]
+            The alpha word length pattern
+        """
+        twlp = self.twlp(max_length=4)
+        a3_vector = twlp[0] + [0] * (3 - len(twlp[0]))  # Right pad with 0
+        a4_vector = twlp[1] + [0] * (4 - len(twlp[1]))
+        omega_weights = {
+            "w2": [3 / 3, 2 / 3, 1 / 3],
+            "w4": [0 / 3, 1 / 3, 2 / 3],
+            "w22": [6 / 6, 3 / 6, 1 / 6, 0 / 6],
+            "w42": [0 / 6, 3 / 6, 4 / 6, 3 / 6],
+            "w44": [0 / 6, 0 / 6, 1 / 6, 3 / 6],
+        }
+        omega_values = dict()
+        for name, weight_vector in omega_weights.items():
+            if len(name) == 2:
+                value = [w * a for w, a in zip(weight_vector, a3_vector)]
+            else:
+                value = [w * a for w, a in zip(weight_vector, a4_vector)]
+            omega_values[name] = sum(value)
+        alpha_wlp = [omega_values[i] for i in ["w4", "w2", "w42", "w22", "w44"]]
+        if rounding:
+            alpha_wlp = [round(i, 3) for i in alpha_wlp]
+        return alpha_wlp
+
     def resolution(self) -> int | None:
         """
         Compute the resolution of the design.
         """
         wlp = self.wlp()
         res = next((i + 3 for i, x in enumerate(wlp) if x), None)
         return res
@@ -497,15 +569,15 @@
                     clarity_df.loc["Any type", column_label] += 1  # type: ignore
                     all_clear += 1
                 if all_clear == 3:
                     clarity_df.loc[int_type, "Totally clear"] += 1  # type: ignore
                     clarity_df.loc["Any type", "Totally clear"] += 1  # type: ignore
         return clarity_df
 
-    def clear(self, interaction_type: str, clear_from: str) -> int:
+    def clear(self, interaction_type: str, clear_from: str = "all") -> int:
         """
         Compute the number of interactions of type `interaction_type` that are clear
         from interactions of the `clear_from` type.
 
         Parameters
         ----------
         interaction_type : str
@@ -660,15 +732,15 @@
     cols_id, _ = np.nonzero(cols_mat)
     cols_gen = [labels_list[i] for i in cols_id]
     cols_num = [gen2num(i) for i in cols_gen]
     added_cols = [i for i in cols_num if np.log2(i) % 1 != 0]
     return Design(run_size, n_flvl, added_cols)
 
 
-def beta_wlp(
+def qwlp(
     design: Design,
     permutation_list: list[list[list[int]]],
     max_length: None | int = None,
 ) -> list[list[float]]:
     """
     Compute the beta WLP of the design.
 
@@ -861,7 +933,26 @@
     # Ones represent an active factor in the interaction
     index = 0
     for i in range(max_length):
         for c in combinations(range(n), i + 1):
             tfi_model_matrix[c, index] = 1
             index += 1
     return tfi_model_matrix
+
+
+def build_w2_vector(blocking_wlp: list[int], treatment_wlp: list[int]) -> list[int]:
+    """
+    Compute the W_2 word length pattern (WLP) of a design, given its treatment WLP and
+    blocking WLP.
+    Both WLP must start with words of length 0 (so that list indices matches word
+    lengths).
+    """
+    if len(blocking_wlp) != len(treatment_wlp):
+        raise ValueError("Both WLP must have the same length")
+    w2_vector = [treatment_wlp[3], blocking_wlp[3]]
+    n_words = len(blocking_wlp) - 1
+    max_i = 1 + (n_words - 1) // 2
+    for i in range(2, max_i):
+        w2_vector.append(treatment_wlp[2 * i])
+        w2_vector.append(treatment_wlp[2 * i + 1])
+        w2_vector.append(blocking_wlp[i + 2])
+    return w2_vector
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fatld-0.1.6/fatld/main.py` & `fatld-0.1.7/fatld/main.py`

 * *Files identical despite different names*

### Comparing `fatld-0.1.6/fatld/relation.py` & `fatld-0.1.7/fatld/relation.py`

 * *Files identical despite different names*

### Comparing `fatld-0.1.6/pyproject.toml` & `fatld-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fatld"
-version = "0.1.6"
+version = "0.1.7"
 description = "Generate and characterize designs with four-and-two-level (FATL) factors"
 authors = ["Alexandre Bohyn <alexandre.bohyn@kuleuven.be>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://abohyndoe.github.io/fatld/"
 repository = "https://github.com/ABohynDOE/fatld"
 keywords = ["design", "doe"]
```

### Comparing `fatld-0.1.6/PKG-INFO` & `fatld-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fatld
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generate and characterize designs with four-and-two-level (FATL) factors
 Home-page: https://abohyndoe.github.io/fatld/
 License: MIT
 Keywords: design,doe
 Author: Alexandre Bohyn
 Author-email: alexandre.bohyn@kuleuven.be
 Requires-Python: >=3.8,<4.0
@@ -40,16 +40,16 @@
 ```python
 >>> import fatld
 >>> D = fatld.Design(runsize=32, m=1, cols=[21, 27, 29])
 >>> D.wlp()
 [1, 3, 3, 0, 0]
 >>> D.defining_relation()
 ['A1cef', 'A3deg', 'A1cdeh']
->>> print("There are %s 2-2 interactions totally clear from any main effect or other interaction." % D.clear('2-2', 'all'))
-There are 6 2-2 interactions totally clear from any main effect or other interaction.
+>>> print("There are %s 2-2 interactions clear from any main effect or other two-factor interaction." % D.clear('2-2'))
+There are 6 2-2 interactions clear from any main effect or other two-factor interaction.
 >>> print("The design contains %s four-level factors and %s two-level factors" % (D.m, D.n))
 The design contains 1 four-level factors and 6 two-level factors
 ```
 
 For more examples see the documentation.
 
 ## Installation
```

