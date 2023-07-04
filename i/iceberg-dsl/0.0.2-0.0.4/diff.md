# Comparing `tmp/iceberg-dsl-0.0.2.tar.gz` & `tmp/iceberg-dsl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg-dsl-0.0.2.tar", last modified: Wed Jun 21 20:33:16 2023, max compression
+gzip compressed data, was "iceberg-dsl-0.0.4.tar", last modified: Tue Jul  4 22:10:47 2023, max compression
```

## Comparing `iceberg-dsl-0.0.2.tar` & `iceberg-dsl-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.383538 iceberg-dsl-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-21 20:19:08.000000 iceberg-dsl-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3186 2023-06-21 20:33:16.383538 iceberg-dsl-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2044 2023-06-21 20:29:02.000000 iceberg-dsl-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.353821 iceberg-dsl-0.0.2/iceberg/
--rw-rw-rw-   0        0        0      169 2023-06-21 20:33:05.000000 iceberg-dsl-0.0.2/iceberg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.359821 iceberg-dsl-0.0.2/iceberg/core/
--rw-rw-rw-   0        0        0      177 2023-06-11 16:49:29.000000 iceberg-dsl-0.0.2/iceberg/core/__init__.py
--rw-rw-rw-   0        0        0     6192 2023-06-21 18:45:19.000000 iceberg-dsl-0.0.2/iceberg/core/drawable.py
--rw-rw-rw-   0        0        0    12151 2023-06-21 18:31:42.000000 iceberg-dsl-0.0.2/iceberg/core/properties.py
--rw-rw-rw-   0        0        0     3637 2023-06-21 18:42:22.000000 iceberg-dsl-0.0.2/iceberg/core/renderer.py
--rw-rw-rw-   0        0        0     2788 2023-03-01 05:13:30.000000 iceberg-dsl-0.0.2/iceberg/geometry.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.371807 iceberg-dsl-0.0.2/iceberg/primitives/
--rw-rw-rw-   0        0        0      264 2023-06-21 07:45:12.000000 iceberg-dsl-0.0.2/iceberg/primitives/__init__.py
--rw-rw-rw-   0        0        0     1124 2023-06-21 07:44:59.000000 iceberg-dsl-0.0.2/iceberg/primitives/filters.py
--rw-rw-rw-   0        0        0     4244 2023-06-21 07:51:02.000000 iceberg-dsl-0.0.2/iceberg/primitives/latex.py
--rw-rw-rw-   0        0        0    11915 2023-06-21 18:52:10.000000 iceberg-dsl-0.0.2/iceberg/primitives/layout.py
--rw-rw-rw-   0        0        0     3691 2023-06-11 16:28:19.000000 iceberg-dsl-0.0.2/iceberg/primitives/shapes.py
--rw-rw-rw-   0        0        0     1612 2023-06-21 18:52:45.000000 iceberg-dsl-0.0.2/iceberg/primitives/svg.py
--rw-rw-rw-   0        0        0     2227 2023-06-21 07:27:18.000000 iceberg-dsl-0.0.2/iceberg/primitives/text.py
--rw-rw-rw-   0        0        0     1281 2023-06-21 18:54:51.000000 iceberg-dsl-0.0.2/iceberg/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:33:16.382527 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/
--rw-rw-rw-   0        0        0     3186 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 20:33:16.000000 iceberg-dsl-0.0.2/iceberg_dsl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-06-21 20:33:16.385609 iceberg-dsl-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      488 2023-06-21 20:31:57.000000 iceberg-dsl-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.773097 iceberg-dsl-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-21 20:19:08.000000 iceberg-dsl-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5814 2023-07-04 22:10:47.773097 iceberg-dsl-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4672 2023-07-04 18:55:35.000000 iceberg-dsl-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.753097 iceberg-dsl-0.0.4/iceberg/
+-rw-rw-rw-   0        0        0      202 2023-07-03 23:26:54.000000 iceberg-dsl-0.0.4/iceberg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.754097 iceberg-dsl-0.0.4/iceberg/arrows/
+-rw-rw-rw-   0        0        0     7173 2023-06-23 03:25:22.000000 iceberg-dsl-0.0.4/iceberg/arrows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.757098 iceberg-dsl-0.0.4/iceberg/core/
+-rw-rw-rw-   0        0        0      205 2023-06-23 03:35:17.000000 iceberg-dsl-0.0.4/iceberg/core/__init__.py
+-rw-rw-rw-   0        0        0     7938 2023-07-04 18:52:13.000000 iceberg-dsl-0.0.4/iceberg/core/drawable.py
+-rw-rw-rw-   0        0        0    13769 2023-07-04 07:10:50.000000 iceberg-dsl-0.0.4/iceberg/core/properties.py
+-rw-rw-rw-   0        0        0     5090 2023-07-04 21:58:07.000000 iceberg-dsl-0.0.4/iceberg/core/renderer.py
+-rw-rw-rw-   0        0        0     2788 2023-03-01 05:13:30.000000 iceberg-dsl-0.0.4/iceberg/geometry.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.762098 iceberg-dsl-0.0.4/iceberg/primitives/
+-rw-rw-rw-   0        0        0      361 2023-06-28 02:25:22.000000 iceberg-dsl-0.0.4/iceberg/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1124 2023-06-21 07:44:59.000000 iceberg-dsl-0.0.4/iceberg/primitives/filters.py
+-rw-rw-rw-   0        0        0     1542 2023-07-03 22:55:06.000000 iceberg-dsl-0.0.4/iceberg/primitives/image.py
+-rw-rw-rw-   0        0        0     4325 2023-06-23 06:40:33.000000 iceberg-dsl-0.0.4/iceberg/primitives/latex.py
+-rw-rw-rw-   0        0        0    12350 2023-07-04 07:10:50.000000 iceberg-dsl-0.0.4/iceberg/primitives/layout.py
+-rw-rw-rw-   0        0        0     3935 2023-07-04 07:10:50.000000 iceberg-dsl-0.0.4/iceberg/primitives/shapes.py
+-rw-rw-rw-   0        0        0     1612 2023-06-23 04:10:37.000000 iceberg-dsl-0.0.4/iceberg/primitives/svg.py
+-rw-rw-rw-   0        0        0     4338 2023-06-23 05:34:56.000000 iceberg-dsl-0.0.4/iceberg/primitives/text.py
+-rw-rw-rw-   0        0        0     1281 2023-06-21 18:54:51.000000 iceberg-dsl-0.0.4/iceberg/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.767098 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/
+-rw-rw-rw-   0        0        0     5814 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      756 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-04 22:10:47.000000 iceberg-dsl-0.0.4/iceberg_dsl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2023-07-04 22:10:47.774096 iceberg-dsl-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      488 2023-06-21 20:31:57.000000 iceberg-dsl-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:10:47.772097 iceberg-dsl-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-04 19:01:04.000000 iceberg-dsl-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1115 2023-07-04 21:59:42.000000 iceberg-dsl-0.0.4/tests/scene_tester.py
+-rw-rw-rw-   0        0        0      474 2023-07-04 21:58:36.000000 iceberg-dsl-0.0.4/tests/test_blank.py
+-rw-rw-rw-   0        0        0     2315 2023-07-04 22:04:53.000000 iceberg-dsl-0.0.4/tests/test_connect.py
+-rw-rw-rw-   0        0        0     3380 2023-07-04 22:01:27.000000 iceberg-dsl-0.0.4/tests/test_neural_net.py
+-rw-rw-rw-   0        0        0     1137 2023-07-04 22:03:24.000000 iceberg-dsl-0.0.4/tests/test_quickstart.py
```

### Comparing `iceberg-dsl-0.0.2/LICENSE` & `iceberg-dsl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.2/iceberg/core/drawable.py` & `iceberg-dsl-0.0.4/iceberg/core/drawable.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 from abc import ABC, abstractmethod, abstractproperty
 from iceberg.core import Bounds, Corner
 from iceberg.utils import direction_equal
 import numpy as np
 import skia
 
+# Global variable to store the stack of scene contexts.
+_scene_context_stack = []
+
 
 class ChildNotFoundError(ValueError):
     pass
 
 
 class Drawable(ABC):
-    """Asbtract base class for all drawable objects.
+    """Abstract base class for all drawable objects.
 
     Each drawable object must know its bounds, and be able to draw itself on a Skia canvas.
     It may also have children, which are also drawable objects.
 
     You almost always want to inherit from `iceberg.layout.Compose` instead of this class
     so that you can easily compose multiple drawables together without having to worry about
     the details of drawing them on a canvas with skia.
@@ -29,14 +32,36 @@
 
     @abstractmethod
     def draw(self, canvas: skia.Canvas):
         """Execute the Skia drawing commands on the canvas."""
         pass
 
     @property
+    def relative_bounds(self) -> Bounds:
+        """Get the bounds of the drawable relative to the current scene context.
+
+        Example:
+            >>> with some_drawable:
+            >>>     print(child_drawable.relative_bounds)
+
+        The above code will print the bounds of `child_drawable` relative to `some_drawable`.
+        """
+
+        # Go from innermost to outermost context and return the transformed bounds
+        # if self is a child of that context.
+        for scene in reversed(_scene_context_stack):
+            try:
+                return scene.child_bounds(self)
+            except ChildNotFoundError:
+                pass
+
+        # Self is not a child of any context, so raise an error.
+        raise ChildNotFoundError()
+
+    @property
     def children(self) -> Sequence["Drawable"]:
         """Return the children of the drawable."""
         return []
 
     def move(self, x: float, y: float):
         """Move the drawable by the specified amount."""
         from iceberg.primitives.layout import Transform
@@ -76,30 +101,47 @@
         from iceberg.primitives.layout import Padding
 
         return Padding(
             child=self,
             padding=padding,
         )
 
+    def crop(self, bounds: Bounds) -> "Drawable":
+        """Crop the drawable to the specified bounds."""
+        from iceberg import Colors
+        from iceberg.primitives.layout import Anchor, Blank
+
+        blank = Blank(bounds, Colors.TRANSPARENT)
+
+        return Anchor(
+            [blank, self],
+        )
+
     def next_to(
-        self, other: "Drawable", direction: np.ndarray = np.zeros(2)
+        self,
+        other: "Drawable",
+        direction: np.ndarray = np.zeros(2),
+        no_gap: bool = False,
     ) -> "Drawable":
         """Place another drawable next to this one, and return the new drawable.
 
         The `direction` parameter specifies the direction to place the other drawable.
 
         Example:
             >>> from iceberg.primitives import Rectangle, Directions
             >>> rect1 = Rectangle(100, 100)
             >>> rect2 = Rectangle(100, 100)
             >>> rect1_and_rect2 = rect1.next_to(rect2, Directions.RIGHT * 10)
 
         Args:
             other: The other drawable to place next to this one.
             direction: The direction to place the other drawable. This is a 2D vector.
+            no_gap: If True, the other drawable will be placed right next to this one, with no gap.
+                The scale of `direction` is ignored in this case (`direction` is only used
+                to determine which corners to align).
 
         Returns:
             The new drawable that contains both this drawable and the other drawable.
         """
 
         from iceberg.primitives.layout import Align, Directions
 
@@ -120,17 +162,20 @@
         elif direction_equal(direction, Directions.LEFT):
             anchor_corner = Corner.MIDDLE_LEFT
             other_corner = Corner.MIDDLE_RIGHT
         elif direction_equal(direction, Directions.UP):
             anchor_corner = Corner.TOP_MIDDLE
             other_corner = Corner.BOTTOM_MIDDLE
 
+        if no_gap:
+            direction = Directions.ORIGIN
+
         return Align(self, other, anchor_corner, other_corner, direction)
 
-    def center_to(self, other: "Drawable") -> "Drawable":
+    def add_centered(self, other: "Drawable") -> "Drawable":
         """Place another drawable in the center of this one, and return the new drawable.
 
         Args:
             other: The other drawable to place in the center of this one.
 
         Returns:
             The new drawable that contains both this drawable and the other drawable.
@@ -182,7 +227,13 @@
 
         Raises:
             ChildNotFoundError: If the specified child is not a child of this drawable.
         """
 
         transform = self.child_transform(search_child)
         return search_child.bounds.transform(transform)
+
+    def __enter__(self):
+        _scene_context_stack.append(self)
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        assert _scene_context_stack.pop() is self
```

### Comparing `iceberg-dsl-0.0.2/iceberg/core/properties.py` & `iceberg-dsl-0.0.4/iceberg/core/properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from dataclasses import dataclass
-from typing import Tuple
+
+from typing import List, Optional, Tuple
+from enum import Enum
 
 import skia
 import numpy as np
 
 from iceberg.geometry import apply_transform
 
 
@@ -117,24 +119,27 @@
     def height(self) -> float:
         return self.bottom - self.top
 
     @property
     def center(self) -> Tuple[float, float]:
         return (self.left + self.right) / 2, (self.top + self.bottom) / 2
 
-    def inset(self, dx: float, dy: float) -> "Bounds":
+    def inset(self, dx: float, dy: Optional[float] = None) -> "Bounds":
         """Inset the bounds by the specified amount.
 
         Args:
             dx: The amount to inset the bounds in the x direction.
             dy: The amount to inset the bounds in the y direction.
+                If `None`, then `dx` is used.
 
         Returns:
             The inset bounds.
         """
+        if dy is None:
+            dy = dx
 
         return Bounds(
             left=self.left + dx,
             right=self.right - dx,
             top=self.top + dy,
             bottom=self.bottom - dy,
         )
@@ -380,35 +385,55 @@
     BLUE = Color.from_hex("#0000FF")
     YELLOW = Color.from_hex("#FFFF00")
     CYAN = Color.from_hex("#00FFFF")
     MAGENTA = Color.from_hex("#FF00FF")
     TRANSPARENT = Color.from_rgba(0, 0, 0, 0)
 
 
+class StrokeCap(Enum):
+    """The cap at the end of a stroke."""
+
+    BUTT = skia.Paint.kButt_Cap
+    ROUND = skia.Paint.kRound_Cap
+    SQUARE = skia.Paint.kSquare_Cap
+
+
 class PathStyle(object):
     """A style for drawing paths."""
 
-    def __init__(self, color: Color, thickness: float = 1.0, anti_alias: bool = True):
+    def __init__(
+        self,
+        color: Color,
+        thickness: float = 1.0,
+        anti_alias: bool = True,
+        stroke: bool = True,
+        stroke_cap: StrokeCap = StrokeCap.BUTT,
+    ):
         """Create a path style.
 
         Args:
             color: The color of the path.
             thickness: The thickness of the path.
             anti_alias: Whether to use anti-aliasing.
+            stroke: Whether to stroke the path or fill it.
+            stroke_cap: The cap at the end of a stroke.
         """
 
         self._color = color
         self._thickness = thickness
         self._anti_alias = anti_alias
+        self._stroke = stroke
+        self._stroke_cap = stroke_cap
 
         self._skia_paint = skia.Paint(
-            Style=skia.Paint.kStroke_Style,
+            Style=skia.Paint.kStroke_Style if stroke else skia.Paint.kFill_Style,
             AntiAlias=anti_alias,
             StrokeWidth=thickness,
             Color4f=color.to_skia(),
+            StrokeCap=stroke_cap.value,
         )
 
     @property
     def color(self) -> Color:
         return self._color
 
     @property
@@ -422,26 +447,50 @@
     @property
     def skia_paint(self) -> skia.Paint:
         return self._skia_paint
 
 
 @dataclass
 class FontStyle(object):
+    class Style(Enum):
+        NORMAL = skia.FontStyle.Normal()
+        ITALIC = skia.FontStyle.Italic()
+        BOLD = skia.FontStyle.Bold()
+        BOLD_ITALIC = skia.FontStyle.BoldItalic()
+
     family: str
+    filename: str = None
     size: float = 16
     font_weight: int = 400
-    font_style: int = 0
+    font_style: Style = Style.NORMAL
     color: Color = Color(0, 0, 0)
     anti_alias: bool = True
 
+    def __post_init__(self):
+        families = set(FontStyle.available_fonts())
+        if self.filename is None and not self.family in families:
+            raise ValueError(
+                f"Invalid font family: {self.family}. Please call FontStyle.get_available_fonts_families() to get the list of available fonts."
+            )
+
     def get_skia_paint(self) -> skia.Paint:
         return skia.Paint(
             Style=skia.Paint.kFill_Style,
             AntiAlias=self.anti_alias,
             Color4f=self.color.to_skia(),
         )
 
     def get_skia_font(self) -> skia.Font:
+        if self.filename is not None:
+            return skia.Font(
+                skia.Typeface.MakeFromFile(self.filename, self.font_style.value),
+                self.size,
+            )
+
         return skia.Font(
-            skia.Typeface(self.family),
+            skia.Typeface(self.family, self.font_style.value),
             self.size,
         )
+
+    @staticmethod
+    def available_fonts() -> List[str]:
+        return list(skia.FontMgr())
```

### Comparing `iceberg-dsl-0.0.2/iceberg/geometry.py` & `iceberg-dsl-0.0.4/iceberg/geometry.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.2/iceberg/primitives/filters.py` & `iceberg-dsl-0.0.4/iceberg/primitives/filters.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.2/iceberg/primitives/latex.py` & `iceberg-dsl-0.0.4/iceberg/primitives/latex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Latex rendering adapted from
+https://github.com/ManimCommunity/manim
+"""
+
 from absl import logging
 
 import os
 import re
 
 import skia
 from iceberg.primitives.layout import Transform
```

### Comparing `iceberg-dsl-0.0.2/iceberg/primitives/layout.py` & `iceberg-dsl-0.0.4/iceberg/primitives/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,26 @@
 
     def __init__(
         self,
         child: Drawable,
         position: Tuple[float, float] = (0, 0),
         scale: Tuple[float, float] = (1, 1),
         anchor: Tuple[float, float] = (0, 0),
+        rotation: float = 0.0,
+        rotation_in_degrees: bool = True,
     ):
         """Initialize a transform drawable.
 
         Args:
             child: The child drawable to transform.
             position: The position of the child drawable.
             scale: The scale of the child drawable.
             anchor: The anchor of the child drawable.
+            rotation: The rotation of the child drawable.
+            rotation_in_degrees: Whether the rotation is in degrees.
         """
 
         super().__init__()
 
         self._child = child
         self._position = position
         self._scale = scale
@@ -86,14 +90,16 @@
         left, top = self._child_bounds.left, self._child_bounds.top
         right, bottom = self._child_bounds.right, self._child_bounds.bottom
 
         self._transform = get_transform(
             position=self._position,
             scale=self._scale,
             anchor=self._anchor,
+            rotation=rotation,
+            in_degrees=rotation_in_degrees,
         )
         self._skia_matrix = skia.Matrix(self._transform)
 
         # Transform the corners of the child's bounds.
         transformed_corners = apply_transform(
             points=[
                 (left, top),
@@ -180,24 +186,23 @@
 
         self._padding = padding
         self._child_bounds = self._child.bounds
 
         pl, pt, pr, pb = self._padding
 
         self._padded_bounds = Bounds(
-            left=self._child_bounds.left,
-            top=self._child_bounds.top,
-            right=self._child_bounds.right + pl + pr,
-            bottom=self._child_bounds.bottom + pt + pb,
+            left=self._child_bounds.left - pl,
+            top=self._child_bounds.top - pt,
+            right=self._child_bounds.right + pr,
+            bottom=self._child_bounds.bottom + pb,
         )
 
         super().__init__(
             child=child,
-            position=(pl, pt),
-            anchor=(0, 0),
+            position=(0, 0),
         )
 
     @property
     def bounds(self) -> Bounds:
         return self._padded_bounds
 
 
@@ -349,15 +354,20 @@
         next_to_direction = (
             Directions.RIGHT
             if arrange_direction == Arrange.Direction.HORIZONTAL
             else Directions.DOWN
         )
         arrangement = children[0]
         for next_child in children[1:]:
-            arrangement = arrangement.next_to(next_child, next_to_direction * gap)
+            if gap == 0:
+                arrangement = arrangement.next_to(
+                    next_child, next_to_direction, no_gap=True
+                )
+            else:
+                arrangement = arrangement.next_to(next_child, next_to_direction * gap)
 
         super().__init__([arrangement])
 
 
 class Grid(Compose):
     def __init__(self, children_matrix: List[List[Drawable]], gap=0):
         """Initialize a grid drawable.
```

### Comparing `iceberg-dsl-0.0.2/iceberg/primitives/shapes.py` & `iceberg-dsl-0.0.4/iceberg/primitives/shapes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Tuple, Union
 import skia
 
 from iceberg import Drawable, Bounds, Color
 from iceberg.core import Bounds
 from iceberg.core.properties import PathStyle
 from iceberg.geometry import get_transform, apply_transform
 from dataclasses import dataclass
@@ -22,14 +22,15 @@
 class Rectangle(Drawable):
     rectangle: Bounds
     border_color: Color = None
     fill_color: Color = None
     border_thickness: float = 1.0
     anti_alias: bool = True
     border_position: BorderPosition = BorderPosition.CENTER
+    border_radius: Union[float, Tuple[float, float]] = 0.0
 
     def __post_init__(
         self,
     ) -> None:
         self._border_paint = (
             skia.Paint(
                 Style=skia.Paint.kStroke_Style,
@@ -74,19 +75,24 @@
     @property
     def bounds(self) -> Bounds:
         return self._bounds
 
     def draw(self, canvas):
         self.__post_init__()
 
+        if isinstance(self.border_radius, tuple):
+            rx, ry = self.border_radius
+        else:
+            rx = ry = self.border_radius
+
         if self._fill_paint:
-            canvas.drawRect(self._skia_rect, self._fill_paint)
+            canvas.drawRoundRect(self._skia_rect, rx, ry, self._fill_paint)
 
         if self._border_paint:
-            canvas.drawRect(self._border_skia_rect, self._border_paint)
+            canvas.drawRoundRect(self._border_skia_rect, rx, ry, self._border_paint)
 
 
 @dataclass
 class Ellipse(Rectangle):
     def draw(self, canvas):
         self.__post_init__()
```

### Comparing `iceberg-dsl-0.0.2/iceberg/primitives/svg.py` & `iceberg-dsl-0.0.4/iceberg/primitives/svg.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.2/iceberg/utils.py` & `iceberg-dsl-0.0.4/iceberg/utils.py`

 * *Files identical despite different names*

### Comparing `iceberg-dsl-0.0.2/iceberg_dsl.egg-info/SOURCES.txt` & `iceberg-dsl-0.0.4/iceberg_dsl.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 iceberg/__init__.py
 iceberg/geometry.py
 iceberg/utils.py
+iceberg/arrows/__init__.py
 iceberg/core/__init__.py
 iceberg/core/drawable.py
 iceberg/core/properties.py
 iceberg/core/renderer.py
 iceberg/primitives/__init__.py
 iceberg/primitives/filters.py
+iceberg/primitives/image.py
 iceberg/primitives/latex.py
 iceberg/primitives/layout.py
 iceberg/primitives/shapes.py
 iceberg/primitives/svg.py
 iceberg/primitives/text.py
 iceberg_dsl.egg-info/PKG-INFO
 iceberg_dsl.egg-info/SOURCES.txt
 iceberg_dsl.egg-info/dependency_links.txt
 iceberg_dsl.egg-info/requires.txt
-iceberg_dsl.egg-info/top_level.txt
+iceberg_dsl.egg-info/top_level.txt
+tests/__init__.py
+tests/scene_tester.py
+tests/test_blank.py
+tests/test_connect.py
+tests/test_neural_net.py
+tests/test_quickstart.py
```

### Comparing `iceberg-dsl-0.0.2/setup.cfg` & `iceberg-dsl-0.0.4/setup.cfg`

 * *Files identical despite different names*

