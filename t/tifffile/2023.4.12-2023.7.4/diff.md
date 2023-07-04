# Comparing `tmp/tifffile-2023.4.12.tar.gz` & `tmp/tifffile-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2023.4.12.tar", last modified: Wed Apr 12 22:27:08 2023, max compression
+gzip compressed data, was "tifffile-2023.7.4.tar", last modified: Tue Jul  4 23:29:08 2023, max compression
```

## Comparing `tifffile-2023.4.12.tar` & `tifffile-2023.7.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.119431 tifffile-2023.4.12/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2023.4.12/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    35595 2023-04-12 22:27:05.000000 tifffile-2023.4.12/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2023-04-12 22:27:05.000000 tifffile-2023.4.12/LICENSE
--rw-rw-rw-   0        0        0      540 2023-01-23 07:24:27.000000 tifffile-2023.4.12/MANIFEST.in
--rw-rw-rw-   0        0        0    30901 2023-04-12 22:27:08.119431 tifffile-2023.4.12/PKG-INFO
--rw-rw-rw-   0        0        0    29968 2023-04-12 22:27:05.000000 tifffile-2023.4.12/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.091431 tifffile-2023.4.12/docs/
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.091431 tifffile-2023.4.12/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2023.4.12/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-01-12 21:14:58.000000 tifffile-2023.4.12/docs/conf.py
--rw-rw-rw-   0        0        0     3629 2023-03-04 01:54:58.000000 tifffile-2023.4.12/docs/make.py
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.095431 tifffile-2023.4.12/examples/
--rw-rw-rw-   0        0        0    15054 2023-02-07 15:45:27.000000 tifffile-2023.4.12/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2539 2023-01-10 16:09:24.000000 tifffile-2023.4.12/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2023-04-12 22:27:08.119431 tifffile-2023.4.12/setup.cfg
--rw-rw-rw-   0        0        0     3708 2023-01-23 07:09:38.000000 tifffile-2023.4.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.095431 tifffile-2023.4.12/tests/
--rw-rw-rw-   0        0        0     1601 2023-03-14 03:16:25.000000 tifffile-2023.4.12/tests/conftest.py
--rw-rw-rw-   0        0        0   700808 2023-04-12 22:24:28.000000 tifffile-2023.4.12/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.107430 tifffile-2023.4.12/tifffile/
--rw-rw-rw-   0        0        0      110 2020-01-01 02:31:34.000000 tifffile-2023.4.12/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2023.4.12/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11839 2022-12-29 20:31:08.000000 tifffile-2023.4.12/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2022-07-28 19:50:49.000000 tifffile-2023.4.12/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2022-06-04 00:53:35.000000 tifffile-2023.4.12/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5906 2023-03-10 03:08:14.000000 tifffile-2023.4.12/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0     2410 2022-05-13 03:22:47.000000 tifffile-2023.4.12/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2022-06-04 00:53:09.000000 tifffile-2023.4.12/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   859764 2023-04-12 21:35:37.000000 tifffile-2023.4.12/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2023-04-12 22:27:08.119431 tifffile-2023.4.12/tifffile.egg-info/
--rw-rw-rw-   0        0        0    30901 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-04-12 22:27:07.000000 tifffile-2023.4.12/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 22:27:06.000000 tifffile-2023.4.12/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.172341 tifffile-2023.7.4/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2023.7.4/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    35933 2023-07-04 23:29:02.000000 tifffile-2023.7.4/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2023-07-04 23:29:02.000000 tifffile-2023.7.4/LICENSE
+-rw-rw-rw-   0        0        0      540 2023-01-23 07:24:27.000000 tifffile-2023.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    31571 2023-07-04 23:29:08.172341 tifffile-2023.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0    30606 2023-07-04 23:29:02.000000 tifffile-2023.7.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/docs/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2023.7.4/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-01-12 21:14:58.000000 tifffile-2023.7.4/docs/conf.py
+-rw-rw-rw-   0        0        0     3629 2023-03-04 01:54:58.000000 tifffile-2023.7.4/docs/make.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/examples/
+-rw-rw-rw-   0        0        0    15098 2023-07-04 23:25:39.000000 tifffile-2023.7.4/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2557 2023-06-27 16:33:23.000000 tifffile-2023.7.4/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 23:29:08.172341 tifffile-2023.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-07-03 00:03:17.000000 tifffile-2023.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/tests/
+-rw-rw-rw-   0        0        0     1601 2023-03-14 03:16:25.000000 tifffile-2023.7.4/tests/conftest.py
+-rw-rw-rw-   0        0        0   705766 2023-07-04 21:19:00.000000 tifffile-2023.7.4/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.156716 tifffile-2023.7.4/tifffile/
+-rw-rw-rw-   0        0        0      110 2020-01-01 02:31:34.000000 tifffile-2023.7.4/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2023.7.4/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11855 2023-07-03 00:18:30.000000 tifffile-2023.7.4/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2023.7.4/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2023.7.4/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5906 2023-07-03 00:17:55.000000 tifffile-2023.7.4/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2023.7.4/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2023.7.4/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   864300 2023-07-04 02:52:04.000000 tifffile-2023.7.4/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.172341 tifffile-2023.7.4/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    31571 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-07-04 23:29:07.000000 tifffile-2023.7.4/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2023.4.12/CHANGES.rst` & `tifffile-2023.7.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Revisions
 ---------
 
+2023.7.4
+
+- Pass 4992 tests.
+- Add option to return selection from imread (#200).
+- Fix reading OME series with missing trailing frames (#199).
+- Fix fsspec reference for WebP compressed segments missing alpha channel.
+- Fix linting issues.
+- Detect files written by Agilent Technologies.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2023.4.12
 
-- Pass 4988 tests.
 - Do not write duplicate ImageDescription tags from extratags (breaking).
 - Support multifocal SVS files (#193).
 - Log warning when filtering out extratags.
 - Fix writing OME-TIFF with image description in extratags.
 - Ignore invalid predictor tag value if prediction is not used.
 - Raise KeyError if ZarrStore is missing requested chunk.
 
@@ -978,8 +987,8 @@
 2012.8.3
 
 - Read MD GEL tags and NIH Image header.
 
 2012.7.25
 
 - Read ImageJ tags.
-- ...
+- …
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tifffile-2023.4.12/LICENSE` & `tifffile-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/MANIFEST.in` & `tifffile-2023.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/PKG-INFO` & `tifffile-2023.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2023.4.12
+Version: 2023.7.4
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 License-File: LICENSE
 
 Read and write TIFF files
 =========================
 
 Tifffile is a Python library to
@@ -51,15 +52,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.12
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -87,33 +88,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.7.4
+
+- Pass 4992 tests.
+- Add option to return selection from imread (#200).
+- Fix reading OME series with missing trailing frames (#199).
+- Fix fsspec reference for WebP compressed segments missing alpha channel.
+- Fix linting issues.
+- Detect files written by Agilent Technologies.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2023.4.12
 
-- Pass 4988 tests.
 - Do not write duplicate ImageDescription tags from extratags (breaking).
 - Support multifocal SVS files (#193).
 - Log warning when filtering out extratags.
 - Fix writing OME-TIFF with image description in extratags.
 - Ignore invalid predictor tag value if prediction is not used.
 - Raise KeyError if ZarrStore is missing requested chunk.
 
@@ -226,15 +236,15 @@
 - Convert some warnings to debug messages.
 - Declare all classes final.
 - Add script to generate documentation via Sphinx.
 - Convert docstrings to Google style with Sphinx directives.
 
 2022.5.4
 
-- ...
+- …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 TIFF, the Tagged Image File Format, was created by the Aldus Corporation and
@@ -418,14 +428,20 @@
 array to an interleaved RGB, a planar RGB, or a 3-page grayscale TIFF:
 
 >>> data = numpy.random.randint(0, 255, (3, 3, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb')
 >>> imwrite('temp.tif', data, photometric='rgb', planarconfig='separate')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
+Use the `extrasamples` argument to specify how extra components are
+interpreted, for example, for an RGBA image with unassociated alpha channel:
+
+>>> data = numpy.random.randint(0, 255, (256, 256, 4), 'uint8')
+>>> imwrite('temp.tif', data, photometric='rgb', extrasamples=['unassalpha'])
+
 Write a 3-dimensional NumPy array to a multi-page, 16-bit grayscale TIFF file:
 
 >>> data = numpy.random.randint(0, 2**12, (64, 301, 219), 'uint16')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
 Read the whole image stack from the multi-page TIFF file as NumPy array:
 
@@ -493,15 +509,15 @@
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
 
-Overwrite the value of an existing tag, e.g., XResolution:
+Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
@@ -632,19 +648,19 @@
 >>> with TiffWriter('temp.ome.tif', bigtiff=True) as tif:
 ...     metadata={
 ...         'axes': 'TCYXS',
 ...         'SignificantBits': 10,
 ...         'TimeIncrement': 0.1,
 ...         'TimeIncrementUnit': 's',
 ...         'PhysicalSizeX': pixelsize,
-...         'PhysicalSizeXUnit': 'Âµm',
+...         'PhysicalSizeXUnit': 'µm',
 ...         'PhysicalSizeY': pixelsize,
-...         'PhysicalSizeYUnit': 'Âµm',
+...         'PhysicalSizeYUnit': 'µm',
 ...         'Channel': {'Name': ['Channel 1', 'Channel 2']},
-...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['Âµm'] * 16}
+...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16}
 ...     }
 ...     options = dict(
 ...         photometric='rgb',
 ...         tile=(128, 128),
 ...         compression='jpeg',
 ...         resolutionunit='CENTIMETER'
 ...     )
```

### Comparing `tifffile-2023.4.12/README.rst` & `tifffile-2023.7.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.12
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -62,33 +62,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.7.4
+
+- Pass 4992 tests.
+- Add option to return selection from imread (#200).
+- Fix reading OME series with missing trailing frames (#199).
+- Fix fsspec reference for WebP compressed segments missing alpha channel.
+- Fix linting issues.
+- Detect files written by Agilent Technologies.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2023.4.12
 
-- Pass 4988 tests.
 - Do not write duplicate ImageDescription tags from extratags (breaking).
 - Support multifocal SVS files (#193).
 - Log warning when filtering out extratags.
 - Fix writing OME-TIFF with image description in extratags.
 - Ignore invalid predictor tag value if prediction is not used.
 - Raise KeyError if ZarrStore is missing requested chunk.
 
@@ -201,15 +210,15 @@
 - Convert some warnings to debug messages.
 - Declare all classes final.
 - Add script to generate documentation via Sphinx.
 - Convert docstrings to Google style with Sphinx directives.
 
 2022.5.4
 
-- ...
+- …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 TIFF, the Tagged Image File Format, was created by the Aldus Corporation and
@@ -393,14 +402,20 @@
 array to an interleaved RGB, a planar RGB, or a 3-page grayscale TIFF:
 
 >>> data = numpy.random.randint(0, 255, (3, 3, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb')
 >>> imwrite('temp.tif', data, photometric='rgb', planarconfig='separate')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
+Use the `extrasamples` argument to specify how extra components are
+interpreted, for example, for an RGBA image with unassociated alpha channel:
+
+>>> data = numpy.random.randint(0, 255, (256, 256, 4), 'uint8')
+>>> imwrite('temp.tif', data, photometric='rgb', extrasamples=['unassalpha'])
+
 Write a 3-dimensional NumPy array to a multi-page, 16-bit grayscale TIFF file:
 
 >>> data = numpy.random.randint(0, 2**12, (64, 301, 219), 'uint16')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
 Read the whole image stack from the multi-page TIFF file as NumPy array:
 
@@ -468,15 +483,15 @@
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
 
-Overwrite the value of an existing tag, e.g., XResolution:
+Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
```

### Comparing `tifffile-2023.4.12/docs/conf.py` & `tifffile-2023.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/docs/make.py` & `tifffile-2023.7.4/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/examples/earthbigdata.py` & `tifffile-2023.7.4/examples/earthbigdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 
 # %% [markdown]
 """
 # Create a fsspec ReferenceFileSystem for a large set of remote GeoTIFF files
 
 by [Christoph Gohlke](https://www.cgohlke.com)
 
-Updated on July 31, 2022
+Updated on July 4, 2023
 
 This Python script uses the [tifffile](https://github.com/cgohlke/tifffile) and
 [imagecodecs](https://github.com/cgohlke/imagecodecs) packages to create a
 [fsspec ReferenceFileSystem](https://github.com/fsspec/kerchunk) file in
 JSON format for the [Earthbigdata](
 http://sentinel-1-global-coherence-earthbigdata.s3-website-us-west-2.amazonaws.com
 ) set, which consists of 1,033,422 GeoTIFF files stored on AWS.
 The ReferenceFileSystem is used to create a multi-dimensional Xarray dataset.
 
-See discussion at [kerchunk/issues/78](
+Refer to the discussion at [kerchunk/issues/78](
 https://github.com/fsspec/kerchunk/issues/78).
 """
 
 # %%
 import os
 import base64
 
@@ -77,15 +77,15 @@
 # %%
 if not os.path.exists('earthbigdata.txt'):
     os.system(
         'aws s3 ls sentinel-1-global-coherence-earthbigdata/data/tiles'
         ' --recursive > earthbigdata.txt'
     )
 
-with open('earthbigdata.txt') as fh:
+with open('earthbigdata.txt', encoding='utf-8') as fh:
     tiff_files = [
         line.split()[-1][11:] for line in fh.readlines() if '.tif' in line
     ]
 print('Number of TIFF files:', len(tiff_files))
 
 
 # %% [markdown]
@@ -178,15 +178,15 @@
 
 # %% [markdown]
 """
 ## Open a file for writing the fsspec ReferenceFileSystem in JSON format
 """
 
 # %%
-jsonfile = open('earthbigdata.json', 'w', newline='\n')
+jsonfile = open('earthbigdata.json', 'w', encoding='utf-8', newline='\n')
 
 # %% [markdown]
 """
 ## Write the coordinate arrays
 
 Add the coordinate arrays to a Zarr group, convert it to a fsspec
 ReferenceFileSystem JSON string, and write it to the open file.
```

### Comparing `tifffile-2023.4.12/examples/issue125.py` & `tifffile-2023.7.4/examples/issue125.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     'anon': True,
     'client_kwargs': {'endpoint_url': 'https://mghp.osn.xsede.org'},
 }
 fs = fsspec.filesystem('s3', **remote_options)
 files = [f's3://{f}' for f in fs.ls('/rsignellbucket1/lcmap/cog')]
 
 # write the ReferenceFileSystem of each file to a JSON file
-with open('issue125.json', 'w', newline='\n') as jsonfile:
+with open('issue125.json', 'w', encoding='utf-8', newline='\n') as jsonfile:
     for i, filename in enumerate(tifffile.natural_sorted(files)):
         url, name = filename.rsplit('/', 1)
         with fs.open(filename) as fh:
             with tifffile.TiffFile(fh, name=name) as tif:
                 print(tif.geotiff_metadata)
                 with tif.series[0].aszarr() as store:
                     store.write_fsspec(
```

### Comparing `tifffile-2023.4.12/setup.py` & `tifffile-2023.7.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     # return first match for pattern in code
     match = re.search(pattern, code, flags)
     if match is None:
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
-with open('tifffile/tifffile.py') as fh:
+with open('tifffile/tifffile.py', encoding='utf-8') as fh:
     code = fh.read().replace('\r\n', '\n').replace('\r', '\n')
 
-version = search(r"__version__ = '(.*?)'", code)
+version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev')
 version += ('.' + buildnumber) if buildnumber else ''
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}r"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
@@ -34,48 +34,49 @@
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
 if 'sdist' in sys.argv:
     # update README, LICENSE, and CHANGES files
 
-    with open('README.rst', 'w') as fh:
+    with open('README.rst', 'w', encoding='utf-8') as fh:
         fh.write(readme)
 
     license = search(
         r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+r""',
         code,
         re.MULTILINE | re.DOTALL,
     )
     license = license.replace('# ', '').replace('#', '')
 
-    with open('LICENSE', 'w') as fh:
+    with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
 
     revisions = search(
-        r'(?:\r\n|\r|\n){2}(Revisions.*)- \.\.\.',
+        r'(?:\r\n|\r|\n){2}(Revisions.*)- …',
         readme,
         re.MULTILINE | re.DOTALL,
     ).strip()
 
-    with open('CHANGES.rst') as fh:
+    with open('CHANGES.rst', encoding='utf-8') as fh:
         old = fh.read()
 
     old = old.split(revisions.splitlines()[-1])[-1]
-    with open('CHANGES.rst', 'w') as fh:
+    with open('CHANGES.rst', 'w', encoding='utf-8') as fh:
         fh.write(revisions.strip())
         fh.write(old)
 
 setup(
     name='tifffile',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
+    long_description_content_type='text/x-rst',
     author='Christoph Gohlke',
     author_email='cgohlke@cgohlke.com',
     url='https://www.cgohlke.com',
     project_urls={
         'Bug Tracker': 'https://github.com/cgohlke/tifffile/issues',
         'Source Code': 'https://github.com/cgohlke/tifffile',
         # 'Documentation': 'https://',
@@ -125,13 +126,13 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tifffile-2023.4.12/tests/conftest.py` & `tifffile-2023.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/tests/test_tifffile.py` & `tifffile-2023.7.4/tests/test_tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2023.4.12
+:Version: 2023.7.4
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -55,15 +55,14 @@
 import struct
 import sys
 import tempfile
 import urllib.error
 import urllib.request
 from io import BytesIO
 
-import fsspec
 import numpy
 import pytest
 from numpy.testing import (
     assert_allclose,
     assert_array_almost_equal,
     assert_array_equal,
 )
@@ -191,22 +190,22 @@
 
 HERE = os.path.dirname(__file__)
 TEMP_DIR = os.path.join(HERE, '_tmp')
 PRIVATE_DIR = os.path.join(HERE, 'data', 'private')
 PUBLIC_DIR = os.path.join(HERE, 'data', 'public')
 
 IS_BE = sys.byteorder == 'big'
-IS_PYPY = 'PyPy' in sys.version
+IS_PYPY = 'pypy' in sys.version.lower()
 IS_WIN = sys.platform == 'win32'
 IS_CG = os.environ.get('COMPUTERNAME', '').startswith('CG-T')
 
 
 # skip certain tests
 def skip(key, default):
-    return os.getenv(key, default) in (True, 1, '1')
+    return os.getenv(key, default) in {True, 1, '1'}
 
 
 # skip tests requiring large memory
 SKIP_LARGE = skip('SKIP_LARGE', sys.maxsize < 2**32)
 SKIP_EXTENDED = skip('SKIP_EXTENDED', False)
 # skip public files
 SKIP_PUBLIC = skip('SKIP_PUBLIC', not os.path.exists(PUBLIC_DIR))
@@ -258,15 +257,15 @@
 PAGE_FLAGS = [name for name in dir(TiffPage) if name.startswith('is_')]
 
 URL = 'http://localhost:8386/'  # TEMP_DIR
 
 if not SKIP_HTTP:
     try:
         urllib.request.urlopen(URL + '/test/test.txt', timeout=0.2)
-    except urllib.error.URLError:
+    except (urllib.error.URLError, TimeoutError):
         SKIP_HTTP = True
 
 if not os.path.exists(TEMP_DIR):
     TEMP_DIR = tempfile.gettempdir()
 
 if not SKIP_CODECS:
     try:
@@ -282,16 +281,18 @@
     SKIP_HTTP = True
 
 if SKIP_ZARR:
     zarr = None
 else:
     try:
         import zarr  # type: ignore
+        import fsspec  # type: ignore
     except ImportError:
         zarr = None
+        fsspec = None  # type: ignore
         SKIP_ZARR = True
 
 if SKIP_DASK:
     dask = None
 else:
     try:
         import dask  # type: ignore
@@ -1777,14 +1778,49 @@
         page = tif.pages.first
         assert page.compression == WEBP
         assert page.shape == (2967, 2220, 4)
         assert tuple(page.asarray()[25, 25]) == (246, 244, 245, 255)
         assert f'corrupted {name}' not in caplog.text
 
 
+@pytest.mark.skipif(
+    SKIP_PRIVATE or SKIP_ZARR or SKIP_CODECS or not imagecodecs.WEBP,
+    reason=REASON,
+)
+def test_issue_webp_fsspec():
+    """Test read WebP segments with missing alpha channel via fsspec."""
+    try:
+        from imagecodecs.numcodecs import register_codecs
+    except ImportError:
+        register_codecs = None
+    else:
+        register_codecs('imagecodecs_webp', verbose=False)
+
+    fname = private_file('issues/CMU-1-Small-Region.tile.webp.tiff')
+    url = os.path.dirname(fname).replace('\\', '/')
+    data = imread(fname, series=0)
+    with TempFileName('webp_fsspec', ext='.json') as jsonfile:
+        tiff2fsspec(
+            fname,
+            url,
+            out=jsonfile,
+            series=0,
+            level=0,
+            version=0,
+        )
+        mapper = fsspec.get_mapper(
+            'reference://',
+            fo=jsonfile,
+            target_protocol='file',
+            remote_protocol='file',
+        )
+        zobj = zarr.open(mapper, mode='r')
+        assert_array_equal(zobj[:], data)
+
+
 @pytest.mark.skipif(SKIP_PRIVATE or SKIP_ZARR, reason=REASON)
 def test_issue_tiffslide():
     """Test no ValueError when closing TiffSlide with Zarr group."""
     # https://github.com/bayer-science-for-a-better-life/tiffslide/issues/25
     try:
         from tiffslide import TiffSlide
     except ImportError:
@@ -2537,26 +2573,60 @@
             tags = tif.pages.first.tags
             assert 322 not in tags
             assert 34665 not in tags
             assert tags.get(270, index=1) is None
             assert tags[266].value == 1
 
 
+@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
 def test_issue_invalid_predictor(caplog):
     """Test decoding JPEG compression with invalid predictor tag."""
     fname = private_file('issues/invalid_predictor.tiff')
     with TiffFile(fname) as tif:
         page = tif.pages.first
         assert page.predictor == 58240
         assert page.compression == 7
         data = page.asarray()
         assert 'ignoring predictor' in caplog.text
         assert data.shape == (1275, 1650, 4)
 
 
+@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+def test_issue_ome_missing_frames(caplog):
+    """Test read OME TIFF with missing pages at end."""
+    # https://github.com/cgohlke/tifffile/issues/199
+    fname = private_file('issues/stack_t24_y2048_x2448.tiff')
+    with TiffFile(fname) as tif:
+        assert tif.is_ome
+        assert tif.byteorder == '<'
+        assert len(tif.pages) == 16
+        assert len(tif.series) == 1
+        # assert page properties
+        page = tif.pages.first
+        assert page.photometric == MINISBLACK
+        assert page.imagewidth == 2448
+        assert page.imagelength == 2048
+        assert page.bitspersample == 8
+        assert not page.is_contiguous
+        # assert series properties
+        series = tif.series[0]
+        assert len(series._pages) == 24
+        assert len(series.pages) == 24
+        assert series[16] is None
+        assert series[23] is None
+        assert series.shape == (24, 2048, 2448)
+        assert series.dtype == numpy.uint8
+        assert series.axes == 'TYX'
+        assert series.kind == 'ome'
+        data = series.asarray()
+        assert_aszarr_method(tif, data)
+        assert_aszarr_method(tif, data, chunkmode='page')
+        assert__str__(tif)
+
+
 class TestExceptions:
     """Test various Exceptions and Warnings."""
 
     data = random_data(numpy.uint16, (5, 13, 17))
 
     @pytest.fixture(scope='class')
     def fname(self):
@@ -3175,15 +3245,15 @@
                 tags[305].value
             with pytest.raises(KeyError):
                 tags['Software'].value
             assert len(tags.values()) == len(tags.items())
             assert len(tags.keys()) == len(tags.items()) - 1
             assert set(tags.keys()) == {i[0] for i in tags.items()}
             assert list(tags.values()) == [i[1] for i in tags.items()]
-            assert list(tags.values()) == [t for t in tags]
+            assert list(tags.values()) == list(tags)
 
             tag270 = tags[270]
             del tags[270]
             assert 270 not in tags
             assert 'ImageDescription' not in tags
             with pytest.raises(KeyError):
                 del tags[270]
@@ -3204,15 +3274,15 @@
             assert 0 not in tags
             assert 'None' not in tags
             assert None not in tags
 
 
 def test_class_tifftagregistry():
     """Test TiffTagRegistry."""
-    numtags = 654
+    numtags = 656
     tags = TIFF.TAGS
     assert len(tags) == numtags
     assert tags[11] == 'ProcessingSoftware'
     assert tags['ProcessingSoftware'] == 11
     assert tags.getall(11) == ['ProcessingSoftware']
     assert tags.getall('ProcessingSoftware') == [11]
     tags.add(11, 'ProcessingSoftware')
@@ -4729,15 +4799,15 @@
             [2, 16601, 1431655765, 32],
             [3, 16441, 2863311530, 30],
         ],
         dtype='uint32',
     )
     if int(numpy.__version__.split('.')[1]) < 23:
         with pytest.raises(NotImplementedError):
-            bitorder_decode(data[1:, 1:3]), reverse[1:, 1:3]
+            bitorder_decode(data[1:, 1:3])
     else:
         assert_array_equal(bitorder_decode(data[1:, 1:3]), reverse[1:, 1:3])
 
 
 @pytest.mark.parametrize(
     'kind',
     ['u1', 'u2', 'u4', 'u8', 'i1', 'i2', 'i4', 'i8', 'f4', 'f8', 'B'],
@@ -5126,42 +5196,39 @@
     """Test FileHandle from UNC path."""
     with FileHandle(r'\\localhost\test$\test_FileHandle.bin') as fh:
         assert fh.name == 'test_FileHandle.bin'
         assert fh.dirname == '\\\\localhost\\test$\\'
         assert_filehandle(fh)
 
 
-@pytest.mark.skipif(SKIP_PUBLIC, reason=REASON)
+@pytest.mark.skipif(SKIP_PUBLIC or SKIP_ZARR, reason=REASON)
 def test_filehandle_fsspec_localfileopener():
     """Test FileHandle from fsspec LocalFileOpener."""
-    fsspec = pytest.importorskip('fsspec')
     with fsspec.open(FILEHANDLE_NAME, 'rb') as fhandle:
         with FileHandle(fhandle) as fh:
             assert fh.name == 'test_FileHandle.bin'
             assert fh.is_file  # fails with fsspec 2022.7
             assert_filehandle(fh)
         assert not fhandle.closed
 
 
-@pytest.mark.skipif(SKIP_PUBLIC, reason=REASON)
+@pytest.mark.skipif(SKIP_PUBLIC or SKIP_ZARR, reason=REASON)
 def test_filehandle_fsspec_openfile():
     """Test FileHandle from fsspec OpenFile."""
-    fsspec = pytest.importorskip('fsspec')
     fhandle = fsspec.open(FILEHANDLE_NAME, 'rb')
     with FileHandle(fhandle) as fh:
         assert fh.name == 'test_FileHandle.bin'
         assert fh.is_file
         assert_filehandle(fh)
     fhandle.close()
 
 
-@pytest.mark.skipif(SKIP_PUBLIC or SKIP_HTTP, reason=REASON)
+@pytest.mark.skipif(SKIP_PUBLIC or SKIP_HTTP or SKIP_ZARR, reason=REASON)
 def test_filehandle_fsspec_http():
     """Test FileHandle from HTTP via fsspec."""
-    fsspec = pytest.importorskip('fsspec')
     with open(FILEHANDLE_NAME, 'rb') as fh:
         data = fh.read()
     with TempFileName('test_FileHandle', ext='.bin') as fname:
         with open(fname, 'wb') as fh:
             data = fh.write(data)
     with fsspec.open(URL + 'test/test_FileHandle.bin', 'rb') as fhandle:
         with FileHandle(fhandle) as fh:
@@ -5639,15 +5706,15 @@
         assert page.samplesperpixel == 1
         # assert series properties
         series = tif.series[0]
         assert series.shape == (14, 256, 256)
         assert series.dtype == numpy.int16
         assert series.axes == 'IYX'  # ZYX
         assert series.kind == 'uniform'
-        assert type(series.pages[3]) == TiffFrame
+        assert isinstance(series.pages[3], TiffFrame)
         assert_aszarr_method(series)
         assert__str__(tif)
 
 
 @pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
 def test_read_vips():
     """Test read 347x641 RGB, bigtiff, pyramid, tiled, produced by VIPS."""
@@ -8180,14 +8247,15 @@
         assert tuple(tags['CameraChipOffset'][10]) == (0.0, 0.0)
         assert tags['PlaneDescriptions'][0].startswith('Acquired from MV-1500')
         assert str(tags['DatetimeCreated'][0]) == (
             '2000-02-02T15:06:02.000783000'
         )
         # assert series properties
         series = tif.series[0]
+        assert series.is_truncated
         assert series.shape == (11, 256, 320)
         assert series.dtype == numpy.uint16
         assert series.axes == 'ZYX'
         assert series.kind == 'stk'
         # assert data
         data = tif.asarray()
         assert isinstance(data, numpy.ndarray)
@@ -8232,14 +8300,15 @@
         assert tuple(tags['StagePosition'][10]) == (0.0, 0.0)
         assert tuple(tags['CameraChipOffset'][10]) == (320.0, 256.0)
         assert str(tags['DatetimeCreated'][0]) == (
             '2000-02-02T15:10:34.000264000'
         )
         # assert series properties
         series = tif.series[0]
+        assert series.is_truncated
         assert series.shape == (11, 128, 160, 3)
         assert series.dtype == numpy.uint8
         assert series.axes == 'ZYXS'
         assert series.kind == 'stk'
         # assert data
         data = tif.asarray()
         assert isinstance(data, numpy.ndarray)
@@ -8555,15 +8624,15 @@
 
 
 @pytest.mark.skipif(
     SKIP_LARGE or SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG,
     reason=REASON,
 )
 def test_read_ndpi_4gb():
-    """Test read > 4GB Hamamatsu NDPI slide, JPEG 103680x188160."""
+    """Test read > 4 GB Hamamatsu NDPI slide, JPEG 103680x188160."""
     fname = private_file('HamamatsuNDPI/103680x188160.ndpi')
     with TiffFile(fname) as tif:
         assert tif.is_ndpi
         assert len(tif.pages) == 8
         assert len(tif.series) == 3
         for page in tif.pages:
             assert page.ndpi_tags['Model'] == 'C13220'
@@ -8941,15 +9010,15 @@
         assert page.shape == (12990, 5741, 3)
         metadata = tif.scn_metadata
         assert metadata.startswith('<?xml version="1.0" encoding="utf-8"?>')
         for series in tif.series[2:]:
             assert series.kind == 'scn'
             assert series.axes == 'CZYX'
             assert series.shape[:2] == (4, 8)
-            assert len(series.levels) in (2, 3, 4, 5)
+            assert len(series.levels) in {2, 3, 4, 5}
             assert len(series.pages) == 32
         # third series
         series = tif.series[2]
         assert series.shape == (4, 8, 946, 993)
         assert_aszarr_method(series)
         assert__str__(tif)
 
@@ -9854,15 +9923,17 @@
     fname = private_file('OME/companion/multifile-Z2.ome.tiff')
     with TiffFile(fname) as tif:
         assert tif.is_ome
         with caplog.at_level(logging.DEBUG):
             assert tif.series[0].kind == 'generic'
             assert 'OME series is BinaryOnly' in caplog.text
 
-    with open(private_file('OME/companion/multifile.companion.ome')) as fh:
+    with open(
+        private_file('OME/companion/multifile.companion.ome'), encoding='utf-8'
+    ) as fh:
         omexml = fh.read()
     with TiffFile(fname, omexml=omexml) as tif:
         assert tif.is_ome
         series = tif.series[0]
         assert series.kind == 'ome'
         image = series.asarray()
 
@@ -10277,15 +10348,15 @@
         assert t['Frames'] == 100.0
         # assert series properties
         series = tif.series[0]
         assert series.shape == (100, 512, 512)
         assert series.dtype == numpy.uint16
         assert series.axes == 'IYX'
         assert series.kind == 'uniform'
-        assert type(series.pages[2]) == TiffFrame
+        assert isinstance(series.pages[2], TiffFrame)
         # assert data
         data = tif.asarray()
         assert data.shape == (100, 512, 512)
         assert data.dtype == numpy.uint16
         assert round(abs(data[50, 256, 256] - 703), 7) == 0
         assert_aszarr_method(tif, data)
         assert_aszarr_method(tif, data, chunkmode='page')
@@ -10945,15 +11016,15 @@
         # assert series properties
         series = tif.series[0]
         assert series.kind == 'imagej'
         assert series.dataoffset is None  # not contiguous
         assert series.shape == (343, 1024, 1024)
         assert series.dtype == numpy.uint8
         assert series.axes == 'IYX'
-        assert type(series.pages[2]) == TiffFrame
+        assert isinstance(series.pages[2], TiffFrame)
         # assert ImageJ tags
         ijmeta = tif.imagej_metadata
         assert ijmeta is not None
         assert ijmeta['SCIFIO'] == '0.42.0'
         assert ijmeta['hyperstack']
         assert ijmeta['images'] == 343
         # assert data
@@ -11797,20 +11868,20 @@
         fei = tif.fei_metadata
         assert fei['User']['User'] == 'supervisor'
         assert fei['System']['DisplayHeight'] == 0.324
         assert_aszarr_method(tif)
         assert__str__(tif)
 
 
-@pytest.mark.skipif(SKIP_PRIVATE or SKIP_LARGE, reason=REASON)
+@pytest.mark.skipif(SKIP_PRIVATE or SKIP_LARGE or SKIP_ZARR, reason=REASON)
 def test_read_mmstack_multifile(caplog):
     """Test read MicroManager 2.0 multi-file, multi-position dataset."""
     # TODO: what version of MicroManager does not write corrupted files?
-    # second ImageDescription tag value is beyond 4GB
-    # MicroManager headers are beyond 4GB
+    # second ImageDescription tag value is beyond 4 GB
+    # MicroManager headers are beyond 4 GB
     # MicroManager display settings are truncated
     fname = private_file('MMStack/NDTiff.index/_4_MMStack_Pos0.ome.tif')
     with TiffFile(fname) as tif:
         assert 'coercing invalid ASCII to bytes' in caplog.text
         assert tif.is_micromanager
         assert tif.is_mmstack
         assert tif.is_ome
@@ -12504,14 +12575,81 @@
         xscale = meta['Scaling']['ScalingXScaling']
         assert xscale.size == 672
         assert xscale[0] == 231.09092712402344
         assert xscale[-1] == 242.59259033203125
         assert__str__(tif)
 
 
+@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+def test_read_agilent():
+    """Test read Agilent Technologies file."""
+    fname = private_file('Agilent/SG11410002_253174651388_S001.tif')
+    with TiffFile(fname) as tif:
+        assert tif.is_agilent
+        assert not tif.is_mdgel
+        assert len(tif.pages) == 4
+        assert len(tif.series) == 2
+        # assert page properties
+        page = tif.pages.first
+        assert page.is_contiguous
+        assert page.photometric == MINISBLACK
+        assert page.imagewidth == 20334
+        assert page.imagelength == 7200
+        assert page.bitspersample == 16
+        assert page.samplesperpixel == 1
+        assert page.tags[285].value == 'Red'
+        assert page.tags[37702].value == 'Unknown'
+        # assert data
+        series = tif.series[0]
+        assert series.shape == (2, 7200, 20334)
+        assert series.asarray()[1, 277, 341] == 24
+        series = tif.series[1]
+        assert series.shape == (2, 2400, 6778)
+        assert series.asarray()[1, 277, 341] == 634
+        assert__str__(tif)
+
+
+@pytest.mark.skipif(SKIP_PUBLIC or SKIP_ZARR, reason=REASON)
+@pytest.mark.parametrize('chunkmode', [0, 2])
+def test_read_selection(chunkmode):
+    """Test read selection via imread."""
+    fname = public_file('tifffile/multiscene_pyramidal.ome.tif')
+    selection = (8, slice(16, 17), slice(None), slice(51, 99), slice(51, 99))
+    # series 0
+    assert_array_equal(
+        imread(fname)[8, 16:17, :, 51:99, 51:99],
+        imread(fname, selection=selection),
+    )
+    # level 1
+    assert_array_equal(
+        imread(fname, series=0, level=1)[8, 16:17, :, 51:99, 51:99],
+        imread(fname, series=0, level=1, selection=selection),
+    )
+    # page 99
+    assert_array_equal(
+        imread(fname, key=99)[51:99, 51:99],
+        imread(fname, key=99, selection=(slice(51, 99), slice(51, 99))),
+    )
+    # series 1
+    assert_array_equal(
+        imread(fname, series=1)[51:99, 51:99],
+        imread(fname, series=1, selection=(slice(51, 99), slice(51, 99))),
+    )
+
+
+@pytest.mark.skipif(SKIP_PRIVATE or SKIP_CODECS, reason=REASON)
+def test_read_selection_filesequence():
+    """Test read selection from file sequence via imread."""
+    fname = private_file('TiffSequence/*.tif')
+    assert_array_equal(
+        imread(fname)[5:8, 51:99, 51:99],
+        imread(fname, selection=(slice(5, 8), slice(51, 99), slice(51, 99))),
+    )
+
+
 def test_read_xarray_page_properties():
     """Test read TiffPage xarray properties."""
     dtype = numpy.uint8
     resolution = (1.1, 2.2)
     with TempFileName('xarray_page_properties') as fname:
         with TiffWriter(fname) as tif:
             # gray
@@ -12734,21 +12872,20 @@
                         tif.write(
                             shape=shape,
                             dtype=dtype,
                             tile=tile,
                             photometric=photometric,
                         )
                     return
-                else:
-                    tif.write(
-                        shape=shape,
-                        dtype=dtype,
-                        tile=tile,
-                        photometric=photometric,
-                    )
+                tif.write(
+                    shape=shape,
+                    dtype=dtype,
+                    tile=tile,
+                    photometric=photometric,
+                )
                 assert__repr__(tif)
             with TiffFile(fname) as tif:
                 assert__str__(tif)
                 image = tif.asarray()
         else:
             data = random_data(dtype, shape)
             imwrite(
@@ -12800,15 +12937,15 @@
         'jpegxr',
         'jpeg2000',
     ],
 )
 @pytest.mark.parametrize('mode', ['gray', 'rgb', 'planar'])
 def test_write_codecs(mode, tile, codec):
     """Test write various compression."""
-    if mode in ('gray', 'planar') and codec == 'webp':
+    if mode in {'gray', 'planar'} and codec == 'webp':
         pytest.xfail("WebP doesn't support grayscale or planar mode")
     level = {'webp': -1, 'jpeg': 99}.get(codec, None)
     if level:
         compressionargs = {'level': level}
     else:
         compressionargs = None
     tile = (16, 16) if tile else None
@@ -12842,31 +12979,31 @@
         )
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == shape[0]
             page = tif.pages.first
             assert not page.is_contiguous
             assert page.compression == enumarg(TIFF.COMPRESSION, codec)
-            assert page.photometric in (photometric, YCBCR)
+            assert page.photometric in {photometric, YCBCR}
             if planarconfig is not None:
                 assert page.planarconfig == planarconfig
             assert page.imagewidth == 31
             assert page.imagelength == 32
             assert page.samplesperpixel == 1 if mode == 'gray' else 3
             # samplesperpixel = page.samplesperpixel
             image = tif.asarray()
-            if codec in ('jpeg',):
+            if codec == 'jpeg':
                 assert_allclose(data, image, atol=10)
             else:
                 assert_array_equal(data, image)
             assert_decode_method(page)
             assert__str__(tif)
         if (
             imagecodecs.TIFF
-            and codec not in ('png', 'jpegxr', 'jpeg2000', 'jpegxl')
+            and codec not in {'png', 'jpegxr', 'jpeg2000', 'jpegxl'}
             and mode != 'planar'
         ):
             im = imagecodecs.imread(fname, index=None)
             # if codec == 'jpeg':
             #     # tiff_decode returns JPEG compressed TIFF as RGBA
             #     im = numpy.squeeze(im[..., :samplesperpixel])
             assert_array_equal(im, numpy.squeeze(image))
@@ -13419,14 +13556,15 @@
             assert len(tif.pages) == 1  # not 4
             page = tif.pages.first
             assert page.is_shaped
             assert page.shape == (5, 6)
             assert '"shape": [4, 5, 6, 1]' in page.description
             assert '"truncated": true' in page.description
             series = tif.series[0]
+            assert series.is_truncated
             assert series.kind == 'shaped'
             assert series.shape == shape
             assert len(series._pages) == 1
             assert len(series.pages) == 1
             data = tif.asarray()
             assert data.shape == shape
             assert_aszarr_method(tif, data)
@@ -13986,15 +14124,15 @@
         (7, 'zlib', None, {'level': 5}),
     ],
 )
 def test_write_compression_args(args):
     """Test compression parameter."""
     i = args[0]
     compressionargs = args[1:]
-    compressed = compressionargs[0] not in (0, 1, NONE)
+    compressed = compressionargs[0] not in {0, 1, NONE}
     if len(compressionargs) == 1:
         compressionargs = compressionargs[0]
 
     data = WRITE_DATA
     with TempFileName(f'compression_args_{i}') as fname:
         if i > 4:
             # TODO: with pytest.warns(DeprecationWarning):
@@ -15911,15 +16049,15 @@
 def test_write_pyramids():
     """Test write two pyramids to shaped file."""
     data = random_data(numpy.uint8, (31, 64, 96, 3))
     with TempFileName('pyramids') as fname:
         with TiffWriter(fname) as tif:
             # use pages
             tif.write(data, tile=(16, 16), photometric=RGB)
-            # interrupt pyramid, e.g. thumbnail
+            # interrupt pyramid, for example thumbnail
             tif.write(data[0, :, :, 0])
             # pyramid levels
             tif.write(
                 data[:, ::2, ::2],
                 tile=(16, 16),
                 subfiletype=1,
                 photometric=RGB,
@@ -16725,14 +16863,15 @@
         with TiffFile(fname, mode='r+') as tif:
             with tif.series[3].aszarr() as store:
                 z = zarr.open(store, mode='r+')
                 with pytest.raises(PermissionError):
                     z[100, 20] = 106
 
 
+@pytest.mark.skipif(SKIP_ZARR, reason=REASON)
 def assert_fsspec(url, data, target_protocol='http'):
     """Assert fsspec ReferenceFileSystem from local http server."""
     mapper = fsspec.get_mapper(
         'reference://', fo=url, target_protocol=target_protocol
     )
     zobj = zarr.open(mapper, mode='r')
     if isinstance(zobj, zarr.Group):
@@ -16854,15 +16993,15 @@
     """Test write fsspec for multi-file OME series."""
     fname = public_file('OME/multifile/multifile-Z1.ome.tiff')
     url = os.path.dirname(fname).replace('\\', '/')
     with TempFileName(
         f'write_fsspec_multifile_{version}{chunkmode}', ext='.json'
     ) as jsonfile:
         # write to file handle
-        with open(jsonfile, 'w') as fh:
+        with open(jsonfile, 'w', encoding='utf-8') as fh:
             with TiffFile(fname) as tif:
                 data = tif.series[0].asarray()
                 with tif.series[0].aszarr(chunkmode=chunkmode) as store:
                     store.write_fsspec(
                         fh, url=url, version=version, templatename='f'
                     )
         mapper = fsspec.get_mapper(
@@ -16872,15 +17011,16 @@
             remote_protocol='file',
         )
         zobj = zarr.open(mapper, mode='r')
         assert_array_equal(zobj[:], data)
 
 
 @pytest.mark.skipif(
-    SKIP_PRIVATE or SKIP_LARGE or SKIP_CODECS or SKIP_ZARR, reason=REASON
+    SKIP_PRIVATE or SKIP_LARGE or SKIP_CODECS or SKIP_ZARR,
+    reason=REASON,
 )
 @pytest.mark.parametrize('version', [1])  # 0,
 def test_write_fsspec_sequence(version):
     """Test write fsspec for multi-file sequence."""
     # https://bbbc.broadinstitute.org/BBBC006
     categories = {'p': {chr(i + 97): i for i in range(25)}}
     ptrn = r'(?:_(z)_(\d+)).*_(?P<p>[a-z])(?P<a>\d+)(?:_(s)(\d))(?:_(w)(\d))'
@@ -17018,15 +17158,15 @@
     'dtype', [numpy.uint8, numpy.uint16, numpy.int16, numpy.float32]
 )
 @pytest.mark.parametrize('byteorder', ['>', '<'])
 def test_write_imagej(byteorder, dtype, shape):
     """Test write ImageJ format."""
     # TODO: test compression and bigtiff ?
     dtype = numpy.dtype(dtype)
-    if dtype != numpy.uint8 and shape[-1] in (3, 4):
+    if dtype != numpy.uint8 and shape[-1] in {3, 4}:
         pytest.xfail('ImageJ only supports uint8 RGB')
     data = random_data(dtype, shape)
     fname = 'imagej_{}_{}_{}'.format(
         {'<': 'le', '>': 'be'}[byteorder], dtype, str(shape).replace(' ', '')
     )
     with TempFileName(fname) as fname:
         imwrite(fname, data, byteorder=byteorder, imagej=True)
@@ -17223,14 +17363,15 @@
             assert page.planarconfig == CONTIG
             assert page.photometric == RGB
             assert page.imagewidth == 61
             assert page.imagelength == 49
             assert page.samplesperpixel == 3
             # assert series properties
             series = tif.series[0]
+            assert series.is_truncated == truncate
             assert series.kind == 'imagej'
             assert series.shape == shape
             assert len(series._pages) == 1
             assert len(series.pages) == 1 if truncate else 210
             assert series.dtype == numpy.uint8
             assert series.axes == 'TZCYXS'
             assert series.get_axes(False) == 'TZCYXS'
@@ -17362,18 +17503,18 @@
         ((2, 3, 4, 5, 6, 7, 33, 31, 3), 'TQCPZRYXS'),
     ],
 )
 def test_write_ome(shape, axes):
     """Test write OME-TIFF format."""
     photometric = None
     planarconfig = None
-    if shape[-1] in (3, 4):
+    if shape[-1] in {3, 4}:
         photometric = RGB
         planarconfig = CONTIG
-    elif shape[-3] in (3, 4):
+    elif shape[-3] in {3, 4}:
         photometric = RGB
         planarconfig = SEPARATE
 
     metadata = {'axes': axes} if axes is not None else {}
     data = random_data(numpy.uint8, shape)
     fname = 'write_ome_{}.ome'.format(str(shape).replace(' ', ''))
     with TempFileName(fname) as fname:
@@ -18292,15 +18433,15 @@
 def test_dependent_roifile():
     """Test roifile.ImagejRoi class."""
     from roifile import ImagejRoi
 
     for roi in ImagejRoi.fromfile(private_file('imagej/IJMetadata.tif')):
         assert roi == ImagejRoi.frombytes(roi.tobytes())
         roi.coordinates()
-        roi.__str__()
+        str(roi)
 
 
 @pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
 def test_dependent_lfdfiles():
     """Test lfdfiles conversion to TIFF."""
     from lfdfiles import LfdFileSequence, SimfcsInt, SimfcsZ64
 
@@ -18515,125 +18656,118 @@
     assert img.current_scene == 'Image:1'
     assert img.shape == (1, 1, 1, 128, 128, 3)
     img.set_scene('Image:0')
     lazy_t1 = img.get_image_dask_data('ZCYX', T=1)
     assert_array_equal(lazy_t1.compute(), t1)
 
 
-@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+@pytest.mark.xfail(reason=REASON)
+@pytest.mark.skipif(SKIP_PUBLIC, reason=REASON)
 def test_dependent_imageio():
     """Test imageio package."""
     # https://github.com/imageio/imageio/blob/master/tests/test_tifffile.py
+    # TODO: use imageio.v3
     try:
-        import imageio
-        from imageio.v2 import (
-            imread,
-            imwrite,
-            mimread,
-            mimwrite,
-            mvolread,
-            volread,
-            volwrite,
-        )
+        import imageio.v2 as iio
     except ImportError:
         pytest.skip('imageio missing')
 
     data = numpy.ones((10, 10, 3), numpy.uint8) * 2
     filename2 = public_file('imageio/multipage_rgb.tif')
     filename3 = public_file('imageio/test_tiff2.tiff')
 
     with TempFileName('depend_imageio') as fname1:
         # one image
-        imwrite(fname1, data)
-        im = imread(fname1)
-        ims = mimread(fname1)
+        iio.imwrite(fname1, data)
+        im = iio.imread(fname1)
+        ims = iio.mimread(fname1)
         assert im.shape == data.shape
         assert_array_equal(im, data)
         assert len(ims) == 1
 
         # multiple images
-        mimwrite(fname1, [data, data, data])
-        im = imread(fname1)
-        ims = mimread(fname1)
+        iio.mimwrite(fname1, [data, data, data])
+        im = iio.imread(fname1)
+        ims = iio.mimread(fname1)
         assert im.shape == data.shape
         assert_array_equal(im, data)
         assert len(ims) == 3
         for i in range(3):
             assert ims[i].shape == data.shape
             assert_array_equal(ims[i], data)
 
         # volumetric data
-        volwrite(fname1, numpy.tile(data, (3, 1, 1, 1)))
-        vol = volread(fname1)
-        vols = mvolread(fname1)
+        iio.volwrite(fname1, numpy.tile(data, (3, 1, 1, 1)))
+        vol = iio.volread(fname1)
+        vols = iio.mvolread(fname1)
         assert vol.shape == (3,) + data.shape
         assert len(vols) == 1 and vol.shape == vols[0].shape
         for i in range(3):
             assert_array_equal(vol[i], data)
 
         # remote channel-first volume rgb (2, 3, 10, 10)
 
-        img = mimread(filename2)
+        img = iio.mimread(filename2)
         assert len(img) == 2
         assert img[0].shape == (3, 10, 10)
 
         # mixed
-        W = imageio.save(fname1)
+        W = iio.save(fname1)
         W.set_meta_data({'planarconfig': 'SEPARATE'})
         assert W.format.name == 'TIFF'
         W.append_data(data)
         W.append_data(data)
         W.close()
         #
-        R = imageio.read(fname1)
+        R = iio.read(fname1)
         assert R.format.name == 'TIFF'
         ims = list(R)  # == [im for im in R]
         assert_array_equal(ims[0], data)
         # fail
         with pytest.raises(IndexError):
             R.get_data(-1)
 
         with pytest.raises(IndexError):
             R.get_data(3)
 
         # ensure imread + imwrite works round trip
-        im1 = imread(fname1)
-        imwrite(filename3, im1)
-        im3 = imread(filename3)
+        im1 = iio.imread(fname1)
+        iio.imwrite(filename3, im1)
+        im3 = iio.imread(filename3)
         assert im1.ndim == 3
         assert im1.shape == im3.shape
         assert_array_equal(im1, im3)
 
         # ensure imread + imwrite works round trip - volume like
-        im1 = numpy.stack(imageio.mimread(fname1))
-        volwrite(filename3, im1)
-        im3 = volread(filename3)
+        im1 = numpy.stack(iio.mimread(fname1))
+        iio.volwrite(filename3, im1)
+        im3 = iio.volread(filename3)
         assert im1.ndim == 4
         assert im1.shape == im3.shape
         assert_array_equal(im1, im3)
 
         # read metadata
-        md = imageio.get_reader(filename2).get_meta_data()
+        md = iio.get_reader(filename2).get_meta_data()
         assert not md['is_imagej']
         assert md['description'] == 'shape=(2,3,10,10)'
         assert md['description1'] == ""
         assert md['datetime'] == datetime.datetime(2015, 5, 9, 9, 8, 29)
         assert md['software'] == 'tifffile.py'
 
         # write metadata
         dt = datetime.datetime(2018, 8, 6, 15, 35, 5)
-        with imageio.get_writer(fname1, software='testsoftware') as w:
+        with iio.get_writer(fname1, software='testsoftware') as w:
             w.append_data(
                 numpy.zeros((10, 10)),
                 meta={'description': 'test desc', 'datetime': dt},
             )
             w.append_data(
                 numpy.zeros((10, 10)), meta={'description': 'another desc'}
             )
-        with imageio.get_reader(fname1) as r:
+        with iio.get_reader(fname1) as r:
             for md in r.get_meta_data(), r.get_meta_data(0):
                 assert 'datetime' in md
                 assert md['datetime'] == dt
                 assert 'software' in md
                 assert md['software'] == 'testsoftware'
                 assert 'description' in md
                 assert md['description'] == 'test desc'
@@ -18656,22 +18790,20 @@
 
     ims = TiffStack_tifffile(fname)
     assert_array_equal(ims.get_frame(2), imread(fname, key=2))
     repr(ims)
     ims.close()
 
 
-@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+@pytest.mark.skipif(SKIP_PRIVATE or SKIP_ZARR, reason=REASON)
 def test_dependent_kerchunk():
     """Test kerchunk package."""
     # https://github.com/fsspec/kerchunk/blob/main/kerchunk/tests/test_tiff.py
     try:
         import kerchunk.tiff
-        import fsspec
-        import zarr
         import pathlib
     except ImportError:
         pytest.skip('kerchunk or dependencies missing')
 
     fname = private_file('kerchunk/lcmap_tiny_cog_2019.tif')
     fname = pathlib.Path(fname).as_uri()
```

### Comparing `tifffile-2023.4.12/tifffile/_imagecodecs.py` & `tifffile-2023.7.4/tifffile/_imagecodecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,18 +307,18 @@
         _bitorder.append(numpy.frombuffer(_bitorder[0], dtype=numpy.uint8))
     if isinstance(data, (bytes, bytearray)):
         return data.translate(_bitorder[0])
     try:
         view = data.view('uint8')
         numpy.take(_bitorder[1], view, out=view)
         return data
-    except ValueError:
+    except ValueError as exc:
         raise NotImplementedError(
             "bitorder_decode of slices requires the 'imagecodecs' package"
-        )
+        ) from exc
     return None
 
 
 def packints_decode(
     data: bytes,
     /,
     dtype: numpy.dtype | str,
```

### Comparing `tifffile-2023.4.12/tifffile/geodb.py` & `tifffile-2023.7.4/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/tifffile/lsm2bin.py` & `tifffile-2023.7.4/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/tifffile/numcodecs.py` & `tifffile-2023.7.4/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/tifffile/tiff2fsspec.py` & `tifffile-2023.7.4/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/tifffile/tiffcomment.py` & `tifffile-2023.7.4/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.4.12/tifffile/tifffile.py` & `tifffile-2023.7.4/tifffile/tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.12
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -92,33 +92,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.7.4
+
+- Pass 4992 tests.
+- Add option to return selection from imread (#200).
+- Fix reading OME series with missing trailing frames (#199).
+- Fix fsspec reference for WebP compressed segments missing alpha channel.
+- Fix linting issues.
+- Detect files written by Agilent Technologies.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2023.4.12
 
-- Pass 4988 tests.
 - Do not write duplicate ImageDescription tags from extratags (breaking).
 - Support multifocal SVS files (#193).
 - Log warning when filtering out extratags.
 - Fix writing OME-TIFF with image description in extratags.
 - Ignore invalid predictor tag value if prediction is not used.
 - Raise KeyError if ZarrStore is missing requested chunk.
 
@@ -231,15 +240,15 @@
 - Convert some warnings to debug messages.
 - Declare all classes final.
 - Add script to generate documentation via Sphinx.
 - Convert docstrings to Google style with Sphinx directives.
 
 2022.5.4
 
-- ...
+- …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 TIFF, the Tagged Image File Format, was created by the Aldus Corporation and
@@ -423,14 +432,20 @@
 array to an interleaved RGB, a planar RGB, or a 3-page grayscale TIFF:
 
 >>> data = numpy.random.randint(0, 255, (3, 3, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb')
 >>> imwrite('temp.tif', data, photometric='rgb', planarconfig='separate')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
+Use the `extrasamples` argument to specify how extra components are
+interpreted, for example, for an RGBA image with unassociated alpha channel:
+
+>>> data = numpy.random.randint(0, 255, (256, 256, 4), 'uint8')
+>>> imwrite('temp.tif', data, photometric='rgb', extrasamples=['unassalpha'])
+
 Write a 3-dimensional NumPy array to a multi-page, 16-bit grayscale TIFF file:
 
 >>> data = numpy.random.randint(0, 2**12, (64, 301, 219), 'uint16')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
 Read the whole image stack from the multi-page TIFF file as NumPy array:
 
@@ -498,15 +513,15 @@
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
 
-Overwrite the value of an existing tag, e.g., XResolution:
+Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
@@ -802,15 +817,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.4.12'
+__version__ = '2023.7.4'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -959,14 +974,15 @@
     files: str
     | os.PathLike[Any]
     | FileHandle
     | BinaryIO
     | Sequence[str | os.PathLike[Any]]
     | None = None,
     *,
+    selection: Any | None = None,  # TODO: type this
     aszarr: bool = False,
     key: int | slice | Iterable[int] | None = None,
     series: int | None = None,
     level: int | None = None,
     squeeze: bool | None = None,
     maxworkers: int | None = None,
     mode: Literal['r', 'r+'] | None = None,
@@ -998,17 +1014,26 @@
 
     The first image series in the file(s) is returned by default.
 
     Parameters:
         files:
             File name, seekable binary stream, glob pattern, or sequence of
             file names. May be *None* if `container` is specified.
+        selection:
+            Subset of image to be extracted.
+            If not None, a Zarr array is created, indexed with the `selection`
+            value, and returned as a NumPy array. Only segments that are part
+            of the selection will be read from file.
+            Refer to the Zarr documentation for valid indices.
+            Depending on selection size, image size, and storage properties,
+            it may be more efficient to read the whole image from file and
+            then index it.
         aszarr:
             Return file sequences, series, or single pages as Zarr store
-            instead of NumPy array.
+            instead of NumPy array if `selection` is None.
         mode, name, offset, size, omexml, _multifile, _useframes:
             Passed to :py:class:`TiffFile`.
         key, series, level, squeeze, maxworkers:
             Passed to :py:meth:`TiffFile.asarray`
             or :py:meth:`TiffFile.aszarr`.
         imread, container, sort, pattern, axesorder, axestiled, categories,\
         ioworkers:
@@ -1031,14 +1056,16 @@
     Returns:
         Images from specified files, series, or pages.
         Zarr store instances must be closed after use.
         See :py:meth:`TiffPage.asarray` for operations that are applied
         (or not) to the image data stored in the file.
 
     """
+    store: ZarrStore
+    aszarr = aszarr or (selection is not None)
     is_flags = parse_kwargs(kwargs, *(k for k in kwargs if k[:3] == 'is_'))
 
     if imread is None and kwargs:
         raise TypeError(
             'imread() got unexpected keyword arguments '
             + ', '.join(f"'{key}'" for key in kwargs)
         )
@@ -1068,25 +1095,28 @@
                 omexml=omexml,
                 _multifile=_multifile,
                 _useframes=_useframes,
                 **is_flags,
             ) as tif:
                 if aszarr:
                     assert key is None or isinstance(key, int)
-                    return tif.aszarr(
+                    store = tif.aszarr(
                         key=key,
                         series=series,
                         level=level,
                         squeeze=squeeze,
                         maxworkers=maxworkers,
                         chunkmode=chunkmode,
                         fillvalue=fillvalue,
                         zattrs=zattrs,
                         multiscales=multiscales,
                     )
+                    if selection is None:
+                        return store
+                    return zarr_selection(store, selection)
                 return tif.asarray(
                     key=key,
                     series=series,
                     level=level,
                     squeeze=squeeze,
                     maxworkers=maxworkers,
                     out=out,
@@ -1113,23 +1143,26 @@
         axesorder=axesorder,
         categories=categories,
         container=container,
         sort=sort,
         **kwargs_notnone(imread=imread),
     ) as imseq:
         if aszarr:
-            return imseq.aszarr(
+            store = imseq.aszarr(
                 axestiled=axestiled,
                 chunkmode=chunkmode,
                 chunkshape=chunkshape,
                 dtype=dtype,
                 fillvalue=fillvalue,
                 zattrs=zattrs,
                 **imread_kwargs,
             )
+            if selection is None:
+                return store
+            return zarr_selection(store, selection)
         return imseq.asarray(
             axestiled=axestiled,
             chunkshape=chunkshape,
             dtype=dtype,
             ioworkers=ioworkers,
             out=out,
             out_inplace=out_inplace,
@@ -1232,15 +1265,15 @@
             datasize = 0
 
     if bigtiff is None:
         bigtiff = (
             datasize > 2**32 - 2**25
             and not imagej
             and not truncate
-            and compression in (None, 0, 1, 'NONE', 'none')
+            and compression in {None, 0, 1, 'NONE', 'none'}
         )
 
     with TiffWriter(
         file,
         bigtiff=bigtiff,
         byteorder=byteorder,
         append=append,
@@ -1396,15 +1429,15 @@
     TiffWriter's main purpose is saving multi-dimensional NumPy arrays in
     TIFF containers, not to create any possible TIFF format.
     Specifically, ExifIFD and GPSIFD tags are not supported.
 
     TiffWriter instances must be closed with :py:meth:`TiffWriter.close`,
     which is automatically called when using the 'with' context manager.
 
-    TiffWriter instances are not thread-safe.
+    TiffWriter instances are not thread-safe. All attributes are read-only.
 
     Parameters:
         file:
             Specifies file to write.
             An empty TIFF file is created if the file does not exist, else
             the file is overwritten with an empty TIFF file unless `append`
             is enabled.
@@ -1434,14 +1467,16 @@
             Use FIJI's Bio-Formats import function for compressed files.
         ome:
             Write OME-TIFF compatible file.
             By default, the OME-TIFF format is used if the file name extension
             contains '.ome.', `imagej` is not enabled, and the `description`
             argument in the first call of :py:meth:`TiffWriter.write` is not
             specified.
+            The format supports multiple, up to 9 dimensional image series.
+            The default axes order is TZC(S)YX(S).
             Refer to the OME model for restrictions of this format.
         shaped:
             Write tifffile "shaped" compatible file.
             The shape of multi-dimensional images is stored in JSON format in
             a ImageDescription tag of the first page of a series.
             This is the default format used by tifffile unless `imagej` or
             `ome` are enabled or ``metadata=None`` is passed to
@@ -1510,17 +1545,17 @@
                             )
                     finally:
                         fh.seek(pos)
                     append = True
             except (OSError, FileNotFoundError):
                 append = False
 
-        if byteorder in (None, '=', '|'):
+        if byteorder in {None, '=', '|'}:
             byteorder = '<' if sys.byteorder == 'little' else '>'
-        elif byteorder not in ('<', '>'):
+        elif byteorder not in {'<', '>'}:
             raise ValueError(f'invalid byteorder {byteorder}')
 
         if byteorder == '<':
             self.tiff = TIFF.BIG_LE if bigtiff else TIFF.CLASSIC_LE
         else:
             self.tiff = TIFF.BIG_BE if bigtiff else TIFF.CLASSIC_BE
 
@@ -1727,17 +1762,17 @@
                 RGB(A), uint8 or 12-bit uint16.
                 JPEG compression is experimental. JPEG markers and TIFF tags
                 may not match.
                 Only a limited set of compression schemes are implemented.
                 'ZLIB' is short for ADOBE_DEFLATE.
                 The value is written to the Compression tag.
             compressionargs:
-                Extra arguments passed to compression codec, e.g., compression
-                level. Refer to the Imagecodecs implementation for supported
-                arguments.
+                Extra arguments passed to compression codec, for example,
+                compression level. Refer to the Imagecodecs implementation
+                for supported arguments.
             predictor:
                 Horizontal differencing operator applied to image data before
                 compression.
                 By default, no operator is applied.
                 Predictors can only be used with certain compression schemes
                 and data types.
                 The value is written to the Predictor tag.
@@ -1869,16 +1904,16 @@
                 Maximum number of threads to concurrently compress tiles
                 or strips.
                 If *1*, multi-threading is disabled.
                 By default, multithreading is disabled for small segments
                 <8 KB and PackBits compression. Else, up to half the CPU
                 cores are used.
                 Using multiple threads can significantly speed up this
-                function if the bottleneck is encoding the data, e.g., in case
-                of large JPEG compressed tiles.
+                function if the bottleneck is encoding the data, for example,
+                in case of large JPEG compressed tiles.
                 If the bottleneck is I/O or pure Python code, using multiple
                 threads might be detrimental.
             returnoffset:
                 Return offset and number of bytes of memory-mappable image
                 data in file.
 
         Returns:
@@ -1993,15 +2028,15 @@
                 and compression[0] in (None, 0, 1, 'NONE', 'none')
             )
         ):
             compression = False
 
         if not predictor or (
             not isinstance(predictor, bool)  # because True == 1
-            and predictor in ('NONE', 'none', 1)
+            and predictor in {'NONE', 'none', 1}
         ):
             predictor = False
 
         inputshape = datashape
 
         packints = (
             bitspersample is not None
@@ -2024,15 +2059,15 @@
                 self._write_remaining_pages()
 
                 if self._imagej:
                     raise ValueError(
                         'the ImageJ format does not support '
                         'non-contiguous series'
                     )
-                elif self._omexml is not None:
+                if self._omexml is not None:
                     if self._subifdslevel < 0:
                         # add image to OME-XML
                         assert self._storedshape is not None
                         assert self._metadata is not None
                         self._omexml.addimage(
                             dtype=self._datadtype,
                             shape=self._datashape[
@@ -2065,15 +2100,15 @@
                         )
 
                 self._datashape = None
                 self._colormap = None
 
             elif compression or packints or tile:
                 raise ValueError(
-                    'contiguous cannot be used with compression, tiles, etc.'
+                    'contiguous mode cannot be used with compression or tiles'
                 )
 
             else:
                 # consecutive mode
                 # write all data, write IFDs/tags later
                 self._datashape = (self._datashape[0] + 1,) + datashape
                 offset = fh.tell()
@@ -2172,15 +2207,15 @@
             compression = True
         else:
             compressiontag = 1
             compression = False
 
         if compressiontag == 1:
             compressionargs = {}
-        elif compressiontag in (33003, 33004, 33005, 34712):
+        elif compressiontag in {33003, 33004, 33005, 34712}:
             # JPEG2000: use J2K instead of JP2
             compressionargs['codecformat'] = 0  # OPJ_CODEC_J2K
 
         if predictor:
             if not compression:
                 raise ValueError('cannot use predictor without compression')
             if compressiontag in TIFF.IMAGE_COMPRESSIONS:
@@ -2198,19 +2233,19 @@
                     raise ValueError(
                         f'cannot use predictor with {datadtype!r}'
                     )
             else:
                 predictor = enumarg(PREDICTOR, predictor)
                 if (
                     datadtype.kind in 'iu'
-                    and predictor.value not in (2, 34892, 34893)
+                    and predictor.value not in {2, 34892, 34893}
                     and datadtype.itemsize <= 4
                 ) or (
                     datadtype.kind == 'f'
-                    and predictor.value not in (3, 34894, 34895)
+                    and predictor.value not in {3, 34894, 34895}
                 ):
                     raise ValueError(
                         f'cannot use {predictor!r} with {datadtype!r}'
                     )
                 predictortag = predictor.value
         else:
             predictortag = 1
@@ -2269,15 +2304,15 @@
             else:
                 axes = metadata.get('axes', None)
             ijshape = imagej_shape(datashape, rgb=ijrgb, axes=axes)
             if planarconfig == SEPARATE:
                 raise ValueError(
                     'the ImageJ format does not support planar samples'
                 )
-            if ijshape[-1] in (3, 4):
+            if ijshape[-1] in {3, 4}:
                 photometric = RGB
             elif photometric is None:
                 photometric = MINISBLACK
                 planarconfig = None
             planarconfig = CONTIG if ijrgb else None
 
         # verify colormap and indices
@@ -2327,36 +2362,36 @@
 
         if photometric is None:
             deprecate = False
             photometric = MINISBLACK
             if bilevel:
                 photometric = MINISWHITE
             elif planarconfig == CONTIG:
-                if ndim > 2 and shape[-1] in (3, 4):
+                if ndim > 2 and shape[-1] in {3, 4}:
                     photometric = RGB
                     deprecate = datadtypechar not in 'BH'
             elif planarconfig == SEPARATE:
-                if volumetric and ndim > 3 and shape[-4] in (3, 4):
+                if volumetric and ndim > 3 and shape[-4] in {3, 4}:
                     photometric = RGB
                     deprecate = True
-                elif ndim > 2 and shape[-3] in (3, 4):
+                elif ndim > 2 and shape[-3] in {3, 4}:
                     photometric = RGB
                     deprecate = True
-            elif ndim > 2 and shape[-1] in (3, 4):
+            elif ndim > 2 and shape[-1] in {3, 4}:
                 photometric = RGB
                 planarconfig = CONTIG
                 deprecate = datadtypechar not in 'BH'
             elif self._imagej or self._ome:
                 photometric = MINISBLACK
                 planarconfig = None
-            elif volumetric and ndim > 3 and shape[-4] in (3, 4):
+            elif volumetric and ndim > 3 and shape[-4] in {3, 4}:
                 photometric = RGB
                 planarconfig = SEPARATE
                 deprecate = True
-            elif ndim > 2 and shape[-3] in (3, 4):
+            elif ndim > 2 and shape[-3] in {3, 4}:
                 photometric = RGB
                 planarconfig = SEPARATE
                 deprecate = True
 
             if deprecate:
                 if planarconfig == CONTIG:
                     msg = 'contiguous samples', 'parameter is'
@@ -2508,15 +2543,15 @@
                 storedshape.extrasamples = storedshape.samples - 1
 
         if subfiletype is not None and subfiletype & 0b100:
             # FILETYPE_MASK
             if not (
                 bilevel
                 and storedshape.samples == 1
-                and photometric in (0, 1, 4)
+                and photometric in {0, 1, 4}
             ):
                 raise ValueError('invalid SubfileType MASK')
             photometric = PHOTOMETRIC.MASK
 
         packints = False
         if bilevel:
             if bitspersample is not None and bitspersample != 1:
@@ -2624,15 +2659,15 @@
                 'prop',
             )
 
             for t in imagej_metadata_tag(ijmetadata, byteorder):
                 addtag(tags, *t)
             description = imagej_description(
                 inputshape,
-                rgb=storedshape.contig_samples in (3, 4),
+                rgb=storedshape.contig_samples in {3, 4},
                 colormaped=self._colormap is not None,
                 **self._metadata,
             )
             description += '\x00' * 64  # add buffer for in-place update
         elif self._tifffile and (metadata or metadata == {}):
             if self._truncate:
                 self._metadata.update(truncated=True)
@@ -2769,21 +2804,21 @@
 
         if jpegtables is not None:
             addtag(tags, 347, 7, len(jpegtables), jpegtables)
 
         if (
             compressiontag == 7
             and storedshape.planarconfig == 1
-            and photometric in (RGB, YCBCR)
+            and photometric in {RGB, YCBCR}
         ):
             # JPEG compression with subsampling
             # TODO: use JPEGTables for multiple tiles or strips
             if subsampling is None:
                 subsampling = (2, 2)
-            elif subsampling not in ((1, 1), (2, 1), (2, 2), (4, 1)):
+            elif subsampling not in {(1, 1), (2, 1), (2, 2), (4, 1)}:
                 raise ValueError(
                     f'invalid subsampling factors {subsampling!r}'
                 )
             maxsampling = max(subsampling) * 8
             if tile and (tile[-1] % maxsampling or tile[-2] % maxsampling):
                 raise ValueError(f'tile shape not a multiple of {maxsampling}')
             if storedshape.extrasamples > 1:
@@ -2804,15 +2839,15 @@
                         tags,
                         532,
                         5,
                         6,
                         (0, 1, 255, 1, 128, 1, 255, 1, 128, 1, 255, 1),
                     )
         else:
-            if subsampling not in (None, (1, 1)):
+            if subsampling not in {None, (1, 1)}:
                 log_warning(
                     f'{self!r} cannot apply subsampling {subsampling!r}'
                 )
             subsampling = None
             maxsampling = 1
             addtag(
                 tags, 262, 3, 1, photometric.value
@@ -3028,15 +3063,15 @@
 
         if bilevel:
             if compressiontag == 1:
 
                 def compressionfunc(data, axis=compressionaxis) -> bytes:
                     return numpy.packbits(data, axis=axis).tobytes()
 
-            elif compressiontag in (5, 32773):
+            elif compressiontag in {5, 32773}:
                 # LZW, PackBits
                 def compressionfunc(
                     data,
                     compressor=TIFF.COMPRESSORS[compressiontag],
                     axis=compressionaxis,
                     kwargs=compressionargs,
                 ) -> bytes:
@@ -3526,22 +3561,24 @@
                 if pos % 2:
                     # tag value is expected to begin on word boundary
                     ifd.write(b'\x00')
                     pos += 1
                 ifd.seek(offset)
                 try:
                     ifd.write(pack(offsetformat, fhpos + pos))
-                except Exception:  # struct.error
+                except Exception as exc:  # struct.error
                     if self._imagej:
                         warnings.warn(
                             f'{self!r} truncating ImageJ file', UserWarning
                         )
                         self._truncate = True
                         return
-                    raise ValueError('data too large for non-BigTIFF file')
+                    raise ValueError(
+                        'data too large for non-BigTIFF file'
+                    ) from exc
                 ifd.seek(pos)
                 ifd.write(value)
                 if code == self._dataoffsetstag:
                     # save strip/tile offsets for later updates
                     dataoffsetsoffset = offset, pos
                 elif code == 330:
                     # save subifds offsets for later updates
@@ -3672,15 +3709,15 @@
             return
         # elif self._subifdslevel >= 0:
         #     # don't write metadata to SubIFDs
         #     return
         elif self._imagej:
             assert self._metadata is not None
             colormapped = self._colormap is not None
-            isrgb = self._storedshape.samples in (3, 4)
+            isrgb = self._storedshape.samples in {3, 4}
             description = imagej_description(
                 self._datashape,
                 rgb=isrgb,
                 colormaped=colormapped,
                 **self._metadata,
             )
         elif not self._tifffile:
@@ -3763,15 +3800,15 @@
             rawcount = count
 
         elif count is None:
             raise ValueError('invalid count')
         else:
             count = int(count)
 
-        if datatype in (5, 10):  # rational
+        if datatype in {5, 10}:  # rational
             count *= 2
             dataformat = dataformat[-1]
 
         ifdentry = [
             pack('HH', code, datatype),
             pack(self.tiff.offsetformat, rawcount),
         ]
@@ -3848,50 +3885,50 @@
             or numchunks < 2
             or chunksize < 1024
             or compression == 48124  # Jetraw is not thread-safe?
         ):
             return 1
         # the following is based on benchmarking RGB tile sizes vs maxworkers
         # using a (8228, 11500, 3) uint8 WSI slide:
-        if chunksize < 131072 and compression in (
+        if chunksize < 131072 and compression in {
             7,  # JPEG
             33007,  # ALT_JPG
             32773,  # PackBits
             34887,  # LERC
-        ):
+        }:
             return 1
-        if chunksize < 32768 and compression in (
+        if chunksize < 32768 and compression in {
             5,  # LZW
             8,  # zlib
             32946,  # zlib
             50000,  # zstd
             50013,  # zlib/pixtiff
-        ):
+        }:
             # zlib,
             return 1
-        if chunksize < 8192 and compression in (
+        if chunksize < 8192 and compression in {
             34934,  # JPEG XR
             22610,  # JPEG XR
             34933,  # PNG
-        ):
+        }:
             return 1
-        if chunksize < 2048 and compression in (
+        if chunksize < 2048 and compression in {
             33003,  # JPEG2000
             33004,  # JPEG2000
             33005,  # JPEG2000
             34712,  # JPEG2000
             50002,  # JPEG XL
-        ):
+        }:
             return 1
-        if chunksize < 1024 and compression in (
+        if chunksize < 1024 and compression in {
             34925,  # LZMA
             50001,  # WebP
-        ):
+        }:
             return 1
-        if compression in (34887,):  # LERC
+        if compression == 34887:  # LERC
             # limit to 4 threads
             return min(numchunks, 4)
         return min(numchunks, TIFF.MAXWORKERS)
 
     def __enter__(self) -> TiffWriter:
         return self
 
@@ -3922,16 +3959,16 @@
         offset:
             Start position of embedded file.
             The default is the current file position.
         size:
             Size of embedded file. The default is the number of bytes
             from the `offset` to the end of the file.
         omexml:
-            OME metadata in XML format, e.g., from external companion file
-            or sanitized XML overriding XML in file.
+            OME metadata in XML format, for example, from external companion
+            file or sanitized XML overriding XML in file.
         _multifile, _useframes, _parent:
             Internal use.
         **is_flags:
             Override `TiffFile.is_` flags, for example:
 
             ``is_ome=False``: disable processing of OME-XML metadata.
             ``is_lsm=False``: disable special handling of LSM files.
@@ -3983,15 +4020,15 @@
         for key, value in is_flags.items():
             if key[:3] == 'is_' and key[3:] in TIFF.FILE_FLAGS:
                 if value is not None:
                     setattr(self, key, bool(value))
             else:
                 raise TypeError(f'unexpected keyword argument: {key}')
 
-        if mode not in (None, 'r', 'r+', 'rb', 'r+b'):
+        if mode not in {None, 'r', 'r+', 'rb', 'r+b'}:
             raise ValueError(f'invalid mode {mode!r}')
 
         fh = FileHandle(file, mode=mode, name=name, offset=offset, size=size)
         self._fh = fh
         self._multifile = True if _multifile is None else bool(_multifile)
         self._files = {fh.name: self}
         self._decoders = {}
@@ -4005,16 +4042,16 @@
             self.is_ome = True
 
         try:
             fh.seek(0)
             header = fh.read(4)
             try:
                 byteorder = {b'II': '<', b'MM': '>', b'EP': '<'}[header[:2]]
-            except KeyError:
-                raise TiffFileError(f'not a TIFF file {header!r}')
+            except KeyError as exc:
+                raise TiffFileError(f'not a TIFF file {header!r}') from exc
 
             version = struct.unpack(byteorder + 'H', header[2:4])[0]
             if version == 43:
                 # BigTiff
                 offsetsize, zero = struct.unpack(byteorder + 'HH', fh.read(4))
                 if zero != 0 or offsetsize != 8:
                     raise TiffFileError(
@@ -4038,15 +4075,15 @@
                     self.tiff = TIFF.CLASSIC_LE
             elif version == 0x4E31:
                 # NIFF
                 if byteorder == '>':
                     raise TiffFileError('invalid NIFF file')
                 log_warning(f'{self!r} NIFF format not supported')
                 self.tiff = TIFF.CLASSIC_LE
-            elif version == 0x55 or version == 0x4F52 or version == 0x5352:
+            elif version in {0x55, 0x4F52, 0x5352}:
                 # Panasonic or Olympus RAW
                 log_warning(
                     f'{self!r} RAW format 0x{version:04X} not supported'
                 )
                 if byteorder == '>':
                     self.tiff = TIFF.CLASSIC_BE
                 else:
@@ -4148,30 +4185,30 @@
                 By default, the image of the specified `series` and `level`
                 is returned.
                 If not *None*, the images from the specified pages in the
                 whole file (if `series` is *None*) or a specified series are
                 returned as a stacked array.
                 Requesting an array from multiple pages that are not
                 compatible wrt. shape, dtype, compression etc. is undefined,
-                i.e., may crash or return incorrect values.
+                that is, it may crash or return incorrect values.
             series:
                 Specifies which series of pages to return as array.
                 The default is 0.
             level:
                 Specifies which level of multi-resolution series to return
                 as array. The default is 0.
             squeeze:
                 If *True*, remove all length-1 dimensions (except X and Y)
                 from array.
                 If *False*, single pages are returned as 5D array of shape
                 :py:attr:`TiffPage.shaped`.
                 For series, the shape of the returned array also includes
                 singlet dimensions specified in some file formats.
-                E.g., ImageJ series, and most commonly also OME series, are
-                returned in TZCYXS order.
+                For example, ImageJ series and most commonly also OME series,
+                are returned in TZCYXS order.
                 By default, all but `"shaped"` series are squeezed.
             out:
                 Specifies how image array is returned.
                 By default, a new NumPy array is created.
                 If a *numpy.ndarray*, a writable array to which the image
                 is copied.
                 If *'memmap'*, directly memory-map the image data in the
@@ -4182,17 +4219,17 @@
             maxworkers:
                 Maximum number of threads to concurrently decode data from
                 multiple pages or compressed segments.
                 By default, up to half the CPU cores are used.
                 If *1*, multi-threading is disabled.
                 Reading data from file is limited to a single thread.
                 Using multiple threads can significantly speed up this
-                function if the bottleneck is decoding compressed data, e.g.,
-                in case of large LZW compressed LSM files or JPEG compressed
-                tiled slides.
+                function if the bottleneck is decoding compressed data,
+                for example, in case of large LZW compressed LSM files or
+                JPEG compressed tiled slides.
                 If the bottleneck is I/O or pure Python code, using multiple
                 threads might be detrimental.
 
         Returns:
             Images from specified pages. See `TiffPage.asarray`
             for operations that are applied (or not) to the image data
             stored in the file.
@@ -4293,16 +4330,16 @@
                 raise ValueError('page is None')
             result.shape = page0.shape if squeeze else page0.shaped
         else:
             if squeeze is None:
                 squeeze = True
             try:
                 page0 = next(p for p in pages if p is not None)
-            except StopIteration:
-                raise ValueError('pages are all None')
+            except StopIteration as exc:
+                raise ValueError('pages are all None') from exc
             assert page0 is not None
             result.shape = (-1,) + (page0.shape if squeeze else page0.shaped)
         return result
 
     def aszarr(
         self,
         key: int | None = None,
@@ -4341,14 +4378,16 @@
         if series is None:
             pages = self.pages
         else:
             if not isinstance(series, TiffPageSeries):
                 series = self.series[series]
             if key is None:
                 return series.aszarr(level=level, **kwargs)
+            if level is not None:
+                series = series.levels[level]
             pages = series
 
         if isinstance(key, (int, numpy.integer)):
             page: TiffPage | TiffFrame = pages[key]
             return page.aszarr(**kwargs)
         raise TypeError('key must be an integer index')
 
@@ -4402,15 +4441,15 @@
                 break
         if not series:
             series = self._series_generic()
 
         self.pages.useframes = useframes
         self.pages.set_keyframe(keyframe)
 
-        # remove empty series, e.g., in MD Gel files
+        # remove empty series, for example, in MD Gel files
         # series = [s for s in series if product(s.shape) > 0]
         assert series is not None
         for i, s in enumerate(series):
             s.index = i
         return series
 
     def _series_uniform(self) -> list[TiffPageSeries] | None:
@@ -4488,15 +4527,16 @@
             series.append(
                 TiffPageSeries(
                     pagelist, shape, page.dtype, axes, kind='generic'
                 )
             )
 
         self.is_uniform = len(series) == 1
-        pyramidize_series(series)
+        if not self.is_agilent:
+            pyramidize_series(series)
         return series
 
     def _series_shaped(self) -> list[TiffPageSeries] | None:
         """Return image series in tifffile "shaped" formatted file."""
         # TODO: all series need to have JSON metadata for this to succeed
 
         def append(
@@ -4758,15 +4798,15 @@
             page_list = [page]
         else:
             page_list = pages[:]
 
         shape: tuple[int, ...]
         axes: str
 
-        if order in ('czt', 'default'):
+        if order in {'czt', 'default'}:
             axes = 'TZC'
             shape = (frames, slices, channels)
         elif order == 'ctz':
             axes = 'ZTC'
             shape = (slices, frames, channels)
         elif order == 'zct':
             axes = 'TCZ'
@@ -4857,19 +4897,21 @@
                 #     framedata.get('SI.hStackManager.numSlices', None),
                 # )
                 # if slices is None:
                 #     raise ValueError('unable to determine numSlices')
                 slices = None
                 try:
                     frames = int(framedata['SI.hStackManager.framesPerSlice'])
-                except Exception:
+                except Exception as exc:
                     # framesPerSlice is inf
                     slices = 1
                     if len(pages) % channels:
-                        raise ValueError('unable to determine framesPerSlice')
+                        raise ValueError(
+                            'unable to determine framesPerSlice'
+                        ) from exc
                     frames = len(pages) // channels
                 if slices is None:
                     slices = max(len(pages) // (frames * channels), 1)
                 shape = (slices, frames, channels) + page.shape
                 axes = 'ZTC' + page.axes
             except Exception as exc:
                 log_warning(
@@ -4915,15 +4957,15 @@
         meta = self.mdgel_metadata
         if meta is None:
             return None
         transform: Callable[[NDArray[Any]], NDArray[Any]] | None
         self.pages.useframes = False
         self.pages.set_keyframe(0)
 
-        if meta['FileTag'] in (2, 128):
+        if meta['FileTag'] in {2, 128}:
             dtype = numpy.dtype('float32')
             scale = meta['ScalePixel']
             scale = scale[0] / scale[1]  # rational
             if meta['FileTag'] == 2:
                 # squary root data format
                 def transform(a: NDArray[Any], /) -> NDArray[Any]:
                     return a.astype('float32') ** 2 * scale
@@ -5514,30 +5556,34 @@
                             try:
                                 if not self.filehandle.is_file:
                                     raise ValueError
                                 tif = TiffFile(
                                     os.path.join(dirname, fname), _parent=self
                                 )
                                 load_pages(tif)
-                            except (OSError, FileNotFoundError, ValueError):
+                            except (
+                                OSError,
+                                FileNotFoundError,
+                                ValueError,
+                            ) as exc:
                                 if files_missing == 0:
                                     log_warning(
                                         f'{self!r} OME series failed to read '
                                         f'{fname!r}. Missing data are zeroed'
                                     )
                                 files_missing += 1
                                 # assume that size is same as in previous file
                                 # if no NumPlanes or PlaneCount are given
                                 if num:
                                     size = num
                                 elif size == -1:
                                     raise ValueError(
                                         'OME series missing '
                                         'NumPlanes or PlaneCount'
-                                    )
+                                    ) from exc
                                 ifds.extend([None] * (size + idx - len(ifds)))
                                 break
                             self._files[uuid.text] = tif
                             tif.close()
                         pages = self._files[uuid.text].pages
                         try:
                             size = num if num else len(pages)
@@ -5605,28 +5651,35 @@
                     else:
                         shape = shape[:-2] + [spp] + shape[-2:]
                         axes = axes[:-2] + 'S' + axes[-2:]
                 if 'S' not in axes:
                     shape += [1]
                     axes += 'S'
 
-                # there might be more pages in the file than referenced in XML
-                # e.g., Nikon-cell011.ome.tif
+                # number of pages in the file might mismatch XML metadata, for
+                # example Nikon-cell011.ome.tif or stack_t24_y2048_x2448.tiff
                 size = max(product(shape) // keyframe.size, 1)
-                if size != len(ifds):
+                if size < len(ifds):
                     log_warning(
                         f'{self!r} '
                         f'OME series expected {size} frames, got {len(ifds)}'
                     )
                     ifds = ifds[:size]
+                elif size > len(ifds):
+                    log_warning(
+                        f'{self!r} '
+                        f'OME series is missing {size - len(ifds)} frames.'
+                        ' Missing data are zeroed'
+                    )
+                    ifds.extend([None] * (size - len(ifds)))
 
                 # FIXME: this implementation assumes the last dimensions are
                 # stored in TIFF pages. Apparently that is not always the case.
-                # E.g. TCX (20000, 2, 500) is stored in 2 pages of (20000, 500)
-                # in 'Image 7.ome_h00.tiff'.
+                # For example, TCX (20000, 2, 500) is stored in 2 pages of
+                # (20000, 500) in 'Image 7.ome_h00.tiff'.
                 # For now, verify that shapes of keyframe and series match.
                 # If not, skip series.
                 squeezed = _squeeze_axes(shape, axes)[0]
                 if keyframe.shape != tuple(squeezed[-len(keyframe.shape) :]):
                     log_warning(
                         f'{self!r} OME series '
                         'cannot handle discontiguous storage (%s != %s)',
@@ -6510,16 +6563,16 @@
         except IndexError:
             return False
         if page.subifds:
             return False
         if page.is_scanimage or page.is_nih:
             return True
         i = 0
+        useframes = pages.useframes
         try:
-            useframes = pages.useframes
             pages.useframes = False
             h = page.hash
             for i in (1, 7, -1):
                 if pages[i].aspage().hash != h:
                     return False
         except IndexError:
             return i == 1  # single page TIFF is uniform
@@ -7002,16 +7055,16 @@
         )
 
 
 @final
 class TiffPages:
     """Sequence of TIFF image file directories (IFD chain).
 
-    TiffPages instances have a state (cache, keyframe, etc.) and are not
-    thread-safe.
+    TiffPages instances have a state, such as a cache and keyframe, and are not
+    thread-safe. All attributes are read-only.
 
     Parameters:
         arg:
             If a *TiffFile*, the file position must be at offset to offset to
             TiffPage.
             If a *TiffPage* or *TiffFrame*, page offsets are read from the
             SubIFDs tag.
@@ -7575,15 +7628,15 @@
         return f'<tifffile.TiffPages @{self._offset}>'
 
 
 @final
 class TiffPage:
     """TIFF image file directory (IFD).
 
-    TiffPage instances are not thread-safe.
+    TiffPage instances are not thread-safe. All attributes are read-only.
 
     Parameters:
         parent:
             TiffFile instance to read page from.
             The file handle position must be at an offset to an IFD structure.
         index:
             Index of page in IFD tree.
@@ -7784,15 +7837,15 @@
         if not tags:
             return  # found in FIBICS
 
         for code, name in TIFF.TAG_ATTRIBUTES.items():
             value = tags.valueof(code)
             if value is None:
                 continue
-            if (code == 270 or code == 305) and not isinstance(value, str):
+            if code in {270, 305} and not isinstance(value, str):
                 # wrong string type for software or description
                 continue
             setattr(self, name, value)
 
         value = tags.valueof(270, index=1)
         if isinstance(value, str):
             self.description1 = value
@@ -7876,17 +7929,17 @@
                 # RGB -> YCbCr
                 self.photometric = PHOTOMETRIC.YCBCR
             if 258 not in tags:
                 # BitsPerSample missing
                 self.bitspersample = 8
             if 277 not in tags:
                 # SamplesPerPixel missing
-                if self.photometric in (2, 6):
+                if self.photometric in {2, 6}:
                     self.samplesperpixel = 3
-                elif self.photometric in (0, 1):
+                elif self.photometric in {0, 1}:
                     self.samplesperpixel = 3
 
         elif self.is_lsm or (self.index != 0 and self.parent.is_lsm):
             # correct non standard LSM bitspersample tags
             tags[258]._fix_lsm_bitspersample()
             if self.compression == 1 and self.predictor != 1:
                 # work around bug in LSM510 software
@@ -8217,15 +8270,15 @@
                     raise ValueError(
                         f'sample formats do not match {tag.value}'
                     )
 
                 return cache(decode_raise_sampleformat)
 
         if self.is_subsampled and (
-            self.compression not in (6, 7, 34892, 33007)
+            self.compression not in {6, 7, 34892, 33007}
             or self.planarconfig == 2
         ):
 
             def decode_raise_subsampling(*args, **kwargs):
                 raise NotImplementedError(
                     'chroma subsampling not supported without JPEG compression'
                 )
@@ -8235,15 +8288,15 @@
         if self.compression == 50001 and self.samplesperpixel == 4:
             # WebP segments may be missing all-opaque alpha channel
             def decompress_webp_rgba(data, out=None):
                 return imagecodecs.webp_decode(data, hasalpha=True, out=out)
 
             decompress = decompress_webp_rgba
 
-        # normalize segments shape to [depth, length, length, contig]
+        # normalize segments shape to [depth, length, width, contig]
         if self.is_tiled:
             stshape = (
                 self.tiledepth,
                 self.tilelength,
                 self.tilewidth,
                 self.samplesperpixel if self.planarconfig == 1 else 1,
             )
@@ -8419,15 +8472,15 @@
 
             def pad_none(
                 shape: tuple[int, int, int, int], /
             ) -> tuple[int, int, int, int]:
                 # return shape of strip
                 return (shape[0], stlength, shape[2], shape[3])
 
-        if self.compression in (6, 7, 34892, 33007):
+        if self.compression in {6, 7, 34892, 33007}:
             # JPEG needs special handling
             if self.fillorder == 2:
                 log_debug(f'{self!r} disabling LSB2MSB for JPEG')
             if unpredict:
                 log_debug(f'{self!r} disabling predictor for JPEG')
             if 28672 in self.tags:  # SonyRawFileType
                 log_warning(
@@ -8563,15 +8616,15 @@
                 f'{self.parent.byteorder}f{dtype.itemsize // 2}'
             )
 
             def unpack(data: bytes, /) -> NDArray[Any]:
                 # return complex integer as numpy.complex
                 return numpy.frombuffer(data, itype).astype(ftype).view(dtype)
 
-        elif self.bitspersample in (8, 16, 32, 64, 128):
+        elif self.bitspersample in {8, 16, 32, 64, 128}:
             # regular data types
 
             if (self.bitspersample * stwidth * samples) % 8:
                 raise ValueError('data and sample size mismatch')
             if self.predictor == 3:  # PREDICTOR.FLOATINGPOINT
                 # floating-point horizontal differencing decoder needs
                 # raw byte order
@@ -8579,21 +8632,21 @@
 
             def unpack(data: bytes, /) -> NDArray[Any]:
                 # return numpy array from buffer
                 try:
                     # read only numpy array
                     return numpy.frombuffer(data, dtype)
                 except ValueError:
-                    # e.g., LZW strips may be missing EOI
+                    # for example, LZW strips may be missing EOI
                     bps = self.bitspersample // 8
                     size = (len(data) // bps) * bps
                     return numpy.frombuffer(data[:size], dtype)
 
         elif isinstance(self.bitspersample, tuple):
-            # e.g., RGB 565
+            # for example, RGB 565
             def unpack(data: bytes, /) -> NDArray[Any]:
                 # return numpy array from packed integers
                 return unpack_rgb(data, dtype, self.bitspersample)
 
         elif self.bitspersample == 24 and dtype.char == 'f':
             # float24
             if unpredict is not None:
@@ -8693,15 +8746,15 @@
         fh = self.parent.filehandle
         if lock is None:
             lock = fh.lock
         if _fullsize is None:
             _fullsize = keyframe.is_tiled
 
         decodeargs: dict[str, Any] = {'_fullsize': bool(_fullsize)}
-        if keyframe.compression in (6, 7, 34892, 33007):  # JPEG
+        if keyframe.compression in {6, 7, 34892, 33007}:  # JPEG
             decodeargs['jpegtables'] = self.jpegtables
             decodeargs['jpegheader'] = keyframe.jpegheader
 
         if func is None:
 
             def decode(args, decodeargs=decodeargs, decode=keyframe.decode):
                 return decode(*args, **decodeargs)
@@ -8914,15 +8967,15 @@
                         s, d : d + shape[0], h : h + shape[1], w : w + shape[2]
                     ] = segment[
                         : keyframe.imagedepth - d,
                         : keyframe.imagelength - h,
                         : keyframe.imagewidth - w,
                     ]
                 # except IndexError:
-                #     pass  # corrupted file, e.g., with too many strips
+                #     pass  # corrupted file, for example, with too many strips
 
             for _ in self.segments(
                 func=func,
                 lock=lock,
                 maxworkers=maxworkers,
                 sort=True,
                 _fullsize=False,
@@ -9365,15 +9418,15 @@
         ``offset=TiffPage.dataoffsets[0]`` with ``size=TiffPage.nbytes``.
         Excludes prediction and fillorder.
 
         """
         if (
             self.sampleformat == 5
             or self.compression != 1
-            or self.bitspersample not in (8, 16, 32, 64)
+            or self.bitspersample not in {8, 16, 32, 64}
         ):
             return False
         if 322 in self.tags:  # TileWidth
             if (
                 self.imagewidth != self.tilewidth
                 or self.imagelength % self.tilelength
                 or self.tilewidth % 16
@@ -9523,15 +9576,15 @@
         elif self.photometric == 1:
             names = ['BlackIsZero']
         elif self.photometric == 2:
             names = ['Red', 'Green', 'Blue']
         elif self.photometric == 5:
             names = ['Cyan', 'Magenta', 'Yellow', 'Black']
         elif self.photometric == 6:
-            if self.compression in (6, 7, 34892, 33007):
+            if self.compression in {6, 7, 34892, 33007}:
                 # YCBCR -> RGB for JPEG
                 names = ['Red', 'Green', 'Blue']
             else:
                 names = ['Luma', 'Cb', 'Cr']
         else:
             return None
         if extrasamples > 0:
@@ -9768,15 +9821,15 @@
                 return description
         return None
 
     @cached_property
     def is_jfif(self) -> bool:
         """JPEG compressed segments contain JFIF metadata."""
         if (
-            self.compression not in (6, 7, 34892, 33007)
+            self.compression not in {6, 7, 34892, 33007}
             or len(self.dataoffsets) < 1
             or self.dataoffsets[0] == 0
             or len(self.databytecounts) < 1
             or self.databytecounts[0] < 11
         ):
             return False
         fh = self.parent.filehandle
@@ -9834,15 +9887,24 @@
     def is_shaped(self) -> bool:
         """Page contains Tifffile JSON metadata."""
         return self.shaped_description is not None
 
     @property
     def is_mdgel(self) -> bool:
         """Page contains MDFileTag tag."""
-        return 33445 in self.tags  # MDFileTag
+        return (
+            37701 not in self.tags  # AgilentBinary
+            and 33445 in self.tags  # MDFileTag
+        )
+
+    @property
+    def is_agilent(self) -> bool:
+        """Page contains Agilent Technologies tags."""
+        # tag 270 and 285 contain color names
+        return 285 in self.tags and 37701 in self.tags  # AgilentBinary
 
     @property
     def is_mediacy(self) -> bool:
         """Page contains Media Cybernetics Id tag."""
         tag = self.tags.get(50288)  # MC_Id
         try:
             return tag is not None and tag.value[:7] == b'MC TIFF'
@@ -10032,15 +10094,15 @@
         ].strip().endswith('</DataObject>')
 
     @property
     def is_eer(self) -> bool:
         """Page contains EER metadata."""
         return (
             self.parent.is_bigtiff
-            and self.compression in (65000, 65001)
+            and self.compression in {5000, 65001}
             and 65001 in self.tags
         )
 
 
 @final
 class TiffFrame:
     """Lightweight TIFF image file directory (IFD).
@@ -10050,15 +10112,15 @@
     Properties other than `offset`, `index`, `dataoffsets`, `databytecounts`,
     `subifds`, and `jpegtables` are assumed to be identical with a specified
     TiffPage instance, the keyframe.
     TiffFrame instances have no `tag` property.
     Virtual frames just reference the image data in the file. They may not
     have an IFD structure in the file.
 
-    TiffFrame instances are not thread-safe.
+    TiffFrame instances are not thread-safe. All attributes are read-only.
 
     Parameters:
         parent:
             TiffFile instance to read frame from.
             The file handle position must be at an offset to an IFD structure.
             Only a limited number of tag values are read from file.
         index:
@@ -10153,17 +10215,17 @@
             # use databytecounts from keyframe
             tags = {256, 273, 324, 330}
             self.databytecounts = keyframe.databytecounts
         else:
             tags = {256, 273, 279, 324, 325, 330, 347}
 
         for code, tag in self._gettags(tags):
-            if code == 273 or code == 324:
+            if code in {273, 324}:
                 self.dataoffsets = tag.value
-            elif code == 279 or code == 325:
+            elif code in {279, 325}:
                 self.databytecounts = tag.value
             elif code == 330:
                 self.subifds = tag.value
             elif code == 347:
                 self.jpegtables = tag.value
             elif keyframe is None or (
                 code == 256 and keyframe.imagewidth != tag.value
@@ -10492,15 +10554,15 @@
         return f'TiffFrame {index} @{self.offset}  {info}'
 
 
 @final
 class TiffTag:
     """TIFF tag structure.
 
-    TiffTag instances are not thread-safe.
+    TiffTag instances are not thread-safe. All attributes are read-only.
 
     Parameters:
         parent:
             TIFF file tag belongs to.
         offset:
             Position of tag structure in file.
         code:
@@ -10608,21 +10670,21 @@
 
         valueoffset = offset + tiff.tagsize - tiff.tagoffsetthreshold
         code, dtype = struct.unpack(tiff.tagformat1, header[:4])
         count, value = struct.unpack(tiff.tagformat2, header[4:])
 
         try:
             valueformat = TIFF.DATA_FORMATS[dtype]
-        except KeyError:
+        except KeyError as exc:
             msg = (
                 f'<tifffile.TiffTag {code} @{offset}> '
                 f'invalid data type {dtype!r}'
             )
             if validate:
-                raise TiffFileError(msg)
+                raise TiffFileError(msg) from exc
             log_warning(msg)
             return cls(parent, offset, code, dtype, count, None, 0)
 
         valuesize = count * struct.calcsize(valueformat)
         if (
             valuesize > tiff.tagoffsetthreshold
             or code in TIFF.TAG_READERS  # TODO: only works with offsets?
@@ -10646,24 +10708,24 @@
                 value = None
             elif code in TIFF.TAG_LOAD:
                 value = TiffTag._read_value(
                     parent, offset, code, dtype, count, valueoffset
                 )
             else:
                 value = None
-        elif dtype in (1, 2, 7):
+        elif dtype in {1, 2, 7}:
             # BYTES, ASCII, UNDEFINED
             value = value[:valuesize]
         elif (
             tiff.is_ndpi
             and count == 1
-            and dtype in (4, 9, 13)
+            and dtype in {4, 9, 13}
             and value[4:] != b'\x00\x00\x00\x00'
         ):
-            # NDPI IFD or LONG, e.g., in StripOffsets or StripByteCounts
+            # NDPI IFD or LONG, for example, in StripOffsets or StripByteCounts
             value = struct.unpack('<Q', value)
         else:
             fmt = '{}{}{}'.format(
                 tiff.byteorder, count * int(valueformat[0]), valueformat[1]
             )
             value = struct.unpack(fmt, value[:valuesize])
 
@@ -10680,19 +10742,19 @@
         count: int,
         valueoffset: int,
         /,
     ) -> Any:
         """Read tag value from file."""
         try:
             valueformat = TIFF.DATA_FORMATS[dtype]
-        except KeyError:
+        except KeyError as exc:
             raise TiffFileError(
                 f'<tifffile.TiffTag {code} @{offset}> '
                 f'invalid data type {dtype!r}'
-            )
+            ) from exc
 
         fh = parent.filehandle
         tiff = parent.tiff
 
         valuesize = count * struct.calcsize(valueformat)
         if valueoffset < 8 or valueoffset + valuesize > fh.size:
             raise TiffFileError(
@@ -10705,15 +10767,15 @@
         #         'value does not begin on word boundary'
         #     )
 
         fh.seek(valueoffset)
         if code in TIFF.TAG_READERS:
             readfunc = TIFF.TAG_READERS[code]
             value = readfunc(fh, tiff.byteorder, dtype, count, tiff.offsetsize)
-        elif dtype == 1 or dtype == 2 or dtype == 7:
+        elif dtype in {1, 2, 7}:
             # BYTES, ASCII, UNDEFINED
             value = fh.read(valuesize)
             if len(value) != valuesize:
                 log_warning(
                     f'<tifffile.TiffTag {code} @{offset}> '
                     'could not read all values'
                 )
@@ -10757,15 +10819,15 @@
             return value
 
         if code in TIFF.TAG_ENUM:
             t = TIFF.TAG_ENUM[code]
             try:
                 value = tuple(t(v) for v in value)
             except ValueError as exc:
-                if code not in (259, 317):  # ignore compression/predictor
+                if code not in {259, 317}:  # ignore compression/predictor
                     log_warning(f'<tifffile.TiffTag {code} @{offset}> {exc}')
 
         if len(value) == 1 and code not in TIFF.TAG_TUPLE:
             value = value[0]
 
         return value
 
@@ -10918,15 +10980,15 @@
                 'as first argument'
             )
 
         fh = self.parent.filehandle
         tiff = self.parent.tiff
         if tiff.is_ndpi:
             # only support files < 4GB
-            if self.count == 1 and self.dtype in (4, 13):
+            if self.count == 1 and self.dtype in {4, 13}:
                 if isinstance(self.value, tuple):
                     v = self.value[0]
                 else:
                     v = self.value
                 if v > 4294967295:
                     raise ValueError('cannot patch NDPI > 4 GB files')
             tiff = TIFF.CLASSIC_LE
@@ -10980,15 +11042,15 @@
 
         else:
             try:
                 count = len(value)
             except TypeError:
                 value = (value,)
                 count = 1
-            if dtype in (5, 10):
+            if dtype in {5, 10}:
                 if count < 2 or count % 2:
                     raise ValueError('invalid RATIONAL value')
                 count //= 2  # rational
 
         if packedvalue is None:
             packedvalue = struct.pack(
                 '{}{}{}'.format(
@@ -11163,15 +11225,15 @@
     - keys are :py:attr:`TiffTag.code` (int).
     - multiple values can be stored per key.
     - can be indexed by :py:attr:`TiffTag.name` (`str`), slower than by key.
     - `iter()` returns values instead of keys.
     - `values()` and `items()` contain all values sorted by offset.
     - `len()` returns number of all values.
     - `get()` takes optional index argument.
-    - some functions are not implemented, e.g., `update`, `setdefault`, `pop`.
+    - some functions are not implemented, such as, `update` and `pop`.
 
     """
 
     __slots__ = ('_dict', '_list')
 
     _dict: dict[int, TiffTag]
     _list: list[dict[int, TiffTag]]
@@ -11379,15 +11441,15 @@
             tlines.append(value[:width].strip())
             if detail > 0 and len(value) > width:
                 try:
                     value = tag.value
                 except Exception:
                     # delay load failed or closed file
                     continue
-                if tag.code in (273, 279, 324, 325):
+                if tag.code in {273, 279, 324, 325}:
                     if detail < 1:
                         value = value[:256]
                     elif len(value) > 1024:
                         value = value[:512] + value[-512:]
                     value = pformat(value, width=width, height=detail * 3)
                 else:
                     value = pformat(value, width=width, height=detail * 8)
@@ -11405,18 +11467,18 @@
 
 
 @final
 class TiffTagRegistry:
     """Registry of TIFF tag codes and names.
 
     Map tag codes and names to names and codes respectively.
-    One tag code may be registered with several names, e.g., 34853 is used for
-    GPSTag or OlympusSIS2.
-    Different tag codes may be registered with the same name, e.g., 37387 and
-    41483 are both named FlashEnergy.
+    One tag code may be registered with several names, for example, 34853 is
+    used for GPSTag or OlympusSIS2.
+    Different tag codes may be registered with the same name, for example,
+    37387 and 41483 are both named FlashEnergy.
 
     Parameters:
         arg: Mapping of codes to names.
 
     Examples:
         >>> tags = TiffTagRegistry(
         ...     [(34853, 'GPSTag'), (34853, 'OlympusSIS2')]
@@ -11592,15 +11654,25 @@
         return 'TiffTagRegistry(((\n  {}\n))'.format(
             ',\n  '.join(f'({code}, {name!r})' for code, name in self.items())
         )
 
 
 @final
 class TiffPageSeries:
-    """Series of TIFF pages with compatible shape and data type (same hash).
+    """Series of TIFF pages making up multi-dimensional image.
+
+    Many TIFF based formats, such as OME-TIFF, use series of TIFF pages to
+    store chunks of larger, multi-dimensional images.
+    The image shape and position of chunks in the multi-dimensional image is
+    defined in format-specific metadata.
+    All pages in a series must have the same :py:meth:`TiffPage.hash`,
+    that is, the same shape, data type, and storage properties.
+    Items of a series may be None (missing) or instances of
+    :py:class:`TiffPage` or :py:class:`TiffFrame`, possibly belonging to
+    different files.
 
     Parameters:
         pages:
             List of TiffPage, TiffFrame, or None.
             The file handles of TiffPages or TiffFrames may not be open.
         shape:
             Shape of image array in series.
@@ -11614,17 +11686,17 @@
         index:
             Index of series in multi-series files.
         parent:
             TiffFile instance series belongs to.
         name:
             Name of series.
         kind:
-            Nature of series, e.g., 'OME' or 'ImageJ'.
+            Nature of series, such as, 'ome' or 'imagej'.
         truncated:
-            Series is truncated, e.g., ImageJ hyperstack > 4 GB.
+            Series is truncated, for example, ImageJ hyperstack > 4 GB.
         multifile:
             Series contains pages from multiple files.
         squeeze:
             Remove length-1 dimensions (except X and Y) from shape and axes
             by default.
         transform:
             Function to transform image data after decoding.
@@ -11652,15 +11724,18 @@
     index: int
     """Index of series in multi-series files."""
 
     transform: Callable[[NDArray[Any]], NDArray[Any]] | None
     """Function to transform image data after decoding."""
 
     is_multifile: bool
-    """Series contains frames from multiple files."""
+    """Series contains pages from multiple files."""
+
+    is_truncated: bool
+    """Series contains single page describing multi-dimensional image."""
 
     _pages: list[TiffPage | TiffFrame | None]
     _squeeze: bool
     _axes: str
     _axes_squeezed: str
     _shape: tuple[int, ...]
     _shape_squeezed: tuple[int, ...]
@@ -11723,14 +11798,15 @@
 
         self.dtype = numpy.dtype(dtype)
         self.kind = kind if kind else ''
         self.name = name if name else ''
         self.transform = transform
         self.keyframe = keyframe
         self.is_multifile = bool(multifile)
+        self.is_truncated = bool(truncated)
 
         if parent is not None:
             self.parent = parent
         elif self._pages:
             self.parent = self.keyframe.parent
         else:
             self.parent = None
@@ -12266,15 +12342,15 @@
         lock: threading.RLock | NullContext | None = None,
         squeeze: bool | None = None,
         maxworkers: int | None = None,
         _openfiles: int | None = None,
     ) -> None:
         super().__init__(fillvalue=fillvalue, chunkmode=chunkmode)
 
-        if self._chunkmode not in (0, 2):
+        if self._chunkmode not in {0, 2}:
             raise NotImplementedError(f'{self._chunkmode!r} not implemented')
 
         self._maxworkers = maxworkers
         self._squeeze = None if squeeze is None else bool(squeeze)
 
         if isinstance(arg, TiffPageSeries):
             self._data = arg.levels
@@ -12444,19 +12520,19 @@
 
         Raises:
             ValueError:
                 ZarrTiffStore cannot be represented as ReferenceFileSystem
                 due to features that are not supported by Zarr, Numcodecs,
                 or Imagecodecs:
 
-                - compressors, e.g., CCITT
-                - filters, e.g., bitorder reversal, packed integers
-                - dtypes, e.g., float24
+                - compressors, such as CCITT
+                - filters, such as bitorder reversal, packed integers
+                - dtypes, such as float24
                 - JPEGTables in multi-page files
-                - incomplete chunks, e.g., `imagelength % rowsperstrip != 0`
+                - incomplete chunks, such as `imagelength % rowsperstrip != 0`
 
                 Files containing incomplete tiles may fail at runtime.
 
         Notes:
             Parameters `_shape`,  `_axes`, `_index`, `_append`, and `_close`
             are an experimental API for joining the ReferenceFileSystems of
             multiple files of a TiffSequence.
@@ -12495,28 +12571,28 @@
         for series in self._data:
             errormsg = ' not supported by the fsspec ReferenceFileSystem'
             keyframe = series.keyframe
             if keyframe.compression not in compressors:
                 raise ValueError(f'{keyframe.compression!r} is' + errormsg)
             if keyframe.fillorder != 1:
                 raise ValueError(f'{keyframe.fillorder!r} is' + errormsg)
-            if keyframe.sampleformat not in (1, 2, 3, 6):
+            if keyframe.sampleformat not in {1, 2, 3, 6}:
                 # TODO: support float24 and cint via filters?
                 raise ValueError(f'{keyframe.sampleformat!r} is' + errormsg)
-            if keyframe.bitspersample not in (
+            if keyframe.bitspersample not in {
                 8,
                 16,
                 32,
                 64,
                 128,
-            ) and keyframe.compression not in (
+            } and keyframe.compression not in {
                 7,
                 33007,
                 34892,
-            ):  # JPEG
+            }:  # JPEG
                 raise ValueError(
                     f'BitsPerSample {keyframe.bitspersample} is' + errormsg
                 )
             if (
                 not self._chunkmode
                 and not keyframe.is_tiled
                 and keyframe.imagelength % keyframe.rowsperstrip
@@ -12646,26 +12722,34 @@
                             'id': codec_id,
                             'tables': tables,
                             'header': header,
                             'bitspersample': keyframe.bitspersample,
                             'colorspace_jpeg': colorspace_jpeg,
                             'colorspace_data': colorspace_data,
                         }
+                    elif (
+                        codec_id == 'imagecodecs_webp'
+                        and keyframe.samplesperpixel == 4
+                    ):
+                        value['compressor'] = {
+                            'id': codec_id,
+                            'hasalpha': True,
+                        }
                     elif codec_id is not None:
                         value['compressor'] = {'id': codec_id}
                     if keyframe.predictor > 1:
                         # predictors need access to chunk shape and dtype
                         # requires imagecodecs > 2021.8.26 to read
-                        if keyframe.predictor in (2, 34892, 34893):
+                        if keyframe.predictor in {2, 34892, 34893}:
                             filter_id = 'imagecodecs_delta'
                         else:
                             filter_id = 'imagecodecs_floatpred'
                         if keyframe.predictor <= 3:
                             dist = 1
-                        elif keyframe.predictor in (34892, 34894):
+                        elif keyframe.predictor in {34892, 34894}:
                             dist = 2
                         else:
                             dist = 4
                         if (
                             keyframe.planarconfig == 1
                             and keyframe.samplesperpixel > 1
                         ):
@@ -12687,15 +12771,15 @@
 
                 refzarr[groupname + key] = value.decode()
 
         fh: TextIO
         if hasattr(jsonfile, 'write'):
             fh = jsonfile  # type: ignore
         else:
-            fh = open(jsonfile, 'w')
+            fh = open(jsonfile, 'w', encoding='utf-8')
 
         if version == 1:
             fh.write(json.dumps(refs, indent=1).rsplit('}"', 1)[0] + '}"')
             indent = '  '
         elif _append:
             indent = ' '
         else:
@@ -12820,16 +12904,16 @@
         int | None,
     ]:
         """Return keyframe, page, index, offset, and bytecount from key."""
         if self._multiscales:
             try:
                 level, key = key.split('/')
                 series = self._data[int(level)]
-            except ValueError:
-                raise KeyError(key)
+            except ValueError as exc:
+                raise KeyError(key) from exc
         else:
             series = self._data[0]
         keyframe = series.keyframe
         pageindex, chunkindex = self._indices(key, series)
         if pageindex > 0 and len(series) == 1:
             # truncated ImageJ, STK, or shaped
             if series.dataoffset is None:
@@ -12859,16 +12943,16 @@
 
     def _indices(self, key: str, series: TiffPageSeries, /) -> tuple[int, int]:
         """Return page and strile indices from Zarr chunk index."""
         keyframe = series.keyframe
         shape = series.get_shape(self._squeeze)
         try:
             indices = [int(i) for i in key.split('.')]
-        except ValueError:
-            raise KeyError(key)
+        except ValueError as exc:
+            raise KeyError(key) from exc
         assert len(indices) == len(shape)
         if self._chunkmode:
             chunked = (1,) * len(keyframe.shape)
         else:
             chunked = keyframe.chunked
         p = 1
         for i, s in enumerate(shape[::-1]):
@@ -12954,16 +13038,16 @@
 
     @staticmethod
     def _is_writable(keyframe: TiffPage) -> bool:
         """Return True if chunks are writable."""
         return (
             keyframe.compression == 1
             and keyframe.fillorder == 1
-            and keyframe.sampleformat in (1, 2, 3, 6)
-            and keyframe.bitspersample in (8, 16, 32, 64, 128)
+            and keyframe.sampleformat in {1, 2, 3, 6}
+            and keyframe.bitspersample in {8, 16, 32, 64, 128}
             # and (
             #     keyframe.rowsperstrip == 0
             #     or keyframe.imagelength % keyframe.rowsperstrip == 0
             # )
         )
 
     def __enter__(self) -> ZarrTiffStore:
@@ -13026,15 +13110,15 @@
         dtype: DTypeLike | None = None,
         axestiled: dict[int, int] | Sequence[tuple[int, int]] | None = None,
         zattrs: dict[str, Any] | None = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(fillvalue=fillvalue, chunkmode=chunkmode)
 
-        if self._chunkmode not in (0, 3):
+        if self._chunkmode not in {0, 3}:
             raise ValueError(f'invalid chunkmode {self._chunkmode!r}')
 
         if not isinstance(arg, FileSequence):
             raise TypeError('not a FileSequence')
 
         if arg._container:
             raise NotImplementedError('cannot open container as Zarr store')
@@ -13181,24 +13265,24 @@
             url += '/'
 
         if groupname is None:
             groupname = ''
         elif groupname and groupname[-1] != '/':
             groupname += '/'
 
-        refs: dict[str, Any] = dict()
+        refs: dict[str, Any] = {}
         if version == 1:
             if _append:
                 raise ValueError('cannot append to version 1 files')
             if templatename is None:
                 templatename = 'u'
             refs['version'] = 1
             refs['templates'] = {templatename: url}
             refs['gen'] = []
-            refs['refs'] = refzarr = dict()
+            refs['refs'] = refzarr = {}
             url = '{{%s}}' % templatename
         else:
             refzarr = refs
 
         if groupname and not _append:
             refzarr['.zgroup'] = ZarrStore._json({'zarr_format': 2}).decode()
 
@@ -13210,15 +13294,15 @@
                 value = ZarrStore._json(value)
             refzarr[groupname + key] = value.decode()
 
         fh: TextIO
         if hasattr(jsonfile, 'write'):
             fh = jsonfile  # type: ignore
         else:
-            fh = open(jsonfile, 'w')
+            fh = open(jsonfile, 'w', encoding='utf-8')
 
         if version == 1:
             fh.write(json.dumps(refs, indent=1).rsplit('}"', 1)[0] + '}"')
             indent = '  '
         elif _append:
             fh.write(',\n')
             fh.write(json.dumps(refs, indent=1)[2:-2])
@@ -13845,15 +13929,15 @@
 
 @final
 class FileHandle:
     """Binary file handle.
 
     A limited, special purpose binary file handle that can:
 
-    - handle embedded files (e.g., for LSM within LSM files).
+    - handle embedded files (for example, LSM within LSM files).
     - re-open closed files (for multi-file formats, such as OME-TIFF).
     - read and write NumPy arrays and records from file-like objects.
 
     When initialized from another file handle, do not use the other handle
     unless this FileHandle is closed.
 
     FileHandle instances are not thread-safe.
@@ -13911,15 +13995,15 @@
         offset: int | None = None,
         size: int | None = None,
     ) -> None:
         if mode is None:
             mode = 'rb'
         elif mode[-1] != 'b':
             mode += 'b'  # type: ignore
-        if mode != 'rb' and mode != 'r+b' and mode != 'wb':
+        if mode not in {'rb', 'r+b', 'wb'}:
             raise ValueError(f'invalid mode {mode}')
         self._mode = mode
         self._fh = None
         self._file = file  # reference to original argument for re-opening
         self._name = name if name else ''
         self._dir = ''
         self._offset = -1 if offset is None else offset
@@ -13937,23 +14021,23 @@
         if isinstance(self._file, os.PathLike):
             self._file = os.fspath(self._file)
 
         if isinstance(self._file, str):
             # file name
             self._file = os.path.realpath(self._file)
             self._dir, self._name = os.path.split(self._file)
-            self._fh = open(self._file, self._mode)  # type: ignore
+            self._fh = open(
+                self._file, self._mode, encoding=None
+            )  # type: ignore
             self._close = True
-            if self._offset < 0:
-                self._offset = 0
+            self._offset = max(0, self._offset)
         elif isinstance(self._file, FileHandle):
             # FileHandle
             self._fh = self._file._fh
-            if self._offset < 0:
-                self._offset = 0
+            self._offset = max(0, self._offset)
             self._offset += self._file._offset
             self._close = False
             if not self._name:
                 if self._offset:
                     name, ext = os.path.splitext(self._file._name)
                     self._name = f'{name}@{self._offset}{ext}'
                 else:
@@ -13964,16 +14048,16 @@
             self._dir = self._file._dir
         elif hasattr(self._file, 'seek'):
             # binary stream: open file, BytesIO, fsspec LocalFileOpener
             # cast to BinaryIO even it might not be
             self._fh = cast(BinaryIO, self._file)
             try:
                 self._fh.tell()
-            except Exception:
-                raise ValueError('binary stream is not seekable')
+            except Exception as exc:
+                raise ValueError('binary stream is not seekable') from exc
 
             if self._offset < 0:
                 self._offset = self._fh.tell()
             self._close = False
             if not self._name:
                 try:
                     self._dir, self._name = os.path.split(self._fh.name)
@@ -13990,20 +14074,20 @@
                 pass
         elif hasattr(self._file, 'open'):
             # fsspec OpenFile
             _file: Any = self._file
             self._fh = cast(BinaryIO, _file.open())
             try:
                 self._fh.tell()
-            except Exception:
+            except Exception as exc:
                 try:
                     self._fh.close()
                 except Exception:
                     pass
-                raise ValueError('OpenFile is not seekable')
+                raise ValueError('OpenFile is not seekable') from exc
 
             if self._offset < 0:
                 self._offset = self._fh.tell()
             self._close = True
             if not self._name:
                 try:
                     self._dir, self._name = os.path.split(_file.path)
@@ -14125,15 +14209,15 @@
         assert self._fh is not None
         return self._fh.write(buffer)
 
     def flush(self) -> None:
         """Flush write buffers of stream if applicable."""
         assert self._fh is not None
         if hasattr(self._fh, 'flush'):
-            return self._fh.flush()
+            self._fh.flush()
 
     def memmap_array(
         self,
         dtype: DTypeLike,
         shape: tuple[int, ...],
         offset: int = 0,
         *,
@@ -14908,15 +14992,15 @@
 
     @property
     def planarconfig(self) -> int | None:
         """Value of PlanarConfiguration tag."""
         if self.separate_samples > 1:
             return 2  # PLANARCONFIG.SEPARATE
         if self.contig_samples > 1:
-            return 1  # PLANARCONFIG.SEPARATE
+            return 1  # PLANARCONFIG.CONTIG
         return None
 
     def __len__(self) -> int:
         return 6
 
     @overload
     def __getitem__(self, key: int, /) -> int:
@@ -14966,15 +15050,15 @@
     """Null context manager. Can be used as a dummy reentrant lock.
 
     >>> with NullContext():
     ...     pass
 
     """
 
-    __slots = ()
+    __slots__ = ()
 
     def __enter__(self) -> NullContext:
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:  # type: ignore
         pass
 
@@ -15138,16 +15222,15 @@
     elements: list[str]
     """Other OME-XML elements."""
 
     _xml: str
     _ifd: int
 
     def __init__(self, **metadata: Any) -> None:
-        if 'OME' in metadata:
-            metadata = metadata['OME']
+        metadata = metadata.get('OME', metadata)
 
         self._ifd = 0
         self.images = []
         self.annotations = []
         self.elements = []
         # TODO: parse other OME elements from metadata
         #   Project
@@ -15271,16 +15354,16 @@
                 'uint32': 'uint32',
                 'float32': 'float',
                 'float64': 'double',
                 'complex64': 'complex',
                 'complex128': 'double-complex',
                 'bool': 'bit',
             }[dtype]
-        except KeyError:
-            raise OmeXmlError(f'data type {dtype!r} not supported')
+        except KeyError as exc:
+            raise OmeXmlError(f'data type {dtype!r} not supported') from exc
 
         if metadata.get('Type', dtype) != dtype:
             raise OmeXmlError(
                 f'metadata Pixels Type {metadata["Type"]!r} '
                 f'does not match array dtype {dtype!r}'
             )
 
@@ -15391,15 +15474,15 @@
                         # use next unused axis
                         for x in 'TZC':
                             if x not in dimorder and x not in modulo:
                                 modulo[x] = axestype[ax], shape[i]
                                 dimorder.append(x)
                                 break
                         else:
-                            # TODO: support any order of axes, e.g., APRTZC
+                            # TODO: support any order of axes, such as, APRTZC
                             raise OmeXmlError('more than 3 modulo dimensions')
                 else:
                     dimorder.append(ax)
             hiaxes = ''.join(dimorder)
 
             # TODO: use user-specified start, stop, step, or labels
             moduloalong = ''.join(
@@ -15618,21 +15701,21 @@
             from lxml import etree
 
             parser = etree.XMLParser(remove_blank_text=True)
             tree = etree.fromstring(xml, parser)
             xml = etree.tostring(
                 tree, encoding='utf-8', pretty_print=True, xml_declaration=True
             ).decode()
+        except ImportError:
+            pass
         except Exception as exc:
             warnings.warn(
                 f'<tifffile.OmeXml.__str__> {exc.__class__.__name__}: {exc}',
                 UserWarning,
             )
-        except ImportError:
-            pass
         return xml
 
     @staticmethod
     def _escape(value: object, /) -> str:
         """Return escaped string of value."""
         if not isinstance(value, str):
             value = str(value)
@@ -15797,22 +15880,22 @@
             #     else:
             #         codec = imagecodecs.ccittrle_decode
             if key == 5:
                 if self._encode:
                     codec = imagecodecs.lzw_encode
                 else:
                     codec = imagecodecs.lzw_decode
-            elif key == 6 or key == 7 or key == 33007:
+            elif key in {6, 7, 33007}:
                 if self._encode:
-                    if key == 6 or key == 33007:
+                    if key in {6, 33007}:
                         raise NotImplementedError
                     codec = imagecodecs.jpeg_encode
                 else:
                     codec = imagecodecs.jpeg_decode
-            elif key == 8 or key == 32946 or key == 50013:
+            elif key in {8, 32946, 50013}:
                 if hasattr(imagecodecs, 'DEFLATE') and imagecodecs.DEFLATE:
                     # imagecodecs built with deflate
                     if self._encode:
                         codec = imagecodecs.deflate_encode
                     else:
                         codec = imagecodecs.deflate_decode
                 elif hasattr(imagecodecs, 'ZLIB') and imagecodecs.ZLIB:
@@ -15832,15 +15915,15 @@
                     else:
                         codec = _imagecodecs.zlib_decode
             elif key == 32773:
                 if self._encode:
                     codec = imagecodecs.packbits_encode
                 else:
                     codec = imagecodecs.packbits_decode
-            elif key == 33003 or key == 33004 or key == 33005 or key == 34712:
+            elif key in {33003, 33004, 33005, 34712}:
                 if self._encode:
                     codec = imagecodecs.jpeg2k_encode
                 else:
                     codec = imagecodecs.jpeg2k_decode
             elif key == 34887:
                 if self._encode:
                     codec = imagecodecs.lerc_encode
@@ -15870,30 +15953,30 @@
                     else:
                         codec = _imagecodecs.lzma_decode
             elif key == 34933:
                 if self._encode:
                     codec = imagecodecs.png_encode
                 else:
                     codec = imagecodecs.png_decode
-            elif key == 34934 or key == 22610:
+            elif key in {34934, 22610}:
                 if self._encode:
                     codec = imagecodecs.jpegxr_encode
                 else:
                     codec = imagecodecs.jpegxr_decode
             elif key == 48124:
                 if self._encode:
                     codec = imagecodecs.jetraw_encode
                 else:
                     codec = imagecodecs.jetraw_decode
-            elif key == 50000 or key == 34926:  # 34926 deprecated
+            elif key in {50000, 34926}:  # 34926 deprecated
                 if self._encode:
                     codec = imagecodecs.zstd_encode
                 else:
                     codec = imagecodecs.zstd_decode
-            elif key == 50001 or key == 34927:  # 34927 deprecated
+            elif key in {50001, 34927}:  # 34927 deprecated
                 if self._encode:
                     codec = imagecodecs.webp_encode
                 else:
                     codec = imagecodecs.webp_decode
             elif key == 50002:
                 if self._encode:
                     codec = imagecodecs.jpegxl_encode
@@ -15901,20 +15984,20 @@
                     codec = imagecodecs.jpegxl_decode
             else:
                 try:
                     msg = f'{COMPRESSION(key)!r} not supported'
                 except ValueError:
                     msg = f'{key} is not a known COMPRESSION'
                 raise KeyError(msg)
-        except (AttributeError, ImportError):
+        except (AttributeError, ImportError) as exc:
             raise KeyError(
                 f'{COMPRESSION(key)!r} ' "requires the 'imagecodecs' package"
-            )
-        except NotImplementedError:
-            raise KeyError(f'{COMPRESSION(key)!r} not implemented')
+            ) from exc
+        except NotImplementedError as exc:
+            raise KeyError(f'{COMPRESSION(key)!r} not implemented') from exc
         self._codecs[key] = codec
         return codec
 
     def __contains__(self, key: Any, /) -> bool:
         try:
             self[key]
         except KeyError:
@@ -16017,20 +16100,20 @@
                     def codec(data, axis=-1, out=None):
                         return imagecodecs.floatpred_decode(
                             data, axis=axis, out=out, dist=4
                         )
 
             else:
                 raise KeyError(f'{key} is not a known PREDICTOR')
-        except AttributeError:
+        except AttributeError as exc:
             raise KeyError(
                 f'{PREDICTOR(key)!r}' " requires the 'imagecodecs' package"
-            )
-        except NotImplementedError:
-            raise KeyError(f'{PREDICTOR(key)!r} not implemented')
+            ) from exc
+        except NotImplementedError as exc:
+            raise KeyError(f'{PREDICTOR(key)!r} not implemented') from exc
         self._codecs[key] = codec
         return codec
 
     def __contains__(self, key: Any, /) -> bool:
         try:
             self[key]
         except KeyError:
@@ -16882,14 +16965,16 @@
                 (37510, 'UserComment'),
                 (37520, 'SubsecTime'),
                 (37521, 'SubsecTimeOriginal'),
                 (37522, 'SubsecTimeDigitized'),
                 (37679, 'MODIText'),  # Microsoft Office Document Imaging
                 (37680, 'MODIOLEPropertySetStorage'),
                 (37681, 'MODIPositioning'),
+                (37701, 'AgilentBinary'),  # private structure
+                (37702, 'AgilentString'),  # file description
                 (37706, 'TVIPS'),  # offset to TemData structure
                 (37707, 'TVIPS1'),
                 (37708, 'TVIPS2'),  # same TemData structure as undefined
                 (37724, 'ImageSourceData'),  # Photoshop
                 (37888, 'Temperature'),
                 (37889, 'Humidity'),
                 (37890, 'Pressure'),
@@ -17692,15 +17777,15 @@
 
         - **X : width** (image width)
         - **Y : height** (image length)
         - **Z : depth** (image depth)
         - **S : sample** (color space and extra samples)
         - **I : sequence** (generic sequence of images, frames, planes, pages)
         - **T : time** (time series)
-        - **C : channel** (e.g., acquisition path or emission wavelength)
+        - **C : channel** (acquisition path or emission wavelength)
         - **A : angle** (OME)
         - **P : phase** (OME. In LSM, **P** maps to **position**)
         - **R : tile** (OME. Region, position, or mosaic)
         - **H : lifetime** (OME. Histogram)
         - **E : lambda** (OME. Excitation wavelength)
         - **Q : other** (OME)
         - **L : exposure** (FluoView)
@@ -17753,15 +17838,15 @@
         # map axes character codes to dimension names and reverse.
         warnings.warn(
             '<tifffile.TIFF.AXES_LABELS> is deprecated. '
             'Use TIFF.AXES_NAMES or TIFF.AXES_CODES.',
             DeprecationWarning,
             stacklevel=2,
         )
-        return dict(**TIFF.AXES_NAMES, **TIFF.AXES_CODES)
+        return {**TIFF.AXES_NAMES, **TIFF.AXES_CODES}
 
     @cached_property
     def GEO_KEYS(self) -> type[enum.IntEnum]:
         """:py:class:`geodb.GeoKeys`."""
         try:
             from .geodb import GeoKeys
         except ImportError:
@@ -18768,15 +18853,16 @@
             The file handle position must be at a valid IFD header.
         byteorder:
             Byte order of TIFF file.
         offsetsize:
             Size of offsets in TIFF file (8 for BigTIFF, else 4).
         tagnames:
             Map of tag codes to names.
-            E.g., :py:class:`_TIFF.GPS_TAGS` or :py:class:`_TIFF.IOP_TAGS`.
+            For example, :py:class:`_TIFF.GPS_TAGS` or
+            :py:class:`_TIFF.IOP_TAGS`.
         maxifds:
             Maximum number of IFDs to read.
             By default, read the whole IFD chain.
         customtags:
             Mapping of tag codes to functions reading special tag value from
             file.
 
@@ -18840,46 +18926,46 @@
             count, valuebytes = unpack(
                 tagformat2, data[index + 4 : index + tagsize]
             )
             index += tagsize
             name = tagnames.get(code, str(code))
             try:
                 valueformat = TIFF.DATA_FORMATS[dtype]
-            except KeyError:
+            except KeyError as exc:
                 raise TiffFileError(
                     f'invalid data type {dtype!r} for tag #{code}'
-                )
+                ) from exc
 
             valuesize = count * struct.calcsize(valueformat)
             if valuesize > offsetsize or code in customtags:
                 valueoffset = unpack(offsetformat, valuebytes)[0]
                 if valueoffset < 8 or valueoffset + valuesize > fh.size:
                     raise TiffFileError(
                         f'invalid value offset {valueoffset} for tag #{code}'
                     )
                 fh.seek(valueoffset)
                 if code in customtags:
                     readfunc = customtags[code]
                     value = readfunc(fh, byteorder, dtype, count, offsetsize)
-                elif dtype == 1 or dtype == 2 or dtype == 7:
+                elif dtype in {1, 2, 7}:
                     # BYTES, ASCII, UNDEFINED
                     value = fh.read(valuesize)
                     if len(value) != valuesize:
                         log_warning(
                             '<tifffile.read_tags> '
                             f'could not read all values for tag #{code}'
                         )
                 elif code in tagnames:
                     fmt = '{}{}{}'.format(
                         byteorder, count * int(valueformat[0]), valueformat[1]
                     )
                     value = unpack(fmt, fh.read(valuesize))
                 else:
                     value = read_numpy(fh, byteorder, dtype, count, offsetsize)
-            elif dtype == 1 or dtype == 2 or dtype == 7:
+            elif dtype in {1, 2, 7}:
                 # BYTES, ASCII, UNDEFINED
                 value = valuebytes[:valuesize]
             else:
                 fmt = '{}{}{}'.format(
                     byteorder, count * int(valueformat[0]), valueformat[1]
                 )
                 value = unpack(fmt, valuebytes[:valuesize])
@@ -18901,15 +18987,15 @@
                     )
             else:
                 if code in TIFF.TAG_ENUM:
                     t = TIFF.TAG_ENUM[code]
                     try:
                         value = tuple(t(v) for v in value)
                     except ValueError as exc:
-                        if code not in (259, 317):
+                        if code not in {259, 317}:
                             # ignore compression/predictor
                             log_warning(
                                 '<tifffile.read_tags> '
                                 f'failed for tag #{code}: {exc}'
                             )
                 if process and len(value) == 1:
                     value = value[0]
@@ -19109,25 +19195,25 @@
     planecount: int = 0,
 ) -> dict[str, Any]:
     """Read MetaMorph STK UIC1Tag value from file.
 
     Return empty dictionary if planecount is unknown.
 
     """
-    if dtype not in (4, 5) or byteorder != '<':
+    if dtype not in {4, 5} or byteorder != '<':
         raise ValueError(f'invalid UIC1Tag {byteorder}{dtype}')
     result = {}
     if dtype == 5:
         # pre MetaMorph 2.5 (not tested)
         values = fh.read_array('<u4', 2 * count).reshape(count, 2)
         result = {'ZDistance': values[:, 0] / values[:, 1]}
     else:
         for _ in range(count):
             tagid = struct.unpack('<I', fh.read(4))[0]
-            if tagid in (28, 29, 37, 40, 41):
+            if tagid in {28, 29, 37, 40, 41}:
                 # silently skip unexpected tags
                 fh.read(4)
                 continue
             name, value = read_uic_tag(fh, tagid, planecount, True)
             result[name] = value
     return result
 
@@ -19211,15 +19297,15 @@
         # unknown tag
         return f'_TagId{tagid}', read_int()
 
     Fraction = TIFF.UIC_TAGS[4][1]
 
     if offset:
         pos = fh.tell()
-        if dtype not in (int, None):
+        if dtype not in {int, None}:
             off = read_int()
             if off < 8:
                 if dtype is str:
                     return name, ''
                 log_warning(
                     '<tifffile.read_uic_tag> '
                     f'invalid offset for tag {name!r} @{off}'
@@ -19315,30 +19401,30 @@
     flags, prop = struct.unpack('<IB', fh.read(5))
     if prop == 1:
         value = struct.unpack('II', fh.read(8))
         value = value[0] / value[1]
     else:
         size = struct.unpack('B', fh.read(1))[0]
         value = struct.unpack(f'{size}s', fh.read(size))[0]
-    return dict(name=name, flags=flags, value=value)
+    return {'name': name, 'flags': flags, 'value': value}
 
 
 def read_cz_lsminfo(
     fh: FileHandle,
     byteorder: ByteOrder,
     dtype: int,
     count: int,
     offsetsize: int,
     /,
 ) -> dict[str, Any]:
     """Read CZ_LSMINFO tag value from file."""
     if byteorder != '<':
         raise ValueError('invalid CZ_LSMINFO structure')
     magic_number, structure_size = struct.unpack('<II', fh.read(8))
-    if magic_number not in (50350412, 67127628):
+    if magic_number not in {50350412, 67127628}:
         raise ValueError('invalid CZ_LSMINFO structure')
     fh.seek(-8, os.SEEK_CUR)
     CZ_LSMINFO = TIFF.CZ_LSMINFO
 
     if structure_size < numpy.dtype(CZ_LSMINFO).itemsize:
         # adjust structure according to structure_size
         lsminfo: list[tuple[str, str]] = []
@@ -19734,17 +19820,17 @@
                 if number != v:
                     value = number
                     unit = u
             except Exception:
                 number = astype(value, (int, float))
                 if number != value:
                     value = number
-                if value in ('No', 'Off'):
+                if value in {'No', 'Off'}:
                     value = False
-                elif value in ('Yes', 'On'):
+                elif value in {'Yes', 'On'}:
                     value = True
             result[key] = (name.strip(), value)
             if unit:
                 result[key] += (unit,)
             key = None
         else:
             result[''] += (astype(line, (int, float)),)
@@ -19794,15 +19880,15 @@
     fh.seek(0)
     try:
         byteorder, version = struct.unpack('<2sH', fh.read(4))
         if byteorder != b'II' or version != 43:
             raise ValueError('not a BigTIFF file')
         fh.seek(16)
         magic, version, size0, size1 = struct.unpack('<IIII', fh.read(16))
-        if magic != 117637889 or version not in (3, 4):
+        if magic != 117637889 or version not in {3, 4}:
             raise ValueError(
                 f'invalid magic {magic} or version {version} number'
             )
     except UnicodeDecodeError as exc:
         raise ValueError('file must be opened in binary mode') from exc
     except Exception as exc:
         raise ValueError('not a ScanImage BigTIFF v3 or v4 file') from exc
@@ -19858,16 +19944,16 @@
     try:
         byteorder = {b'II': '<', b'MM': '>'}[fh.read(2)]
         fh.seek(8)
         (
             index_header,
             index_offset,
         ) = struct.unpack(byteorder + 'II', fh.read(8))
-    except Exception:
-        raise ValueError('not a Micro-Manager TIFF file')
+    except Exception as exc:
+        raise ValueError('not a Micro-Manager TIFF file') from exc
 
     result = {}
     if index_header == 483729:
         # NDTiff >= v2
         result['MajorVersion'] = index_offset
         try:
             (
@@ -20071,15 +20157,15 @@
 
     Return None if the file does not contain valid GDAL structural metadata.
     The metadata can be used to optimize reading image data from a COG file.
 
     """
     fh.seek(0)
     try:
-        if fh.read(2) not in (b'II', b'MM'):
+        if fh.read(2) not in {b'II', b'MM'}:
             raise ValueError('not a TIFF file')
         fh.seek({b'*': 8, b'+': 16}[fh.read(1)])
         header = fh.read(43).decode()
         if header[:30] != 'GDAL_STRUCTURAL_METADATA_SIZE=':
             return None
         size = int(header[30:36])
         lines = fh.read(size).decode()
@@ -20226,15 +20312,15 @@
             Byte order of TIFF file.
 
     Returns:
         Metadata dict with optional items:
 
             'Info' (str):
                 Human-readable information as string.
-                Some formats, e.g., OIF or ScanImage, can be parsed into
+                Some formats, such as OIF or ScanImage, can be parsed into
                 dicts with :py:func:`matlabstr2py` or the
                 `oiffile.SettingsFile()` function of the
                 `oiffile <https://pypi.org/project/oiffile/>`_  package.
             'Labels' (Sequence[str]):
                 Human-readable labels for each channel.
             'Ranges' (Sequence[float]):
                 Lower and upper values for each channel.
@@ -20278,15 +20364,15 @@
     }
     # little-endian
     metadata_types.update({k[::-1]: v for k, v in metadata_types.items()})
 
     if len(bytecounts) == 0:
         raise ValueError('no ImageJ metadata')
 
-    if data[:4] not in (b'IJIJ', b'JIJI'):
+    if data[:4] not in {b'IJIJ', b'JIJI'}:
         raise ValueError('invalid ImageJ metadata')
 
     header_size = bytecounts[0]
     if header_size < 12 or header_size > 804:
         raise ValueError('invalid ImageJ metadata header size')
 
     ntypes = (header_size - 4) // 8
@@ -20416,15 +20502,15 @@
     version = metadata.pop('ImageJ', '1.11a')
 
     if colormaped:
         hyperstack = False
         rgb = False
 
     shape = imagej_shape(shape, rgb=rgb, axes=axes)
-    rgb = shape[-1] in (3, 4)
+    rgb = shape[-1] in {3, 4}
 
     append = []
     result = [f'ImageJ={version}']
     result.append(f'images={product(shape[:-3])}')
     if hyperstack is None:
         hyperstack = True
         append.append('hyperstack=true')
@@ -20442,15 +20528,15 @@
         result.append(f'frames={shape[0]}')
         if loop is None:
             append.append('loop=false')
     if loop is not None:
         append.append(f'loop={bool(loop)}'.lower())
 
     for key, value in metadata.items():
-        if key not in ('images', 'channels', 'slices', 'frames', 'SCIFIO'):
+        if key not in {'images', 'channels', 'slices', 'frames', 'SCIFIO'}:
             if isinstance(value, bool):
                 value = str(value).lower()
             append.append(f'{key.lower()}={value}')
 
     return '\n'.join(result + append + [''])
 
 
@@ -20491,23 +20577,23 @@
         i = 0
         for ax in 'TZCYXS':
             if i < ndims and ax == axes[i]:
                 newshape.append(shape[i])
                 i += 1
             else:
                 newshape.append(1)
-        if newshape[-1] not in (1, 3, 4):
+        if newshape[-1] not in {1, 3, 4}:
             raise ValueError(
                 'ImageJ hyperstack must contain 1, 3, or 4 samples'
             )
         return tuple(newshape)
 
     if rgb is None:
-        rgb = shape[-1] in (3, 4) and ndim > 2
-    if rgb and shape[-1] not in (3, 4):
+        rgb = shape[-1] in {3, 4} and ndim > 2
+    if rgb and shape[-1] not in {3, 4}:
         raise ValueError('ImageJ hyperstack is not a RGB image')
     if not rgb and ndim == 6 and shape[-1] != 1:
         raise ValueError('ImageJ hyperstack is not a grayscale image')
     if rgb or shape[-1] == 1:
         return (1,) * (6 - ndim) + shape
     return (1,) * (5 - ndim) + shape + (1,)
 
@@ -20679,15 +20765,15 @@
     >>> shaped_description_metadata('shape=(256, 256, 3)')
     {'shape': (256, 256, 3)}
 
     """
     if description[:6] == 'shape=':
         # old-style 'shaped' description; not JSON
         shape = tuple(int(i) for i in description[7:-1].split(','))
-        return dict(shape=shape)
+        return {'shape': shape}
     if description[:1] == '{' and description[-1:] == '}':
         # JSON description
         return json.loads(description)
     raise ValueError('invalid JSON image description', description)
 
 
 def fluoview_description_metadata(
@@ -20875,15 +20961,15 @@
 
     root = etree.fromstring(description)
     types: dict[str, Callable[..., Any]] = {
         'float': float,
         'int': int,
         'bool': lambda x: asbool(x, 'on', 'off'),
         'time': lambda x: strptime(x, '%Y%m%d %H:%M:%S.%f'),
-        'guid': lambda x: uuid.UUID(x),
+        'guid': uuid.UUID,
         # 'float-array':
         # 'colorref':
     }
 
     def parse(
         root: etree.Element, result: dict[str, Any], /
     ) -> dict[str, Any]:
@@ -21049,15 +21135,15 @@
         if not line:
             continue
 
         key = line[:8].strip()
         value = line[8:]
 
         if not value.startswith('='):
-            # e.g., COMMENT, HISTORY
+            # for example, COMMENT or HISTORY
             if key + f'{sep}0' not in result:
                 result[key + f'{sep}0'] = value
                 counts[key] = 1
             else:
                 result[key + f'{sep}{counts[key]}'] = value
                 counts[key] += 1
             continue
@@ -21593,14 +21679,27 @@
 
     # pagedata is in memory and strips returns views so just call
     # ThreadPoolExecutor.map once
     with ThreadPoolExecutor(maxworkers) as executor:
         yield from executor.map(encode, strips())
 
 
+def zarr_selection(store: ZarrStore, selection: Any) -> NDArray[Any]:
+    """Return selection from Zarr store."""
+    import zarr
+
+    z = zarr.open(store, mode='r')
+    if isinstance(z, zarr.hierarchy.Group):
+        result = z[0][selection]
+    else:
+        result = z[selection]
+    store.close()
+    return result
+
+
 def reorient(
     image: NDArray[Any], orientation: ORIENTATION | int | str, /
 ) -> NDArray[Any]:
     """Return reoriented view of image array.
 
     Parameters:
         image:
@@ -21698,16 +21797,15 @@
     else:
         shape = data_or_shape.shape
     if len(shape) >= ndim:
         return data_or_shape
     shape = (1,) * (ndim - len(shape)) + shape
     if isinstance(data_or_shape, tuple):
         return shape
-    else:
-        return data_or_shape.reshape(shape)
+    return data_or_shape.reshape(shape)
 
 
 def squeeze_axes(
     shape: Sequence[int],
     axes: str,
     /,
     skip: str | None = None,
@@ -22367,33 +22465,33 @@
         # return Python value of token
         s = s.strip()
         if not s:
             return s
         if len(s) == 1:
             try:
                 return int(s)
-            except Exception:
+            except Exception as exc:
                 if fail:
-                    raise ValueError
+                    raise ValueError from exc
                 return s
         if s[0] == "'":
             if fail and s[-1] != "'" or "'" in s[1:-1]:
                 raise ValueError
             return s[1:-1]
         if s[0] == '<':
             if fail and s[-1] != '>' or '<' in s[1:-1]:
                 raise ValueError
             return s
         if fail and any(i in s for i in " ';[]{}"):
             raise ValueError
         if s[0] == '@':
             return s
-        if s == 'true' or s == 'True':
+        if s in {'true', 'True'}:
             return True
-        if s == 'false' or s == 'False':
+        if s in {'false', 'False'}:
             return False
         if s[:6] == 'zeros(':
             return numpy.zeros([int(i) for i in s[6:-1].split(',')]).tolist()
         if s[:5] == 'ones(':
             return numpy.ones([int(i) for i in s[5:-1].split(',')]).tolist()
         if '.' in s or 'e' in s:
             try:
@@ -22402,17 +22500,17 @@
                 pass
         try:
             return int(s)
         except Exception:
             pass
         try:
             return float(s)  # nan, inf
-        except Exception:
+        except Exception as exc:
             if fail:
-                raise ValueError
+                raise ValueError from exc
         return s
 
     def parse(s: str, /) -> Any:
         # return Python value from string representation of Matlab value
         s = s.strip()
         try:
             return value(s, True)
@@ -22863,30 +22961,30 @@
 def byteorder_isnative(byteorder: str, /) -> bool:
     """Return if byteorder matches system's byteorder.
 
     >>> byteorder_isnative('=')
     True
 
     """
-    if byteorder == '=' or byteorder == sys.byteorder:
+    if byteorder in {'=', sys.byteorder}:
         return True
     keys = {'big': '>', 'little': '<'}
     return keys.get(byteorder, byteorder) == keys[sys.byteorder]
 
 
 def byteorder_compare(byteorder: str, other: str, /) -> bool:
     """Return if byteorders match.
 
     >>> byteorder_compare('<', '<')
     True
     >>> byteorder_compare('>', '<')
     False
 
     """
-    if byteorder == other or byteorder == '|' or other == '|':
+    if byteorder in {other, '|'} or other == '|':
         return True
     if byteorder == '=':
         byteorder = {'big': '>', 'little': '<'}[sys.byteorder]
     elif other == '=':
         other = {'big': '>', 'little': '<'}[sys.byteorder]
     return byteorder == other
 
@@ -23319,16 +23417,15 @@
         elif 0 < abs(snipat) < 1:
             split = int(math.floor(linelen * snipat))
         else:
             split = int(snipat)
 
         if split < 0:
             split += linelen
-            if split < 0:
-                split = 0
+            split = max(split, 0)
 
         if esize == 0 or width < esize + 1:
             if split <= 0:
                 result.append(string[-width:])
             else:
                 result.append(string[:width])
         elif split <= 0:
@@ -23380,16 +23477,16 @@
 
     """
     try:
         return enum(arg)
     except Exception:
         try:
             return enum[arg.upper()]
-        except Exception:
-            raise ValueError(f'invalid argument {arg!r}')
+        except Exception as exc:
+            raise ValueError(f'invalid argument {arg!r}') from exc
 
 
 def parse_kwargs(
     kwargs: dict[str, Any], /, *keys: str, **keyvalues: Any
 ) -> dict[str, Any]:
     """Return dict with keys from keys|keyvals and values from kwargs|keyvals.
 
@@ -23766,63 +23863,63 @@
     """
     # TODO: rewrite detection of isrgb, iscontig
     # TODO: use planarconfig
     if photometric is None:
         photometric = 'RGB'
     if maxdim is None:
         maxdim = 2**16
-    isrgb = photometric in ('RGB', 'YCBCR')  # 'PALETTE', 'YCBCR'
+    isrgb = photometric in {'RGB', 'YCBCR'}  # 'PALETTE', 'YCBCR'
 
     if data.dtype == 'float16':
         data = data.astype('float32')
 
     if data.dtype.kind == 'b':
         isrgb = False
 
     if isrgb and not (
-        data.shape[-1] in (3, 4)
-        or (data.ndim > 2 and data.shape[-3] in (3, 4))
+        data.shape[-1] in {3, 4}
+        or (data.ndim > 2 and data.shape[-3] in {3, 4})
     ):
         isrgb = False
         photometric = 'MINISBLACK'
 
     data = data.squeeze()
-    if photometric in (
+    if photometric in {
         None,
         'MINISWHITE',
         'MINISBLACK',
         'CFA',
         'MASK',
         'PALETTE',
         'LOGL',
         'LOGLUV',
         'DEPTH_MAP',
         'SEMANTIC_MASK',
-    ):
+    }:
         data = reshape_nd(data, 2)
     else:
         data = reshape_nd(data, 3)
 
     dims = data.ndim
     if dims < 2:
         raise ValueError('not an image')
     if dims == 2:
         dims = 0
         isrgb = False
     else:
-        if isrgb and data.shape[-3] in (3, 4) and data.shape[-1] not in (3, 4):
+        if isrgb and data.shape[-3] in {3, 4} and data.shape[-1] not in {3, 4}:
             data = numpy.swapaxes(data, -3, -2)
             data = numpy.swapaxes(data, -2, -1)
         elif not isrgb and (
             data.shape[-1] < data.shape[-2] // 8
             and data.shape[-1] < data.shape[-3] // 8
         ):
             data = numpy.swapaxes(data, -3, -1)
             data = numpy.swapaxes(data, -2, -1)
-        isrgb = isrgb and data.shape[-1] in (3, 4)
+        isrgb = isrgb and data.shape[-1] in {3, 4}
         dims -= 3 if isrgb else 2
 
     if interpolation is None:
         threshold = 512
     elif isinstance(interpolation, int):
         threshold = interpolation
     else:
@@ -23854,15 +23951,15 @@
     elif data.dtype.kind in 'ui':
         if not (isrgb and data.dtype.itemsize <= 1) or bitspersample is None:
             try:
                 bitspersample = int(math.ceil(math.log(data.max(), 2)))
             except Exception:
                 bitspersample = data.dtype.itemsize * 8
         elif not isinstance(bitspersample, (int, numpy.integer)):
-            # bitspersample can be tuple, e.g., (5, 6, 5)
+            # bitspersample can be tuple, such as (5, 6, 5)
             bitspersample = data.dtype.itemsize * 8
         assert bitspersample is not None
         datamax = 2**bitspersample
         if isrgb:
             if bitspersample < 8:
                 data = data << (8 - bitspersample)
             elif bitspersample > 8:
@@ -24338,15 +24435,15 @@
                         if vmax <= vmin:
                             vmin, vmax = settings.vmin, settings.vmax
                 if series:
                     title = f'{tif}\n{page}\n{series}'
                 else:
                     title = f'{tif}\n {page}'
                 photometric = 'MINISBLACK'
-                if keyframe.photometric not in (3,):
+                if keyframe.photometric != 3:
                     photometric = PHOTOMETRIC(keyframe.photometric).name
                 imshow(
                     img,
                     title=title,
                     vmin=vmin,
                     vmax=vmax,
                     cmap=settings.cmap,
@@ -24404,15 +24501,15 @@
     def __get__(self, instance, owner):
         # with self.lock:
         if instance is None:
             return self
         try:
             value = self.func(instance)
         except AttributeError as exc:
-            raise RuntimeError(exc)
+            raise RuntimeError(exc) from exc
         if value is NotImplemented:
             return getattr(super(owner, instance), self.func.__name__)
         setattr(instance, self.func.__name__, value)
         return value
 
 
 if __name__ == '__main__':
```

### Comparing `tifffile-2023.4.12/tifffile.egg-info/PKG-INFO` & `tifffile-2023.7.4/tifffile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2023.4.12
+Version: 2023.7.4
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 License-File: LICENSE
 
 Read and write TIFF files
 =========================
 
 Tifffile is a Python library to
@@ -51,15 +52,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.12
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -87,33 +88,42 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.8.10, 3.9.13, 3.10.11, 3.11.3, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.3.16
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.14.2
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.4.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2023.7.4
+
+- Pass 4992 tests.
+- Add option to return selection from imread (#200).
+- Fix reading OME series with missing trailing frames (#199).
+- Fix fsspec reference for WebP compressed segments missing alpha channel.
+- Fix linting issues.
+- Detect files written by Agilent Technologies.
+- Drop support for Python 3.8 and numpy < 1.21 (NEP29).
+
 2023.4.12
 
-- Pass 4988 tests.
 - Do not write duplicate ImageDescription tags from extratags (breaking).
 - Support multifocal SVS files (#193).
 - Log warning when filtering out extratags.
 - Fix writing OME-TIFF with image description in extratags.
 - Ignore invalid predictor tag value if prediction is not used.
 - Raise KeyError if ZarrStore is missing requested chunk.
 
@@ -226,15 +236,15 @@
 - Convert some warnings to debug messages.
 - Declare all classes final.
 - Add script to generate documentation via Sphinx.
 - Convert docstrings to Google style with Sphinx directives.
 
 2022.5.4
 
-- ...
+- …
 
 Refer to the CHANGES file for older revisions.
 
 Notes
 -----
 
 TIFF, the Tagged Image File Format, was created by the Aldus Corporation and
@@ -418,14 +428,20 @@
 array to an interleaved RGB, a planar RGB, or a 3-page grayscale TIFF:
 
 >>> data = numpy.random.randint(0, 255, (3, 3, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb')
 >>> imwrite('temp.tif', data, photometric='rgb', planarconfig='separate')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
+Use the `extrasamples` argument to specify how extra components are
+interpreted, for example, for an RGBA image with unassociated alpha channel:
+
+>>> data = numpy.random.randint(0, 255, (256, 256, 4), 'uint8')
+>>> imwrite('temp.tif', data, photometric='rgb', extrasamples=['unassalpha'])
+
 Write a 3-dimensional NumPy array to a multi-page, 16-bit grayscale TIFF file:
 
 >>> data = numpy.random.randint(0, 2**12, (64, 301, 219), 'uint16')
 >>> imwrite('temp.tif', data, photometric='minisblack')
 
 Read the whole image stack from the multi-page TIFF file as NumPy array:
 
@@ -493,15 +509,15 @@
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
 
-Overwrite the value of an existing tag, e.g., XResolution:
+Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
@@ -632,19 +648,19 @@
 >>> with TiffWriter('temp.ome.tif', bigtiff=True) as tif:
 ...     metadata={
 ...         'axes': 'TCYXS',
 ...         'SignificantBits': 10,
 ...         'TimeIncrement': 0.1,
 ...         'TimeIncrementUnit': 's',
 ...         'PhysicalSizeX': pixelsize,
-...         'PhysicalSizeXUnit': 'Âµm',
+...         'PhysicalSizeXUnit': 'µm',
 ...         'PhysicalSizeY': pixelsize,
-...         'PhysicalSizeYUnit': 'Âµm',
+...         'PhysicalSizeYUnit': 'µm',
 ...         'Channel': {'Name': ['Channel 1', 'Channel 2']},
-...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['Âµm'] * 16}
+...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16}
 ...     }
 ...     options = dict(
 ...         photometric='rgb',
 ...         tile=(128, 128),
 ...         compression='jpeg',
 ...         resolutionunit='CENTIMETER'
 ...     )
```

### Comparing `tifffile-2023.4.12/tifffile.egg-info/SOURCES.txt` & `tifffile-2023.7.4/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

