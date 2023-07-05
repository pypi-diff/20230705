# Comparing `tmp/adaptivecard-0.0.9.tar.gz` & `tmp/adaptivecard-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.0.9.tar", last modified: Thu Jun 29 21:32:53 2023, max compression
+gzip compressed data, was "adaptivecard-0.1.0.tar", last modified: Wed Jul  5 05:00:51 2023, max compression
```

## Comparing `adaptivecard-0.0.9.tar` & `adaptivecard-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:32:53.500735 adaptivecard-0.0.9/
--rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-06-29 21:21:04.000000 adaptivecard-0.0.9/LICENSE.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-06-29 21:32:53.500540 adaptivecard-0.0.9/PKG-INFO
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.0.9/README.md
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:32:53.499108 adaptivecard-0.0.9/adaptivecard/
--rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.0.9/adaptivecard/__init__.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)    15621 2023-06-18 21:56:27.000000 adaptivecard-0.0.9/adaptivecard/classes.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.0.9/adaptivecard/exceptions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1610 2023-06-18 21:56:27.000000 adaptivecard-0.0.9/adaptivecard/mixin.py
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:32:53.500242 adaptivecard-0.0.9/adaptivecard.egg-info/
--rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 cabutchei   (501) staff       (20)      307 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       10 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/requires.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-06-29 21:32:53.500802 adaptivecard-0.0.9/setup.cfg
--rw-r--r--   0 cabutchei   (501) staff       (20)      955 2023-06-29 21:32:03.000000 adaptivecard-0.0.9/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 05:00:51.990020 adaptivecard-0.1.0/
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/LICENSE.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 05:00:51.989762 adaptivecard-0.1.0/PKG-INFO
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.1.0/README.md
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 05:00:51.988551 adaptivecard-0.1.0/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.1.0/adaptivecard/__init__.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)      418 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/_base_types.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3155 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/abstract_types.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1132 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/actions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     2980 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/card_elements.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     3516 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/cards.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)    13967 2023-07-05 04:51:20.000000 adaptivecard-0.1.0/adaptivecard/containers.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.1.0/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1611 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/adaptivecard/mixin.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-07-05 05:00:51.989418 adaptivecard-0.1.0/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      445 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       19 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/requires.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-07-05 05:00:51.000000 adaptivecard-0.1.0/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-07-05 05:00:51.990082 adaptivecard-0.1.0/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)      975 2023-07-05 04:12:51.000000 adaptivecard-0.1.0/setup.py
```

### Comparing `adaptivecard-0.0.9/LICENSE.txt` & `adaptivecard-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.0.9/PKG-INFO` & `adaptivecard-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.0.9
+Version: 0.1.0
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,card,adaptive card,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adaptivecard-0.0.9/adaptivecard/classes.py` & `adaptivecard-0.1.0/adaptivecard/containers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,85 @@
+from typing import Any, Optional, Union, Literal, Sequence, List, get_type_hints
+from adaptivecard._base_types import Element, Action, ISelectAction
 from adaptivecard.mixin import Mixin
-from typing import Union, List, Optional, Any, Collection
+from tabulate import tabulate
+from typeguard import check_type
+from adaptivecard.card_elements import TextBlock
 
 
-class Element():
-    pass
 
-
-class TableRow(Mixin):
-    def __init__(self, cells: Union["TableCell", Collection["TableCell"]]):
-        if not self.is_collection(cells):
-            raise TypeError("'cells' attribute must be a collection of some kind")
-        if isinstance(cells, TableCell):
-            cells = [cells]
-        else:
-            cells = list(cells)
-        self.type = "TableRow"
-        self.cells = cells
-        self.json_fields = ("type", "cells")
-
-    def __len__(self):
-        return len(self.cells)
-
-    def add_cell(self, cell: "TableCell"):
-        if not isinstance(cell, TableCell):
-            raise TypeError("'cell' attribute must be of type 'TableCell'")
-        self.cells.append(cell)
-
-
-class TableCell(Mixin):
-    def __init__(self,
-                 items: Optional[list] = None,
-                 selectAction = None,   # definir mais tarde
-                 style: Optional[str] = None,
-                 verticalAlignment: Optional[str] = None,
-                 bleed: Optional[bool] = None,
-                 backgroundImage: Optional[str] = None,
-                 minHeight: Optional[str] = None,
-                 rtl: Optional[bool] = None):
-
-        if items is None:
-            items = []
-        self.type = "TableCell"
-        self.items = items
-        self.selectAction = selectAction
-        self.items = items
-        self.style = style
-        self.verticalAlignment = verticalAlignment
-        self.bleed = bleed
-        self.backgroundImage = backgroundImage
-        self.minHeight = minHeight
-        self.rtl = rtl
-        self.json_fields = ('type', 'items', 'selectAction', 'style', 'verticalAlignment', 'bleed', 'backgroundImage', 'minHeight', 'rtl')
-
-    def add_to_items(self, element: Element):
-        self.items.append(element)
-
-
-class Content:
-    """Content é o elemento que recebe o AdaptiveCard e é adicionado à lista atachments, atributo de Message"""
-    def __init__(self, content: "AdaptiveCard"):
-        self.contentType = "application/vnd.microsoft.card.adaptive"
-        self.content = content
-
-
-class Message(Mixin):
-    """"Estrutura final do card tal como se requer para envio a um canal do Teams"""
-    def __init__(self, attachments: Optional[Collection["Content"]] = None):
-        self.type = "message"
-        if attachments is None:
-            attachments = []
-        if not self.is_collection(attachments):
-            raise TypeError("'attachments' attribute must be a collection of some kind")
-        self.attachments = list(attachments)
-
-    def attach(self, content):
-        self.attachments.append(content)
-
-# -------------------------Cards------------------------- #
-
-
-class AdaptiveCard(Mixin):
-    """O template principal do card"""  # Essas descrições hão de ficar mais detalhadas à medida que eu desenvolver a lib e sua documentação
-    def __init__(self, version: str = "1.2",
-                 schema: str = "http://adaptivecards.io/schemas/adaptive-card.json",
-                 body: Optional[Collection[Element]] = None,
-                 fallbackText: Optional[str] = None,
-                 backgroundImage: Optional[str] = None,
-                 minHeight: Optional[str] = None,
-                 rtl: Optional[bool] = None,
-                 speak: Optional[str] = None,
-                 lang: Optional[str] = None,
-                 verticalContentAlignment: Optional[str] = None):
-
-        if body is None:
-            body = []
-        if not self.is_collection(body):
-            raise TypeError("'body' attribute must be a collection of some kind")
-        
-        self.type = "AdaptiveCard"
-        self.version = version  
-        self.schema = schema
-        self.body = list(body)
-        self.fallbackText = fallbackText
-        self.backgroundImage = backgroundImage
-        self.minHeight = minHeight
-        self.rtl = rtl
-        self.speak = speak
-        self.lang = lang
-        self.verticalContentAlignment = verticalContentAlignment
-        self.json_fields = ('type', 'version', 'schema', 'body', 'fallbackText', 'backgroundImage',
-                                      'minHeight', 'rtl', 'speak', 'lang', 'verticalContentAlignment', 'actions')
-
-    @property
-    def empty(self):
-        return len(self.body) == 0
-
-    def add_to_body(self, card_element):
-        self.body.append(card_element)
-
-    def add_action(self, action):
-        if not hasattr(self, 'actions'):
-            self.actions = []
-        self.actions.append(action)
-
-    def to_message(self):
-        content = Content(card=self)
-        msg = Message(attachments=[content])
-        return msg
-
-    def __setattr__(self, __name: str, __value: Any) -> None:
-        if __name == 'verticalContentAlignment' and isinstance(__value, str) \
-                and __value not in (allowed_values := ("top", "center", "bottom")):
-            raise AttributeError(f"'{__name}' atribute can only take either of the following values: {', '.join(allowed_values)}")
-        return super().__setattr__(__name, __value)
-
-# ---------------------Containers------------------------- #
-
-
-class Container(Mixin):
+class Container(Mixin, Element):
     """Um contâiner é um agrupamento de elementos"""
     def __init__(self,
-                 items: Optional[list] = None,
-                 style: Optional[str] = None,
-                 verticalContentAlignment: Optional[str] = None,
+                 items: Optional[Union[Element, Sequence[Element]]] = None,
+                 style: Optional[Literal["default", "emphasis", "good", "attention", "warning", "accent"]] = None,
+                 verticalContentAlignment: Optional[Literal["top", "center", "bottom"]] = None,
                  bleed: Optional[bool] = None,
                  minHeight: Optional[str] = None,
                  rtl: Optional[bool] = None,
-                 height: Optional[str] = None,
-                 separator: Optional[str] = None,
+                 height: Optional[Literal["auto", "stretch"]] = None,
+                 separator: Optional[bool] = None,
+                 spacing: Optional[Literal["default", "none", "small", "medium", "large", "extraLarge", "padding"]] = None,
                  id: Optional[str] = None,
                  isVisible: Optional[bool] = None):
 
-        if items is None:
-            items = []
-
         self.type = "Container"
         self.items = items
         self.style = style
         self.verticalContentAlignment = verticalContentAlignment
         self.bleed = bleed
         self.minHeight = minHeight
         self.rtl = rtl
         self.height = height
         self.separator = separator
+        self.spacing = spacing
         self.id = id
         self.isVisible = isVisible
         self.json_fields = ('type', 'items', 'style', 'verticalContentAlignment', 'bleed', 'minHeight', 'rtl',
                                       'height', 'separator', 'id', 'isVisible')
 
     @property
     def empty(self):
         return len(self.items) == 0
 
-    def add_to_items(self, card_element):
-        self.items.append(card_element)
+    def append_element(self, element: Element):
+        self.items.append(element)
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(items={self.items})"
+
+    def __str__(self) -> str:
+        return "[" + ", ".join([str(item) for item in self.items]) + "]"
+    
     def __setattr__(self, __name: str, __value: Any) -> None:
-        if __name == 'style' and __value not in (allowed_values := ("default", "emphasis", "good", "attention", "warning", "accent")):
-            raise AttributeError(f"'{__name}' attribute can only take either of the following values: {', '.join(allowed_values)}")
-        if __name == 'verticalContentAlignment' and __value not in (allowed_values := ("top", "center", "bottom")):
-            raise AttributeError(f"'{__name}' atribute can only take either of the following values: {', '.join(allowed_values)}")
-        if __name == 'height' and __value not in (allowed_values := ("auto", "stretch")):
-            raise AttributeError(f"'{__name}' atribute can only take either of the following values: {', '.join(allowed_values)}")
-        if __name == 'spacing' and __value not in (allowed_values := ("default", "none", "small", "medium", "large", "extraLarge", "padding")):
-            raise AttributeError(f"'{__name}' atribute can only take either of the following values: {', '.join(allowed_values)}")
+        if __name == 'items':
+            if __value is None:
+                __value = []
+            elif isinstance(__value, Element):
+                __value = [__value]
         return super().__setattr__(__name, __value)
 
 
 class ColumnSet(Mixin, Element):
     """ColumnSet define um grupo de colunas"""
-    def __init__(self, columns: Optional[Collection["Column"]] = None,
-                 style: Optional[str] = None,
+    def __init__(self, columns: Optional[Sequence["Column"]] = None,
+                 style: Optional[Literal["default", "emphasis", "good", "attention", "warning", "accent"]] = None,
                  bleed: Optional[bool] = None,
-                 minHeight: Optional[str] = None,
-                 horizontalAlignment: Optional[str] = None,
-                 height: Optional[str] = None,
+                 minHeight: Optional[str] = None,   # pensar em algum type check para isso
+                 horizontalAlignment: Optional[Literal["left", "center", "right"]] = None,
+                 height: Optional[Literal["auto", "stretch"]] = None,
                  separator: Optional[bool] = None,
-                 spacing: Optional[str] = None,
+                 spacing: Optional[Literal["default", "none", "small", "medium", "large", "extraLarge", "padding"]] = None,
                  id_: Optional[str] = None,
                  isVisible: Optional[bool] = None):
 
         if columns is None:
             columns = []
-        if not self.is_collection(columns):
-            raise TypeError("'columns' attribute must be a collection of some kind")
+        if not self.is_sequence(columns):
+            raise TypeError("'columns' attribute must be a Sequence of some kind")
 
         self.type = 'ColumnSet'
         self.columns = list(columns)
         self.style = style
         self.bleed = bleed
         self.minHeight = minHeight
         self.horizontalAlignment = horizontalAlignment
@@ -222,15 +94,15 @@
     def add_to_columns(self, column_element):
         self.columns.append(column_element)
 
 
 class Column(Mixin, Element):
     """O contâiner Column define um elemento de coluna, que é parte de um ColumnSet."""
     def __init__(self,
-                 items: Optional[Collection[Union["Image", "TextBlock"]]] = None,
+                 items: Optional[Sequence[Element]] = None,
                  backgroundImage=None,
                  bleed: Optional[bool] = None,
                  fallback: Optional["Column"] = None,
                  minHeight: Optional[str] = None,
                  rtl: Optional[bool] = None,
                  separator: Optional[bool] = None,
                  spacing: Optional[Union[str, int]] = None,
@@ -238,16 +110,16 @@
                  verticalContentAlignment: Optional[str] = None,
                  width: Optional[Union[str, int]] = None,
                  id_: Optional[str] = None,
                  isVisible: Optional[bool] = None):
 
         if items is None:
             items = []
-        if self.is_collection(items):
-            raise TypeError("'items' must be a collections of some kind")
+        if not self.is_sequence(items):
+            raise TypeError(f"'items' must be a Sequence of some kind, not {type(items)}")
 
         self.type = "Column"
         self.items = list(items)
         self.backgroundImage = backgroundImage
         self.bleed = bleed
         self.fallback = fallback
         self.minHeight = minHeight
@@ -258,49 +130,106 @@
         self.verticalContentAlignment = verticalContentAlignment
         self.width = width
         self.id = id_
         self.isVisible = isVisible
         self.json_fields = ('type', 'items', 'backgroundImage', 'bleed', 'fallback', 'minHeight', 'rtl', 'separator',
                                       'spacing', 'style', 'verticalContentAlignment', 'rtl', 'width', 'id', 'isVisible')
 
-
-    def __setattr__(self, __name: str, __value: Any) -> None:
-        return super().__setattr__(__name, __value)
-
     def add_to_items(self, card_element):
         self.items.append(card_element)
 
 
+class TableCell(Mixin):
+    def __init__(self,
+                 items: Optional[Union[Any, Sequence[Any]]] = None,
+                 selectAction: Optional[ISelectAction] = None,
+                 style: Optional[Literal["default", "emphasis", "good", "attention", "warning", "accent"]] = None,
+                 verticalAlignment: Optional[Literal["top", "center", "bottom"]] = None,
+                 bleed: Optional[bool] = None,
+                 backgroundImage: Optional[str] = None,
+                 minHeight: Optional[str] = None,
+                 rtl: Optional[bool] = None):
+      
+        if items is None:
+            items = []
+        elif isinstance(items, Element):
+            items = [items]
+        elif not self.is_sequence(items):
+            items = [TextBlock(text=str(items))]
+        else:
+            items = list(items)
+            for i, item in enumerate(items):
+                if not isinstance(item, Element):
+                    items[i] = TextBlock(text=str(item))
+        self.type = "TableCell"
+        self.items = items
+        self.selectAction = selectAction
+        self.items = items
+        self.style = style
+        self.verticalAlignment = verticalAlignment
+        self.bleed = bleed
+        self.backgroundImage = backgroundImage
+        self.minHeight = minHeight
+        self.rtl = rtl
+        self.json_fields = ('type', 'items', 'selectAction', 'style', 'verticalAlignment', 'bleed', 'backgroundImage', 'minHeight', 'rtl')
+
+    def add_to_items(self, element: Element):
+        self.items.append(element)
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(items={[str(item) for item in self.items]})"
+
+    def __str__(self) -> str:
+        return "[" + ", ".join([str(item) for item in self.items]) + "]"
+
+
+class TableRow(Mixin, Sequence):
+    def __init__(self, cells: List, style: Optional[Literal["default", "emphasis", "good", "attention", "warning", "accent"]] = None):
+        self.type = "TableRow"
+        for i, cell in enumerate(cells):
+            if not isinstance(cell, TableCell):
+                cells[i] = TableCell(cell)
+        self.cells = cells
+        self.style = style
+        self.json_fields = ("type", "cells", "style")
+    def __getitem__(self, __i):
+        if isinstance(__i, slice):
+            return self.__class__(cells=self.cells[__i])
+        return self.cells.__getitem__(__i)
+    def __setitem__(self, __key, __value):
+        self.cells.__setitem__(__key, TableCell(__value))
+    def __len__(self):
+        return len(self.cells)
+    def __repr__(self):
+        return f"{self.__class__.__name__}({str(self.cells)})"
+    def __str__(self):
+        return "[" + ", ".join([str(cell) for cell in self.cells]) + "]"
+
+
 class Table(Mixin, Element):
+
     def __init__(self,
-                 columns: Collection[int],
-                 rows: List[TableRow],
+                 rows: Optional[Sequence[Sequence[Union[Element, TableCell]]]] = None,
                  firstRowAsHeader: Optional[bool] = None,
+                 columns: Sequence[int] = [],
                  showGridLines: Optional[bool] = None,
-                 gridStyle: Optional[str] = None,
-                 horizontalCellContentAlignment: Optional[str] = None,
-                 verticalCellContentAlignment: Optional[str] = None,
-                 fallback: Optional[Union["ColumnSet", "Container", "Image", "Table"]] = None,
-                 height: Optional[str] = None,
+                 gridStyle: Optional[Literal["default", "emphasis", "good", "attention", "warning", "accent"]] = None,
+                 horizontalCellContentAlignment: Optional[Literal["left", "center", "right"]] = None,
+                 verticalCellContentAlignment: Optional[Literal["top", "center", "bottom"]] = None,
+                 fallback: Optional[Element] = None,
+                 height: Optional[Literal["auto", "stretch"]] = None,
                  separator: Optional[bool] = None,
-                 spacing: Optional[str] = None,
+                 spacing: Optional[Literal["default", "none", "small", "medium", "large", "extraLarge", "padding"]] = None,
                  id_: Optional[str] = None,
                  isVisible: Optional[bool] = None):
 
         self.type = "Table"
-        if len(columns) == 0:
-            raise AttributeError("Number of columns cannot be zero")
-        if not self.is_collection(columns):
-            raise TypeError("'columns' attribute must be a collection of some kind")
-        self._columns = list(columns)
-        if len(rows) == 0:
-            raise Exception
-        if not all(len(row) == len(columns) for row in rows):
-            raise Exception("The number of cells must match the number of columns in all rows")
+
         self.rows = rows
+        self._columns = list(columns)
         self.firstRowAsHeader = firstRowAsHeader
         self.showGridLines = showGridLines
         self.gridStyle = gridStyle
         self.horizontalCellContentAlignment = horizontalCellContentAlignment
         self.verticalCellContentAlignment = verticalCellContentAlignment
         self.fallback = fallback
         self.height = height
@@ -310,72 +239,93 @@
         self.isVisible = isVisible
         self.json_fields = ('type', 'columns', 'rows', 'firstRowAsHeader', 'showGridLines', 'gridStyle',
                                       'horizontalCellContentAlignment', 'verticalContentAlignment', 'fallback', 'height',
                                       'separator', 'spacing', 'id', 'isVisible')
     
     @property
     def columns(self):
-        return [{"width": value} for value in self._columns]
+        if len(self.rows) > 0:
+            if len(self._columns) == 0:
+                return [{"width": 1} for _ in self.rows[0]]
+            else:
+                return [{"width": value} for value in self._columns]
+
+    @columns.setter
+    def columns(self, value):
+        check_type(value, get_type_hints(self.__init__)['columns'])
+        cols = list(value)
+        if len(self.rows) > 0 and len(cols) < len(self.rows[0]):
+            raise Exception("'length of columns must match the length of rows'")
+        self._columns = value
+
+    def __getitem__(self, __i):
+        return self.rows.__getitem__(__i)
+    
+    def append_row(self, row: Sequence):
+        if not self.is_sequence(row):
+            raise Exception("'row' attribute must be a sequence of some kind")
+        row = TableRow(row)
+        self.rows.append(row)
+    
+    def __len__(self):
+        return len(self.rows)
+    
+    def __str__(self):
+        rows = [["\n".join([str(item) for item in cell.items]) for cell in row.cells] for row in self.rows]
+        if self.firstRowAsHeader:
+            headers = rows[0]
+            rows = rows[1:]
+        else:
+            headers = []
+        return tabulate(rows, headers=headers, tablefmt='grid')
 
     def __setattr__(self, __name: str, __value: Any) -> None:
+        if __name == 'rows':
+            rows = __value
+            if rows is None:
+                rows = []
+            elif not self.is_sequence(rows):
+                raise TypeError("'rows' attribute must be a sequence of some kind")
+            elif len(rows) > 0 and not all(self.is_sequence(row) for row in rows):
+                raise TypeError("'rows' attribute must be a sequence of sequences")
+            else:
+                for i, row in enumerate(rows):
+                    for j, cell in enumerate(row):
+                        if not isinstance(cell, TableCell):
+                            row[j] = TableCell(cell)
+                    rows[i] = TableRow(cells=row)
+
+            if len(rows) > 1 and not all([len(rows[i]) == len(rows[i-1]) for i, _ in enumerate(rows[1:])]):
+                raise Exception("Length mismatch, all rows must have the same length")
+            __value = rows
         return super().__setattr__(__name, __value)
 
-# -------------------------Card Elements--------------------------- #
-
 
-class TextBlock(Mixin, Element):
-    """Elemento de texto"""
+class ActionSet(Mixin, Element):
     def __init__(self,
-                 text: str = "",
-                 color: Optional[str] = None,
-                 fontType: Optional[str] = None,
-                 horizontalAlignment: Optional[str] = None,
-                 isSubtle: Optional[bool] = None,
-                 maxLines: Optional[int] = None,
-                 size: Optional[str] = None,
-                 weight: Optional[str] = None,
-                 wrap: Optional[bool] = None,
-                 style: Optional[str] = None,
-                 fallback: Optional[Union[str, ColumnSet, "Container", "TextBlock"]] = None,
-                 height: Optional[str] = None,
+                 actions: Optional[Union[Action, Sequence[Action]]] = None,
+                 fallback: Optional[Element] = None,
+                 height: Optional[Any] = None,
                  separator: Optional[bool] = None,
-                 spacing: Optional[str] = None,
+                 spacing: Optional[Literal["default", "none", "small", "medium", "large", "extraLarge", "padding"]] = None,
                  id_: Optional[str] = None,
-                 isVisible: Optional[bool] = None):
-
-        self.type = "TextBlock"
-        self.text = text
-        self.color = color
-        self.fontType = fontType
-        self.horizontalAlignment = horizontalAlignment
-        self.isSubtle = isSubtle
-        self.maxLines = maxLines
-        self.size = size
-        self.weight = weight
-        self.wrap = wrap
-        self.style = style
+                 isVisible: Optional[bool] = None
+                 ) -> None:
+        self.type = "ActionSet"
+        self.actions = actions
         self.fallback = fallback
         self.height = height
         self.separator = separator
         self.spacing = spacing
         self.id = id_
         self.isVisible = isVisible
-        self.json_fields = ['type', 'text', 'color', 'fontType', 'horizontalAlignment', 'isSubtle', 'maxLines', 'size', 'weight', 'wrap', 'style', 'fallback',
-                            'height', 'separator', 'spacing', 'id', 'isVisible']
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(text={self.text})"
-
-    def __str__(self):
-        return self.text
-
+        self.json_fields = ("actions", "fallback", "height", "separator", "spacing", "id", "isVisible")
+    
+    def append_action(self, action: Action):
+        self.actions.append(action)
 
-class Image(Mixin):
-    def __init__(self,
-                 url: str,
-                 altText: Optional[str] = None,
-                 backgroundColor: Optional[str] = None,
-                 height: Optional[str] = None,
-                 horizontalAlignment: Optional[str] = None,
-                 selectAction: Optional[str] = None):
-        self.type = "Image"
-        self.json_fields = ['url', 'altText', 'backgroundColor', 'height', 'horizontalAlignment', 'selectAction']
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        if __value is None:
+            __value = []
+        elif isinstance(__value, Element):
+            __value = [__value]
+        return super().__setattr__(__name, __value)
```

### Comparing `adaptivecard-0.0.9/adaptivecard/mixin.py` & `adaptivecard-0.1.0/adaptivecard/mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import json
-from typing import Any, get_type_hints, Collection
+from typing import Any, get_type_hints, Sequence
 from typeguard import check_type
+from adaptivecard._base_types import Element
 
 
 class Mixin:    # essa é uma classe do tipo mixin. Não tem funcionalidade própria, serve para fornecer funcionalidade a outras classes.
 
     protected_attributes = frozenset(('json_fields', 'type'))
 
     def to_dict(self):
         """
         Returns a json/dictionary representative of the card element
         """
 
         def get_json_dic(obj):
-            # breakpoint()
-            return {key: value for key in obj.json_fields if hasattr(obj, key) and (value := obj.__getattribute__(key)) is not None}
+            return {key: value for key in obj.json_fields if hasattr(obj, key) and (value := getattr(obj, key)) is not None}
 
         # possível problema de circular reference ao passar o mesmo objeto em dois lugares diferentes do card. Averiguar depois.
         dic = json.loads(json.dumps(self, default=lambda obj: get_json_dic(obj)))
         return dic
     
-    def is_collection(self, value):
-        if isinstance(value, Collection) and not isinstance(value, str):
+    def is_sequence(self, value):
+        if isinstance(value, Sequence) and not isinstance(value, str):
             return True
         return False
 
     def __setattr__(self, __name: str, __value: Any) -> None:
         if __name in (type_hints := get_type_hints(self.__init__)):
-            check_type(__name, __value, type_hints[__name])
+                check_type(__value, type_hints[__name])
         if __name in self.protected_attributes and hasattr(self, __name):
             raise AttributeError(f"Can't set '{__name}' attribute")
         super().__setattr__(__name, __value)
 
     def __delattr__(self, __name: str) -> None:
         if __name in self.protected_attributes or hasattr(self, 'json_fields') and __name in self.json_fields:
             raise AttributeError(f"Cannot delete '{__name}' attribute")
+
```

### Comparing `adaptivecard-0.0.9/adaptivecard.egg-info/PKG-INFO` & `adaptivecard-0.1.0/adaptivecard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.0.9
+Version: 0.1.0
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,card,adaptive card,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `adaptivecard-0.0.9/setup.py` & `adaptivecard-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Microsoft Adaptive Cards'
 LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 setup(
     name="adaptivecard",
     version=VERSION,
     author="cabutchei (Luan Paz)",
     author_email="<luropa_paz@hotmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
-        'typeguard'
+        'typeguard',
+        'tabulate'
     ],
     keywords=['python', 'adaptive', 'card', 'adaptive card', 'microsoft'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License", 
         "Programming Language :: Python :: 3",
```

