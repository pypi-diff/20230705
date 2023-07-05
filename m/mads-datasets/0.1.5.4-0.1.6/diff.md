# Comparing `tmp/mads_datasets-0.1.5.4.tar.gz` & `tmp/mads_datasets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.5.4.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.6.tar", last modified: Wed Jul  5 12:27:32 2023, max compression
```

## Comparing `mads_datasets-0.1.5.4.tar` & `mads_datasets-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1393 2023-06-07 14:25:34.493117 mads_datasets-0.1.5.4/README.md
--rw-r--r--   0        0        0      189 2023-06-20 16:18:21.605626 mads_datasets-0.1.5.4/mads_datasets/__init__.py
--rw-r--r--   0        0        0    17460 2023-06-20 16:46:34.577959 mads_datasets-0.1.5.4/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     5708 2023-06-20 16:36:42.711266 mads_datasets-0.1.5.4/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5.4/mads_datasets/datatools.py
--rw-r--r--   0        0        0     3733 2023-06-20 16:24:56.942012 mads_datasets-0.1.5.4/mads_datasets/settings.py
--rw-r--r--   0        0        0     1051 2023-06-20 16:11:11.413974 mads_datasets-0.1.5.4/pyproject.toml
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 mads_datasets-0.1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1408 2023-06-21 07:02:25.478815 mads_datasets-0.1.6/README.md
+-rw-r--r--   0        0        0      187 2023-07-05 12:26:35.859652 mads_datasets-0.1.6/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    17872 2023-07-04 15:26:46.051334 mads_datasets-0.1.6/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     5708 2023-07-04 15:18:06.790943 mads_datasets-0.1.6/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.6/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     4003 2023-06-21 07:28:25.959229 mads_datasets-0.1.6/mads_datasets/settings.py
+-rw-r--r--   0        0        0     1111 2023-07-05 12:27:32.349985 mads_datasets-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2932 2023-06-05 11:35:08.197025 mads_datasets-0.1.6/tests/test_data.py
+-rw-r--r--   0        0        0      134 2023-06-05 13:30:33.572743 mads_datasets-0.1.6/tests/test_tokenizer.py
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 mads_datasets-0.1.6/PKG-INFO
```

### Comparing `mads_datasets-0.1.5.4/README.md` & `mads_datasets-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 # Install with poetry
 poetry add mads_datasets
 ```
 
 ## Data Types
 Currently, it supports the following datasets:
-* Sunspots Time-Series data
+* SUNSPOTS Time-Series data
 * IMDB Text data
-* Flowers Image data
-* Fashion MNIST Image data
-* Gestures Time-Series data
+* FLOWERS Image data
+* FASHION MNIST Image data
+* GESTURES Time-Series data
+* IRIS dataset
 
 ## Usage
 
 After installation, import the necessary components:
 
 ```python
 from mads_datasets import DatasetFactoryProvider, DatasetType
```

### Comparing `mads_datasets-0.1.5.4/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.6/mads_datasets/datasetfactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     WindowedDatasetSettings,
     fashionmnistsettings,
     flowersdatasetsettings,
     gesturesdatasetsettings,
     imdbdatasetsettings,
     irissettings,
     sunspotsettings,
+    penguinssettings,
 )
 
 Tensor = torch.Tensor
 
 
 class DatastreamerProtocol(Protocol):
     def stream(self) -> Iterator:
@@ -136,14 +137,17 @@
             traindataset, batchsize=batchsize, preprocessor=preprocessor
         )
         validstreamer = BaseDatastreamer(
             validdataset, batchsize=batchsize, preprocessor=preprocessor
         )
         return {"train": trainstreamer, "valid": validstreamer}
 
+class PenguinsDatasetFactory(AbstractDatasetFactory[DatasetSettings]):
+    def create_dataset(self, *args, **kwargs) -> Mapping[str, DatasetProtocol]:
+        pass
 
 class IrisDatasetFactory(AbstractDatasetFactory[PdDatasetSettings]):
     def create_dataset(
         self, *args: Any, **kwargs: Any
     ) -> Mapping[str, DatasetProtocol]:
         try:
             import pandas as pd
@@ -460,14 +464,18 @@
             return SunspotsDatasetFactory(
                 sunspotsettings, preprocessor=preprocessor, datadir=datadir
             )
         if dataset_type == DatasetType.IRIS:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
             return IrisDatasetFactory(irissettings, preprocessor=preprocessor, datadir=datadir)
 
+        if dataset_type == DatasetType.PENGUINS:
+            preprocessor = kwargs.get("preprocessor", BasePreprocessor)
+            return PenguinsDatasetFactory(penguinssettings, preprocessor=preprocessor, datadir=datadir)
+
         raise ValueError(f"Invalid dataset type: {dataset_type}")
 
 
 class BaseDatastreamer:
     """This datastreamer wil never stop
     The dataset should have a:
         __len__ method
```

### Comparing `mads_datasets-0.1.5.4/mads_datasets/datasets.py` & `mads_datasets-0.1.6/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.4/mads_datasets/datatools.py` & `mads_datasets-0.1.6/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.4/mads_datasets/settings.py` & `mads_datasets-0.1.6/mads_datasets/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     TXT = ".txt"
     ZIP = ".zip"
     TGZ = ".tgz"
     TAR = ".tar.gz"
     GZ = ".gz"
     PT = ".pt"
     CSV = ".csv"
+    PARQ = ".parq"
 
 
 class ReportTypes(Enum):
     GIN = 1
     TENSORBOARD = 2
     MLFLOW = 3
     RAY = 4
@@ -29,29 +30,30 @@
 class DatasetType(Enum):
     FLOWERS = 1
     IMDB = 2
     GESTURES = 3
     FASHION = 4
     SUNSPOTS = 5
     IRIS = 6
+    PENGUINS = 7
 
 
 class BaseSettings(BaseModel):
     def __str__(self) -> str:
         return "\n".join(f"{k}: {v}" for k, v in self.__dict__.items())
 
     def __repr__(self) -> str:
         return "\n".join(f"{k}: {v}" for k, v in self.__dict__.items())
 
 
 class DatasetSettings(BaseSettings):
     dataset_url: HttpUrl
     filename: Path
     name: str
-    formats: List[FileTypes]
+    formats: Optional[List[FileTypes]] = None
     digest: Optional[str] = None
 
 
 class ImgDatasetSettings(DatasetSettings):
     trainfrac: float
     img_size: Tuple[int, int]
 
@@ -67,22 +69,27 @@
     window_size: int
 
 
 class PdDatasetSettings(DatasetSettings):
     target: str
     features: List[str]
 
+penguinssettings = DatasetSettings(
+    dataset_url=cast(HttpUrl, "https://github.com/raoulg/juliaintro/raw/main/data/palmerpenguins.parq"),
+    filename=Path("penguins.parq"),
+    name="penguins",
+    digest="675e2a75750d0e076df810893e675476"
+)
 
 irissettings = PdDatasetSettings(
     dataset_url=cast(
         HttpUrl, "https://github.com/raoulg/data_assets/raw/main/iris_dirty.csv"
     ),
     filename=Path("iris.csv"),
     name="iris",
-    formats=[FileTypes.CSV],
     target="class",
     features=["sepal_length", "sepal_width", "petal_length", "petal_width"],
     digest="3679279dc61f6fdd859be9888db27f75",
 )
 
 sunspotsettings = WindowedDatasetSettings(
     dataset_url=cast(HttpUrl, "https://www.sidc.be/SILSO/DATA/SN_m_tot_V2.0.txt"),
```

### Comparing `mads_datasets-0.1.5.4/PKG-INFO` & `mads_datasets-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.5.4
+Version: 0.1.6
 Summary: Datasets for the master applied data science
+Author-Email: Raoul Grouls <Raoul.Grouls@han.nl>
 License: MIT
-Author: Raoul Grouls
-Author-email: Raoul.Grouls@han.nl
-Requires-Python: >=3.9.16,<4.0.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Project-URL: Github, https://github.com/raoulg/mads_datasets
+Requires-Python: >=3.8
+Requires-Dist: torch>=2.0.1
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: pydantic>=1.10.8
+Requires-Dist: pillow>=9.5.0
+Requires-Dist: torchtext>=0.15.2
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: pandas>=2.0.2; extra == "pandas"
 Provides-Extra: pandas
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0) ; extra == "pandas"
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: torchtext (>=0.15.2,<0.16.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Project-URL: GitHub, https://github.com/raoulg/mads_datasets
 Description-Content-Type: text/markdown
 
 # MADS Datasets Library
 
 This library provides the functionality to download, process, and stream several datasets.
 
 ## Installation
@@ -36,19 +32,20 @@
 
 # Install with poetry
 poetry add mads_datasets
 ```
 
 ## Data Types
 Currently, it supports the following datasets:
-* Sunspots Time-Series data
+* SUNSPOTS Time-Series data
 * IMDB Text data
-* Flowers Image data
-* Fashion MNIST Image data
-* Gestures Time-Series data
+* FLOWERS Image data
+* FASHION MNIST Image data
+* GESTURES Time-Series data
+* IRIS dataset
 
 ## Usage
 
 After installation, import the necessary components:
 
 ```python
 from mads_datasets import DatasetFactoryProvider, DatasetType
@@ -79,8 +76,7 @@
 ```
 
 Or download the data:
 
 ```python
 fashion_factory.download_data()
 ```
-
```

