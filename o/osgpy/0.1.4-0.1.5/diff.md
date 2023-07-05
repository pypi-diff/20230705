# Comparing `tmp/osgpy-0.1.4-py3-none-any.whl.zip` & `tmp/osgpy-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10390 bytes, number of entries: 9
+Zip file size: 9764 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       40 b- defN 23-Mar-06 06:50 osg/__init__.py
--rw-r--r--  2.0 unx    13253 b- defN 23-Jul-04 07:40 osg/flamegraph.py
+-rw-r--r--  2.0 unx    11065 b- defN 23-Jul-05 13:50 osg/flamegraph.py
 -rw-r--r--  2.0 unx     9586 b- defN 23-Jul-03 10:22 osg/pandas.py
 -rw-r--r--  2.0 unx      803 b- defN 23-Mar-06 06:50 osg/plot.py
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-04 07:52 osgpy-0.1.4.data/data/requirements.txt
--rw-r--r--  2.0 unx     1358 b- defN 23-Jul-04 08:00 osgpy-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 08:00 osgpy-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-04 08:00 osgpy-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-04 08:00 osgpy-0.1.4.dist-info/RECORD
-9 files, 25957 bytes uncompressed, 9256 bytes compressed:  64.3%
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-04 07:52 osgpy-0.1.5.data/data/requirements.txt
+-rw-r--r--  2.0 unx     1358 b- defN 23-Jul-05 14:06 osgpy-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 14:06 osgpy-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-05 14:06 osgpy-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      665 b- defN 23-Jul-05 14:06 osgpy-0.1.5.dist-info/RECORD
+9 files, 23769 bytes uncompressed, 8630 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: osg/pandas.py
 Comment: 
 
 Filename: osg/plot.py
 Comment: 
 
-Filename: osgpy-0.1.4.data/data/requirements.txt
+Filename: osgpy-0.1.5.data/data/requirements.txt
 Comment: 
 
-Filename: osgpy-0.1.4.dist-info/METADATA
+Filename: osgpy-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: osgpy-0.1.4.dist-info/WHEEL
+Filename: osgpy-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: osgpy-0.1.4.dist-info/top_level.txt
+Filename: osgpy-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: osgpy-0.1.4.dist-info/RECORD
+Filename: osgpy-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osg/flamegraph.py

```diff
@@ -1,10 +1,10 @@
 import sys
 import pandas as pd
-from plotnine import geom_rect, geom_text
+from plotnine import geom_rect, geom_text, aes
 import plotnine as p9
 from fnmatch import fnmatch
 from plydata import *
 from matplotlib.font_manager import FontProperties, findfont, get_font
 from matplotlib.backends.backend_agg import get_hinting_flag
 from collections import OrderedDict
 from pathlib import Path
@@ -167,33 +167,36 @@
         total_count = self.count
         data = []
         def recr(name, node, height, x_min, x_max):
             data.append(dict(
                 name=name,
                 name_hash=name_hash(name),
                 count=node.count,
-                percent=node.count/total_count * 100,
+                rect_width=node.count/total_count,
+                rect_start=x_min,
                 level=height,
-                xmin=x_min,
-                xmax=x_max,
-                ymin=height,
-                ymax=height+1,
                 **node.attrs
             ))
             x = x_max
             for name, child in reversed(node.children.items()):
                 percent = child.count / total_count
                 child_x_max = x
                 child_x_min = x - percent
                 x = child_x_min
                 recr(name, child, height+1, child_x_min, child_x_max)
         recr("<root>", self, -1, 0.0, 1.0)
 
         return pd.DataFrame(data=data)
 
+    @staticmethod
+    def aes(**kwargs):
+        return aes(**kwargs).inherit(dict(xmin='rect_start', xmax='rect_start+rect_width', ymin='level',ymax='level+1', label='name'))
+    
+        
+
 def name_hash(name):
     """The namehash algorithm from flamegraph.pl"""
     vector = 0
     weight = 1
     max = 1
     mod = 10
     for c in name:
@@ -207,16 +210,18 @@
 
         return (1 - vector / max)
 
 
 _params = geom_text.DEFAULT_PARAMS.copy()
 _params.update(
     dict(
-        font_scale=1.0,
+        font_scale=0.8,
         font_max_size=11,
+        padding_left=0.005,
+        padding_right=0.005,
     )
 )
 
 
 class geom_text_truncate(geom_text):
     """An derived geom that scales and clips a text to fit a certain geom_rect."""
     REQUIRED_AES = {"label", "xmin", "xmax", "ymin", "ymax"}
@@ -224,129 +229,79 @@
 
     def draw_panel(self, data, panel_params, coord, ax, **params):
         bb = ax.get_window_extent()
 
         A, B = panel_params.x.limits
         total_width = B - A
         df = data.copy()
-        df['x'] = data['xmin'] + 0.005 * total_width
+        padding_left = params.get("padding_left")
+        padding_right = params.get("padding_right")
+        df['x'] = data['xmin'] + padding_left  * total_width
         df['y'] = (data['ymax']  + data['ymin'])/ 2
         df['ha'] = 'left'
         df['va'] = 'center'
 
         A, B = panel_params.y.limits
         total_height = (B  - A)
         rect_height = (data.ymax - data.ymin)
         df['size'] = (bb.height * (rect_height / total_height) / 1.33 / data.lineheight) * params.get("font_scale")
         df['size'] = df['size'].clip(upper=params.get("font_max_size"))
 
-        subpixels = 64
-        df['label_width'] = ((df.xmax - df.xmin)/total_width - 0.005) * bb.width * subpixels
+        df['label_percent'] = ((df.xmax - df.xmin)/total_width) - padding_left - padding_right
+        df['label_percent'] = df.label_percent.clip(lower=0)
+        df['label_width']   = df.label_percent * bb.width
 
         dpi = p9.options.get_option('dpi')
         family = p9.options.get_option('base_family')
         props = FontProperties(family=family)
         font = get_font(findfont(props))
+        df['label_trunc'] = None
         for idx, row in df.iterrows():
-            # FIXME: the 1.1 is a magic constant here.
             font.set_size(row['size'], dpi)
             def test(s):
                 font.set_text(s, 0, flags=get_hinting_flag())
                 text_width, _ = font.get_width_height()
-                # print(row.label_width, text_width, s)
-                if row.label_width >= text_width + 64 * 10:
+                # print(row.label_width, row.label_percent, text_width, s)
+                if row.label_width >= text_width/64:
                     df.at[idx, 'label_trunc'] = s
                     return True
             if not test(row['label']):
                 i = len(row['label'])
-                while i > 3 and not test(row['label'][:i] + '..'):
+                while i >= 3 and not test(row['label'][:i] + '..'):
                     i -= 1
         df['label'] = df['label_trunc']
         df = df[~df.label.isna()]
 
         geom_text.draw_group(df, panel_params, coord, ax, **params)
 
 
 if __name__ == "__main__":
-    fn = "/home/stettberger/w/eurosys-exmap/data/flamegraphs/exmap_read_raid-random-local-128.perf.counts"
-    def prepare(tree):
-        tree = tree.prune(cutoff_percent=0.3, cutoff_height=5)
-        tree = tree.attr_set(label=[('asm_exc_page_fault', 'pagefault'),
-                                    ('error_entry', 'pagefault'),
-                                    ('entry_SYSCALL_64', 'munmap'),
-                                    ('datasource', 'datasource'),
-                                    ('sender', 'sender'),
-                                    ('checksum', 'checksum'),
-                                    ],
-                             initial=dict(label=None)
-                             )
-
-        def sort_frames(name, node):
-            if 'asm_exc_page_fault' in node.children and 'error_entry' in node.children:
-                for N in ('entry_SYSCALL_64', 'error_entry', 'asm_exc_page_fault'):
-                    tmp = node.children[N]
-                    del node.children[N]
-                    node.children[N] = tmp
-
-        tree = tree.transform(sort_frames)
-
-        T = sample_tree()
-        T.count = 0
-        T.attrs = tree.attrs
-        T.children = OrderedDict()
-        for process in ('checksum', 'sender', 'datasource'):
-            S = tree.children[process]
-            T.count += S.count
-            T.children[process] = S
-
-        return tree, T.to_table()
-
-
-    treeA = sample_tree.from_counts('data/FlamePipeline-632cdbe17dea38a865c6eba6deeffc65/out.perf-folded')
-    treeA, tableA = prepare(treeA)
-    tableA['benchmark'] = 'memfd'
-
-    treeB = sample_tree.from_counts('data/FlamePipeline-318d655de08519299bd8de70206195c6/out.perf-folded')
-    treeB, tableB = prepare(treeB)
-    tableB['benchmark'] = 'Morsel'
-
-    # Normalize xmin and xmaxprint(treeA.count/treeB.count)
-    tableB['xmin'] *= (treeB.count/treeA.count)
-    tableB['xmax'] *= (treeB.count/treeA.count)
-
-    table = pd.concat([tableA,tableB])
-    
-
-    table['label'] = table['label'].astype('category').cat.set_categories(['pagefault', 'munmap', 'checksum', 'sender', 'datasource'], ordered=True)
-
-
+    import sys
     from plotnine import *
+    from pathlib import Path
 
-    # (ggplot(treeA.to_table(), aes(xmin='xmin', xmax='xmax', ymin='ymin',ymax='ymax',
-    #                               fill='label', label='name'))
-    #  + geom_rect()
-    #  + geom_text_truncate(show_legend=False)).save("test.pdf")
-
-    g = (
-        ggplot(table.query('level>=0'), aes(xmin='xmin*100', xmax='xmax*100', ymin='ymin',ymax='ymax',
-                                            fill='label', label='name'))
-        + facet_wrap('~benchmark', ncol=1)
-        + geom_rect()
-        + geom_text_truncate(aes(label='name'), show_legend=False)
-        + labs(x="Run-Time (Normalized to memfd) [%]", y="Call Stack", fill='Component')
-        + scale_x_continuous()
+    fn = Path(__file__).parent.parent / 'data'/ 'perf-example.counts'
+    tree = sample_tree.from_counts(fn)
+    print("Tree Nodes before pruning:", tree.size())
+    tree = tree.prune(cutoff_percent=0.1, cutoff_height=8)
+    print("Tree Nodes after pruning:", tree.size())
+    tree = tree.attr_set(
+        component=[
+            ('*geos*', 'GEOS'),
+            ('*GEOS*', 'GEOS')
+        ],
+        initial=dict(component='other')
+    )
+    table = tree.to_table()
+    
+    flamegraph = (
+        ggplot(table, tree.aes(fill='component'))
+        + geom_rect(color='white',size=0.1)
+        + geom_text_truncate(show_legend=False)
+        + scale_fill_brewer('qual', palette=2)
         + scale_y_continuous(breaks=[])
-        + scale_fill_manual(values=['tab:red', 'tab:blue', 'lightsalmon', 'palegreen', 'lightsteelblue'],
-                            breaks=['pagefault', 'munmap', 'datasource', 'sender', 'checksum'],
-                            labels=['Pagefault', 'Munmap', 'P: source', 'P:sender', 'P:checksum'])
-        # + scale_fill_identity()
-        # + scale_size_identity()
-        # + scale_fill_continuous('RdYlBu')
-        + coord_cartesian(xlim=(0, 100), expand=False)
-        # + theme_tufte()
         + theme(
-            figure_size=(10,3),
+            figure_size=(6,3),
         )
     )
-    g.save("test.pdf")
-
 
+    flamegraph.save('test.pdf')
```

## Comparing `osgpy-0.1.4.dist-info/METADATA` & `osgpy-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osgpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python utilities of the Operating System Group
 Home-page: http://github.com/tuhhosg/osgpy
 Author: Christian Dietrich
 Author-email: christian.dietrich@tuhh.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

