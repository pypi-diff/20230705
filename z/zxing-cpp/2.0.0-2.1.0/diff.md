# Comparing `tmp/zxing-cpp-2.0.0.tar.gz` & `tmp/zxing-cpp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zxing-cpp-2.0.0.tar", last modified: Thu Jan  5 22:33:48 2023, max compression
+gzip compressed data, was "zxing-cpp-2.1.0.tar", last modified: Wed Jul  5 16:38:44 2023, max compression
```

## Comparing `zxing-cpp-2.0.0.tar` & `zxing-cpp-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,285 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 22:33:48.601654 zxing-cpp-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-01-05 22:33:46.000000 zxing-cpp-2.0.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-05 22:33:46.000000 zxing-cpp-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-05 22:33:48.601654 zxing-cpp-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-05 22:33:46.000000 zxing-cpp-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-05 22:33:46.000000 zxing-cpp-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 22:33:48.601654 zxing-cpp-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-01-05 22:33:46.000000 zxing-cpp-2.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-01-05 22:33:46.000000 zxing-cpp-2.0.0/zxing.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 22:33:48.601654 zxing-cpp-2.0.0/zxing_cpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-05 22:33:48.000000 zxing-cpp-2.0.0/zxing_cpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-05 22:33:48.000000 zxing-cpp-2.0.0/zxing_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 22:33:48.000000 zxing-cpp-2.0.0/zxing_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 22:33:48.000000 zxing-cpp-2.0.0/zxing_cpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-05 22:33:48.000000 zxing-cpp-2.0.0/zxing_cpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-05 22:33:48.000000 zxing-cpp-2.0.0/zxing_cpp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.839513 zxing-cpp-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-05 16:38:44.839513 zxing-cpp-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.807513 zxing-cpp-2.1.0/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/ZXVersion.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/ZXingConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.815513 zxing-cpp-2.1.0/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BarcodeFormat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BarcodeFormat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BinaryBitmap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BinaryBitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitHacks.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitMatrixCursor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitMatrixIO.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitMatrixIO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitSource.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/BitSource.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ByteArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ByteMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/CharacterSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/CharacterSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ConcentricFinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ConcentricFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Content.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Content.h
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/CustomData.h
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/DecodeHints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/DecodeHints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/DecoderResult.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/DetectorResult.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ECI.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ECI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Flags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GTIN.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GTIN.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GenericGF.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GenericGF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GenericGFPoly.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GenericGFPoly.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GlobalHistogramBinarizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GlobalHistogramBinarizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GridSampler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/GridSampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/HRI.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/HRI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/HybridBinarizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/HybridBinarizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ImageView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/LogMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/MultiFormatReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/MultiFormatReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/MultiFormatWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/MultiFormatWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Pattern.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/PerspectiveTransform.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/PerspectiveTransform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Point.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Quadrilateral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Range.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ReadBarcode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ReadBarcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ReedSolomonDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ReedSolomonDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ReedSolomonEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ReedSolomonEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/RegressionLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Result.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Result.h
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ResultPoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ResultPoint.h
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Scope.h
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/StructuredAppend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TextDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TextDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TextEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TextEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TextUtfEncoding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TextUtfEncoding.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ThresholdBinarizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/TritMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Utf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/Utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/WhiteRectDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/WhiteRectDetector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ZXAlgorithms.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ZXBigInteger.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ZXBigInteger.h
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ZXConfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ZXNullable.h
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/ZXTestSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.819513 zxing-cpp-2.1.0/core/src/aztec/
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZDetector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZDetectorResult.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZEncodingState.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZHighLevelEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZHighLevelEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZToken.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZToken.h
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/aztec/AZWriter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.819513 zxing-cpp-2.1.0/core/src/datamatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMBitLayout.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMBitLayout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMDataBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMDataBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31996 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMDetector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMECEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMECEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMEncoderContext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25853 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMHighLevelEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMHighLevelEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMSymbolInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMSymbolInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMSymbolShape.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMVersion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/datamatrix/DMWriter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.823513 zxing-cpp-2.1.0/core/src/libzueci/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    56583 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci.h
+-rw-r--r--   0 runner    (1001) docker     (123)   261105 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_big5.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_gb18030.h
+-rw-r--r--   0 runner    (1001) docker     (123)   158530 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_gb2312.h
+-rw-r--r--   0 runner    (1001) docker     (123)   271655 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_gbk.h
+-rw-r--r--   0 runner    (1001) docker     (123)   195926 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_ksx1001.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57278 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_sb.h
+-rw-r--r--   0 runner    (1001) docker     (123)   152478 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/libzueci/zueci_sjis.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.823513 zxing-cpp-2.1.0/core/src/maxicode/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/maxicode/MCBitMatrixParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/maxicode/MCBitMatrixParser.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/maxicode/MCDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/maxicode/MCDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/maxicode/MCReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/maxicode/MCReader.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.831513 zxing-cpp-2.1.0/core/src/oned/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCodabarReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCodabarReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCodabarWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCodabarWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode128Patterns.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode128Patterns.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode128Reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode128Reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode128Writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode128Writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode39Reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode39Reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode39Writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode39Writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode93Reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode93Reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode93Writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODCode93Writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarCommon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarCommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarExpandedBitDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarExpandedBitDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarExpandedReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarExpandedReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODDataBarReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODEAN13Writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODEAN13Writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODEAN8Writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODEAN8Writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODITFReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODITFReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODITFWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODITFWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODMultiUPCEANReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODMultiUPCEANReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODRowReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODRowReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODUPCAWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODUPCAWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODUPCEANCommon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODUPCEANCommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODUPCEWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODUPCEWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODWriterHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/oned/ODWriterHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.835513 zxing-cpp-2.1.0/core/src/pdf417/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFBarcodeMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFBarcodeValue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFBarcodeValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFBoundingBox.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFBoundingBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFCodeword.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45482 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFCodewordDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFCodewordDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFCompaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDecoderResultExtra.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDetectionResult.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDetectionResult.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDetectionResultColumn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDetectionResultColumn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFDetector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40307 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFHighLevelEncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFHighLevelEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFModulusGF.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFModulusGF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFModulusPoly.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFModulusPoly.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27667 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFScanningDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFScanningDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/pdf417/PDFWriter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.839513 zxing-cpp-2.1.0/core/src/qrcode/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRBitMatrixParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRBitMatrixParser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRCodecMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRCodecMode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDataBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDataBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDataMask.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDecoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRDetector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRECB.h
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QREncodeResult.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QREncoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QREncoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRErrorCorrectionLevel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRErrorCorrectionLevel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRFormatInformation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRFormatInformation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRMaskUtil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRMaskUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRMatrixUtil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRMatrixUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRVersion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRVersion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/src/qrcode/QRWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/core/zxing.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:38:44.839513 zxing-cpp-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/zxing.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-07-05 16:38:43.000000 zxing-cpp-2.1.0/zxing.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:38:44.839513 zxing-cpp-2.1.0/zxing_cpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-05 16:38:44.000000 zxing-cpp-2.1.0/zxing_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-05 16:38:44.000000 zxing-cpp-2.1.0/zxing_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:38:44.000000 zxing-cpp-2.1.0/zxing_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:38:44.000000 zxing-cpp-2.1.0/zxing_cpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 16:38:44.000000 zxing-cpp-2.1.0/zxing_cpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:38:44.000000 zxing-cpp-2.1.0/zxing_cpp.egg-info/top_level.txt
```

### Comparing `zxing-cpp-2.0.0/PKG-INFO` & `zxing-cpp-2.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: zxing-cpp
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python bindings for the zxing-cpp barcode library
 Home-page: https://github.com/zxing-cpp/zxing-cpp
 Author: ZXing-C++ Community
 Author-email: zxingcpp@gmail.com
 License: Apache License 2.0
 Keywords: barcode
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,15 +28,15 @@
 ```
 or
 
 ```bash
 python setup.py install
 ```
 
-Note: To install via `setup.py`, you need a suitable [build environment](https://github.com/zxing-cpp/zxing-cpp#build-instructions) including a c++ compiler.
+[Note: To install via `setup.py` (or via `pip install` in case there is no pre-build wheel available for your platfor or python version), you need a suitable [build environment](https://github.com/zxing-cpp/zxing-cpp#build-instructions) including a c++ compiler.]
 
 ## Usage
 
 ```python
 import cv2
 import zxingcpp
 
@@ -43,7 +44,11 @@
 results = zxingcpp.read_barcodes(img)
 for result in results:
 	print("Found barcode:\n Text:    '{}'\n Format:   {}\n Position: {}"
 		.format(result.text, result.format, result.position))
 if len(results) == 0:
 	print("Could not find any barcode.")
 ```
+
+To get a full list of available parameters for `read_barcodes` and `write_barcode` as well as the properties of the result objects, have a look at the `PYBIND11_MODULE` definition in [this c++ source file](https://github.com/zxing-cpp/zxing-cpp/blob/master/wrappers/python/zxing.cpp).
+
+
```

### Comparing `zxing-cpp-2.0.0/setup.py` & `zxing-cpp-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     # the .git directory of the repo, so that setuptools_scm cannot guess the current version.
     # use_scm_version={
     #     "root": "../..",
     #     "version_scheme": "guess-next-dev",
     #     "local_scheme": "no-local-version",
     #     "tag_regex": "v?([0-9]+.[0-9]+.[0-9]+)",
     # },
-    version='2.0.0',
+    version='2.1.0',
     description='Python bindings for the zxing-cpp barcode library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='ZXing-C++ Community',
     author_email='zxingcpp@gmail.com',
     url='https://github.com/zxing-cpp/zxing-cpp',
     license='Apache License 2.0',
```

### Comparing `zxing-cpp-2.0.0/zxing.cpp` & `zxing-cpp-2.1.0/zxing.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -46,46 +46,51 @@
 		.setTextMode(text_mode)
 		.setBinarizer(binarizer)
 		.setIsPure(is_pure)
 		.setMaxNumberOfSymbols(max_number_of_symbols)
 		.setEanAddOnSymbol(ean_add_on_symbol);
 	const auto _type = std::string(py::str(py::type::of(_image)));
 	Image image;
+	ImageFormat imgfmt = ImageFormat::None;
 	try {
+		if (_type.find("PIL.") != std::string::npos) {
+			_image.attr("load")();
+			const auto mode = _image.attr("mode").cast<std::string>();
+			if (mode == "L")
+				imgfmt = ImageFormat::Lum;
+			else if (mode == "RGB")
+				imgfmt = ImageFormat::RGB;
+			else if (mode == "RGBA")
+				imgfmt = ImageFormat::RGBX;
+			else {
+				// Unsupported mode in ImageFormat. Let's do conversion to L mode with PIL.
+				_image = _image.attr("convert")("L");
+				imgfmt = ImageFormat::Lum;
+			}
+		}
 		image = _image.cast<Image>();
-	}
-	catch(...) {
-		throw py::type_error("Unsupported type " + _type + ". Expect a PIL Image or numpy array");
+#if PYBIND11_VERSION_HEX > 0x02080000 // py::raise_from is available starting from 2.8.0
+	} catch (py::error_already_set &e) {
+		py::raise_from(e, PyExc_TypeError, ("Could not convert " + _type + " to numpy array of dtype 'uint8'.").c_str());
+		throw py::error_already_set();
+#endif
+	} catch (...) {
+		throw py::type_error("Could not convert " + _type + " to numpy array. Expecting a PIL Image or numpy array.");
 	}
 	const auto height = narrow_cast<int>(image.shape(0));
 	const auto width = narrow_cast<int>(image.shape(1));
-	auto channels = image.ndim() == 2 ? 1 : narrow_cast<int>(image.shape(2));
-	ImageFormat imgfmt;
-	if (_type.find("PIL.") != std::string::npos) {
-		const auto mode = _image.attr("mode").cast<std::string>();
-		if (mode == "L")
-			imgfmt = ImageFormat::Lum;
-		else if (mode == "RGB")
-			imgfmt = ImageFormat::RGB;
-		else if (mode == "RGBA")
-			imgfmt = ImageFormat::RGBX;
-		else {
-			// Unsupported mode in ImageFormat. Let's do conversion to L mode with PIL
-			image = _image.attr("convert")("L").cast<Image>();
-			imgfmt = ImageFormat::Lum;
-			channels = 1;
-		}
-	} else {
+	const auto channels = image.ndim() == 2 ? 1 : narrow_cast<int>(image.shape(2));
+	if (imgfmt == ImageFormat::None) {
 		// Assume grayscale or BGR image depending on channels number
 		if (channels == 1)
 			imgfmt = ImageFormat::Lum;
 		else if (channels == 3)
 			imgfmt = ImageFormat::BGR;
 		else
-			throw py::type_error("Unsupported number of channels for numpy array: " + std::to_string(channels));
+			throw py::value_error("Unsupported number of channels for numpy array: " + std::to_string(channels));
 	}
 
 	const auto bytes = image.data();
 	return ReadBarcodes({bytes, width, height, imgfmt, width * channels, channels}, hints);
 }
 
 std::optional<Result> read_barcode(py::object _image, const BarcodeFormats& formats, bool try_rotate, bool try_downscale,
@@ -132,15 +137,15 @@
 		.value("DataMatrix", BarcodeFormat::DataMatrix)
 		.value("EAN8", BarcodeFormat::EAN8)
 		.value("EAN13", BarcodeFormat::EAN13)
 		.value("ITF", BarcodeFormat::ITF)
 		.value("MaxiCode", BarcodeFormat::MaxiCode)
 		.value("PDF417", BarcodeFormat::PDF417)
 		.value("QRCode", BarcodeFormat::QRCode)
-		.value("MircoQRCode", BarcodeFormat::MicroQRCode)
+		.value("MicroQRCode", BarcodeFormat::MicroQRCode)
 		.value("DataBar", BarcodeFormat::DataBar)
 		.value("DataBarExpanded", BarcodeFormat::DataBarExpanded)
 		.value("UPCA", BarcodeFormat::UPCA)
 		.value("UPCE", BarcodeFormat::UPCE)
 		// use upper case 'NONE' because 'None' is a reserved identifier in python
 		.value("NONE", BarcodeFormat::None)
 		.value("LinearCodes", BarcodeFormat::LinearCodes)
```

### Comparing `zxing-cpp-2.0.0/zxing_cpp.egg-info/PKG-INFO` & `zxing-cpp-2.1.0/zxing_cpp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: zxing-cpp
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python bindings for the zxing-cpp barcode library
 Home-page: https://github.com/zxing-cpp/zxing-cpp
 Author: ZXing-C++ Community
 Author-email: zxingcpp@gmail.com
 License: Apache License 2.0
 Keywords: barcode
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -27,15 +28,15 @@
 ```
 or
 
 ```bash
 python setup.py install
 ```
 
-Note: To install via `setup.py`, you need a suitable [build environment](https://github.com/zxing-cpp/zxing-cpp#build-instructions) including a c++ compiler.
+[Note: To install via `setup.py` (or via `pip install` in case there is no pre-build wheel available for your platfor or python version), you need a suitable [build environment](https://github.com/zxing-cpp/zxing-cpp#build-instructions) including a c++ compiler.]
 
 ## Usage
 
 ```python
 import cv2
 import zxingcpp
 
@@ -43,7 +44,11 @@
 results = zxingcpp.read_barcodes(img)
 for result in results:
 	print("Found barcode:\n Text:    '{}'\n Format:   {}\n Position: {}"
 		.format(result.text, result.format, result.position))
 if len(results) == 0:
 	print("Could not find any barcode.")
 ```
+
+To get a full list of available parameters for `read_barcodes` and `write_barcode` as well as the properties of the result objects, have a look at the `PYBIND11_MODULE` definition in [this c++ source file](https://github.com/zxing-cpp/zxing-cpp/blob/master/wrappers/python/zxing.cpp).
+
+
```

