# Comparing `tmp/pysvgedit-0.0.3.tar.gz` & `tmp/pysvgedit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysvgedit-0.0.3.tar", last modified: Thu Jun 22 22:08:45 2023, max compression
+gzip compressed data, was "pysvgedit-0.0.4.tar", last modified: Tue Jul  4 22:28:51 2023, max compression
```

## Comparing `pysvgedit-0.0.3.tar` & `pysvgedit-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/
--rw-------   0 joe       (1000) joe       (1000)    35142 2023-06-18 18:53:00.000000 pysvgedit-0.0.3/LICENSE
--rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)      207 2023-06-20 07:23:51.000000 pysvgedit-0.0.3/README.md
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/pysvgedit/
--rw-------   0 joe       (1000) joe       (1000)      975 2023-06-22 13:27:51.000000 pysvgedit-0.0.3/pysvgedit/Exceptions.py
--rw-------   0 joe       (1000) joe       (1000)     4993 2023-06-22 16:21:37.000000 pysvgedit-0.0.3/pysvgedit/SVGAnimation.py
--rw-------   0 joe       (1000) joe       (1000)     1377 2023-06-22 17:42:00.000000 pysvgedit-0.0.3/pysvgedit/SVGCircle.py
--rw-------   0 joe       (1000) joe       (1000)     1005 2023-06-18 08:01:04.000000 pysvgedit-0.0.3/pysvgedit/SVGDefs.py
--rw-------   0 joe       (1000) joe       (1000)     3259 2023-06-22 20:08:06.000000 pysvgedit-0.0.3/pysvgedit/SVGDocument.py
--rw-------   0 joe       (1000) joe       (1000)     1422 2023-06-18 17:58:55.000000 pysvgedit-0.0.3/pysvgedit/SVGGroup.py
--rw-------   0 joe       (1000) joe       (1000)     4774 2023-06-22 20:09:10.000000 pysvgedit-0.0.3/pysvgedit/SVGObject.py
--rw-------   0 joe       (1000) joe       (1000)     7539 2023-06-22 21:53:42.000000 pysvgedit-0.0.3/pysvgedit/SVGPath.py
--rw-------   0 joe       (1000) joe       (1000)     1513 2023-06-22 17:50:27.000000 pysvgedit-0.0.3/pysvgedit/SVGRect.py
--rw-------   0 joe       (1000) joe       (1000)     4340 2023-06-22 17:34:07.000000 pysvgedit-0.0.3/pysvgedit/SVGStyle.py
--rw-------   0 joe       (1000) joe       (1000)     3007 2023-06-22 21:05:48.000000 pysvgedit-0.0.3/pysvgedit/SVGText.py
--rw-------   0 joe       (1000) joe       (1000)     1708 2023-06-22 18:25:55.000000 pysvgedit-0.0.3/pysvgedit/SVGTransformation.py
--rw-------   0 joe       (1000) joe       (1000)     2466 2023-06-22 15:53:47.000000 pysvgedit-0.0.3/pysvgedit/SVGValidator.py
--rw-------   0 joe       (1000) joe       (1000)     1693 2023-06-22 18:01:49.000000 pysvgedit-0.0.3/pysvgedit/Vector2D.py
--rw-------   0 joe       (1000) joe       (1000)     1967 2023-06-18 18:50:02.000000 pysvgedit-0.0.3/pysvgedit/XMLTools.py
--rw-------   0 joe       (1000) joe       (1000)     1385 2023-06-22 22:08:02.000000 pysvgedit-0.0.3/pysvgedit/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/pysvgedit/apps/
--rw-------   0 joe       (1000) joe       (1000)     3109 2023-06-22 16:15:36.000000 pysvgedit-0.0.3/pysvgedit/apps/AnimationRendererApp.py
--rw-------   0 joe       (1000) joe       (1000)     3101 2023-06-18 08:03:19.000000 pysvgedit-0.0.3/pysvgedit/apps/FriendlyArgumentParser.py
--rw-------   0 joe       (1000) joe       (1000)     4243 2023-06-22 15:58:07.000000 pysvgedit-0.0.3/pysvgedit/apps/MakoRendererApp.py
--rw-------   0 joe       (1000) joe       (1000)     1536 2023-06-22 15:58:00.000000 pysvgedit-0.0.3/pysvgedit/apps/ValidatorApp.py
--rw-------   0 joe       (1000) joe       (1000)      841 2023-06-18 08:03:02.000000 pysvgedit-0.0.3/pysvgedit/apps/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/pysvgedit.egg-info/
--rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)      738 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/SOURCES.txt
--rw-------   0 joe       (1000) joe       (1000)        1 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/dependency_links.txt
--rw-------   0 joe       (1000) joe       (1000)      229 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/entry_points.txt
--rw-------   0 joe       (1000) joe       (1000)       10 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/top_level.txt
--rw-------   0 joe       (1000) joe       (1000)       38 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/setup.cfg
--rw-------   0 joe       (1000) joe       (1000)     1438 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/setup.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-07-04 22:28:51.683052 pysvgedit-0.0.4/
+-rw-------   0 joe       (1000) joe       (1000)    35142 2023-06-18 18:53:00.000000 pysvgedit-0.0.4/LICENSE
+-rw-------   0 joe       (1000) joe       (1000)     1178 2023-07-04 22:28:51.683052 pysvgedit-0.0.4/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)      207 2023-06-20 07:23:51.000000 pysvgedit-0.0.4/README.md
+drwx------   0 joe       (1000) joe       (1000)        0 2023-07-04 22:28:51.683052 pysvgedit-0.0.4/pysvgedit/
+-rw-------   0 joe       (1000) joe       (1000)     5723 2023-07-04 22:18:44.000000 pysvgedit-0.0.4/pysvgedit/Convenience.py
+-rw-------   0 joe       (1000) joe       (1000)     1022 2023-07-03 18:18:58.000000 pysvgedit-0.0.4/pysvgedit/Exceptions.py
+-rw-------   0 joe       (1000) joe       (1000)     4993 2023-06-22 16:21:37.000000 pysvgedit-0.0.4/pysvgedit/SVGAnimation.py
+-rw-------   0 joe       (1000) joe       (1000)     1638 2023-07-04 11:41:56.000000 pysvgedit-0.0.4/pysvgedit/SVGCircle.py
+-rw-------   0 joe       (1000) joe       (1000)     1360 2023-07-03 21:52:04.000000 pysvgedit-0.0.4/pysvgedit/SVGDefs.py
+-rw-------   0 joe       (1000) joe       (1000)     3306 2023-07-04 17:08:22.000000 pysvgedit-0.0.4/pysvgedit/SVGDocument.py
+-rw-------   0 joe       (1000) joe       (1000)     1422 2023-06-18 17:58:55.000000 pysvgedit-0.0.4/pysvgedit/SVGGroup.py
+-rw-------   0 joe       (1000) joe       (1000)     2632 2023-07-04 22:18:24.000000 pysvgedit-0.0.4/pysvgedit/SVGImage.py
+-rw-------   0 joe       (1000) joe       (1000)     6287 2023-07-04 22:19:17.000000 pysvgedit-0.0.4/pysvgedit/SVGObject.py
+-rw-------   0 joe       (1000) joe       (1000)    10110 2023-07-04 17:35:42.000000 pysvgedit-0.0.4/pysvgedit/SVGPath.py
+-rw-------   0 joe       (1000) joe       (1000)     1633 2023-07-04 09:17:55.000000 pysvgedit-0.0.4/pysvgedit/SVGRect.py
+-rw-------   0 joe       (1000) joe       (1000)     4340 2023-06-22 17:34:07.000000 pysvgedit-0.0.4/pysvgedit/SVGStyle.py
+-rw-------   0 joe       (1000) joe       (1000)     3414 2023-07-04 07:21:37.000000 pysvgedit-0.0.4/pysvgedit/SVGText.py
+-rw-------   0 joe       (1000) joe       (1000)     1708 2023-06-22 18:25:55.000000 pysvgedit-0.0.4/pysvgedit/SVGTransformation.py
+-rw-------   0 joe       (1000) joe       (1000)     2466 2023-06-22 15:53:47.000000 pysvgedit-0.0.4/pysvgedit/SVGValidator.py
+-rw-------   0 joe       (1000) joe       (1000)     6477 2023-07-04 22:19:07.000000 pysvgedit-0.0.4/pysvgedit/Vector2D.py
+-rw-------   0 joe       (1000) joe       (1000)     3076 2023-07-03 21:50:38.000000 pysvgedit-0.0.4/pysvgedit/XMLTools.py
+-rw-------   0 joe       (1000) joe       (1000)     1489 2023-07-04 22:28:42.000000 pysvgedit-0.0.4/pysvgedit/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-07-04 22:28:51.683052 pysvgedit-0.0.4/pysvgedit/apps/
+-rw-------   0 joe       (1000) joe       (1000)     3109 2023-06-22 16:15:36.000000 pysvgedit-0.0.4/pysvgedit/apps/AnimationRendererApp.py
+-rw-------   0 joe       (1000) joe       (1000)     3101 2023-06-18 08:03:19.000000 pysvgedit-0.0.4/pysvgedit/apps/FriendlyArgumentParser.py
+-rw-------   0 joe       (1000) joe       (1000)     4243 2023-06-22 15:58:07.000000 pysvgedit-0.0.4/pysvgedit/apps/MakoRendererApp.py
+-rw-------   0 joe       (1000) joe       (1000)     1536 2023-06-22 15:58:00.000000 pysvgedit-0.0.4/pysvgedit/apps/ValidatorApp.py
+-rw-------   0 joe       (1000) joe       (1000)      841 2023-06-18 08:03:02.000000 pysvgedit-0.0.4/pysvgedit/apps/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-07-04 22:28:51.683052 pysvgedit-0.0.4/pysvgedit.egg-info/
+-rw-------   0 joe       (1000) joe       (1000)     1178 2023-07-04 22:28:51.000000 pysvgedit-0.0.4/pysvgedit.egg-info/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)      785 2023-07-04 22:28:51.000000 pysvgedit-0.0.4/pysvgedit.egg-info/SOURCES.txt
+-rw-------   0 joe       (1000) joe       (1000)        1 2023-07-04 22:28:51.000000 pysvgedit-0.0.4/pysvgedit.egg-info/dependency_links.txt
+-rw-------   0 joe       (1000) joe       (1000)      229 2023-07-04 22:28:51.000000 pysvgedit-0.0.4/pysvgedit.egg-info/entry_points.txt
+-rw-------   0 joe       (1000) joe       (1000)       10 2023-07-04 22:28:51.000000 pysvgedit-0.0.4/pysvgedit.egg-info/top_level.txt
+-rw-------   0 joe       (1000) joe       (1000)       38 2023-07-04 22:28:51.683052 pysvgedit-0.0.4/setup.cfg
+-rw-------   0 joe       (1000) joe       (1000)     1438 2023-07-04 22:28:51.000000 pysvgedit-0.0.4/setup.py
```

### Comparing `pysvgedit-0.0.3/LICENSE` & `pysvgedit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/PKG-INFO` & `pysvgedit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysvgedit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Native Python library to create and edit SVG documents
 Home-page: https://github.com/johndoe31415/pysvgedit
-Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.4.tar.gz
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
 Keywords: svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pysvgedit-0.0.3/pysvgedit/Exceptions.py` & `pysvgedit-0.0.4/pysvgedit/Exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,7 +17,8 @@
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
 class SVGException(Exception): pass
 class SVGValidationException(SVGException): pass
 class SVGInputFileException(SVGException): pass
+class SVGLibUsageException(SVGException): pass
```

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGAnimation.py` & `pysvgedit-0.0.4/pysvgedit/SVGAnimation.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGCircle.py` & `pysvgedit-0.0.4/pysvgedit/SVGCircle.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,38 @@
 #	GNU General Public License for more details.
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
+import math
 from .SVGObject import SVGObject, SVGXYObject, SVGStyleObject
+from .Vector2D import Vector2D
 
 @SVGObject.register
 class SVGCircle(SVGObject, SVGXYObject, SVGStyleObject):
 	_TAG_NAME = "circle"
 	_X_ATTRIBUTE_NAME = "cx"
-	_X_ATTRIBUTE_NAME = "cy"
+	_Y_ATTRIBUTE_NAME = "cy"
 
 	@property
 	def radius(self):
 		return self._get_float_attribute("r")
 
 	@radius.setter
 	def radius(self, value):
 		self.node.setAttribute("r", str(float(value)))
 
+	def hull_vertices(self, max_interpolation_count = 100):
+		pos = self.pos
+		r = self.radius
+		for i in range(max_interpolation_count):
+			yield pos + (r * Vector2D.angled((i / max_interpolation_count) * 2 * math.pi))
+
 	@classmethod
 	def new(cls, pos, radius):
 		path = cls(cls._new_element())
 		path.pos = pos
 		path.radius = radius
 		path.style.default_path()
 		return path
```

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGDefs.py` & `pysvgedit-0.0.4/pysvgedit/SVGDefs.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,23 @@
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
 from .SVGObject import SVGObject
+from .XMLTools import XMLTools
 
 @SVGObject.register
 class SVGDefs(SVGObject):
 	_TAG_NAME = "defs"
 
 	@classmethod
 	def new(cls):
 		return cls(cls._new_element())
+
+	def get(self, shape_spec):
+		if (shape_spec is not None) and shape_spec.startswith("url(#") and shape_spec.endswith(")"):
+			shape_id = shape_spec[5 : -1]
+			node = XMLTools.find_first_element(self.node, constraint = lambda node: node.getAttribute("id") == shape_id)
+			return SVGObject.attempt_handle(node)
+		return None
```

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGDocument.py` & `pysvgedit-0.0.4/pysvgedit/SVGDocument.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 from .XMLTools import XMLTools
 
 class SVGDocument(SVGObject, SVGWidthHeightObject):
 	_TAG_NAME = "svg"
 	_DEFAULT_WIDTH = 300
 	_DEFAULT_HEIGHT = 150
 	_NAMESPACES = {
-		"inkscape": "http://www.inkscape.org/namespaces/inkscape",
-		"sodipodi": "http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd",
-		"svg": "http://www.w3.org/2000/svg",
-		"rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
-		"cc": "http://creativecommons.org/ns#",
-		"dc": "http://purl.org/dc/elements/1.1/",
+		"inkscape":	"http://www.inkscape.org/namespaces/inkscape",
+		"sodipodi":	"http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd",
+		"svg":		"http://www.w3.org/2000/svg",
+		"rdf":		"http://www.w3.org/1999/02/22-rdf-syntax-ns#",
+		"cc":		"http://creativecommons.org/ns#",
+		"dc":		"http://purl.org/dc/elements/1.1/",
+		"xlink":	"http://www.w3.org/1999/xlink",
 	}
 
 	def __init__(self, svg_node):
 		super().__init__(svg_node)
 		svg_node.ownerDocument._pysvgedit = self
 		self._used_ids = set(node.getAttribute("id") for node in XMLTools.walk_elements(svg_node) if node.hasAttribute("id"))
```

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGGroup.py` & `pysvgedit-0.0.4/pysvgedit/SVGGroup.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGRect.py` & `pysvgedit-0.0.4/pysvgedit/SVGRect.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 	def p3(self):
 		return self.pos + self.extents
 
 	@property
 	def p4(self):
 		return Vector2D(self.pos.x + self.extents.x, self.pos.y)
 
+	def hull_vertices(self, max_interpolation_count = 4):
+		yield self.p1
+		yield self.p2
+		yield self.p3
+		yield self.p4
+
 	@classmethod
 	def new(cls, pos, extents):
-		path = cls(cls._new_element())
-		path.pos = pos
-		path.extents = extents
-		path.style.default_path()
-		return path
+		rect = cls(cls._new_element())
+		rect.pos = pos
+		rect.extents = extents
+		rect.style.default_path()
+		return rect
```

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGStyle.py` & `pysvgedit-0.0.4/pysvgedit/SVGStyle.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGText.py` & `pysvgedit-0.0.4/pysvgedit/SVGText.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,23 @@
 				svg_text.style.shape_inside = rect
 			svg_text.post_add_hook = post_add_hook
 
 		svg_text.style.default_text()
 		svg_text.node.appendChild(SVGTextSpan.new(pos = pos, text = text).node)
 		return svg_text
 
+	def hull_vertices(self, max_interpolation_count = 4):
+		inside_shape = self.svg_document.defs.get(self.style.shape_inside)
+		if inside_shape is not None:
+			# If inside shape is defined, all is well; otherwise we would need
+			# to render the actual text/glyphs to determine the extents, which
+			# we don't do.
+			yield from inside_shape.hull_vertices(max_interpolation_count = max_interpolation_count)
+
+
 	@property
 	def tspans(self):
 		return (SVGTextSpan(node) for node in XMLTools.find_all_elements(self.node, "tspan"))
 
 	@property
 	def tspan(self):
 		return next(self.tspans)
```

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGTransformation.py` & `pysvgedit-0.0.4/pysvgedit/SVGTransformation.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/SVGValidator.py` & `pysvgedit-0.0.4/pysvgedit/SVGValidator.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/XMLTools.py` & `pysvgedit-0.0.4/pysvgedit/XMLTools.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,30 +18,45 @@
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
 import xml.dom.minidom
 
 class XMLTools():
 	@classmethod
-	def find_all_elements(cls, node, tagname):
-		return (child for child in node.childNodes if (child.nodeType == child.ELEMENT_NODE) and (child.tagName == tagname))
+	def find_all_elements(cls, node, tagname = None, constraint = None):
+		return (child for child in node.childNodes if (child.nodeType == child.ELEMENT_NODE) and ((tagname is None) or (child.tagName == tagname)) and ((constraint is None) or constraint(child)))
 
 	@classmethod
-	def find_first_element(cls, node, tagname):
-		return next(cls.find_all_elements(node, tagname))
+	def find_first_element(cls, node, tagname = None, constraint = None):
+		return next(cls.find_all_elements(node, tagname, constraint))
 
 	@classmethod
 	def walk_elements(cls, node, tagname = None, constraint = None):
 		if node.nodeType == node.ELEMENT_NODE:
 			if ((constraint is None) or (constraint(node))) and ((tagname is None) or (node.tagName == tagname)):
 				yield node
 			for child in node.childNodes:
 				yield from cls.walk_elements(child, tagname = tagname, constraint = constraint)
 
 	@classmethod
+	def _walk_elements_with_context(cls, node, context, transform_context_function, exclude, parent = None):
+		yield (node, context)
+		for child in node.childNodes:
+			if (child.nodeType == child.ELEMENT_NODE) and (child.tagName not in exclude):
+				child_context = transform_context_function(context, parent, child)
+				yield from cls._walk_elements_with_context(child, child_context, transform_context_function, exclude, parent = node)
+
+	@classmethod
+	def walk_elements_with_context(cls, node, root_context, transform_context_function, exclude = None):
+		assert(node.nodeType == node.ELEMENT_NODE)
+		if exclude is None:
+			exclude = tuple()
+		yield from cls._walk_elements_with_context(node = node, context = root_context, transform_context_function = transform_context_function, exclude = exclude)
+
+	@classmethod
 	def default_get_attribute(cls, node, name, default_value = None):
 		if node.hasAttribute(name):
 			return node.getAttribute(name)
 		else:
 			return default_value
 
 	@classmethod
@@ -50,7 +65,14 @@
 		element = doc.createElement(tagname)
 		return element
 
 	@classmethod
 	def try_remove_attribute(cls, node, name):
 		if node.hasAttribute(name):
 			node.removeAttribute(name)
+
+	@classmethod
+	def all_parent_elements(cls, node):
+		while node is not None:
+			if node.nodeType == node.ELEMENT_NODE:
+				yield node
+			node = node.parentNode
```

### Comparing `pysvgedit-0.0.3/pysvgedit/__init__.py` & `pysvgedit-0.0.4/pysvgedit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 #	GNU General Public License for more details.
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
-from .Vector2D import Vector2D
+from .Vector2D import Vector2D, TransformationMatrix, SVGTransform
 from .SVGDefs import SVGDefs
 from .SVGDocument import SVGDocument
 from .SVGGroup import SVGGroup
 from .SVGStyle import SVGStyle
 from .SVGRect import SVGRect
 from .SVGCircle import SVGCircle
 from .SVGText import SVGText
 from .SVGPath import SVGPath
+from .SVGImage import SVGImage
 from .SVGAnimation import SVGAnimation, SVGAnimationMode
 from .SVGValidator import SVGValidator, SVGValidatorErrorClass
 from .SVGTransformation import FormatTextTransformation, ChangeVisibilityTransformation
+from .Convenience import Convenience
 from .Exceptions import SVGException
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
```

### Comparing `pysvgedit-0.0.3/pysvgedit/apps/AnimationRendererApp.py` & `pysvgedit-0.0.4/pysvgedit/apps/AnimationRendererApp.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/apps/FriendlyArgumentParser.py` & `pysvgedit-0.0.4/pysvgedit/apps/FriendlyArgumentParser.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/apps/MakoRendererApp.py` & `pysvgedit-0.0.4/pysvgedit/apps/MakoRendererApp.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/apps/ValidatorApp.py` & `pysvgedit-0.0.4/pysvgedit/apps/ValidatorApp.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit/apps/__init__.py` & `pysvgedit-0.0.4/pysvgedit/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.3/pysvgedit.egg-info/PKG-INFO` & `pysvgedit-0.0.4/pysvgedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysvgedit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Native Python library to create and edit SVG documents
 Home-page: https://github.com/johndoe31415/pysvgedit
-Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.4.tar.gz
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
 Keywords: svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pysvgedit-0.0.3/pysvgedit.egg-info/SOURCES.txt` & `pysvgedit-0.0.4/pysvgedit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 setup.py
+pysvgedit/Convenience.py
 pysvgedit/Exceptions.py
 pysvgedit/SVGAnimation.py
 pysvgedit/SVGCircle.py
 pysvgedit/SVGDefs.py
 pysvgedit/SVGDocument.py
 pysvgedit/SVGGroup.py
+pysvgedit/SVGImage.py
 pysvgedit/SVGObject.py
 pysvgedit/SVGPath.py
 pysvgedit/SVGRect.py
 pysvgedit/SVGStyle.py
 pysvgedit/SVGText.py
 pysvgedit/SVGTransformation.py
 pysvgedit/SVGValidator.py
```

### Comparing `pysvgedit-0.0.3/setup.py` & `pysvgedit-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md") as f:
 	long_description = f.read()
 
 setuptools.setup(
 	name = "pysvgedit",
 	packages = setuptools.find_packages(),
-	version = "0.0.3",
+	version = "0.0.4",
 	license = "gpl-3.0",
 	description = "Native Python library to create and edit SVG documents",
 	long_description = long_description,
 	long_description_content_type = "text/markdown",
 	author = "Johannes Bauer",
 	author_email = "joe@johannes-bauer.com",
 	url = "https://github.com/johndoe31415/pysvgedit",
-	download_url = "https://github.com/johndoe31415/pysvgedit/archive/v0.0.3.tar.gz",
+	download_url = "https://github.com/johndoe31415/pysvgedit/archive/v0.0.4.tar.gz",
 	keywords = [ "svg" ],
 	install_requires = [
 	],
 	entry_points = {
 		"console_scripts": [
 			"svgmakorender = pysvgedit.apps.MakoRendererApp:MakoRendererApp.main",
 			"svganimationrender = pysvgedit.apps.AnimationRendererApp:AnimationRendererApp.main",
```

