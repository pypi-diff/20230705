# Comparing `tmp/covdrugsim-0.1.0.tar.gz` & `tmp/covdrugsim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covdrugsim-0.1.0.tar", max compression
+gzip compressed data, was "covdrugsim-0.2.0.tar", max compression
```

## Comparing `covdrugsim-0.1.0.tar` & `covdrugsim-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
--rwxr-xr-x   0        0        0     1082 2023-06-25 06:40:55.376092 covdrugsim-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     5081 2023-06-25 15:10:03.390306 covdrugsim-0.1.0/README.md
--rwxr-xr-x   0        0        0     1232 2023-06-25 15:21:18.795581 covdrugsim-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-25 07:06:17.007612 covdrugsim-0.1.0/src/covdrugsim/__init__.py
--rwxr-xr-x   0        0        0        1 2023-06-25 14:55:55.394786 covdrugsim-0.1.0/src/covdrugsim/covdrugsim.py
--rwxr-xr-x   0        0        0     3833 2023-06-25 09:03:59.690086 covdrugsim-0.1.0/src/covdrugsim/mdsim/SCbondDist.py
--rwxr-xr-x   0        0        0     8135 2023-06-25 09:03:41.579868 covdrugsim-0.1.0/src/covdrugsim/mdsim/baseID.py
--rwxr-xr-x   0        0        0     6071 2023-06-25 09:03:11.585350 covdrugsim-0.1.0/src/covdrugsim/mdsim/bbRMSD.py
--rwxr-xr-x   0        0        0      331 2023-06-25 08:30:52.899621 covdrugsim-0.1.0/src/covdrugsim/mdsim/config.py
--rwxr-xr-x   0        0        0     3078 2023-06-25 09:02:35.308230 covdrugsim-0.1.0/src/covdrugsim/mdsim/hbondAnalysis.py
--rwxr-xr-x   0        0        0     3911 2023-06-25 09:01:45.594821 covdrugsim-0.1.0/src/covdrugsim/mdsim/ligDihedral.py
--rwxr-xr-x   0        0        0     5644 2023-06-25 14:35:06.411726 covdrugsim-0.1.0/src/covdrugsim/mdsim/prepMTB.py
--rwxr-xr-x   0        0        0      454 2023-06-25 08:30:52.900944 covdrugsim-0.1.0/src/covdrugsim/mdsim/sumCharge.py
--rwxr-xr-x   0        0        0     1837 2023-06-25 09:11:46.641050 covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/admin.py
--rwxr-xr-x   0        0        0     1377 2023-06-25 08:55:59.258113 covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/gsub.sh
--rwxr-xr-x   0        0        0     4401 2023-06-25 09:10:58.751316 covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/prepGaussian.py
--rwxr-xr-x   0        0        0     1325 2023-06-25 09:10:22.150861 covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/settings.py
--rwxr-xr-x   0        0        0     4963 2023-06-25 09:10:43.657395 covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/tabulate.py
--rwxr-xr-x   0        0        0     3047 2023-06-25 21:06:10.609582 covdrugsim-0.1.0/src/covdrugsim/qmcalc/unitConv/unitConv.py
--rwxr-xr-x   0        0        0      189 2023-06-25 08:26:39.463954 covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/README.md
--rwxr-xr-x   0        0        0    17871 2023-06-25 08:57:19.019498 covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
--rwxr-xr-x   0        0        0     2622 2023-06-25 08:26:39.401013 covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/example.inp
--rwxr-xr-x   0        0        0    11782 2023-06-25 09:07:45.245749 covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
--rwxr-xr-x   0        0        0    13760 2023-06-25 09:08:28.709471 covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
--rw-r--r--   0        0        0     6093 2023-06-25 21:27:14.971735 covdrugsim-0.1.0/setup.py
--rw-r--r--   0        0        0     5707 2023-06-25 21:27:14.973716 covdrugsim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-05 09:33:37.229976 covdrugsim-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6643 2023-07-05 09:33:37.229976 covdrugsim-0.2.0/README.md
+-rw-r--r--   0        0        0     1956 2023-07-05 09:34:16.390584 covdrugsim-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      733 2023-07-05 09:34:16.390584 covdrugsim-0.2.0/setup.py
+-rw-r--r--   0        0        0     1058 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/data/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/data/chargesExample.txt
+-rw-r--r--   0        0        0     4449 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/data/energyLevellerExample.inp
+-rw-r--r--   0        0        0      474 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/datasets.py
+-rw-r--r--   0        0        0      241 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/main.py
+-rw-r--r--   0        0        0     3839 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/SCbondDist.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/__init__.py
+-rw-r--r--   0        0        0     8141 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/baseID.py
+-rw-r--r--   0        0        0     6071 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/bbRMSD.py
+-rw-r--r--   0        0        0      331 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/config.py
+-rw-r--r--   0        0        0     3084 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/hbondAnalysis.py
+-rw-r--r--   0        0        0     3917 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/ligDihedral.py
+-rw-r--r--   0        0        0      769 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/mdAnalyse.py
+-rw-r--r--   0        0        0     5644 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/mdsim/prepMTB.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/admin.py
+-rw-r--r--   0        0        0     1377 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/gsub.sh
+-rw-r--r--   0        0        0     4421 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/prepGaussian.py
+-rw-r--r--   0        0        0     1325 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/settings.py
+-rw-r--r--   0        0        0     4914 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/tabulate.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/unitConv/__init__.py
+-rw-r--r--   0        0        0     4241 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/unitConv/unitConv.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/__init__.py
+-rw-r--r--   0        0        0    17951 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
+-rw-r--r--   0        0        0    11782 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
+-rw-r--r--   0        0        0    13749 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
+-rw-r--r--   0        0        0     1134 2023-07-05 09:33:37.233976 covdrugsim-0.2.0/tests/test_covdrugsim.py
+-rw-r--r--   0        0        0     7780 1970-01-01 00:00:00.000000 covdrugsim-0.2.0/PKG-INFO
```

### Comparing `covdrugsim-0.1.0/LICENSE` & `covdrugsim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/mdsim/SCbondDist.py` & `covdrugsim-0.2.0/src/covdrugsim/mdsim/SCbondDist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
-from Honours.MD.config import MD_PATH, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT, SIX_PLOTS_HORIZONTAL_WIDTH, SIX_PLOTS_HORIZONTAL_HEIGHT, inhibitor_list
+from covdrugsim.mdsim.config import MD_PATH, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT, SIX_PLOTS_HORIZONTAL_WIDTH, SIX_PLOTS_HORIZONTAL_HEIGHT, inhibitor_list
 
 sns.set(context='paper', font_scale=1.5)
 CURR_DIR = os.getcwd()
 
 
 if __name__ == "__main__":
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/mdsim/baseID.py` & `covdrugsim-0.2.0/src/covdrugsim/mdsim/baseID.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
-from Honours.MD.config import MD_PATH, SINGLE_PLOT_WIDTH, SINGLE_PLOT_HEIGHT, SINGLE_PLOT_LEG_WIDTH, \
+from covdrugsim.mdsim.config import MD_PATH, SINGLE_PLOT_WIDTH, SINGLE_PLOT_HEIGHT, SINGLE_PLOT_LEG_WIDTH, \
     SINGLE_PLOT_LEG_HEIGHT, FOUR_PLOTS_WIDTH, FOUR_PLOTS_HEIGHT, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT
 
 sns.set(context='talk', font_scale=0.8)
 CURR_DIR = os.getcwd()
 
 
 if __name__ == "__main__":
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/mdsim/bbRMSD.py` & `covdrugsim-0.2.0/src/covdrugsim/mdsim/bbRMSD.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/mdsim/hbondAnalysis.py` & `covdrugsim-0.2.0/src/covdrugsim/mdsim/hbondAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
-from Honours.MD.config import MD_PATH, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT, inhibitor_list
+from covdrugsim.mdsim.config import MD_PATH, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT, inhibitor_list
 
 sns.set(context='paper', font_scale=1.5)
 CURR_DIR = os.getcwd()
 
 
 if __name__ == "__main__":
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/mdsim/ligDihedral.py` & `covdrugsim-0.2.0/src/covdrugsim/mdsim/ligDihedral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
-from Honours.MD.config import MD_PATH, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT, SIX_PLOTS_HORIZONTAL_WIDTH, SIX_PLOTS_HORIZONTAL_HEIGHT, inhibitor_list
+from covdrugsim.mdsim.config import MD_PATH, SIX_PLOTS_WIDTH, SIX_PLOTS_HEIGHT, SIX_PLOTS_HORIZONTAL_WIDTH, SIX_PLOTS_HORIZONTAL_HEIGHT, inhibitor_list
 
 sns.set(context='paper', font_scale=1.5)
 CURR_DIR = os.getcwd()
 
 
 if __name__ == "__main__":
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/mdsim/prepMTB.py` & `covdrugsim-0.2.0/src/covdrugsim/mdsim/prepMTB.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/admin.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/admin.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/gsub.sh` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/gsub.sh`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/prepGaussian.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/prepGaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from os.path import isdir
-from QM_Gaussian.settings import keyword_dict
+
+from covdrugsim.qmcalc.runGaussian.settings import keyword_dict
 
 
 def gen_from_dir(input_dir, WALLTIME, VMEM, MEM, JOBFS, CHARGE, SPIN, METHOD, BASIS_SET, SOLVENT, SOLVENT_MODEL, CLUSTER, CALC_TYPE, NCPUS, SOFTWARE, VERSION):
     """Generate Gaussian input job files and submission files for molecules in given directories"""
     assert CALC_TYPE in keyword_dict.keys(), 'Calculation type not known!'
     conformers = [g for g in os.listdir(input_dir) if isdir('{0}/{1}'.format(input_dir, g))]
     for j, title in enumerate(conformers):
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/settings.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/settings.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/runGaussian/tabulate.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/runGaussian/tabulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
-import pandas as pd
-import re
 from os.path import isdir
-from QM.runGaussian.settings import DATA_PATH
+import re
+
+import pandas as pd
 
 
-def sort_human(list):
+def sortHuman(list):
     """Sort a given list in a more "human" way"""
     convert = lambda text: float(text) if text.isdigit() else text
     alphanum = lambda key: [convert(c) for c in re.split('([-+]?[0-9]*\.?[0-9]*)', key)]
     list.sort(key=alphanum)
     return list
 
 
@@ -17,15 +17,15 @@
     """Replace multiple strings of main_str"""
     for elem in toBeReplaced:
         if elem in main_str:
             main_str = main_str.replace(elem, new_str)
     return main_str
 
 
-def find_val(line_list, target_str):
+def findVal(line_list, target_str):
     """Find the values of interest from Gaussian output files"""
     val, isEnergy, isMethod = None, 'Energies' in target_str[0] or 'Enthalpies' in target_str[0], '%chk' in target_str[0]
     for i, string in enumerate(target_str):
         for j, line in enumerate(line_list):
             if string in line:
                 if isMethod:
                     value_inc = line_list[j - 2]
@@ -60,26 +60,26 @@
         conformer_dir = '{0}/{1}'.format(input_dir, title)
         print("Conformer:", title)
         try:
             with open('{0}/{1}.out'.format(conformer_dir, title), 'r') as f:
                 line_list = f.readlines()
                 line_list.reverse()
                 for i, var_list in enumerate(var_fill_list):
-                    val = find_val(line_list, keyword_list[i])
+                    val = findVal(line_list, keyword_list[i])
                     var_list.append(val)
                 title_list.append(title)
                 molecule_list.append(replace_multiple(title.split('c')[0].replace('_', ''), ['TR', 'TSS', 'TP'], ''))
                 conformer_list.append('c' + title.split('c')[-1])
         except FileNotFoundError:
             print("{0}/{1}.out not found!".format(conformer_dir, title))
             continue
     data = {'Method': method_list, 'Title': title_list, 'Molecule': molecule_list, 'Conformer': conformer_list, 'NImag': NImag_list,
            'Z (Hartree)': Z_list, 'E (Hartree)': E_list, 'H (Hartree)': H_list, 'G (Hartree)': G_list}
     df = pd.DataFrame(data, columns=['Method', 'Title', 'Molecule', 'Conformer', 'NImag', 'Z (Hartree)', 'E (Hartree)', 'H (Hartree)', 'G (Hartree)'])
-    title_list = sort_human(title_list)
+    title_list = sortHuman(title_list)
     sorted_df = df.set_index('Title').reindex(title_list).reset_index()
     print("# Sorted data frame:\n", sorted_df)
 
     print("# Writing to Excel sheet...")
     # sorted_df.to_excel('{0}/Energies.xlsx'.format(input_dir), sheet_name='Sheet1')
     writer = pd.ExcelWriter('{0}/Energies.xlsx'.format(input_dir), engine='xlsxwriter')
     sorted_df.to_excel(writer, startrow=1, sheet_name='Sheet1', index=False)
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     if height == 0:
         print("ERROR: Image height not set! e.g.:\nheight = 500")
         sys.exit("Height not set")
     if width == 0:
         print("ERROR: Image width not set! e.g.:\nwidth = 500")
         sys.exit("Width not set")
     if outName == "":
-        print("ERROR: output file name not set! e.g.:\n output-file = example.pdf")
+        print("ERROR: output file name not set! e.g.:\n output-file = energyLevellerExample.pdf")
         sys.exit("Output name not set")
 
     outDiagram = Diagram(width, height, fontSize, outName)
     outDiagram.energyUnits = energyUnits
     for color in colorsToAdd:
         outDiagram.COLORS[color] = colorsToAdd[color]
     maxColumn = 0
@@ -290,17 +290,17 @@
 
 ######################################################################################################
 #          Example printing function. Skip to bottom.
 ######################################################################################################
 
 
 def MakeExampleFile():
-    output = open("example.inp", 'w')
+    output = open("energyLevellerExample.inp", 'w')
 
-    output.write("output-file     = example.pdf\nwidth           = 8\nheight          = 8\nenergy-units    = $\\Delta$E"
+    output.write("output-file     = energyLevellerExample.pdf\nwidth           = 8\nheight          = 8\nenergy-units    = $\\Delta$E"
                  "  kJ/mol\nfont size       = 10\n\n#   This is a comment. Lines that begin with a # are ignored.\n#   "
                  "Available colours are those accepted by matplotlib \n\n#   Now begins the states input\n\n#—————–  Pa"
                  "th 1 ————————————————\n\n#   Add the first path, all paths are relative to the reactant energies so\n"
                  "#   start at zero\n\n{\n    name        = reactants\n    text-colour = black\n    label       = CH$_3"
                  "$O$\\cdot$ + X\n    energy      = 0.0\n    labelColour = black\n    linksto     = pre-react1:red, tra"
                  "nsition2:#003399, pre-react3:#009933\n    column      = 1\n}\n\n{\n    name        = pre-react1\n    "
                  "text-colour = red\n    label       = CH$_3$O$\\cdot$ $\\ldots$ X\n    energy      = -10.5\n    labelC"
@@ -321,33 +321,33 @@
                  "     = transition3\n    text-colour = #009933\n    label       = [CH$_3$O$\\cdot$ $\\ldots$ X]$^{++}$"
                  "\n    energy      = +25.4\n    labelColour = #009933\n    linksto     = post-react3:#009933\n    colu"
                  "mn      = 3\n}\n\n{\n    name        = post-react3\n    text-colour = #009933\n    label       = $\\c"
                  "dot$CH$_2$OH $\\ldots$ X\n    energy      = -6.1\n    labelColour = #009933\n    linksto     = produc"
                  "ts:#009933\n    column      = 4\n    labelOffset = 0,1\n    textOffset  = 0,1.4\n}\n")
 
     output.close()
-    print("Made example file as 'example.inp'.")
+    print("Made example file as 'energyLevellerExample.inp'.")
 
 
 ######################################################################################################
 #           Main driver function
 ######################################################################################################
 
 
 def main(inp_path):
 
     print("o=======================================================o")
     print("         Beginning Energy Level Diagram")
     print("o=======================================================o")
-    #if len(sys.argv) == 1:
-    #   print("\nI need an input file!\n")
-    #    if not os.path.exists("example.inp"):
-    #        print("\nAn example file will be made.")
-    #        MakeExampleFile()
-    #    sys.exit("No Input file.")
+    if len(sys.argv) == 1:
+        print("\nI need an input file!\n")
+        if not os.path.exists("energyLevellerExample.inp"):
+            print("\nAn example file will be made.")
+            MakeExampleFile()
+        sys.exit("No Input file.")
     if len(sys.argv) > 2:
         print("Incorrect arguments. Correct call:\npython EnergyLeveler.py <INPUT FILE>")
         sys.exit("Incorrect Arguments.")
     elif len(sys.argv) == 2:
         diagram = ReadInput(sys.argv[1])
     else:
         diagram = ReadInput(inp_path)
@@ -358,8 +358,9 @@
 
     print("o=======================================================o")
     print("         Image "+diagram.outputName+" made!")
     print("o=======================================================o")
 
 
 if __name__ == "__main__":
-    main("C:/Users/s4425412/PycharmProjects/CovInhib/run_gaussian/a-santonin.inp")
+    main('')
+    #main("C:/Users/s4425412/PycharmProjects/CovInhib/run_gaussian/a-santonin.inp")
```

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.1.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py` & `covdrugsim-0.2.0/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import seaborn as sns
 import pandas as pd
 import numpy as np
 from matplotlib import pyplot as plt
-from QM.runGaussian.settings import DATA_PATH
-from QM.visAnalysis.plotConfig import combination_dict, charge_list, charge_list_A, charge_list_B, DI_list, \
+from covdrugsim.qmcalc.visAnalysis.plotConfig import combination_dict, charge_list, charge_list_A, charge_list_B, DI_list, \
     benchmarking_data, barrier_data
 
 sns.set(context='talk', font_scale=0.9)
 # sns.despine()  # Remove "chartjunk"
 
 SINGLE_PLOT_WIDTH, SINGLE_PLOT_HEIGHT = 6, 4
 TWO_PLOT_WIDTH, TWO_PLOT_HEIGHT = 9, 3.5
@@ -23,14 +22,15 @@
     plt.plot(x, y, '--r', label="$y = {0:.1f}x + {1:.1f}$\n$R^2 = {2:.2f}$".format(m, c, r2))
     plt.legend(loc=leg_loc, fontsize=font_size)
     plt.locator_params(axis='x', nbins=6)
 
 
 if __name__ == "__main__":
     analysis_type = "Regression"
+    DATA_PATH = '.'
     if analysis_type == "Bar":
 
         # Statistical Measures
         df = pd.DataFrame(benchmarking_data)
         fig = plt.figure(figsize=(BAR_PLOTS_WIDTH, BAR_PLOTS_HEIGHT))
         fig.subplots_adjust(top=0.95, bottom=0.15, left=0.1, right=0.98)
         data = df.groupby("Error (kcal/mol)").size()
```

### Comparing `covdrugsim-0.1.0/setup.py` & `covdrugsim-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,113 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# CovDrugSim
 
-package_dir = \
-{'': 'src'}
+[![ci-cd](https://github.com/Jon-Ting/covdrugsim/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/covdrugsim/actions/workflows/ci-cd.yml)
 
-packages = \
-['covdrugsim',
- 'covdrugsim.mdsim',
- 'covdrugsim.qmcalc.runGaussian',
- 'covdrugsim.qmcalc.unitConv',
- 'covdrugsim.qmcalc.visAnalysis']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['matplotlib>=3.7.1,<4.0.0',
- 'numpy>=1.25.0,<2.0.0',
- 'pandas>=2.0.2,<3.0.0',
- 'seaborn>=0.12.2,<0.13.0']
-
-setup_kwargs = {
-    'name': 'covdrugsim',
-    'version': '0.1.0',
-    'description': 'Quantum mechanical calculations and molecular dynamics simulations of covalent drugs',
-    'long_description': '# covdrugsim\n\nQuantum mechanical calculations and molecular dynamics simulations of covalent drugs.\n\nWritten by Jonathan Yik Chang Ting (Student ID: 44254124) for UQ BAdSc(Hons) Honours Project 2019.\nProject Title: Molecular Modelling of Reversible Covalent Inhibition of Bruton’s Tyrosine Kinase by Cyanoacrylamides\n\n## Installation\n\n```bash\n$ pip install covdrugsim\n```\n\n## Usage\n\n`covdrugsim` can be used to conduct quantum mechanical calculations and molecular dynamics simulations as follows:\n\n```python\nfrom covdrugsim.qmCalc import qmCalc\nfrom covdrugsim.mdSim import mdSim\nimport matplotlib.pyplot as plt\n\nfilePath = "test.txt"  # Path to your file\nqmCalc(filePath)\nmdSim(filePath)\nplt.show()\n```\n\n\nDescriptions of source codes:\n### Quantum Mechanical Calculations (qmcalc)\n\n#### unitConv\nunitConv.py - Interconverts between kinetics and thermodynamic quantities (dGbarr, k, t_half, RT).\n\n#### runGaussian\nsettings.py - Contains variables for different type of Gaussian jobs that are used by prepGaussian.py.\nadmin.py - Group files with the same names (before extension, e.g. abc.inp is the same as abc.xyz) into individual directories.\nprepGaussian.py - Batch generation of Gaussian input files and job submission files on HPCs with PBS Scheduler.\ntabulate.py - Batch tabulation of interested values from Gaussian (version 16) output files into an Excel file.\ngsub.sh - Batch submission of Gaussian QM calculation jobs on HPCs.\n\nTypical work flow for a mechanism-based project where flexible molecules are involved would be:\n1) Conduct conformational searches on the species along the reaction coordinate (using MacroModel).\n2) Export all conformers within 3 kcal/mol of the lowest energy structure to a directory in .xyz format. The naming convention is very important, be consistent, but make sure each conformer has a different name (I do this by adding numbers at the end of their names, signifying their ranks from the conformational searches).\n3) Change your input directory in admin.py to where you store the coordinate files and run it. This will group all of the conformers into individual directories.\n4) Change your input directory in prepGaussian.py to the same location and run it. This will generate the Gaussian input files and job submission files in the corresponding directory. Make sure you check at least a few of the files generated to see that you got the charges, spacing at the end of file, solvents, resources requested, etc right. I named all of the Gaussian job submission jobs with *.sh, feel free to change it according to your preference (Line 52 in prepGaussian.py).\n5) Copy the directories across to the HPCs (Raijin/Gadi/Tinaroo/Awoonga, NOTE: The details for job submissions on Raijin and RCC HPCs are different, specify the cluster before running prepGaussian.py in Step 4).\n6) Change directory to the directory that contains all the conformers subdirectories and run \'gsub.sh\' (Make sure it\'s an executable, if you can\'t run it, use chmod to change it). This will submit all of the Gaussian submission jobs to the HPC. Note that prior to this you need to adjust Line 6 in the gsub.sh file to the naming convention you give to your Gaussian submit files if you have changed them in the prepGaussian.py.\n7) After the jobs are done, copy them over to your local machine.\n8) Change your input directory in tabulate.py to the directory that contains all the conformers and run it. Note that you need to have the Python package pandas installed for it to work.\n\n#### visAnalysis\nenergyLeveller.py - Draws energy profile diagrams.\nplotConfig.py - Stores configuration for figure-plotting functions.\nplotFigs.py - Plots figures for QM data analysis.\n\n\n### Molecular Dynamics Simulations (mdsim)\n- config.py contains some variables that are used repetitively for almost all files.\n- baseID.py plots the distances between potential base species and the targeted protons.\n- bbRMSD.py plots the RMSD of BTK backbones over time, for the purpose of checking the stability of the simulations.\n- hbondAnalysis.py plots the distribution of the number of hydrogen bonds between BTK backbones over time.\n- ligDihedral.py plots the distribution of the critical C=C-C=O dihedral angle near BTK active site over time.\n- SCbondDist.py plots the distances between the reacting S and C atoms over time.\n- sumCharge.py sums up the charges to aid in the parameterisation of non-standard amino acids.\n- prepMTB.py was written during an attempt to map the unbound ligand to covalently bound ligand. Was not utilised in the end.\n\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`covdrugsim` was created by Jonathan Yik Chang Ting. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`covdrugsim` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
-    'author': 'Jonathan Yik Chang Ting',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+## Description
 
+`CovDrugSim` is a package that provides functionalities to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
+
+## Features
+
+### Aims
+* Automatic creation of HPC submission files to run Gaussian calculations.
+* Automatic analysis of molecular dynamics simulation trajectories.
+
+### Under Development
+* Restructure the source code.
+* Complete unit tests in tests/.
+* Add function docstrings.
+* Complete example.ipynb.
+
+## Installation
+
+Use `pip` or `conda` to install `CovDrugSim`:
+
+```bash
+$ pip install covdrugsim
+```
+```bash
+$ conda install -c conda-forge covdrugsim
+```
+
+## Usage
+
+`covdrugsim` can be used to conduct quantum mechanical calculations and molecular dynamics simulations as follows:
+
+```python
+from covdrugsim.qmCalc import qmCalc
+from covdrugsim.mdSim import mdSim
+import matplotlib.pyplot as plt
+
+filePath = "test.txt"  # Path to your file
+qmCalc(filePath)
+mdSim(filePath)
+plt.show()
+```
+Check out the [notebook tutorial](https://github.com/Jon-Ting/covdrugsim/blob/main/docs/example.ipynb) for further explanations and demonstrations!
+
+Descriptions of source codes:
+### Quantum Mechanical Calculations (qmcalc)
+
+#### unitConv
+unitConv.py - Interconverts between kinetics and thermodynamic quantities (dGbarr, k, t_half, RT).
+
+#### runGaussian
+* settings.py - Contains variables for different type of Gaussian jobs that are used by prepGaussian.py.
+* admin.py - Group files with the same names (before extension, e.g. abc.inp is the same as abc.xyz) into individual directories.
+* prepGaussian.py - Batch generation of Gaussian input files and job submission files on HPCs with PBS Scheduler.
+* tabulate.py - Batch tabulation of interested values from Gaussian (version 16) output files into an Excel file.
+* gsub.sh - Batch submission of Gaussian QM calculation jobs on HPCs.
+
+Typical workflow for a mechanism-based project where flexible molecules are involved would be:
+1) Conduct conformational searches on the species along the reaction coordinate (using MacroModel).
+2) Export all conformers within 3 kcal/mol of the lowest energy structure to a directory in .xyz format. The naming convention is very important, be consistent, but make sure each conformer has a different name (I do this by adding numbers at the end of their names, signifying their ranks from the conformational searches).
+3) Change your input directory in admin.py to where you store the coordinate files and run it. This will group all of the conformers into individual directories.
+4) Change your input directory in prepGaussian.py to the same location and run it. This will generate the Gaussian input files and job submission files in the corresponding directory. Make sure you check at least a few of the files generated to see that you got the charges, spacing at the end of file, solvents, resources requested, etc right. I named all of the Gaussian job submission jobs with \*.sh, feel free to change it according to your preference (Line 52 in prepGaussian.py).
+5) Copy the directories across to the HPCs (Raijin/Gadi/Tinaroo/Awoonga, NOTE: The details for job submissions on Raijin and RCC HPCs are different, specify the cluster before running prepGaussian.py in Step 4).
+6) Change directory to the directory that contains all the conformers subdirectories and run 'gsub.sh' (Make sure it's an executable, if you can't run it, use chmod to change it). This will submit all of the Gaussian submission jobs to the HPC. Note that prior to this you need to adjust Line 6 in the gsub.sh file to the naming convention you give to your Gaussian submit files if you have changed them in the prepGaussian.py.
+7) After the jobs are done, copy them over to your local machine.
+8) Change your input directory in tabulate.py to the directory that contains all the conformers and run it. Note that you need to have the Python package pandas installed for it to work.
+
+#### visAnalysis
+energyLeveller.py - Draws energy profile diagrams.
+plotConfig.py - Stores configuration for figure-plotting functions.
+plotFigs.py - Plots figures for QM data analysis.
+
+
+### Molecular Dynamics Simulations (mdsim)
+- config.py contains some variables that are used repetitively for almost all files.
+- baseID.py plots the distances between potential base species and the targeted protons.
+- bbRMSD.py plots the RMSD of BTK backbones over time, for the purpose of checking the stability of the simulations.
+- hbondAnalysis.py plots the distribution of the number of hydrogen bonds between BTK backbones over time.
+- ligDihedral.py plots the distribution of the critical C=C-C=O dihedral angle near BTK active site over time.
+- SCbondDist.py plots the distances between the reacting S and C atoms over time.
+- sumCharge.py sums up the charges to aid in the parameterisation of non-standard amino acids.
+- prepMTB.py was written during an attempt to map the unbound ligand to covalently bound ligand. Was not utilised in the end.
+
+## Documentation
+
+Detailed documentation and usage examples are hosted by [Read the Docs](https://covdrugsim.readthedocs.io/en/latest/).
+
+## Contributing
+
+`CovDrugSim` appreciates your enthusiasm and welcomes your expertise! 
+
+Please check out the [contributing guidelines](https://github.com/Jon-Ting/covdrugsim/blob/main/CONTRIBUTING.md) and 
+[code of conduct](https://github.com/Jon-Ting/covdrugsim/blob/main/CONDUCT.md). 
+By contributing to this project, you agree to abide by its terms.
+
+## License
+
+The project is distributed under an [MIT License](https://github.com/Jon-Ting/covdrugsim/blob/main/LICENSE).
+
+## Credits
+
+The package was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) using the 
+The codes were written by [Jonathan Yik Chang Ting](https://github.com/Jon-Ting) for [University of Queensland Bachelors of Advanced Science (Honours)](https://study.uq.edu.au/study-options/programs/bachelor-advanced-science-honours-2516) [CHEM6511](https://my.uq.edu.au/programs-courses/course.html?course_code=CHEM6511) under the title "[Molecular Modelling of Reversible Covalent Inhibition of Bruton’s Tyrosine Kinase by Cyanoacrylamides](https://github.com/Jon-Ting/Molecular-Modelling-of-Reversible-Covalent-Inhibition-of-Brutons-Tyrosine-Kinase-by-Cyanoacrylamide)". Click on the title to see the details of the project.
+
+## Contact
+
+Email: `Jonathan.Ting@anu.edu.au`/`jonting97@gmail.com`
+
+Feel free to reach out if you have any questions, suggestions, or feedback.
 
-setup(**setup_kwargs)
```

### Comparing `covdrugsim-0.1.0/PKG-INFO` & `covdrugsim-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 Metadata-Version: 2.1
 Name: covdrugsim
-Version: 0.1.0
-Summary: Quantum mechanical calculations and molecular dynamics simulations of covalent drugs
+Version: 0.2.0
+Summary: Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
+Home-page: https://github.com/Jon-Ting/covdrugsim
 License: MIT
+Keywords: covalent,drug,quantum,mechanic,molecular,dynamics,simulation
 Author: Jonathan Yik Chang Ting
-Requires-Python: >=3.9,<4.0
+Author-email: jonting97@gmail.com
+Requires-Python: >=3.9
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.25.0,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: matplotlib (>=3.7.1)
+Requires-Dist: numpy (>=1.25.0)
+Requires-Dist: pandas (>=2.0.2)
+Requires-Dist: seaborn (>=0.12.2)
+Project-URL: Documentation, https://covdrugsim.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/Jon-Ting/covdrugsim
 Description-Content-Type: text/markdown
 
-# covdrugsim
+# CovDrugSim
+
+[![ci-cd](https://github.com/Jon-Ting/covdrugsim/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/covdrugsim/actions/workflows/ci-cd.yml)
+
+## Description
 
-Quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
+`CovDrugSim` is a package that provides functionalities to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
 
-Written by Jonathan Yik Chang Ting (Student ID: 44254124) for UQ BAdSc(Hons) Honours Project 2019.
-Project Title: Molecular Modelling of Reversible Covalent Inhibition of Bruton’s Tyrosine Kinase by Cyanoacrylamides
+## Features
+
+### Aims
+* Automatic creation of HPC submission files to run Gaussian calculations.
+* Automatic analysis of molecular dynamics simulation trajectories.
+
+### Under Development
+* Restructure the source code.
+* Complete unit tests in tests/.
+* Add function docstrings.
+* Complete example.ipynb.
 
 ## Installation
 
+Use `pip` or `conda` to install `CovDrugSim`:
+
 ```bash
 $ pip install covdrugsim
 ```
+```bash
+$ conda install -c conda-forge covdrugsim
+```
 
 ## Usage
 
 `covdrugsim` can be used to conduct quantum mechanical calculations and molecular dynamics simulations as follows:
 
 ```python
 from covdrugsim.qmCalc import qmCalc
@@ -38,34 +66,34 @@
 import matplotlib.pyplot as plt
 
 filePath = "test.txt"  # Path to your file
 qmCalc(filePath)
 mdSim(filePath)
 plt.show()
 ```
-
+Check out the [notebook tutorial](https://github.com/Jon-Ting/covdrugsim/blob/main/docs/example.ipynb) for further explanations and demonstrations!
 
 Descriptions of source codes:
 ### Quantum Mechanical Calculations (qmcalc)
 
 #### unitConv
 unitConv.py - Interconverts between kinetics and thermodynamic quantities (dGbarr, k, t_half, RT).
 
 #### runGaussian
-settings.py - Contains variables for different type of Gaussian jobs that are used by prepGaussian.py.
-admin.py - Group files with the same names (before extension, e.g. abc.inp is the same as abc.xyz) into individual directories.
-prepGaussian.py - Batch generation of Gaussian input files and job submission files on HPCs with PBS Scheduler.
-tabulate.py - Batch tabulation of interested values from Gaussian (version 16) output files into an Excel file.
-gsub.sh - Batch submission of Gaussian QM calculation jobs on HPCs.
+* settings.py - Contains variables for different type of Gaussian jobs that are used by prepGaussian.py.
+* admin.py - Group files with the same names (before extension, e.g. abc.inp is the same as abc.xyz) into individual directories.
+* prepGaussian.py - Batch generation of Gaussian input files and job submission files on HPCs with PBS Scheduler.
+* tabulate.py - Batch tabulation of interested values from Gaussian (version 16) output files into an Excel file.
+* gsub.sh - Batch submission of Gaussian QM calculation jobs on HPCs.
 
-Typical work flow for a mechanism-based project where flexible molecules are involved would be:
+Typical workflow for a mechanism-based project where flexible molecules are involved would be:
 1) Conduct conformational searches on the species along the reaction coordinate (using MacroModel).
 2) Export all conformers within 3 kcal/mol of the lowest energy structure to a directory in .xyz format. The naming convention is very important, be consistent, but make sure each conformer has a different name (I do this by adding numbers at the end of their names, signifying their ranks from the conformational searches).
 3) Change your input directory in admin.py to where you store the coordinate files and run it. This will group all of the conformers into individual directories.
-4) Change your input directory in prepGaussian.py to the same location and run it. This will generate the Gaussian input files and job submission files in the corresponding directory. Make sure you check at least a few of the files generated to see that you got the charges, spacing at the end of file, solvents, resources requested, etc right. I named all of the Gaussian job submission jobs with *.sh, feel free to change it according to your preference (Line 52 in prepGaussian.py).
+4) Change your input directory in prepGaussian.py to the same location and run it. This will generate the Gaussian input files and job submission files in the corresponding directory. Make sure you check at least a few of the files generated to see that you got the charges, spacing at the end of file, solvents, resources requested, etc right. I named all of the Gaussian job submission jobs with \*.sh, feel free to change it according to your preference (Line 52 in prepGaussian.py).
 5) Copy the directories across to the HPCs (Raijin/Gadi/Tinaroo/Awoonga, NOTE: The details for job submissions on Raijin and RCC HPCs are different, specify the cluster before running prepGaussian.py in Step 4).
 6) Change directory to the directory that contains all the conformers subdirectories and run 'gsub.sh' (Make sure it's an executable, if you can't run it, use chmod to change it). This will submit all of the Gaussian submission jobs to the HPC. Note that prior to this you need to adjust Line 6 in the gsub.sh file to the naming convention you give to your Gaussian submit files if you have changed them in the prepGaussian.py.
 7) After the jobs are done, copy them over to your local machine.
 8) Change your input directory in tabulate.py to the directory that contains all the conformers and run it. Note that you need to have the Python package pandas installed for it to work.
 
 #### visAnalysis
 energyLeveller.py - Draws energy profile diagrams.
@@ -79,20 +107,35 @@
 - bbRMSD.py plots the RMSD of BTK backbones over time, for the purpose of checking the stability of the simulations.
 - hbondAnalysis.py plots the distribution of the number of hydrogen bonds between BTK backbones over time.
 - ligDihedral.py plots the distribution of the critical C=C-C=O dihedral angle near BTK active site over time.
 - SCbondDist.py plots the distances between the reacting S and C atoms over time.
 - sumCharge.py sums up the charges to aid in the parameterisation of non-standard amino acids.
 - prepMTB.py was written during an attempt to map the unbound ligand to covalently bound ligand. Was not utilised in the end.
 
+## Documentation
+
+Detailed documentation and usage examples are hosted by [Read the Docs](https://covdrugsim.readthedocs.io/en/latest/).
 
 ## Contributing
 
-Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
+`CovDrugSim` appreciates your enthusiasm and welcomes your expertise! 
+
+Please check out the [contributing guidelines](https://github.com/Jon-Ting/covdrugsim/blob/main/CONTRIBUTING.md) and 
+[code of conduct](https://github.com/Jon-Ting/covdrugsim/blob/main/CONDUCT.md). 
+By contributing to this project, you agree to abide by its terms.
 
 ## License
 
-`covdrugsim` was created by Jonathan Yik Chang Ting. It is licensed under the terms of the MIT license.
+The project is distributed under an [MIT License](https://github.com/Jon-Ting/covdrugsim/blob/main/LICENSE).
 
 ## Credits
 
-`covdrugsim` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
+The package was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) using the 
+The codes were written by [Jonathan Yik Chang Ting](https://github.com/Jon-Ting) for [University of Queensland Bachelors of Advanced Science (Honours)](https://study.uq.edu.au/study-options/programs/bachelor-advanced-science-honours-2516) [CHEM6511](https://my.uq.edu.au/programs-courses/course.html?course_code=CHEM6511) under the title "[Molecular Modelling of Reversible Covalent Inhibition of Bruton’s Tyrosine Kinase by Cyanoacrylamides](https://github.com/Jon-Ting/Molecular-Modelling-of-Reversible-Covalent-Inhibition-of-Brutons-Tyrosine-Kinase-by-Cyanoacrylamide)". Click on the title to see the details of the project.
+
+## Contact
+
+Email: `Jonathan.Ting@anu.edu.au`/`jonting97@gmail.com`
+
+Feel free to reach out if you have any questions, suggestions, or feedback.
+
```

