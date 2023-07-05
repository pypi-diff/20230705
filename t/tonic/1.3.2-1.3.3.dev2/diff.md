# Comparing `tmp/tonic-1.3.2.tar.gz` & `tmp/tonic-1.3.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.3.2.tar", last modified: Sun Jul  2 06:38:17 2023, max compression
+gzip compressed data, was "tonic-1.3.3.dev2.tar", last modified: Wed Jul  5 02:34:08 2023, max compression
```

## Comparing `tonic-1.3.2.tar` & `tonic-1.3.3.dev2.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 06:37:55.000000 tonic-1.3.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.852789 tonic-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.856789 tonic-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-02 06:37:55.000000 tonic-1.3.2/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 06:37:55.000000 tonic-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 06:37:55.000000 tonic-1.3.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-02 06:38:17.000000 tonic-1.3.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    39958 2023-07-02 06:38:17.000000 tonic-1.3.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 06:37:55.000000 tonic-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 06:37:55.000000 tonic-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-02 06:38:17.884791 tonic-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-02 06:37:55.000000 tonic-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.860789 tonic-1.3.2/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.864790 tonic-1.3.2/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.868790 tonic-1.3.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 06:37:55.000000 tonic-1.3.2/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-02 06:37:55.000000 tonic-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-02 06:38:17.884791 tonic-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-02 06:37:55.000000 tonic-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.868790 tonic-1.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-02 06:37:55.000000 tonic-1.3.2/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-02 06:37:55.000000 tonic-1.3.2/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 06:37:55.000000 tonic-1.3.2/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.872790 tonic-1.3.2/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-02 06:37:55.000000 tonic-1.3.2/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-02 06:37:55.000000 tonic-1.3.2/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.876790 tonic-1.3.2/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.876790 tonic-1.3.2/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.880791 tonic-1.3.2/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    37426 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-07-02 06:37:55.000000 tonic-1.3.2/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:38:17.876790 tonic-1.3.2/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 06:38:17.000000 tonic-1.3.2/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.603172 tonic-1.3.3.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.583172 tonic-1.3.3.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.583172 tonic-1.3.3.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    40015 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-05 02:34:08.603172 tonic-1.3.3.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.583172 tonic-1.3.3.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.587172 tonic-1.3.3.dev2/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.591172 tonic-1.3.3.dev2/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.591172 tonic-1.3.3.dev2/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.591172 tonic-1.3.3.dev2/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.591172 tonic-1.3.3.dev2/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.591172 tonic-1.3.3.dev2/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.591172 tonic-1.3.3.dev2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 02:34:08.603172 tonic-1.3.3.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.595172 tonic-1.3.3.dev2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.595172 tonic-1.3.3.dev2/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.595172 tonic-1.3.3.dev2/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.599172 tonic-1.3.3.dev2/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.599172 tonic-1.3.3.dev2/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.599172 tonic-1.3.3.dev2/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.599172 tonic-1.3.3.dev2/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.599172 tonic-1.3.3.dev2/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37426 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-07-05 02:33:51.000000 tonic-1.3.3.dev2/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:34:08.595172 tonic-1.3.3.dev2/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 02:34:08.000000 tonic-1.3.3.dev2/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.3.2/.github/workflows/ci-pipeline.yml` & `tonic-1.3.3.dev2/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/AUTHORS` & `tonic-1.3.3.dev2/AUTHORS`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/ChangeLog` & `tonic-1.3.3.dev2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 CHANGES
 =======
 
+* update plot\_animation fn
+* update plot\_animation fn
+
 v1.3.2
 ------
 
 * update docs notebook with new ToTimesurface transform
 
 v1.3.1
 ------
```

### Comparing `tonic-1.3.2/LICENSE.txt` & `tonic-1.3.3.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/PKG-INFO` & `tonic-1.3.3.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.3.2
+Version: 1.3.3.dev2
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.3.2/README.md` & `tonic-1.3.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/Makefile` & `tonic-1.3.3.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/event-cameras/eventstream.png` & `tonic-1.3.3.dev2/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/event-cameras/framestream.png` & `tonic-1.3.3.dev2/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.3.3.dev2/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.3.3.dev2/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/snn/neuron-models.png` & `tonic-1.3.3.dev2/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/snn/surrogates.png` & `tonic-1.3.3.dev2/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/tonic-logo-black.png` & `tonic-1.3.3.dev2/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/tonic-logo-white.png` & `tonic-1.3.3.dev2/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/_static/tonic_favicon.png` & `tonic-1.3.3.dev2/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/about/info.rst` & `tonic-1.3.3.dev2/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/about/prototype.rst` & `tonic-1.3.3.dev2/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/about/release_notes.rst` & `tonic-1.3.3.dev2/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/conf.py` & `tonic-1.3.3.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/datasets.rst` & `tonic-1.3.3.dev2/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.3.3.dev2/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/representations/plot_toframe.py` & `tonic-1.3.3.dev2/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/representations/plot_toimage.py` & `tonic-1.3.3.dev2/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_decimation.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_denoise.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_downsample.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.3.3.dev2/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/getting_involved/communication_channels.rst` & `tonic-1.3.3.dev2/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/getting_involved/contribute.rst` & `tonic-1.3.3.dev2/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/getting_started/install.rst` & `tonic-1.3.3.dev2/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/getting_started/nmnist.ipynb` & `tonic-1.3.3.dev2/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.3.3.dev2/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/how-tos/visualizing-data.ipynb` & `tonic-1.3.3.dev2/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.3.3.dev2/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/index.md` & `tonic-1.3.3.dev2/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/make.bat` & `tonic-1.3.3.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/reading_material/design_choices.rst` & `tonic-1.3.3.dev2/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/reading_material/intro-event-cameras.rst` & `tonic-1.3.3.dev2/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/reading_material/intro-snns.rst` & `tonic-1.3.3.dev2/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/reading_material/training-snns.rst` & `tonic-1.3.3.dev2/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/transformations.rst` & `tonic-1.3.3.dev2/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/tutorials/batching.ipynb` & `tonic-1.3.3.dev2/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/tutorials/davis_data.ipynb` & `tonic-1.3.3.dev2/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.3.3.dev2/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/tutorials/large_datasets.ipynb` & `tonic-1.3.3.dev2/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/docs/tutorials/slicing.ipynb` & `tonic-1.3.3.dev2/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/setup.cfg` & `tonic-1.3.3.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/dataset_utils.py` & `tonic-1.3.3.dev2/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/prototype_dataset_utils.py` & `tonic-1.3.3.dev2/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_audio_transforms.py` & `tonic-1.3.3.dev2/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_caching.py` & `tonic-1.3.3.dev2/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_chained_transforms.py` & `tonic-1.3.3.dev2/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_data/sample.aedat4` & `tonic-1.3.3.dev2/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_data/sample_ncars.dat` & `tonic-1.3.3.dev2/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_data/sample_nmnist.bin` & `tonic-1.3.3.dev2/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_data/sample_stmnist.mat` & `tonic-1.3.3.dev2/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_datasets.py` & `tonic-1.3.3.dev2/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_dsec.py` & `tonic-1.3.3.dev2/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_io.py` & `tonic-1.3.3.dev2/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_prototype_datasets.py` & `tonic-1.3.3.dev2/test/test_prototype_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_representations.py` & `tonic-1.3.3.dev2/test/test_representations.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_sliced_dataset.py` & `tonic-1.3.3.dev2/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_slicers.py` & `tonic-1.3.3.dev2/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_tonic_utils.py` & `tonic-1.3.3.dev2/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/test_transforms.py` & `tonic-1.3.3.dev2/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/test/utils.py` & `tonic-1.3.3.dev2/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/audio_transforms.py` & `tonic-1.3.3.dev2/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/cached_dataset.py` & `tonic-1.3.3.dev2/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/collation.py` & `tonic-1.3.3.dev2/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/dataset.py` & `tonic-1.3.3.dev2/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/__init__.py` & `tonic-1.3.3.dev2/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/asl_dvs.py` & `tonic-1.3.3.dev2/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/cifar10dvs.py` & `tonic-1.3.3.dev2/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/davisdataset.py` & `tonic-1.3.3.dev2/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/dsec.py` & `tonic-1.3.3.dev2/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/dvs_lips.py` & `tonic-1.3.3.dev2/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/dvsgesture.py` & `tonic-1.3.3.dev2/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/hsd.py` & `tonic-1.3.3.dev2/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/mvsec.py` & `tonic-1.3.3.dev2/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/ncaltech101.py` & `tonic-1.3.3.dev2/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/nmnist.py` & `tonic-1.3.3.dev2/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/pokerdvs.py` & `tonic-1.3.3.dev2/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/s_mnist.py` & `tonic-1.3.3.dev2/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/tum_vie.py` & `tonic-1.3.3.dev2/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/datasets/visual_place_recognition.py` & `tonic-1.3.3.dev2/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/download_utils.py` & `tonic-1.3.3.dev2/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/__init__.py` & `tonic-1.3.3.dev2/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/crop.py` & `tonic-1.3.3.dev2/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/decimate.py` & `tonic-1.3.3.dev2/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/denoise.py` & `tonic-1.3.3.dev2/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/drop_event.py` & `tonic-1.3.3.dev2/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/drop_pixel.py` & `tonic-1.3.3.dev2/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/refractory_period.py` & `tonic-1.3.3.dev2/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/spatial_jitter.py` & `tonic-1.3.3.dev2/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/time_jitter.py` & `tonic-1.3.3.dev2/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/time_skew.py` & `tonic-1.3.3.dev2/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/to_averaged_timesurface.py` & `tonic-1.3.3.dev2/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/to_bina_rep.py` & `tonic-1.3.3.dev2/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/to_frame.py` & `tonic-1.3.3.dev2/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/to_timesurface.py` & `tonic-1.3.3.dev2/tonic/functional/to_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/to_voxel_grid.py` & `tonic-1.3.3.dev2/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/functional/uniform_noise.py` & `tonic-1.3.3.dev2/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/io.py` & `tonic-1.3.3.dev2/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/README.md` & `tonic-1.3.3.dev2/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/datasets/ncars.py` & `tonic-1.3.3.dev2/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/datasets/nmnist.py` & `tonic-1.3.3.dev2/tonic/prototype/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/datasets/prophesee.py` & `tonic-1.3.3.dev2/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/datasets/stmnist.py` & `tonic-1.3.3.dev2/tonic/prototype/datasets/stmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.3.3.dev2/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.3.3.dev2/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/prototype/slicers.py` & `tonic-1.3.3.dev2/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/sliced_dataset.py` & `tonic-1.3.3.dev2/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/slicers.py` & `tonic-1.3.3.dev2/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/transforms.py` & `tonic-1.3.3.dev2/tonic/transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic/utils.py` & `tonic-1.3.3.dev2/tonic/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from typing import Tuple
+
 import numpy as np
 
 import tonic.transforms as transforms
 
 
-def plot_event_grid(events, axis_array=(1, 3), plot_frame_number=False):
+def plot_event_grid(
+    events: np.ndarray,
+    axis_array: Tuple[int, int] = (1, 3),
+    plot_frame_number: bool = False,
+):
     """Plot events accumulated as frames equal to the product of axes for visual inspection.
 
     Parameters:
         events: Structured numpy array of shape [num_events, num_event_channels].
         axis_array: dimensions of plotting grid. The larger the grid,
                     the more fine-grained the events will be sliced in time.
         plot_frame_number: optional index of frame when plotting
@@ -63,16 +69,17 @@
 
         frames = frame_transform(events)
         plt.imshow(frames.squeeze().T)
         plt.xlabel("Time")
         plt.ylabel("Channels")
 
 
-def plot_animation(frames: np.ndarray):
-    """Helper function that animates a tensor of frames of shape (TCHW).
+def plot_animation(frames: np.ndarray, figsize: Tuple[int, int] = (5, 5)):
+    """Helper function that animates a tensor of frames of shape (TCHW). If you run this in a
+    Jupyter notebook, you can display the animation inline like shown in the example below.
 
     Parameters:
         frames: numpy array or tensor of shape (TCHW)
 
     Example:
         >>> import tonic
         >>> nmnist = tonic.datasets.NMNIST(save_to='./data', train=False)
@@ -81,38 +88,40 @@
         >>> transform = tonic.transforms.ToFrame(
         >>>     sensor_size=nmnist.sensor_size,
         >>>     time_window=10000,
         >>> )
         >>>
         >>> frames = transform(events)
         >>> animation = tonic.utils.plot_animation(frames)
+        >>>
+        >>> # Display the animation inline in a Jupyter notebook
+        >>> from IPython.display import HTML
+        >>> HTML(animation.to_jshtml())
 
     Returns:
         The animation object. Store this in a variable to keep it from being garbage collected until displayed.
     """
     try:
         import matplotlib.pyplot as plt
         from matplotlib import animation
     except ImportError:
         raise ImportError(
             "Please install the matplotlib package to plot events. This is an optional"
             " dependency."
         )
-    fig = plt.figure(figsize=(2, 2))
-    if frames[0].shape[0] == 2:
-        first_frame = frames[0][1] - frames[0][0]
-    else:
-        first_frame = frames[0][0]
-    ax = plt.imshow(first_frame)
+    fig = plt.figure(figsize=figsize)
+    if frames.shape[1] == 2:
+        rgb = np.zeros((frames.shape[0], 3, *frames.shape[2:]))
+        rgb[:, 1:, ...] = frames
+        frames = rgb
+    if frames.shape[1] in [1, 2, 3]:
+        frames = np.moveaxis(frames, 1, 3)
+    ax = plt.imshow(frames[0])
     plt.axis("off")
 
     def animate(frame):
-        if frame.shape[0] == 2:
-            frame = frame[1] - frame[0]
-        else:
-            frame = frame[0]
         ax.set_data(frame)
         return ax
 
     anim = animation.FuncAnimation(fig, animate, frames=frames, interval=100)
     plt.show()
     return anim
```

### Comparing `tonic-1.3.2/tonic-logo-padded.png` & `tonic-1.3.3.dev2/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.2/tonic.egg-info/PKG-INFO` & `tonic-1.3.3.dev2/tonic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.3.2
+Version: 1.3.3.dev2
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.3.2/tonic.egg-info/SOURCES.txt` & `tonic-1.3.3.dev2/tonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

