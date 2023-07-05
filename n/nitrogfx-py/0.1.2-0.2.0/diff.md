# Comparing `tmp/nitrogfx-py-0.1.2.tar.gz` & `tmp/nitrogfx-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrogfx-py-0.1.2.tar", last modified: Sun Jun 25 17:09:35 2023, max compression
+gzip compressed data, was "nitrogfx-py-0.2.0.tar", last modified: Wed Jul  5 20:02:15 2023, max compression
```

## Comparing `nitrogfx-py-0.1.2.tar` & `nitrogfx-py-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.426729 nitrogfx-py-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)    35150 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    41806 2023-06-25 17:09:35.426729 nitrogfx-py-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 17:09:35.426729 nitrogfx-py-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.422729 nitrogfx-py-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.424729 nitrogfx-py-0.1.2/src/nitrogfx/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8702 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/ncer.py
--rw-rw-rw-   0 root         (0) root         (0)     6144 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/ncgr.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/nclr.py
--rw-rw-rw-   0 root         (0) root         (0)     3605 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/nscr.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-06-25 17:09:18.000000 nitrogfx-py-0.1.2/src/nitrogfx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 17:09:35.425729 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)    41806 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-25 17:09:35.000000 nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:02:15.805375 nitrogfx-py-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35150 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    41842 2023-07-05 20:02:15.805375 nitrogfx-py-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 20:02:15.805375 nitrogfx-py-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:02:15.801375 nitrogfx-py-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:02:15.803375 nitrogfx-py-0.2.0/src/nitrogfx/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10341 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     7419 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/nanr.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/ncer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6144 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/ncgr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/nclr.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/nscr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2713 2023-07-05 20:01:57.000000 nitrogfx-py-0.2.0/src/nitrogfx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:02:15.804375 nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    41842 2023-07-05 20:02:15.000000 nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-05 20:02:15.000000 nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 20:02:15.000000 nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-05 20:02:15.000000 nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 20:02:15.000000 nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/top_level.txt
```

### Comparing `nitrogfx-py-0.1.2/LICENSE.txt` & `nitrogfx-py-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.2/PKG-INFO` & `nitrogfx-py-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrogfx-py
-Version: 0.1.2
+Version: 0.2.0
 Summary: Nintendo DS Graphic format library
 Author-email: Fexean <3699814-Fexean@users.noreply.gitlab.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,16 +675,16 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
         
-Project-URL: Homepage, https://gitlab/Fexean/ntrgfx-py
-Keywords: NDS,Nintendo DS,NCGR,NCLR,NSCR
+Project-URL: Homepage, https://gitlab.com/Fexean/ntrgfx-py
+Keywords: NDS,Nintendo DS,NCGR,NCLR,NSCR,NCER,NANR
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -694,14 +694,15 @@
 
 Currently it supports:
 
 - NCGR/NCBR tilesets
 - NSCR tilemaps
 - NCLR palettes
 - NCER sprite data
+- NANR animation data
 
 The formats aren't perfectly implemented so this most likely won't work with every file from every game out there.
 
 ## Install from pip
 
     pip install nitrogfx-py
```

### Comparing `nitrogfx-py-0.1.2/README.md` & `nitrogfx-py-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Currently it supports:
 
 - NCGR/NCBR tilesets
 - NSCR tilemaps
 - NCLR palettes
 - NCER sprite data
+- NANR animation data
 
 The formats aren't perfectly implemented so this most likely won't work with every file from every game out there.
 
 ## Install from pip
 
     pip install nitrogfx-py
```

### Comparing `nitrogfx-py-0.1.2/pyproject.toml` & `nitrogfx-py-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "nitrogfx-py"
-version = "0.1.2"
-keywords = ["NDS", "Nintendo DS", "NCGR", "NCLR", "NSCR"]
+version = "0.2.0"
+keywords = ["NDS", "Nintendo DS", "NCGR", "NCLR", "NSCR", "NCER", "NANR"]
 authors = [
   { name="Fexean", email="3699814-Fexean@users.noreply.gitlab.com" },
 ]
 description = "Nintendo DS Graphic format library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
@@ -17,9 +17,9 @@
 dependencies = [
 	"Pillow==7.0.0"
 ]
 
 
 
 [project.urls]
-"Homepage" = "https://gitlab/Fexean/ntrgfx-py"
+"Homepage" = "https://gitlab.com/Fexean/ntrgfx-py"
```

### Comparing `nitrogfx-py-0.1.2/src/nitrogfx/convert.py` & `nitrogfx-py-0.2.0/src/nitrogfx/convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from nitrogfx.ncgr import NCGR, flip_tile
 from nitrogfx.nscr import NSCR, MapEntry
 from nitrogfx.nclr import NCLR
 from nitrogfx.ncer import NCER, Cell, OAM
 from nitrogfx.util import draw_tile
+from nitrogfx.nanr import NANR, Sequence, SeqMode, SeqType
 from PIL import Image
 import json
 
 def get_img_palette(img):
         """Creates NCLR palette from the color table of an indexed Image
         :param img: Indexed Pillow Image
         :return: NCLR object
@@ -41,15 +42,15 @@
         nclr.bpp = bpp
         
         ncgr = NCGR()
         ncgr.tiles.append([0 for i in range(64)])
         ncgr.bpp = bpp
 
         tiles = ncgr.tiles
-        nscr = NSCR(img.width, img.height)
+        nscr = NSCR(img.width, img.height, bpp==8)
 
         for y in range(0, img.height, 8):
                 for x in range(0, img.width, 8):
                         tile = get_tile_data(img, x, y)
                         map_entry = ncgr.find_tile(tile, use_flipping)
                         if map_entry == None:
                                 map_entry = MapEntry(len(tiles))
@@ -259,7 +260,58 @@
     data["labels"] = [label for label in ncer.labels]
     data["labelCount"] = len(ncer.labels)
 
     with open(json_filename, "w") as f:
         json.dump(data, f, indent=4)
 
 
+
+def nanr_to_json(nanr, json_filename):
+    """Stores a NANR object in a file as JSON
+    :param nanr: NANR object
+    :param json_filename: path to produced JSON file
+    """
+    def seq_to_json(seq):
+        return {    "first_frame": seq.first_frame,
+                    "type" : str(seq.type)[8:],
+                    "mode" : str(seq.mode)[8:],
+                    "frames": [vars(frame) for frame in seq.frames]
+                }
+    obj = {
+        "anims": [seq_to_json(seq) for seq in nanr.anims],
+        "texu": nanr.texu,
+        "labels": nanr.labels
+    }
+    
+    with open(json_filename, "w") as f:
+        json.dump(obj, f, indent=4)
+
+
+def json_to_nanr(json_filename):
+    """Reads NANR data from a JSON file
+    :param json_filename: path to a file generated with nanr_to_json
+    :return: NANR object
+    """
+    def json_to_seq(json):
+        seq = Sequence()
+        if "sx" in json["frames"][0].keys():
+            seq.frame_type = 1
+        elif "px" in json["frames"][0].keys():
+            seq.frame_type = 2
+        else:
+            seq.frame_type = 0
+        seq.mode = SeqMode[json["mode"]]
+        seq.type = SeqType[json["type"]]
+        for frame in json["frames"]:
+            f = seq.add_frame()
+            for key in frame.keys():
+                f.__dict__.update({key : frame[key]})
+        return seq
+
+    with open(json_filename) as f:
+        data = json.loads(f.read())
+    nanr = NANR()
+    nanr.texu = data["texu"]
+    nanr.labels = data["labels"]
+    nanr.anims = [json_to_seq(anim) for anim in data["anims"]]
+    return nanr
+
```

### Comparing `nitrogfx-py-0.1.2/src/nitrogfx/ncer.py` & `nitrogfx-py-0.2.0/src/nitrogfx/ncer.py`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.2/src/nitrogfx/ncgr.py` & `nitrogfx-py-0.2.0/src/nitrogfx/ncgr.py`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.2/src/nitrogfx/nclr.py` & `nitrogfx-py-0.2.0/src/nitrogfx/nclr.py`

 * *Files identical despite different names*

### Comparing `nitrogfx-py-0.1.2/src/nitrogfx/nscr.py` & `nitrogfx-py-0.2.0/src/nitrogfx/nscr.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,29 +17,32 @@
                 x |= (self.yflip & 1) << 11
                 x |= (self.pal & 0xf) << 12
                 return struct.pack("<H", x)
 
         def unpack(data : bytes):
                 ":return: MapEntry"
                 raw = data 
-                return MapEntry(raw & 0x3ff, raw >> 12, raw >> 10, raw >> 11)
+                return MapEntry(raw & 0x3ff, (raw >> 12) & 0xf, (raw >> 10) & 1, (raw >> 11) & 1)
         
         def __eq__(self, other):
                 if not isinstance(other, MapEntry):
                     return False
                 return self.pack() == other.pack()
 
+        def __repr__(self):
+            return f"<MapEntry tile={self.tile} pal={self.pal} xflip={self.xflip} yflip={self.yflip}>"
+
 class NSCR():
         "Class for representing an NSCR tilemap file"
 
-        def __init__(self, w, h):
+        def __init__(self, w, h, _8bpp=True):
                 # in pixels
                 self.width = w
                 self.height = h
-
+                self.is8bpp = _8bpp
                 self.map = [MapEntry() for i in range(w*h//64)]
 
         def set_entry(self, x, y, entry : MapEntry):
             """Set tilemap entry at position. Note that x & y are tile coordinates, not pixel coordinates.
             :param x: x coordinate in tile grid
             :param y: y coordinate in tile grid
             :param entry: MapEntry object
@@ -57,27 +60,27 @@
         def pack(self):
                 """Pack NSCR to bytes.
                 :return: bytes
                 """
                 map_size = self.width * self.height * 2 // 64
                 size = map_size + 0x14
                 header = util.pack_nitro_header("RCSN", size, 1)
-                data = "NRCS".encode("ascii") + struct.pack("<IHHII", size, self.width, self.height, 1, map_size)
+                data = "NRCS".encode("ascii") + struct.pack("<IHHII", size, self.width, self.height, 1 if self.is8bpp else 0, map_size)
                 for m in self.map:
                         data += m.pack()
                 return header + data
 
         def unpack(data : bytes):
                 """Unpack NSCR from bytes.
                 :param data: bytes
                 :return: NSCR object
                 """
-                size, w, h, x, map_size = struct.unpack("<IHHII", data[0x14:0x24])
+                size, w, h, bpp, map_size = struct.unpack("<IHHII", data[0x14:0x24])
                 
-                nscr = NSCR(w, h)
+                nscr = NSCR(w, h, bpp==1)
                 map_ = []
                 for i in range(0, map_size, 2):
                         raw = data[0x24+i] | (data[0x25+i] << 8)
                         map_.append(MapEntry.unpack(raw))
                 nscr.map = map_
                 return nscr
```

### Comparing `nitrogfx-py-0.1.2/src/nitrogfx_py.egg-info/PKG-INFO` & `nitrogfx-py-0.2.0/src/nitrogfx_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrogfx-py
-Version: 0.1.2
+Version: 0.2.0
 Summary: Nintendo DS Graphic format library
 Author-email: Fexean <3699814-Fexean@users.noreply.gitlab.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,16 +675,16 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
         
-Project-URL: Homepage, https://gitlab/Fexean/ntrgfx-py
-Keywords: NDS,Nintendo DS,NCGR,NCLR,NSCR
+Project-URL: Homepage, https://gitlab.com/Fexean/ntrgfx-py
+Keywords: NDS,Nintendo DS,NCGR,NCLR,NSCR,NCER,NANR
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -694,14 +694,15 @@
 
 Currently it supports:
 
 - NCGR/NCBR tilesets
 - NSCR tilemaps
 - NCLR palettes
 - NCER sprite data
+- NANR animation data
 
 The formats aren't perfectly implemented so this most likely won't work with every file from every game out there.
 
 ## Install from pip
 
     pip install nitrogfx-py
```

