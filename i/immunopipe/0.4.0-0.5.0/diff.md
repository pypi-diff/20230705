# Comparing `tmp/immunopipe-0.4.0.tar.gz` & `tmp/immunopipe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immunopipe-0.4.0.tar", max compression
+gzip compressed data, was "immunopipe-0.5.0.tar", max compression
```

## Comparing `immunopipe-0.4.0.tar` & `immunopipe-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0    35128 2022-12-12 04:29:27.873320 immunopipe-0.4.0/LICENSE
--rw-r--r--   0        0        0     3185 2022-12-12 04:29:27.873320 immunopipe-0.4.0/README.md
--rw-r--r--   0        0        0       33 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/__init__.py
--rw-r--r--   0        0        0      109 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/__main__.py
--rw-r--r--   0        0        0     1100 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/args.py
--rw-r--r--   0        0        0     2601 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/inhouse.py
--rw-r--r--   0        0        0      520 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/pipeline.py
--rw-r--r--   0        0        0     4651 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/processes.py
--rw-r--r--   0        0        0     1598 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/reports/CloneHeterogeneity.svelte
--rw-r--r--   0        0        0      680 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/reports/MarkersOverlapping.svelte
--rw-r--r--   0        0        0      676 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/reports/MetaMarkersForClones.svelte
--rw-r--r--   0        0        0      178 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/reports/RadarPlots.svelte
--rw-r--r--   0        0        0      211 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/reports/SampleInfo.svelte
--rw-r--r--   0        0        0      268 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/reports/SelectTCells.svelte
--rw-r--r--   0        0        0     4769 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/scripts/CloneHeterogeneity.R
--rw-r--r--   0        0        0     2029 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/scripts/MarkersOverlapping.R
--rw-r--r--   0        0        0     3262 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/scripts/MetaMarkersForClones.R
--rw-r--r--   0        0        0     2314 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/scripts/RadarPlots.R
--rw-r--r--   0        0        0     2112 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/scripts/SelectTCells.R
--rw-r--r--   0        0        0      170 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/utils.py
--rw-r--r--   0        0        0       22 2022-12-12 04:29:27.873320 immunopipe-0.4.0/immunopipe/version.py
--rw-r--r--   0        0        0      890 2022-12-12 04:29:27.877320 immunopipe-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 immunopipe-0.4.0/setup.py
--rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 immunopipe-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2023-07-05 16:52:10.608739 immunopipe-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3185 2023-07-05 16:52:10.608739 immunopipe-0.5.0/README.md
+-rw-r--r--   0        0        0      143 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/__main__.py
+-rw-r--r--   0        0        0     4551 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/inhouse.py
+-rw-r--r--   0        0        0      432 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/pipeline.py
+-rw-r--r--   0        0        0     7596 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/processes.py
+-rw-r--r--   0        0        0     1581 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/CloneHeterogeneity.svelte
+-rw-r--r--   0        0        0      683 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/MarkersOverlapping.svelte
+-rw-r--r--   0        0        0      679 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/MetaMarkersForClones.svelte
+-rw-r--r--   0        0        0      181 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/RadarPlots.svelte
+-rw-r--r--   0        0        0      214 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/SampleInfo.svelte
+-rw-r--r--   0        0        0     1012 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/reports/SelectTCells.svelte
+-rw-r--r--   0        0        0     4769 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/CloneHeterogeneity.R
+-rw-r--r--   0        0        0     2029 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/MarkersOverlapping.R
+-rw-r--r--   0        0        0     3289 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/MetaMarkersForClones.R
+-rw-r--r--   0        0        0     3699 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/RadarPlots.R
+-rw-r--r--   0        0        0     4029 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/scripts/SelectTCells.R
+-rw-r--r--   0        0        0       22 2023-07-05 16:52:10.612739 immunopipe-0.5.0/immunopipe/version.py
+-rw-r--r--   0        0        0      855 2023-07-05 16:52:10.612739 immunopipe-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 immunopipe-0.5.0/setup.py
+-rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 immunopipe-0.5.0/PKG-INFO
```

### Comparing `immunopipe-0.4.0/LICENSE` & `immunopipe-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `immunopipe-0.4.0/README.md` & `immunopipe-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `immunopipe-0.4.0/immunopipe/reports/CloneHeterogeneity.svelte` & `immunopipe-0.5.0/immunopipe/reports/CloneHeterogeneity.svelte`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <script>
-    import { Image, DataTable } from "@@";
-    import { Tabs, Tab, TabContent, Tile } from "carbon-components-svelte";
+    import { Image, DataTable } from "$libs";
+    import { Tabs, Tab, TabContent, Tile } from "$ccs";
 </script>
 
 {% for cdir in job.out.outdir | joinpaths: "*" | glob %}
 <h1>{{cdir | basename}}</h1>
 
 <h2>Chi-square test summary table</h2>
```

### Comparing `immunopipe-0.4.0/immunopipe/reports/MarkersOverlapping.svelte` & `immunopipe-0.5.0/immunopipe/reports/MarkersOverlapping.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% from "utils/misc.liq" import report_jobs -%}
 
 <script>
-    import { Image, DataTable } from "@@";
+    import { Image, DataTable } from "$libs";
 </script>
 
 
 {%- macro report_job(job, h=1) -%}
 
 {% for casedir in job.out.outdir | glob: "*" %}
 <h{{h}}>{{casedir | stem}}</h{{h}}>
```

### Comparing `immunopipe-0.4.0/immunopipe/reports/MetaMarkersForClones.svelte` & `immunopipe-0.5.0/immunopipe/reports/MetaMarkersForClones.svelte`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% from "utils/misc.liq" import report_jobs, table_of_images -%}
 
 <script>
-    import { Image, DataTable } from "@@";
+    import { Image, DataTable } from "$libs";
 </script>
 
 
 {%- macro report_job(job, h=1) -%}
 
 {% for casedir in job.out.outdir | glob: "*" %}
 <h{{h}}>{{casedir | joinpaths: "case.txt" | read | escape}}</h{{h}}>
```

### Comparing `immunopipe-0.4.0/immunopipe/scripts/CloneHeterogeneity.R` & `immunopipe-0.5.0/immunopipe/scripts/CloneHeterogeneity.R`

 * *Files identical despite different names*

### Comparing `immunopipe-0.4.0/immunopipe/scripts/MarkersOverlapping.R` & `immunopipe-0.5.0/immunopipe/scripts/MarkersOverlapping.R`

 * *Files identical despite different names*

### Comparing `immunopipe-0.4.0/immunopipe/scripts/MetaMarkersForClones.R` & `immunopipe-0.5.0/immunopipe/scripts/MetaMarkersForClones.R`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 library(tibble)
 library(parallel)
 library(Seurat)
 library(ggprism)
 library(tidyseurat)
 
 srtfile = {{in.srtobj | r}}
-cases = {{envs.cases | r}}
+cases = {{envs.cases | r: todot="-", sortkeys=False}}
 outdir = {{out.outdir | r}}
 ncores = {{envs.ncores | r}}
 
 
 print("- Reading seurat object ...")
 srtobj = readRDS(srtfile)
```

### Comparing `immunopipe-0.4.0/pyproject.toml` & `immunopipe-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "immunopipe"
 description = "A pipeline for integrative analysis for scTCR- and scRNA-seq data"
 authors = [ "pwwang <pwwang@pwwang.com>",]
-version = "0.4.0"
+version = "0.5.0"
 license = "GNU General Public License v3.0"
 readme = "README.md"
 homepage = "https://github.com/pwwang/immunopipe"
 repository = "https://github.com/pwwang/immunopipe"
 
+[tool.poetry.build]
+generate-setup-file = true
+
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen-args = "^0.3"
-pipen-report = "^0.4"
-pipen-filters = "^0.1"
-biopipen = "^0.6"
-datar = {version = "^0.10.3", extras = ["pandas"]}
-pipen-verbose = "^0.1"
+python = "^3.8"
+# pipen-report and pipen-board are required by biopipen
+biopipen = "^0.15"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 immunopipe = "immunopipe.pipeline:main"
 
 [tool.poetry.group.dev.dependencies]
 # pipen-dry = "^0.1.0"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
```

### Comparing `immunopipe-0.4.0/setup.py` & `immunopipe-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,31 @@
 packages = \
 ['immunopipe']
 
 package_data = \
 {'': ['*'], 'immunopipe': ['reports/*', 'scripts/*']}
 
 install_requires = \
-['biopipen>=0.6,<0.7',
- 'datar[pandas]>=0.10.3,<0.11.0',
- 'pipen-args>=0.3,<0.4',
- 'pipen-filters>=0.1,<0.2',
- 'pipen-report>=0.4,<0.5',
- 'pipen-verbose>=0.1,<0.2']
+['biopipen>=0.15,<0.16']
 
 entry_points = \
 {'console_scripts': ['immunopipe = immunopipe.pipeline:main']}
 
 setup_kwargs = {
     'name': 'immunopipe',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'A pipeline for integrative analysis for scTCR- and scRNA-seq data',
     'long_description': '# immunopipe\n\nIntegrative analysis for scTCR- and scRNA-seq data\n\n## Requirements & Installation\n\n- `python`: `3.7+`\n    - Other python depedencies should be installed via `pip install -U immunopipe`\n\n- `R`\n    - A bunch of R packages\n\n- Other\n  - VDJtools: https://vdjtools-doc.readthedocs.io/en/master/install.html\n\n- Checking requirements\n\n  ```shell\n  pip install -U pipen-cli-require\n  pipen require immunopipe.pipeline:pipeline <pipeline arguments>\n  ```\n\n- Quick way to install the dependencies using conda\n  ```shell\n  conda env install --name <env_name> --file docker/environment.yml\n  # then\n  conda activate <env_name>\n  ```\n\n## Running as a container\n\n### Using docker:\n\n```bash\ndocker run \\\n    -w /immunopipe/workdir \\\n    -v $(pwd)/:/immunopipe/workdir \\\n    -v /tmp \\\n    -v $(pwd)/prepared-data:/mnt \\\n    justold/immunopipe:<tag>  # or :dev to use the development version\n```\n\n### Using singularity:\n\n```bash\nsingularity run -w \\  # need it to be writable\n  --pwd /immunopipe/workdir -B .:/immunopipe/workdir \\  # Could use other directory instead of "."\n  # --contain: don\'t map host filesystem\n  # --cleanenv: recommended, to avoid other host\'s environment variables to be used\n  #   For example, $CONDA_PREFIX to affect host\'s conda environment\n  --contain --cleanenv \\\n  docker://justold/immunopipe:<tag>  # or :dev to use the development version\n\n# The mount your data directory to /mnt, which will make startup faster\n# For example\n#   -B .:/immunopipe/workdir,/path/to/data:/mnt\n# Where /path/to/data is the data directory containing the data files\n# You may also want to bind other directories (i.e. /tmp)\n#   -B <other bindings>,/tmp\n\n# Or you can pull the image first by:\nsingularity pull --force --dir images/ docker://justold/immunopipe:<tag>\n# Then you can replace "docker://justold/immunopipe:<tag>" with "images/immunopipe.sif"\n```\n\n## Modules\n\n![immunopipe](./immunopipe.png)\n\n- Basic TCR data analysis using `immunarch`\n- Clone Residency analysis if you have paired samples (i.e. Tumor vs Normal)\n- V-J usage, the frequency of various V-J junctions in circos-style plots\n- Clustering cells and configurale arguments to separate T and non-T cells\n- Clustering T cell, markers for each cluster and enrichment analysis for the markers\n- Radar plots to show the composition of cells for clusters\n- (Meta-)Markers finder for selected groups/clones of cells\n- Psedo-bulk GSEA analysis of two groups of cells\n- Seurat cluster statistics, including:\n  - Basic statistics of the clusters (e.g. number of cells in each cluster)\n  - Gene expressions (e.g. ridge, violin, feature, dot and heatmap plots)\n  - Dimensional reduction plots\n- TCR clustering using CDR3 sequences and the statistics of the clusters\n- Cell group distribution (TCR clones/clusters) in Seurat clusters\n- Clone heterogeneity (TCR clone distribution) in Seurat clusters\n- Metabolic landscape analysis (Ref: Xiao, Zhengtao, Ziwei Dai, and Jason W. Locasale. "Metabolic landscape of the tumor microenvironment at single cell resolution." Nature communications 10.1 (2019): 1-12.)\n\n## Documentaion\n\nhttps://pwwang.github.io/immunopipe\n\n## Example\n\nhttps://github.com/pwwang/immunopipe-example\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/immunopipe',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `immunopipe-0.4.0/PKG-INFO` & `immunopipe-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: immunopipe
-Version: 0.4.0
+Version: 0.5.0
 Summary: A pipeline for integrative analysis for scTCR- and scRNA-seq data
 Home-page: https://github.com/pwwang/immunopipe
 License: GNU General Public License v3.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: biopipen (>=0.6,<0.7)
-Requires-Dist: datar[pandas] (>=0.10.3,<0.11.0)
-Requires-Dist: pipen-args (>=0.3,<0.4)
-Requires-Dist: pipen-filters (>=0.1,<0.2)
-Requires-Dist: pipen-report (>=0.4,<0.5)
-Requires-Dist: pipen-verbose (>=0.1,<0.2)
+Requires-Dist: biopipen (>=0.15,<0.16)
 Project-URL: Repository, https://github.com/pwwang/immunopipe
 Description-Content-Type: text/markdown
 
 # immunopipe
 
 Integrative analysis for scTCR- and scRNA-seq data
```

