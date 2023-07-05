# Comparing `tmp/mccoygroup-mcutils-0.1.0.1.tar.gz` & `tmp/mccoygroup-mcutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccoygroup-mcutils-0.1.0.1.tar", last modified: Fri Mar 24 21:45:31 2023, max compression
+gzip compressed data, was "mccoygroup-mcutils-0.1.1.tar", last modified: Wed Jul  5 17:50:18 2023, max compression
```

## Comparing `mccoygroup-mcutils-0.1.0.1.tar` & `mccoygroup-mcutils-0.1.1.tar`

### file list

```diff
@@ -1,225 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.030073 mccoygroup-mcutils-0.1.0.1/McUtils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.030073 mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/
--rw-r--r--   0 runner    (1001) docker     (123)   145811 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/Permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/Sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.030073 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/Conveniences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.030073 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14789 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13283 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6157 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26533 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12958 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/DefaultConverters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8885 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.030073 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3640 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1573 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.030073 mccoygroup-mcutils-0.1.0.1/McUtils/Data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/AtomData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/BondData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7160 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/CommonData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15316 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/ConstantsData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/PotentialData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7767 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/QuantityArray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/
--rwxr-xr-x   0 runner    (1001) docker     (123)   114295 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/AtomData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13861 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/BondData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61435 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/ConstantsData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/PotentialData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/WavefunctionData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/Docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38079 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Docs/DocWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Docs/DocsBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Docs/ExamplesParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Docs/MarkdownTemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16442 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/ArgumentSignature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15111 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/CLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/DynamicFFILibrary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/Loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18255 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/Module.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4699 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/ModuleLoader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7145 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/SharedLibraryManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/ExternalPrograms/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/ExternalPrograms/Babel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/ExternalPrograms/OpenChem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/ExternalPrograms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7680 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/FChkDerivatives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5261 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianFChkComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13822 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianImporter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23349 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianLogComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.034073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/InteractiveTools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.038073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.038073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/ActiveHTMLWidget.json
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.038073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.038073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   322229 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js
--rw-r--r--   0 runner    (1001) docker     (123)    43040 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js
--rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)   299473 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js
--rw-r--r--   0 runner    (1001) docker     (123)   289256 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.038073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)   750963 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2514969 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.042073 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_nbextension_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/Bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    52345 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/BootstrapEnums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/Enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    41729 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/HTML.py
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/HTMLWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/HackWidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/JHTML.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/WidgetTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/MoleculeGraphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/NBExporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.042073 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/DebugTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/Decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/FileMatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/NumbaTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/SBatchHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/Singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)    28255 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/Symbolics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.042073 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateEngine/
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateEngine/ObjectWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateEngine/TemplateEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateEngine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateWriter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.046073 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38376 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/AnalyticDerivs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3743 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/EulerSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/Misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/Options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/SetOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    95985 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/Sparse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7552 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/TransformationMatrices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/TransformationTransformations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/VectorOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.046073 mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/
--rw-r--r--   0 runner    (1001) docker     (123)    58677 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/Parallelizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/Runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/SharedMemory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.046073 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/FileStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/Parsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36223 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/RegexPatterns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43416 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/StringParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48561 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/StructuredType.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.046073 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Backends.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    71035 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12351 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Interactive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45079 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Primitives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29775 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Properties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9315 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Styling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19806 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/VTKInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.046073 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/CLIs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Caches.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Checkpointing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21633 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/ObjectBackers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    37898 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6989 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/FittableModels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19361 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Interpolator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/LazyTensors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    81351 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/NeighborBasedInterpolators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7602 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/BaseSurface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/Surface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)    64296 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)    73503 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/TensorExpressions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30411 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/Derivatives.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34945 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19723 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/FunctionExpansions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5570 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/McUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-03-24 21:45:30.000000 mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-03-24 21:45:30.000000 mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 21:45:30.000000 mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-24 21:45:30.000000 mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 21:45:30.000000 mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 21:45:31.050073 mccoygroup-mcutils-0.1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-03-24 21:45:22.000000 mccoygroup-mcutils-0.1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1083 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.206547 mccoygroup-mcutils-0.1.1/McUtils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.206547 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/
+-rw-r--r--   0 runner    (1001) docker     (123)   157171 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.206547 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/Conveniences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2261 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14789 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13283 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6157 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26533 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12958 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/DefaultConverters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8885 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3640 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1573 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1603 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/AtomData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2444 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/BondData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7160 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/CommonData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15316 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/ConstantsData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/PotentialData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7767 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/QuantityArray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114295 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/AtomData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13861 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/BondData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61435 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/WavefunctionData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38079 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/DocWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/DocsBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/ExamplesParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/MarkdownTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16442 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/ArgumentSignature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15111 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/CLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.210548 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4229 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4699 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/ModuleLoader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7145 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/SharedLibraryManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/Babel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/OpenChem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7680 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/FChkDerivatives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5261 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13822 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianImporter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23349 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianLogComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/InteractiveTools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/ActiveHTMLWidget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.214548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.218548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   322229 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43040 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)   299473 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js
+-rw-r--r--   0 runner    (1001) docker     (123)   289256 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.218548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)   750963 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2514969 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52345 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41729 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HackWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/JHTML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/WidgetTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/MoleculeGraphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/NBExporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Jupyter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/DebugTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/Decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/FileMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/NumbaTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/SBatchHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/Singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28255 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/Symbolics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateWriter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Numputils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38376 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/AnalyticDerivs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3743 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/EulerSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/Misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/Options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/SetOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    95985 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/Sparse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7552 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationMatrices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationTransformations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23079 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/VectorOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Numputils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.222548 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    58677 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Parallelizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/SharedMemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16427 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/FileStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/Parsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36223 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/RegexPatterns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43416 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/StringParser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48561 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/StructuredType.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1470 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Plots/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Backends.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71035 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12351 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Interactive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45079 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11105 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Primitives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29775 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9360 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/Styling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19806 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/VTKInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/CLIs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2800 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Checkpointing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8561 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21633 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/ObjectBackers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6989 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/FittableModels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19361 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Interpolator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9707 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/LazyTensors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11104 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81351 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/NeighborBasedInterpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Polynomials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7602 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/BaseSurface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/Surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      740 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.226549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)    64296 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73503 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30417 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/Derivatives.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34945 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19721 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5570 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/Zachary/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/McUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 17:50:18.000000 mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 17:50:18.230549 mccoygroup-mcutils-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-07-05 17:50:07.000000 mccoygroup-mcutils-0.1.1/setup.py
```

### Comparing `mccoygroup-mcutils-0.1.0.1/LICENSE.txt` & `mccoygroup-mcutils-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/MANIFEST.in` & `mccoygroup-mcutils-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/Permutations.py` & `mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Permutations.py`

 * *Files 3% similar despite different names*

```diff
@@ -493,15 +493,15 @@
         import math
 
         subfac = np.prod([math.factorial(x) for x in counts])
         ndim_fac = math.factorial(np.sum(counts))
 
         return ndim_fac // subfac
 
-    def permutations(self, initial_permutation=None, return_indices=False, num_perms=None):
+    def permutations(self, initial_permutation=None, return_indices=False, num_perms=None, position_blocks=None):
         """
         Returns the permutations of the input array
         :param initial_permutation:
         :type initial_permutation:
         :param return_indices:
         :type return_indices:
         :param classes:
@@ -510,23 +510,93 @@
         :type counts:
         :param num_perms:
         :type num_perms:
         :return:
         :rtype:
         """
 
-        if initial_permutation is None:
-            initial_permutation = self.part
-            if num_perms is None:
-                num_perms = self.num_permutations
+        if position_blocks is None:
+            if initial_permutation is None:
+                initial_permutation = self.part
+                if num_perms is None:
+                    num_perms = self.num_permutations
+            else:
+                if num_perms is None:
+                    num_perms = self.num_permutations - self.index_permutations(initial_permutation)
+
+            return self.get_subsequent_permutations(initial_permutation, return_indices=return_indices, num_perms=num_perms)
         else:
-            if num_perms is None:
-                num_perms = self.num_permutations - self.index_permutations(initial_permutation)
+            # we'll read a position block spec like [3, 3, 4, 4, 4, 6, 6]
+            # to mean that the first two elements can only go as far as position 3,
+            # the third through fifth can only go as far as position 4
+            # and the sixth and seventh can go anywhere
+
+            # from this, we treat this by pairs of blocks, first getting all valid permutations for the final five elements
+            # under this constraint by taking all permutations of the final two elements and taking their direct product with
+            # the permutations of the third through fifth elements, since all of the space up through position 4 is taken up
+            # by elements that can only go up through position 4
+
+            # next, we take the permutations of the final 5 elements and instead of taking a plain direct product with the first two,
+            # since it's possible for the first two to go up through position 3 we need to first enumerate the partitions of
+            # the first two elements AND two dummy elements that will correspond to the first two elements of the partition of
+            # each permutation of the final 5
+
+            # these two sets of permutations can be composed by determining where the dummy elements go in the permutations of
+            # the first four and simply populating the appropriate locations in a tensor of permutations
+
+            # in this way, we can build up the full set of valid permutations by taking direct-products with substitution of
+            # each valid subblock
+
+            block_edges = np.where(np.diff(position_blocks) != 0)
+            if len(block_edges) == 0:
+                return self.permutations(initial_permutation=initial_permutation, return_indices=return_indices, num_perms=num_perms, position_blocks=None)
+
+            # if initial_permutation is None:
+            #     initial_permutation = self.part
+            #     if num_perms is None:
+            #         num_perms = self.num_permutations
+            # else:
+            #     if num_perms is None:
+            #         num_perms = self.num_permutations - self.index_permutations(initial_permutation)
 
-        return self.get_subsequent_permutations(initial_permutation, return_indices=return_indices, num_perms=num_perms)
+            idx_blocks = np.split(position_blocks, block_edges[0]+1)
+            groups = np.split(self.part, block_edges[0]+1)
+
+            perm_blocks = []
+            cur = 0
+            for part, block in zip(groups, idx_blocks):
+                end = block[0] + 1
+                block_len = end - cur
+                cur += len(part)
+                padding = block_len - len(part)
+                padding_indices = np.flip(np.arange(padding))
+                padded_part = np.concatenate([part + padding, padding_indices])
+                perm_blocks.append([UniquePermutations(padded_part).permutations(), padding_indices])
+
+            num_perms = np.prod([len(b[0]) for b in perm_blocks], dtype=int)
+            storage = np.zeros((num_perms, len(self.part)), dtype=self.part.dtype)
+            end_idx = len(self.part)
+            for block, swaps in reversed(perm_blocks):
+                reps = num_perms // len(block)
+                nswaps = len(swaps)
+                if nswaps > 0:
+                    inserts = storage[:, end_idx:end_idx+nswaps].copy()
+                    insert_where = [np.where(block==s)[1] for s in swaps] # note that swaps is inverted from arange
+                    block_size, nel = block.shape
+                    bs = end_idx - nel + nswaps
+                    for i in range(reps):
+                        storage[i*block_size:(i+1)*block_size, bs:bs+nel] = block - nswaps
+                        for j,w in enumerate(insert_where):
+                            storage[np.arange(i*block_size, (i+1)*block_size), w] = inserts[i*block_size:(i+1)*block_size, j]
+                else:
+                    bs = end_idx - len(block[0])
+                    storage[:, bs:end_idx] = np.broadcast_to(block[np.newaxis], (reps,) + block.shape).reshape((reps * block.shape[0], block.shape[1]))
+                end_idx = bs
+
+            return storage
 
     @classmethod
     def get_subsequent_permutations(cls, initial_permutation, return_indices=False, classes=None, counts=None, num_perms=None):
         """
         Returns the permutations of the input array
         :return:
         :rtype:
@@ -566,43 +636,45 @@
         """
         Builds off of this algorithm for generating permutations
         in lexicographic order: https://en.wikipedia.org/wiki/Permutation#Generation_in_lexicographic_order
         Then we adapt it so that it works in _reverse_ lex order since that's how our partitions come in
         This adaption is done just by pretending the the numbers are all negated so all ordering relations
         flip
 
+        We also make it so a given partition element can only go out to `max_pos`
+
         :param storage:
         :type storage:
         :param inds:
         :type inds:
         :return:
         :rtype:
         """
 
         swap = np.arange(len(partition))
-        for i in range(len(storage)):
-            storage[i] = partition
+        for n in range(len(storage)):
+            storage[n] = partition
             if inds is not None:
-                inds[i] = swap
+                inds[n] = swap
 
             # find largest index such that the next element in the
             # partition is smaller (i.e. find where we need to do our next swap)
             # I'd like to do this with numpy builtins instead of a loop
             # or maybe some partial ordering approach or something
             # but don't have it quite figured out yet
-            for i in range(dim-2, -1, -1):
+            for i in range(dim - 2, -1, -1):
                 if partition[i] > partition[i+1]:
                     break
             else:
                 break
 
             # find the next-smallest index such that
             # the partition element is smaller than the one at the swap
             # position
-            for j in range(dim-1, i, -1):
+            for j in range(dim - 1, i, -1):
                 if partition[i] > partition[j]:
                     break
 
             # swap the terms and reverse the sequence of elements leading
             # up to it
             tmp = partition[j]
             partition[j] = partition[i]
@@ -831,25 +903,26 @@
             class_map[v] = i
 
         init_counts = counts
         nterms = len(counts)
 
         ndim = dim
 
+        # back track the initial number of states
         n_steps = int(np.ceil(len(perms)/block_size))
-        block_counts = np.zeros((n_steps, len(counts)), dtype=counts.dtype)
+        block_counts = np.zeros((n_steps, len(counts)))#, dtype=counts.dtype)
         for i in range(n_steps):
             block_counts[i] = counts
 
-        block_tree_datas = np.zeros((n_steps, dim, 2), dtype=counts.dtype)
+        block_tree_datas = np.zeros((n_steps, dim, 2))#, dtype=counts.dtype)
         cur_dims = np.full(n_steps, dim - 1)
         block_tree_datas[:, cur_dims[0], 1] = num_permutations
 
         half_dim = ndim // 2
-        for _ in prange(n_steps):
+        for _ in prange(n_steps): # we iterate over initial states
             idx_start = block_size * _
 
             cur_dim = cur_dims[_]
             tree_data = block_tree_datas[_]
             cts = block_counts[_]
 
             rem_els = block_size if idx_start + block_size < len(perms) else len(perms) - idx_start
@@ -2177,15 +2250,16 @@
     @classmethod
     def _filter_negatives_perms(cls,
                                 i, idx, idx_starts, perms, new_rep_perm,
                                 storage,
                                 ndim,
                                 cls_inds, class_negs,
                                 perm_counts, cum_counts,
-                                mask, can_be_negative
+                                mask, can_be_negative,
+                                full_rep_changes, changed_positions
                                 ):
         # if we run into negatives we need to mask them out
         if len(can_be_negative[i]) == 0:
             not_negs = np.full(len(cls_inds[i]), True)
         else:
             not_negs = cls._get_filter_mask(new_rep_perm, cls_inds[i], can_be_negative[i], class_negs)
 
@@ -2197,14 +2271,18 @@
             cls._filter_negs_by_comp(comp, not_negs, idx, idx_starts, mask, perm_counts, cum_counts[i],
                                       cum_counts[i + 1])
         if len(comp) > 0:
             sel = np.where(not_negs)[0]
             new_perms = new_rep_perm[sel[:, np.newaxis, np.newaxis], perms[np.newaxis, :, :]]
             stored_inds = np.reshape(sel[:, np.newaxis] + idx_starts[np.newaxis, :], -1)
             storage[stored_inds] = new_perms.reshape(-1, ndim)
+
+            if changed_positions is not None:
+                full_change_mask = full_rep_changes[sel[:, np.newaxis, np.newaxis], perms[np.newaxis, :, :]]
+                changed_positions[stored_inds] = cls._compute_changed_index_numbers(full_change_mask.reshape(-1, ndim))
         else:
             sel = []
             new_perms = None
 
         return comp, sel, new_perms
 
     # def filter_from_ind_spec(i, j, block_idx, block_sizes, insert_inds, full_inds_sorted, inv, *,
@@ -2277,19 +2355,41 @@
                 # 'storage_blocks': [stored_inds],
                 block_sizes = np.cumsum([len(x) for x in block_dat['storage_blocks']])
                 for b, s in zip(block_dat['idx_blocs'], np.split(sort_mask, block_sizes)):
                     perm_counts[b[0]:b[1], b[2]] -= 1 - s
 
                 # filter_from_ind_spec(i, j, block_idx, block_sizes, perm_pos, full_inds_sorted, inv)
 
+    @classmethod
+    def changed_index_number(cls, idx, radix):
+        return np.ravel_multi_index(np.sort(idx)+1, [radix+1]*len(idx))
+    @classmethod
+    def _compute_changed_index_numbers(cls, mask):
+        # we loop for this because I'm not totally sure how to do better here...
+        if not mask.any():
+            return np.zeros(len(mask))
+        radix = len(mask[0])
+        indices = np.where(mask,
+                        np.broadcast_to(np.arange(radix)[np.newaxis], mask.shape),
+                        np.full(mask.shape, -1)
+                        )
+        sorted = np.sort(indices, axis=-1)
+        # now we prune out bad elements
+        max_col = np.min(np.where(sorted > -1)[1])
+        sorted = sorted[:, max_col:]+1
+        # raise Exception(sorted, max_col)
+        return np.ravel_multi_index(sorted.T, [radix+1]*(radix-max_col))
+        # return np.array([cls.changed_index_number(np.where(m)[0], radix) for m in mask])
+
     def _build_direct_sums(self,
                            input_perm_classes,
                            counts,
                            classes,
                            return_indices=False,
+                           return_change_positions=False,
                            return_excitations=True,
                            filter_negatives=True,
                            allow_widen_dtypes=True,
                            filter=None, inds_dtype=None,
                            excluded_permutations=None,
                            full_basis=None
                            ):
@@ -2305,17 +2405,20 @@
         :type counts:
         :param classes:
         :type classes:
         :return:
         :rtype:
         """
 
-        input_perm_classes = [(_as_pos_neg_dtype(x[0]), _as_pos_neg_dtype(x[1]), x[2],
-                               UniquePermutations.get_standard_permutation(_as_pos_neg_dtype(x[1]), _as_pos_neg_dtype(x[0]))
-                               ) for x in input_perm_classes]
+        #prepare initial permutation data for grouping
+        input_perm_classes = [
+            (_as_pos_neg_dtype(x[0]), _as_pos_neg_dtype(x[1]), x[2],
+             UniquePermutations.get_standard_permutation(_as_pos_neg_dtype(x[1]), _as_pos_neg_dtype(x[0]))
+             ) for x in input_perm_classes
+        ]
 
         # set up storage
         num_perms = UniquePermutations.count_permutations(counts)
 
         if inds_dtype is None:
             inds_dtype = int
 
@@ -2407,14 +2510,19 @@
                 inferred = _infer_dtype(max_val + max_rule)
                 if inferred > dtype:
                     dtype = inferred
 
         storage = np.zeros((total_perm_count, ndim), dtype=dtype)
         if return_indices:
             indices = np.zeros((total_perm_count,), dtype=inds_dtype)
+        if return_change_positions:
+            changed_positions = np.full((total_perm_count,), -1, dtype=int)
+        else:
+            changed_positions = None
+
 
         if filter is not None or (filter_negatives and any(len(x)>0 for x in can_be_negative)):
             mask = np.full((total_perm_count,), True)
         else:
             mask = None
 
         storage_indexing_dtype = _infer_dtype(total_perm_count)
@@ -2422,14 +2530,15 @@
         # make it easier to determine where the total runtime is
         # del cls_inds
         cls_cache = {}
         def add_new_perms(idx, perm, cls_pos, cts, depth, tree_data,
                           classes=classes,
                           input_perm_classes=input_perm_classes,
                           class_negatives=class_negatives,
+                          changed_positions=changed_positions,
                           excluded_permutations=excluded_permutations
                           ):
             """
             Adds each new permutation to the existing states
              and then to the final storage
 
             :param idx: which permutation this one is
@@ -2445,14 +2554,19 @@
             :param class_negatives: the combinations within each class that can be negative?
             :type class_negatives:
             :return:
             :rtype:
             """
 
             class_perms = np.array([c[perm] for c in classes])
+            if changed_positions is not None:
+                changes = class_perms != 0
+            else:
+                changes = None
+
             class_neg_list = [
                 np.concatenate([cls_pos[j] for j in neg]) if len(neg) > 0 else ()
                 for neg in class_negatives
             ]
             for i,class_data in enumerate(input_perm_classes):
                 if len(cls_inds[i]) == 0:
                     continue
@@ -2480,30 +2594,40 @@
                 #         keep = np.setdiff1d(np.arange(len(added)), exclude)
                 #         added = added[keep,]
                 #         # we need to update the mask appropriately...
                 #     print(perms)
                 # else:
                 #     keep = np.arange(len(added))
                 new_rep_perm = rep[np.newaxis, :] + class_perms[cls_inds[i], :]
+                if changes is not None:
+                    full_rep_changes = changes[cls_inds[i], :]
+                    # print(full_rep_changes)
+                else:
+                    full_rep_changes = None
                 if filter_negatives and mask is not None:
                     class_negs = tuple(np.array(class_neg_list[j], dtype=class_negatives[0].dtype) for j in cls_inds[i])
                     comp, sel, new_perms = self._filter_negatives_perms(
                                 i, idx, idx_starts, perms, new_rep_perm,
                                 storage,
                                 ndim,
                                 cls_inds, class_negs,
                                 perm_counts, cum_counts,
-                                mask, can_be_negative
+                                mask, can_be_negative,
+                                full_rep_changes, changed_positions
                                 )
                 else:
                     comp = cls_inds[i]
                     sel = np.arange(len(cls_inds[i]))#np.where(not_negs)[0]
                     new_perms = new_rep_perm[sel[:, np.newaxis, np.newaxis], perms[np.newaxis, :, :]]
                     stored_inds = np.reshape(sel[:, np.newaxis] + idx_starts[np.newaxis, :], -1)
                     storage[stored_inds] = new_perms.reshape(-1, ndim)
+                    if changes is not None:
+                        full_change_mask = full_rep_changes[sel[:, np.newaxis, np.newaxis], perms[np.newaxis, :, :]]
+                        changed_positions[stored_inds] = self._compute_changed_index_numbers(full_change_mask.reshape(-1, ndim))
+
 
                     # raise NotImplementedError("need to get storage right but never touch this code path anymore")
                     # comp = cls_inds[i]
                     # sel = np.arange(len(comp))
                     # new_perms = new_rep_perm[:, perms].transpose(1, 0, 2)
                     # # shape used to be `(total_perm_count, num_perms, len(classes), ndim)`
                     # # but we collapsed this down to a 2D shape so we could use less memory/calculate less
@@ -2542,23 +2666,27 @@
             # process_cached_index_blocks(storage)
 
         if mask is not None:
             if return_excitations:
                 storage = storage[mask]
             if return_indices:
                 indices = indices[mask]
+            if return_change_positions:
+                changed_positions = changed_positions[mask]
         perm_counts = np.sum(perm_counts, axis=1)
 
         if not return_excitations:
             storage = None
 
+        ret = (storage, perm_counts)
         if return_indices:
-            return storage, perm_counts, indices
-        else:
-            return storage, perm_counts
+            ret = ret + (indices,)
+        if return_change_positions:
+            ret = ret + (changed_positions,)
+        return ret
 
     def _get_direct_sum_rule_groups(self, rules, dim, dtype):
         # first up we pad the rules
         rules = [
             np.concatenate([np.array(r, dtype=dtype), np.zeros(dim - len(r), dtype=dtype)]) if len(
                 r) < dim else np.array(r, dtype=dtype)
             for r in rules
@@ -2656,14 +2784,15 @@
 
     def take_permutation_rule_direct_sum(self,
                                          perms, rules,
                                          sums=None,
                                          assume_sorted=False,
                                          return_indices=False,
                                          return_excitations=True,
+                                         return_change_positions=False,
                                          full_basis=None,
                                          split_results=False,
                                          excluded_permutations=None,
                                          filter_perms=None,
                                          return_filter=False,
                                          preserve_ordering=True,
                                          indexing_method='direct',
@@ -2698,15 +2827,15 @@
         if isinstance(perms.dtype, np.unsignedinteger):
             perms = perms.astype(_infer_nearest_pos_neg_dtype(perms.dtype))
         if perms.dtype.names is not None:
             perms = unflatten_dtype(perms, (len(perms), self.dim), perms.dtype[0])
 
         if perms.ndim == 1:
             perms = perms[np.newaxis]
-        # og_perms = perms # for debug
+        og_perms = perms # for debug
         # next we pad up the perms as needed
         if perms.shape[1] < dim:
             perms = np.concatenate([
                 perms,
                 np.zeros((perms.shape[0], dim - perms.shape[1]), dtype=perms.dtype)
             ],
                 axis=1
@@ -2821,14 +2950,16 @@
             return_indices = False
         else:
             secondary_inds = False
 
         perms = []
         if return_indices:
             indices = []
+        if return_change_positions:
+            changes = []
 
         # we now set up filtering so that we can efficiently prune branches
         # as we calculate partition permutations
         filter = self.direct_sum_filter.from_data(self, filter_perms)
         if filter is not None and not return_indices:
             raise ValueError("if a filter is used indices must be requested since they are used in filtering")
 
@@ -2856,35 +2987,66 @@
                         input_classes_fmt = ["Class/Counts/Permutations"] + [
                              "{}/{}/{}".format(y[0], y[1], len(y[2])) for y in input_classes
                         ]
                         logger.log_print(input_classes_fmt, log_level=logger.LogLevel.Debug)
                     perm_block = []
                     if return_indices:
                         ind_block = []
+                    if return_change_positions:
+                        change_block = []
 
                     for counts, classes, exc in zip(rule_counts, rule_classes, excluded_permutations):
                         res = self._build_direct_sums(input_classes, counts, classes,
                                                       return_indices=return_indices,
                                                       return_excitations=return_excitations,
+                                                      return_change_positions=return_change_positions,
                                                       filter=filter, inds_dtype=inds_dtype,
                                                       excluded_permutations=exc,
                                                       full_basis=full_basis
                                                       )
                         # gc.collect()
                         if split_results or preserve_ordering:
                             split_blocks = np.cumsum(res[1][:-1])
                             if return_excitations:
                                 res_perms = np.split(res[0], split_blocks)
                             if return_indices:
                                 ind_block.append(np.split(res[2], split_blocks))
+                            if return_change_positions:
+                                if return_indices:
+                                    change_block.append(np.split(res[3], split_blocks))
+                                else:
+                                    change_block.append(np.split(res[2], split_blocks))
+                                # x = input_classes[0]
+                                # p0 = UniquePermutations.get_standard_permutation(_as_pos_neg_dtype(x[1]), _as_pos_neg_dtype(x[0]))
+                                # test = res_perms[0] - p0[np.newaxis]
+                                # radix = len(test[0])
+                                # test_changes = np.array([
+                                #     self.changed_index_number(np.where(idx != 0)[0], radix)
+                                #     for idx in test
+                                # ])
+                                # if (test_changes != change_block[-1][0]).any():
+                                #     raise Exception(
+                                #         p0,
+                                #         [
+                                #             np.where(idx != 0)[0]
+                                #             for idx in test
+                                #         ],
+                                #         test_changes,
+                                #         change_block[-1][0]
+                                #     )
                         else:
                             if return_excitations:
                                 res_perms = res[0]
                             if return_indices:
                                 ind_block.append(res[2])
+                            if return_change_positions:
+                                if return_indices:
+                                    change_block.append(res[3])
+                                else:
+                                    change_block.append(res[2])
                         if return_excitations:
                             perm_block.append(res_perms)
 
                     # if nq == 5:# and len(counts) == 3 and counts[-1] == 9:
                     #     #     raise Exception(perm_pos.dtype)
                     #     raise Exception("oookay")
 
@@ -2914,21 +3076,36 @@
                             if preserve_ordering and sorts is not None and len(new_inds) > 0:
                                 if not return_excitations:
                                     cumlens = np.cumsum([0] + [len(x) for x in sorts[:-1]])
                                     sorts = np.concatenate([x + s for x, s in zip(sorts, cumlens)])
                                     argsorts = np.argsort(sorts)
                                 new_inds = [new_inds[i] for i in argsorts]
                             indices.append(new_inds)
+                        if return_change_positions:
+                            new_chng = [
+                                np.concatenate(blocks)
+                                for blocks in zip(*change_block)
+                            ]
+                            if preserve_ordering and sorts is not None and len(new_inds) > 0:
+                                # if not return_excitations:
+                                #     cumlens = np.cumsum([0] + [len(x) for x in sorts[:-1]])
+                                #     sorts = np.concatenate([x + s for x, s in zip(sorts, cumlens)])
+                                #     argsorts = np.argsort(sorts)
+                                new_chng = [new_chng[i] for i in argsorts]
+                            changes.append(new_chng)
                     else:
                         if return_excitations:
                             new_perms = np.concatenate(perm_block, axis=0)
                             perms.append(new_perms)
                         if return_indices:
                             new_inds = np.concatenate(ind_block)
                             indices.append(new_inds)
+                        if return_change_positions:
+                            new_chng = np.concatenate(change_block)
+                            changes.append(new_chng)
 
                     if return_excitations:
                         subend = time.time()
                         logger.log_print([
                             'got {nt} partition-permutations{and_inds}',
                             'took {e:.3f}s...'
                         ],
@@ -2973,30 +3150,50 @@
                         indices = new_inds
                     else:
                         indices = sum(indices, [])
                     if preserve_ordering and sum_sorting is not None and len(indices) > 0:
                         if not return_excitations:
                             inv = np.argsort(sum_sorting)
                         indices = [indices[i] for i in inv]
+                if return_change_positions:
+                    if preserve_ordering:
+                        new_chng = []
+                        for d,s in zip(changes, perm_sorting):
+                            if len(d) > 0:
+                                new_chng += [d[i] for i in np.argsort(s)]
+                        changes = new_chng
+                    else:
+                        changes = sum(new_chng, [])
+                    if preserve_ordering and sum_sorting is not None and len(changes) > 0:
+                        # if not return_excitations:
+                        #     inv = np.argsort(sum_sorting)
+                        changes = [changes[i] for i in inv]
                 if not split_results:
                     if return_excitations:
                         if len(perms) == 0:
                             perms = np.array([], dtype='int8')
                         else:
                             perms = np.concatenate(perms, axis=0)
                     if return_indices:
                         if len(perms) == 0:
                             indices = np.array([], dtype='int8')
                         else:
                             indices = np.concatenate(indices, axis=0)
+                    if return_change_positions:
+                        if len(perms) == 0:
+                            changes = np.array([], dtype='int8')
+                        else:
+                            changes = np.concatenate(changes, axis=0)
             else:
                 if return_excitations:
                     perms = np.concatenate(perms, axis=0)
                 if return_indices:
                     indices = np.concatenate(indices)
+                if return_change_positions:
+                    changes = np.concatenate(changes)
 
             end = time.time()
             if return_excitations:
                 logger.log_print([
                     'in total got {nt} partition-permutations{and_inds}',
                     'took {e:.3f}s...'
                     ],
@@ -3013,33 +3210,45 @@
                     nt=len(indices) if not (split_results or preserve_ordering) else sum(len(x) for x in indices),
                     e=end-start,
                     log_level=logger.LogLevel.Debug
                 )
 
             if not return_excitations:
                 perms = None
-            if return_indices:
-                if return_filter:
-                    return perms, indices, filter
-                else:
-                    return perms, indices
-            elif secondary_inds:
+            ret = (perms,)
+            if secondary_inds:
                 if split_results:
                     full_perms = np.concatenate(perms, axis=0)
                     indices = self.to_indices(full_perms)
                     splits = np.cumsum([len(x) for x in perms])[:-1]
                     indices = np.split(indices, splits)
                 else:
                     indices = self.to_indices(perms)
-                if return_filter:
-                    return perms, indices, filter
-                else:
-                    return perms, indices
-            else:
-                return perms
+            if return_indices:
+                ret += (indices,)
+            if return_change_positions:
+                ret += (changes,)
+            if return_filter:
+                ret += (filter,)
+            #     return ret
+            # elif secondary_inds:
+            #     if split_results:
+            #         full_perms = np.concatenate(perms, axis=0)
+            #         indices = self.to_indices(full_perms)
+            #         splits = np.cumsum([len(x) for x in perms])[:-1]
+            #         indices = np.split(indices, splits)
+            #     else:
+            #         indices = self.to_indices(perms)
+            #
+            #     if return_filter:
+            #         return perms, indices, filter
+            #     else:
+            #         return perms, indices
+
+            return ret
 
 class CompleteSymmetricGroupSpace:
     """
     An object representing a full integer partition-permutation basis
     which will work nominally at any level of excitation
     """
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/Sequences.py` & `mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/Sequences.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Combinatorics/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Combinatorics/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/Conveniences.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/Conveniences.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToSpherical.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CartesianToZMatrix.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CommonCoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CompositeCoordinateSystems.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSet.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateSystemConverter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/CoordinateUtils.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/SphericalToCartesian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/ZMatrixToCartesian.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateSystems/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateSystems/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/AffineTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/CoordinateTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/RotationTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/ScalingTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TransformationFunction.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/TranslationTransform.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/CoordinateTransformations/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Coordinerds/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Coordinerds/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/AtomData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/AtomData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/BondData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/BondData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/CommonData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/CommonData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/ConstantsData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/ConstantsData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/PotentialData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/PotentialData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/QuantityArray.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/QuantityArray.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/AtomData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/AtomData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/BondData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/BondData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/ConstantsData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/ConstantsData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/PotentialData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/PotentialData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/TheRealMcCoy/WavefunctionData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/WavefunctionData.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/WavefunctionData.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Data/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Data/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Docs/DocWalker.py` & `mccoygroup-mcutils-0.1.1/McUtils/Docs/DocWalker.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Docs/DocsBuilder.py` & `mccoygroup-mcutils-0.1.1/McUtils/Docs/DocsBuilder.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Docs/ExamplesParser.py` & `mccoygroup-mcutils-0.1.1/McUtils/Docs/ExamplesParser.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Docs/MarkdownTemplates.py` & `mccoygroup-mcutils-0.1.1/McUtils/Docs/MarkdownTemplates.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/ArgumentSignature.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/ArgumentSignature.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/CLoader.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/CLoader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/DynamicFFILibrary.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/DynamicFFILibrary.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/Loader.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Loader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/FFI/Module.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/FFI/Module.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     _type_map[NUMPY_Float32] = ("float32", np.float32)
     NUMPY_Float64 = NUMPY_TYPES + 22
     _type_map[NUMPY_Float64] = ("float64", np.float64)
     NUMPY_Float128 = NUMPY_TYPES + 23
     _type_map[NUMPY_Float128] = ("float128", np.float128)
 
     NUMPY_Bool = NUMPY_TYPES + 30
-    _type_map[NUMPY_Bool] = ("bool", np.bool)
+    _type_map[NUMPY_Bool] = ("bool", bool)
 
     @classmethod
     def type_data(cls, val):
         mapp = cls._type_map.value
         if isinstance(val, cls):
             val = val.value
         return mapp[val]
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/ModuleLoader.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/ModuleLoader.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/SharedLibraryManager.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/SharedLibraryManager.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Extensions/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/ExternalPrograms/Babel.py` & `mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/Babel.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/ExternalPrograms/OpenChem.py` & `mccoygroup-mcutils-0.1.1/McUtils/ExternalPrograms/OpenChem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/FChkDerivatives.py` & `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/FChkDerivatives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianFChkComponents.py` & `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianFChkComponents.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianImporter.py` & `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianImporter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianJob.py` & `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianJob.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/GaussianLogComponents.py` & `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/GaussianLogComponents.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/GaussianInterface/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/GaussianInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Apps.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Apps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Controls.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Controls.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Interfaces.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Interfaces.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/Variables.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/Variables.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/Apps/types.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/Apps/types.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/InteractiveTools.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/InteractiveTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/package.json`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/css_index_css.0a349ad0ce82fa2494b2.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_index_js.bf6ffa79db984e284e73.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_plugin_js.b1c0c1ef97bb24e5f05c.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/lib_widget_js.211a0992bac58d84b14c.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/remoteEntry.3a5659ddcc7f242cedc3.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.cae8f50ef89487b19021.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/labextension/static/vendors-node_modules_jquery_dist_jquery_js.4405729320014649bb98.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/ActiveHTMLWidget/widget.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/Bootstrap.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Bootstrap.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/BootstrapEnums.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapEnums.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/BootstrapWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/Enums.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/Enums.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/HTML.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTML.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/HTMLWidgets.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HTMLWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/HackWidgets.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/HackWidgets.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/JHTML.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/JHTML.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/WidgetTools.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/WidgetTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/JHTML/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/JHTML/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/MoleculeGraphics.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/MoleculeGraphics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/NBExporter.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/NBExporter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Jupyter/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/DebugTools.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/DebugTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/FileMatcher.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/FileMatcher.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/NumbaTools.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/NumbaTools.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/SBatchHelper.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/SBatchHelper.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/Symbolics.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/Symbolics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateEngine/ObjectWalker.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/ObjectWalker.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateEngine/TemplateEngine.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateEngine/TemplateEngine.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/TemplateWriter.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/TemplateWriter.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Misc/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/AnalyticDerivs.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/AnalyticDerivs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/EulerSystem.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/EulerSystem.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/Misc.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/Misc.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/Options.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/Options.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/SetOps.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/SetOps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/Sparse.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/Sparse.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/TransformationMatrices.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationMatrices.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/TransformationTransformations.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/TransformationTransformations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/VectorOps.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/VectorOps.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Numputils/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Numputils/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/Parallelizers.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Parallelizers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/Runner.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/Runner.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/SharedMemory.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/SharedMemory.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parallelizers/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parallelizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/FileStreamer.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parsers/FileStreamer.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/Parsers.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parsers/Parsers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/RegexPatterns.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parsers/RegexPatterns.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/StringParser.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parsers/StringParser.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/StructuredType.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parsers/StructuredType.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Parsers/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Graphics.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Graphics.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Image.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Image.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Interactive.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Interactive.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Plots.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Plots.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Primitives.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Primitives.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Properties.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Properties.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/Styling.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/Styling.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,16 @@
 
 class ThemeManager:
     """
     Simple manager class for plugging into themes in a semi-background agnostic way
     """
     extra_themes = {
         'mccoy': (
-            ('seaborn-dark-palette'),
+            # ('seaborn-dark-palette'),
+            ('seaborn-v0_8-dark-palette'),
             {
                 'axes.labelsize': 13,
                 'xtick.labelsize':13,
                 'ytick.labelsize':13,
                 'padding': 50,
                 'aspect_ratio': 'auto'
             }
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/VTKInterface.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/VTKInterface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Plots/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/CLIs.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/CLIs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Caches.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Caches.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Checkpointing.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Checkpointing.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Configurations.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Configurations.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Jobs.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Jobs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Logging.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Logging.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/ObjectBackers.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/ObjectBackers.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Persistence.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Persistence.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Schema.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Schema.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/Serializers.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/Serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                  b64encode=False
                  ):
         self.allow_pickle=allow_pickle
         self.protocol=protocol
         self.b64encode=b64encode
 
     _primitive_types = (int, float, bool, str,
-                        np.integer, np.floating, np.bool
+                        np.integer, np.floating
                         )
     _list_types = (tuple, list)
     _dict_types = (dict, OrderedDict)
     _importable_types = (type, #types.MethodType, types.ModuleType,
                          bytes, bytearray, memoryview,
                          np.dtype
                          )
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Scaffolding/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/FittableModels.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/FittableModels.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Interpolator.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Interpolator.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/LazyTensors.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/LazyTensors.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Mesh.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Mesh.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/NeighborBasedInterpolators.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/NeighborBasedInterpolators.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/BaseSurface.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/BaseSurface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/Surface.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/Surface.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Surfaces/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/ElementaryFunctions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/TensorExpressions.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/TensorExpressions.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Symbolic/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/Derivatives.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/Derivatives.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         :param cache_evaluations: whether or not to cache function evaluations for reuse in other derivatives
         :type cache_evaluations: bool
         :param fd_opts:
         :type fd_opts:
         """
 
         # set up the coordinate parameters
-        if isinstance(center, (int, float, np.integer, np.float)):
+        if isinstance(center, (int, float, np.integer, np.floating)):
             center = [center]
         center = np.asarray(center)
 
         input_shape = f_spec.in_shape if isinstance(f_spec, FunctionSpec) else 0
         # determine if center is multiple configurations or just one
         input_dims = (0 if isinstance(input_shape, (int, np.integer)) else len(input_shape))
         multiconfig = len(center.shape) > input_dims
@@ -325,15 +325,15 @@
         :type mesh_spacing:
         :return:
         :rtype:
         """
         if mesh_spacing is None:
             mesh_spacing = self.mesh_spacing
         displacement = self.displacement_function(self._coord_index(coord)[0], mesh_spacing)
-        if isinstance(displacement, (float, np.float)):
+        if isinstance(displacement, (float, np.floating)):
             displacement = np.full(self.coord_shape, displacement)
         elif displacement.shape == self.coord_shape[-1:]:
             displacement = np.broadcast_to(displacement, self.coord_shape)
 
         return displacement
 
     def _build_displacement_array(self, coord, stencil_shapes, stencil_widths, displacement, use_sparse=False):
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FiniteDifferenceFunction.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/FunctionExpansions.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/FunctionExpansions.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'FunctionExpansion'
 ]
 
 ########################################################################################################################
 #
 #                                           Polynomial
 #
-class Polynomial:
+class TaylorPoly:
     """
     A handler for dealing with multidimensional polynomials
 
     Can be used to handle multiple polynomials simultaneously, but requires
     that all expansions are provided up to the same order.
     """
 
@@ -398,16 +398,14 @@
                         #       ordering conditions
                         base_perm = np.arange(ng)
                         shift_idx = 0
                         for p in range():
                             ...
 
 
-
-
     def shift(self, new_origin):
         """
         Uses binomial expansion to new polynomial centered at the `new_origin`
 
         :param new_origin:
         :type new_origin:
         :return:
@@ -476,15 +474,15 @@
 
 ########################################################################################################################
 #
 #                                           FunctionExpansion
 #
 class FunctionExpansionException(Exception):
     pass
-class FunctionExpansion(Polynomial):
+class FunctionExpansion(TaylorPoly):
     """
     Specifically for expanding functions
     """
 
     @classmethod
     def expand_function(cls,
                         f, point,
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/coeffuncs.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/Taylor/ZachLib/src/setup.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/Zachary/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/Zachary/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,8 +13,10 @@
 from .FittableModels import *; from .FittableModels import __all__ as exposed
 __all__ += exposed
 from .Interpolator import *; from .Interpolator import __all__ as exposed
 __all__ += exposed
 from .LazyTensors import *; from .LazyTensors import __all__ as exposed
 __all__ += exposed
 from .Symbolic import *; from .Symbolic import __all__ as exposed
+__all__ += exposed
+from .Polynomials import *; from .Polynomials import __all__ as exposed
 __all__ += exposed
```

### Comparing `mccoygroup-mcutils-0.1.0.1/McUtils/__init__.py` & `mccoygroup-mcutils-0.1.1/McUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/PKG-INFO` & `mccoygroup-mcutils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-mcutils
-Version: 0.1.0.1
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # McUtils [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mccoygroup/binder-mcutils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmccoygroup%252FMcUtils%26urlpath%3Dlab%252Ftree%252FMcUtils%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-mcutils-0.1.0.1/README.md` & `mccoygroup-mcutils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/PKG-INFO` & `mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccoygroup-mcutils
-Version: 0.1.0.1
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Mark Boyer
 Author-email: b3m2a1@uw.edu
 License: MIT
 Description: # McUtils [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mccoygroup/binder-mcutils/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Fmccoygroup%252FMcUtils%26urlpath%3Dlab%252Ftree%252FMcUtils%252Fbinder%252Findex.ipynb%26branch%3Dmaster)
```

### Comparing `mccoygroup-mcutils-0.1.0.1/mccoygroup_mcutils.egg-info/SOURCES.txt` & `mccoygroup-mcutils-0.1.1/mccoygroup_mcutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 McUtils/Scaffolding/Serializers.py
 McUtils/Scaffolding/__init__.py
 McUtils/Zachary/FittableModels.py
 McUtils/Zachary/Interpolator.py
 McUtils/Zachary/LazyTensors.py
 McUtils/Zachary/Mesh.py
 McUtils/Zachary/NeighborBasedInterpolators.py
+McUtils/Zachary/Polynomials.py
 McUtils/Zachary/__init__.py
 McUtils/Zachary/Surfaces/BaseSurface.py
 McUtils/Zachary/Surfaces/Surface.py
 McUtils/Zachary/Surfaces/__init__.py
 McUtils/Zachary/Symbolic/ElementaryFunctions.py
 McUtils/Zachary/Symbolic/TensorExpressions.py
 McUtils/Zachary/Symbolic/__init__.py
```

### Comparing `mccoygroup-mcutils-0.1.0.1/setup.py` & `mccoygroup-mcutils-0.1.1/setup.py`

 * *Files identical despite different names*

