# Comparing `tmp/xplorts-0.6.tar.gz` & `tmp/xplorts-0.7.tar.gz`

## Comparing `xplorts-0.6.tar` & `xplorts-0.7.tar`

### file list

```diff
@@ -1,68 +1,76 @@
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 xplorts-0.6/_NOTES.ipynb
--rw-r--r--   0        0        0  1246655 2020-02-02 00:00:00.000000 xplorts-0.6/tt.html
--rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph annual bespoke.csv
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph annual by division.csv
--rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph annual by section.csv
--rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.6/data/oph quarterly by section.csv
--rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.6/data/outputperhourworked.xls
--rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.6/docs/html/xplor_lprod oph annual by section.html
--rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.6/docs/html/xplor_lprod oph quarterly by section.html
--rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/slideselect_date.png
--rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/slideselect_industry.png
--rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_lines_thumbnail_large.png
--rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
--rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_thumbnail.png
--rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.6/docs/png/xplor_lprod_tscomp_thumbnail_large.png
--rw-r--r--   0        0        0   947883 2020-02-02 00:00:00.000000 xplorts-0.6/src/tt.html
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 xplorts-0.6/src/tt.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/__init__.py
--rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/base.ipynb
--rw-r--r--   0        0        0    16803 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/base.py
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dutils.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/ghostbokeh.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/slideselect.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/__main__.py
--rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/dblprod.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/prodgrowsnap.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/prodgrowts.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/prodlines.py
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/dblprod/xpdblprod.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/heatmap/__init__.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/heatmap/heatmap.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/__main__.py
--rw-r--r--   0        0        0    13921 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/lines.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/lines/xplines.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/__main__.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/scatter.py
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/scatter/xpscatter.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/__main__.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/snapcomp.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/snapcomp/xpsnapcomp.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/__main__.py
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/bokeh_stacks.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/stacks.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/stacks_util.py
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/stacks/xpstacks.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/__main__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/tscomp.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/tscomp/xptscomp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/utils/__init__.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.6/src/xplorts/utils/ukons_lprod_to_csv.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.6/tests/conftest.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_dblprod.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_lines.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_scatter.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_snapcomp.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_stacks.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.6/tests/test_tscomp.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.6/.gitignore
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.6/LICENSE
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xplorts-0.6/README.md
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 xplorts-0.6/pyproject.toml
--rw-r--r--   0        0        0    15776 2020-02-02 00:00:00.000000 xplorts-0.6/PKG-INFO
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 xplorts-0.7/_NOTES.ipynb
+-rw-r--r--   0        0        0  1246655 2020-02-02 00:00:00.000000 xplorts-0.7/tt.html
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 xplorts-0.7/data/.~lock.totalpspreferencetables2020.xlsx#
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph annual bespoke.csv
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph annual by division.csv
+-rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph annual by section.csv
+-rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.7/data/oph quarterly by section.csv
+-rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.7/data/outputperhourworked.xls
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 xplorts-0.7/data/psp non-quality adjusted.csv
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 xplorts-0.7/data/psp quality adjusted.csv
+-rw-r--r--   0        0        0    79893 2020-02-02 00:00:00.000000 xplorts-0.7/data/totalpspreferencetables2020.xlsx
+-rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.7/docs/html/xplor_lprod oph annual by section.html
+-rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.7/docs/html/xplor_lprod oph quarterly by section.html
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/slideselect_date.png
+-rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/slideselect_industry.png
+-rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_lines_thumbnail_large.png
+-rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
+-rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_thumbnail.png
+-rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.7/docs/png/xplor_lprod_tscomp_thumbnail_large.png
+-rw-r--r--   0        0        0   947883 2020-02-02 00:00:00.000000 xplorts-0.7/src/tt.html
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 xplorts-0.7/src/tt.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/__init__.py
+-rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/base.ipynb
+-rw-r--r--   0        0        0    16670 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/base.py
+-rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dutils.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/ghostbokeh.py
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/slideselect.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/__main__.py
+-rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/dblprod.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/prodgrowsnap.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/prodgrowts.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/prodlines.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/dblprod/xpdblprod.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/__main__.py
+-rw-r--r--   0        0        0    11819 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/heatmap.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/heatmap/xpheatmap.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/__main__.py
+-rw-r--r--   0        0        0    13921 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/lines.py
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/lines/xplines.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/__main__.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/scatter.py
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/scatter/xpscatter.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/__main__.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/snapcomp.py
+-rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/snapcomp/xpsnapcomp.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/__main__.py
+-rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/bokeh_stacks.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/stacks.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/stacks_util.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/stacks/xpstacks.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/__main__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/tscomp.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/tscomp/xptscomp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/utils/__init__.py
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/utils/ukons_lprod_to_csv.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 xplorts-0.7/src/xplorts/utils/ukons_psp_to_csv.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.7/tests/conftest.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_dblprod.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_heatmap.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_lines.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_scatter.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_snapcomp.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_stacks.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.7/tests/test_tscomp.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.7/.gitignore
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.7/LICENSE
+-rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 xplorts-0.7/README.md
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 xplorts-0.7/pyproject.toml
+-rw-r--r--   0        0        0    16364 2020-02-02 00:00:00.000000 xplorts-0.7/PKG-INFO
```

### Comparing `xplorts-0.6/_NOTES.ipynb` & `xplorts-0.7/_NOTES.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999477424749164%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(21, '> python -m pip install openpyxl\\n')]}}}"}*

```diff
@@ -159,14 +159,15 @@
                 "\n",
                 "\n",
                 "```\n",
                 "> conda create -n p38_xp python=3.8  # Try newer Python.\n",
                 "> conda activate p38_xp\n",
                 "> python -m pip install --upgrade pip\n",
                 "> python -m pip install xplorts\n",
+                "> python -m pip install openpyxl\n",
                 "```\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
```

### Comparing `xplorts-0.6/tt.html` & `xplorts-0.7/tt.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/data/oph annual bespoke.csv` & `xplorts-0.7/data/oph annual bespoke.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/data/oph annual by division.csv` & `xplorts-0.7/data/oph annual by division.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/data/oph annual by section.csv` & `xplorts-0.7/data/oph annual by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/data/oph quarterly by section.csv` & `xplorts-0.7/data/oph quarterly by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/data/outputperhourworked.xls` & `xplorts-0.7/data/outputperhourworked.xls`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/html/xplor_lprod oph annual by section.html` & `xplorts-0.7/docs/html/xplor_lprod oph annual by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/html/xplor_lprod oph quarterly by section.html` & `xplorts-0.7/docs/html/xplor_lprod oph quarterly by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/png/slideselect_date.png` & `xplorts-0.7/docs/png/slideselect_date.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/png/slideselect_industry.png` & `xplorts-0.7/docs/png/slideselect_industry.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/png/xplor_lprod_lines_thumbnail_large.png` & `xplorts-0.7/docs/png/xplor_lprod_lines_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/png/xplor_lprod_snapcomp_thumbnail_large.png` & `xplorts-0.7/docs/png/xplor_lprod_snapcomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/png/xplor_lprod_thumbnail.png` & `xplorts-0.7/docs/png/xplor_lprod_thumbnail.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/docs/png/xplor_lprod_tscomp_thumbnail_large.png` & `xplorts-0.7/docs/png/xplor_lprod_tscomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/tt.html` & `xplorts-0.7/src/tt.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/tt.py` & `xplorts-0.7/src/tt.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/__init__.py` & `xplorts-0.7/src/xplorts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """
 The xplorts ("explore ts") package contains tools to make
 standalone interactive HTML charts to explore time series datasets.
 
-Once created, the HTML documents can be used with any web browser. 
+Once created, the HTML documents can be used with any web browser.
 They do not need an active internet connection.
 
 Generally the tools work with annual, quarterly, or monthly time series
 with a categorical "split factor".  An example would be annual jobs counts
 by industry.
 
 The interactive charts provide widgets to select different subsets of
 data for display.  A hover tool displays detail for the data under the
 cursor.  Chart tools support zoom and plot save.
 
-xplorts uses the [Bokeh](https://bokeh.org) interactive visualization 
+xplorts uses the [Bokeh](https://bokeh.org) interactive visualization
 library.
 
 Command line interface entrypoints
 ----------------------------------
 dblprod
     Create a labour productivity dashboard, with three charts including:
-        - a lines chart showing levels of labour productivity, gross value 
+        - a lines chart showing levels of labour productivity, gross value
             added, and labour,
         - a time series growth components chart showing cumulative growth
             in labour productivity, gross value added, and labour, and
         - a snapshot growth components chart showing period-on-period
             growth in labour productivity, gross value added, and labour.
 
 lines
     Create a line chart showing several time series with a split
     factor.  Widgets select one split factor category at a time.
-    
+
+heatmap
+    Create a heatmap showing a dependent variable as a function of
+    two categorical variables (typically a date variable and a split
+    factor).
+
 scatter
     Create scatter chart showing one or more time series with a split
     factor.  Widgets select one split factor category at a time.
 
 snapcomp
     Create a snapshot growth components chart, with a categorical
-    vertical axis showing levels of a split factor, horizontal stacked 
+    vertical axis showing levels of a split factor, horizontal stacked
     bars showing growth components, and markers showing overall growth
     for each stack of bars.  A widget selects one time period at a time.
 
 stacks
     Create stacked bar chart showing several data series with a split
     factor.  Widgets select one split factor at a time (or one time
     period at a time if the split factor is plotted as a chart axis).
@@ -60,61 +65,66 @@
 ---------------------------------
 base
     Miscellaneous helper functions and classes.
 
 ghostbokeh
     Define an abstract base class to a build pseudo-subclass of a Bokeh class.
 
+heatmap
+    Functions to create a heatmap showing data values as a function of
+    horizontal and vertical categorical variables.
+
 lines
     Modify a Bokeh Figure by adding line charts to show several time
     series with a split factor.
 
 scatter
     Modify a Bokeh Figure by adding scatter charts to show one or more
     categorical series with a split factor.
 
 slideselect
-    Defines a class combining select and slider widgets, with support for 
+    Defines a class combining select and slider widgets, with support for
     javascript linking to other objects.
 
 snapcomp
-    Modify a Bokeh Figure by adding a snapshot growth components chart, with a 
-    categorical vertical axis showing levels of a split factor, horizontal 
+    Modify a Bokeh Figure by adding a snapshot growth components chart, with a
+    categorical vertical axis showing levels of a split factor, horizontal
     stacked bars showing growth components, and markers showing overall growth
-    for each stack of bars.  
+    for each stack of bars.
 
 stacks
-    Modify a Bokeh Figure by adding a horizontal or vertical stacked bar 
+    Modify a Bokeh Figure by adding a horizontal or vertical stacked bar
     chart showing several data series with a split factor.
 
 tscomp
-    Modify a Bokeh Figure by adding a time series growth components chart, with 
-    a categorical vertical axis showing levels of a split factor, horizontal 
-    stacked bars showing growth components, and a line showing overall growth.  
+    Modify a Bokeh Figure by adding a time series growth components chart, with
+    a categorical vertical axis showing levels of a split factor, horizontal
+    stacked bars showing growth components, and a line showing overall growth.
 
 
 Subpackages (not exported)
 --------------------------
 dblprod
     Make standalone interactive labour productvity dashboard charts
 
 utils
     Utilities for extracting data from particular datasets to use with
     xplorts charts.
 """
 
-from . import (base, dutils, ghostbokeh, 
+from . import (base, dutils, ghostbokeh, heatmap,
                slideselect)
 # Export API modules within sub-packages.
 from .lines import lines
 from .scatter import scatter
 from .snapcomp import snapcomp
 from .stacks import stacks
 from .tscomp import tscomp
 
-# Suppress code analysis warnings of unused imports; 
+# Suppress code analysis warnings of unused imports;
 #   see https://stackoverflow.com/a/31079085/16327476.
-__all__ = ["base", "dutils", "ghostbokeh", 
+__all__ = ["base", "dutils", "ghostbokeh",
+           "heatmap",
            "lines", "scatter",
-           "slideselect", 
+           "slideselect",
            "snapcomp", "stacks",
            "tscomp"]
```

### Comparing `xplorts-0.6/src/xplorts/base.ipynb` & `xplorts-0.7/src/xplorts/base.ipynb`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/base.py` & `xplorts-0.7/src/xplorts/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Map variable names to colors
 """
 
 #%%
 
 from bokeh import palettes
 from bokeh.io import output_file
-from bokeh.models import (CDSView, ColumnDataSource, CustomJS, GroupFilter, FactorRange, 
+from bokeh.models import (CDSView, ColumnDataSource, CustomJS, GroupFilter, FactorRange,
                           HoverTool, Legend, LegendItem)
 from bokeh.models import formatters as bk_formatters
 #from bokeh.models.formatters import FuncTickFormatter
 from bokeh.plotting import figure
 from bokeh.util.warnings import BokehDeprecationWarning
 
 import functools
@@ -58,30 +58,45 @@
 
 # Imports from this package.
 from xplorts.dutils import dict_fill
 from xplorts.slideselect import SlideSelect
 
 #%%
 
-# Use CustomJSTickFormatter for newer bokeh, or 
-# FuncTickFormatter for older bokeh.    
+# Use CustomJSTickFormatter for newer bokeh, or
+# FuncTickFormatter for older bokeh.
 def _custom_tick_formatter(code):
     try:
         cls = bk_formatters.CustomJSTickFormatter
     except AttributeError:
         cls = bk_formatters.FuncTickFormatter
     return cls(code=code)
 
 
+
+# Tick formatter to suppress most lowest level categorical tick labels.
+# If tick labels are tuples, higher levels will be displayed
+# as normal.
+tf_margins_only = _custom_tick_formatter(
+    code="""
+    if ((index == 0) | (index == ticks.length - 1)) {
+        return tick;
+    } else {
+        return '';
+    }
+    """
+)
+
+
 #%%
 
 def add_hover_tool(fig, renderers, *tooltips, simplify=True, **kwargs):
     """
     Add a hover tool to a Bokeh figure, for given renderers
-    
+
     Parameters
     ----------
     fig : Bokeh Figure
         Figure to add hover tool to.
     renderers : list
         Renderers that should trigger the hover tool.
     tooltips : list or dict
@@ -96,92 +111,92 @@
     kwargs : mapping, optional
         Additional keyword arguments are passed to `Hovertool()`.
     """
 
     if isinstance(tooltips, dict):
         # Convert mapping to list of (label, value) tuples.
         tooltips = tooltips.items()
-    
+
     tooltips = list(tooltips)  # Coerce to list from *args tuple, or .items().
     if len(tooltips) == 1 and simplify:
         # Just use the tooltip string without a tabular label.
         _, tooltips = tooltips[0]
-    
+
     hover_tool = HoverTool(
         tooltips=tooltips,
         renderers=renderers,
         **kwargs
     )
 
     fig.add_tools(hover_tool)
     return hover_tool
 
 
 def extend_legend_items(fig, renderers=None, items=None, **kwargs):
     """
     Add legend items to figure
-    
+
     Extends the legend items of a Bokeh figure.
-    
+
     Parameters
     ----------
     fig : Bokeh Figure
         Figure to add legend items to.
     renderers : mapping
         Mapping of labels to renderers, to create `LegendItem`
         objects.  Each value should be a renderer or list of renderers.
         Either `renderers` or `items` must be specified.
-        The `renderers` parameter is ignored if `items` are given.  
+        The `renderers` parameter is ignored if `items` are given.
     items : list of LegendItem
         Will be added to the figure's legend items.
         Either `renderers` or `items` must be specified.
     kwargs : mapping, optional
         Keyword arguments passed to `fig.Legend` if
         `fig` does not already have a legend.
-    
+
     Raises
     ------
     ValueError
         If neither renderers nor items is given.
-        
+
     Example
     -------
     from bokeh.io import show
     from bokeh.models import Legend
     from bokeh.plotting import figure
     fig = figure()
     fig.add_layout(Legend(location="top_left",
                           background_fill_alpha=0.0))
     plot = fig.circle(x=1, y=3)
     extend_legend_items(fig, {"x": plot})
     show(fig)
     """
-    
+
     if renderers is None and items is None:
         raise ValueError("either renderers or items required")
-        
-    if items is None and renderers is not None:        
+
+    if items is None and renderers is not None:
         # Make a legend item for each renderer.
         items = [
             # Include legend item for each factor level.
             LegendItem(
-                label=var, 
-                renderers=renderer if isinstance(renderer, list) else [renderer], 
+                label=var,
+                renderers=renderer if isinstance(renderer, list) else [renderer],
             ) \
             for var, renderer in renderers.items()
         ]
-    
+
     fig.legend.items.extend(items)
     return None
 
 
 def factor_filters(by, source=None, name_template="filter"):
     """
     Return list of GroupFilter objects for specified variables
-    
+
     Arguments
     ---------
     by: str, sequence, or dict
         Categorical variables to filter by, or a mapping
         from variable names to initial values to use in the
         corresponding filters.  The `dict` form must be
         used if `source` is not given.
@@ -190,89 +205,89 @@
         if `by` is not a `dict`.
     name_template: str, optional
         Combined with each `by` variable to assign a name to
         the corresponding filter.  The default is "filter",
         assigning names of the form "filter_X", "filter_Y",
         and so forth, where "X" and "Y" are among the `by`
         variables.
-    
+
     Returns
     -------
     A list of filters that can be used with CDSView tofilter
     a `ColumnDataSource` on values of the `by` variables.
-    
+
     Examples
     --------
     data = pd.DataFrame.from_records(
         [("A", 2001, 10),
          ("A", 2002, 15),
          ("B", 2001, 20),
          ("B", 2002, 18)],
          columns=["industry", "year", "sales"]
     )
     cds = ColumnDataSource(data)
     filters = factor_filters("industry", source=cds)
     view = CDSView(source=cds, filters=filters)
-    
+
     # Explicit initial filter value.
     filters = factor_filters({"industry": "B"})
     """
-    
+
     if isinstance(by, str):
         # Wrap in list, for convenience.
         by = [by]
-    
+
     if not isinstance(by, dict):
         # Map `by` variables to initial values to use in filter.
         is_cds = isinstance(source, ColumnDataSource)
         data = (source.data if is_cds else source)
         # Use first value of each variable named by `by`.
         by = {key: next(iter(data[key])) for key in by}
 
     filters = [
         GroupFilter(
             column_name=var,
             group=initial,
             name="_".join([name_template, var])
         ) \
-        for var, initial in by.items() 
+        for var, initial in by.items()
     ]
     return filters
 
 
 def factor_view(source, by, **kwargs):
     """
     Return a CDSView to filter source on specified variables
-    
+
     Parameters
     ---------
     source : ColumnDataSource
         Data to filter.
     by : str or sequence of str
         Categorical variables to filter by.
     kwargs : mapping, optional
         Keyword arguments passed into `factor_filter()`.
-    
+
     Returns
     -------
     A CSDView that filters `source` on values of the `by` variables.
-    
+
     Examples
     --------
     data = pd.DataFrame.from_records(
         [("A", 2001, 10),
          ("A", 2002, 15),
          ("B", 2001, 20),
          ("B", 2002, 18)],
          columns=["industry", "year", "sales"]
     )
     cds = ColumnDataSource(data)
     view = factor_view(cds, "category")
     """
-    
+
     assert isinstance(source, ColumnDataSource), f"source must be ColumnDataSource, not {type(source)}"
 
     # Get list of one or more filters.
     filters = factor_filters(by, source=source, **kwargs)
     with warnings.catch_warnings():
         # Catch deprecations from bokeh CDSView if necessary.
         warnings.simplefilter("error")
@@ -287,20 +302,20 @@
             if len(filters):
                 if len(filters) == 1:
                     # use the single filter as is.
                     filter = filters[0]
                 else:
                     # Combine multiple filters with logical `and`.
                     filter = functools.reduce(operator.and_, filters)
-                    
+
                 view = CDSView(filter=filter)
             else:
                 # No filters to apply.
                 view = CDSView()
-        
+
     return view
 
 
 def filter_widget(options, title=None, start_value="first"):
     """
     Make a widget to select among values of a sequence
     """
@@ -324,36 +339,36 @@
     iv_axis = "x",
     legend = "default",
     legend_place = "center",
     suppress_factors = False,
     **kwargs
 ):
     """
-    Return default figure options, updated with optional keywords
-    
+    Make empty bokeh Figure with one categorical axis and one continuous axis
+
     Parameters
     ----------
     iv_data: array or series
         Independent variable against which data will be plotted.  If the
-        data provided satisfy pandas `is_datetime()`, the relevant axis type 
+        data provided satisfy pandas `is_datetime()`, the relevant axis type
         will be "datetime".  Otherwise the default axis type will be used,
         with categorical values and a factor range determined by the unique
         data values.  For regular time periods like annual, quarterly, or
         monthly economic data, a categorical axis is often easier to work
         with and format than a datetime axis.
     iv_axis: str, default "x"
         Whether the independent variable is to be plotted against the "x"
         (horizontal) or "y" (vertical) axis.
     keywords : mapping, optional
         Override default options.
     Returns
     -------
     Bokeh `Figure`.
     """
-    
+
     # Default figure options.
     fopts = dict(
         background_fill_color = "#fafafa",
         tools = "reset,save,pan,box_zoom,wheel_zoom",
     )
     if iv_data is not None:
         # Specify option to configure independent axis.
@@ -369,117 +384,108 @@
                                      factor_padding = 0.2,
                                      group_padding = 0.2,
                                      subgroup_padding = 0.2)
 
     # Fold in explicit options to override others.
     fopts.update(kwargs)
     fig = figure(**fopts)
-    
+
     if suppress_factors:
         # Suppress most lowest level categorical tick labels.
         # If tick labels are tuples, higher levels will be displayed
         # as normal.
-        tf_margins_only = _custom_tick_formatter(
-            code="""
-            if ((index == 0) | (index == ticks.length - 1)) {
-                return tick;
-            } else {
-                return '';
-            }
-            """
-        )
         axis = fig.xaxis if iv_axis == "x" else fig.yaxis
         axis[0].formatter = tf_margins_only
 
     if legend is not None:
         if legend == "default":
             legend = Legend(
                 location = "top_left",
                 background_fill_alpha = 0.0)  # Transparent.
         fig.add_layout(legend, place=legend_place)
-    
+
     fig.toolbar.logo = None
-    
+
     return fig
 
 
 def link_widgets_to_groupfilters(widgets, source, filter):
     """
     Link values of widgets to corresponding GroupFilter objects
-    
+
     Parameters
     ----------
     widgets : Bokeh widget or list of widgets
         The `value` property of each widget will be linked to the
         `group` property of the corresponding `GroupFilter`.  If there are
         more widgets than filters, the excess widgets are ignored.
     source : ColumnDataSource
         Data source, which will be configured to emit a change signal when
         a filter's `group` property changes, to re-render the relevant figure.
     filter : GroupFilter or sequence of GroupFilter
         The `group` property of each filter will be updated whenever the
         `value` of the corresponding widget changes, and `source` will emit
         a change signal whenever the `group` property of a filter changes.  If
         there are more filters than widgets, excess filters are ignored.
-    
+
     Examples
     --------
     from bokeh.models import ColumnDataSource
     from base import factor_view
     source = ColumnDataSource({"industry": ["A", "B"],
                                "growth": [10, 12]})
     view_by_factor = factor_view(source, "industry")
     widget = SlideSelect(options=["A", "B"],
                          name="industry_filter")  # Show this in a layout.
-    link_widgets_to_groupfilters(widget, 
+    link_widgets_to_groupfilters(widget,
                                  source=source,
                                  filter=view_by_factor.filters)
     """
-    
+
     # Wrap singleton widget or filter, for convenience.
     if not isinstance(widgets, (list, tuple)):
         widgets = [widgets]
     if not isinstance(filter, (list, tuple)):
         filter = [filter]
-        
+
     for widget, filt in zip(widgets, filter):
         # Link widget to the GroupFilter.
         assert isinstance(filt, GroupFilter)
         widget.js_link("value", other=filt, other_attr="group")
 
-        # Signal change in data when filter `group` attribute changes, 
+        # Signal change in data when filter `group` attribute changes,
         # so chart refreshes.
         filt.js_on_change(
             "group",
             CustomJS(args=dict(source=source),
                      code="""
                          source.change.emit()
-                     """))    
+                     """))
 
 
 def set_output_file(outfile, title):
     """
     Set Bokeh output file for standalone application
-    
+
     Filename suffix is coerced to 'html'
-    
+
     Examples
     --------
     set_output_file(args.save or args.datafile, "OPH by industry")
     """
-    
+
     outfile = Path(outfile).with_suffix(".html").as_posix()
     output_file(outfile, title=title, mode='inline')
 
 
 def unpack_data_varnames(args, arg_names, defaults=None):
     """
     Look up command line arguments or defaults
     """
-    
+
     # Assemble CL arguments, which default to None.
     mapping = {arg: getattr(args, arg) for arg in arg_names}
     if (defaults is not None
         and all(arg is None for arg in mapping.values())):
         # Use default names.
         mapping = dict(zip(arg_names, defaults))
         if len(defaults) > len(arg_names):
@@ -487,39 +493,39 @@
             mapping[arg_names[-1]] = defaults[len(arg_names):]
     return mapping
 
 
 def variables_cmap(variables, palette):
     """
     Map variables to colors
-    
+
     If there are more variables than colors in the palette,
     colors are recycled.
-    
+
     Parameters
     ----------
     variables: str or list[str]
         Variable name or list of names.
     palette: str or array
         Named palette from Bokeh.palettes, or array of colors.
-    
+
     Returns
     -------
     dict mapping variable names to colors.
     """
-    
+
     if isinstance(variables, str):
         # Wrap simple string in a list, for convenience.
         variables = [variables]
     n_data_series = len(variables)
-    
+
     if isinstance(palette, str):
         # Access named palette from bokeh.palettes.
         palette = getattr(palettes, palette)
-    
+
     if isinstance(palette, dict):
         # Extract color palette from palette dict, by number of colors needed.
         last_palette = [palette.values()][-1]
         palette = palette.get(n_data_series, last_palette)
 
     # Map variables to palette colors, recycling colors as needed.
     color_map = dict_fill(keys=variables, values=palette)
```

### Comparing `xplorts-0.6/src/xplorts/dutils.py` & `xplorts-0.7/src/xplorts/dutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,99 +47,101 @@
     #   https://docs.python.org/3/library/itertools.html#itertools.pairwise
     # "Copyright © 2001-2023 Python Software Foundation; All Rights Reserved"
     # Used here under the ZERO-CLAUSE BSD LICENSE FOR CODE IN THE PYTHON 3.11.3 DOCUMENTATION
     #   https://docs.python.org/3/license.html#bsd0
     def pairwise(iterable):
         """
         Stand-in for itertools.pairwise()
-        
+
         pairwise('ABCDEFG') --> AB BC CD DE EF FG.
         """
-        
+
         a, b = tee(iterable)
         next(b, None)  # Remove first item of second sequence.
         return zip(a, b)  # Pairs until second sequence is exhausted.
 
 
 #%%
 
 def accumulate_list(items):
     """
     Initial subsequences of increasing length from list of items
-    
+
     Generator of lists.
-    
+
     Examples
     --------
     gen = accumulate_list([1, 2])
     list(gen)
     # [[], [1], [1, 2]]
     """
     for i in range(len(items) + 1):
         yield items[:i]
 
 
 def cumulative_growth(data, columns, date_var="date"):
     """
     Growth of specified dataframe columns relative to earliest date
-    
+
     The row containing the minimum value of `date_var` provides baseline
     values for calculating growth of the columns named by `columns`.
-    
+
     Parameters
     ----------
     data: DataFrame
-        Dataframe including a date column and one or more columns for which 
+        Dataframe including a date column and one or more columns for which
         to calculate growth.
 
     columns: str or list
         Names of columns for which to calculate growth.
-    
+
     date_var: str, default "date"
         Name of column whose minimum value determines the baseline row of data.
-    
+
     Returns
     -------
     DataFrame with same index as `data`, and columns from `columns`.
     """
     # Wrap single column name in a list, for convenience.
     columns = [columns] if isinstance(columns, str) else columns
-    
+
     # Classify each row as having the earliest date or not.
     is_min_date = data[date_var] == data[date_var].min()
-    
+
     # Calculate baseline for each column from row with earliest date.
     baseline = data.loc[is_min_date, columns] \
         .reindex(index=data.index, method="nearest")  # Broadcast baseline to match shape of data.
     return growth_pct_from(data[columns],
                            baseline)
 
 
 def date_tuples(dates, length_threshold = np.inf):
     """
     Coerce monthly, quarterly, or annual dates to tuples
-    
+
     Tuples (if converted to a list) are suitable for `bokeh` categorical axis
-    
+
     Parameters
-    dates : Series of str
+    dates : Sequence of str
         Dates which may be annual ('2021'), quarterly ('2021 Q3'), or
-        monthly ('March 2021' or anything recognised by Pandas 
+        monthly ('March 2021' or anything recognised by Pandas
         `.to_period()`).
     length_threshold : integer, default np.inf
         If the number of unique `dates` exceeds this threshold, only the
         last two digits of years are used.  The default is to always
         use four-digit years.  If 0 is given, only the last two digits
         of years will be used, regardless of how many different `dates`
         there are.
     """
-    
+
+    dates = pd.Series(dates)
+
     sample_date = dates[0]
     n_dates = len(dates.unique())
-    
+
     if re.fullmatch("\d{4}", sample_date):
         # Annual like '2019', use as is.
         if n_dates > length_threshold:
             # Keep only last two digits of year.
             tdate = [year[-2:] for year in dates]
         else:
             tdate = list(dates)
@@ -150,148 +152,148 @@
         # Wrap in a tuple for Bokeh categorical axis.
         tdate = dates.str.split(" ").apply(tuple)
     else:
         # Maybe monthly will work.
         # Create canonical (year, Mmm) category via datetime.
         dt_dates = pd.to_datetime(dates).dt.to_period("M")
         tdate = list(zip(dt_dates.dt.year.astype(str), dt_dates.dt.month.apply('M{:02d}'.format)))
-        
+
     if n_dates > length_threshold:
         # Keep only last two digits of year.
         tdate = [(year[-2:], _) for (year, _) in tdate]
     return tdate
 
 
 def dict_fill(keys, values):
     """
     Map keys to values, recycling values as necessary
     """
-    
+
     return dict(zip(keys, cycle(values)))
 
 
 def growth_pct_from(data, baseline):
     """
     Percentage growth relative to baseline value
-    
+
     Parameters
     ----------
     data: numeric, Series or DataFrame
         Data for which to calculate growth
-        
+
     baseline: numeric, Series or DataFrame
         Value or values to calculate growth relative to.
-    
+
     Returns
     -------
     Same shape as `data`, calculated as `(data / baseline - 1) * 100`, which
     is often written as `100 * (data - baseline)/baseline`.
-    
+
     Examples
     --------
     ## Single value
     growth_pct_from(110, 100)
     # 10
-    
+
     ## Year on year growth
     df = pd.DataFrame(dict(year=[2000, 2001, 2002], jobs=[40, 50, 20]))
     baseline = df.jobs[df.year == 2001].values[0]
     df["jobs_yoy"] = growth_pct_from(df, baseline)
-    
+
     ## Cumulative growth for two columns
     df = pd.DataFrame(dict(
-        year=[2000, 2001, 2002], 
-        jobs=[40, 50, 20], 
+        year=[2000, 2001, 2002],
+        jobs=[40, 50, 20],
         gva=[200, 250, 275]))
-    baseline = df.loc[df.year == df.year.min(), 
-                      ("jobs", "gva")].reindex(index=df.index, 
+    baseline = df.loc[df.year == df.year.min(),
+                      ("jobs", "gva")].reindex(index=df.index,
                                                method="nearest")
-    df[["jobs_growth", "gva_growth"]] = growth_pct_from(df[["jobs", "gva"]], 
+    df[["jobs_growth", "gva_growth"]] = growth_pct_from(df[["jobs", "gva"]],
                                                         baseline)
     df
     """
-    
+
     return (data / baseline - 1) * 100
 
 
-def growth_vars(data, columns=[], date_var=None, by=None, 
+def growth_vars(data, columns=[], date_var=None, by=None,
                 periods=1, baseline=None):
     """
     Calculate growth for columns in a dataframe
-    
+
     Parameters
     ----------
     data: DataFrame
-        Dataframe including a date column and one or more columns for which 
+        Dataframe including a date column and one or more columns for which
         to calculate growth.
 
     columns: str or list
         Names of columns for which to calculate growth.
-    
+
     date_var: str, optional
         Name of column whose values determine temporal order among data rows.
-    
+
     by: str, optional
         Name of column used to determine groups for `groupby`.
-    
+
     periods: int, default 1
         Lag, in number of rows, for calculating growth within time series.
         Ignored if `baseline` is specified.
-    
+
     baseline: "first", numeric, Series or DataFrame
         Value or values to calculate growth relative to.  If "first",
         cumulative growth is calculated relative to the row with the smallest
         value of `date_var`.  If `baseline` is not given, growth is
         calculated within each time series.
-    
+
     Returns
     -------
     DataFrame with same index as `data`, and columns from `columns`.
-    
+
     Examples
     --------
     # Period-on-period
     growth_vars(df, columns=["gva"], date_var="date", periods=1)
-    
+
     # Cumulative growth
     growth_vars(df, columns=["gva"], date_var="date", baseline="first")
 
     # Growth relative to single date.
     growth_vars(df, columns=["gva"], date_var="date", baseline="2019 Q4")
-    
+
     # Revisions from comparable dataframe.
     growth_vars(df, columns=["gva"], baseline=df_baseline)
 
 
     # Growth relative to single date, with a split factor.
     growth_vars(df, columns=["gva"], date_var="date", by="industry", baseline="2019 Q4")
-    
+
     # Same as:
     baseline = data.loc[df["date"]==min(df["date"]), :].groupby("industry")["gva"].first()
     growth_vars(df, columns=["gva"], date_var="date", baseline=baseline)
 
-    
+
     # Relative to calculated baseline for each level of `by`
     baseline = data.loc[data["year"]=="2019", :].groupby("industry")["gva"].mean()
     growth_vars(df, columns=["gva"], by="industry", baseline=baseline)
     """
-    
+
     # Ensure data columns include the ones we need.
     if date_var is not None:
         assert date_var in data.columns
     if by is not None:
         assert by in data.columns
     assert all(col in data.columns for col in columns), \
         f"Some of {columns} are missing from data columns {data.columns}"
 
-    
+
     # Make placeholder copy of data ready to inject results into `columns`.
     result = data.copy()
     result[columns] = np.nan
-    
+
     # Expand baseline shortcuts ("first" or a value to match data[date_var]).
     if baseline == "first":
         # Put baseline at earliest date value to get cumulative growth.
         if by is not None:
             baseline = data.loc[data[date_var]==min(data[date_var]), :].groupby(by)[columns].first()
         else:
             baseline = data.loc[data[date_var]==min(data[date_var]), :]
@@ -306,15 +308,15 @@
             # Take mean for each of the columns.
             baseline = df_baseline_raw.mean()
     elif isinstance(baseline, pd.DataFrame):
         # Expect baseline dataframe to have a value for each column, with optional `by` splits.
         pass
     else:
         assert baseline is None
-    
+
     if isinstance(baseline, pd.DataFrame):
         # Get relative change of data compared to baseline dataframe.
 
         assert all(col in baseline.columns for col in columns), \
             f"Some of {columns} are missing from baseline columns {baseline.columns}"
 
         if by is not None and date_var not in baseline.columns:
@@ -338,22 +340,22 @@
         result[columns] = 100 * sorted_data.pct_change(periods=periods)
     return result
 
 
 def index_to(data, baseline, to=100):
     """
     Scale data so values at `baseline` map to `to`
-    
+
     Examples
     --------
     # Index (2001 = 100)
     df = pd.DataFrame(dict(year=[2000, 2001, 2002], jobs=[40, 50, 20]))
     baseline = df.jobs[df.year == 2001].values[0]
     df["jobs_index"] = index_to(df.jobs, baseline)
     df
     #    year  jobs  jobs_index
     # 0  2000    40        80.0
     # 1  2001    50       100.0
     # 2  2002    20        40.0
     """
-    
+
     return data / baseline * to
```

### Comparing `xplorts-0.6/src/xplorts/ghostbokeh.py` & `xplorts-0.7/src/xplorts/ghostbokeh.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/slideselect.py` & `xplorts-0.7/src/xplorts/slideselect.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/dblprod/__init__.py` & `xplorts-0.7/src/xplorts/dblprod/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/dblprod/dblprod.py` & `xplorts-0.7/src/xplorts/dblprod/dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/dblprod/prodgrowsnap.py` & `xplorts-0.7/src/xplorts/dblprod/prodgrowsnap.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/dblprod/prodgrowts.py` & `xplorts-0.7/src/xplorts/dblprod/prodgrowts.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,93 +18,93 @@
 
 #%%
 
 # Suppress quarterly or monthly axis labels for time series longer than this.
 DATE_THRESHOLD = 40
 
 
-def figprodgrowts(data, 
-                  widget=None, 
+def figprodgrowts(data,
+                  widget=None,
                   varnames=None,
-                  date=None, 
-                  by=None, 
+                  date=None,
+                  by=None,
                   lprod=None,
                   gva=None,
                   labour=None,
                   color_map=None,
                   reverse_suffix=" (sign reversed)",
                   **kwargs):
     """
     Make interactive time series vertical bar chart of productivity growth components
-    
+
     Parameters
     ----------
     data : DataFrame
         Including columns to be plotted, which are named in other parameters.
     widget : Bokeh widget, optional
         The `value` attribute will be linked to the chart to make visible one
         value of the `by` variable.
     varnames : dict, optional
-        Mapping to specify column names for 'by', 'date', and the three 
+        Mapping to specify column names for 'by', 'date', and the three
         individual data variables 'lprod', 'gva', and 'labour'.
     date : str, optional
         Name of column containing time series dates to plot along the horizontal
         chart axis.  If not given, `varnames["date"]` is used.
     by : str, optional
         Name of column containing split levels.  The chart displays a single split
         level at a time.  If not given, `varnames["by"]` is used.
     lprod, gva, labour : str, optional
         Name of column containing values to be plotted as a time
         series line.  If not given, the value is looked up in `varnames`.
     kwargs : mapping
         Keyword arguments passed to `iv_dv_figure()`.
-    
+
     Returns
     -------
     Bokeh figure.
     """
-    
+
     if date is None:
         date = varnames["date"]
     if by is None:
         by = varnames["by"]
     if lprod is None:
         lprod = varnames["lprod"]
     if gva is None:
         gva = varnames["gva"]
     if labour is None:
         labour = varnames["labour"]
-    
+
     # Transform monthly and quarterly dates to nested categories.
-    datevar = varnames["date"]
+    datevar = date
     data_local = data.copy()
     data_local["_date_factor"] = date_tuples(data_local[datevar],
                                              length_threshold=DATE_THRESHOLD)
 
     # Prepare to suppress most quarters or months on axis if lots of them.
     suppress_factors = (isinstance(data_local["_date_factor"][0], tuple)
                         and len(data_local["_date_factor"].unique()) > DATE_THRESHOLD)
-    
+
     # Reverse sign of denominator variable (into new dataframe).
     labour_reversed = labour + reverse_suffix
     data_local = data_local.assign(**{labour_reversed: -data_local[labour]})
-    
+
     bar_variables = [gva, labour_reversed]
 
     ## Show time series growth components (bars) and total (line).
     fig_combi = iv_dv_figure(
         iv_data = data_local["_date_factor"],
         iv_axis = "x",
         suppress_factors = suppress_factors,
         title = "Cumulative growth",
         x_axis_label = kwargs.pop("x_axis_label", date),
         y_axis_label = kwargs.pop("y_axis_label", "Growth (percent)"),
         **kwargs
     )
-    
+
     if color_map is None:
         palette = palettes.Category20_3[::-1]
     else:
         palette = [color_map[var] for var in ("lprod", "gva", "labour")]
 
     ts_components_figure(
         fig_combi,
```

### Comparing `xplorts-0.6/src/xplorts/dblprod/prodlines.py` & `xplorts-0.7/src/xplorts/dblprod/prodlines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/dblprod/xpdblprod.py` & `xplorts-0.7/src/xplorts/dblprod/xpdblprod.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Make standalone interactive charts for time series productivity data
 
 When run from the command line, reads data from a CSV file and
 creates an HTML document that displays time series levels and cumulative
-growth components for one level of a split factor at a time, as well as 
+growth components for one level of a split factor at a time, as well as
 a snapshot of growth components across all levels of the split factor for
 one time period.
-      
-    In the CSV file, the first row of data defines column names.  
+
+    In the CSV file, the first row of data defines column names.
     The file should include:
-        - a column of dates (annual, quarterly or monthly), 
-        - a column of category names, and 
-        - one or more columns of data values to be plotted against dates.  
+        - a column of dates (annual, quarterly or monthly),
+        - a column of category names, and
+        - one or more columns of data values to be plotted against dates.
 
     An interactive chart is created, with widgets to select one of the
     category names (from a pulldown list or a slider).  The chart shows
     one line for each value column, with dates plotted along the horizontal
     axis.
-    
-    The interactive chart is saved as an HTML file which requires 
-    a web browser to view, but does not need an active internet connection.  
+
+    The interactive chart is saved as an HTML file which requires
+    a web browser to view, but does not need an active internet connection.
     Once created, the HTML file does not require Python,
     so it is easy to share the interactive chart.
 
 Command line interface
 ----------------------
 usage: dblprod.py [-h] [-b BY] [-d DATE] [-p LPROD] [-v GVA] [-l LABOUR]
                       [-g ARGS] [-t SAVE] [-s]
@@ -41,204 +41,248 @@
   -d DATE, --date DATE  Date variable
   -p LPROD, --lprod LPROD
                         Productivity variable
   -v GVA, --gva GVA     Gross value added (GVA) variable
   -l LABOUR, --labour LABOUR
                         Labour variable (e.g. jobs or hours worked)
   -g ARGS, --args ARGS  Keyword arguments.  YAML mapping of mappings.  The
-                        keys 'lines', 'growth_series' and 'growth_snapshot' 
+                        keys 'lines', 'growth_series' and 'growth_snapshot'
                         can provide keyword arguments to pass to
-                        `prod_ts_lines`, `prod_ts_growth` and 
+                        `prod_ts_lines`, `prod_ts_growth` and
                         `prod_growth_snapshot`, respectively.
   -t SAVE, --save SAVE  Interactive .html to save, if different from the
                         datafile base
   -s, --show            Show interactive .html
 """
 
 #%%
 # Bokeh imports.
-from bokeh.layouts import column, layout
+from bokeh.layouts import column, layout, row
+from bokeh.models import TabPanel, Tabs
 from bokeh.models.widgets import Div
 from bokeh.io import save, show
 from bokeh import palettes
 
 # Other external imports.
 import argparse
 from collections import defaultdict
 import pandas as pd
 from pathlib import Path
 import sys
 import textwrap
 import yaml
 
 # Internal imports.
-from ..base import (filter_widget, 
-                          set_output_file, unpack_data_varnames, 
+from ..base import (filter_widget,
+                          set_output_file, unpack_data_varnames,
                           variables_cmap)
 from ..dutils import growth_vars
+from ..heatmap import figheatmap
 from . import figprodgrowsnap, figprodlines, figprodgrowts
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
-    
+
     Returns
     -------
     `argparse.Namespace` object
-    
+
     Examples
     --------
     args = _parse_args()
     data = pd.read_csv(args.datafile)
-    
+
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
         prog="python -m xplorts.dblprod",
         description="Create interactive visualiser for labour productivity levels with a split factor"
     )
-    parser.add_argument("datafile", 
+    parser.add_argument("datafile",
                         help="File (CSV) with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Factor variable for splits")
 
     parser.add_argument("-d", "--date", type=str,
                         help="Date variable")
     parser.add_argument("-p", "--lprod", type=str,
-                        help="Productivity variable")    
-    parser.add_argument("-v", "--gva", 
+                        help="Productivity variable")
+    parser.add_argument("-v", "--gva",
                         type=str,
                         help="Gross value added (GVA) variable")
-    parser.add_argument("-l", "--labour", 
+    parser.add_argument("-l", "--labour",
                         type=str,
                         help="Labour variable (e.g. jobs or hours worked)")
-    parser.add_argument("-g", "--args", 
+    parser.add_argument("-g", "--args",
                         type=str,
                         help="""Keyword arguments.  YAML mapping of mappings.  The
-                            keys 'lines', 'growth_series' and 'growth_snapshot' 
+                            keys 'lines', 'growth_series' and 'growth_snapshot'
                             can provide keyword arguments to pass to
-                            `prod_ts_lines`, `prod_ts_growth` and 
+                            `prod_ts_lines`, `prod_ts_growth` and
                             `prod_growth_snapshot`, respectively.""")
 
-    parser.add_argument("-t", "--save", type=str, 
+    parser.add_argument("-t", "--save", type=str,
                         help="Interactive .html to save, if different from the datafile base")
 
-    parser.add_argument("-s", "--show", action="store_true", 
+    parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
 
     args = parser.parse_args()
 
     # Unpack YAML args into dict of dict of keyword args for various figures.
     # Will return an empty dict for keys not specified in --args option.
     args.args = {} if args.args is None else yaml.safe_load(args.args)
     args.args = defaultdict(dict, args.args)
 
     return(args)
 
-
 #%%
-    
+
+# Suppress quarterly or monthly axis labels for time series longer than this.
+DATE_THRESHOLD = 40
+
 def main():
     args = _parse_args()
 
     # Read the data as is.
     data = pd.read_csv(args.datafile, dtype=str)
-    
+
     # Unpack args specifying which data columns to use.
     varnames = unpack_data_varnames(
         args,
         ["date", "by", "lprod", "gva", "labour"],
         data.columns)
-    
+
     datevar = varnames["date"]
     dependent_variables = [varnames[var] for var in ("lprod", "gva", "labour")]
-    
+
     title = "xplor lprod: " + Path(args.datafile).stem
-    
+
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
 
     # Make palettes.
     color_map = variables_cmap(["labour", "gva", "lprod"],
                                palettes.Category20_3)
-    
+
     # Convert str to float so we can plot the data.
     data[dependent_variables] = data[dependent_variables].astype(float)
 
-    
+
     # Widget for `by`.
     split_widget = filter_widget(data[varnames["by"]], title=varnames["by"])
 
     # Widget for date.
     date_widget = filter_widget(data[datevar], start_value="last")
 
     fig_index_lines = figprodlines(
-        data, 
+        data,
         varnames=varnames,
         color_map=color_map,
-        widget=split_widget, 
+        widget=split_widget,
         height=300, width=600,
         **args.args["lines"])
 
 
     # Calculate cumulative growth.
     df_growth_cum = growth_vars(data,
                             date_var=datevar,
-                            columns=dependent_variables, 
+                            columns=dependent_variables,
                             by=varnames["by"],
                             baseline="first",
                            )
 
     fig_ts_growth = figprodgrowts(
         df_growth_cum,
-        varnames=varnames, 
+        varnames=varnames,
         color_map=color_map,
-        widget=split_widget, 
+        widget=split_widget,
         height=300, width=600,
         **args.args["growth_series"])
 
 
     # Calculate period-on-period growth.
     df_growth = growth_vars(data,
                             date_var=datevar,
-                            columns=dependent_variables, 
+                            columns=dependent_variables,
                             by=varnames["by"],
                             periods=1,
                            )
-    
+
     # Truncate long levels of `by`, for axis labels.
     by_var = varnames["by"]
     df_growth[by_var] = df_growth[by_var].apply(
         textwrap.shorten, args=(15,), placeholder='..'
     )
-    
+
     fig_growth_snapshot = figprodgrowsnap(
         df_growth,
-        varnames=varnames, 
+        varnames=varnames,
         color_map=color_map,
-        widget=date_widget, 
+        widget=date_widget,
         height=600, width=300,
         **args.args["growth_snapshot"])
 
-    # Make app that shows widget and charts.
+    # Put level and growth charts, with widgets, on a tab.
     ts_charts = column(split_widget, fig_index_lines, fig_ts_growth)
     snapshot = column(date_widget, fig_growth_snapshot)
+    tab_levels = TabPanel(
+        title="Levels",
+        child=layout([
+            [ts_charts, snapshot],
+            ]))
+
+
+    ## Growth heatmap tab.
+    growth_heatmap = figheatmap(
+        df_growth,
+        x=varnames["date"],
+        y=varnames["by"],
+        values=varnames["lprod"],
+        x_widget=date_widget.handle,
+        y_widget=split_widget.handle,
+        title=varnames["lprod"] + " growth",
+        figure_options=dict(width=900, height=600),
+        )
+    tab_growth = TabPanel(
+        title="Growth heatmap",
+        child=row([growth_heatmap, fig_growth_snapshot, date_widget.handle]),
+        )
+
+
+    ## Cumulative growth heatmap tab.
+    cum_growth_heatmap = figheatmap(
+        df_growth_cum,
+        x=varnames["date"],
+        y=varnames["by"],
+        values=varnames["lprod"],
+        x_widget=date_widget.handle,
+        y_widget=split_widget.handle,
+        title=varnames["lprod"] + " cumulative growth",
+        figure_options=dict(width=900, height=600),
+        )
+    tab_cum_growth = TabPanel(
+        title="Cum growth heatmap",
+        child=column([cum_growth_heatmap, fig_ts_growth, split_widget.handle]),
+        )
+
+    # Make app that shows tabs of various charts.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
-        [ts_charts, snapshot], 
-    ])
-    
+        Tabs(tabs=[tab_levels, tab_growth, tab_cum_growth])])
+
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
 #%%
```

### Comparing `xplorts-0.6/src/xplorts/lines/lines.py` & `xplorts-0.7/src/xplorts/lines/lines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/lines/xplines.py` & `xplorts-0.7/src/xplorts/lines/xplines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/scatter/scatter.py` & `xplorts-0.7/src/xplorts/scatter/scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/scatter/xpscatter.py` & `xplorts-0.7/src/xplorts/scatter/xpscatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/snapcomp/__init__.py` & `xplorts-0.7/src/xplorts/snapcomp/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/snapcomp/snapcomp.py` & `xplorts-0.7/src/xplorts/snapcomp/snapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/snapcomp/xpsnapcomp.py` & `xplorts-0.7/src/xplorts/snapcomp/xpsnapcomp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Make standalone chart showing horizontal snapshot components and total.
 
 When run from the command line, reads data from a CSV file and
 creates an HTML document that displays snapshot
 components for one level of a split factor at a time.
-      
-    In the CSV file, the first row of data defines column names.  
+
+    In the CSV file, the first row of data defines column names.
     The file should include:
-        - a column of category names for the vertical chart axis, 
+        - a column of category names for the vertical chart axis,
         - a column of category names for the split factor
-        - a column of data totals at each level along the vertical axis, and 
+        - a column of data totals at each level along the vertical axis, and
         - one or more columns of value components for each total.
 
     An interactive chart is created, with widgets to select one of the
     split factor levels (from a pulldown list or a slider).  The chart plots
     value components as horizontal stacked bars with a marker for each total.
-    
-    The interactive chart is saved as an HTML file which requires 
-    a web browser to view, but does not need an active internet connection.  
+
+    The interactive chart is saved as an HTML file which requires
+    a web browser to view, but does not need an active internet connection.
     Once created, the HTML file does not require Python,
     so it is easy to share the interactive chart.
 
 Command line interface
 ----------------------
 usage: snapcomp.py [-h] [-b BY] [-y IV] [-m MARKERS] [-x BARS [BARS ...]] [-L]
                    [-g ARGS] [-t SAVE] [-s]
@@ -63,126 +63,126 @@
 from pathlib import Path
 import pandas as pd
 import sys
 import yaml
 
 ## Imports from this package
 from xplorts.snapcomp import components_figure, link_widget_to_snapcomp_figure
-from xplorts.base import (iv_dv_figure, filter_widget, 
-                          set_output_file, 
+from xplorts.base import (iv_dv_figure, filter_widget,
+                          set_output_file,
                           unpack_data_varnames, variables_cmap)
 
 #%%
 
 def _parse_args():
     """
     Parse command line arguments
-    
+
     Returns
     -------
     `argparse.Namespace` object
-    
+
     Examples
     --------
     args = _parse_args()
     data = pd.read_csv(args.datafile)
-    
+
     Resources
     ---------
     [argparse — Parser for command-line options, arguments and sub-commands](https://docs.python.org/3/library/argparse.html#dest)
     """
     # Check command line arguments.
     parser = argparse.ArgumentParser(
         prog="python -m xplorts.snapcomp",
         description="Create interactive horizontal bar chart for snapshot components with a split factor"
     )
-    parser.add_argument("datafile", 
+    parser.add_argument("datafile",
                         help="File (CSV) with data series and split factor")
     parser.add_argument("-b", "--by", type=str,
                         help="Factor variable for splits")
 
     parser.add_argument("-y", "--iv", type=str,
                         help="Name of independent categorical variable for vertical axis")
 
     parser.add_argument("-m", "--markers", type=str,
                         help="Variable to show as marker points")
-    parser.add_argument("-x", "--bars", 
+    parser.add_argument("-x", "--bars",
                         nargs="+", type=str,
                         help="Variables to show as horizontal stacked bars")
 
-    parser.add_argument("-L", "--last", action="store_true", 
+    parser.add_argument("-L", "--last", action="store_true",
                         help="Initial chart shows last level of `by` variable")
 
-    parser.add_argument("-g", "--args", 
+    parser.add_argument("-g", "--args",
                         type=str,
                         help="""Keyword arguments.  YAML mapping of mappings.  The
-                            keys 'lines' and 'bars' 
+                            keys 'lines' and 'bars'
                             can provide keyword arguments to pass to
                             `components_figure()`.""")
 
-    parser.add_argument("-t", "--save", type=str, 
+    parser.add_argument("-t", "--save", type=str,
                         help="Interactive .html to save, if different from the datafile base")
 
-    parser.add_argument("-s", "--show", action="store_true", 
+    parser.add_argument("-s", "--show", action="store_true",
                         help="Show interactive .html")
 
     args = parser.parse_args()
 
     # Unpack YAML args into dict of keyword args for ts_components_figure().
     args.args = {} if args.args is None else yaml.safe_load(args.args)
     return(args)
 
 #%%
 
 def main():
-    # Running from command line.    
+    # Running from command line.
     args = _parse_args()
 
     data = pd.read_csv(args.datafile, dtype=str)
-    
-    title = "tscomp: " + Path(args.datafile).stem
-    
+
+    title = "snapcomp: " + Path(args.datafile).stem
+
     # Configure output file for interactive html.
     set_output_file(
         args.save or args.datafile,
         title = title
     )
-    
+
     # Unpack args specifying which data columns to use.
     varnames = unpack_data_varnames(
         args,
         ["iv", "by", "markers", "bars"],
         data.columns)
-    
+
     # Make list of dependent variables for bars plus markers, if any.
     markervar = varnames["markers"]
     dependent_variables = varnames["bars"].copy()
     if markervar is not None:
         dependent_variables.insert(0, markervar)
-    
+
     # Convert str to float so we can plot the data.
     data[dependent_variables] = data[dependent_variables].astype(float)
 
     default_color_map = variables_cmap(dependent_variables[::-1],
                                        palettes.Category20_20)
     default_bar_colors = [default_color_map[var] for var in varnames["bars"]]
 
     fig = iv_dv_figure(
         iv_data = reversed(data[varnames["iv"]].unique()),
         iv_axis = "y",
     )
-    
+
     if markervar is None:
         scatter_args = {}
     else:
         # Use specified scatter_args, else defaults.
         scatter_args = args.args.pop(
             "scatter_args",
             {"color": default_color_map[markervar]})
-        
+
     # Use specified bar_args, else defaults.
     bar_args = args.args.pop(
         "bar_args",
         {"color": default_bar_colors})
 
     # Make chart, and link widget to make one factor level visible.
     renderers = components_figure(
@@ -205,15 +205,15 @@
 
     # Make app that shows widget and chart.
     app = layout([
         Div(text="<h1>" + title),  # Show title as level 1 heading.
         [widget],
         [fig]
     ])
-    
+
     if args.show:
         show(app)  # Save file and display in web browser.
     else:
         save(app)  # Save file.
 
 #%%
 if __name__ == "__main__":
```

### Comparing `xplorts-0.6/src/xplorts/stacks/bokeh_stacks.py` & `xplorts-0.7/src/xplorts/stacks/bokeh_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/stacks/stacks.py` & `xplorts-0.7/src/xplorts/stacks/stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/stacks/stacks_util.py` & `xplorts-0.7/src/xplorts/stacks/stacks_util.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/stacks/xpstacks.py` & `xplorts-0.7/src/xplorts/stacks/xpstacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/tscomp/__init__.py` & `xplorts-0.7/src/xplorts/tscomp/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/tscomp/tscomp.py` & `xplorts-0.7/src/xplorts/tscomp/tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/tscomp/xptscomp.py` & `xplorts-0.7/src/xplorts/tscomp/xptscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/src/xplorts/utils/ukons_lprod_to_csv.py` & `xplorts-0.7/src/xplorts/utils/ukons_lprod_to_csv.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/conftest.py` & `xplorts-0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/test_dblprod.py` & `xplorts-0.7/tests/test_dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/test_lines.py` & `xplorts-0.7/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/test_scatter.py` & `xplorts-0.7/tests/test_scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/test_snapcomp.py` & `xplorts-0.7/tests/test_snapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/test_stacks.py` & `xplorts-0.7/tests/test_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/tests/test_tscomp.py` & `xplorts-0.7/tests/test_tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/.gitignore` & `xplorts-0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/LICENSE` & `xplorts-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xplorts-0.6/README.md` & `xplorts-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 
 <!-- This document uses
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) -->
 
-# Explore time series datasets 
+# Explore time series datasets
 
-**`xplorts`** ("explore-ts") is a collection of Python tools to make standalone HTML documents containing interactive charts.  It is particularly aimed at showing time series data (hence the "ts") with annual, quarterly or monthly periodicity, such as that published by national statistical institutes by way of national accounts, productivity, or labour markets series. 
+**`xplorts`** ("explore-ts") is a collection of Python tools to make standalone HTML documents containing interactive charts.  It is particularly aimed at showing time series data (hence the "ts") with annual, quarterly or monthly periodicity, such as that published by national statistical institutes by way of national accounts, productivity, or labour markets series.
 
 Once created, the HTML documents can be used with any web browser.  They do not need an
 active internet connection.
 
 <details>
    <summary>
 
 ## Installation
 </summary>
-   
+
 ```
 pip install xplorts
 ```
+
+For `xplorts.utils.ukons_lprod_to_csv`, you also need `openpyxl`:
+```
+pip install openpyxl
+```
 </details>
 <details>
 <summary>
-   
+
 ## Demo
 </summary>
 
 To see an interactive sample data explorer, try [Explore UK output per hour worked](docs/xplor_lprod%20oph%20annual%20by%20section.html).
 
 > Source: Office for National Statistics licensed under the Open Government Licence v.3.0
 
@@ -51,21 +56,22 @@
 1. Use the explorer in any web browser.
 </details>
 
 
 <details>
 <summary>
 
-## Features 
+## Features
 </summary>
-   
+
 The labour productivity explorer demonstrates these features:
 - A grouped multi-line chart shows a set of related lines for one split level at a time, like time series for productivity, gross value added, and hours worked for a particular industry.<br> ![Thumbnail screenshot of lines chart](docs/png/xplor_lprod_lines_thumbnail_large.png)
 - A time series components chart shows a set of stacked bars in combination with a totals line, for one split level at a time, like cumulative growth time series for gross value added, hours worked (sign reversed), and productivity for a particular industry.<br> ![Thumbnail screenshot of time series growth components chart](docs/png/xplor_lprod_tscomp_thumbnail_large.png)
 - A snapshot growth components chart shows a set of stacked bars in combination with markers showing total growth, as a function of a categorical factor, like growth for gross value added and hours worked (sign reversed) by industry, along with growth in productivity, for a selectable time period.<br> ![Thumbnail screenshot of snapshot growth components chart](docs/png/xplor_lprod_snapcomp_thumbnail_large.png)
+- A heatmap chart shows data values as a function of a categorical split variable across time.
 - Drop-down list and slider widgets provide interactive selection of a categorical split level or snapshot time period to show. Static screenshots are shown here, but check out the interactive sample data explorer at the link above.<br> ![Screenshot of widgets to select industry](docs/png/slideselect_industry.png) ![Screenshot of widgets to select date](docs/png/slideselect_date.png)
 - Hover tool displays data values at the cursor location.
 - Chart tools include box zoom, wheel zoom, pan, and save to file.
 - Time periods can be represented on a chart axis as nested categories like (year, quarter).
 - A categorical chart axis can represent time periods or levels of a split factor.
 </details>
 
@@ -95,87 +101,98 @@
 ### Modules
 
 Module | Description
 --- | ---
 base | Miscellaneous helper functions and classes.
 dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
 ghostbokeh | Define an abstract base class to a build pseudo-subclass of a Bokeh class.
+heatmap | Functions to create a heatmap of data values as a function of horizontal and vertical categorical variables.
 lines | Modify a Bokeh Figure by adding line charts to show several time series with a split factor.
 scatter | Modify a Bokeh Figure by adding scatter charts to show one or more categorical series with a split factor.
 slideselect | Defines a class combining select and slider widgets, with support for javascript linking to other objects.
 snapcomp | Modify a Bokeh Figure by adding a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
 stacks | Modify a Bokeh Figure by adding a horizontal or vertical stacked bar chart showing several data series with a split factor.
-tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.  
+tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.
 </details>
 
 <details>
    <summary>
 
 ## Using `xplorts` on the command line
    </summary>
-   
+
 - Install (once, possibly within a particular virtual environment)
 - Open a `Terminal` window (Macintosh) or `Command prompt` window (Windows)
 - Activate virtual environment, if relevant
 
     On Windows:
-    
+
     ```activate my_env```
-    
+
     On Mac:
-    
+
     ```conda activate my_env```
-- Tell `python` to run an `xplorts` module
+- Execute an `xplorts` module entry point
+  ```
+  xp-dblprod ...
+  ```
+- Or tell `python` explicitly to run an `xplorts` module
 
   ```
   python -m xplorts.dblprod ...
   ```
 
 ### Getting help about command line options
 
 Pass the option `-h` to any `xplorts` script to get help.  For example:
-```
-python -m xplorts.dblprod -h
-```
+  ```
+  xp-dblprod -h
+  ```
+
+Or
+  ```
+  python -m xplorts.dblprod -h
+  ```
 
 > <pre>
 > usage: dblprod.py [-h] [-b BY] [-d DATE] [-p LPROD] [-v GVA] [-l LABOUR]
 >                       [-g ARGS] [-t SAVE] [-s]
 >                       datafile
-> 
+>
 > Create interactive visualiser for labour productivity levels with a split
 > factor
-> 
+>
 > positional arguments:
 >   datafile              File (CSV) with data series and split factor
-> 
+>
 > optional arguments:
 >   -h, --help            Show this help message and exit
 >   -b BY, --by BY        Factor variable for splits
 >   -d DATE, --date DATE  Date variable
 >   -p LPROD, --lprod LPROD
 >                         Productivity variable
 >   -v GVA, --gva GVA     Gross value added (GVA) variable
 >   -l LABOUR, --labour LABOUR
 >                         Labour variable (e.g. jobs or hours worked)
 >   -g ARGS, --args ARGS  Keyword arguments.  YAML mapping of mappings.  The
->                         keys 'lines', 'growth_series' and 'growth_snapshot' 
+>                         keys 'lines', 'growth_series' and 'growth_snapshot'
 >                         can provide keyword arguments to pass to
->                         `prod_ts_lines`, `prod_ts_growth` and 
+>                         `prod_ts_lines`, `prod_ts_growth` and
 >                         `prod_growth_snapshot`, respectively.
 >   -t SAVE, --save SAVE  Interactive .html to save, if different from the
 >                         datafile base
 >   -s, --show            Show interactive .html
 </pre>
 
 ### `xplorts` scripts
 
-Script | Description
---- | ---
-dblprod | Create a labour productivity dashboard, with three charts including: <ul><li>a lines chart showing levels of labour productivity, gross value added, and labour,</li> <li>a time series growth components chart showing cumulative growth in labour productivity, gross value added, and labour, and</li> <li>a snapshot growth components chart showing period-on-period growth in labour productivity, gross value added, and labour.</li>
-lines | Create a line chart showing several time series with a split factor.  Widgets select one split factor category at a time.
-scatter | Create scatter chart showing one or more time series with a split factor.  Widgets select one split factor category at a time.
-snapcomp | Create a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and a line showing overall growth.  A widget selects one time period at a time.
-stacks | Create stacked bar chart showing several data series with a split factor.  Widgets select one split factor at a time (or one time period at a time if the split factor is plotted as a chart axis).
-tscomp | Create a time series growth components chart, with time periods along the horizontal axis, vertical stacked bars showing growth components, and a line showing overall growth.  Widgets select one split factor category at a time.
-utils/ukons_lprod_to_csv.py | Extract data from ONS labour productivity datasets such as [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk), in a format suitable for use with `xplorts` charts.
+Script | Entry point | Description
+--- | --- | ---
+dblprod | xp-dblprod | Create a labour productivity dashboard, with three charts including: <ul><li>a lines chart showing levels of labour productivity, gross value added, and labour,</li> <li>a time series growth components chart showing cumulative growth in labour productivity, gross value added, and labour, and</li> <li>a snapshot growth components chart showing period-on-period growth in labour productivity, gross value added, and labour.</li>
+heatmap | xp-heatmap | Create a heatmap of values as a function of two categorical variables.
+lines | xp-lines | Create a line chart showing several time series with a split factor.  Widgets select one split factor category at a time.
+scatter | xp-scatter | Create scatter chart showing one or more time series with a split factor.  Widgets select one split factor category at a time.
+snapcomp | xp-snapcomp | Create a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and a line showing overall growth.  A widget selects one time period at a time.
+stacks | xp-stacks | Create stacked bar chart showing several data series with a split factor.  Widgets select one split factor at a time (or one time period at a time if the split factor is plotted as a chart axis).
+tscomp | xp-tscomp | Create a time series growth components chart, with time periods along the horizontal axis, vertical stacked bars showing growth components, and a line showing overall growth.  Widgets select one split factor category at a time.
+utils.ukons_lprod_to_csv |  | Extract data from ONS labour productivity datasets such as [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk), in a format suitable for use with `xplorts` charts.
 </details>
```

### Comparing `xplorts-0.6/pyproject.toml` & `xplorts-0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xplorts"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Todd M Bailey", email="tmb@baileywick.plus.com" },
 ]
 description = "Make standalone interactive HTML charts to explore time series datasets"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.6"
@@ -23,14 +23,15 @@
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     'Development Status :: 3 - Alpha',
 ]
 
 [project.scripts]
 xp-dblprod = "xplorts.dblprod.xpdblprod:main"
+xp-heatmap = "xplorts.heatmap.xpheatmap:main"
 xp-lines = "xplorts.lines.xplines:main"
 xp-scatter = "xplorts.scatter.xpscatter:main"
 xp-snapcomp = "xplorts.snapcomp.xpsnapcomp:main"
 xp-stacks = "xplorts.stacks.xpstacks:main"
 xp-tscomp = "xplorts.tscomp.xptscomp:main"
 
 [project.urls]
```

### Comparing `xplorts-0.6/PKG-INFO` & `xplorts-0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplorts
-Version: 0.6
+Version: 0.7
 Summary: Make standalone interactive HTML charts to explore time series datasets
 Project-URL: Homepage, https://github.com/xplorts/xplorts
 Project-URL: Bug Tracker, https://github.com/xplorts/xplorts/issues
 Author-email: Todd M Bailey <tmb@baileywick.plus.com>
 License: Copyright 2023 Todd Bailey
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
@@ -103,34 +103,39 @@
 Requires-Dist: pyyaml>=5.4.1
 Description-Content-Type: text/markdown
 
 
 <!-- This document uses
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) -->
 
-# Explore time series datasets 
+# Explore time series datasets
 
-**`xplorts`** ("explore-ts") is a collection of Python tools to make standalone HTML documents containing interactive charts.  It is particularly aimed at showing time series data (hence the "ts") with annual, quarterly or monthly periodicity, such as that published by national statistical institutes by way of national accounts, productivity, or labour markets series. 
+**`xplorts`** ("explore-ts") is a collection of Python tools to make standalone HTML documents containing interactive charts.  It is particularly aimed at showing time series data (hence the "ts") with annual, quarterly or monthly periodicity, such as that published by national statistical institutes by way of national accounts, productivity, or labour markets series.
 
 Once created, the HTML documents can be used with any web browser.  They do not need an
 active internet connection.
 
 <details>
    <summary>
 
 ## Installation
 </summary>
-   
+
 ```
 pip install xplorts
 ```
+
+For `xplorts.utils.ukons_lprod_to_csv`, you also need `openpyxl`:
+```
+pip install openpyxl
+```
 </details>
 <details>
 <summary>
-   
+
 ## Demo
 </summary>
 
 To see an interactive sample data explorer, try [Explore UK output per hour worked](docs/xplor_lprod%20oph%20annual%20by%20section.html).
 
 > Source: Office for National Statistics licensed under the Open Government Licence v.3.0
 
@@ -156,21 +161,22 @@
 1. Use the explorer in any web browser.
 </details>
 
 
 <details>
 <summary>
 
-## Features 
+## Features
 </summary>
-   
+
 The labour productivity explorer demonstrates these features:
 - A grouped multi-line chart shows a set of related lines for one split level at a time, like time series for productivity, gross value added, and hours worked for a particular industry.<br> ![Thumbnail screenshot of lines chart](docs/png/xplor_lprod_lines_thumbnail_large.png)
 - A time series components chart shows a set of stacked bars in combination with a totals line, for one split level at a time, like cumulative growth time series for gross value added, hours worked (sign reversed), and productivity for a particular industry.<br> ![Thumbnail screenshot of time series growth components chart](docs/png/xplor_lprod_tscomp_thumbnail_large.png)
 - A snapshot growth components chart shows a set of stacked bars in combination with markers showing total growth, as a function of a categorical factor, like growth for gross value added and hours worked (sign reversed) by industry, along with growth in productivity, for a selectable time period.<br> ![Thumbnail screenshot of snapshot growth components chart](docs/png/xplor_lprod_snapcomp_thumbnail_large.png)
+- A heatmap chart shows data values as a function of a categorical split variable across time.
 - Drop-down list and slider widgets provide interactive selection of a categorical split level or snapshot time period to show. Static screenshots are shown here, but check out the interactive sample data explorer at the link above.<br> ![Screenshot of widgets to select industry](docs/png/slideselect_industry.png) ![Screenshot of widgets to select date](docs/png/slideselect_date.png)
 - Hover tool displays data values at the cursor location.
 - Chart tools include box zoom, wheel zoom, pan, and save to file.
 - Time periods can be represented on a chart axis as nested categories like (year, quarter).
 - A categorical chart axis can represent time periods or levels of a split factor.
 </details>
 
@@ -200,87 +206,98 @@
 ### Modules
 
 Module | Description
 --- | ---
 base | Miscellaneous helper functions and classes.
 dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
 ghostbokeh | Define an abstract base class to a build pseudo-subclass of a Bokeh class.
+heatmap | Functions to create a heatmap of data values as a function of horizontal and vertical categorical variables.
 lines | Modify a Bokeh Figure by adding line charts to show several time series with a split factor.
 scatter | Modify a Bokeh Figure by adding scatter charts to show one or more categorical series with a split factor.
 slideselect | Defines a class combining select and slider widgets, with support for javascript linking to other objects.
 snapcomp | Modify a Bokeh Figure by adding a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
 stacks | Modify a Bokeh Figure by adding a horizontal or vertical stacked bar chart showing several data series with a split factor.
-tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.  
+tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.
 </details>
 
 <details>
    <summary>
 
 ## Using `xplorts` on the command line
    </summary>
-   
+
 - Install (once, possibly within a particular virtual environment)
 - Open a `Terminal` window (Macintosh) or `Command prompt` window (Windows)
 - Activate virtual environment, if relevant
 
     On Windows:
-    
+
     ```activate my_env```
-    
+
     On Mac:
-    
+
     ```conda activate my_env```
-- Tell `python` to run an `xplorts` module
+- Execute an `xplorts` module entry point
+  ```
+  xp-dblprod ...
+  ```
+- Or tell `python` explicitly to run an `xplorts` module
 
   ```
   python -m xplorts.dblprod ...
   ```
 
 ### Getting help about command line options
 
 Pass the option `-h` to any `xplorts` script to get help.  For example:
-```
-python -m xplorts.dblprod -h
-```
+  ```
+  xp-dblprod -h
+  ```
+
+Or
+  ```
+  python -m xplorts.dblprod -h
+  ```
 
 > <pre>
 > usage: dblprod.py [-h] [-b BY] [-d DATE] [-p LPROD] [-v GVA] [-l LABOUR]
 >                       [-g ARGS] [-t SAVE] [-s]
 >                       datafile
-> 
+>
 > Create interactive visualiser for labour productivity levels with a split
 > factor
-> 
+>
 > positional arguments:
 >   datafile              File (CSV) with data series and split factor
-> 
+>
 > optional arguments:
 >   -h, --help            Show this help message and exit
 >   -b BY, --by BY        Factor variable for splits
 >   -d DATE, --date DATE  Date variable
 >   -p LPROD, --lprod LPROD
 >                         Productivity variable
 >   -v GVA, --gva GVA     Gross value added (GVA) variable
 >   -l LABOUR, --labour LABOUR
 >                         Labour variable (e.g. jobs or hours worked)
 >   -g ARGS, --args ARGS  Keyword arguments.  YAML mapping of mappings.  The
->                         keys 'lines', 'growth_series' and 'growth_snapshot' 
+>                         keys 'lines', 'growth_series' and 'growth_snapshot'
 >                         can provide keyword arguments to pass to
->                         `prod_ts_lines`, `prod_ts_growth` and 
+>                         `prod_ts_lines`, `prod_ts_growth` and
 >                         `prod_growth_snapshot`, respectively.
 >   -t SAVE, --save SAVE  Interactive .html to save, if different from the
 >                         datafile base
 >   -s, --show            Show interactive .html
 </pre>
 
 ### `xplorts` scripts
 
-Script | Description
---- | ---
-dblprod | Create a labour productivity dashboard, with three charts including: <ul><li>a lines chart showing levels of labour productivity, gross value added, and labour,</li> <li>a time series growth components chart showing cumulative growth in labour productivity, gross value added, and labour, and</li> <li>a snapshot growth components chart showing period-on-period growth in labour productivity, gross value added, and labour.</li>
-lines | Create a line chart showing several time series with a split factor.  Widgets select one split factor category at a time.
-scatter | Create scatter chart showing one or more time series with a split factor.  Widgets select one split factor category at a time.
-snapcomp | Create a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and a line showing overall growth.  A widget selects one time period at a time.
-stacks | Create stacked bar chart showing several data series with a split factor.  Widgets select one split factor at a time (or one time period at a time if the split factor is plotted as a chart axis).
-tscomp | Create a time series growth components chart, with time periods along the horizontal axis, vertical stacked bars showing growth components, and a line showing overall growth.  Widgets select one split factor category at a time.
-utils/ukons_lprod_to_csv.py | Extract data from ONS labour productivity datasets such as [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk), in a format suitable for use with `xplorts` charts.
+Script | Entry point | Description
+--- | --- | ---
+dblprod | xp-dblprod | Create a labour productivity dashboard, with three charts including: <ul><li>a lines chart showing levels of labour productivity, gross value added, and labour,</li> <li>a time series growth components chart showing cumulative growth in labour productivity, gross value added, and labour, and</li> <li>a snapshot growth components chart showing period-on-period growth in labour productivity, gross value added, and labour.</li>
+heatmap | xp-heatmap | Create a heatmap of values as a function of two categorical variables.
+lines | xp-lines | Create a line chart showing several time series with a split factor.  Widgets select one split factor category at a time.
+scatter | xp-scatter | Create scatter chart showing one or more time series with a split factor.  Widgets select one split factor category at a time.
+snapcomp | xp-snapcomp | Create a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and a line showing overall growth.  A widget selects one time period at a time.
+stacks | xp-stacks | Create stacked bar chart showing several data series with a split factor.  Widgets select one split factor at a time (or one time period at a time if the split factor is plotted as a chart axis).
+tscomp | xp-tscomp | Create a time series growth components chart, with time periods along the horizontal axis, vertical stacked bars showing growth components, and a line showing overall growth.  Widgets select one split factor category at a time.
+utils.ukons_lprod_to_csv |  | Extract data from ONS labour productivity datasets such as [Output per hour worked, UK](https://www.ons.gov.uk/economy/economicoutputandproductivity/productivitymeasures/datasets/outputperhourworkeduk), in a format suitable for use with `xplorts` charts.
 </details>
```

