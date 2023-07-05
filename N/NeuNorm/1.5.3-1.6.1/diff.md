# Comparing `tmp/NeuNorm-1.5.3.tar.gz` & `tmp/NeuNorm-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NeuNorm-1.5.3.tar", last modified: Tue May  3 18:40:45 2022, max compression
+gzip compressed data, was "NeuNorm-1.6.1.tar", last modified: Wed Jul  5 16:42:28 2023, max compression
```

## Comparing `NeuNorm-1.5.3.tar` & `NeuNorm-1.6.1.tar`

### file list

```diff
@@ -1,281 +1,269 @@
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      130 2020-07-28 18:12:39.000000 NeuNorm-1.5.3/.gitignore
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1283 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/.travis.yml
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      678 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/CONTRIBUTING.md
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1529 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/LICENSE.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      105 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/MANIFEST.in
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      120 2022-05-03 18:34:30.000000 NeuNorm-1.5.3/NeuNorm/__init__.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      684 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/NeuNorm/_utilities.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      334 2022-05-03 18:36:03.000000 NeuNorm-1.5.3/NeuNorm/exporter.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1143 2021-10-22 14:59:29.000000 NeuNorm-1.5.3/NeuNorm/loader.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    37987 2022-05-03 18:37:14.000000 NeuNorm-1.5.3/NeuNorm/normalization.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      965 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/NeuNorm/roi.py
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm.egg-info/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      595 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm.egg-info/PKG-INFO
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9369 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm.egg-info/SOURCES.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        1 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm.egg-info/dependency_links.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       35 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm.egg-info/requires.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        8 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/NeuNorm.egg-info/top_level.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      595 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/PKG-INFO
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4187 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/README.md
--rwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)      409 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/clean.sh
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       54 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/codecov.yml
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/conda-recipes/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       33 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/conda-recipes/conda_build_config.yaml
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      739 2020-07-28 14:11:45.000000 NeuNorm-1.5.3/conda-recipes/meta.yaml
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    27983 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/coverage.xml
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/data/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/data/df/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40176 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/df/DC0000.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40176 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/df/DC0001.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40176 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/df/DC0002.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/data/ob/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0001.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0002.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0003.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0004.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0005.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0006.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0007.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0008.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0009.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0010.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0011.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0012.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0013.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0014.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/ob/0015.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/data/sample/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0002.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0003.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0004.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0005.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0006.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0007.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0008.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0009.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0010.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0011.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0012.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0013.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0014.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/data/sample/0015.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      617 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/Makefile
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      230 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.buildinfo
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/.doctrees/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4620 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/cropping_data.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3112 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/dark_field_correction.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    27263 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/environment.pickle
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3428 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/export_data.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5108 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/index.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3109 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/installation.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    37278 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/loading.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6096 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/normalization.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4096 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/notebook.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3811 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/retrieve_normalized_data.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    13595 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    17659 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/tutorial_using_array_input.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    16609 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.doctrees/tutorial_using_folder_input.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/.nojekyll
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/doctrees/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4649 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/cropping_data.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3135 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/dark_field_correction.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    18098 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/environment.pickle
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3451 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/export_data.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4975 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/index.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3648 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/installation.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    46780 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/loading.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7072 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/normalization.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4119 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/notebook.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3834 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/retrieve_normalized_data.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9513 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11820 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/tutorial_using_array_input.doctree
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11793 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/doctrees/tutorial_using_folder_input.doctree
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      230 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/.buildinfo
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/.nojekyll
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/_images/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3317 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_images/progress_bar_loading.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3493 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_images/progress_bar_normalization.png
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/_sources/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      513 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/cropping_data.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      318 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/dark_field_correction.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      418 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/export_data.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      585 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/index.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      404 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/installation.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11521 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/loading.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1217 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/normalization.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      707 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/notebook.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      535 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/retrieve_normalized_data.rst.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7289 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/tutorial_normalization_with_fewer_ob_than_sample.ipynb.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8991 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/tutorial_using_array_input.ipynb.txt
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8531 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_sources/tutorial_using_folder_input.ipynb.txt
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/_static/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      673 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/ajax-loader.gif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    10317 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/basic.css
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      756 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/comment-bright.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      829 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/comment-close.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      641 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/comment.png
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/_static/css/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3376 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/css/badge_only.css
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   112267 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/css/theme.css
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8166 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/doctools.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      222 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/down-pressed.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      202 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/down.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      286 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/file.png
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   109948 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    96964 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   656544 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/Lato-Bold.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   656568 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/Lato-Regular.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   170616 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   169064 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    76518 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   391622 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   152796 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    90412 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   263767 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/jquery-3.1.0.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    86351 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/jquery.js
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/build/html/_static/js/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    15414 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/js/modernizr.min.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6477 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/js/theme.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       90 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/minus.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    14545 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/normalization_equation.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   158109 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/normalization_principle.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       90 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/plus.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3317 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/progress_bar_loading.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3493 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/progress_bar_normalization.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4395 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/pygments.css
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    25370 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/searchtools.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    35168 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    12140 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/underscore.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      214 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/up-pressed.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      203 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/up.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    25351 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/_static/websupport.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7915 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/cropping_data.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6984 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/dark_field_correction.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7806 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/export_data.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4969 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/genindex.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9001 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/index.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7490 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/installation.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    46993 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/loading.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    10703 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/normalization.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7500 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/notebook.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      936 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/objects.inv
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9264 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/retrieve_normalized_data.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5364 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/search.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4576 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/searchindex.js
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    18969 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/tutorial_normalization_with_fewer_ob_than_sample.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    23023 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/tutorial_using_array_input.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    20590 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/build/html/tutorial_using_folder_input.html
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      215 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/readthedocs-environment.yml
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/source/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/documentation/source/_static/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    14545 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/_static/normalization_equation.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   158109 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/_static/normalization_principle.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3317 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/_static/progress_bar_loading.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3493 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/_static/progress_bar_normalization.png
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5470 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/conf.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      513 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/cropping_data.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      318 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/dark_field_correction.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      418 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/export_data.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      585 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/index.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      404 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/installation.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11521 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/loading.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1217 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/normalization.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      707 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/notebook.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      535 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/retrieve_normalized_data.rst
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7289 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/tutorial_normalization_with_fewer_ob_than_sample.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8991 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/tutorial_using_array_input.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8531 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/documentation/source/tutorial_using_folder_input.ipynb
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/notebooks/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7361 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/debugging_multi_roi_bug.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4429 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/ipts-16259.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4074 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/notebook_display_with_time_estimation.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4816 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/testing_new_auto_gamma_filtering.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6661 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/tutorial_normalization_with_fewer_ob_than_sample.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7286 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/tutorial_normalization_with_fewer_ob_than_sample_MAYBE_BUG.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8386 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/tutorial_using_array_input.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4961 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/tutorial_using_array_input_and_export_array.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8587 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/tutorial_using_array_input_and_several_roi.ipynb
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8116 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/notebooks/tutorial_using_folder_input.ipynb
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/paper/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      818 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/paper/paper.bib
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3292 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/paper/paper.md
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      328 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/readthedocs.yml
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       90 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/setup.cfg
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     2458 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/setup.py
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/tests/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/NeuNorm/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6554 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/NeuNorm/cropping_test.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6622 2022-05-03 18:38:42.000000 NeuNorm-1.5.3/tests/NeuNorm/export_test.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    13393 2022-03-15 18:44:53.000000 NeuNorm-1.5.3/tests/NeuNorm/loading_test.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    36504 2022-03-21 12:18:27.000000 NeuNorm-1.5.3/tests/NeuNorm/normalizing_test.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3204 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/NeuNorm/roi_test.py
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1816 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/NeuNorm/utilities_test.py
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/different_format/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      198 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/different_format/df001_4_by_4.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      198 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/different_format/image001_4_by_4.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      368 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/different_format/image001_with_gamma.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/different_format/not_supported_file.fake
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      198 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/different_format/ob001_4_by_4.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/tests/data/fits/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/fits/df/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/df/df001.fits
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/fits/ob/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/ob/ob001.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/ob/ob002.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/ob/ob003.fits
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/fits/sample/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/sample/image001.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/sample/image002.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/fits/sample/image003.fits
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/fits/test_roi/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 15:52:29.000000 NeuNorm-1.5.3/tests/data/fits/test_roi/ob.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 14:59:31.000000 NeuNorm-1.5.3/tests/data/fits/test_roi/sample.fits
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/tests/data/fits/tof/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/fits/tof/ob/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2021-08-26 12:47:42.000000 NeuNorm-1.5.3/tests/data/fits/tof/ob/ob_001.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2021-08-26 12:47:52.000000 NeuNorm-1.5.3/tests/data/fits/tof/ob/ob_002.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2021-08-26 12:48:02.000000 NeuNorm-1.5.3/tests/data/fits/tof/ob/ob_003.fits
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/fits/tof/sample/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2021-08-26 12:46:18.000000 NeuNorm-1.5.3/tests/data/fits/tof/sample/sample_001.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2021-08-26 12:46:53.000000 NeuNorm-1.5.3/tests/data/fits/tof/sample/sample_002.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2021-08-26 12:47:22.000000 NeuNorm-1.5.3/tests/data/fits/tof/sample/sample_003.fits
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/format_not_suppored.txt
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/hdf5/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/hdf5/dump_file.hdf5
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/ob001.fits
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/tests/data/tif/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/df/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/df/df001.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/df/df002.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/df/df003.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/ob/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/ob/ob001.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/ob/ob002.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/ob/ob003.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/sample/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      304 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/data/tif/sample/image001.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      304 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/data/tif/sample/image002.tif
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      304 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/data/tif/sample/image003.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/sample_with_gamma/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2020-07-28 12:15:35.000000 NeuNorm-1.5.3/tests/data/tif/sample_with_gamma/image001.tif
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/special_ob/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/data/tif/special_ob/ob_0001_2rois.tiff
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/special_sample/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/data/tif/special_sample/image_0001_2rois.tiff
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-25 20:52:04.000000 NeuNorm-1.5.3/tests/data/tif/special_sample/image_0001_roi_no_ob.tiff
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:44.000000 NeuNorm-1.5.3/tests/data/tif/tof/
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/tof/ob/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-26 11:50:47.000000 NeuNorm-1.5.3/tests/data/tif/tof/ob/ob_01.tiff
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-26 11:51:00.000000 NeuNorm-1.5.3/tests/data/tif/tof/ob/ob_02.tiff
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-26 11:51:18.000000 NeuNorm-1.5.3/tests/data/tif/tof/ob/ob_03.tiff
-drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2022-05-03 18:40:45.000000 NeuNorm-1.5.3/tests/data/tif/tof/sample/
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-26 11:49:41.000000 NeuNorm-1.5.3/tests/data/tif/tof/sample/tof_01.tiff
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-26 11:49:59.000000 NeuNorm-1.5.3/tests/data/tif/tof/sample/tof_02.tiff
--rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2021-08-26 11:50:24.000000 NeuNorm-1.5.3/tests/data/tif/tof/sample/tof_03.tiff
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.512245 NeuNorm-1.6.1/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      130 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/.gitignore
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1283 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/.travis.yml
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      678 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/CONTRIBUTING.md
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.480890 NeuNorm-1.6.1/ImagingReso.egg-info/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      581 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/ImagingReso.egg-info/PKG-INFO
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      341 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/ImagingReso.egg-info/SOURCES.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        1 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/ImagingReso.egg-info/dependency_links.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       42 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/ImagingReso.egg-info/requires.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        8 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/ImagingReso.egg-info/top_level.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1529 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/LICENSE.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      105 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/MANIFEST.in
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.482025 NeuNorm-1.6.1/NeuNorm/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      120 2023-07-05 12:22:20.000000 NeuNorm-1.6.1/NeuNorm/__init__.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      684 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/NeuNorm/_utilities.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      331 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/NeuNorm/exporter.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1146 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/NeuNorm/loader.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    36768 2023-07-05 12:32:14.000000 NeuNorm-1.6.1/NeuNorm/normalization.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      965 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/NeuNorm/roi.py
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.482719 NeuNorm-1.6.1/NeuNorm.egg-info/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      576 2023-07-05 16:42:28.000000 NeuNorm-1.6.1/NeuNorm.egg-info/PKG-INFO
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9096 2023-07-05 16:42:28.000000 NeuNorm-1.6.1/NeuNorm.egg-info/SOURCES.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        1 2023-07-05 16:42:28.000000 NeuNorm-1.6.1/NeuNorm.egg-info/dependency_links.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       35 2023-07-05 16:42:28.000000 NeuNorm-1.6.1/NeuNorm.egg-info/requires.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        8 2023-07-05 16:42:28.000000 NeuNorm-1.6.1/NeuNorm.egg-info/top_level.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      576 2023-07-05 16:42:28.512402 NeuNorm-1.6.1/PKG-INFO
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4187 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/README.md
+-rwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)      409 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/clean.sh
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       54 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/codecov.yml
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.482996 NeuNorm-1.6.1/conda-recipes/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       33 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/conda-recipes/conda_build_config.yaml
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      739 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/conda-recipes/meta.yaml
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    27983 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/coverage.xml
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.476186 NeuNorm-1.6.1/data/
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.483475 NeuNorm-1.6.1/data/df/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40176 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/df/DC0000.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40176 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/df/DC0001.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40176 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/df/DC0002.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.485859 NeuNorm-1.6.1/data/ob/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0001.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0002.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0003.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0004.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0005.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0006.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0007.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0008.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0009.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0010.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0011.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0012.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0013.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0014.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/ob/0015.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.488005 NeuNorm-1.6.1/data/sample/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0002.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0003.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0004.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0005.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0006.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0007.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0008.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0009.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0010.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0011.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0012.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0013.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0014.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    40134 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/data/sample/0015.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.488275 NeuNorm-1.6.1/documentation/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      617 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/Makefile
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.488529 NeuNorm-1.6.1/documentation/build/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      230 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.buildinfo
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.490261 NeuNorm-1.6.1/documentation/build/.doctrees/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4620 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/cropping_data.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3112 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/dark_field_correction.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    27263 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/environment.pickle
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3428 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/export_data.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5108 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/index.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3109 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/installation.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    37278 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/loading.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6096 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/normalization.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4096 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/notebook.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3811 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/retrieve_normalized_data.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    13595 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    17659 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/tutorial_using_array_input.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    16609 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.doctrees/tutorial_using_folder_input.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/.nojekyll
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.491985 NeuNorm-1.6.1/documentation/build/doctrees/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4649 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/cropping_data.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3135 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/dark_field_correction.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    18098 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/environment.pickle
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3451 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/export_data.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4975 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/index.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3648 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/installation.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    46780 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/loading.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7072 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/normalization.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4119 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/notebook.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3834 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/retrieve_normalized_data.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9513 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11820 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/tutorial_using_array_input.doctree
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11793 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/doctrees/tutorial_using_folder_input.doctree
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.494285 NeuNorm-1.6.1/documentation/build/html/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      230 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/.buildinfo
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/.nojekyll
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.494559 NeuNorm-1.6.1/documentation/build/html/_images/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3317 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_images/progress_bar_loading.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3493 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_images/progress_bar_normalization.png
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.496080 NeuNorm-1.6.1/documentation/build/html/_sources/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      513 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/cropping_data.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      318 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/dark_field_correction.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      418 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/export_data.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      585 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/index.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      404 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/installation.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11521 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/loading.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1217 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/normalization.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      707 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/notebook.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      535 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/retrieve_normalized_data.rst.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7289 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/tutorial_normalization_with_fewer_ob_than_sample.ipynb.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8991 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/tutorial_using_array_input.ipynb.txt
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8531 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_sources/tutorial_using_folder_input.ipynb.txt
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.499454 NeuNorm-1.6.1/documentation/build/html/_static/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      673 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/ajax-loader.gif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    10317 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/basic.css
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      756 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/comment-bright.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      829 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/comment-close.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      641 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/comment.png
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.499726 NeuNorm-1.6.1/documentation/build/html/_static/css/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3376 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/css/badge_only.css
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   112267 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/css/theme.css
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8166 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/doctools.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      222 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/down-pressed.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      202 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/down.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      286 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/file.png
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.502669 NeuNorm-1.6.1/documentation/build/html/_static/fonts/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   109948 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    96964 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   656544 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   656568 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/Lato-Regular.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   170616 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   169064 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    76518 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   391622 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   152796 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    90412 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   263767 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/jquery-3.1.0.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    86351 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/jquery.js
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.502991 NeuNorm-1.6.1/documentation/build/html/_static/js/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    15414 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/js/modernizr.min.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6477 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/js/theme.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       90 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/minus.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    14545 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/normalization_equation.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   158109 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/normalization_principle.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       90 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/plus.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3317 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/progress_bar_loading.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3493 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/progress_bar_normalization.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4395 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/pygments.css
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    25370 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/searchtools.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    35168 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    12140 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/underscore.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      214 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/up-pressed.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      203 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/up.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    25351 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/_static/websupport.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7915 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/cropping_data.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6984 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/dark_field_correction.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7806 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/export_data.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4969 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/genindex.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9001 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/index.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7490 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/installation.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    46993 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/loading.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    10703 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/normalization.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7500 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/notebook.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      936 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/objects.inv
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     9264 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/retrieve_normalized_data.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5364 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/search.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4576 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/searchindex.js
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    18969 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/tutorial_normalization_with_fewer_ob_than_sample.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    23023 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/tutorial_using_array_input.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    20590 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/build/html/tutorial_using_folder_input.html
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      215 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/readthedocs-environment.yml
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.504612 NeuNorm-1.6.1/documentation/source/
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.505205 NeuNorm-1.6.1/documentation/source/_static/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    14545 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/_static/normalization_equation.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)   158109 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/_static/normalization_principle.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3317 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/_static/progress_bar_loading.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3493 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/_static/progress_bar_normalization.png
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5470 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/conf.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      513 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/cropping_data.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      318 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/dark_field_correction.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      418 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/export_data.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      585 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/index.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      404 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/installation.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    11521 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/loading.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1217 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/normalization.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      707 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/notebook.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      535 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/retrieve_normalized_data.rst
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7289 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/tutorial_normalization_with_fewer_ob_than_sample.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8991 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/tutorial_using_array_input.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8531 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/documentation/source/tutorial_using_folder_input.ipynb
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.506509 NeuNorm-1.6.1/notebooks/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7361 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/debugging_multi_roi_bug.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4429 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/ipts-16259.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4074 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/notebook_display_with_time_estimation.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4816 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/testing_new_auto_gamma_filtering.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6661 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/tutorial_normalization_with_fewer_ob_than_sample.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     7286 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/tutorial_normalization_with_fewer_ob_than_sample_MAYBE_BUG.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8386 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/tutorial_using_array_input.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     4961 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/tutorial_using_array_input_and_export_array.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8587 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/tutorial_using_array_input_and_several_roi.ipynb
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     8116 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/notebooks/tutorial_using_folder_input.ipynb
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.506832 NeuNorm-1.6.1/paper/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      818 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/paper/paper.bib
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3292 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/paper/paper.md
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      328 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/readthedocs.yml
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)       90 2023-07-05 16:42:28.512856 NeuNorm-1.6.1/setup.cfg
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     2458 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/setup.py
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.477470 NeuNorm-1.6.1/tests/
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.507988 NeuNorm-1.6.1/tests/NeuNorm/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6554 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/NeuNorm/cropping_test.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     6620 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/NeuNorm/export_test.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    13285 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/NeuNorm/loading_test.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)    32384 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/NeuNorm/normalizing_test.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     3204 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/NeuNorm/roi_test.py
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     1816 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/NeuNorm/utilities_test.py
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.508226 NeuNorm-1.6.1/tests/data/
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.508828 NeuNorm-1.6.1/tests/data/different_format/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      198 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/different_format/df001_4_by_4.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      198 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/different_format/image001_4_by_4.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      368 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/different_format/image001_with_gamma.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/different_format/not_supported_file.fake
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      198 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/different_format/ob001_4_by_4.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.477886 NeuNorm-1.6.1/tests/data/fits/
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.508948 NeuNorm-1.6.1/tests/data/fits/df/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/df/df001.fits
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.509306 NeuNorm-1.6.1/tests/data/fits/ob/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/ob/ob001.fits
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/ob/ob002.fits
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/ob/ob003.fits
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.509682 NeuNorm-1.6.1/tests/data/fits/sample/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/sample/image001.fits
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/sample/image002.fits
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/sample/image003.fits
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.509977 NeuNorm-1.6.1/tests/data/fits/test_roi/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/test_roi/ob.fits
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/fits/test_roi/sample.fits
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/format_not_suppored.txt
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.510153 NeuNorm-1.6.1/tests/data/hdf5/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/hdf5/dump_file.hdf5
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)     5760 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/ob001.fits
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.478456 NeuNorm-1.6.1/tests/data/tif/
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.510581 NeuNorm-1.6.1/tests/data/tif/df/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/df/df001.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/df/df002.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/df/df003.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.511032 NeuNorm-1.6.1/tests/data/tif/ob/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/ob/ob001.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/ob/ob002.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/ob/ob003.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.511506 NeuNorm-1.6.1/tests/data/tif/sample/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      304 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/sample/image001.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      304 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/sample/image002.tif
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      304 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/sample/image003.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.511659 NeuNorm-1.6.1/tests/data/tif/sample_with_gamma/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/sample_with_gamma/image001.tif
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.511797 NeuNorm-1.6.1/tests/data/tif/special_ob/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/special_ob/ob_0001_2rois.tiff
+drwxr-xr-x   0 j35      (1376125886) ORNL\Domain Users (1551083765)        0 2023-07-05 16:42:28.512069 NeuNorm-1.6.1/tests/data/tif/special_sample/
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/special_sample/image_0001_2rois.tiff
+-rw-r--r--   0 j35      (1376125886) ORNL\Domain Users (1551083765)      234 2023-07-05 12:20:43.000000 NeuNorm-1.6.1/tests/data/tif/special_sample/image_0001_roi_no_ob.tiff
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `NeuNorm-1.5.3/.travis.yml` & `NeuNorm-1.6.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/CONTRIBUTING.md` & `NeuNorm-1.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/LICENSE.txt` & `NeuNorm-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/NeuNorm/_utilities.py` & `NeuNorm-1.6.1/NeuNorm/_utilities.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/NeuNorm/loader.py` & `NeuNorm-1.6.1/NeuNorm/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     try:
         tmp = fits.open(file_name,ignore_missing_end=True)[0].data
         if len(tmp.shape) == 3:
             tmp = tmp.reshape(tmp.shape[1:])
         return tmp
     except OSError:
         raise OSError("Unable to read the FITS file provided!")
-
-
+    
 def load_tiff(file_name):
     '''load tiff image
     
     Parameters:
     -----------
        full file name of tiff image
     '''
```

### Comparing `NeuNorm-1.5.3/NeuNorm/normalization.py` & `NeuNorm-1.6.1/NeuNorm/normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 import numpy as np
 import os
 import copy
 import time
 from scipy.ndimage import convolve
-from scipy.ndimage import median_filter
 
 from NeuNorm.loader import load_hdf, load_tiff, load_fits
-from NeuNorm.exporter import make_fits, make_tiff
+from NeuNorm.exporter import make_fits, make_tif
 from NeuNorm.roi import ROI
 from NeuNorm._utilities import get_sorted_list_images, average_df
 from NeuNorm import DataType
 
 
 class Normalization(object):
     working_data_type = np.float32
@@ -53,15 +52,15 @@
         self.data['sample'] = self.dict_image
         self.data['ob'] = self.dict_ob
         self.data['df'] = self.dict_df
         self.data['normalized'] = None
         self.export_file_name = None
 
     def load(self, file='', folder='', data=None, data_type='sample', auto_gamma_filter=True,
-             manual_gamma_filter=False, notebook=False, manual_gamma_threshold=0.1):
+             manual_gamma_filter=False, notebook=False, manual_gamma_threshold=0.1, check_shape=True):
         """
         Function to read individual files, entire files from folder, list of files or event data arrays.
         Data are also gamma filtered if requested.
         
         Parameters:
            file: list -  full path to a single file, or list of files
            folder: string - full path to folder containing files to load
@@ -91,15 +90,16 @@
 
         if not file == '':
             if isinstance(file, str):
                 self.load_file(file=file,
                                data_type=data_type,
                                auto_gamma_filter=auto_gamma_filter,
                                manual_gamma_filter=manual_gamma_filter,
-                               manual_gamma_threshold=manual_gamma_threshold)
+                               manual_gamma_threshold=manual_gamma_threshold,
+                               check_shape=check_shape)
             elif isinstance(file, list):
                 if notebook:
                     # turn on progress bar
                     _message = "Loading {}".format(data_type)
                     box1 = widgets.HBox([widgets.Label(_message,
                                                        layout=widgets.Layout(width='20%')),
                                          widgets.IntProgress(max=len(file)),
@@ -112,22 +112,23 @@
 
                 start_time = time.time()
                 for _index, _file in enumerate(file):
                     self.load_file(file=_file,
                                    data_type=data_type,
                                    auto_gamma_filter=auto_gamma_filter,
                                    manual_gamma_filter=manual_gamma_filter,
-                                   manual_gamma_threshold=manual_gamma_threshold)
+                                   manual_gamma_threshold=manual_gamma_threshold,
+                                   check_shape=check_shape)
                     if notebook:
                         w1.value = _index + 1
                         end_time = time.time()
                         takes_its_going_to_take = self.calculate_how_long_its_going_to_take(index_we_are=_index + 1,
                                                                                             time_it_took_so_far=end_time - start_time,
                                                                                             total_number_of_loop=len(
-                                                                                                    file))
+                                                                                                file))
                         time_remaining_ui.value = "{}".format(takes_its_going_to_take)
 
                 if notebook:
                     box1.close()
 
         elif not folder == '':
             # load all files from folder
@@ -148,23 +149,24 @@
             start_time = time.time()
             for _index, _image in enumerate(list_images):
                 full_path_image = os.path.join(folder, _image)
                 self.load_file(file=full_path_image,
                                data_type=data_type,
                                auto_gamma_filter=auto_gamma_filter,
                                manual_gamma_filter=manual_gamma_filter,
-                               manual_gamma_threshold=manual_gamma_threshold)
+                               manual_gamma_threshold=manual_gamma_threshold,
+                               check_shape=check_shape)
                 if notebook:
                     # update progress bar
                     w1.value = _index + 1
                     end_time = time.time()
                     takes_its_going_to_take = self.calculate_how_long_its_going_to_take(index_we_are=_index + 1,
                                                                                         time_it_took_so_far=end_time - start_time,
                                                                                         total_number_of_loop=len(
-                                                                                                list_images))
+                                                                                            list_images))
                     time_remaining_ui.value = "{}".format(takes_its_going_to_take)
 
             if notebook:
                 box1.close()
 
         elif not data is None:
             self.load_data(data=data, data_type=data_type)
@@ -254,15 +256,16 @@
         else:
             self.data[data_type]['metadata'].append('')
         self.save_or_check_shape(data=data, data_type=data_type)
 
     def load_file(self, file='', data_type='sample',
                   auto_gamma_filter=True,
                   manual_gamma_filter=False,
-                  manual_gamma_threshold=0.1):
+                  manual_gamma_threshold=0.1,
+                  check_shape=True):
         """
         Function to read data from the specified path, it can read FITS, TIFF and HDF.
     
         Parameters
             file : string - full path of the input file with his extension.
             data_type: string - 'sample', 'df' or 'ob' (default 'sample')
             manual_gamma_filter: boolean  - apply or not gamma filtering (default False)
@@ -307,15 +310,16 @@
                 self.data[data_type]['metadata'].append(metadata)
 
             if self.data[data_type]['file_name'] is None:
                 self.data[data_type]['file_name'] = [file]
             else:
                 self.data[data_type]['file_name'].append(file)
 
-            self.save_or_check_shape(data=data, data_type=data_type)
+            if check_shape:
+                self.save_or_check_shape(data=data, data_type=data_type)
 
         else:
             raise OSError("The file name does not exist")
 
     def _auto_gamma_filtering(self, data=None):
         """perform the automatic gamma filtering
 
@@ -353,15 +357,15 @@
         mean_kernel = np.array([[1, 1, 1], [1, 0, 1], [1, 1, 1]]) / 8.0
         convolved_data = convolve(data_gamma_filtered, mean_kernel, mode='constant')
 
         data_gamma_filtered[gamma_indexes] = convolved_data[gamma_indexes]
 
         return data_gamma_filtered
 
-    def _manual_gamma_filtering(self, data=None, manual_gamma_threshold=0.95):
+    def _manual_gamma_filtering(self, data=None, manual_gamma_threshold=0.1):
         """perform manual gamma filtering on the data
 
         This algoritm uses the manual_gamma_threshold value to estimate if a pixel is a gamma or not.
         1. mean value of data array is calculated
         2. pixel is considered gamma if its value times the manual gamma threshold is bigger than the mean value
         3. if pixel is gamma, its value is replaced by the mean value of the 8 pixels surrounding it.
 
@@ -376,19 +380,21 @@
         Raises:
              ValueError if data is empty
         """
         if data is None:
             raise ValueError("Data array is empty!")
 
         data_gamma_filtered = np.copy(data)
+        mean_counts = np.mean(data_gamma_filtered)
+        gamma_indexes = np.where(manual_gamma_threshold * data_gamma_filtered > mean_counts)
 
-        radius = 2
-        median_counts = median_filter(data_gamma_filtered, radius, mode='grid-wrap')
-        gamma_indexes = np.where(manual_gamma_threshold * data_gamma_filtered > median_counts)
-        data_gamma_filtered[gamma_indexes] = median_counts[gamma_indexes]
+        mean_kernel = np.array([[1, 1, 1], [1, 0, 1], [1, 1, 1]]) / 8.0
+        convolved_data = convolve(data_gamma_filtered, mean_kernel, mode='constant')
+
+        data_gamma_filtered[gamma_indexes] = convolved_data[gamma_indexes]
 
         return data_gamma_filtered
 
     def save_or_check_shape(self, data=None, data_type='sample'):
         """save the shape for the first data loaded (of each type) otherwise
         check if the size match
 
@@ -408,41 +414,37 @@
         else:
             _prev_width = self.data[data_type]['shape']['width']
             _prev_height = self.data[data_type]['shape']['height']
 
             if (not (_prev_width == width)) or (not (_prev_height == height)):
                 raise IOError("Shape of {} do not match previous loaded data set!".format(data_type))
 
-    def normalization(self, roi=None, force=False, force_mean_ob=False, force_median_ob=False, notebook=False,
-                      use_only_sample=False):
+    def normalization(self, roi=None, force=False, force_mean_ob=False, notebook=False, use_only_sample=False):
         """normalization of the data
                 
         Parameters:
             roi: ROI object or list of ROI objects - object defines the region of the sample and OB that have to match
-                in intensity
+        in intensity
             force: boolean - True will force the normalization to occur, even if it had been
                 run before with the same data set (default False)
-            force_mean_ob: boolean - True will force using only 1 OB that is the mean of all the OBs
-            force_median_ob: boolean - True will force using only 1 OB that is the median of all the OBs
-            notebook: boolean - turn on this option if you run the library from a
-                notebook to have a progress bar displayed showing you the progress of the loading (default False)
-            use_only_sample: turn on this option to normalize the sample data using the ROI on the sample. each pixel
-                counts will be divided by the average counts of all the ROI of the same image
+        notebook: boolean - turn on this option if you run the library from a
+             notebook to have a progress bar displayed showing you the progress of the loading (default False)
+        use_only_sample - turn on this option to normalize the sample data using the ROI on the sample. each pixel
+            counts will be divided by the average counts of all the ROI of the same image
 
         Return:
             True - status of the normalization (True if every went ok, this is mostly used for the unit test)
 
         Raises:
             IOError: if no sample loaded
             IOError: if no OB loaded and use_only_sample if False
             IOError: if use_only_sample is True and no ROI provided
             IOError: if size of sample and OB do not match
         
         """
-
         if not force:
             # does nothing if normalization has already been run
             if self.__exec_process_status['normalization']:
                 return
         self.__exec_process_status['normalization'] = True
 
         # make sure we loaded some sample data
@@ -480,33 +482,31 @@
 
                 else:
                     _x0 = roi.x0
                     _y0 = roi.y0
                     _x1 = roi.x1
                     _y1 = roi.y1
 
-                    _sample_corrected_normalized = [_sample / np.median(_sample[_y0:_y1 + 1, _x0:_x1 + 1])
+                    _sample_corrected_normalized = [_sample / np.mean(_sample[_y0:_y1 + 1, _x0:_x1 + 1])
                                                     for _sample in self.data['sample']['data']]
-                    _ob_corrected_normalized = [_ob / np.median(_ob[_y0:_y1 + 1, _x0:_x1 + 1])
+                    _ob_corrected_normalized = [_ob / np.mean(_ob[_y0:_y1 + 1, _x0:_x1 + 1])
                                                 for _ob in self.data['ob']['data']]
 
             else:
 
                 _sample_corrected_normalized = copy.deepcopy(self.data['sample']['data'])
                 _ob_corrected_normalized = copy.deepcopy(self.data['ob']['data'])
 
             self.data[DataType.sample]['data'] = _sample_corrected_normalized
             self.data[DataType.ob]['data'] = _ob_corrected_normalized
 
-            # if the number of sample and ob do not match, use median of obs
+            # if the number of sample and ob do not match, use mean of obs
             nbr_sample = len(self.data['sample']['file_name'])
             nbr_ob = len(self.data['ob']['file_name'])
-
-            # will be deprecated soon!
-            if force_mean_ob:  # work with mean ob
+            if (nbr_sample != nbr_ob) or force_mean_ob:  # work with mean ob
                 _ob_corrected_normalized = np.mean(_ob_corrected_normalized, axis=0)
                 self.data['ob']['data_mean'] = _ob_corrected_normalized
                 _working_ob = copy.deepcopy(_ob_corrected_normalized)
                 _working_ob[_working_ob == 0] = np.NaN
 
                 if notebook:
                     # turn on progress bar
@@ -523,39 +523,14 @@
                     _norm[np.isnan(_norm)] = 0
                     _norm[np.isinf(_norm)] = 0
                     normalized_data.append(_norm)
 
                     if notebook:
                         w1.value = _index + 1
 
-            elif (nbr_sample != nbr_ob) or force_median_ob:  # work with median ob
-                _ob_corrected_normalized = np.median(_ob_corrected_normalized, axis=0)
-                self.data['ob']['data_mean'] = _ob_corrected_normalized
-                _working_ob = copy.deepcopy(_ob_corrected_normalized)
-                _working_ob[_working_ob == 0] = np.NaN
-
-                if notebook:
-                    # turn on progress bar
-                    _message = "Normalization"
-                    box1 = widgets.HBox([widgets.Label(_message,
-                                                       layout=widgets.Layout(width='20%')),
-                                         widgets.IntProgress(max=len(self.data['sample']['data']))])
-                    display(box1)
-                    w1 = box1.children[1]
-
-                normalized_data = []
-                for _index, _sample in enumerate(self.data['sample']['data']):
-                    _norm = np.divide(_sample, _working_ob)
-                    _norm[np.isnan(_norm)] = 0
-                    _norm[np.isinf(_norm)] = 0
-                    normalized_data.append(_norm)
-
-                    if notebook:
-                        w1.value = _index + 1
-
             else:  # 1 ob for each sample
                 # produce normalized data
                 sample_ob = zip(self.data['sample']['data'], self.data['ob']['data'])
 
                 if notebook:
                     # turn on progress bar
                     _message = "Normalization"
@@ -611,15 +586,15 @@
         else:
 
             _x0 = roi.x0
             _y0 = roi.y0
             _x1 = roi.x1
             _y1 = roi.y1
 
-            normalized_data = [_sample / np.median(_sample[_y0:_y1 + 1, _x0:_x1 + 1])
+            normalized_data = [_sample / np.mean(_sample[_y0:_y1 + 1, _x0:_x1 + 1])
                                for _sample in self.data['sample']['data']]
 
         return normalized_data
 
     def calculate_corrected_normalized(self, data_type=DataType.sample, roi=None):
         corrected_normalized = []
         for _sample in self.data[data_type]['data']:
@@ -793,22 +768,22 @@
         if not (self.data['normalized'] is None):
             new_normalized = [_data[_y0:_y1 + 1, _x0:_x1 + 1] for
                               _data in self.data['normalized']]
             self.data['normalized'] = new_normalized
 
         return True
 
-    def export(self, folder='./', data_type='normalized', file_type='tiff'):
+    def export(self, folder='./', data_type='normalized', file_type='tif'):
         """export all the data from the type specified into a folder
         
         Parameters:
             folder: String - where to create all the images. Folder must exist otherwise an error is
                 raised (default is './')
             data_type: String - Must be one of the following 'sample','ob','df','normalized' (default is 'normalized').
-            file_type: String - format in which to export the data. Must be either 'tiff' or 'fits' (default is 'tiff')
+            file_type: String - format in which to export the data. Must be either 'tif' or 'fits' (default is 'tif')
 
         Raises:
             IOError if the folder does not exist
             KeyError if data_type can not be found in the list ['normalized','sample','ob','df']
 
         """
         if not os.path.exists(folder):
@@ -837,39 +812,39 @@
                                       suffix=file_type)
 
         self.__export_data(data=data,
                            metadata=metadata,
                            output_file_names=self._export_file_name,
                            suffix=file_type)
 
-    def __export_data(self, data=[], metadata=[], output_file_names=[], suffix='tiff'):
+    def __export_data(self, data=[], metadata=[], output_file_names=[], suffix='tif'):
         """save the list of files with the data specified
         
         Parameters:
             data: numpy array that contains the array of data to save (default [])
             output_file_names: numpy array of string of full file names (default [])
-            suffix: String - format in which the file will be created (default 'tiff')
+            suffix: String - format in which the file will be created (default 'tif')
         """
         name_data_metadata_array = zip(output_file_names, data, metadata)
         for _file_name, _data, _metadata in name_data_metadata_array:
-            if suffix == 'tiff':
-                make_tiff(data=_data, metadata=_metadata, file_name=_file_name)
+            if suffix == 'tif':
+                make_tif(data=_data, metadata=_metadata, file_name=_file_name)
             elif suffix == 'fits':
                 make_fits(data=_data, file_name=_file_name)
 
     def __create_list_file_names(self, initial_list=[], output_folder='', prefix='', suffix=''):
         """create a list of the new file name used to export the images
         
         Parameters:
             initial_list: array of full file name
-               ex: ['/users/me/image001.tiff',/users/me/image002.tiff',/users/me/image003.tiff']
+               ex: ['/users/me/image001.tif',/users/me/image002.tif',/users/me/image003.tif']
             output_folder: String (default is ./ as specified by calling function) where we want to create the data
             prefix: String. what to add to the output file name in front of base name
-                ex: 'normalized' will produce 'normalized_image001.tiff'
-            suffix: String. extension to file. 'tiff' for TIFF and 'fits' for FITS
+                ex: 'normalized' will produce 'normalized_image001.tif'
+            suffix: String. extension to file. 'tif' for TIFF and 'fits' for FITS
         """
         _base_name = [os.path.basename(_file) for _file in initial_list]
         _raw_name = [os.path.splitext(_file)[0] for _file in _base_name]
         _prefix = ''
         if prefix:
             _prefix = prefix + '_'
         full_file_names = [os.path.join(output_folder, _prefix + _file + '.' + suffix) for _file in _raw_name]
```

### Comparing `NeuNorm-1.5.3/NeuNorm/roi.py` & `NeuNorm-1.6.1/NeuNorm/roi.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/NeuNorm.egg-info/PKG-INFO` & `NeuNorm-1.6.1/NeuNorm.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: NeuNorm
-Version: 1.5.3
+Version: 1.6.1
 Summary: neutron normalization data
 Home-page: https://github.com/ornlneutronimaging/NeuNorm
 Author: Jean Bilheux
 Author-email: bilheuxjm@ornl.gov
 License: BSD
 Keywords: neutron normalization imaging
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE.txt
 
 See the README.md file on GitHub for more information
-
```

### Comparing `NeuNorm-1.5.3/NeuNorm.egg-info/SOURCES.txt` & `NeuNorm-1.6.1/NeuNorm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 README.md
 clean.sh
 codecov.yml
 coverage.xml
 readthedocs.yml
 setup.cfg
 setup.py
+ImagingReso.egg-info/PKG-INFO
+ImagingReso.egg-info/SOURCES.txt
+ImagingReso.egg-info/dependency_links.txt
+ImagingReso.egg-info/requires.txt
+ImagingReso.egg-info/top_level.txt
 NeuNorm/__init__.py
 NeuNorm/_utilities.py
 NeuNorm/exporter.py
 NeuNorm/loader.py
 NeuNorm/normalization.py
 NeuNorm/roi.py
 NeuNorm.egg-info/PKG-INFO
@@ -202,33 +207,21 @@
 tests/data/fits/ob/ob002.fits
 tests/data/fits/ob/ob003.fits
 tests/data/fits/sample/image001.fits
 tests/data/fits/sample/image002.fits
 tests/data/fits/sample/image003.fits
 tests/data/fits/test_roi/ob.fits
 tests/data/fits/test_roi/sample.fits
-tests/data/fits/tof/ob/ob_001.fits
-tests/data/fits/tof/ob/ob_002.fits
-tests/data/fits/tof/ob/ob_003.fits
-tests/data/fits/tof/sample/sample_001.fits
-tests/data/fits/tof/sample/sample_002.fits
-tests/data/fits/tof/sample/sample_003.fits
 tests/data/hdf5/dump_file.hdf5
 tests/data/tif/df/df001.tif
 tests/data/tif/df/df002.tif
 tests/data/tif/df/df003.tif
 tests/data/tif/ob/ob001.tif
 tests/data/tif/ob/ob002.tif
 tests/data/tif/ob/ob003.tif
 tests/data/tif/sample/image001.tif
 tests/data/tif/sample/image002.tif
 tests/data/tif/sample/image003.tif
 tests/data/tif/sample_with_gamma/image001.tif
 tests/data/tif/special_ob/ob_0001_2rois.tiff
 tests/data/tif/special_sample/image_0001_2rois.tiff
-tests/data/tif/special_sample/image_0001_roi_no_ob.tiff
-tests/data/tif/tof/ob/ob_01.tiff
-tests/data/tif/tof/ob/ob_02.tiff
-tests/data/tif/tof/ob/ob_03.tiff
-tests/data/tif/tof/sample/tof_01.tiff
-tests/data/tif/tof/sample/tof_02.tiff
-tests/data/tif/tof/sample/tof_03.tiff
+tests/data/tif/special_sample/image_0001_roi_no_ob.tiff
```

### Comparing `NeuNorm-1.5.3/PKG-INFO` & `NeuNorm-1.6.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: NeuNorm
-Version: 1.5.3
+Version: 1.6.1
 Summary: neutron normalization data
 Home-page: https://github.com/ornlneutronimaging/NeuNorm
 Author: Jean Bilheux
 Author-email: bilheuxjm@ornl.gov
 License: BSD
 Keywords: neutron normalization imaging
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE.txt
 
 See the README.md file on GitHub for more information
-
```

### Comparing `NeuNorm-1.5.3/README.md` & `NeuNorm-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/conda-recipes/meta.yaml` & `NeuNorm-1.6.1/conda-recipes/meta.yaml`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/coverage.xml` & `NeuNorm-1.6.1/coverage.xml`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/df/DC0000.tif` & `NeuNorm-1.6.1/data/df/DC0000.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/df/DC0001.tif` & `NeuNorm-1.6.1/data/df/DC0001.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/df/DC0002.tif` & `NeuNorm-1.6.1/data/df/DC0002.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0001.tif` & `NeuNorm-1.6.1/data/ob/0001.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0002.tif` & `NeuNorm-1.6.1/data/ob/0002.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0003.tif` & `NeuNorm-1.6.1/data/ob/0003.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0004.tif` & `NeuNorm-1.6.1/data/ob/0004.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0005.tif` & `NeuNorm-1.6.1/data/ob/0005.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0006.tif` & `NeuNorm-1.6.1/data/ob/0006.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0007.tif` & `NeuNorm-1.6.1/data/ob/0007.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0008.tif` & `NeuNorm-1.6.1/data/ob/0008.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0009.tif` & `NeuNorm-1.6.1/data/ob/0009.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0010.tif` & `NeuNorm-1.6.1/data/ob/0010.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0011.tif` & `NeuNorm-1.6.1/data/ob/0011.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0012.tif` & `NeuNorm-1.6.1/data/ob/0012.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0013.tif` & `NeuNorm-1.6.1/data/ob/0013.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0014.tif` & `NeuNorm-1.6.1/data/ob/0014.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/ob/0015.tif` & `NeuNorm-1.6.1/data/ob/0015.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0002.tif` & `NeuNorm-1.6.1/data/sample/0002.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0003.tif` & `NeuNorm-1.6.1/data/sample/0003.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0004.tif` & `NeuNorm-1.6.1/data/sample/0004.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0005.tif` & `NeuNorm-1.6.1/data/sample/0005.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0006.tif` & `NeuNorm-1.6.1/data/sample/0006.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0007.tif` & `NeuNorm-1.6.1/data/sample/0007.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0008.tif` & `NeuNorm-1.6.1/data/sample/0008.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0009.tif` & `NeuNorm-1.6.1/data/sample/0009.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0010.tif` & `NeuNorm-1.6.1/data/sample/0010.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0011.tif` & `NeuNorm-1.6.1/data/sample/0011.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0012.tif` & `NeuNorm-1.6.1/data/sample/0012.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0013.tif` & `NeuNorm-1.6.1/data/sample/0013.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0014.tif` & `NeuNorm-1.6.1/data/sample/0014.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/data/sample/0015.tif` & `NeuNorm-1.6.1/data/sample/0015.tif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/Makefile` & `NeuNorm-1.6.1/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/cropping_data.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/cropping_data.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/dark_field_correction.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/dark_field_correction.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/environment.pickle` & `NeuNorm-1.6.1/documentation/build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/export_data.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/export_data.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/index.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/installation.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/loading.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/loading.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/normalization.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/normalization.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/notebook.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/notebook.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/retrieve_normalized_data.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/retrieve_normalized_data.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/tutorial_using_array_input.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/tutorial_using_array_input.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/.doctrees/tutorial_using_folder_input.doctree` & `NeuNorm-1.6.1/documentation/build/.doctrees/tutorial_using_folder_input.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/cropping_data.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/cropping_data.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/dark_field_correction.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/dark_field_correction.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/environment.pickle` & `NeuNorm-1.6.1/documentation/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/export_data.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/export_data.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/index.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/installation.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/loading.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/loading.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/normalization.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/normalization.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/notebook.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/notebook.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/retrieve_normalized_data.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/retrieve_normalized_data.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/tutorial_normalization_with_fewer_ob_than_sample.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/tutorial_using_array_input.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/tutorial_using_array_input.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/doctrees/tutorial_using_folder_input.doctree` & `NeuNorm-1.6.1/documentation/build/doctrees/tutorial_using_folder_input.doctree`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_images/progress_bar_loading.png` & `NeuNorm-1.6.1/documentation/build/html/_images/progress_bar_loading.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_images/progress_bar_normalization.png` & `NeuNorm-1.6.1/documentation/build/html/_images/progress_bar_normalization.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/cropping_data.rst.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/cropping_data.rst.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/index.rst.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/loading.rst.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/loading.rst.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/normalization.rst.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/normalization.rst.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/notebook.rst.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/notebook.rst.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/retrieve_normalized_data.rst.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/retrieve_normalized_data.rst.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/tutorial_normalization_with_fewer_ob_than_sample.ipynb.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/tutorial_normalization_with_fewer_ob_than_sample.ipynb.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/tutorial_using_array_input.ipynb.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/tutorial_using_array_input.ipynb.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_sources/tutorial_using_folder_input.ipynb.txt` & `NeuNorm-1.6.1/documentation/build/html/_sources/tutorial_using_folder_input.ipynb.txt`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/ajax-loader.gif` & `NeuNorm-1.6.1/documentation/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/basic.css` & `NeuNorm-1.6.1/documentation/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/comment-bright.png` & `NeuNorm-1.6.1/documentation/build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/comment-close.png` & `NeuNorm-1.6.1/documentation/build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/comment.png` & `NeuNorm-1.6.1/documentation/build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/css/badge_only.css` & `NeuNorm-1.6.1/documentation/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/css/theme.css` & `NeuNorm-1.6.1/documentation/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/doctools.js` & `NeuNorm-1.6.1/documentation/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/Inconsolata-Bold.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/Inconsolata-Regular.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/Lato-Bold.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/Lato-Regular.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/RobotoSlab-Bold.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/RobotoSlab-Regular.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.eot` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.svg` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.ttf` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/fonts/fontawesome-webfont.woff` & `NeuNorm-1.6.1/documentation/build/html/_static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/jquery-3.1.0.js` & `NeuNorm-1.6.1/documentation/build/html/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/jquery.js` & `NeuNorm-1.6.1/documentation/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/js/modernizr.min.js` & `NeuNorm-1.6.1/documentation/build/html/_static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/js/theme.js` & `NeuNorm-1.6.1/documentation/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/normalization_equation.png` & `NeuNorm-1.6.1/documentation/build/html/_static/normalization_equation.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/normalization_principle.png` & `NeuNorm-1.6.1/documentation/build/html/_static/normalization_principle.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/progress_bar_loading.png` & `NeuNorm-1.6.1/documentation/build/html/_static/progress_bar_loading.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/progress_bar_normalization.png` & `NeuNorm-1.6.1/documentation/build/html/_static/progress_bar_normalization.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/pygments.css` & `NeuNorm-1.6.1/documentation/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/searchtools.js` & `NeuNorm-1.6.1/documentation/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/underscore-1.3.1.js` & `NeuNorm-1.6.1/documentation/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/underscore.js` & `NeuNorm-1.6.1/documentation/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/_static/websupport.js` & `NeuNorm-1.6.1/documentation/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/cropping_data.html` & `NeuNorm-1.6.1/documentation/build/html/cropping_data.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/dark_field_correction.html` & `NeuNorm-1.6.1/documentation/build/html/dark_field_correction.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/export_data.html` & `NeuNorm-1.6.1/documentation/build/html/export_data.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/genindex.html` & `NeuNorm-1.6.1/documentation/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/index.html` & `NeuNorm-1.6.1/documentation/build/html/index.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/installation.html` & `NeuNorm-1.6.1/documentation/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/loading.html` & `NeuNorm-1.6.1/documentation/build/html/loading.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/normalization.html` & `NeuNorm-1.6.1/documentation/build/html/normalization.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/notebook.html` & `NeuNorm-1.6.1/documentation/build/html/notebook.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/objects.inv` & `NeuNorm-1.6.1/documentation/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/retrieve_normalized_data.html` & `NeuNorm-1.6.1/documentation/build/html/retrieve_normalized_data.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/search.html` & `NeuNorm-1.6.1/documentation/build/html/search.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/searchindex.js` & `NeuNorm-1.6.1/documentation/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/tutorial_normalization_with_fewer_ob_than_sample.html` & `NeuNorm-1.6.1/documentation/build/html/tutorial_normalization_with_fewer_ob_than_sample.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/tutorial_using_array_input.html` & `NeuNorm-1.6.1/documentation/build/html/tutorial_using_array_input.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/build/html/tutorial_using_folder_input.html` & `NeuNorm-1.6.1/documentation/build/html/tutorial_using_folder_input.html`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/_static/normalization_equation.png` & `NeuNorm-1.6.1/documentation/source/_static/normalization_equation.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/_static/normalization_principle.png` & `NeuNorm-1.6.1/documentation/source/_static/normalization_principle.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/_static/progress_bar_loading.png` & `NeuNorm-1.6.1/documentation/source/_static/progress_bar_loading.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/_static/progress_bar_normalization.png` & `NeuNorm-1.6.1/documentation/source/_static/progress_bar_normalization.png`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/conf.py` & `NeuNorm-1.6.1/documentation/source/conf.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/cropping_data.rst` & `NeuNorm-1.6.1/documentation/source/cropping_data.rst`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/index.rst` & `NeuNorm-1.6.1/documentation/source/index.rst`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/loading.rst` & `NeuNorm-1.6.1/documentation/source/loading.rst`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/normalization.rst` & `NeuNorm-1.6.1/documentation/source/normalization.rst`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/notebook.rst` & `NeuNorm-1.6.1/documentation/source/notebook.rst`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/retrieve_normalized_data.rst` & `NeuNorm-1.6.1/documentation/source/retrieve_normalized_data.rst`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/tutorial_normalization_with_fewer_ob_than_sample.ipynb` & `NeuNorm-1.6.1/documentation/source/tutorial_normalization_with_fewer_ob_than_sample.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/tutorial_using_array_input.ipynb` & `NeuNorm-1.6.1/documentation/source/tutorial_using_array_input.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/documentation/source/tutorial_using_folder_input.ipynb` & `NeuNorm-1.6.1/documentation/source/tutorial_using_folder_input.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/debugging_multi_roi_bug.ipynb` & `NeuNorm-1.6.1/notebooks/debugging_multi_roi_bug.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/ipts-16259.ipynb` & `NeuNorm-1.6.1/notebooks/ipts-16259.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/notebook_display_with_time_estimation.ipynb` & `NeuNorm-1.6.1/notebooks/notebook_display_with_time_estimation.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/testing_new_auto_gamma_filtering.ipynb` & `NeuNorm-1.6.1/notebooks/testing_new_auto_gamma_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/tutorial_normalization_with_fewer_ob_than_sample.ipynb` & `NeuNorm-1.6.1/notebooks/tutorial_normalization_with_fewer_ob_than_sample.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/tutorial_normalization_with_fewer_ob_than_sample_MAYBE_BUG.ipynb` & `NeuNorm-1.6.1/notebooks/tutorial_normalization_with_fewer_ob_than_sample_MAYBE_BUG.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/tutorial_using_array_input.ipynb` & `NeuNorm-1.6.1/notebooks/tutorial_using_array_input.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/tutorial_using_array_input_and_export_array.ipynb` & `NeuNorm-1.6.1/notebooks/tutorial_using_array_input_and_export_array.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/tutorial_using_array_input_and_several_roi.ipynb` & `NeuNorm-1.6.1/notebooks/tutorial_using_array_input_and_several_roi.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/notebooks/tutorial_using_folder_input.ipynb` & `NeuNorm-1.6.1/notebooks/tutorial_using_folder_input.ipynb`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/paper/paper.bib` & `NeuNorm-1.6.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/paper/paper.md` & `NeuNorm-1.6.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/setup.py` & `NeuNorm-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/NeuNorm/cropping_test.py` & `NeuNorm-1.6.1/tests/NeuNorm/cropping_test.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/NeuNorm/export_test.py` & `NeuNorm-1.6.1/tests/NeuNorm/export_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,26 @@
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
 
         # OB
         o_norm.export(folder=self.export_folder, data_type='ob') 
         _output_file_name_0 = o_norm._export_file_name[0]
         
         _file_name_0 = os.path.basename(o_norm.data['ob']['file_name'][0])
-        _new_file_name = os.path.splitext(_file_name_0)[0] + '.tiff'
+        _new_file_name = os.path.splitext(_file_name_0)[0] + '.tif'
         _expected_file_name_0 = os.path.join(self.export_folder, _new_file_name)
         
         self.assertTrue(_expected_file_name_0 == _output_file_name_0)
         
         # Normalized
         o_norm.normalization()
         o_norm.export(folder=self.export_folder, data_type='normalized')
         _output_file_name_0 = o_norm._export_file_name[0]
     
         _file_name_0 = os.path.basename(o_norm.data['sample']['file_name'][0])
-        _new_file_name = 'normalized_' + os.path.splitext(_file_name_0)[0] + '.tiff'
+        _new_file_name = 'normalized_' + os.path.splitext(_file_name_0)[0] + '.tif'
         _expected_file_name_0 = os.path.join(self.export_folder, _new_file_name)
         self.assertTrue(_expected_file_name_0 == _output_file_name_0)        
         
     def test_export_works_for_tif(self):
         '''assert the file created is correct for tif images'''
         sample_path = self.data_path + '/tif/sample'
         o_norm = Normalization()
```

### Comparing `NeuNorm-1.5.3/tests/NeuNorm/loading_test.py` & `NeuNorm-1.6.1/tests/NeuNorm/loading_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,23 +249,19 @@
         """assert gamma filtering works"""
         path = self.data_path + '/tif/sample_with_gamma/'
 
         # gamma filter is True
         o_norm = Normalization()
         o_norm.load(folder=path, data_type='sample', manual_gamma_filter=True, auto_gamma_filter=False)
         _expected_sample = np.ones((5, 5))
-        _expected_sample[0, 0] = 4
+        _expected_sample[0, 0] = 0.375
         _expected_sample[:, 2] = 2
         _expected_sample[:, 3] = 3
         _expected_sample[:, 4] = 4
         _returned_sample = o_norm.data['sample']['data']
-
-        print(f"_expected_sample: {_expected_sample}")
-        print(f"_returned_sample: {_returned_sample}")
-
         self.assertTrue((_expected_sample == _returned_sample).all())
         
         # gamma filter is False
         o_norm = Normalization()
         o_norm.load(folder=path, data_type='sample', manual_gamma_filter=False, auto_gamma_filter=False)
         _expected_sample = np.ones((5, 5))
         _expected_sample[0, 0] = 1000
```

### Comparing `NeuNorm-1.5.3/tests/NeuNorm/normalizing_test.py` & `NeuNorm-1.6.1/tests/NeuNorm/normalizing_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 import numpy as np
 import os
 from PIL import Image
 
 from NeuNorm.normalization import Normalization
 from NeuNorm.roi import ROI
-from NeuNorm import DataType
 
 
 class TestNormalization:
 
     def setup_method(self):
         _file_path = os.path.dirname(__file__)
         self.data_path = os.path.abspath(os.path.join(_file_path, '../data/'))
@@ -17,129 +16,129 @@
     def test_loading_list_of_files(self):
         """assert initialization using list of files"""
         list_files = [self.data_path + '/tif/sample/image001.tif',
                       self.data_path + '/tif/sample/image002.tif',
                       self.data_path + '/tif/sample/image003.tif']
         o_norm = Normalization()
         o_norm.load(file=list_files, auto_gamma_filter=False)
-        data_returned = o_norm.data[DataType.sample]['data']
+        data_returned = o_norm.data['sample']['data']
         assert (3, 5, 5) == np.shape(data_returned)
-
+        
     def test_initialization_using_array_with_data(self):
         """assert initialization using arrays with data"""
         sample_01 = self.data_path + '/tif/sample/image001.tif'
         sample_02 = self.data_path + '/tif/sample/image002.tif'
         data = []
         data.append(np.asarray(Image.open(sample_01)))
         data.append(np.asarray(Image.open(sample_02)))
         o_norm = Normalization()
         o_norm.load(data=data, auto_gamma_filter=False)
 
-        data_returned = o_norm.data[DataType.sample]['data']
+        data_returned = o_norm.data['sample']['data']
         assert (2, 5, 5) == np.shape(data_returned)
-
+        
     def test_initialization_using_array_with_data_one_by_one(self):
         """assert initialization using arrays with data one by one"""
         o_norm = Normalization()
 
         sample_01 = self.data_path + '/tif/sample/image001.tif'
         _data = np.asarray(Image.open(sample_01))
         o_norm.load(data=_data, auto_gamma_filter=False)
-
+        
         sample_02 = self.data_path + '/tif/sample/image002.tif'
         _data = np.asarray(Image.open(sample_01))
         o_norm.load(data=_data, auto_gamma_filter=False)
 
-        data_returned = o_norm.data[DataType.sample]['data']
+        data_returned = o_norm.data['sample']['data']
         assert (2, 5, 5) == np.shape(data_returned)
 
     def test_initialization_using_array_with_ob(self):
         """assert initialization using arrays with ob"""
         ob_01 = self.data_path + '/tif/ob/ob001.tif'
         ob_02 = self.data_path + '/tif/ob/ob002.tif'
         data = []
         data.append(np.asarray(Image.open(ob_01)))
         data.append(np.asarray(Image.open(ob_02)))
         o_norm = Normalization()
         o_norm.load(data=data, data_type='ob', auto_gamma_filter=False)
 
         data_returned = o_norm.data['ob']['data']
         assert (2, 5, 5) == np.shape(data_returned)
-
+        
     def test_normalization_raises_error_if_no_ob_or_sample(self):
         """assert error raises when no ob or sample provided"""
         path = self.data_path + '/tif/sample'
         o_norm = Normalization()
-        o_norm.load(folder=path, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(folder=path, data_type='sample', auto_gamma_filter=False)
         with pytest.raises(IOError):
             o_norm.normalization()
-
+        
         path = self.data_path + '/tif/ob'
         o_norm = Normalization()
         o_norm.load(folder=path, data_type='ob', auto_gamma_filter=False)
         with pytest.raises(IOError):
             o_norm.normalization()
-
+        
         sample_path = self.data_path + '/tif/sample'
         ob_path = self.data_path + '/tif/ob'
         o_norm = Normalization()
-        o_norm.load(folder=sample_path, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(folder=sample_path, data_type='sample', auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
         assert o_norm.normalization()
-
+ 
     def test_normalization_ran_only_once(self):
         """assert normalization is only once if force switch not turn on"""
         sample_tif_folder = self.data_path + '/tif/sample'
         ob_tif_folder = self.data_path + '/tif/ob'
-
+    
         # testing sample with norm_roi
         o_norm = Normalization()
         o_norm.load(folder=sample_tif_folder, auto_gamma_filter=False)
         o_norm.load(folder=ob_tif_folder, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=0, y0=0, x1=3, y1=2)
         o_norm.normalization(roi=roi)
-        _returned_first_time = o_norm.data[DataType.sample]['data'][0]
+        _returned_first_time = o_norm.data['sample']['data'][0]
         o_norm.normalization(roi=roi)
-        _returned_second_time = o_norm.data[DataType.sample]['data'][0]
+        _returned_second_time = o_norm.data['sample']['data'][0]
         assert (_returned_first_time == _returned_second_time).all()
 
     def test_normalization_ran_twice_with_force_flag(self):
         """assert normalization can be ran twice using force flag"""
         sample_tif_folder = self.data_path + '/tif/sample'
         ob_tif_folder = self.data_path + '/tif/ob'
-
+    
         # testing sample with norm_roi
         o_norm = Normalization()
         o_norm.load(folder=sample_tif_folder, auto_gamma_filter=False)
         o_norm.load(folder=ob_tif_folder, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=0, y0=0, x1=3, y1=2)
         o_norm.normalization(roi=roi)
-        _returned_first_time = o_norm.data[DataType.sample]['data'][0]
+        _returned_first_time = o_norm.data['sample']['data'][0]
         roi = ROI(x0=0, y0=0, x1=2, y1=3)
         o_norm.normalization(roi=roi, force=True)
-        _returned_second_time = o_norm.data[DataType.sample]['data'][0]
+        _returned_second_time = o_norm.data['sample']['data'][0]
         assert not ((_returned_first_time == _returned_second_time).all())
-
+  
     def test_normalization_works_if_input_arrays_are_type_int(self):
         """assert normalization works when input arrays are type int"""
         o_norm = Normalization()
-
+        
         sample_01 = self.data_path + '/tif/sample/image001.tif'
         _data = np.asarray(Image.open(sample_01), dtype=int)
         o_norm.load(data=_data, auto_gamma_filter=False)
-
+        
         sample_02 = self.data_path + '/tif/sample/image002.tif'
         _data = np.asarray(Image.open(sample_01), dtype=int)
         o_norm.load(data=_data, auto_gamma_filter=False)
 
         ob_01 = self.data_path + '/tif/ob/ob001.tif'
         _data = np.asarray(Image.open(ob_01), dtype=int)
-        _data[0, 0] = 0
+        _data[0,0] = 0
         o_norm.load(data=_data, data_type='ob', auto_gamma_filter=False)
-
+    
         ob_02 = self.data_path + '/tif/ob/ob002.tif'
         _data = np.asarray(Image.open(ob_01), dtype=int)
         o_norm.load(data=_data, data_type='ob', auto_gamma_filter=False)
 
         o_norm.normalization()
 
     def test_normalization_works(self):
@@ -148,153 +147,134 @@
         ob_tif_folder = self.data_path + '/tif/ob'
 
         # testing sample with norm_roi
         o_norm = Normalization()
         o_norm.load(folder=sample_tif_folder, auto_gamma_filter=False)
         o_norm.load(folder=ob_tif_folder, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=0, y0=0, x1=3, y1=2)
-        _sample = o_norm.data[DataType.sample]['data'][0]
-        _expected = _sample / np.median(_sample[0:3, 0:4])
+        _sample = o_norm.data['sample']['data'][0]
+        _expected = _sample / np.mean(_sample[0:3, 0:4])
         o_norm.normalization(roi=roi)
-        _returned = o_norm.data[DataType.sample]['data'][0]
-
+        _returned = o_norm.data['sample']['data'][0]
         assert (_expected == _returned).all()
 
         # testing sample without norm_roi
         o_norm1 = Normalization()
         o_norm1.load(folder=sample_tif_folder, auto_gamma_filter=False)
         o_norm1.load(folder=ob_tif_folder, data_type='ob', auto_gamma_filter=False)
-        _expected = o_norm1.data[DataType.sample]['data'][0]
+        _expected = o_norm1.data['sample']['data'][0]
         o_norm1.normalization()
-        _returned = o_norm1.data[DataType.sample]['data'][0]
+        _returned = o_norm1.data['sample']['data'][0]
         assert (_expected == _returned).all()
-
+        
         # testing ob with norm_roi
         o_norm = Normalization()
         o_norm.load(folder=sample_tif_folder, auto_gamma_filter=False)
         o_norm.load(folder=ob_tif_folder, data_type='ob', auto_gamma_filter=False)
         norm_roi = ROI(x0=0, y0=0, x1=3, y1=2)
         o_norm.normalization(roi=norm_roi)
         _ob = o_norm.data['ob']['data'][0]
-        _expected = _ob / np.median(_ob[0:3, 0:4])
+        _expected = _ob / np.mean(_ob[0:3, 0:4])
         _returned = o_norm.data['ob']['data'][0]
         assert (_expected == _returned).all()
-
+        
         # testing ob without norm_roi
         o_norm = Normalization()
         o_norm.load(folder=sample_tif_folder, auto_gamma_filter=False)
         o_norm.load(folder=ob_tif_folder, data_type='ob', auto_gamma_filter=False)
         _expected = o_norm.data['ob']['data'][0]
         o_norm.normalization()
         _returned = o_norm.data['ob']['data'][0]
         assert (_expected == _returned).all()
-
+  
     def test_normalization_with_same_ob_and_sample_but_forced_mean_ob(self):
         """assert normalization with same ob and sample number of files force to use mean ob when flag used"""
-        samples_path = self.data_path + '/tif/sample/'  # 3 files
+        samples_path =  self.data_path + '/tif/sample/' # 3 files
         ob1 = self.data_path + '/tif/ob/ob001.tif'
         ob2 = self.data_path + '/tif/ob/ob002.tif'
         ob3 = self.data_path + '/tif/ob/ob003.tif'
         o_norm = Normalization()
         o_norm.load(folder=samples_path, auto_gamma_filter=False)
         o_norm.load(file=[ob1, ob2, ob3], data_type='ob', auto_gamma_filter=False)
         o_norm.normalization(force_mean_ob=True)
-        expected_normalized_array = np.ones((5, 5))
-        expected_normalized_array[:, 2] = 2
-        expected_normalized_array[:, 3] = 3
-        expected_normalized_array[:, 4] = 4
-        assert (o_norm.data['normalized'][0] == expected_normalized_array).all()
-
-    def test_normalization_with_same_ob_and_sample_but_forced_median_ob(self):
-        """assert normalization with same ob and sample number of files force to use mean ob when flag used"""
-        samples_path = self.data_path + '/tif/sample/'  # 3 files
-        ob1 = self.data_path + '/tif/ob/ob001.tif'
-        ob2 = self.data_path + '/tif/ob/ob002.tif'
-        ob3 = self.data_path + '/tif/ob/ob003.tif'
-        o_norm = Normalization()
-        o_norm.load(folder=samples_path, auto_gamma_filter=False)
-        o_norm.load(file=[ob1, ob2, ob3], data_type='ob', auto_gamma_filter=False)
-        # double value of last OB
-        o_norm.data['ob']['data'][2] *= 3
-        o_norm.normalization(force_median_ob=True)
-        expected_normalized_array = np.ones((5, 5))
-        expected_normalized_array[:, 2] = 2
-        expected_normalized_array[:, 3] = 3
-        expected_normalized_array[:, 4] = 4
+        expected_normalized_array = np.ones((5,5))
+        expected_normalized_array[:,2] = 2
+        expected_normalized_array[:,3] = 3
+        expected_normalized_array[:,4] = 4
         assert (o_norm.data['normalized'][0] == expected_normalized_array).all()
 
     def test_normalization_with_fewer_ob_than_sample_works(self):
         """assert normalization works when number of ob and sample is different"""
         samples_path = self.data_path + '/tif/sample/'  # 3 files
         ob1 = self.data_path + '/tif/ob/ob001.tif'
-        ob2 = self.data_path + '/tif/ob/ob002.tif'
+        ob2 = self.data_path + '/tif/ob/ob002.tif' 
         df1 = self.data_path + '/tif/df/df001.tif'
         o_norm = Normalization()
         o_norm.load(folder=samples_path, auto_gamma_filter=False)
         o_norm.load(file=[ob1, ob2], data_type='ob', auto_gamma_filter=False)
-        o_norm.load(file=df1, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(file=df1, data_type='df', auto_gamma_filter=False)
         o_norm.df_correction()
         o_norm.normalization()
         expected_normalized_array = np.zeros((5, 5))
         expected_normalized_array[0, 0] = 1
         assert (o_norm.data['normalized'] == expected_normalized_array).all()
 
     def test_nbr_data_files_same_after_normalization_by_list_roi(self):
         """assert the number of data files is the same after normalization by a list of ROI"""
-        samples_path = self.data_path + '/tif/sample/'  # 3 files
+        samples_path =  self.data_path + '/tif/sample/' # 3 files
         ob1 = self.data_path + '/tif/ob/ob001.tif'
         ob2 = self.data_path + '/tif/ob/ob002.tif'
         o_norm = Normalization()
         o_norm.load(folder=samples_path, auto_gamma_filter=False)
         o_norm.load(file=[ob1, ob2], data_type='ob', auto_gamma_filter=False)
-        _roi1 = ROI(x0=0, y0=0, x1=2, y1=2)
-        _roi2 = ROI(x0=1, y0=1, x1=3, y1=3)
+        _roi1 = ROI(x0=0,y0=0,x1=2,y1=2)
+        _roi2 = ROI(x0=1,y0=1,x1=3,y1=3)
         _list_roi = [_roi1, _roi2]
-        nbr_data_before = len(o_norm.data[DataType.sample]['data'])
+        nbr_data_before = len(o_norm.data['sample']['data'])
         o_norm.normalization(roi=_list_roi)
-        nbr_data_after = len(o_norm.data[DataType.sample]['data'])
+        nbr_data_after = len(o_norm.data['sample']['data'])
         assert nbr_data_after == nbr_data_before
 
     def test_normalization_works_with_only_1_df(self):
         """assert using 1 df in normalization works"""
-        samples_path = self.data_path + '/tif/sample/'  # 3 files
+        samples_path =  self.data_path + '/tif/sample/' # 3 files
         ob1 = self.data_path + '/tif/ob/ob001.tif'
         ob2 = self.data_path + '/tif/ob/ob002.tif'
         df1 = self.data_path + '/tif/df/df001.tif'
         o_norm = Normalization()
         o_norm.load(folder=samples_path, auto_gamma_filter=False)
         o_norm.load(file=[ob1, ob2], data_type='ob', auto_gamma_filter=False)
-        o_norm.load(file=df1, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(file=df1, data_type='df', auto_gamma_filter=False)
         o_norm.df_correction()
         _roi1 = ROI(x0=0, y0=0, x1=2, y1=2)
         _roi2 = ROI(x0=1, y0=1, x1=3, y1=3)
         _list_roi = [_roi1, _roi2]
-        nbr_data_before = len(o_norm.data[DataType.sample]['data'])
+        nbr_data_before = len(o_norm.data['sample']['data'])
         o_norm.normalization(roi=_list_roi)
-        nbr_data_after = len(o_norm.data[DataType.sample]['data'])
+        nbr_data_after = len(o_norm.data['sample']['data'])
         assert nbr_data_after == nbr_data_before
 
     def test_normalization_works_with_2_dfs(self):
         """assert using 2 df in normalization works"""
         samples_path = self.data_path + '/tif/sample/'  # 3 files
         ob1 = self.data_path + '/tif/ob/ob001.tif'
         ob2 = self.data_path + '/tif/ob/ob002.tif'
         df1 = self.data_path + '/tif/df/df001.tif'
         df2 = self.data_path + '/tif/df/df002.tif'
         o_norm = Normalization()
         o_norm.load(folder=samples_path, auto_gamma_filter=False)
         o_norm.load(file=[ob1, ob2], data_type='ob', auto_gamma_filter=False)
-        o_norm.load(file=[df1, df2], data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(file=[df1, df2], data_type='df', auto_gamma_filter=False)
         o_norm.df_correction()
         _roi1 = ROI(x0=0, y0=0, x1=2, y1=2)
         _roi2 = ROI(x0=1, y0=1, x1=3, y1=3)
         _list_roi = [_roi1, _roi2]
-        nbr_data_before = len(o_norm.data[DataType.sample]['data'])
+        nbr_data_before = len(o_norm.data['sample']['data'])
         o_norm.normalization(roi=_list_roi)
-        nbr_data_after = len(o_norm.data[DataType.sample]['data'])
+        nbr_data_after = len(o_norm.data['sample']['data'])
         assert nbr_data_after == nbr_data_before
 
     def test_normalization_works_with_1_roi_given_as_a_list(self):
         """Make sure the normalization works when 2 ROI are used"""
         sample = self.data_path + '/fits/test_roi/sample.fits'
         ob = self.data_path + '/fits/test_roi/ob.fits'
         _roi = ROI(x0=0, y0=0, x1=1, y1=2)
@@ -311,252 +291,222 @@
 
         height, width = np.shape(expected_normalized_data)
         for _h in np.arange(height):
             for _w in np.arange(width):
                 assert expected_normalized_data[_h, _w] == pytest.approx(normalized_data[_h, _w], 1e-5)
 
 
-class TestOBMedian:
-
-    def setup_method(self):
-        _file_path = os.path.dirname(__file__)
-        self.data_path = os.path.abspath(os.path.join(_file_path, '../data/'))
-
-    def test_ob_median(self):
-        """make sure combining the OB will use the median"""
-
-        # without normalization roi
-        sample_path = self.data_path + '/tif/sample'
-        ob_path = self.data_path + '/tif/ob'
-        df_path = self.data_path + '/tif/df'
-
-        o_norm = Normalization()
-        o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-
-        # replace last ob with crazy one, that shouldn't be use when using median (instead of mean)
-        o_norm.data['ob']['data'][-1] = np.ones((5, 5)) * 1000
-
-        o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
-        o_norm.normalization(force_median_ob=True)
-        _norm_expected = np.ones((5, 5))
-        _norm_expected[:, 2] = 2
-        _norm_expected[:, 3] = 3
-        _norm_expected[:, 4] = 4
-        _norm_returned = o_norm.data['normalized']
-        assert (_norm_expected == _norm_returned).all()
-
 
 class TestDFCorrection:
 
     def setup_method(self):
         _file_path = os.path.dirname(__file__)
-        self.data_path = os.path.abspath(os.path.join(_file_path, '../data/'))
-
+        self.data_path = os.path.abspath(os.path.join(_file_path, '../data/'))  
+        
     def test_df_correction_when_no_df(self):
         """assert sample and ob are inchanged if df is empty"""
 
         # sample
         path = self.data_path + '/tif/sample'
         o_norm = Normalization()
-        o_norm.load(folder=path, data_type=DataType.sample, auto_gamma_filter=False)
-        data_before = o_norm.data[DataType.sample]['data'][0]
+        o_norm.load(folder=path, data_type='sample', auto_gamma_filter=False)
+        data_before = o_norm.data['sample']['data'][0]
         o_norm.df_correction()
-        data_after = o_norm.data[DataType.sample]['data'][0]
+        data_after = o_norm.data['sample']['data'][0]
         assert (data_before == data_after).all()
-
-        # ob
+        
+        #ob
         path = self.data_path + '/tif/ob'
         o_norm = Normalization()
         o_norm.load(folder=path, data_type='ob', auto_gamma_filter=False)
         data_before = o_norm.data['ob']['data'][0]
         o_norm.df_correction()
         data_after = o_norm.data['ob']['data'][0]
         assert (data_before == data_after).all()
-
+        
     def test_df_fails_when_not_identical_data_shape(self):
         o_norm = Normalization()
-        sample_1 = np.ones([5, 5])
-        df_1 = np.ones([6, 6])
-        o_norm.data[DataType.sample]['data'] = sample_1
-        o_norm.data[DataType.df]['data'] = df_1
+        sample_1 = np.ones([5,5])
+        df_1 = np.ones([6,6])
+        o_norm.data['sample']['data'] = sample_1
+        o_norm.data['df']['data'] = df_1
         with pytest.raises(IOError):
             o_norm.df_correction()
-
+        
         o_norm = Normalization()
-        ob_1 = np.ones([6, 6])
+        ob_1 = np.ones([6,6])
         o_norm.data['ob']['data'] = sample_1
-        o_norm.data[DataType.df]['data'] = ob_1
+        o_norm.data['df']['data'] = ob_1
         with pytest.raises(IOError):
             o_norm.df_correction()
 
     def test_df_averaging_only_run_the_first_time(self):
         """assert the average_df is only run the first time the df_correction is run"""
         sample_path = self.data_path + '/tif/sample/'
         ob_path = self.data_path + '/tif/ob/'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
         df_file_1 = self.data_path + '/tif/df/df002.tif'
         df_file_2 = self.data_path + '/tif/df/df003.tif'
-        o_norm.load(file=df_file_1, data_type=DataType.df, auto_gamma_filter=False)
-        o_norm.load(file=df_file_2, data_type=DataType.df, auto_gamma_filter=False)
-
-        df_average_data = o_norm.data[DataType.df]['data_average']
+        o_norm.load(file=df_file_1, data_type='df', auto_gamma_filter=False)
+        o_norm.load(file=df_file_2, data_type='df', auto_gamma_filter=False)
+    
+        df_average_data = o_norm.data['df']['data_average']
         assert not df_average_data
-
-        # sample
+    
+        #sample
         o_norm.df_correction()
-        df_average_data = o_norm.data[DataType.df]['data_average']
+        df_average_data = o_norm.data['df']['data_average']
         assert df_average_data.size != 0
-
-        # ob
+    
+        #ob
         o_norm.df_correction()
         expected_df_average = df_average_data
-        df_average = o_norm.data[DataType.df]['data_average']
+        df_average = o_norm.data['df']['data_average']
         assert (expected_df_average == df_average).all()
 
     def test_df_correction(self):
         """assert df corrction works"""
         sample_path = self.data_path + '/tif/sample/'
         ob_path = self.data_path + '/tif/ob/'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
         df_file_1 = self.data_path + '/tif/df/df002.tif'
         df_file_2 = self.data_path + '/tif/df/df003.tif'
-        o_norm.load(file=df_file_1, data_type=DataType.df, auto_gamma_filter=False)
-        o_norm.load(file=df_file_2, data_type=DataType.df, auto_gamma_filter=False)
-
-        # sample
-        o_norm.df_correction()
-        _expected_data = np.zeros([5, 5])
-        _expected_data[:, 2] = 1
-        _expected_data[:, 3] = 2
-        _expected_data[:, 4] = 3
-        _sample_data = o_norm.data[DataType.sample]['data'][0]
-        assert (_expected_data == o_norm.data[DataType.sample]['data'][0]).all()
-
-        # ob
-        _expected_data = np.zeros([5, 5])
+        o_norm.load(file=df_file_1, data_type='df', auto_gamma_filter=False)
+        o_norm.load(file=df_file_2, data_type='df', auto_gamma_filter=False)
+        
+        #sample
+        o_norm.df_correction()
+        _expected_data = np.zeros([5,5])
+        _expected_data[:,2] = 1
+        _expected_data[:,3] = 2
+        _expected_data[:,4] = 3       
+        _sample_data = o_norm.data['sample']['data'][0]
+        assert (_expected_data == o_norm.data['sample']['data'][0]).all()
+        
+        #ob
+        _expected_data = np.zeros([5,5])
         _ob_data = o_norm.data['ob']['data'][0]
         assert (_expected_data == _ob_data).all()
 
     def test_df_correction_locked_when_run_twice_without_force_flag(self):
         """assert df corrction run only one time if force flag is False"""
         sample_path = self.data_path + '/tif/sample/'
         ob_path = self.data_path + '/tif/ob/'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
         df_file_1 = self.data_path + '/tif/df/df002.tif'
         df_file_2 = self.data_path + '/tif/df/df003.tif'
-        o_norm.load(file=df_file_1, data_type=DataType.df, auto_gamma_filter=False)
-        o_norm.load(file=df_file_2, data_type=DataType.df, auto_gamma_filter=False)
-
+        o_norm.load(file=df_file_1, data_type='df', auto_gamma_filter=False)
+        o_norm.load(file=df_file_2, data_type='df', auto_gamma_filter=False)
+        
         # first iteration
         o_norm.df_correction()
-        _sample_first_run = o_norm.data[DataType.sample]['data'][0]
+        _sample_first_run = o_norm.data['sample']['data'][0]
         _ob_first_run = o_norm.data['ob']['data'][0]
-
+        
         # second iteration
         o_norm.df_correction()
-        _sample_second_run = o_norm.data[DataType.sample]['data'][0]
+        _sample_second_run = o_norm.data['sample']['data'][0]
         _ob_second_run = o_norm.data['ob']['data'][0]
-
+         
         assert (_sample_first_run == _sample_second_run).all()
         assert (_ob_first_run == _ob_second_run).all()
-
+         
     def test_df_correction_run_twice_with_force_flag(self):
         """assert df corrction run more than once with force flag"""
         sample_path = self.data_path + '/tif/sample/'
         ob_path = self.data_path + '/tif/ob/'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
         df_file_1 = self.data_path + '/tif/df/df002.tif'
         df_file_2 = self.data_path + '/tif/df/df003.tif'
-        o_norm.load(file=df_file_1, data_type=DataType.df, auto_gamma_filter=False)
-        o_norm.load(file=df_file_2, data_type=DataType.df, auto_gamma_filter=False)
-
+        o_norm.load(file=df_file_1, data_type='df', auto_gamma_filter=False)
+        o_norm.load(file=df_file_2, data_type='df', auto_gamma_filter=False)
+        
         # first iteration
         o_norm.df_correction()
-        _sample_first_run = o_norm.data[DataType.sample]['data'][0]
+        _sample_first_run = o_norm.data['sample']['data'][0]
         _ob_first_run = o_norm.data['ob']['data'][0]
-        _average_df = o_norm.data[DataType.df]['data_average']
-
+        _average_df = o_norm.data['df']['data_average']
+        
         # second iteration
         o_norm.df_correction(force=True)
-        _sample_second_run = o_norm.data[DataType.sample]['data'][0]
+        _sample_second_run = o_norm.data['sample']['data'][0]
         _ob_second_run = o_norm.data['ob']['data'][0]
 
         # expected
         _expected_sample_after_second_run = _sample_first_run - _average_df
         _expected_ob_after_second_run = _ob_first_run - _average_df
-
+         
         assert (_sample_second_run == _expected_sample_after_second_run).all()
         assert (_ob_second_run == _expected_ob_after_second_run).all()
-
-
+         
+        
 class TestApplyingROI:
 
     def setup_method(self):
         _file_path = os.path.dirname(__file__)
-        self.data_path = os.path.abspath(os.path.join(_file_path, '../data/'))
-
+        self.data_path = os.path.abspath(os.path.join(_file_path, '../data/'))       
+        
     def test_roi_type_in_normalization(self):
         """assert error is raised when type of norm roi are not ROI in normalization"""
         sample_tif_file = self.data_path + '/tif/sample/image001.tif'
         ob_tif_file = self.data_path + '/tif/ob/ob001.tif'
         o_norm = Normalization()
-        o_norm.load(file=sample_tif_file, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(file=sample_tif_file, data_type='sample', auto_gamma_filter=False)
         o_norm.load(file=ob_tif_file, data_type='ob', auto_gamma_filter=False)
-        roi = {'x0': 0, 'y0': 0, 'x1': 2, 'y1': 2}
+        roi = {'x0':0, 'y0':0, 'x1':2, 'y1':2}
         with pytest.raises(ValueError):
             o_norm.normalization(roi=roi)
-
+        
     def test_roi_fit_images(self):
         """assert norm roi do fit the images"""
         sample_tif_file = self.data_path + '/tif/sample/image001.tif'
         ob_tif_file = self.data_path + '/tif/ob/ob001.tif'
-
+        
         # x0 < 0 or x1 > image_width
         o_norm = Normalization()
-        o_norm.load(file=sample_tif_file, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(file=sample_tif_file, data_type='sample', auto_gamma_filter=False)
         o_norm.load(file=ob_tif_file, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=0, y0=0, x1=20, y1=4)
         with pytest.raises(ValueError):
             o_norm.normalization(roi=roi)
-
+       
         o_norm = Normalization()
-        o_norm.load(file=sample_tif_file, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(file=sample_tif_file, data_type='sample', auto_gamma_filter=False)
         o_norm.load(file=ob_tif_file, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=-1, y0=0, x1=4, y1=4)
         with pytest.raises(ValueError):
             o_norm.normalization(roi=roi)
-
+        
         # y0 < 0 or y1 > image_height
         o_norm = Normalization()
-        o_norm.load(file=sample_tif_file, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(file=sample_tif_file, data_type='sample', auto_gamma_filter=False)
         o_norm.load(file=ob_tif_file, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=0, y0=-1, x1=4, y1=4)
         with pytest.raises(ValueError):
             o_norm.normalization(roi=roi)
 
         # y1>image_height
         o_norm = Normalization()
-        o_norm.load(file=sample_tif_file, data_type=DataType.sample, auto_gamma_filter=False)
+        o_norm.load(file=sample_tif_file, data_type='sample', auto_gamma_filter=False)
         o_norm.load(file=ob_tif_file, data_type='ob', auto_gamma_filter=False)
         roi = ROI(x0=0, y0=0, x1=4, y1=20)
         with pytest.raises(ValueError):
             o_norm.normalization(roi=roi)
 
     def test_error_raised_when_data_shape_of_different_type_do_not_match(self):
         """assert shape of data must match to allow normalization"""
-
+        
         # sample and ob
         image1 = self.data_path + '/tif/sample/image001.tif'
         ob1 = self.data_path + '/different_format/ob001_4_by_4.tif'
         o_norm = Normalization()
         o_norm.load(file=image1, auto_gamma_filter=False)
         o_norm.load(file=ob1, data_type='ob', auto_gamma_filter=False)
         with pytest.raises(ValueError):
@@ -565,29 +515,29 @@
         # sample, ob and df
         image1 = self.data_path + '/tif/sample/image001.tif'
         ob1 = self.data_path + '/tif/ob/ob001.tif'
         df1 = self.data_path + '/different_format/df001_4_by_4.tif'
         o_norm = Normalization()
         o_norm.load(file=image1, auto_gamma_filter=False)
         o_norm.load(file=ob1, data_type='ob', auto_gamma_filter=False)
-        o_norm.load(file=df1, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(file=df1, data_type='df', auto_gamma_filter=False)
         with pytest.raises(ValueError):
             o_norm.normalization()
 
     def test_full_normalization_sample_with_several_roi(self):
         """assert the full normalization works with several roi selected"""
         sample_path = self.data_path + '/tif/sample'
         ob_path = self.data_path + '/tif/ob'
         df_path = self.data_path + '/tif/df'
 
         # without DF
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
-        # o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
+        # o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
         _roi_1 = ROI(x0=0, y0=0, x1=1, y1=1)
         _roi_2 = ROI(x0=0, y0=0, x1=1, y1=1)
         o_norm.normalization(roi=[_roi_1, _roi_2])
         _norm_returned = o_norm.data['normalized'][0]
         _norm_expected = np.ones((5, 5))
         _norm_expected[:, 2] = 2
         _norm_expected[:, 3] = 3
@@ -595,15 +545,15 @@
 
         assert _norm_expected[0, 0] == pytest.approx(_norm_returned[0, 0], 1e-8)
 
         # with DF
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
-        o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
         _roi_1 = ROI(x0=0, y0=0, x1=1, y1=1)
         _roi_2 = ROI(x0=0, y0=0, x1=1, y1=1)
         o_norm.normalization(roi=[_roi_1, _roi_2])
         _norm_returned = o_norm.data['normalized'][0]
         _norm_expected = np.ones((5, 5))
         _norm_expected[:, 2] = 2
         _norm_expected[:, 3] = 3
@@ -614,74 +564,36 @@
         sample_path = self.data_path + '/tif/special_sample'
         ob_path = self.data_path + '/tif/special_ob'
 
         # without DF
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
         o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
-        # o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
+        # o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
         _roi_1 = ROI(x0=0, y0=0, x1=0, y1=0)
         _roi_2 = ROI(x0=4, y0=4, x1=4, y1=4)
         o_norm.normalization(roi=[_roi_1, _roi_2])
         _norm_returned = o_norm.data['normalized'][0]
         _norm_expected = np.ones((5, 5))
         _norm_expected[:, 2] = 2
         _norm_expected[:, 3] = 3
         _norm_expected[:, 4] = 4
 
         assert _norm_expected[0, 0] == pytest.approx(_norm_returned[0, 0], 1e-8)
 
-    def test_tof_normalization_without_roi_with_tiff(self):
-        """assert the normalization works when each sample data is normalized by its own ob"""
-        sample_path = self.data_path + '/tif/tof/sample'
-        ob_path = self.data_path + '/tif/tof/ob'
-
-        o_norm = Normalization()
-        o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-        o_norm.normalization(force=True)
-
-        first_normalized_data_returned = o_norm.get_normalized_data()[0]
-        first_normalized_data_expected = np.ones((5, 5))
-        first_normalized_data_expected[0:3, 0:2] = 5
-
-        nbr_col, nbr_row = np.shape(first_normalized_data_expected)
-        for _col in np.arange(nbr_col):
-            for _row in np.arange(nbr_row):
-                assert first_normalized_data_returned[_col, _row] == first_normalized_data_expected[_col, _row]
-
-    def test_tof_normalization_without_roi_with_fits(self):
-        """assert the normalization works when each sample data is normalized by its own ob"""
-        sample_path = self.data_path + '/fits/tof/sample'
-        ob_path = self.data_path + '/fits/tof/ob'
-
-        o_norm = Normalization()
-        o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-        o_norm.normalization(force=True)
-
-        first_normalized_data_returned = o_norm.get_normalized_data()[0]
-        first_normalized_data_expected = np.ones((5, 5))
-        first_normalized_data_expected[0:3, 0:2] = 5
-
-        nbr_col, nbr_row = np.shape(first_normalized_data_expected)
-        for _col in np.arange(nbr_col):
-            for _row in np.arange(nbr_row):
-                assert first_normalized_data_returned[_col, _row] == first_normalized_data_expected[_col, _row]
-
     def test_full_normalization_sample_with_one_roi(self):
         """assert the full normalization works with several roi selected"""
         sample_path = self.data_path + '/tif/sample'
         ob_path = self.data_path + '/tif/ob'
         df_path = self.data_path + '/tif/df'
 
         # without DF
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
+        o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
         _roi_1 = ROI(x0=0, y0=0, x1=1, y1=1)
         o_norm.normalization(roi=[_roi_1])
         _norm_returned = o_norm.data['normalized'][0]
         _norm_expected = np.ones((5, 5))
         _norm_expected[:, 2] = 2
         _norm_expected[:, 3] = 3
         _norm_expected[:, 4] = 4
@@ -690,16 +602,16 @@
         for _col in np.arange(nbr_col):
             for _row in np.arange(nbr_row):
                 assert _norm_expected[_col, _row] == _norm_returned[_col, _row]
 
         # with DF
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-        o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
+        o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
         _roi_1 = ROI(x0=0, y0=0, x1=1, y1=1)
         o_norm.normalization(roi=[_roi_1])
         _norm_returned = o_norm.data['normalized'][0]
         _norm_expected = np.ones((5, 5))
         _norm_expected[:, 2] = 2
         _norm_expected[:, 3] = 3
         _norm_expected[:, 4] = 4
@@ -714,70 +626,73 @@
 
         # without normalization roi
         sample_path = self.data_path + '/tif/sample'
         ob_path = self.data_path + '/tif/ob'
         df_path = self.data_path + '/tif/df'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-        o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
+        o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
         o_norm.normalization()
         _norm_expected = np.ones((5, 5))
         _norm_expected[:, 2] = 2
         _norm_expected[:, 3] = 3
         _norm_expected[:, 4] = 4
         _norm_returned = o_norm.data['normalized']
         assert (_norm_expected == _norm_returned).all()
-
+        
         # with normalization roi
         sample_path = self.data_path + '/tif/sample'
         ob_path = self.data_path + '/tif/ob'
         df_path = self.data_path + '/tif/df'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-        o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
+        o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
+        o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
         _roi = ROI(x0=0, y0=0, x1=2, y1=2)
         o_norm.normalization(roi=_roi)
-        _norm_expected = o_norm.data['sample']['data'][0]
-        _norm_expected[0, 0] = 1
+        _norm_expected = np.ones((5, 5))
+        _norm_expected.fill(0.8125)
+        _norm_expected[:, 2] = 1.625
+        _norm_expected[:, 3] = 2.4375
+        _norm_expected[:, 4] = 3.25
         _norm_returned = o_norm.data['normalized']
-        assert (_norm_expected == _norm_returned[0]).all()
-
+        assert (_norm_expected == _norm_returned).all()
+        
     def test_various_data_type_correctly_returned(self):
         """assert normalized, sample, ob and df data are correctly returned"""
         sample_path = self.data_path + '/tif/sample'
         ob_path = self.data_path + '/tif/ob'
         df_path = self.data_path + '/tif/df'
         o_norm = Normalization()
         o_norm.load(folder=sample_path, auto_gamma_filter=False)
-        o_norm.load(folder=ob_path, data_type=DataType.ob, auto_gamma_filter=False)
-        o_norm.load(folder=df_path, data_type=DataType.df, auto_gamma_filter=False)
-
+        o_norm.load(folder=ob_path, data_type='ob', auto_gamma_filter=False)
+        o_norm.load(folder=df_path, data_type='df', auto_gamma_filter=False)
+        
         # sample
-        _data_expected = o_norm.data[DataType.sample]['data'][0]
+        _data_expected = o_norm.data['sample']['data'][0]
         _data_returned = o_norm.get_sample_data()[0]
         assert (_data_expected == _data_returned).all()
-
+        
         # ob
-        _ob_expected = o_norm.data[DataType.ob]['data']
+        _ob_expected = o_norm.data['ob']['data']
         _ob_returned = o_norm.get_ob_data()[0]
         assert (_ob_expected == _ob_returned).all()
-
+        
         # df
-        _df_expected = o_norm.data[DataType.df]['data']
+        _df_expected = o_norm.data['df']['data']
         _df_returned = o_norm.get_df_data()
         assert _df_expected == _df_returned
-
+        
         # normalized is empty before normalization
         assert o_norm.get_normalized_data() is None
-
+        
         # run normalization
         o_norm.normalization()
-
+        
         _norm_expected = o_norm.data['normalized'][0]
         _norm_returned = o_norm.get_normalized_data()[0]
         assert (_norm_expected == _norm_returned).all()
 
     def test_normalization_using_roi_of_sample_only(self):
         """testing features that will normalized the data according to a ROI of the sample
         this feature require at least 1 ROI. the average counts of the ROI for each image will be used as
@@ -793,18 +708,18 @@
 
         o_norm = Normalization()
         o_norm.load(file=sample_file, auto_gamma_filter=False)
         _roi = ROI(x0=0, y0=0, x1=0, y1=0)
         o_norm.normalization(roi=_roi, use_only_sample=True)
 
         _norm_expected = np.ones((5, 5))
-        _norm_expected[1:, 0] = 1. / 10
-        _norm_expected[:, 1] = 2. / 10
-        _norm_expected[:, 2] = 3. / 10
-        _norm_expected[:, 3] = 4. / 10
-        _norm_expected[:-1, 4] = 5. / 10
+        _norm_expected[1:, 0] = 1./10
+        _norm_expected[:, 1] = 2./10
+        _norm_expected[:, 2] = 3./10
+        _norm_expected[:, 3] = 4./10
+        _norm_expected[:-1, 4] = 5./10
         _norm_returned = o_norm.get_normalized_data()[0]
 
         nbr_col, nbr_row = np.shape(_norm_expected)
         for _col in np.arange(nbr_col):
             for _row in np.arange(nbr_row):
                 assert _norm_expected[_col, _row] == pytest.approx(_norm_returned[_col, _row], 1e-5)
```

### Comparing `NeuNorm-1.5.3/tests/NeuNorm/roi_test.py` & `NeuNorm-1.6.1/tests/NeuNorm/roi_test.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/NeuNorm/utilities_test.py` & `NeuNorm-1.6.1/tests/NeuNorm/utilities_test.py`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/df/df001.fits` & `NeuNorm-1.6.1/tests/data/fits/df/df001.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/ob/ob001.fits` & `NeuNorm-1.6.1/tests/data/fits/ob/ob001.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/ob/ob002.fits` & `NeuNorm-1.6.1/tests/data/fits/ob/ob002.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/ob/ob003.fits` & `NeuNorm-1.6.1/tests/data/fits/ob/ob003.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/sample/image001.fits` & `NeuNorm-1.6.1/tests/data/fits/sample/image001.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/sample/image002.fits` & `NeuNorm-1.6.1/tests/data/fits/sample/image002.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/sample/image003.fits` & `NeuNorm-1.6.1/tests/data/fits/sample/image003.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/test_roi/ob.fits` & `NeuNorm-1.6.1/tests/data/fits/test_roi/ob.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/test_roi/sample.fits` & `NeuNorm-1.6.1/tests/data/fits/test_roi/sample.fits`

 * *Files identical despite different names*

### Comparing `NeuNorm-1.5.3/tests/data/fits/tof/ob/ob_001.fits` & `NeuNorm-1.6.1/tests/data/ob001.fits`

 * *Files identical despite different names*

