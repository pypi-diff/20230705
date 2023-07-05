# Comparing `tmp/checkatlas-0.2.2.tar.gz` & `tmp/checkatlas-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.2.2.tar", max compression
+gzip compressed data, was "checkatlas-0.2.3.tar", max compression
```

## Comparing `checkatlas-0.2.2.tar` & `checkatlas-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1211 2023-03-23 17:01:13.699003 checkatlas-0.2.2/LICENSE
--rw-r--r--   0        0        0     3841 2023-03-23 17:01:13.699003 checkatlas-0.2.2/README.md
--rw-r--r--   0        0        0      130 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/__init__.py
--rw-r--r--   0        0        0     7774 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/__main__.py
--rw-r--r--   0        0        0    20197 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/atlas.py
--rw-r--r--   0        0        0    17277 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/atlas_seurat.py
--rw-r--r--   0        0        0    13711 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/checkatlas.py
--rw-r--r--   0        0        0      929 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/checkatlas_workflow.nf
--rw-r--r--   0        0        0    10123 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0     1127 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/convertSeurat.R
--rw-r--r--   0        0        0     1271 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/folders.py
--rw-r--r--   0        0        0        0 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4103 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0      410 2023-03-23 17:01:13.699003 checkatlas-0.2.2/checkatlas/multiqc.py
--rw-r--r--   0        0        0     1458 2023-03-23 17:01:13.887005 checkatlas-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 checkatlas-0.2.2/setup.py
--rw-r--r--   0        0        0     4868 1970-01-01 00:00:00.000000 checkatlas-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-05 14:37:24.916213 checkatlas-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3841 2023-07-05 14:37:24.916213 checkatlas-0.2.3/README.md
+-rw-r--r--   0        0        0      130 2023-07-05 14:37:24.916213 checkatlas-0.2.3/checkatlas/__init__.py
+-rw-r--r--   0        0        0     8445 2023-07-05 14:37:24.916213 checkatlas-0.2.3/checkatlas/__main__.py
+-rw-r--r--   0        0        0    20197 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/atlas.py
+-rw-r--r--   0        0        0    17277 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/atlas_seurat.py
+-rw-r--r--   0        0        0    12728 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0      931 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/checkatlas_workflow.nf
+-rw-r--r--   0        0        0    10123 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0     1127 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/convertSeurat.R
+-rw-r--r--   0        0        0     1905 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/folders.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4103 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0      721 2023-07-05 14:37:24.920213 checkatlas-0.2.3/checkatlas/multiqc.py
+-rw-r--r--   0        0        0     1436 2023-07-05 14:37:25.108215 checkatlas-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 checkatlas-0.2.3/setup.py
+-rw-r--r--   0        0        0     4824 1970-01-01 00:00:00.000000 checkatlas-0.2.3/PKG-INFO
```

### Comparing `checkatlas-0.2.2/LICENSE` & `checkatlas-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/README.md` & `checkatlas-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/__main__.py` & `checkatlas-0.2.3/checkatlas/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     `python -m checkatlas` and `$ checkatlas `.
 
     This is checkatlas entry point.
 
     Arguments are managed here
     Search fo atlases is managed here
     Then checkatlas is ran with the list of atlases found
+
+    Returns:
+        None
+
     """
     # Set up logging
     logger = logging.getLogger("checkatlas")
     logging.basicConfig(format="|--- %(levelname)-8s %(message)s")
 
     parser = argparse.ArgumentParser(
         prog="checkatlas",
@@ -67,21 +71,21 @@
         action="store_true",
         help="Set this argument, if you added "
         "atlas files since the last run of "
         "checkatlas and you want to check "
         "only the new files.",
     )
 
-    parser.add_argument(
+    """     parser.add_argument(
         "--nextflow",
         type=int,
         default=0,
         help="Activate Nextflow and specify the number of threads to use. \n"
         "Example: --nextflow 8 (for 8 threads)",
-    )
+    ) """
 
     parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
         help="Print out all debug messages.",
     )
@@ -153,42 +157,63 @@
         "use in the clustering metric calculus."
         "Example: --obs_cluster celltype leuven seurat_clusters",
     )
     metric_options.add_argument(
         "--metric_cluster",
         nargs="+",
         type=str,
-        default=["silhouette", "davies_bouldin"],
+        # default=["silhouette", "davies_bouldin"],
+        default=["davies_bouldin"],
         help="Specify the list of clustering metrics to calculate.\n"
         "   Example: --metric_cluster silhouette davies_bouldin\n"
         f"   List of cluster metrics: {cluster.__all__}",
     )
     metric_options.add_argument(
         "--metric_annot",
         nargs="+",
         type=str,
-        default=["rand_index"],
+        default=[],
+        # default=["rand_index"],
         help=f"Specify the list of clustering metrics to calculate."
         f"   Example: --metric_annot rand_index"
         f"   List of annotation metrics: {annot.__all__}",
     )
     metric_options.add_argument(
         "--metric_dimred",
         nargs="+",
         type=str,
-        default=["kruskal_stress"],
+        # default=["kruskal_stress"],
+        default=[],
         help="Specify the list of dimensionality reduction "
         "metrics to calculate.\n"
         "   Example: --metric_dimred kruskal_stress\n"
         f"   List of dim. red. metrics: {dimred.__all__}",
     )
+    metric_options.add_argument(
+        "--TEST_ALLMETRICS",
+        action="store_true",
+        help="Run the pipeline with all metrics available.\n"
+        f"   List of cluster metrics: {cluster.__all__}\n"
+        f"   List of annotation metrics: {annot.__all__}\n"
+        f"   List of dim. red. metrics: {dimred.__all__}",
+    )
 
     # Parse all args
     args = parser.parse_args()
 
+    # Validate TEST_ALLMETRICS
+    if args.TEST_ALLMETRICS:
+        logger.info(
+            "TEST_ALLMETRICS parameter is present : "
+            "All Metrics will be added for processing"
+        )
+        args.metric_cluster = cluster.__all__
+        args.metric_annot = annot.__all__
+        args.metric_dimred = dimred.__all__
+
     # If a config file was provided, load the new args
     if args.config != "":
         logger.info(
             "Read config file {} to get new checkatlas configs".format(
                 args.config
             )
         )
@@ -198,18 +223,14 @@
     if args.debug:
         logger.setLevel(getattr(logging, "DEBUG"))
     else:
         logger.setLevel(getattr(logging, "INFO"))
 
     logger.debug(f"Program arguments: {args}")
 
-    args.metric_cluster = cluster.__all__
-    args.metric_annot = annot.__all__
-    args.metric_dimred = dimred.__all__
-
     # Save all arguments to yaml (only run it when
     # generating example file config.yaml
     # save_arguments(args, 'config/default_config.yaml')
 
     #   ######    Run Checkatlas   #########
     checkatlas.run(args)
```

### Comparing `checkatlas-0.2.2/checkatlas/atlas.py` & `checkatlas-0.2.3/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/atlas_seurat.py` & `checkatlas-0.2.3/checkatlas/atlas_seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/checkatlas.py` & `checkatlas-0.2.3/checkatlas/checkatlas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 import csv
 import inspect
 import logging
 import os
 from datetime import datetime
 
 from . import atlas, atlas_seurat, checkatlas_workflow, folders, multiqc
@@ -42,62 +43,57 @@
     List all atlases files in the path
     Detect .rds, .h5, .h5ad
 
     Args:
         path: Path for searching single-cell atlases.
 
     Returns:
-        List of file atlases to check.
+        list: List of file atlases to check.
     """
     atlas_list = list()
     for root, dirs, files in os.walk(path):
         for file in files:
             for extension in EXTENSIONS:
                 if file.endswith(extension):
                     atlas_list.append(os.path.join(root, file))
     return atlas_list
 
 
-def get_atlas_name(atlas_path):
+def get_atlas_name(atlas_path: str) -> str:
     """
     From atlas_path extract the atlas_name
     Args:
         atlas_path:
     Returns:
-
+        str: The atlas_name
     """
     return os.path.splitext(os.path.basename(atlas_path))[0]
 
 
-def get_atlas_extension(atlas_path):
+def get_atlas_extension(atlas_path: str) -> str:
     """
     From atlas_path extract the atlas file extension
     Args:
         atlas_path:
     Returns:
-
+        None
     """
     return os.path.splitext(os.path.basename(atlas_path))[1]
 
 
-def clean_list_atlases(atlas_list, path) -> tuple:
+def clean_list_atlases(atlas_list: list, checkatlas_path: str) -> tuple:
     """
-    Go through all files and detect Seurat or Scanpy Atlas
-    Then:
-    - Convert Seurat files to Scanpy
-    - Clean Scanpy files
+    Go through all files and detect Seurat, CellRanger or Scanpy Atlas
+    The "cleaning means that we test if the atlas is valid or not.
     Args:
-        atlas_list:
+        atlas_list: list of atlases found with proper extension
+        checkatlas_path: the path where checkatlas files are saved
     Returns:
-         clean_list_atlas will only cleaned Scanpy atlas. A dict with
-    these info ['Atlas_Name','Type','Atlas_file_extension',
-    'Checkatlas_folder']
+         tuple: clean_atlas_scanpy, clean_atlas_seurat, clean_atlas_cellranger
     """
-    # Create dict with these info ['Atlas_Name','Type','Converted',
-    # 'Checkatlas_path']
     clean_atlas_scanpy = dict()
     clean_atlas_seurat = dict()
     clean_atlas_cellranger = dict()
     for atlas_path in atlas_list:
         atlas_name = get_atlas_name(atlas_path)
         if atlas_path.endswith(".rds"):
             logger.debug(f"Include Atlas: {atlas_name} from {atlas_path}")
@@ -126,40 +122,43 @@
             info = [
                 atlas_name,
                 "Scanpy",
                 ".h5ad",
                 os.path.dirname(atlas_path) + "/",
             ]
             clean_atlas_scanpy[atlas_path] = info
-    # open file for writing, "w" is writing
+    # Save the list of atlas taken into account
     dict_file = open(
-        os.path.join(folders.get_workingdir(path), "list_atlases.csv"), "w"
+        os.path.join(
+            folders.get_workingdir(checkatlas_path), "list_atlases.csv"
+        ),
+        "w",
     )
     w = csv.writer(dict_file)
     # loop over dictionary keys and values
     for key, val in clean_atlas_scanpy.items():
         w.writerow([key, ",".join(val)])
     for key, val in clean_atlas_seurat.items():
         w.writerow([key, ",".join(val)])
     for key, val in clean_atlas_cellranger.items():
         w.writerow([key, ",".join(val)])
     dict_file.close()
     return clean_atlas_scanpy, clean_atlas_seurat, clean_atlas_cellranger
 
 
-def get_pipeline_functions(module, args):
+def get_pipeline_functions(module, args) -> list:
     """
     Using arguments of checkatlas program -> build
     the list of functions to run on each adata
     and seurat object
     Args:
-        module:
-        args:
+        module: Module to use either atlas or atlas_seurat
+        args: List of args for checkatlas program
     Returns:
-         list of functions to run
+         list: list of functions to run
     """
     checkatlas_functions = list()
 
     if not args.NOADATA:
         checkatlas_functions.append(module.create_anndata_table)
     if not args.NOQC:
         if "violin_plot" in args.qc_display:
@@ -193,29 +192,30 @@
     # Create summary by default, it is ran at last so it marks
     # the end of the pipeline
     # This table is then used by the resume option
     checkatlas_functions.append(module.create_summary_table)
     return checkatlas_functions
 
 
-def run(args):
+def run(args: argparse.Namespace) -> None:
     """
     Main function of checkatlas
     Run all functions for all atlases:
     - Clean files list by getting only Scanpy atlas (converted from Seurat
     if necessary)
     - Extract summary tables
     - Create UMAP and T-sne figures
     - Calculate every metrics
 
     Args:
-        args:
+        args: List of args for checkatlas program
     Returns:
-
+        None
     """
+
     logger.debug(f"Transform path to absolute:{args.path}")
     args.path = os.path.abspath(args.path)
     logger.debug(f"Check checkatlas folders in:{args.path}")
     folders.checkatlas_folders(args.path)
 
     logger.info("Searching Seurat, Cellranger and Scanpy files")
     atlas_list = list_atlases(args.path)
@@ -244,73 +244,89 @@
     clean_atlas.update(clean_atlas_seurat)
 
     if len(clean_atlas_cellranger) > 0:
         logger.debug("Install Seurat if needed")
         atlas_seurat.check_seurat_install()
 
     # Run all checkatlas analysis
-    if args.nextflow == 0:
-        logger.info(
-            "--nextflow option not found: Run checkatlas workflow "
-            "without Nextflow"
-        )
-        run_checkatlas(clean_atlas, args)
-    else:
+    # if args.nextflow == 0:
+    logger.info(
+        "--nextflow option not found: Run checkatlas workflow "
+        "without Nextflow"
+    )
+    run_checkatlas(clean_atlas, args)
+    """ else:
         clean_atlas.update(clean_atlas_seurat)
         logger.info(
             "--nextflow option found: Run checkatlas workflow with Nextflow"
         )
         logger.info(f"Use {args.nextflow} threads")
-        checkatlas_workflow.create_checkatlas_worflows(clean_atlas, args)
-        script_path = os.path.dirname(os.path.realpath(__file__))
-        nextflow_main = os.path.join(script_path, "checkatlas_workflow.nf")
-        yaml_files = os.path.join(
-            folders.get_folder(args.path, folders.TEMP), "*.yaml"
-        )
-
-        # getting the current date and time
-        current_datetime = datetime.now()
-        current_time = current_datetime.strftime("%Y%d%m-%H%M%S")
-        report_file = os.path.join(
-            folders.get_workingdir(args.path),
-            f"Nextflow_report-{current_time}.html",
-        )
-        timeline_file = os.path.join(
-            folders.get_workingdir(args.path),
-            f"Nextflow_timeline-{current_time}.html",
-        )
-        working_dir_nextflow = folders.get_folder(args.path, folders.NEXTFLOW)
-        nextflow_cmd = (
-            f"nextflow run -w "
-            f"{working_dir_nextflow}"
-            f" {nextflow_main} -queue-size {args.nextflow} --files "
-            f'"{yaml_files}" -with-report {report_file}'
-            f" -with-timeline {timeline_file}"
-        )
-        logger.debug(f"Execute: {nextflow_cmd}")
-        script_path = os.path.dirname(os.path.realpath(__file__))
-        nextflow_main = os.path.join(script_path, "checkatlas_workflow.nf")
-        # Run Nextflow
-        os.system(nextflow_cmd)
-        logger.debug(f"Nextflow report saved in {report_file}")
-        logger.debug(f"Nextflow timeline saved in {timeline_file}")
+        run_checkatlas_nextflow(clean_atlas, args) """
 
     if not args.NOMULTIQC:
         logger.info("Run MultiQC")
         multiqc.run_multiqc(args)
 
 
-def run_checkatlas(clean_atlas, args):
+def run_checkatlas_nextflow(clean_atlas, args) -> None:
     """
-    Run Checkatlas pipeline for all Scanpy and Cellranger objects
+    Run the checkatlas pipeline by using Nextflow.
+    checkatlas_workflow.nf will be run with specific
+    parameters.
+
     Args:
-        clean_atlas_scanpy:
-        args:
+        clean_atlas: List of atlases
+        args: List of args for checkatlas program
+
     Returns:
+        None
+    """
+    checkatlas_workflow.create_checkatlas_worflows(clean_atlas, args)
+    script_path = os.path.dirname(os.path.realpath(__file__))
+    nextflow_main = os.path.join(script_path, "checkatlas_workflow.nf")
+    yaml_files = os.path.join(
+        folders.get_folder(args.path, folders.TEMP), "*.yaml"
+    )
 
+    # getting the current date and time
+    current_datetime = datetime.now()
+    current_time = current_datetime.strftime("%Y%d%m-%H%M%S")
+    report_file = os.path.join(
+        folders.get_workingdir(args.path),
+        f"Nextflow_report-{current_time}.html",
+    )
+    timeline_file = os.path.join(
+        folders.get_workingdir(args.path),
+        f"Nextflow_timeline-{current_time}.html",
+    )
+    working_dir_nextflow = folders.get_folder(args.path, folders.NEXTFLOW)
+    nextflow_cmd = (
+        f"nextflow run -w "
+        f"{working_dir_nextflow}"
+        f" {nextflow_main} -queue-size {args.nextflow} --files "
+        f'"{yaml_files}" -with-report {report_file}'
+        f" -with-timeline {timeline_file}"
+    )
+    logger.debug(f"Execute: {nextflow_cmd}")
+    script_path = os.path.dirname(os.path.realpath(__file__))
+    nextflow_main = os.path.join(script_path, "checkatlas_workflow.nf")
+    # Run Nextflow
+    os.system(nextflow_cmd)
+    logger.debug(f"Nextflow report saved in {report_file}")
+    logger.debug(f"Nextflow timeline saved in {timeline_file}")
+
+
+def run_checkatlas(clean_atlas, args) -> None:
+    """
+    Run Checkatlas pipeline for all Scanpy and Cellranger objects
+    Args:
+        clean_atlas: List of atlas
+        args: List of args for checkatlas program
+    Returns:
+        None
     """
 
     # List all functions to run
     pipeline_functions_scanpy = get_pipeline_functions(atlas, args)
     pipeline_functions_seurat = get_pipeline_functions(atlas_seurat, args)
     logger.debug(
         f"List of functions which will be ran "
@@ -354,35 +370,7 @@
 
 if __name__ == "__main__":
     path = "/Users/christophebecavin/Documents/testatlas/"
     # atlas_path = "/Users/christophebecavin/Documents/testatlas/"
     atlas_info = ["test_version", "Scanpy", ".h5ad", "data/test_version.h5ad"]
     # folders.checkatlas_folders(path)
     # atlas_list = list_atlases(path)
-    # clean_atlas_dict = clean_list_atlases(atlas_list, path)
-    #
-    # for atlas_path, atlas_info in clean_atlas_dict.items():
-    #     print(atlas_path, atlas_info)
-    #     adata = read_atlas(atlas_path, atlas_info)
-    #     print(adata is not None)
-    #     if adata is not None:
-    #         adata = atlas.clean_scanpy_atlas(adata, atlas_info)
-    #         atlas.create_summary_table(adata, atlas_path, atlas_info, path)
-    #         atlas.create_anndata_table(adata, atlas_path, atlas_info, path)
-    #         # atlas.create_qc_plots(adata, atlas_path, atlas_info, path)
-    #         atlas.create_umap_fig(adata, atlas_path, atlas_info, path)
-    #         # atlas.create_tsne_fig(adata, atlas_path, atlas_info, path)
-    #         atlas.metric_cluster(adata, atlas_path, atlas_info, path)
-    #         atlas.metric_annot(adata, atlas_path, atlas_info, path)
-    #         atlas.metric_dimred(adata, atlas_path, atlas_info, path)
-# atlas_path = '/Users/christophebecavin/Documents/testatlas/hca/
-# HCA_Barbry_Grch38_Raw_filter_Norm.h5ad'
-# atlas_path = '/Users/christophebecavin/Documents/testatlas/Endothelial.h5ad'
-# atlas_name = get_atlas_name(atlas_path)
-# print('Read atlas')
-#     adata = read_atlas(atlas_path, atlas_info)
-#     sc.pp.subsample(adata, fraction=0.05)
-#     adata.write('/Users/christophebecavin/Documents/testatlas/Endothelial_lite.h5ad')
-#     print(adata)
-# print('Calc QC')
-# figure_path = '/Users/christophebecavin/Documents/testatlas/'
-# atlas.create_qc_plots(adata, atlas_path, atlas_name, figure_path)
```

### Comparing `checkatlas-0.2.2/checkatlas/checkatlas_workflow.nf` & `checkatlas-0.2.3/checkatlas/checkatlas_workflow.nf`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 process metric_dimred {
     input:
       path config_file
     script:
       """
       checkatlas-workflow metric_dimred ${config_file}
       """
+
+
 }
 
 
 workflow {
     config_file = channel.fromPath(params.files)
     summary(config_file)
     qc(config_file)
```

### Comparing `checkatlas-0.2.2/checkatlas/checkatlas_workflow.py` & `checkatlas-0.2.3/checkatlas/checkatlas_workflow.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/convertSeurat.R` & `checkatlas-0.2.3/checkatlas/convertSeurat.R`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.2.3/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/metrics/metrics.py` & `checkatlas-0.2.3/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.2.3/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.2.3/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.2.3/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.2.3/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.2/pyproject.toml` & `checkatlas-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.2.2"
+version = "0.2.3"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/convertSeurat.R", "checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
@@ -20,15 +20,14 @@
 matplotlib = "^3.7.0"
 rpy2 = "^3.5.8"
 llvmlite = "^0.39.1"
 numba = "^0.56.4"
 types-pyyaml = "^6.0.12.6"
 scanpy = "^1.9.1"
 numpy = "^1.23.5"
-nextflow = "^22.10.7"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^67.3.2"
 gitchangelog = "^3.0.4"
```

### Comparing `checkatlas-0.2.2/setup.py` & `checkatlas-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,29 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['llvmlite>=0.39.1,<0.40.0',
  'matplotlib>=3.7.0,<4.0.0',
  'multiqc>=1.14,<2.0',
- 'nextflow>=22.10.7,<23.0.0',
  'numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
  'rpy2>=3.5.8,<4.0.0',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main',
                      'checkatlas-workflow = '
                      'checkatlas.checkatlas_workflow:workflow']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "\n# CheckAtlas\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.2.2/PKG-INFO` & `checkatlas-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.2.2
+Version: 0.2.3
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: MIT
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: multiqc (>=1.14,<2.0)
-Requires-Dist: nextflow (>=22.10.7,<23.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: rpy2 (>=3.5.8,<4.0.0)
 Requires-Dist: scanpy (>=1.9.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.6,<7.0.0.0)
 Project-URL: Documentation, https://checkatlas.readthedocs.io/
```

