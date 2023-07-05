# Comparing `tmp/imagekitio-3.0.2.tar.gz` & `tmp/imagekitio-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imagekitio-3.0.2.tar", last modified: Fri Jun 23 09:10:15 2023, max compression
+gzip compressed data, was "imagekitio-3.1.0.tar", last modified: Wed Jul  5 10:51:18 2023, max compression
```

## Comparing `imagekitio-3.0.2.tar` & `imagekitio-3.1.0.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    57798 2023-06-23 09:10:15.000000 imagekitio-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    46936 2023-06-23 09:09:41.000000 imagekitio-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10958 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio/constants/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/constants/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/constants/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/constants/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/constants/supported_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/constants/url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/BadRequestException.py
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/ConflictException.py
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/ForbiddenException.py
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/InternalServerException.py
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/NotFoundException.py
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/PartialSuccessException.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/TooManyRequestsException.py
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/UnauthorizedException.py
--rw-r--r--   0 runner    (1001) docker     (122)      367 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/UnknownException.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    37166 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/file.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio/models/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/CopyFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/CopyFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/CreateFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/CustomMetaDataTypeEnum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/CustomMetadataFieldsSchema.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/DeleteFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      814 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/ListAndSearchFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/MoveFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/MoveFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/RenameFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1420 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/UpdateFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/UploadFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio/models/results/
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/AITags.py
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/BulkDeleteFileResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/CustomMetadataFieldsResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/CustomMetadataSchema.py
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/EmbeddedMetadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/FileResult.py
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/FileResultWithResponseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/FolderResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/GetBulkJobStatusResult.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/GetMetadataResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/ListCustomMetadataFieldsResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/ListFileResult.py
--rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/MetadataExif.py
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/MetadataExifExif.py
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/MetadataExifGPS.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/MetadataExifImage.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/MetadataExifInteroperability.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/MetadataExifThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/PurgeCacheResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/PurgeCacheStatusResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/RenameFileResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/ResponseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/ResponseMetadataResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/TagsResult.py
--rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/UploadFileResult.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/VersionInfo.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/models/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     8325 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/utils/calculation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4336 2023-06-23 09:09:41.000000 imagekitio-3.0.2/imagekitio/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    57798 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3484 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-23 09:10:15.000000 imagekitio-3.0.2/imagekitio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-23 09:10:15.000000 imagekitio-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      734 2023-06-23 09:09:41.000000 imagekitio-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:10:15.000000 imagekitio-3.0.2/tests/dummy_data/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/dummy_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/dummy_data/file.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/dummy_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    32586 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_custom_metadata_fields_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)   540419 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_files_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    20838 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_folder_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    17628 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_generate_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    12294 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_tags_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_utils_calculation.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_utils_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3426 2023-06-23 09:09:41.000000 imagekitio-3.0.2/tests/test_utils_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.511790 imagekitio-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-07-05 10:50:50.000000 imagekitio-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    47332 2023-07-05 10:51:18.511790 imagekitio-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    46936 2023-07-05 10:50:50.000000 imagekitio-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.503789 imagekitio-3.1.0/imagekitio/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10958 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.507789 imagekitio-3.1.0/imagekitio/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/constants/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/constants/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/constants/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/constants/supported_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/constants/url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.507789 imagekitio-3.1.0/imagekitio/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/BadRequestException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/ConflictException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/ForbiddenException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/InternalServerException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/NotFoundException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/PartialSuccessException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/TooManyRequestsException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/UnauthorizedException.py
+-rw-r--r--   0 runner    (1001) docker     (122)      367 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/UnknownException.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37166 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/file.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.507789 imagekitio-3.1.0/imagekitio/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/CopyFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/CopyFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/CreateFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/CustomMetaDataTypeEnum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/CustomMetadataFieldsSchema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/DeleteFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/ListAndSearchFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/MoveFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/MoveFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/RenameFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1420 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/UpdateFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/UploadFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.511790 imagekitio-3.1.0/imagekitio/models/results/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/AITags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/BulkDeleteFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/CustomMetadataFieldsResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/CustomMetadataSchema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/EmbeddedMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2010 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/FileResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/FileResultWithResponseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/FolderResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/GetBulkJobStatusResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/GetMetadataResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/ListCustomMetadataFieldsResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/ListFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3401 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/MetadataExif.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/MetadataExifExif.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/MetadataExifGPS.py
+-rw-r--r--   0 runner    (1001) docker     (122)      916 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/MetadataExifImage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/MetadataExifInteroperability.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/MetadataExifThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/PurgeCacheResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/PurgeCacheStatusResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/RenameFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/ResponseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/ResponseMetadataResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/TagsResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/UploadFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/VersionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/models/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8325 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.511790 imagekitio-3.1.0/imagekitio/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/utils/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4137 2023-07-05 10:50:50.000000 imagekitio-3.1.0/imagekitio/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.503789 imagekitio-3.1.0/imagekitio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    47332 2023-07-05 10:51:18.000000 imagekitio-3.1.0/imagekitio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3521 2023-07-05 10:51:18.000000 imagekitio-3.1.0/imagekitio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 10:51:18.000000 imagekitio-3.1.0/imagekitio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-05 10:51:18.000000 imagekitio-3.1.0/imagekitio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-05 10:51:18.000000 imagekitio-3.1.0/imagekitio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 10:51:18.511790 imagekitio-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-05 10:50:50.000000 imagekitio-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.511790 imagekitio-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:51:18.511790 imagekitio-3.1.0/tests/dummy_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/dummy_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/dummy_data/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/dummy_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35697 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_custom_metadata_fields_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)   550047 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_files_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20838 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_folder_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17628 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_generate_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11201 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_models_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12294 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_tags_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_utils_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_utils_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3426 2023-07-05 10:50:50.000000 imagekitio-3.1.0/tests/test_utils_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imagekitio-3.0.2/PKG-INFO` & `imagekitio-3.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,1318 +1,1317 @@
 Metadata-Version: 2.1
 Name: imagekitio
-Version: 3.0.2
+Version: 3.1.0
 Summary: Python wrapper for the ImageKit API
 Home-page: https://github.com/imagekit-developer/imagekit-python
-License: UNKNOWN
-Description: [<img width="250" alt="ImageKit.io" src="https://raw.githubusercontent.com/imagekit-developer/imagekit-javascript/master/assets/imagekit-light-logo.svg"/>](https://imagekit.io)
-        
-        # ImageKit.io Python SDK
-        
-        [![Python CI](https://github.com/imagekit-developer/imagekit-python/workflows/Python%20CI/badge.svg)](https://github.com/imagekit-developer/imagekit-python/)
-        [![imagekitio](https://img.shields.io/pypi/v/imagekitio.svg)](https://pypi.org/project/imagekitio)
-        [![codecov](https://codecov.io/gh/imagekit-developer/imagekit-python/branch/master/graph/badge.svg?token=CwKWqBIlCu)](https://codecov.io/gh/imagekit-developer/imagekit-python)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![Twitter Follow](https://img.shields.io/twitter/follow/imagekitio?label=Follow&style=social)](https://twitter.com/ImagekitIo)
-        
-        Python SDK for [ImageKit](https://imagekit.io/) implements the new APIs and interface for different file operations.
-        
-        ImageKit is complete media storage, optimization, and transformation solution that comes with an [image and video CDN](https://imagekit.io/features/imagekit-infrastructure). It can be integrated with your existing infrastructure - storage like AWS S3, web servers, your CDN, and custom domain names, allowing you to deliver optimized images in minutes with minimal code changes.
-        
-        Supported Python Versions: >=3.6
-        
-        Table of contents -
-        
-        -   [Installation](#installation)
-        -   [Initialization](#initialization)
-        -   [Change Log](#change-log)
-        -   [Usage](#usage)
-            -   [URL Generation](#url-generation)
-            -   [File Upload](#file-upload)
-            -   [File Management](#file-management)
-            -   [Utility Functions](#utility-functions)
-        -   [Handling errors](#handling-errors)
-        -   [Development](#development)
-            -   [Tests](#tests)
-            -   [Sample](#sample)
-        -   [Support](#support)
-        -   [Links](#links)
-        
-        ## Installation
-        
-        Go to your terminal and type the following command.
-        
-        ```bash
-        pip install imagekitio
-        ```
-        
-        ## Initialization
-        
-        ```python
-        from imagekitio import ImageKit
-        
-        imagekit = ImageKit(
-            private_key='your_private_key',
-            public_key='your_public_key',
-            url_endpoint='your_url_endpoint'
-        )
-        ```
-        
-        ## Change log
-        
-        This document presents a list of changes that break the existing functionality of previous versions. We try to minimize these disruptions, but they are sometimes unavoidable, especially in significant updates. Therefore, versions are marked semantically and tagged as major upgrades whenever such breaking changes occur.
-        
-        ### Breaking History:
-        
-        Changes from `2.2.8 -> 3.0.0` are listed below
-        
-        1. Throw an Error:
-        
-        **What changed**
-        
-        -   Before the upgrade, an `error` dict was coming in the return object of any function call. Now, SDK throws an exception in case of an error.
-        
-        **Who is affected?**
-        
-        -   This affects any development in your software that calls APIs from ImageKit IO and handles errors based on what's returned.
-        
-        **How should I update my code?**
-        
-        -   To avoid failures in an application, you could handle errors as [documented here](#handling-errors)
-        
-        # Usage
-        
-        You can use this Python SDK for three different kinds of methods:
-        
-        -   [URL Generation](#url-generation)
-        -   [File Upload](#file-upload)
-        -   [File Management](#file-management)
-        -   [Utility Functions](#utility-functions)
-        
-        ## URL Generation
-        
-        **1. Using Image path and endpoint (hostname)**
-        
-        This method allows you to create a URL using the relative file path where the image exists and the URL
-        endpoint(url_endpoint) you want to use to access the image. You can refer to the documentation
-        [here](https://docs.imagekit.io/integration/url-endpoints) to read more about URL endpoints
-        in ImageKit and the section about [image origins](https://docs.imagekit.io/integration/configure-origin) to understand
-        about paths with different kinds of origins.
-        
-        The file can be an image, video, or any other static file supported by ImageKit.
-        
-        ```python
-        imagekit_url = imagekit.url({
-            "path": "/default-image.jpg",
-            "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
-            "transformation": [{
-                "height": "300",
-                "width": "400",
-                "raw": "ar-4-3,q-40"
-            }],
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/endpoint/tr:h-300,w-400,ar-4-3,q-40/default-image.jpg
-        ```
-        
-        **2. Using full image URL**
-        
-        This method allows you to add transformation parameters to an absolute URL using the `src` parameter. This method should be
-        used if you have the complete image URL stored in your database.
-        
-        ```python
-        image_url = imagekit.url({
-            "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
-            "transformation": [{
-                "height": "300",
-                "width": "400",
-                "raw": "ar-4-3,q-40"
-            }]
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%2Car-4-3%2Cq-40
-        ```
-        
-        The `.url()` method accepts the following parameters.
-        
-        | Option                  | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-        | :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-        | url_endpoint            | Optional. The prepended base URL before the path of the image. If not specified, the URL Endpoint specified during SDK initialization gets used. For example, https://ik.imagekit.io/your_imagekit_id/endpoint/                                                                                                                                                                                                                                                                             |
-        | path                    | Conditional. A path at which the image exists. For example, `/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                                                                                   |
-        | src                     | Conditional. Complete URL of an image already mapped to ImageKit. For example, `https://ik.imagekit.io/your_imagekit_id/endpoint/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                |
-        | transformation          | Optional. Specify an array of objects with name and the value in key-value pair to apply transformation params in the URL. Append different steps of a [chained transformation](https://docs.imagekit.io/features/image-transformations/chained-transformations) as different objects of the array. This document includes a complete list of supported transformations in the SDK with some examples. If one uses an unspecified transformation name, it gets applied as it is in the URL. |
-        | transformation_position | Optional. The default value is `path`, which places the transformation string as a path parameter in the URL. One can also specify it as a query, which adds the transformation string as the query parameter `tr` in the URL. Suppose one uses the `src` parameter to create the URL. In that case, the transformation string is always a query parameter.                                                                                                                                 |
-        | query_parameters        | Optional. These are the other query parameters that one wants to add to the final URL. These can be any query parameters and are not necessarily related to ImageKit. Especially useful if one wants to add some versioning parameter to their URLs.                                                                                                                                                                                                                                        |
-        | signed                  | Optional. Boolean. The default is `false`. If set to `true`, the SDK generates a signed image URL adding the image signature to the image URL. One can only use this if they create the URL with the `url_endpoint` and `path` parameters, not the `src` parameter.                                                                                                                                                                                                                         |
-        | expire_seconds          | Optional. Integer. Used along with the `signed` parameter to specify the time in seconds from `now` when the URL should expire. If specified, the URL contains the expiry timestamp, and the image signature is modified accordingly.                                                                                                                                                                                                                                                       |
-        
-        ## Examples of generating URLs
-        
-        **1. Chained Transformations as a query parameter**
-        
-        ```python
-        image_url = imagekit.url({
-            "path": "/default-image.jpg",
-            "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
-            "transformation": [
-                {
-                    "height": "300",
-                    "width": "400"
-                },
-                {
-                    "rotation": 90
-                }
-            ],
-            "transformation_position": "query"
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%3Art-90
-        ```
-        
-        **2. Sharpening, contrast transform and progressive JPG image**
-        
-        Add transformations like [Sharpening](https://docs.imagekit.io/features/image-transformations/image-enhancement-and-color-manipulation) to the URL with or without any other value. To use such transforms without specifying a value, set it as "-" in the transformation object. Otherwise, use the value that one wants to add to this transformation.
-        
-        ```python
-        image_url = imagekit.url({
-            "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
-            "transformation": [{
-                "format": "jpg",
-                "progressive": "true",
-                "effect_sharpen": "-",
-                "effect_contrast": "1"
-            }]
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        # Note that because the `src` parameter is in effect, the transformation string gets added as a query parameter `tr`
-        
-        https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=f-jpg%2Cpr-true%2Ce-sharpen%2Ce-contrast-1
-        ```
-        
-        **3. Signed URL that expires in 300 seconds with the default URL endpoint and other query parameters**
-        
-        ```python
-        image_url = imagekit.url({
-            "path": "/default-image.jpg",
-            "query_parameters": {
-                "p1": "123",
-                "p2": "345"
-            },
-            "transformation": [{
-                "height": "300",
-                "width": "400"
-            }],
-            "signed": True,
-            "expire_seconds": 300
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/tr:h-300,w-400/default-image.jpg?p1=123&p2=345&ik-t=1658899345&ik-s=8f03aca28432d4e87f697a48143efb4497bbed9e
-        ```
-        
-        **List of transformations**
-        
-        The complete list of transformations supported and their usage in ImageKit is available [here](https://docs.imagekit.io/features/image-transformations/resize-crop-and-other-transformations).
-        The SDK gives a name to each transformation parameter, making the code simpler, more straightforward, and readable. If a transformation is supported in ImageKit, though it cannot be found in the table below, then use the transformation code from ImageKit docs as the name when using the `URL` function.
-        
-        If you want to generate transformations in your application and add them to the URL as it is, use the raw parameter.
-        
-        | Supported Transformation Name | Translates to parameter         |
-        | ----------------------------- | ------------------------------- |
-        | height                        | h                               |
-        | width                         | w                               |
-        | aspect_ratio                  | ar                              |
-        | quality                       | q                               |
-        | crop                          | c                               |
-        | crop_mode                     | cm                              |
-        | x                             | x                               |
-        | y                             | y                               |
-        | focus                         | fo                              |
-        | format                        | f                               |
-        | radius                        | r                               |
-        | background                    | bg                              |
-        | border                        | b                               |
-        | rotation                      | rt                              |
-        | blur                          | bl                              |
-        | named                         | n                               |
-        | overlay_x                     | ox                              |
-        | overlay_y                     | oy                              |
-        | overlay_focus                 | ofo                             |
-        | overlay_height                | oh                              |
-        | overlay_width                 | ow                              |
-        | overlay_image                 | oi                              |
-        | overlay_image_trim            | oit                             |
-        | overlay_image_aspect_ratio    | oiar                            |
-        | overlay_image_background      | oibg                            |
-        | overlay_image_border          | oib                             |
-        | overlay_image_dpr             | oidpr                           |
-        | overlay_image_quality         | oiq                             |
-        | overlay_image_cropping        | oic                             |
-        | overlay_image_focus           | oifo                            |
-        | overlay_text                  | ot                              |
-        | overlay_text_font_size        | ots                             |
-        | overlay_text_font_family      | otf                             |
-        | overlay_text_color            | otc                             |
-        | overlay_text_transparency     | oa                              |
-        | overlay_alpha                 | oa                              |
-        | overlay_text_typography       | ott                             |
-        | overlay_background            | obg                             |
-        | overlay_text_encoded          | ote                             |
-        | overlay_text_width            | otw                             |
-        | overlay_text_background       | otbg                            |
-        | overlay_text_padding          | otp                             |
-        | overlay_text_inner_alignment  | otia                            |
-        | overlay_radius                | or                              |
-        | progressive                   | pr                              |
-        | lossless                      | lo                              |
-        | trim                          | t                               |
-        | metadata                      | md                              |
-        | color_profile                 | cp                              |
-        | default_image                 | di                              |
-        | dpr                           | dpr                             |
-        | effect_sharpen                | e-sharpen                       |
-        | effect_usm                    | e-usm                           |
-        | effect_contrast               | e-contrast                      |
-        | effect_gray                   | e-grayscale                     |
-        | original                      | orig                            |
-        | raw                           | replaced by the parameter value |
-        
-        ## File Upload
-        
-        The SDK provides a simple interface using the `.upload_file()` method to upload files to the ImageKit Media library. It
-        accepts all the parameters supported by
-        the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload).
-        
-        The `upload_file()` method requires at least the `file` as (URL/Base64/Binary) and the `file_name` parameter to upload a
-        file. The method returns a dict data in case of success, or it will throw a custom exception in case of failure.
-        Use the `options` parameter to pass other parameters supported by
-        the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload). Use the same
-        parameter name as specified in the upload API documentation.
-        
-        Simple usage
-        
-        ```python
-        from imagekitio.models.UploadFileRequestOptions import UploadFileRequestOptions
-        
-        extensions = [
-            {
-                'name': 'remove-bg',
-                'options': {
-                    'add_shadow': True,
-                    'bg_color': 'pink'
-                }
-            },
-            {
-                'name': 'google-auto-tagging',
-                'minConfidence': 80,
-                'maxTags': 10
-            }
-        ]
-        
-        options = UploadFileRequestOptions(
-            use_unique_file_name=False,
-            tags=['abc', 'def'],
-            folder='/testing-python-folder/',
-            is_private_file=False,
-            custom_coordinates='10,10,20,20',
-            response_fields=['tags', 'custom_coordinates', 'is_private_file',
-                             'embedded_metadata', 'custom_metadata'],
-            extensions=extensions,
-            webhook_url='https://webhook.site/c78d617f-33bc-40d9-9e61-608999721e2e',
-            overwrite_file=True,
-            overwrite_ai_tags=False,
-            overwrite_tags=False,
-            overwrite_custom_metadata=True,
-            custom_metadata={'testss': 12},
-        )
-        
-        result = imagekit.upload_file(file='<url|base_64|binary>', # required
-                                      file_name='my_file_name.jpg', # required
-                                      options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that uploaded file's ID
-        print(result.file_id)
-        ```
-        
-        If the upload succeeds, the `result` will be the `UploadFileResult` class.
-        
-        If the upload fails, the custom exception will be thrown with:
-        
-        -   `response_help` for any kind of help
-        -   `response_metadata` with `raw`, `http_status_code` and `headers`
-        -   `message` can be called to get the error message received from ImageKit's servers.
-        
-        ## File Management
-        
-        The SDK provides a simple interface for all
-        the [media APIs mentioned here](https://docs.imagekit.io/api-reference/media-api)
-        to manage your files. This also returns `result`.
-        
-        **1. List & Search Files**
-        
-        Accepts an object specifying the parameters used to list and search files. All parameters specified
-        in
-        the [documentation here](https://docs.imagekit.io/api-reference/media-api/list-and-search-files#list-and-search-file-api)
-        can be passed with the correct values to get the results.
-        
-        ```Python
-        from imagekitio.models.ListAndSearchFileRequestOptions import ListAndSearchFileRequestOptions
-        
-        options = ListAndSearchFileRequestOptions(
-            type='file',
-            sort='ASC_CREATED',
-            path='/',
-            search_query="created_at >= '2d' OR size < '2mb' OR format='png'",
-            file_type='all',
-            limit=5,
-            skip=0,
-            tags='Software, Developer, Engineer',
-        )
-        
-        result = imagekit.list_files(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the first file's ID
-        print(result.list[0].file_id)
-        ```
-        
-        **2. Get File Details**
-        
-        Accepts the file ID and fetches the details as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-details)
-        
-        ```python
-        file_id = "your_file_id"
-        result = imagekit.get_file_details(file_id=file_id)  # file_id required
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        ```
-        
-        **3. Get File Versions**
-        
-        Accepts the file ID and fetches the details as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-versions)
-        
-        ```python
-        file_id = "your_file_id"
-        result = imagekit.get_file_versions(file_id=file_id)  # file_id required
-        
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's version id
-        print(result.list[0].version_info.id)
-        ```
-        
-        **4. Get File Version details**
-        
-        Accepts the `file_id` and `version_id` and fetches the details as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-version-details)
-        
-        ```python
-        result = imagekit.get_file_version_details(
-            file_id='file_id',
-            version_id='version_id'
-        )
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        
-        # print that file's version id
-        print(result.version_info.id)
-        ```
-        
-        **5. Update File Details**
-        
-        Accepts all the parameters as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/update-file-details).
-        The first argument to the `update_file_details()` method is the file ID, and a second argument is an object with the
-        parameters to be
-        updated.
-        
-        ```python
-        from imagekitio.models.UpdateFileRequestOptions import UpdateFileRequestOptions
-        
-        extensions = [
-            {
-                'name': 'remove-bg',
-                'options': {
-                    'add_shadow': True,
-                    'bg_color': 'red'
-                }
-            },
-            {
-                'name': 'google-auto-tagging',
-                'minConfidence': 80,
-                'maxTags': 10
-            }
-        ]
-        
-        options = UpdateFileRequestOptions(
-            remove_ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'],
-            webhook_url='url',
-            extensions=extensions,
-            tags=['tag-1', 'tag-2'],
-            custom_coordinates='10,10,100,100',
-            custom_metadata={'test': 11},
-        )
-        
-        result = imagekit.update_file_details(file_id='62cfd39819ca454d82a07182'
-                , options=options)  # required
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        ```
-        
-        **6. Add tags**
-        
-        Accepts a list of `file_ids` and `tags` as a parameter to be used to add tags. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/add-tags-bulk) can be passed to
-        the `.add_tags()` functions to get the results.
-        
-        ```python
-        result = imagekit.add_tags(file_ids=['file-id-1', 'file-id-2'], tags=['add-tag-1', 'add-tag-2'])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully updated file ids
-        print(result.successfully_updated_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_updated_file_ids[0])
-        ```
-        
-        **7. Remove tags**
-        
-        Accepts a list of `file_ids` and `tags` as a parameter to be used to remove tags. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-tags-bulk) can be passed to
-        the `.remove_tags()` functions to get the results.
-        
-        ```python
-        result = imagekit.remove_tags(file_ids=['file-id-1', 'file-id-2'], tags=['remove-tag-1', 'remove-tag-2'])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully updated file ids
-        print(result.successfully_updated_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_updated_file_ids[0])
-        ```
-        
-        **8. Remove AI tags**
-        
-        Accepts a list of `file_ids` and `ai_tags` as a parameter to remove AI tags. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-aitags-bulk) can be passed to
-        the `.remove_ai_tags()` functions to get the results.
-        
-        ```python
-        result = imagekit.remove_ai_tags(file_ids=['file-id-1', 'file-id-2'], ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully updated file ids
-        print(result.successfully_updated_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_updated_file_ids[0])
-        ```
-        
-        **9. Delete File**
-        
-        Delete a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file). It accepts the file ID of the File that has to be
-        deleted.
-        
-        ```python
-        file_id = "file_id"
-        result = imagekit.delete_file(file_id=file_id)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **10. Delete FileVersion**
-        
-        Delete a file version as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file-version).
-        The method accepts the `file_id` and particular version id of the file that has to be deleted.
-        
-        ```python
-        result = imagekit.delete_file_version(file_id="file_id", version_id="version_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **11. Bulk File Delete by IDs**
-        
-        Delete a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-files-bulk).
-        The method accepts a list of file IDs that have to be deleted.
-        
-        ```python
-        result = imagekit.bulk_file_delete(file_ids=["file_id1", "file_id2"])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully deleted file ids
-        print(result.successfully_deleted_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_deleted_file_ids[0])
-        ```
-        
-        **12. Copy file**
-        
-        Copy a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-file).
-        The method accepts `source_file_path`, `destination_path`, and `include_file_versions` of the file that has to be copied.
-        
-        ```python
-        from imagekitio.models.CopyFileRequestOptions import CopyFileRequestOptions
-        
-        options = \
-            CopyFileRequestOptions(source_file_path='/source_file_path.jpg',
-                                   destination_path='/destination_path',
-                                   include_file_versions=True)
-        result = imagekit.copy_file(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **13. Move File**
-        
-        Move a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-file).
-        The method accepts `source_file_path` and `destination_path` of the file that has to be moved.
-        
-        ```python
-        from imagekitio.models.MoveFileRequestOptions import MoveFileRequestOptions
-        
-        options = \
-            MoveFileRequestOptions(source_file_path='/source_file_path.jpg',
-                                   destination_path='/destination_path')
-        result = imagekit.move_file(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **14. Rename File**
-        
-        Rename a file per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/rename-file).
-        The method accepts the `file_path`, `new_file_name`, and `purge_cache` boolean that has to be renamed.
-        
-        ```python
-        from imagekitio.models.RenameFileRequestOptions import RenameFileRequestOptions
-        
-        options = RenameFileRequestOptions(file_path='/file_path.jpg',
-                                           new_file_name='new_file_name.jpg',
-                                           purge_cache=True)
-        result = imagekit.rename_file(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the purge request id
-        print(result.purge_request_id)
-        ```
-        
-        **15. Restore file Version**
-        
-        Restore a file as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/restore-file-version).
-        The method accepts the `file_id` and `version_id` of the file that has to be restored.
-        
-        ```python
-        result = imagekit.restore_file_version(file_id="file_id", version_id="version_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        ```
-        
-        **16. Create Folder**
-        
-        Create a folder per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/create-folder).
-        The method accepts `folder_name` and `parent_folder_path` as options that must be created.
-        
-        ```Python
-        from imagekitio.models.CreateFolderRequestOptions import CreateFolderRequestOptions
-        
-        options = CreateFolderRequestOptions(folder_name='test',
-                                             parent_folder_path='/')
-        result = imagekit.create_folder(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **17. Delete Folder**
-        
-        Delete a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-folder).
-        The method accepts `folder_path` as an option that must be deleted.
-        
-        ```python
-        from imagekitio.models.DeleteFolderRequestOptions import DeleteFolderRequestOptions
-        
-        options = DeleteFolderRequestOptions(folder_path='/test/demo')
-        result = imagekit.delete_folder(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **18. Copy Folder**
-        
-        Copy a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-folder).
-        The method accepts the `source_folder_path`, `destination_path`, and `include_file_versions` boolean as options that
-        have to be copied.
-        
-        ```python
-        from imagekitio.models.CopyFolderRequestOptions import CopyFolderRequestOptions
-        options = \
-            CopyFolderRequestOptions(source_folder_path='/source_folder_path',
-                                     destination_path='/destination/path',
-                                     include_file_versions=True)
-        result = imagekit.copy_folder(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the job's id
-        print(result.job_id)
-        ```
-        
-        **19. Move Folder**
-        
-        Move a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-folder).
-        The method accepts the `source_folder_path` and `destination_path` of a folder as options that must be moved.
-        
-        ```python
-        from imagekitio.models.MoveFolderRequestOptions import MoveFolderRequestOptions
-        options = \
-            MoveFolderRequestOptions(source_folder_path='/source_folder_path',
-                                     destination_path='/destination_path')
-        result = imagekit.move_folder(options=options)
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the job's id
-        print(result.job_id)
-        ```
-        
-        **20. Get Bulk Job Status**
-        
-        Accepts the `job_id` to get bulk job status as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-move-folder-status).
-        The method takes only jobId.
-        
-        ```python
-        result = imagekit.get_bulk_job_status(job_id="job_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the job's id
-        print(result.job_id)
-        
-        # print the status
-        print(result.status)
-        ```
-        
-        **21. Purge Cache**
-        
-        Programmatically issue an explicit cache request as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache).
-        Accepts the full URL of the File for which the cache has to be cleared.
-        
-        ```python
-        result = imagekit.purge_file_cache(file_url="full_url_of_file")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the purge file cache request id
-        print(result.request_id)
-        ```
-        
-        **22. Purge Cache Status**
-        
-        Get the purge cache request status using the `cache_request_id` returned when a purge cache request gets submitted as per the
-        [API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache-status)
-        
-        ```python
-        result = imagekit.get_purge_file_cache_status(purge_cache_id="cache_request_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the purge file cache status
-        print(result.status)
-        ```
-        
-        **23. Get File Metadata**
-        
-        Accepts the `file_id` and fetches the metadata as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-for-uploaded-media-files)
-        
-        ```python
-        result = imagekit.get_file_metadata(file_id="file_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the file metadata fields
-        print(result.width)
-        print(result.exif.image.x_resolution)
-        ```
-        
-        **24. Get File Metadata from remote URL**
-        
-        Accepts the `remote_file_url` and fetches the metadata as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-from-remote-url)
-        
-        ```python
-        result = imagekit.get_remote_file_url_metadata(remote_file_url="remote_file_url")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the file metadata fields
-        print(result.width)
-        print(result.exif.image.x_resolution)
-        ```
-        
-        **25. Create CustomMetaDataFields**
-        
-        Accepts an option specifying the parameters used to create custom metadata fields. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field)
-        can be passed as it is with the correct values to get the results.
-        
-        Check for the [allowed values in the schema](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field#allowed-values-in-the-schema-object).
-        
-        **Example:**
-        
-        ```python
-        # Example for the type number
-        
-        from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
-        schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Number,
-                                            min_value=100,
-                                            max_value=200)
-        options = CreateCustomMetadataFieldsRequestOptions(name='test',
-                                                           label='test',
-                                                           schema=schema)
-        result = imagekit.create_custom_metadata_fields(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the id of created custom metadata fields
-        print(result.id)
-        
-        # print the schema's type of created custom metadata fields
-        print(result.schema.type)
-        
-        ```
-        
-        ```python
-        # MultiSelect type Example
-        
-        from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
-        
-        schema = \
-            CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.MultiSelect,
-                                       is_value_required=True,
-                                       default_value=['small', 30, True],
-                                       select_options=[
-                                            'small',
-                                            'medium',
-                                            'large',
-                                            30,
-                                            40,
-                                            True,
-                                        ])
-        options = \
-            CreateCustomMetadataFieldsRequestOptions(name='test-MultiSelect',
-                label='test-MultiSelect', schema=schema)
-        result = imagekit.create_custom_metadata_fields(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the name of created custom metadata fields
-        print(result.name)
-        
-        # print the schema's select options of created custom metadata fields
-        print(result.schema.select_options)
-        
-        ```
-        
-        ```python
-        # Date type Example
-        
-        from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
-        
-        schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Date,
-                                            min_value='2022-11-29T10:11:10+00:00',
-                                            max_value='2022-11-30T10:11:10+00:00')
-        options = CreateCustomMetadataFieldsRequestOptions(name='test-date',
-                                                           label='test-date',
-                                                           schema=schema)
-        result = imagekit.create_custom_metadata_fields(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the label of created custom metadata fields
-        print(result.label)
-        
-        # print the schema's min value of created custom metadata fields
-        print(result.schema.min_value)
-        
-        ```
-        
-        **26. Get CustomMetaDataFields**
-        
-        Accepts the `include_deleted` boolean as the initial parameter and fetches the metadata as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/get-custom-metadata-field)
-        .
-        
-        ```python
-        result = imagekit.get_custom_metadata_fields()  # in this case, it will consider includeDeleted as a False
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the first customMetadataField's id
-        print(result.list[0].id)
-        
-        # print the first customMetadataField schema's type
-        print(result.list[0].schema.type)
-        ```
-        
-        ```python
-        result = imagekit.get_custom_metadata_fields(include_deleted=True)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the first customMetadataField's name
-        print(result.list[0].name)
-        
-        # print the first customMetadataField schema's default value
-        print(result.list[0].schema.default_value)
-        ```
-        
-        **27. Update CustomMetaDataFields**
-        
-        Accepts a `field_id` and options for specifying the parameters to be used to edit custom metadata fields
-        as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/update-custom-metadata-field)
-        .
-        
-        ```python
-        
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.UpdateCustomMetadataFieldsRequestOptions import UpdateCustomMetadataFieldsRequestOptions
-        
-        schema = CustomMetadataFieldsSchema(min_value=100, max_value=200)
-        options = UpdateCustomMetadataFieldsRequestOptions(
-            label='test-update',
-            schema=schema
-        )
-        result = imagekit.update_custom_metadata_fields(
-            field_id='id_of_custom_metadata_field',
-            options=options
-        )
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the label of updated custom metadata fields
-        print(result.label)
-        
-        # print the schema's min value of updated custom metadata fields
-        print(result.schema.min_value)
-        ```
-        
-        **28. Delete CustomMetaDataFields**
-        
-        Accepts the id to delete the custom metadata fields as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/delete-custom-metadata-field)
-        .
-        
-        ```python
-        result = imagekit.delete_custom_metadata_field(field_id="id_of_custom_metadata_field")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        ## Utility functions
-        
-        We have included the following commonly used utility functions in this package.
-        
-        **Authentication parameter generation**
-        
-        Suppose one wants to implement client-side file upload. In that case, one will need a token, expiry timestamp, and a valid signature for that upload. The SDK provides a simple method that one can use in their code to generate these authentication parameters.
-        
-        <em>Note: Any client-side code should never expose The Private API Key. One must always generate these authentications parameters on the server-side</em>
-        
-        authentication
-        
-        `authentication_parameters = imagekit.get_authentication_parameters(token, expire)`
-        
-        Returns
-        
-        ```python
-        {
-            "token": "unique_token",
-            "expire": "valid_expiry_timestamp",
-            "signature": "generated_signature"
-        }
-        ```
-        
-        Both the `token` and `expire` parameters are optional. If not specified, the SDK uses the UUID to generate a random token and internally generates a valid expiry timestamp. The `token` and `expire` used to generate `signature` is part of a response returned by the server.
-        
-        **Distance calculation between two `pHash` values**
-        
-        Perceptual hashing allows you to construct a has value that uniquely identifies an input image based on the contents
-        of an image. [imagekit.io metadata API](https://docs.imagekit.io/api-reference/metadata-api) returns the `pHash`
-        value of an image in the response. You can use this value
-        to [find a duplicate or similar image](https://docs.imagekit.io/api-reference/metadata-api#using-phash-to-find-similar-or-duplicate-images)
-        by calculating the distance between the two images.
-        
-        This SDK exposes the `phash_distance` function to calculate the distance between two `pHash` values. It accepts two `pHash`
-        hexadecimal
-        strings and returns a numeric value indicative of the difference between the two images.
-        
-        ```python
-        def calculate_distance():
-            # fetch metadata of two uploaded image files
-            ...
-            # extract pHash strings from both: say 'first_hash' and 'second_hash'
-            ...
-            # calculate the distance between them:
-        
-            distance = imagekit.phash_distance(first_hash, second_hash)
-            return distance
-        
-        ```
-        
-        **Distance calculation examples**
-        
-        ```Python
-        imagekit.phash_distance('f06830ca9f1e3e90', 'f06830ca9f1e3e90')
-        # output: 0 (same image)
-        
-        imagekit.phash_distance('2d5ad3936d2e015b', '2d6ed293db36a4fb')
-        # output: 17 (similar images)
-        
-        imagekit.phash_distance('a4a65595ac94518b', '7838873e791f8400')
-        # output: 37 (dissimilar images)
-        ```
-        
-        **HTTP response metadata of Internal API**
-        
-        HTTP response metadata of the internal API call can be accessed using the \_response_metadata on the Result object.
-        Example:
-        
-        ```Python
-        result = imagekit.upload_file(
-            file="<url|base_64|binary>",
-            file_name="my_file_name.jpg",
-        )
-        
-        # Final Result
-        print(result)
-        print(result.response_metadata.raw)
-        print(result.response_metadata.http_status_code)
-        print(result.response_metadata.headers)
-        ```
-        
-        ### Sample Code Instruction
-        
-        To run `sample` code go to the code samples here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python and run.
-        
-        ```shell
-        python sample.py
-        ```
-        
-        ## Handling errors
-        
-        Catch and respond to invalid data, internal problems, and more.
-        
-        ImageKit Python SDK raises exceptions for many reasons, such as not found, invalid parameters, authentication, and
-        internal server errors. Therefore, we recommend writing code that gracefully handles all possible API exceptions.
-        
-        #### Example:
-        
-        ```Python
-        from imagekitio.exceptions.BadRequestException import BadRequestException
-        from imagekitio.exceptions.UnauthorizedException import UnauthorizedException
-        from imagekitio.exceptions.ForbiddenException import ForbiddenException
-        from imagekitio.exceptions.TooManyRequestsException import TooManyRequestsException
-        from imagekitio.exceptions.InternalServerException import InternalServerException
-        from imagekitio.exceptions.PartialSuccessException import PartialSuccessException
-        from imagekitio.exceptions.NotFoundException import NotFoundException
-        from imagekitio.exceptions.UnknownException import UnknownException
-        
-        try:
-        
-            # Use ImageKit's SDK to make requests...
-            print('Run image kit api')
-        except BadRequestException, e:
-            # Missing or Invalid parameters were supplied to Imagekit.io's API
-            print('Status is: ' + e.response_metadata.http_status_code)
-            print('Message is: ' + e.message)
-            print('Headers are: ' + e.response_metadata.headers)
-            print('Raw body is: ' + e.response_metadata.raw)
-        except UnauthorizedException, e:
-            print(e)
-        except ForbiddenException, e:
-            # No valid API key was provided.
-            print(e)
-        except TooManyRequestsException, e:
-            # Can be for the following reasons:
-            # ImageKit could not authenticate your account with the keys provided.
-            # An expired key (public or private) was used with the request.
-            # The account is disabled.
-            # If you use the upload API, the total storage limit (or upload limit) is exceeded.
-            print(e)
-        except InternalServerException, e:
-            # Too many requests made to the API too quickly
-            print(e)
-        except PartialSuccessException, e:
-            # Something went wrong with ImageKit.io API.
-            print(e)
-        except NotFoundException, e:
-            # Error cases on partial success.
-            print(e)
-        except UnknownException, e:
-            # If any of the field or parameter is not found in the data
-            print(e)
-        
-        # Something else happened, which can be unrelated to ImageKit; the reason will be indicated in the message field
-        ```
-        
-        ## Development
-        
-        ### Tests
-        
-        Tests are powered by [Tox](https://tox.wiki/en/latest/).
-        
-        ```bash
-        $ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
-        $ pip install tox
-        $ tox
-        ```
-        
-        ### Sample
-        
-        #### Get & Install local ImageKit Python SDK
-        
-        ```bash
-        $ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
-        $ pip install -e .
-        ```
-        
-        #### Get samples
-        
-        To integrate ImageKit Samples in the Python, the code samples covered here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python.
-        
-        Open the `python/sample.py` file and replace placeholder credentials with actual values. You can get the value of [URL-endpoint](https://imagekit.io/dashboard#url-endpoints) from your ImageKit dashboard. API keys can be obtained from the [developer](https://imagekit.io/dashboard/developer/api-keys) section in your ImageKit dashboard.
-        
-        In the `python/sample.py` file, set the following parameters for authentication:
-        
-        ```python
-        from imagekitio import ImageKit
-        imagekit = ImageKit(
-            private_key='your private_key',
-            public_key='your public_key',
-            url_endpoint = 'your url_endpoint'
-        )
-        ```
-        
-        To install dependencies that are in the `python/requirements.txt` file, can fire this command to install them:
-        
-        ```shell
-        pip install -r python/requirements.txt
-        ```
-        
-        Now run `python/sample.py`. If you are using CLI Tool (Terminal/Command prompt), open the project in CLI and execute it.
-        
-        ```shell
-        # if not installed already
-        pip install imagekitio
-        
-        # if installing local sdk
-        pip install -e <path_to_local_sdk>
-        
-        # to run sample.py file
-        python3 python/sample.py
-        ```
-        
-        ## Support
-        
-        For any feedback or to report any issues or general implementation support, please reach out
-        to [support@imagekit.io](https://github.com/imagekit-developer/imagekit-python)
-        
-        ## Links
-        
-        -   [Documentation](https://docs.imagekit.io/)
-        
-        -   [Main Website](https://imagekit.io/)
-        
-        ## License
-        
-        Released under the MIT license.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[<img width="250" alt="ImageKit.io" src="https://raw.githubusercontent.com/imagekit-developer/imagekit-javascript/master/assets/imagekit-light-logo.svg"/>](https://imagekit.io)
+
+# ImageKit.io Python SDK
+
+[![Python CI](https://github.com/imagekit-developer/imagekit-python/workflows/Python%20CI/badge.svg)](https://github.com/imagekit-developer/imagekit-python/)
+[![imagekitio](https://img.shields.io/pypi/v/imagekitio.svg)](https://pypi.org/project/imagekitio)
+[![codecov](https://codecov.io/gh/imagekit-developer/imagekit-python/branch/master/graph/badge.svg?token=CwKWqBIlCu)](https://codecov.io/gh/imagekit-developer/imagekit-python)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Twitter Follow](https://img.shields.io/twitter/follow/imagekitio?label=Follow&style=social)](https://twitter.com/ImagekitIo)
+
+Python SDK for [ImageKit](https://imagekit.io/) implements the new APIs and interface for different file operations.
+
+ImageKit is complete media storage, optimization, and transformation solution that comes with an [image and video CDN](https://imagekit.io/features/imagekit-infrastructure). It can be integrated with your existing infrastructure - storage like AWS S3, web servers, your CDN, and custom domain names, allowing you to deliver optimized images in minutes with minimal code changes.
+
+Supported Python Versions: >=3.6
+
+Table of contents -
+
+-   [Installation](#installation)
+-   [Initialization](#initialization)
+-   [Change Log](#change-log)
+-   [Usage](#usage)
+    -   [URL Generation](#url-generation)
+    -   [File Upload](#file-upload)
+    -   [File Management](#file-management)
+    -   [Utility Functions](#utility-functions)
+-   [Handling errors](#handling-errors)
+-   [Development](#development)
+    -   [Tests](#tests)
+    -   [Sample](#sample)
+-   [Support](#support)
+-   [Links](#links)
+
+## Installation
+
+Go to your terminal and type the following command.
+
+```bash
+pip install imagekitio
+```
+
+## Initialization
+
+```python
+from imagekitio import ImageKit
+
+imagekit = ImageKit(
+    private_key='your_private_key',
+    public_key='your_public_key',
+    url_endpoint='your_url_endpoint'
+)
+```
+
+## Change log
+
+This document presents a list of changes that break the existing functionality of previous versions. We try to minimize these disruptions, but they are sometimes unavoidable, especially in significant updates. Therefore, versions are marked semantically and tagged as major upgrades whenever such breaking changes occur.
+
+### Breaking History:
+
+Changes from `2.2.8 -> 3.0.0` are listed below
+
+1. Throw an Error:
+
+**What changed**
+
+-   Before the upgrade, an `error` dict was coming in the return object of any function call. Now, SDK throws an exception in case of an error.
+
+**Who is affected?**
+
+-   This affects any development in your software that calls APIs from ImageKit IO and handles errors based on what's returned.
+
+**How should I update my code?**
+
+-   To avoid failures in an application, you could handle errors as [documented here](#handling-errors)
+
+# Usage
+
+You can use this Python SDK for three different kinds of methods:
+
+-   [URL Generation](#url-generation)
+-   [File Upload](#file-upload)
+-   [File Management](#file-management)
+-   [Utility Functions](#utility-functions)
+
+## URL Generation
+
+**1. Using Image path and endpoint (hostname)**
+
+This method allows you to create a URL using the relative file path where the image exists and the URL
+endpoint(url_endpoint) you want to use to access the image. You can refer to the documentation
+[here](https://docs.imagekit.io/integration/url-endpoints) to read more about URL endpoints
+in ImageKit and the section about [image origins](https://docs.imagekit.io/integration/configure-origin) to understand
+about paths with different kinds of origins.
+
+The file can be an image, video, or any other static file supported by ImageKit.
+
+```python
+imagekit_url = imagekit.url({
+    "path": "/default-image.jpg",
+    "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
+    "transformation": [{
+        "height": "300",
+        "width": "400",
+        "raw": "ar-4-3,q-40"
+    }],
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/endpoint/tr:h-300,w-400,ar-4-3,q-40/default-image.jpg
+```
+
+**2. Using full image URL**
+
+This method allows you to add transformation parameters to an absolute URL using the `src` parameter. This method should be
+used if you have the complete image URL stored in your database.
+
+```python
+image_url = imagekit.url({
+    "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
+    "transformation": [{
+        "height": "300",
+        "width": "400",
+        "raw": "ar-4-3,q-40"
+    }]
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%2Car-4-3%2Cq-40
+```
+
+The `.url()` method accepts the following parameters.
+
+| Option                  | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| url_endpoint            | Optional. The prepended base URL before the path of the image. If not specified, the URL Endpoint specified during SDK initialization gets used. For example, https://ik.imagekit.io/your_imagekit_id/endpoint/                                                                                                                                                                                                                                                                             |
+| path                    | Conditional. A path at which the image exists. For example, `/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                                                                                   |
+| src                     | Conditional. Complete URL of an image already mapped to ImageKit. For example, `https://ik.imagekit.io/your_imagekit_id/endpoint/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                |
+| transformation          | Optional. Specify an array of objects with name and the value in key-value pair to apply transformation params in the URL. Append different steps of a [chained transformation](https://docs.imagekit.io/features/image-transformations/chained-transformations) as different objects of the array. This document includes a complete list of supported transformations in the SDK with some examples. If one uses an unspecified transformation name, it gets applied as it is in the URL. |
+| transformation_position | Optional. The default value is `path`, which places the transformation string as a path parameter in the URL. One can also specify it as a query, which adds the transformation string as the query parameter `tr` in the URL. Suppose one uses the `src` parameter to create the URL. In that case, the transformation string is always a query parameter.                                                                                                                                 |
+| query_parameters        | Optional. These are the other query parameters that one wants to add to the final URL. These can be any query parameters and are not necessarily related to ImageKit. Especially useful if one wants to add some versioning parameter to their URLs.                                                                                                                                                                                                                                        |
+| signed                  | Optional. Boolean. The default is `false`. If set to `true`, the SDK generates a signed image URL adding the image signature to the image URL. One can only use this if they create the URL with the `url_endpoint` and `path` parameters, not the `src` parameter.                                                                                                                                                                                                                         |
+| expire_seconds          | Optional. Integer. Used along with the `signed` parameter to specify the time in seconds from `now` when the URL should expire. If specified, the URL contains the expiry timestamp, and the image signature is modified accordingly.                                                                                                                                                                                                                                                       |
+
+## Examples of generating URLs
+
+**1. Chained Transformations as a query parameter**
+
+```python
+image_url = imagekit.url({
+    "path": "/default-image.jpg",
+    "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
+    "transformation": [
+        {
+            "height": "300",
+            "width": "400"
+        },
+        {
+            "rotation": 90
+        }
+    ],
+    "transformation_position": "query"
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%3Art-90
+```
+
+**2. Sharpening, contrast transform and progressive JPG image**
+
+Add transformations like [Sharpening](https://docs.imagekit.io/features/image-transformations/image-enhancement-and-color-manipulation) to the URL with or without any other value. To use such transforms without specifying a value, set it as "-" in the transformation object. Otherwise, use the value that one wants to add to this transformation.
+
+```python
+image_url = imagekit.url({
+    "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
+    "transformation": [{
+        "format": "jpg",
+        "progressive": "true",
+        "effect_sharpen": "-",
+        "effect_contrast": "1"
+    }]
+})
+```
+
+Sample Result URL -
+
+```
+# Note that because the `src` parameter is in effect, the transformation string gets added as a query parameter `tr`
+
+https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=f-jpg%2Cpr-true%2Ce-sharpen%2Ce-contrast-1
+```
+
+**3. Signed URL that expires in 300 seconds with the default URL endpoint and other query parameters**
+
+```python
+image_url = imagekit.url({
+    "path": "/default-image.jpg",
+    "query_parameters": {
+        "p1": "123",
+        "p2": "345"
+    },
+    "transformation": [{
+        "height": "300",
+        "width": "400"
+    }],
+    "signed": True,
+    "expire_seconds": 300
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/tr:h-300,w-400/default-image.jpg?p1=123&p2=345&ik-t=1658899345&ik-s=8f03aca28432d4e87f697a48143efb4497bbed9e
+```
+
+**List of transformations**
+
+The complete list of transformations supported and their usage in ImageKit is available [here](https://docs.imagekit.io/features/image-transformations/resize-crop-and-other-transformations).
+The SDK gives a name to each transformation parameter, making the code simpler, more straightforward, and readable. If a transformation is supported in ImageKit, though it cannot be found in the table below, then use the transformation code from ImageKit docs as the name when using the `URL` function.
+
+If you want to generate transformations in your application and add them to the URL as it is, use the raw parameter.
+
+| Supported Transformation Name | Translates to parameter         |
+| ----------------------------- | ------------------------------- |
+| height                        | h                               |
+| width                         | w                               |
+| aspect_ratio                  | ar                              |
+| quality                       | q                               |
+| crop                          | c                               |
+| crop_mode                     | cm                              |
+| x                             | x                               |
+| y                             | y                               |
+| focus                         | fo                              |
+| format                        | f                               |
+| radius                        | r                               |
+| background                    | bg                              |
+| border                        | b                               |
+| rotation                      | rt                              |
+| blur                          | bl                              |
+| named                         | n                               |
+| overlay_x                     | ox                              |
+| overlay_y                     | oy                              |
+| overlay_focus                 | ofo                             |
+| overlay_height                | oh                              |
+| overlay_width                 | ow                              |
+| overlay_image                 | oi                              |
+| overlay_image_trim            | oit                             |
+| overlay_image_aspect_ratio    | oiar                            |
+| overlay_image_background      | oibg                            |
+| overlay_image_border          | oib                             |
+| overlay_image_dpr             | oidpr                           |
+| overlay_image_quality         | oiq                             |
+| overlay_image_cropping        | oic                             |
+| overlay_image_focus           | oifo                            |
+| overlay_text                  | ot                              |
+| overlay_text_font_size        | ots                             |
+| overlay_text_font_family      | otf                             |
+| overlay_text_color            | otc                             |
+| overlay_text_transparency     | oa                              |
+| overlay_alpha                 | oa                              |
+| overlay_text_typography       | ott                             |
+| overlay_background            | obg                             |
+| overlay_text_encoded          | ote                             |
+| overlay_text_width            | otw                             |
+| overlay_text_background       | otbg                            |
+| overlay_text_padding          | otp                             |
+| overlay_text_inner_alignment  | otia                            |
+| overlay_radius                | or                              |
+| progressive                   | pr                              |
+| lossless                      | lo                              |
+| trim                          | t                               |
+| metadata                      | md                              |
+| color_profile                 | cp                              |
+| default_image                 | di                              |
+| dpr                           | dpr                             |
+| effect_sharpen                | e-sharpen                       |
+| effect_usm                    | e-usm                           |
+| effect_contrast               | e-contrast                      |
+| effect_gray                   | e-grayscale                     |
+| original                      | orig                            |
+| raw                           | replaced by the parameter value |
+
+## File Upload
+
+The SDK provides a simple interface using the `.upload_file()` method to upload files to the ImageKit Media library. It
+accepts all the parameters supported by
+the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload).
+
+The `upload_file()` method requires at least the `file` as (URL/Base64/Binary) and the `file_name` parameter to upload a
+file. The method returns a dict data in case of success, or it will throw a custom exception in case of failure.
+Use the `options` parameter to pass other parameters supported by
+the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload). Use the same
+parameter name as specified in the upload API documentation.
+
+Simple usage
+
+```python
+from imagekitio.models.UploadFileRequestOptions import UploadFileRequestOptions
+
+extensions = [
+    {
+        'name': 'remove-bg',
+        'options': {
+            'add_shadow': True,
+            'bg_color': 'pink'
+        }
+    },
+    {
+        'name': 'google-auto-tagging',
+        'minConfidence': 80,
+        'maxTags': 10
+    }
+]
+
+options = UploadFileRequestOptions(
+    use_unique_file_name=False,
+    tags=['abc', 'def'],
+    folder='/testing-python-folder/',
+    is_private_file=False,
+    custom_coordinates='10,10,20,20',
+    response_fields=['tags', 'custom_coordinates', 'is_private_file',
+                     'embedded_metadata', 'custom_metadata'],
+    extensions=extensions,
+    webhook_url='https://webhook.site/c78d617f-33bc-40d9-9e61-608999721e2e',
+    overwrite_file=True,
+    overwrite_ai_tags=False,
+    overwrite_tags=False,
+    overwrite_custom_metadata=True,
+    custom_metadata={'testss': 12},
+)
+
+result = imagekit.upload_file(file='<url|base_64|binary>', # required
+                              file_name='my_file_name.jpg', # required
+                              options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that uploaded file's ID
+print(result.file_id)
+```
+
+If the upload succeeds, the `result` will be the `UploadFileResult` class.
+
+If the upload fails, the custom exception will be thrown with:
+
+-   `response_help` for any kind of help
+-   `response_metadata` with `raw`, `http_status_code` and `headers`
+-   `message` can be called to get the error message received from ImageKit's servers.
+
+## File Management
+
+The SDK provides a simple interface for all
+the [media APIs mentioned here](https://docs.imagekit.io/api-reference/media-api)
+to manage your files. This also returns `result`.
+
+**1. List & Search Files**
+
+Accepts an object specifying the parameters used to list and search files. All parameters specified
+in
+the [documentation here](https://docs.imagekit.io/api-reference/media-api/list-and-search-files#list-and-search-file-api)
+can be passed with the correct values to get the results.
+
+```Python
+from imagekitio.models.ListAndSearchFileRequestOptions import ListAndSearchFileRequestOptions
+
+options = ListAndSearchFileRequestOptions(
+    type='file',
+    sort='ASC_CREATED',
+    path='/',
+    search_query="created_at >= '2d' OR size < '2mb' OR format='png'",
+    file_type='all',
+    limit=5,
+    skip=0,
+    tags='Software, Developer, Engineer',
+)
+
+result = imagekit.list_files(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the first file's ID
+print(result.list[0].file_id)
+```
+
+**2. Get File Details**
+
+Accepts the file ID and fetches the details as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-details)
+
+```python
+file_id = "your_file_id"
+result = imagekit.get_file_details(file_id=file_id)  # file_id required
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+```
+
+**3. Get File Versions**
+
+Accepts the file ID and fetches the details as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-versions)
+
+```python
+file_id = "your_file_id"
+result = imagekit.get_file_versions(file_id=file_id)  # file_id required
+
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's version id
+print(result.list[0].version_info.id)
+```
+
+**4. Get File Version details**
+
+Accepts the `file_id` and `version_id` and fetches the details as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-version-details)
+
+```python
+result = imagekit.get_file_version_details(
+    file_id='file_id',
+    version_id='version_id'
+)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+
+# print that file's version id
+print(result.version_info.id)
+```
+
+**5. Update File Details**
+
+Accepts all the parameters as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/update-file-details).
+The first argument to the `update_file_details()` method is the file ID, and a second argument is an object with the
+parameters to be
+updated.
+
+```python
+from imagekitio.models.UpdateFileRequestOptions import UpdateFileRequestOptions
+
+extensions = [
+    {
+        'name': 'remove-bg',
+        'options': {
+            'add_shadow': True,
+            'bg_color': 'red'
+        }
+    },
+    {
+        'name': 'google-auto-tagging',
+        'minConfidence': 80,
+        'maxTags': 10
+    }
+]
+
+options = UpdateFileRequestOptions(
+    remove_ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'],
+    webhook_url='url',
+    extensions=extensions,
+    tags=['tag-1', 'tag-2'],
+    custom_coordinates='10,10,100,100',
+    custom_metadata={'test': 11},
+)
+
+result = imagekit.update_file_details(file_id='62cfd39819ca454d82a07182'
+        , options=options)  # required
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+```
+
+**6. Add tags**
+
+Accepts a list of `file_ids` and `tags` as a parameter to be used to add tags. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/add-tags-bulk) can be passed to
+the `.add_tags()` functions to get the results.
+
+```python
+result = imagekit.add_tags(file_ids=['file-id-1', 'file-id-2'], tags=['add-tag-1', 'add-tag-2'])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully updated file ids
+print(result.successfully_updated_file_ids)
+
+# print the first file's id
+print(result.successfully_updated_file_ids[0])
+```
+
+**7. Remove tags**
+
+Accepts a list of `file_ids` and `tags` as a parameter to be used to remove tags. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-tags-bulk) can be passed to
+the `.remove_tags()` functions to get the results.
+
+```python
+result = imagekit.remove_tags(file_ids=['file-id-1', 'file-id-2'], tags=['remove-tag-1', 'remove-tag-2'])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully updated file ids
+print(result.successfully_updated_file_ids)
+
+# print the first file's id
+print(result.successfully_updated_file_ids[0])
+```
+
+**8. Remove AI tags**
+
+Accepts a list of `file_ids` and `ai_tags` as a parameter to remove AI tags. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-aitags-bulk) can be passed to
+the `.remove_ai_tags()` functions to get the results.
+
+```python
+result = imagekit.remove_ai_tags(file_ids=['file-id-1', 'file-id-2'], ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully updated file ids
+print(result.successfully_updated_file_ids)
+
+# print the first file's id
+print(result.successfully_updated_file_ids[0])
+```
+
+**9. Delete File**
+
+Delete a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file). It accepts the file ID of the File that has to be
+deleted.
+
+```python
+file_id = "file_id"
+result = imagekit.delete_file(file_id=file_id)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**10. Delete FileVersion**
+
+Delete a file version as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file-version).
+The method accepts the `file_id` and particular version id of the file that has to be deleted.
+
+```python
+result = imagekit.delete_file_version(file_id="file_id", version_id="version_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**11. Bulk File Delete by IDs**
+
+Delete a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-files-bulk).
+The method accepts a list of file IDs that have to be deleted.
+
+```python
+result = imagekit.bulk_file_delete(file_ids=["file_id1", "file_id2"])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully deleted file ids
+print(result.successfully_deleted_file_ids)
+
+# print the first file's id
+print(result.successfully_deleted_file_ids[0])
+```
+
+**12. Copy file**
+
+Copy a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-file).
+The method accepts `source_file_path`, `destination_path`, and `include_file_versions` of the file that has to be copied.
+
+```python
+from imagekitio.models.CopyFileRequestOptions import CopyFileRequestOptions
+
+options = \
+    CopyFileRequestOptions(source_file_path='/source_file_path.jpg',
+                           destination_path='/destination_path',
+                           include_file_versions=True)
+result = imagekit.copy_file(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**13. Move File**
+
+Move a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-file).
+The method accepts `source_file_path` and `destination_path` of the file that has to be moved.
+
+```python
+from imagekitio.models.MoveFileRequestOptions import MoveFileRequestOptions
+
+options = \
+    MoveFileRequestOptions(source_file_path='/source_file_path.jpg',
+                           destination_path='/destination_path')
+result = imagekit.move_file(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**14. Rename File**
+
+Rename a file per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/rename-file).
+The method accepts the `file_path`, `new_file_name`, and `purge_cache` boolean that has to be renamed.
+
+```python
+from imagekitio.models.RenameFileRequestOptions import RenameFileRequestOptions
+
+options = RenameFileRequestOptions(file_path='/file_path.jpg',
+                                   new_file_name='new_file_name.jpg',
+                                   purge_cache=True)
+result = imagekit.rename_file(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the purge request id
+print(result.purge_request_id)
+```
+
+**15. Restore file Version**
+
+Restore a file as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/restore-file-version).
+The method accepts the `file_id` and `version_id` of the file that has to be restored.
+
+```python
+result = imagekit.restore_file_version(file_id="file_id", version_id="version_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+```
+
+**16. Create Folder**
+
+Create a folder per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/create-folder).
+The method accepts `folder_name` and `parent_folder_path` as options that must be created.
+
+```Python
+from imagekitio.models.CreateFolderRequestOptions import CreateFolderRequestOptions
+
+options = CreateFolderRequestOptions(folder_name='test',
+                                     parent_folder_path='/')
+result = imagekit.create_folder(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**17. Delete Folder**
+
+Delete a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-folder).
+The method accepts `folder_path` as an option that must be deleted.
+
+```python
+from imagekitio.models.DeleteFolderRequestOptions import DeleteFolderRequestOptions
+
+options = DeleteFolderRequestOptions(folder_path='/test/demo')
+result = imagekit.delete_folder(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**18. Copy Folder**
+
+Copy a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-folder).
+The method accepts the `source_folder_path`, `destination_path`, and `include_file_versions` boolean as options that
+have to be copied.
+
+```python
+from imagekitio.models.CopyFolderRequestOptions import CopyFolderRequestOptions
+options = \
+    CopyFolderRequestOptions(source_folder_path='/source_folder_path',
+                             destination_path='/destination/path',
+                             include_file_versions=True)
+result = imagekit.copy_folder(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the job's id
+print(result.job_id)
+```
+
+**19. Move Folder**
+
+Move a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-folder).
+The method accepts the `source_folder_path` and `destination_path` of a folder as options that must be moved.
+
+```python
+from imagekitio.models.MoveFolderRequestOptions import MoveFolderRequestOptions
+options = \
+    MoveFolderRequestOptions(source_folder_path='/source_folder_path',
+                             destination_path='/destination_path')
+result = imagekit.move_folder(options=options)
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the job's id
+print(result.job_id)
+```
+
+**20. Get Bulk Job Status**
+
+Accepts the `job_id` to get bulk job status as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-move-folder-status).
+The method takes only jobId.
+
+```python
+result = imagekit.get_bulk_job_status(job_id="job_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the job's id
+print(result.job_id)
+
+# print the status
+print(result.status)
+```
+
+**21. Purge Cache**
+
+Programmatically issue an explicit cache request as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache).
+Accepts the full URL of the File for which the cache has to be cleared.
+
+```python
+result = imagekit.purge_file_cache(file_url="full_url_of_file")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the purge file cache request id
+print(result.request_id)
+```
+
+**22. Purge Cache Status**
+
+Get the purge cache request status using the `cache_request_id` returned when a purge cache request gets submitted as per the
+[API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache-status)
+
+```python
+result = imagekit.get_purge_file_cache_status(purge_cache_id="cache_request_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the purge file cache status
+print(result.status)
+```
+
+**23. Get File Metadata**
+
+Accepts the `file_id` and fetches the metadata as per
+the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-for-uploaded-media-files)
+
+```python
+result = imagekit.get_file_metadata(file_id="file_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the file metadata fields
+print(result.width)
+print(result.exif.image.x_resolution)
+```
+
+**24. Get File Metadata from remote URL**
+
+Accepts the `remote_file_url` and fetches the metadata as per
+the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-from-remote-url)
+
+```python
+result = imagekit.get_remote_file_url_metadata(remote_file_url="remote_file_url")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the file metadata fields
+print(result.width)
+print(result.exif.image.x_resolution)
+```
+
+**25. Create CustomMetaDataFields**
+
+Accepts an option specifying the parameters used to create custom metadata fields. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field)
+can be passed as it is with the correct values to get the results.
+
+Check for the [allowed values in the schema](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field#allowed-values-in-the-schema-object).
+
+**Example:**
+
+```python
+# Example for the type number
+
+from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
+schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Number,
+                                    min_value=100,
+                                    max_value=200)
+options = CreateCustomMetadataFieldsRequestOptions(name='test',
+                                                   label='test',
+                                                   schema=schema)
+result = imagekit.create_custom_metadata_fields(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the id of created custom metadata fields
+print(result.id)
+
+# print the schema's type of created custom metadata fields
+print(result.schema.type)
+
+```
+
+```python
+# MultiSelect type Example
+
+from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
+
+schema = \
+    CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.MultiSelect,
+                               is_value_required=True,
+                               default_value=['small', 30, True],
+                               select_options=[
+                                    'small',
+                                    'medium',
+                                    'large',
+                                    30,
+                                    40,
+                                    True,
+                                ])
+options = \
+    CreateCustomMetadataFieldsRequestOptions(name='test-MultiSelect',
+        label='test-MultiSelect', schema=schema)
+result = imagekit.create_custom_metadata_fields(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the name of created custom metadata fields
+print(result.name)
+
+# print the schema's select options of created custom metadata fields
+print(result.schema.select_options)
+
+```
+
+```python
+# Date type Example
+
+from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
+
+schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Date,
+                                    min_value='2022-11-29T10:11:10+00:00',
+                                    max_value='2022-11-30T10:11:10+00:00')
+options = CreateCustomMetadataFieldsRequestOptions(name='test-date',
+                                                   label='test-date',
+                                                   schema=schema)
+result = imagekit.create_custom_metadata_fields(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the label of created custom metadata fields
+print(result.label)
+
+# print the schema's min value of created custom metadata fields
+print(result.schema.min_value)
+
+```
+
+**26. Get CustomMetaDataFields**
+
+Accepts the `include_deleted` boolean as the initial parameter and fetches the metadata as per
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/get-custom-metadata-field)
+.
+
+```python
+result = imagekit.get_custom_metadata_fields()  # in this case, it will consider includeDeleted as a False
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the first customMetadataField's id
+print(result.list[0].id)
+
+# print the first customMetadataField schema's type
+print(result.list[0].schema.type)
+```
+
+```python
+result = imagekit.get_custom_metadata_fields(include_deleted=True)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the first customMetadataField's name
+print(result.list[0].name)
+
+# print the first customMetadataField schema's default value
+print(result.list[0].schema.default_value)
+```
+
+**27. Update CustomMetaDataFields**
+
+Accepts a `field_id` and options for specifying the parameters to be used to edit custom metadata fields
+as per
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/update-custom-metadata-field)
+.
+
+```python
+
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.UpdateCustomMetadataFieldsRequestOptions import UpdateCustomMetadataFieldsRequestOptions
+
+schema = CustomMetadataFieldsSchema(min_value=100, max_value=200)
+options = UpdateCustomMetadataFieldsRequestOptions(
+    label='test-update',
+    schema=schema
+)
+result = imagekit.update_custom_metadata_fields(
+    field_id='id_of_custom_metadata_field',
+    options=options
+)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the label of updated custom metadata fields
+print(result.label)
+
+# print the schema's min value of updated custom metadata fields
+print(result.schema.min_value)
+```
+
+**28. Delete CustomMetaDataFields**
+
+Accepts the id to delete the custom metadata fields as per
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/delete-custom-metadata-field)
+.
+
+```python
+result = imagekit.delete_custom_metadata_field(field_id="id_of_custom_metadata_field")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+## Utility functions
+
+We have included the following commonly used utility functions in this package.
+
+**Authentication parameter generation**
+
+Suppose one wants to implement client-side file upload. In that case, one will need a token, expiry timestamp, and a valid signature for that upload. The SDK provides a simple method that one can use in their code to generate these authentication parameters.
+
+<em>Note: Any client-side code should never expose The Private API Key. One must always generate these authentications parameters on the server-side</em>
+
+authentication
+
+`authentication_parameters = imagekit.get_authentication_parameters(token, expire)`
+
+Returns
+
+```python
+{
+    "token": "unique_token",
+    "expire": "valid_expiry_timestamp",
+    "signature": "generated_signature"
+}
+```
+
+Both the `token` and `expire` parameters are optional. If not specified, the SDK uses the UUID to generate a random token and internally generates a valid expiry timestamp. The `token` and `expire` used to generate `signature` is part of a response returned by the server.
+
+**Distance calculation between two `pHash` values**
+
+Perceptual hashing allows you to construct a has value that uniquely identifies an input image based on the contents
+of an image. [imagekit.io metadata API](https://docs.imagekit.io/api-reference/metadata-api) returns the `pHash`
+value of an image in the response. You can use this value
+to [find a duplicate or similar image](https://docs.imagekit.io/api-reference/metadata-api#using-phash-to-find-similar-or-duplicate-images)
+by calculating the distance between the two images.
+
+This SDK exposes the `phash_distance` function to calculate the distance between two `pHash` values. It accepts two `pHash`
+hexadecimal
+strings and returns a numeric value indicative of the difference between the two images.
+
+```python
+def calculate_distance():
+    # fetch metadata of two uploaded image files
+    ...
+    # extract pHash strings from both: say 'first_hash' and 'second_hash'
+    ...
+    # calculate the distance between them:
+
+    distance = imagekit.phash_distance(first_hash, second_hash)
+    return distance
+
+```
+
+**Distance calculation examples**
+
+```Python
+imagekit.phash_distance('f06830ca9f1e3e90', 'f06830ca9f1e3e90')
+# output: 0 (same image)
+
+imagekit.phash_distance('2d5ad3936d2e015b', '2d6ed293db36a4fb')
+# output: 17 (similar images)
+
+imagekit.phash_distance('a4a65595ac94518b', '7838873e791f8400')
+# output: 37 (dissimilar images)
+```
+
+**HTTP response metadata of Internal API**
+
+HTTP response metadata of the internal API call can be accessed using the \_response_metadata on the Result object.
+Example:
+
+```Python
+result = imagekit.upload_file(
+    file="<url|base_64|binary>",
+    file_name="my_file_name.jpg",
+)
+
+# Final Result
+print(result)
+print(result.response_metadata.raw)
+print(result.response_metadata.http_status_code)
+print(result.response_metadata.headers)
+```
+
+### Sample Code Instruction
+
+To run `sample` code go to the code samples here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python and run.
+
+```shell
+python sample.py
+```
+
+## Handling errors
+
+Catch and respond to invalid data, internal problems, and more.
+
+ImageKit Python SDK raises exceptions for many reasons, such as not found, invalid parameters, authentication, and
+internal server errors. Therefore, we recommend writing code that gracefully handles all possible API exceptions.
+
+#### Example:
+
+```Python
+from imagekitio.exceptions.BadRequestException import BadRequestException
+from imagekitio.exceptions.UnauthorizedException import UnauthorizedException
+from imagekitio.exceptions.ForbiddenException import ForbiddenException
+from imagekitio.exceptions.TooManyRequestsException import TooManyRequestsException
+from imagekitio.exceptions.InternalServerException import InternalServerException
+from imagekitio.exceptions.PartialSuccessException import PartialSuccessException
+from imagekitio.exceptions.NotFoundException import NotFoundException
+from imagekitio.exceptions.UnknownException import UnknownException
+
+try:
+
+    # Use ImageKit's SDK to make requests...
+    print('Run image kit api')
+except BadRequestException, e:
+    # Missing or Invalid parameters were supplied to Imagekit.io's API
+    print('Status is: ' + e.response_metadata.http_status_code)
+    print('Message is: ' + e.message)
+    print('Headers are: ' + e.response_metadata.headers)
+    print('Raw body is: ' + e.response_metadata.raw)
+except UnauthorizedException, e:
+    print(e)
+except ForbiddenException, e:
+    # No valid API key was provided.
+    print(e)
+except TooManyRequestsException, e:
+    # Can be for the following reasons:
+    # ImageKit could not authenticate your account with the keys provided.
+    # An expired key (public or private) was used with the request.
+    # The account is disabled.
+    # If you use the upload API, the total storage limit (or upload limit) is exceeded.
+    print(e)
+except InternalServerException, e:
+    # Too many requests made to the API too quickly
+    print(e)
+except PartialSuccessException, e:
+    # Something went wrong with ImageKit.io API.
+    print(e)
+except NotFoundException, e:
+    # Error cases on partial success.
+    print(e)
+except UnknownException, e:
+    # If any of the field or parameter is not found in the data
+    print(e)
+
+# Something else happened, which can be unrelated to ImageKit; the reason will be indicated in the message field
+```
+
+## Development
+
+### Tests
+
+Tests are powered by [Tox](https://tox.wiki/en/latest/).
+
+```bash
+$ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
+$ pip install tox
+$ tox
+```
+
+### Sample
+
+#### Get & Install local ImageKit Python SDK
+
+```bash
+$ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
+$ pip install -e .
+```
+
+#### Get samples
+
+To integrate ImageKit Samples in the Python, the code samples covered here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python.
+
+Open the `python/sample.py` file and replace placeholder credentials with actual values. You can get the value of [URL-endpoint](https://imagekit.io/dashboard#url-endpoints) from your ImageKit dashboard. API keys can be obtained from the [developer](https://imagekit.io/dashboard/developer/api-keys) section in your ImageKit dashboard.
+
+In the `python/sample.py` file, set the following parameters for authentication:
+
+```python
+from imagekitio import ImageKit
+imagekit = ImageKit(
+    private_key='your private_key',
+    public_key='your public_key',
+    url_endpoint = 'your url_endpoint'
+)
+```
+
+To install dependencies that are in the `python/requirements.txt` file, can fire this command to install them:
+
+```shell
+pip install -r python/requirements.txt
+```
+
+Now run `python/sample.py`. If you are using CLI Tool (Terminal/Command prompt), open the project in CLI and execute it.
+
+```shell
+# if not installed already
+pip install imagekitio
+
+# if installing local sdk
+pip install -e <path_to_local_sdk>
+
+# to run sample.py file
+python3 python/sample.py
+```
+
+## Support
+
+For any feedback or to report any issues or general implementation support, please reach out
+to [support@imagekit.io](https://github.com/imagekit-developer/imagekit-python)
+
+## Links
+
+-   [Documentation](https://docs.imagekit.io/)
+
+-   [Main Website](https://imagekit.io/)
+
+## License
+
+Released under the MIT license.
```

### Comparing `imagekitio-3.0.2/README.md` & `imagekitio-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/client.py` & `imagekitio-3.1.0/imagekitio/client.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/constants/defaults.py` & `imagekitio-3.1.0/imagekitio/constants/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
     DEFAULT_TRANSFORMATION_POSITION = "path"
     QUERY_TRANSFORMATION_POSITION = "query"
     VALID_TRANSFORMATION_POSITION = [
         DEFAULT_TRANSFORMATION_POSITION,
         QUERY_TRANSFORMATION_POSITION,
     ]
     DEFAULT_TIMESTAMP = 9999999999
-    SDK_VERSION = "python-3.0.2"
+    SDK_VERSION = "python-3.1.0"
     TRANSFORMATION_PARAMETER = "tr"
     CHAIN_TRANSFORM_DELIMITER = ":"
     TRANSFORM_DELIMITER = ","
     TRANSFORM_KEY_VALUE_DELIMITER = "-"
     SIGNATURE_PARAMETER = "ik-s"
     TIMESTAMP_PARAMETER = "ik-t"
```

### Comparing `imagekitio-3.0.2/imagekitio/constants/errors.py` & `imagekitio-3.1.0/imagekitio/constants/errors.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/constants/files.py` & `imagekitio-3.1.0/imagekitio/constants/files.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/constants/supported_transform.py` & `imagekitio-3.1.0/imagekitio/constants/supported_transform.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/file.py` & `imagekitio-3.1.0/imagekitio/file.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py` & `imagekitio-3.1.0/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/CustomMetadataFieldsSchema.py` & `imagekitio-3.1.0/imagekitio/models/CustomMetadataFieldsSchema.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/ListAndSearchFileRequestOptions.py` & `imagekitio-3.1.0/imagekitio/models/ListAndSearchFileRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py` & `imagekitio-3.1.0/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/UpdateFileRequestOptions.py` & `imagekitio-3.1.0/imagekitio/models/UpdateFileRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/UploadFileRequestOptions.py` & `imagekitio-3.1.0/imagekitio/models/UploadFileRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py` & `imagekitio-3.1.0/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 class CustomMetadataFieldsResultWithResponseMetadata(CustomMetadataFieldsResult):
     def __init__(
         self,
         id=None,
         name=None,
         label=None,
-        schema: CustomMetadataSchema = CustomMetadataSchema(
-            None, None, None, None, None, None, None, None
-        ),
+        schema:dict = {},
+        **kwargs
     ):
         super(CustomMetadataFieldsResultWithResponseMetadata, self).__init__(
-            id, name, label, schema
+            id, name, label, schema,**kwargs
         )
         self.response_metadata: ResponseMetadata = ResponseMetadata("", "", "")
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/CustomMetadataSchema.py` & `imagekitio-3.1.0/imagekitio/models/results/CustomMetadataSchema.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,23 @@
         select_options=None,
         default_value=None,
         is_value_required=None,
         min_value=None,
         max_value=None,
         min_length=None,
         max_length=None,
+        **kwargs
+        
     ):
         self.type = type
         self.select_options = select_options
         self.default_value = default_value
         self.is_value_required = is_value_required
         self.min_value = min_value
         self.max_value = max_value
         self.min_length = min_length
         self.max_length = max_length
+        for key in kwargs.keys():
+                self.__setattr__(key,kwargs[key])
+    def __getattr__(self,key):
+        return None
+
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/FileResult.py` & `imagekitio-3.1.0/imagekitio/models/results/FileResult.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 from .AITags import AITags
 from .VersionInfo import VersionInfo
-
+from ...utils.utils import camel_dict_to_snake_dict
 
 class FileResult:
     def __init__(
         self,
         type=None,
         name=None,
         created_at=None,
@@ -24,39 +24,43 @@
         file_path: str = "",
         height: int = None,
         width: int = None,
         size: int = None,
         has_alpha=False,
         mime: str = None,
         extension_status: dict = {},
+        **kwargs
     ):
         self.type = type
         self.name = name
         self.created_at = created_at
         self.updated_at = updated_at
         self.file_id = file_id
         self.tags = tags
         self.ai_tags: List[AITags] = []
         if ai_tags is not None:
             for i in ai_tags:
                 self.ai_tags.append(
                     AITags(
-                        i["name"] if "name" in i else None,
-                        i["confidence"] if "confidence" in i else None,
-                        i["source"] if "source" in i else None,
+                        **camel_dict_to_snake_dict(i)
                     )
                 )
-        self.version_info = VersionInfo(version_info["id"], version_info["name"])
+        self.version_info = VersionInfo(**camel_dict_to_snake_dict(version_info))
         self.embedded_metadata = embedded_metadata
         self.custom_coordinates = custom_coordinates
         self.custom_metadata = custom_metadata
         self.is_private_file = is_private_file
         self.url = url
         self.thumbnail = thumbnail
         self.file_type = file_type
         self.file_path = file_path
         self.height = height
         self.width = width
         self.size = size
         self.has_alpha = has_alpha
         self.mime = mime
         self.extension_status = extension_status
+        for key in kwargs.keys():
+                self.__setattr__(key,kwargs[key])
+    def __getattr__(self,key):
+        return None
+
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/FileResultWithResponseMetadata.py` & `imagekitio-3.1.0/imagekitio/models/results/FileResultWithResponseMetadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,30 +11,31 @@
         self,
         type=None,
         name=None,
         created_at=None,
         updated_at=None,
         file_id=None,
         tags=None,
-        ai_tags: List[AITags] = AITags(None, None, None),
-        version_info: VersionInfo = VersionInfo(None, None),
+        ai_tags: List[AITags] = [],
+        version_info: dict = {},
         embedded_metadata=None,
         custom_coordinates: str = "",
         custom_metadata=None,
         is_private_file=False,
         url: str = "",
         thumbnail: str = "",
         file_type: str = "",
         file_path: str = "",
         height: int = None,
         width: int = None,
         size: int = None,
         has_alpha=False,
         mime: str = None,
         extension_status=None,
+        **kwargs
     ):
         super().__init__(
             type,
             name,
             created_at,
             updated_at,
             file_id,
@@ -51,9 +52,10 @@
             file_path,
             height,
             width,
             size,
             has_alpha,
             mime,
             extension_status,
+            **kwargs
         )
         self.response_metadata: ResponseMetadata = ResponseMetadata("", "", "")
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/GetMetadataResult.py` & `imagekitio-3.1.0/imagekitio/models/results/GetMetadataResult.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .MetadataExifExif import MetadataExifExif
 from .MetadataExifGPS import MetadataExifGPS
 from .MetadataExifInteroperability import MetadataExifInteroperability
 from .MetadataExifThumbnail import MetadataExifThumbnail
 from .MetadataExif import MetadataExif
 from .MetadataExifImage import MetadataExifImage
 from .ResponseMetadata import ResponseMetadata
+from ...utils.utils import camel_dict_to_snake_dict
 
 
 class GetMetadataResult:
     def __init__(
         self,
         height=None,
         width=None,
@@ -16,34 +17,35 @@
         format=None,
         has_color_profile=None,
         quality=None,
         density=None,
         has_transparency=None,
         p_hash=None,
         exif: dict = {},
+        **kwargs
     ):
         self.height = height
         self.width = width
         self.size = size
         self.format = format
         self.has_color_profile = has_color_profile
         self.quality = quality
         self.density = density
         self.has_transparency = has_transparency
         self.p_hash = p_hash
         self.exif: MetadataExif = MetadataExif(
-            exif["image"] if "image" in exif else None,
-            exif["thumbnail"] if "thumbnail" in exif else None,
-            exif["exif"] if "exif" in exif else None,
-            exif["gps"] if "gps" in exif else None,
-            exif["interoperability"] if "interoperability" in exif else None,
-            exif["makernote"] if "makernote" in exif else None,
+            ** camel_dict_to_snake_dict(exif)
         )
         self.__response_metadata: ResponseMetadata = ResponseMetadata("", "", "")
 
+        for key in kwargs.keys():
+                self.__setattr__(key,kwargs[key])
+    def __getattr__(self,key):
+        return None
+
     @property
     def response_metadata(self):
         return self.__response_metadata
 
     @response_metadata.setter
     def response_metadata(self, value):
         self.__response_metadata = value
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/ListCustomMetadataFieldsResult.py` & `imagekitio-3.1.0/imagekitio/models/results/ListCustomMetadataFieldsResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/models/results/MetadataExifExif.py` & `imagekitio-3.1.0/imagekitio/models/results/MetadataExifExif.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         focal_plane_x_resolution=None,
         focal_plane_y_resolution=None,
         focal_plane_resolution_unit=None,
         custom_rendered=None,
         exposure_mode=None,
         white_balance=None,
         scene_capture_type=None,
+        **kwargs
     ):
         self.exposure_time = exposure_time
         self.f_number = f_number
         self.exposure_program = exposure_program
         self.iso = iso
         self.exif_version = exif_version
         self.date_time_original = date_time_original
@@ -54,7 +55,11 @@
         self.focal_plane_x_resolution = focal_plane_x_resolution
         self.focal_plane_y_resolution = focal_plane_y_resolution
         self.focal_plane_resolution_unit = focal_plane_resolution_unit
         self.custom_rendered = custom_rendered
         self.exposure_mode = exposure_mode
         self.white_balance = white_balance
         self.scene_capture_type = scene_capture_type
+        for key in kwargs.keys():
+                self.__setattr__(key,kwargs[key])
+    def __getattr__(self,key):
+        return None
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/MetadataExifImage.py` & `imagekitio-3.1.0/imagekitio/models/results/MetadataExifImage.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,19 +8,24 @@
         y_resolution=None,
         resolution_unit=None,
         software=None,
         modify_date=None,
         y_cb_cr_positioning=None,
         exif_offset=None,
         gps_info=None,
+        **kwargs
     ):
         self.make = make
         self.model = model
         self.orientation = orientation
         self.x_resolution = x_resolution
         self.y_resolution = y_resolution
         self.resolution_unit = resolution_unit
         self.software = software
         self.modify_date = modify_date
         self.y_cb_cr_positioning = y_cb_cr_positioning
         self.exif_offset = exif_offset
         self.gps_info = gps_info
+        for key in kwargs.keys():
+                self.__setattr__(key,kwargs[key])
+    def __getattr__(self,key):
+        return None
```

### Comparing `imagekitio-3.0.2/imagekitio/models/results/UploadFileResult.py` & `imagekitio-3.1.0/imagekitio/models/results/UploadFileResult.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 from .AITags import AITags
 from .EmbeddedMetadata import EmbeddedMetadata
 from .ResponseMetadata import ResponseMetadata
 from .VersionInfo import VersionInfo
-
+from ...utils.utils import camel_dict_to_snake_dict
 
 class UploadFileResult:
     def __init__(
         self,
         file_id=None,
         name=None,
         url=None,
@@ -22,51 +22,54 @@
         version_info: VersionInfo = VersionInfo(None, None),
         is_private_file=False,
         custom_coordinates: dict = None,
         custom_metadata: dict = None,
         embedded_metadata: EmbeddedMetadata = EmbeddedMetadata(None, None, None, None),
         extension_status: dict = None,
         file_type: str = None,
-        orientation: int = None
+        orientation: int = None,
+        **kwargs
     ):
         self.file_id = file_id
         self.name = name
         self.url = url
         self.thumbnail_url = thumbnail_url
         self.height = height
         self.width = width
         self.size = size
         self.file_path = file_path
         self.tags = tags
         self.ai_tags: List[AITags] = []
         if ai_tags is not None:
             for i in ai_tags:
-                self.ai_tags.append(AITags(i["name"], i["confidence"], i["source"]))
+                self.ai_tags.append(AITags(**camel_dict_to_snake_dict(i)))
         else:
             self.ai_tags.append(AITags(None, None, None))
-        self.version_info = VersionInfo(version_info["id"], version_info["name"])
+        self.version_info = VersionInfo(**camel_dict_to_snake_dict(version_info))
         self.is_private_file = is_private_file
         self.custom_coordinates = custom_coordinates
         self.custom_metadata = custom_metadata
         if embedded_metadata is None or embedded_metadata == {}:
             self.embedded_metadata = EmbeddedMetadata(None, None, None, None)
         else:
             if type(embedded_metadata) == EmbeddedMetadata:
                 self.embedded_metadata = embedded_metadata
             else:
                 self.embedded_metadata: EmbeddedMetadata = EmbeddedMetadata(
-                    embedded_metadata["x_resolution"],
-                    embedded_metadata["y_resolution"],
-                    embedded_metadata["date_created"],
-                    embedded_metadata["date_time_created"],
+                    **camel_dict_to_snake_dict(embedded_metadata)
                 )
         self.extension_status = extension_status
         self.file_type = file_type
         self.orientation = orientation
         self.__response_metadata: ResponseMetadata = ResponseMetadata("", "", "")
+        for key in kwargs.keys():
+            self.__setattr__(key,kwargs[key])
+    def __getattr__(self,key):
+        return None
+    
 
     @property
     def response_metadata(self):
         return self.__response_metadata
 
     @response_metadata.setter
     def response_metadata(self, value):
```

### Comparing `imagekitio-3.0.2/imagekitio/resource.py` & `imagekitio-3.1.0/imagekitio/resource.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/url.py` & `imagekitio-3.1.0/imagekitio/url.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/utils/calculation.py` & `imagekitio-3.1.0/imagekitio/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/utils/formatter.py` & `imagekitio-3.1.0/imagekitio/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/imagekitio/utils/utils.py` & `imagekitio-3.1.0/imagekitio/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,19 +72,15 @@
     elif response.status_code == 404:
         raise NotFoundException(error_message, response_help, response_meta_data)
     else:
         raise UnknownException(error_message, response_help, response_meta_data)
 
 
 def convert_to_response_object(resp: Response, response_object):
-    resp_json = resp.json()
-    embeddedMetadata = resp_json.get("embeddedMetadata")
-    if embeddedMetadata != None:
-        resp_json["embeddedMetadata"] = camel_dict_to_snake_dict(embeddedMetadata)
-    res_new = loads(dumps(camel_dict_to_snake_dict(resp_json)))
+    res_new = loads(dumps(camel_dict_to_snake_dict(resp.json())))
     u = response_object(**res_new)
     u.response_metadata = ResponseMetadata(resp.json(), resp.status_code, resp.headers)
     return u
 
 
 def convert_to_response_metadata_result_object(resp: Response = None):
     u = ResponseMetadataResult()
```

### Comparing `imagekitio-3.0.2/imagekitio.egg-info/PKG-INFO` & `imagekitio-3.1.0/imagekitio.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,1318 +1,1317 @@
 Metadata-Version: 2.1
 Name: imagekitio
-Version: 3.0.2
+Version: 3.1.0
 Summary: Python wrapper for the ImageKit API
 Home-page: https://github.com/imagekit-developer/imagekit-python
-License: UNKNOWN
-Description: [<img width="250" alt="ImageKit.io" src="https://raw.githubusercontent.com/imagekit-developer/imagekit-javascript/master/assets/imagekit-light-logo.svg"/>](https://imagekit.io)
-        
-        # ImageKit.io Python SDK
-        
-        [![Python CI](https://github.com/imagekit-developer/imagekit-python/workflows/Python%20CI/badge.svg)](https://github.com/imagekit-developer/imagekit-python/)
-        [![imagekitio](https://img.shields.io/pypi/v/imagekitio.svg)](https://pypi.org/project/imagekitio)
-        [![codecov](https://codecov.io/gh/imagekit-developer/imagekit-python/branch/master/graph/badge.svg?token=CwKWqBIlCu)](https://codecov.io/gh/imagekit-developer/imagekit-python)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![Twitter Follow](https://img.shields.io/twitter/follow/imagekitio?label=Follow&style=social)](https://twitter.com/ImagekitIo)
-        
-        Python SDK for [ImageKit](https://imagekit.io/) implements the new APIs and interface for different file operations.
-        
-        ImageKit is complete media storage, optimization, and transformation solution that comes with an [image and video CDN](https://imagekit.io/features/imagekit-infrastructure). It can be integrated with your existing infrastructure - storage like AWS S3, web servers, your CDN, and custom domain names, allowing you to deliver optimized images in minutes with minimal code changes.
-        
-        Supported Python Versions: >=3.6
-        
-        Table of contents -
-        
-        -   [Installation](#installation)
-        -   [Initialization](#initialization)
-        -   [Change Log](#change-log)
-        -   [Usage](#usage)
-            -   [URL Generation](#url-generation)
-            -   [File Upload](#file-upload)
-            -   [File Management](#file-management)
-            -   [Utility Functions](#utility-functions)
-        -   [Handling errors](#handling-errors)
-        -   [Development](#development)
-            -   [Tests](#tests)
-            -   [Sample](#sample)
-        -   [Support](#support)
-        -   [Links](#links)
-        
-        ## Installation
-        
-        Go to your terminal and type the following command.
-        
-        ```bash
-        pip install imagekitio
-        ```
-        
-        ## Initialization
-        
-        ```python
-        from imagekitio import ImageKit
-        
-        imagekit = ImageKit(
-            private_key='your_private_key',
-            public_key='your_public_key',
-            url_endpoint='your_url_endpoint'
-        )
-        ```
-        
-        ## Change log
-        
-        This document presents a list of changes that break the existing functionality of previous versions. We try to minimize these disruptions, but they are sometimes unavoidable, especially in significant updates. Therefore, versions are marked semantically and tagged as major upgrades whenever such breaking changes occur.
-        
-        ### Breaking History:
-        
-        Changes from `2.2.8 -> 3.0.0` are listed below
-        
-        1. Throw an Error:
-        
-        **What changed**
-        
-        -   Before the upgrade, an `error` dict was coming in the return object of any function call. Now, SDK throws an exception in case of an error.
-        
-        **Who is affected?**
-        
-        -   This affects any development in your software that calls APIs from ImageKit IO and handles errors based on what's returned.
-        
-        **How should I update my code?**
-        
-        -   To avoid failures in an application, you could handle errors as [documented here](#handling-errors)
-        
-        # Usage
-        
-        You can use this Python SDK for three different kinds of methods:
-        
-        -   [URL Generation](#url-generation)
-        -   [File Upload](#file-upload)
-        -   [File Management](#file-management)
-        -   [Utility Functions](#utility-functions)
-        
-        ## URL Generation
-        
-        **1. Using Image path and endpoint (hostname)**
-        
-        This method allows you to create a URL using the relative file path where the image exists and the URL
-        endpoint(url_endpoint) you want to use to access the image. You can refer to the documentation
-        [here](https://docs.imagekit.io/integration/url-endpoints) to read more about URL endpoints
-        in ImageKit and the section about [image origins](https://docs.imagekit.io/integration/configure-origin) to understand
-        about paths with different kinds of origins.
-        
-        The file can be an image, video, or any other static file supported by ImageKit.
-        
-        ```python
-        imagekit_url = imagekit.url({
-            "path": "/default-image.jpg",
-            "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
-            "transformation": [{
-                "height": "300",
-                "width": "400",
-                "raw": "ar-4-3,q-40"
-            }],
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/endpoint/tr:h-300,w-400,ar-4-3,q-40/default-image.jpg
-        ```
-        
-        **2. Using full image URL**
-        
-        This method allows you to add transformation parameters to an absolute URL using the `src` parameter. This method should be
-        used if you have the complete image URL stored in your database.
-        
-        ```python
-        image_url = imagekit.url({
-            "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
-            "transformation": [{
-                "height": "300",
-                "width": "400",
-                "raw": "ar-4-3,q-40"
-            }]
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%2Car-4-3%2Cq-40
-        ```
-        
-        The `.url()` method accepts the following parameters.
-        
-        | Option                  | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-        | :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-        | url_endpoint            | Optional. The prepended base URL before the path of the image. If not specified, the URL Endpoint specified during SDK initialization gets used. For example, https://ik.imagekit.io/your_imagekit_id/endpoint/                                                                                                                                                                                                                                                                             |
-        | path                    | Conditional. A path at which the image exists. For example, `/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                                                                                   |
-        | src                     | Conditional. Complete URL of an image already mapped to ImageKit. For example, `https://ik.imagekit.io/your_imagekit_id/endpoint/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                |
-        | transformation          | Optional. Specify an array of objects with name and the value in key-value pair to apply transformation params in the URL. Append different steps of a [chained transformation](https://docs.imagekit.io/features/image-transformations/chained-transformations) as different objects of the array. This document includes a complete list of supported transformations in the SDK with some examples. If one uses an unspecified transformation name, it gets applied as it is in the URL. |
-        | transformation_position | Optional. The default value is `path`, which places the transformation string as a path parameter in the URL. One can also specify it as a query, which adds the transformation string as the query parameter `tr` in the URL. Suppose one uses the `src` parameter to create the URL. In that case, the transformation string is always a query parameter.                                                                                                                                 |
-        | query_parameters        | Optional. These are the other query parameters that one wants to add to the final URL. These can be any query parameters and are not necessarily related to ImageKit. Especially useful if one wants to add some versioning parameter to their URLs.                                                                                                                                                                                                                                        |
-        | signed                  | Optional. Boolean. The default is `false`. If set to `true`, the SDK generates a signed image URL adding the image signature to the image URL. One can only use this if they create the URL with the `url_endpoint` and `path` parameters, not the `src` parameter.                                                                                                                                                                                                                         |
-        | expire_seconds          | Optional. Integer. Used along with the `signed` parameter to specify the time in seconds from `now` when the URL should expire. If specified, the URL contains the expiry timestamp, and the image signature is modified accordingly.                                                                                                                                                                                                                                                       |
-        
-        ## Examples of generating URLs
-        
-        **1. Chained Transformations as a query parameter**
-        
-        ```python
-        image_url = imagekit.url({
-            "path": "/default-image.jpg",
-            "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
-            "transformation": [
-                {
-                    "height": "300",
-                    "width": "400"
-                },
-                {
-                    "rotation": 90
-                }
-            ],
-            "transformation_position": "query"
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%3Art-90
-        ```
-        
-        **2. Sharpening, contrast transform and progressive JPG image**
-        
-        Add transformations like [Sharpening](https://docs.imagekit.io/features/image-transformations/image-enhancement-and-color-manipulation) to the URL with or without any other value. To use such transforms without specifying a value, set it as "-" in the transformation object. Otherwise, use the value that one wants to add to this transformation.
-        
-        ```python
-        image_url = imagekit.url({
-            "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
-            "transformation": [{
-                "format": "jpg",
-                "progressive": "true",
-                "effect_sharpen": "-",
-                "effect_contrast": "1"
-            }]
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        # Note that because the `src` parameter is in effect, the transformation string gets added as a query parameter `tr`
-        
-        https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=f-jpg%2Cpr-true%2Ce-sharpen%2Ce-contrast-1
-        ```
-        
-        **3. Signed URL that expires in 300 seconds with the default URL endpoint and other query parameters**
-        
-        ```python
-        image_url = imagekit.url({
-            "path": "/default-image.jpg",
-            "query_parameters": {
-                "p1": "123",
-                "p2": "345"
-            },
-            "transformation": [{
-                "height": "300",
-                "width": "400"
-            }],
-            "signed": True,
-            "expire_seconds": 300
-        })
-        ```
-        
-        Sample Result URL -
-        
-        ```
-        https://ik.imagekit.io/your_imagekit_id/tr:h-300,w-400/default-image.jpg?p1=123&p2=345&ik-t=1658899345&ik-s=8f03aca28432d4e87f697a48143efb4497bbed9e
-        ```
-        
-        **List of transformations**
-        
-        The complete list of transformations supported and their usage in ImageKit is available [here](https://docs.imagekit.io/features/image-transformations/resize-crop-and-other-transformations).
-        The SDK gives a name to each transformation parameter, making the code simpler, more straightforward, and readable. If a transformation is supported in ImageKit, though it cannot be found in the table below, then use the transformation code from ImageKit docs as the name when using the `URL` function.
-        
-        If you want to generate transformations in your application and add them to the URL as it is, use the raw parameter.
-        
-        | Supported Transformation Name | Translates to parameter         |
-        | ----------------------------- | ------------------------------- |
-        | height                        | h                               |
-        | width                         | w                               |
-        | aspect_ratio                  | ar                              |
-        | quality                       | q                               |
-        | crop                          | c                               |
-        | crop_mode                     | cm                              |
-        | x                             | x                               |
-        | y                             | y                               |
-        | focus                         | fo                              |
-        | format                        | f                               |
-        | radius                        | r                               |
-        | background                    | bg                              |
-        | border                        | b                               |
-        | rotation                      | rt                              |
-        | blur                          | bl                              |
-        | named                         | n                               |
-        | overlay_x                     | ox                              |
-        | overlay_y                     | oy                              |
-        | overlay_focus                 | ofo                             |
-        | overlay_height                | oh                              |
-        | overlay_width                 | ow                              |
-        | overlay_image                 | oi                              |
-        | overlay_image_trim            | oit                             |
-        | overlay_image_aspect_ratio    | oiar                            |
-        | overlay_image_background      | oibg                            |
-        | overlay_image_border          | oib                             |
-        | overlay_image_dpr             | oidpr                           |
-        | overlay_image_quality         | oiq                             |
-        | overlay_image_cropping        | oic                             |
-        | overlay_image_focus           | oifo                            |
-        | overlay_text                  | ot                              |
-        | overlay_text_font_size        | ots                             |
-        | overlay_text_font_family      | otf                             |
-        | overlay_text_color            | otc                             |
-        | overlay_text_transparency     | oa                              |
-        | overlay_alpha                 | oa                              |
-        | overlay_text_typography       | ott                             |
-        | overlay_background            | obg                             |
-        | overlay_text_encoded          | ote                             |
-        | overlay_text_width            | otw                             |
-        | overlay_text_background       | otbg                            |
-        | overlay_text_padding          | otp                             |
-        | overlay_text_inner_alignment  | otia                            |
-        | overlay_radius                | or                              |
-        | progressive                   | pr                              |
-        | lossless                      | lo                              |
-        | trim                          | t                               |
-        | metadata                      | md                              |
-        | color_profile                 | cp                              |
-        | default_image                 | di                              |
-        | dpr                           | dpr                             |
-        | effect_sharpen                | e-sharpen                       |
-        | effect_usm                    | e-usm                           |
-        | effect_contrast               | e-contrast                      |
-        | effect_gray                   | e-grayscale                     |
-        | original                      | orig                            |
-        | raw                           | replaced by the parameter value |
-        
-        ## File Upload
-        
-        The SDK provides a simple interface using the `.upload_file()` method to upload files to the ImageKit Media library. It
-        accepts all the parameters supported by
-        the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload).
-        
-        The `upload_file()` method requires at least the `file` as (URL/Base64/Binary) and the `file_name` parameter to upload a
-        file. The method returns a dict data in case of success, or it will throw a custom exception in case of failure.
-        Use the `options` parameter to pass other parameters supported by
-        the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload). Use the same
-        parameter name as specified in the upload API documentation.
-        
-        Simple usage
-        
-        ```python
-        from imagekitio.models.UploadFileRequestOptions import UploadFileRequestOptions
-        
-        extensions = [
-            {
-                'name': 'remove-bg',
-                'options': {
-                    'add_shadow': True,
-                    'bg_color': 'pink'
-                }
-            },
-            {
-                'name': 'google-auto-tagging',
-                'minConfidence': 80,
-                'maxTags': 10
-            }
-        ]
-        
-        options = UploadFileRequestOptions(
-            use_unique_file_name=False,
-            tags=['abc', 'def'],
-            folder='/testing-python-folder/',
-            is_private_file=False,
-            custom_coordinates='10,10,20,20',
-            response_fields=['tags', 'custom_coordinates', 'is_private_file',
-                             'embedded_metadata', 'custom_metadata'],
-            extensions=extensions,
-            webhook_url='https://webhook.site/c78d617f-33bc-40d9-9e61-608999721e2e',
-            overwrite_file=True,
-            overwrite_ai_tags=False,
-            overwrite_tags=False,
-            overwrite_custom_metadata=True,
-            custom_metadata={'testss': 12},
-        )
-        
-        result = imagekit.upload_file(file='<url|base_64|binary>', # required
-                                      file_name='my_file_name.jpg', # required
-                                      options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that uploaded file's ID
-        print(result.file_id)
-        ```
-        
-        If the upload succeeds, the `result` will be the `UploadFileResult` class.
-        
-        If the upload fails, the custom exception will be thrown with:
-        
-        -   `response_help` for any kind of help
-        -   `response_metadata` with `raw`, `http_status_code` and `headers`
-        -   `message` can be called to get the error message received from ImageKit's servers.
-        
-        ## File Management
-        
-        The SDK provides a simple interface for all
-        the [media APIs mentioned here](https://docs.imagekit.io/api-reference/media-api)
-        to manage your files. This also returns `result`.
-        
-        **1. List & Search Files**
-        
-        Accepts an object specifying the parameters used to list and search files. All parameters specified
-        in
-        the [documentation here](https://docs.imagekit.io/api-reference/media-api/list-and-search-files#list-and-search-file-api)
-        can be passed with the correct values to get the results.
-        
-        ```Python
-        from imagekitio.models.ListAndSearchFileRequestOptions import ListAndSearchFileRequestOptions
-        
-        options = ListAndSearchFileRequestOptions(
-            type='file',
-            sort='ASC_CREATED',
-            path='/',
-            search_query="created_at >= '2d' OR size < '2mb' OR format='png'",
-            file_type='all',
-            limit=5,
-            skip=0,
-            tags='Software, Developer, Engineer',
-        )
-        
-        result = imagekit.list_files(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the first file's ID
-        print(result.list[0].file_id)
-        ```
-        
-        **2. Get File Details**
-        
-        Accepts the file ID and fetches the details as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-details)
-        
-        ```python
-        file_id = "your_file_id"
-        result = imagekit.get_file_details(file_id=file_id)  # file_id required
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        ```
-        
-        **3. Get File Versions**
-        
-        Accepts the file ID and fetches the details as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-versions)
-        
-        ```python
-        file_id = "your_file_id"
-        result = imagekit.get_file_versions(file_id=file_id)  # file_id required
-        
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's version id
-        print(result.list[0].version_info.id)
-        ```
-        
-        **4. Get File Version details**
-        
-        Accepts the `file_id` and `version_id` and fetches the details as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-version-details)
-        
-        ```python
-        result = imagekit.get_file_version_details(
-            file_id='file_id',
-            version_id='version_id'
-        )
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        
-        # print that file's version id
-        print(result.version_info.id)
-        ```
-        
-        **5. Update File Details**
-        
-        Accepts all the parameters as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/update-file-details).
-        The first argument to the `update_file_details()` method is the file ID, and a second argument is an object with the
-        parameters to be
-        updated.
-        
-        ```python
-        from imagekitio.models.UpdateFileRequestOptions import UpdateFileRequestOptions
-        
-        extensions = [
-            {
-                'name': 'remove-bg',
-                'options': {
-                    'add_shadow': True,
-                    'bg_color': 'red'
-                }
-            },
-            {
-                'name': 'google-auto-tagging',
-                'minConfidence': 80,
-                'maxTags': 10
-            }
-        ]
-        
-        options = UpdateFileRequestOptions(
-            remove_ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'],
-            webhook_url='url',
-            extensions=extensions,
-            tags=['tag-1', 'tag-2'],
-            custom_coordinates='10,10,100,100',
-            custom_metadata={'test': 11},
-        )
-        
-        result = imagekit.update_file_details(file_id='62cfd39819ca454d82a07182'
-                , options=options)  # required
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        ```
-        
-        **6. Add tags**
-        
-        Accepts a list of `file_ids` and `tags` as a parameter to be used to add tags. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/add-tags-bulk) can be passed to
-        the `.add_tags()` functions to get the results.
-        
-        ```python
-        result = imagekit.add_tags(file_ids=['file-id-1', 'file-id-2'], tags=['add-tag-1', 'add-tag-2'])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully updated file ids
-        print(result.successfully_updated_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_updated_file_ids[0])
-        ```
-        
-        **7. Remove tags**
-        
-        Accepts a list of `file_ids` and `tags` as a parameter to be used to remove tags. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-tags-bulk) can be passed to
-        the `.remove_tags()` functions to get the results.
-        
-        ```python
-        result = imagekit.remove_tags(file_ids=['file-id-1', 'file-id-2'], tags=['remove-tag-1', 'remove-tag-2'])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully updated file ids
-        print(result.successfully_updated_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_updated_file_ids[0])
-        ```
-        
-        **8. Remove AI tags**
-        
-        Accepts a list of `file_ids` and `ai_tags` as a parameter to remove AI tags. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-aitags-bulk) can be passed to
-        the `.remove_ai_tags()` functions to get the results.
-        
-        ```python
-        result = imagekit.remove_ai_tags(file_ids=['file-id-1', 'file-id-2'], ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully updated file ids
-        print(result.successfully_updated_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_updated_file_ids[0])
-        ```
-        
-        **9. Delete File**
-        
-        Delete a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file). It accepts the file ID of the File that has to be
-        deleted.
-        
-        ```python
-        file_id = "file_id"
-        result = imagekit.delete_file(file_id=file_id)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **10. Delete FileVersion**
-        
-        Delete a file version as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file-version).
-        The method accepts the `file_id` and particular version id of the file that has to be deleted.
-        
-        ```python
-        result = imagekit.delete_file_version(file_id="file_id", version_id="version_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **11. Bulk File Delete by IDs**
-        
-        Delete a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-files-bulk).
-        The method accepts a list of file IDs that have to be deleted.
-        
-        ```python
-        result = imagekit.bulk_file_delete(file_ids=["file_id1", "file_id2"])
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # list successfully deleted file ids
-        print(result.successfully_deleted_file_ids)
-        
-        # print the first file's id
-        print(result.successfully_deleted_file_ids[0])
-        ```
-        
-        **12. Copy file**
-        
-        Copy a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-file).
-        The method accepts `source_file_path`, `destination_path`, and `include_file_versions` of the file that has to be copied.
-        
-        ```python
-        from imagekitio.models.CopyFileRequestOptions import CopyFileRequestOptions
-        
-        options = \
-            CopyFileRequestOptions(source_file_path='/source_file_path.jpg',
-                                   destination_path='/destination_path',
-                                   include_file_versions=True)
-        result = imagekit.copy_file(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **13. Move File**
-        
-        Move a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-file).
-        The method accepts `source_file_path` and `destination_path` of the file that has to be moved.
-        
-        ```python
-        from imagekitio.models.MoveFileRequestOptions import MoveFileRequestOptions
-        
-        options = \
-            MoveFileRequestOptions(source_file_path='/source_file_path.jpg',
-                                   destination_path='/destination_path')
-        result = imagekit.move_file(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **14. Rename File**
-        
-        Rename a file per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/rename-file).
-        The method accepts the `file_path`, `new_file_name`, and `purge_cache` boolean that has to be renamed.
-        
-        ```python
-        from imagekitio.models.RenameFileRequestOptions import RenameFileRequestOptions
-        
-        options = RenameFileRequestOptions(file_path='/file_path.jpg',
-                                           new_file_name='new_file_name.jpg',
-                                           purge_cache=True)
-        result = imagekit.rename_file(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the purge request id
-        print(result.purge_request_id)
-        ```
-        
-        **15. Restore file Version**
-        
-        Restore a file as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/restore-file-version).
-        The method accepts the `file_id` and `version_id` of the file that has to be restored.
-        
-        ```python
-        result = imagekit.restore_file_version(file_id="file_id", version_id="version_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print that file's id
-        print(result.file_id)
-        ```
-        
-        **16. Create Folder**
-        
-        Create a folder per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/create-folder).
-        The method accepts `folder_name` and `parent_folder_path` as options that must be created.
-        
-        ```Python
-        from imagekitio.models.CreateFolderRequestOptions import CreateFolderRequestOptions
-        
-        options = CreateFolderRequestOptions(folder_name='test',
-                                             parent_folder_path='/')
-        result = imagekit.create_folder(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **17. Delete Folder**
-        
-        Delete a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-folder).
-        The method accepts `folder_path` as an option that must be deleted.
-        
-        ```python
-        from imagekitio.models.DeleteFolderRequestOptions import DeleteFolderRequestOptions
-        
-        options = DeleteFolderRequestOptions(folder_path='/test/demo')
-        result = imagekit.delete_folder(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        **18. Copy Folder**
-        
-        Copy a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-folder).
-        The method accepts the `source_folder_path`, `destination_path`, and `include_file_versions` boolean as options that
-        have to be copied.
-        
-        ```python
-        from imagekitio.models.CopyFolderRequestOptions import CopyFolderRequestOptions
-        options = \
-            CopyFolderRequestOptions(source_folder_path='/source_folder_path',
-                                     destination_path='/destination/path',
-                                     include_file_versions=True)
-        result = imagekit.copy_folder(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the job's id
-        print(result.job_id)
-        ```
-        
-        **19. Move Folder**
-        
-        Move a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-folder).
-        The method accepts the `source_folder_path` and `destination_path` of a folder as options that must be moved.
-        
-        ```python
-        from imagekitio.models.MoveFolderRequestOptions import MoveFolderRequestOptions
-        options = \
-            MoveFolderRequestOptions(source_folder_path='/source_folder_path',
-                                     destination_path='/destination_path')
-        result = imagekit.move_folder(options=options)
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the job's id
-        print(result.job_id)
-        ```
-        
-        **20. Get Bulk Job Status**
-        
-        Accepts the `job_id` to get bulk job status as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-move-folder-status).
-        The method takes only jobId.
-        
-        ```python
-        result = imagekit.get_bulk_job_status(job_id="job_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the job's id
-        print(result.job_id)
-        
-        # print the status
-        print(result.status)
-        ```
-        
-        **21. Purge Cache**
-        
-        Programmatically issue an explicit cache request as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache).
-        Accepts the full URL of the File for which the cache has to be cleared.
-        
-        ```python
-        result = imagekit.purge_file_cache(file_url="full_url_of_file")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the purge file cache request id
-        print(result.request_id)
-        ```
-        
-        **22. Purge Cache Status**
-        
-        Get the purge cache request status using the `cache_request_id` returned when a purge cache request gets submitted as per the
-        [API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache-status)
-        
-        ```python
-        result = imagekit.get_purge_file_cache_status(purge_cache_id="cache_request_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the purge file cache status
-        print(result.status)
-        ```
-        
-        **23. Get File Metadata**
-        
-        Accepts the `file_id` and fetches the metadata as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-for-uploaded-media-files)
-        
-        ```python
-        result = imagekit.get_file_metadata(file_id="file_id")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the file metadata fields
-        print(result.width)
-        print(result.exif.image.x_resolution)
-        ```
-        
-        **24. Get File Metadata from remote URL**
-        
-        Accepts the `remote_file_url` and fetches the metadata as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-from-remote-url)
-        
-        ```python
-        result = imagekit.get_remote_file_url_metadata(remote_file_url="remote_file_url")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the file metadata fields
-        print(result.width)
-        print(result.exif.image.x_resolution)
-        ```
-        
-        **25. Create CustomMetaDataFields**
-        
-        Accepts an option specifying the parameters used to create custom metadata fields. All parameters specified in
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field)
-        can be passed as it is with the correct values to get the results.
-        
-        Check for the [allowed values in the schema](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field#allowed-values-in-the-schema-object).
-        
-        **Example:**
-        
-        ```python
-        # Example for the type number
-        
-        from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
-        schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Number,
-                                            min_value=100,
-                                            max_value=200)
-        options = CreateCustomMetadataFieldsRequestOptions(name='test',
-                                                           label='test',
-                                                           schema=schema)
-        result = imagekit.create_custom_metadata_fields(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the id of created custom metadata fields
-        print(result.id)
-        
-        # print the schema's type of created custom metadata fields
-        print(result.schema.type)
-        
-        ```
-        
-        ```python
-        # MultiSelect type Example
-        
-        from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
-        
-        schema = \
-            CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.MultiSelect,
-                                       is_value_required=True,
-                                       default_value=['small', 30, True],
-                                       select_options=[
-                                            'small',
-                                            'medium',
-                                            'large',
-                                            30,
-                                            40,
-                                            True,
-                                        ])
-        options = \
-            CreateCustomMetadataFieldsRequestOptions(name='test-MultiSelect',
-                label='test-MultiSelect', schema=schema)
-        result = imagekit.create_custom_metadata_fields(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the name of created custom metadata fields
-        print(result.name)
-        
-        # print the schema's select options of created custom metadata fields
-        print(result.schema.select_options)
-        
-        ```
-        
-        ```python
-        # Date type Example
-        
-        from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
-        
-        schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Date,
-                                            min_value='2022-11-29T10:11:10+00:00',
-                                            max_value='2022-11-30T10:11:10+00:00')
-        options = CreateCustomMetadataFieldsRequestOptions(name='test-date',
-                                                           label='test-date',
-                                                           schema=schema)
-        result = imagekit.create_custom_metadata_fields(options=options)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the label of created custom metadata fields
-        print(result.label)
-        
-        # print the schema's min value of created custom metadata fields
-        print(result.schema.min_value)
-        
-        ```
-        
-        **26. Get CustomMetaDataFields**
-        
-        Accepts the `include_deleted` boolean as the initial parameter and fetches the metadata as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/get-custom-metadata-field)
-        .
-        
-        ```python
-        result = imagekit.get_custom_metadata_fields()  # in this case, it will consider includeDeleted as a False
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the first customMetadataField's id
-        print(result.list[0].id)
-        
-        # print the first customMetadataField schema's type
-        print(result.list[0].schema.type)
-        ```
-        
-        ```python
-        result = imagekit.get_custom_metadata_fields(include_deleted=True)
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the first customMetadataField's name
-        print(result.list[0].name)
-        
-        # print the first customMetadataField schema's default value
-        print(result.list[0].schema.default_value)
-        ```
-        
-        **27. Update CustomMetaDataFields**
-        
-        Accepts a `field_id` and options for specifying the parameters to be used to edit custom metadata fields
-        as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/update-custom-metadata-field)
-        .
-        
-        ```python
-        
-        from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
-        from imagekitio.models.UpdateCustomMetadataFieldsRequestOptions import UpdateCustomMetadataFieldsRequestOptions
-        
-        schema = CustomMetadataFieldsSchema(min_value=100, max_value=200)
-        options = UpdateCustomMetadataFieldsRequestOptions(
-            label='test-update',
-            schema=schema
-        )
-        result = imagekit.update_custom_metadata_fields(
-            field_id='id_of_custom_metadata_field',
-            options=options
-        )
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        
-        # print the label of updated custom metadata fields
-        print(result.label)
-        
-        # print the schema's min value of updated custom metadata fields
-        print(result.schema.min_value)
-        ```
-        
-        **28. Delete CustomMetaDataFields**
-        
-        Accepts the id to delete the custom metadata fields as per
-        the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/delete-custom-metadata-field)
-        .
-        
-        ```python
-        result = imagekit.delete_custom_metadata_field(field_id="id_of_custom_metadata_field")
-        
-        # Final Result
-        print(result)
-        
-        # Raw Response
-        print(result.response_metadata.raw)
-        ```
-        
-        ## Utility functions
-        
-        We have included the following commonly used utility functions in this package.
-        
-        **Authentication parameter generation**
-        
-        Suppose one wants to implement client-side file upload. In that case, one will need a token, expiry timestamp, and a valid signature for that upload. The SDK provides a simple method that one can use in their code to generate these authentication parameters.
-        
-        <em>Note: Any client-side code should never expose The Private API Key. One must always generate these authentications parameters on the server-side</em>
-        
-        authentication
-        
-        `authentication_parameters = imagekit.get_authentication_parameters(token, expire)`
-        
-        Returns
-        
-        ```python
-        {
-            "token": "unique_token",
-            "expire": "valid_expiry_timestamp",
-            "signature": "generated_signature"
-        }
-        ```
-        
-        Both the `token` and `expire` parameters are optional. If not specified, the SDK uses the UUID to generate a random token and internally generates a valid expiry timestamp. The `token` and `expire` used to generate `signature` is part of a response returned by the server.
-        
-        **Distance calculation between two `pHash` values**
-        
-        Perceptual hashing allows you to construct a has value that uniquely identifies an input image based on the contents
-        of an image. [imagekit.io metadata API](https://docs.imagekit.io/api-reference/metadata-api) returns the `pHash`
-        value of an image in the response. You can use this value
-        to [find a duplicate or similar image](https://docs.imagekit.io/api-reference/metadata-api#using-phash-to-find-similar-or-duplicate-images)
-        by calculating the distance between the two images.
-        
-        This SDK exposes the `phash_distance` function to calculate the distance between two `pHash` values. It accepts two `pHash`
-        hexadecimal
-        strings and returns a numeric value indicative of the difference between the two images.
-        
-        ```python
-        def calculate_distance():
-            # fetch metadata of two uploaded image files
-            ...
-            # extract pHash strings from both: say 'first_hash' and 'second_hash'
-            ...
-            # calculate the distance between them:
-        
-            distance = imagekit.phash_distance(first_hash, second_hash)
-            return distance
-        
-        ```
-        
-        **Distance calculation examples**
-        
-        ```Python
-        imagekit.phash_distance('f06830ca9f1e3e90', 'f06830ca9f1e3e90')
-        # output: 0 (same image)
-        
-        imagekit.phash_distance('2d5ad3936d2e015b', '2d6ed293db36a4fb')
-        # output: 17 (similar images)
-        
-        imagekit.phash_distance('a4a65595ac94518b', '7838873e791f8400')
-        # output: 37 (dissimilar images)
-        ```
-        
-        **HTTP response metadata of Internal API**
-        
-        HTTP response metadata of the internal API call can be accessed using the \_response_metadata on the Result object.
-        Example:
-        
-        ```Python
-        result = imagekit.upload_file(
-            file="<url|base_64|binary>",
-            file_name="my_file_name.jpg",
-        )
-        
-        # Final Result
-        print(result)
-        print(result.response_metadata.raw)
-        print(result.response_metadata.http_status_code)
-        print(result.response_metadata.headers)
-        ```
-        
-        ### Sample Code Instruction
-        
-        To run `sample` code go to the code samples here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python and run.
-        
-        ```shell
-        python sample.py
-        ```
-        
-        ## Handling errors
-        
-        Catch and respond to invalid data, internal problems, and more.
-        
-        ImageKit Python SDK raises exceptions for many reasons, such as not found, invalid parameters, authentication, and
-        internal server errors. Therefore, we recommend writing code that gracefully handles all possible API exceptions.
-        
-        #### Example:
-        
-        ```Python
-        from imagekitio.exceptions.BadRequestException import BadRequestException
-        from imagekitio.exceptions.UnauthorizedException import UnauthorizedException
-        from imagekitio.exceptions.ForbiddenException import ForbiddenException
-        from imagekitio.exceptions.TooManyRequestsException import TooManyRequestsException
-        from imagekitio.exceptions.InternalServerException import InternalServerException
-        from imagekitio.exceptions.PartialSuccessException import PartialSuccessException
-        from imagekitio.exceptions.NotFoundException import NotFoundException
-        from imagekitio.exceptions.UnknownException import UnknownException
-        
-        try:
-        
-            # Use ImageKit's SDK to make requests...
-            print('Run image kit api')
-        except BadRequestException, e:
-            # Missing or Invalid parameters were supplied to Imagekit.io's API
-            print('Status is: ' + e.response_metadata.http_status_code)
-            print('Message is: ' + e.message)
-            print('Headers are: ' + e.response_metadata.headers)
-            print('Raw body is: ' + e.response_metadata.raw)
-        except UnauthorizedException, e:
-            print(e)
-        except ForbiddenException, e:
-            # No valid API key was provided.
-            print(e)
-        except TooManyRequestsException, e:
-            # Can be for the following reasons:
-            # ImageKit could not authenticate your account with the keys provided.
-            # An expired key (public or private) was used with the request.
-            # The account is disabled.
-            # If you use the upload API, the total storage limit (or upload limit) is exceeded.
-            print(e)
-        except InternalServerException, e:
-            # Too many requests made to the API too quickly
-            print(e)
-        except PartialSuccessException, e:
-            # Something went wrong with ImageKit.io API.
-            print(e)
-        except NotFoundException, e:
-            # Error cases on partial success.
-            print(e)
-        except UnknownException, e:
-            # If any of the field or parameter is not found in the data
-            print(e)
-        
-        # Something else happened, which can be unrelated to ImageKit; the reason will be indicated in the message field
-        ```
-        
-        ## Development
-        
-        ### Tests
-        
-        Tests are powered by [Tox](https://tox.wiki/en/latest/).
-        
-        ```bash
-        $ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
-        $ pip install tox
-        $ tox
-        ```
-        
-        ### Sample
-        
-        #### Get & Install local ImageKit Python SDK
-        
-        ```bash
-        $ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
-        $ pip install -e .
-        ```
-        
-        #### Get samples
-        
-        To integrate ImageKit Samples in the Python, the code samples covered here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python.
-        
-        Open the `python/sample.py` file and replace placeholder credentials with actual values. You can get the value of [URL-endpoint](https://imagekit.io/dashboard#url-endpoints) from your ImageKit dashboard. API keys can be obtained from the [developer](https://imagekit.io/dashboard/developer/api-keys) section in your ImageKit dashboard.
-        
-        In the `python/sample.py` file, set the following parameters for authentication:
-        
-        ```python
-        from imagekitio import ImageKit
-        imagekit = ImageKit(
-            private_key='your private_key',
-            public_key='your public_key',
-            url_endpoint = 'your url_endpoint'
-        )
-        ```
-        
-        To install dependencies that are in the `python/requirements.txt` file, can fire this command to install them:
-        
-        ```shell
-        pip install -r python/requirements.txt
-        ```
-        
-        Now run `python/sample.py`. If you are using CLI Tool (Terminal/Command prompt), open the project in CLI and execute it.
-        
-        ```shell
-        # if not installed already
-        pip install imagekitio
-        
-        # if installing local sdk
-        pip install -e <path_to_local_sdk>
-        
-        # to run sample.py file
-        python3 python/sample.py
-        ```
-        
-        ## Support
-        
-        For any feedback or to report any issues or general implementation support, please reach out
-        to [support@imagekit.io](https://github.com/imagekit-developer/imagekit-python)
-        
-        ## Links
-        
-        -   [Documentation](https://docs.imagekit.io/)
-        
-        -   [Main Website](https://imagekit.io/)
-        
-        ## License
-        
-        Released under the MIT license.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[<img width="250" alt="ImageKit.io" src="https://raw.githubusercontent.com/imagekit-developer/imagekit-javascript/master/assets/imagekit-light-logo.svg"/>](https://imagekit.io)
+
+# ImageKit.io Python SDK
+
+[![Python CI](https://github.com/imagekit-developer/imagekit-python/workflows/Python%20CI/badge.svg)](https://github.com/imagekit-developer/imagekit-python/)
+[![imagekitio](https://img.shields.io/pypi/v/imagekitio.svg)](https://pypi.org/project/imagekitio)
+[![codecov](https://codecov.io/gh/imagekit-developer/imagekit-python/branch/master/graph/badge.svg?token=CwKWqBIlCu)](https://codecov.io/gh/imagekit-developer/imagekit-python)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Twitter Follow](https://img.shields.io/twitter/follow/imagekitio?label=Follow&style=social)](https://twitter.com/ImagekitIo)
+
+Python SDK for [ImageKit](https://imagekit.io/) implements the new APIs and interface for different file operations.
+
+ImageKit is complete media storage, optimization, and transformation solution that comes with an [image and video CDN](https://imagekit.io/features/imagekit-infrastructure). It can be integrated with your existing infrastructure - storage like AWS S3, web servers, your CDN, and custom domain names, allowing you to deliver optimized images in minutes with minimal code changes.
+
+Supported Python Versions: >=3.6
+
+Table of contents -
+
+-   [Installation](#installation)
+-   [Initialization](#initialization)
+-   [Change Log](#change-log)
+-   [Usage](#usage)
+    -   [URL Generation](#url-generation)
+    -   [File Upload](#file-upload)
+    -   [File Management](#file-management)
+    -   [Utility Functions](#utility-functions)
+-   [Handling errors](#handling-errors)
+-   [Development](#development)
+    -   [Tests](#tests)
+    -   [Sample](#sample)
+-   [Support](#support)
+-   [Links](#links)
+
+## Installation
+
+Go to your terminal and type the following command.
+
+```bash
+pip install imagekitio
+```
+
+## Initialization
+
+```python
+from imagekitio import ImageKit
+
+imagekit = ImageKit(
+    private_key='your_private_key',
+    public_key='your_public_key',
+    url_endpoint='your_url_endpoint'
+)
+```
+
+## Change log
+
+This document presents a list of changes that break the existing functionality of previous versions. We try to minimize these disruptions, but they are sometimes unavoidable, especially in significant updates. Therefore, versions are marked semantically and tagged as major upgrades whenever such breaking changes occur.
+
+### Breaking History:
+
+Changes from `2.2.8 -> 3.0.0` are listed below
+
+1. Throw an Error:
+
+**What changed**
+
+-   Before the upgrade, an `error` dict was coming in the return object of any function call. Now, SDK throws an exception in case of an error.
+
+**Who is affected?**
+
+-   This affects any development in your software that calls APIs from ImageKit IO and handles errors based on what's returned.
+
+**How should I update my code?**
+
+-   To avoid failures in an application, you could handle errors as [documented here](#handling-errors)
+
+# Usage
+
+You can use this Python SDK for three different kinds of methods:
+
+-   [URL Generation](#url-generation)
+-   [File Upload](#file-upload)
+-   [File Management](#file-management)
+-   [Utility Functions](#utility-functions)
+
+## URL Generation
+
+**1. Using Image path and endpoint (hostname)**
+
+This method allows you to create a URL using the relative file path where the image exists and the URL
+endpoint(url_endpoint) you want to use to access the image. You can refer to the documentation
+[here](https://docs.imagekit.io/integration/url-endpoints) to read more about URL endpoints
+in ImageKit and the section about [image origins](https://docs.imagekit.io/integration/configure-origin) to understand
+about paths with different kinds of origins.
+
+The file can be an image, video, or any other static file supported by ImageKit.
+
+```python
+imagekit_url = imagekit.url({
+    "path": "/default-image.jpg",
+    "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
+    "transformation": [{
+        "height": "300",
+        "width": "400",
+        "raw": "ar-4-3,q-40"
+    }],
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/endpoint/tr:h-300,w-400,ar-4-3,q-40/default-image.jpg
+```
+
+**2. Using full image URL**
+
+This method allows you to add transformation parameters to an absolute URL using the `src` parameter. This method should be
+used if you have the complete image URL stored in your database.
+
+```python
+image_url = imagekit.url({
+    "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
+    "transformation": [{
+        "height": "300",
+        "width": "400",
+        "raw": "ar-4-3,q-40"
+    }]
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%2Car-4-3%2Cq-40
+```
+
+The `.url()` method accepts the following parameters.
+
+| Option                  | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| :---------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| url_endpoint            | Optional. The prepended base URL before the path of the image. If not specified, the URL Endpoint specified during SDK initialization gets used. For example, https://ik.imagekit.io/your_imagekit_id/endpoint/                                                                                                                                                                                                                                                                             |
+| path                    | Conditional. A path at which the image exists. For example, `/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                                                                                   |
+| src                     | Conditional. Complete URL of an image already mapped to ImageKit. For example, `https://ik.imagekit.io/your_imagekit_id/endpoint/path/to/image.jpg`. Specify a `path` or `src` parameter for URL generation.                                                                                                                                                                                                                                                                                |
+| transformation          | Optional. Specify an array of objects with name and the value in key-value pair to apply transformation params in the URL. Append different steps of a [chained transformation](https://docs.imagekit.io/features/image-transformations/chained-transformations) as different objects of the array. This document includes a complete list of supported transformations in the SDK with some examples. If one uses an unspecified transformation name, it gets applied as it is in the URL. |
+| transformation_position | Optional. The default value is `path`, which places the transformation string as a path parameter in the URL. One can also specify it as a query, which adds the transformation string as the query parameter `tr` in the URL. Suppose one uses the `src` parameter to create the URL. In that case, the transformation string is always a query parameter.                                                                                                                                 |
+| query_parameters        | Optional. These are the other query parameters that one wants to add to the final URL. These can be any query parameters and are not necessarily related to ImageKit. Especially useful if one wants to add some versioning parameter to their URLs.                                                                                                                                                                                                                                        |
+| signed                  | Optional. Boolean. The default is `false`. If set to `true`, the SDK generates a signed image URL adding the image signature to the image URL. One can only use this if they create the URL with the `url_endpoint` and `path` parameters, not the `src` parameter.                                                                                                                                                                                                                         |
+| expire_seconds          | Optional. Integer. Used along with the `signed` parameter to specify the time in seconds from `now` when the URL should expire. If specified, the URL contains the expiry timestamp, and the image signature is modified accordingly.                                                                                                                                                                                                                                                       |
+
+## Examples of generating URLs
+
+**1. Chained Transformations as a query parameter**
+
+```python
+image_url = imagekit.url({
+    "path": "/default-image.jpg",
+    "url_endpoint": "https://ik.imagekit.io/your_imagekit_id/endpoint/",
+    "transformation": [
+        {
+            "height": "300",
+            "width": "400"
+        },
+        {
+            "rotation": 90
+        }
+    ],
+    "transformation_position": "query"
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=h-300%2Cw-400%3Art-90
+```
+
+**2. Sharpening, contrast transform and progressive JPG image**
+
+Add transformations like [Sharpening](https://docs.imagekit.io/features/image-transformations/image-enhancement-and-color-manipulation) to the URL with or without any other value. To use such transforms without specifying a value, set it as "-" in the transformation object. Otherwise, use the value that one wants to add to this transformation.
+
+```python
+image_url = imagekit.url({
+    "src": "https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg",
+    "transformation": [{
+        "format": "jpg",
+        "progressive": "true",
+        "effect_sharpen": "-",
+        "effect_contrast": "1"
+    }]
+})
+```
+
+Sample Result URL -
+
+```
+# Note that because the `src` parameter is in effect, the transformation string gets added as a query parameter `tr`
+
+https://ik.imagekit.io/your_imagekit_id/endpoint/default-image.jpg?tr=f-jpg%2Cpr-true%2Ce-sharpen%2Ce-contrast-1
+```
+
+**3. Signed URL that expires in 300 seconds with the default URL endpoint and other query parameters**
+
+```python
+image_url = imagekit.url({
+    "path": "/default-image.jpg",
+    "query_parameters": {
+        "p1": "123",
+        "p2": "345"
+    },
+    "transformation": [{
+        "height": "300",
+        "width": "400"
+    }],
+    "signed": True,
+    "expire_seconds": 300
+})
+```
+
+Sample Result URL -
+
+```
+https://ik.imagekit.io/your_imagekit_id/tr:h-300,w-400/default-image.jpg?p1=123&p2=345&ik-t=1658899345&ik-s=8f03aca28432d4e87f697a48143efb4497bbed9e
+```
+
+**List of transformations**
+
+The complete list of transformations supported and their usage in ImageKit is available [here](https://docs.imagekit.io/features/image-transformations/resize-crop-and-other-transformations).
+The SDK gives a name to each transformation parameter, making the code simpler, more straightforward, and readable. If a transformation is supported in ImageKit, though it cannot be found in the table below, then use the transformation code from ImageKit docs as the name when using the `URL` function.
+
+If you want to generate transformations in your application and add them to the URL as it is, use the raw parameter.
+
+| Supported Transformation Name | Translates to parameter         |
+| ----------------------------- | ------------------------------- |
+| height                        | h                               |
+| width                         | w                               |
+| aspect_ratio                  | ar                              |
+| quality                       | q                               |
+| crop                          | c                               |
+| crop_mode                     | cm                              |
+| x                             | x                               |
+| y                             | y                               |
+| focus                         | fo                              |
+| format                        | f                               |
+| radius                        | r                               |
+| background                    | bg                              |
+| border                        | b                               |
+| rotation                      | rt                              |
+| blur                          | bl                              |
+| named                         | n                               |
+| overlay_x                     | ox                              |
+| overlay_y                     | oy                              |
+| overlay_focus                 | ofo                             |
+| overlay_height                | oh                              |
+| overlay_width                 | ow                              |
+| overlay_image                 | oi                              |
+| overlay_image_trim            | oit                             |
+| overlay_image_aspect_ratio    | oiar                            |
+| overlay_image_background      | oibg                            |
+| overlay_image_border          | oib                             |
+| overlay_image_dpr             | oidpr                           |
+| overlay_image_quality         | oiq                             |
+| overlay_image_cropping        | oic                             |
+| overlay_image_focus           | oifo                            |
+| overlay_text                  | ot                              |
+| overlay_text_font_size        | ots                             |
+| overlay_text_font_family      | otf                             |
+| overlay_text_color            | otc                             |
+| overlay_text_transparency     | oa                              |
+| overlay_alpha                 | oa                              |
+| overlay_text_typography       | ott                             |
+| overlay_background            | obg                             |
+| overlay_text_encoded          | ote                             |
+| overlay_text_width            | otw                             |
+| overlay_text_background       | otbg                            |
+| overlay_text_padding          | otp                             |
+| overlay_text_inner_alignment  | otia                            |
+| overlay_radius                | or                              |
+| progressive                   | pr                              |
+| lossless                      | lo                              |
+| trim                          | t                               |
+| metadata                      | md                              |
+| color_profile                 | cp                              |
+| default_image                 | di                              |
+| dpr                           | dpr                             |
+| effect_sharpen                | e-sharpen                       |
+| effect_usm                    | e-usm                           |
+| effect_contrast               | e-contrast                      |
+| effect_gray                   | e-grayscale                     |
+| original                      | orig                            |
+| raw                           | replaced by the parameter value |
+
+## File Upload
+
+The SDK provides a simple interface using the `.upload_file()` method to upload files to the ImageKit Media library. It
+accepts all the parameters supported by
+the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload).
+
+The `upload_file()` method requires at least the `file` as (URL/Base64/Binary) and the `file_name` parameter to upload a
+file. The method returns a dict data in case of success, or it will throw a custom exception in case of failure.
+Use the `options` parameter to pass other parameters supported by
+the [ImageKit Upload API](https://docs.imagekit.io/api-reference/upload-file-api/server-side-file-upload). Use the same
+parameter name as specified in the upload API documentation.
+
+Simple usage
+
+```python
+from imagekitio.models.UploadFileRequestOptions import UploadFileRequestOptions
+
+extensions = [
+    {
+        'name': 'remove-bg',
+        'options': {
+            'add_shadow': True,
+            'bg_color': 'pink'
+        }
+    },
+    {
+        'name': 'google-auto-tagging',
+        'minConfidence': 80,
+        'maxTags': 10
+    }
+]
+
+options = UploadFileRequestOptions(
+    use_unique_file_name=False,
+    tags=['abc', 'def'],
+    folder='/testing-python-folder/',
+    is_private_file=False,
+    custom_coordinates='10,10,20,20',
+    response_fields=['tags', 'custom_coordinates', 'is_private_file',
+                     'embedded_metadata', 'custom_metadata'],
+    extensions=extensions,
+    webhook_url='https://webhook.site/c78d617f-33bc-40d9-9e61-608999721e2e',
+    overwrite_file=True,
+    overwrite_ai_tags=False,
+    overwrite_tags=False,
+    overwrite_custom_metadata=True,
+    custom_metadata={'testss': 12},
+)
+
+result = imagekit.upload_file(file='<url|base_64|binary>', # required
+                              file_name='my_file_name.jpg', # required
+                              options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that uploaded file's ID
+print(result.file_id)
+```
+
+If the upload succeeds, the `result` will be the `UploadFileResult` class.
+
+If the upload fails, the custom exception will be thrown with:
+
+-   `response_help` for any kind of help
+-   `response_metadata` with `raw`, `http_status_code` and `headers`
+-   `message` can be called to get the error message received from ImageKit's servers.
+
+## File Management
+
+The SDK provides a simple interface for all
+the [media APIs mentioned here](https://docs.imagekit.io/api-reference/media-api)
+to manage your files. This also returns `result`.
+
+**1. List & Search Files**
+
+Accepts an object specifying the parameters used to list and search files. All parameters specified
+in
+the [documentation here](https://docs.imagekit.io/api-reference/media-api/list-and-search-files#list-and-search-file-api)
+can be passed with the correct values to get the results.
+
+```Python
+from imagekitio.models.ListAndSearchFileRequestOptions import ListAndSearchFileRequestOptions
+
+options = ListAndSearchFileRequestOptions(
+    type='file',
+    sort='ASC_CREATED',
+    path='/',
+    search_query="created_at >= '2d' OR size < '2mb' OR format='png'",
+    file_type='all',
+    limit=5,
+    skip=0,
+    tags='Software, Developer, Engineer',
+)
+
+result = imagekit.list_files(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the first file's ID
+print(result.list[0].file_id)
+```
+
+**2. Get File Details**
+
+Accepts the file ID and fetches the details as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-details)
+
+```python
+file_id = "your_file_id"
+result = imagekit.get_file_details(file_id=file_id)  # file_id required
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+```
+
+**3. Get File Versions**
+
+Accepts the file ID and fetches the details as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-versions)
+
+```python
+file_id = "your_file_id"
+result = imagekit.get_file_versions(file_id=file_id)  # file_id required
+
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's version id
+print(result.list[0].version_info.id)
+```
+
+**4. Get File Version details**
+
+Accepts the `file_id` and `version_id` and fetches the details as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/get-file-version-details)
+
+```python
+result = imagekit.get_file_version_details(
+    file_id='file_id',
+    version_id='version_id'
+)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+
+# print that file's version id
+print(result.version_info.id)
+```
+
+**5. Update File Details**
+
+Accepts all the parameters as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/update-file-details).
+The first argument to the `update_file_details()` method is the file ID, and a second argument is an object with the
+parameters to be
+updated.
+
+```python
+from imagekitio.models.UpdateFileRequestOptions import UpdateFileRequestOptions
+
+extensions = [
+    {
+        'name': 'remove-bg',
+        'options': {
+            'add_shadow': True,
+            'bg_color': 'red'
+        }
+    },
+    {
+        'name': 'google-auto-tagging',
+        'minConfidence': 80,
+        'maxTags': 10
+    }
+]
+
+options = UpdateFileRequestOptions(
+    remove_ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'],
+    webhook_url='url',
+    extensions=extensions,
+    tags=['tag-1', 'tag-2'],
+    custom_coordinates='10,10,100,100',
+    custom_metadata={'test': 11},
+)
+
+result = imagekit.update_file_details(file_id='62cfd39819ca454d82a07182'
+        , options=options)  # required
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+```
+
+**6. Add tags**
+
+Accepts a list of `file_ids` and `tags` as a parameter to be used to add tags. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/add-tags-bulk) can be passed to
+the `.add_tags()` functions to get the results.
+
+```python
+result = imagekit.add_tags(file_ids=['file-id-1', 'file-id-2'], tags=['add-tag-1', 'add-tag-2'])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully updated file ids
+print(result.successfully_updated_file_ids)
+
+# print the first file's id
+print(result.successfully_updated_file_ids[0])
+```
+
+**7. Remove tags**
+
+Accepts a list of `file_ids` and `tags` as a parameter to be used to remove tags. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-tags-bulk) can be passed to
+the `.remove_tags()` functions to get the results.
+
+```python
+result = imagekit.remove_tags(file_ids=['file-id-1', 'file-id-2'], tags=['remove-tag-1', 'remove-tag-2'])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully updated file ids
+print(result.successfully_updated_file_ids)
+
+# print the first file's id
+print(result.successfully_updated_file_ids[0])
+```
+
+**8. Remove AI tags**
+
+Accepts a list of `file_ids` and `ai_tags` as a parameter to remove AI tags. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/remove-aitags-bulk) can be passed to
+the `.remove_ai_tags()` functions to get the results.
+
+```python
+result = imagekit.remove_ai_tags(file_ids=['file-id-1', 'file-id-2'], ai_tags=['remove-ai-tag-1', 'remove-ai-tag-2'])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully updated file ids
+print(result.successfully_updated_file_ids)
+
+# print the first file's id
+print(result.successfully_updated_file_ids[0])
+```
+
+**9. Delete File**
+
+Delete a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file). It accepts the file ID of the File that has to be
+deleted.
+
+```python
+file_id = "file_id"
+result = imagekit.delete_file(file_id=file_id)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**10. Delete FileVersion**
+
+Delete a file version as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-file-version).
+The method accepts the `file_id` and particular version id of the file that has to be deleted.
+
+```python
+result = imagekit.delete_file_version(file_id="file_id", version_id="version_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**11. Bulk File Delete by IDs**
+
+Delete a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-files-bulk).
+The method accepts a list of file IDs that have to be deleted.
+
+```python
+result = imagekit.bulk_file_delete(file_ids=["file_id1", "file_id2"])
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# list successfully deleted file ids
+print(result.successfully_deleted_file_ids)
+
+# print the first file's id
+print(result.successfully_deleted_file_ids[0])
+```
+
+**12. Copy file**
+
+Copy a file according to the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-file).
+The method accepts `source_file_path`, `destination_path`, and `include_file_versions` of the file that has to be copied.
+
+```python
+from imagekitio.models.CopyFileRequestOptions import CopyFileRequestOptions
+
+options = \
+    CopyFileRequestOptions(source_file_path='/source_file_path.jpg',
+                           destination_path='/destination_path',
+                           include_file_versions=True)
+result = imagekit.copy_file(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**13. Move File**
+
+Move a file as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-file).
+The method accepts `source_file_path` and `destination_path` of the file that has to be moved.
+
+```python
+from imagekitio.models.MoveFileRequestOptions import MoveFileRequestOptions
+
+options = \
+    MoveFileRequestOptions(source_file_path='/source_file_path.jpg',
+                           destination_path='/destination_path')
+result = imagekit.move_file(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**14. Rename File**
+
+Rename a file per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/rename-file).
+The method accepts the `file_path`, `new_file_name`, and `purge_cache` boolean that has to be renamed.
+
+```python
+from imagekitio.models.RenameFileRequestOptions import RenameFileRequestOptions
+
+options = RenameFileRequestOptions(file_path='/file_path.jpg',
+                                   new_file_name='new_file_name.jpg',
+                                   purge_cache=True)
+result = imagekit.rename_file(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the purge request id
+print(result.purge_request_id)
+```
+
+**15. Restore file Version**
+
+Restore a file as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/restore-file-version).
+The method accepts the `file_id` and `version_id` of the file that has to be restored.
+
+```python
+result = imagekit.restore_file_version(file_id="file_id", version_id="version_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print that file's id
+print(result.file_id)
+```
+
+**16. Create Folder**
+
+Create a folder per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/create-folder).
+The method accepts `folder_name` and `parent_folder_path` as options that must be created.
+
+```Python
+from imagekitio.models.CreateFolderRequestOptions import CreateFolderRequestOptions
+
+options = CreateFolderRequestOptions(folder_name='test',
+                                     parent_folder_path='/')
+result = imagekit.create_folder(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**17. Delete Folder**
+
+Delete a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/delete-folder).
+The method accepts `folder_path` as an option that must be deleted.
+
+```python
+from imagekitio.models.DeleteFolderRequestOptions import DeleteFolderRequestOptions
+
+options = DeleteFolderRequestOptions(folder_path='/test/demo')
+result = imagekit.delete_folder(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+**18. Copy Folder**
+
+Copy a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-folder).
+The method accepts the `source_folder_path`, `destination_path`, and `include_file_versions` boolean as options that
+have to be copied.
+
+```python
+from imagekitio.models.CopyFolderRequestOptions import CopyFolderRequestOptions
+options = \
+    CopyFolderRequestOptions(source_folder_path='/source_folder_path',
+                             destination_path='/destination/path',
+                             include_file_versions=True)
+result = imagekit.copy_folder(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the job's id
+print(result.job_id)
+```
+
+**19. Move Folder**
+
+Move a folder as per the [API documentation here](https://docs.imagekit.io/api-reference/media-api/move-folder).
+The method accepts the `source_folder_path` and `destination_path` of a folder as options that must be moved.
+
+```python
+from imagekitio.models.MoveFolderRequestOptions import MoveFolderRequestOptions
+options = \
+    MoveFolderRequestOptions(source_folder_path='/source_folder_path',
+                             destination_path='/destination_path')
+result = imagekit.move_folder(options=options)
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the job's id
+print(result.job_id)
+```
+
+**20. Get Bulk Job Status**
+
+Accepts the `job_id` to get bulk job status as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/copy-move-folder-status).
+The method takes only jobId.
+
+```python
+result = imagekit.get_bulk_job_status(job_id="job_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the job's id
+print(result.job_id)
+
+# print the status
+print(result.status)
+```
+
+**21. Purge Cache**
+
+Programmatically issue an explicit cache request as per
+the [API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache).
+Accepts the full URL of the File for which the cache has to be cleared.
+
+```python
+result = imagekit.purge_file_cache(file_url="full_url_of_file")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the purge file cache request id
+print(result.request_id)
+```
+
+**22. Purge Cache Status**
+
+Get the purge cache request status using the `cache_request_id` returned when a purge cache request gets submitted as per the
+[API documentation here](https://docs.imagekit.io/api-reference/media-api/purge-cache-status)
+
+```python
+result = imagekit.get_purge_file_cache_status(purge_cache_id="cache_request_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the purge file cache status
+print(result.status)
+```
+
+**23. Get File Metadata**
+
+Accepts the `file_id` and fetches the metadata as per
+the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-for-uploaded-media-files)
+
+```python
+result = imagekit.get_file_metadata(file_id="file_id")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the file metadata fields
+print(result.width)
+print(result.exif.image.x_resolution)
+```
+
+**24. Get File Metadata from remote URL**
+
+Accepts the `remote_file_url` and fetches the metadata as per
+the [API documentation here](https://docs.imagekit.io/api-reference/metadata-api/get-image-metadata-from-remote-url)
+
+```python
+result = imagekit.get_remote_file_url_metadata(remote_file_url="remote_file_url")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the file metadata fields
+print(result.width)
+print(result.exif.image.x_resolution)
+```
+
+**25. Create CustomMetaDataFields**
+
+Accepts an option specifying the parameters used to create custom metadata fields. All parameters specified in
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field)
+can be passed as it is with the correct values to get the results.
+
+Check for the [allowed values in the schema](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/create-custom-metadata-field#allowed-values-in-the-schema-object).
+
+**Example:**
+
+```python
+# Example for the type number
+
+from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
+schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Number,
+                                    min_value=100,
+                                    max_value=200)
+options = CreateCustomMetadataFieldsRequestOptions(name='test',
+                                                   label='test',
+                                                   schema=schema)
+result = imagekit.create_custom_metadata_fields(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the id of created custom metadata fields
+print(result.id)
+
+# print the schema's type of created custom metadata fields
+print(result.schema.type)
+
+```
+
+```python
+# MultiSelect type Example
+
+from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
+
+schema = \
+    CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.MultiSelect,
+                               is_value_required=True,
+                               default_value=['small', 30, True],
+                               select_options=[
+                                    'small',
+                                    'medium',
+                                    'large',
+                                    30,
+                                    40,
+                                    True,
+                                ])
+options = \
+    CreateCustomMetadataFieldsRequestOptions(name='test-MultiSelect',
+        label='test-MultiSelect', schema=schema)
+result = imagekit.create_custom_metadata_fields(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the name of created custom metadata fields
+print(result.name)
+
+# print the schema's select options of created custom metadata fields
+print(result.schema.select_options)
+
+```
+
+```python
+# Date type Example
+
+from imagekitio.models.CreateCustomMetadataFieldsRequestOptions import CreateCustomMetadataFieldsRequestOptions
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.CustomMetaDataTypeEnum import CustomMetaDataTypeEnum
+
+schema = CustomMetadataFieldsSchema(type=CustomMetaDataTypeEnum.Date,
+                                    min_value='2022-11-29T10:11:10+00:00',
+                                    max_value='2022-11-30T10:11:10+00:00')
+options = CreateCustomMetadataFieldsRequestOptions(name='test-date',
+                                                   label='test-date',
+                                                   schema=schema)
+result = imagekit.create_custom_metadata_fields(options=options)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the label of created custom metadata fields
+print(result.label)
+
+# print the schema's min value of created custom metadata fields
+print(result.schema.min_value)
+
+```
+
+**26. Get CustomMetaDataFields**
+
+Accepts the `include_deleted` boolean as the initial parameter and fetches the metadata as per
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/get-custom-metadata-field)
+.
+
+```python
+result = imagekit.get_custom_metadata_fields()  # in this case, it will consider includeDeleted as a False
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the first customMetadataField's id
+print(result.list[0].id)
+
+# print the first customMetadataField schema's type
+print(result.list[0].schema.type)
+```
+
+```python
+result = imagekit.get_custom_metadata_fields(include_deleted=True)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the first customMetadataField's name
+print(result.list[0].name)
+
+# print the first customMetadataField schema's default value
+print(result.list[0].schema.default_value)
+```
+
+**27. Update CustomMetaDataFields**
+
+Accepts a `field_id` and options for specifying the parameters to be used to edit custom metadata fields
+as per
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/update-custom-metadata-field)
+.
+
+```python
+
+from imagekitio.models.CustomMetadataFieldsSchema import CustomMetadataFieldsSchema
+from imagekitio.models.UpdateCustomMetadataFieldsRequestOptions import UpdateCustomMetadataFieldsRequestOptions
+
+schema = CustomMetadataFieldsSchema(min_value=100, max_value=200)
+options = UpdateCustomMetadataFieldsRequestOptions(
+    label='test-update',
+    schema=schema
+)
+result = imagekit.update_custom_metadata_fields(
+    field_id='id_of_custom_metadata_field',
+    options=options
+)
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+
+# print the label of updated custom metadata fields
+print(result.label)
+
+# print the schema's min value of updated custom metadata fields
+print(result.schema.min_value)
+```
+
+**28. Delete CustomMetaDataFields**
+
+Accepts the id to delete the custom metadata fields as per
+the [API documentation here](https://docs.imagekit.io/api-reference/custom-metadata-fields-api/delete-custom-metadata-field)
+.
+
+```python
+result = imagekit.delete_custom_metadata_field(field_id="id_of_custom_metadata_field")
+
+# Final Result
+print(result)
+
+# Raw Response
+print(result.response_metadata.raw)
+```
+
+## Utility functions
+
+We have included the following commonly used utility functions in this package.
+
+**Authentication parameter generation**
+
+Suppose one wants to implement client-side file upload. In that case, one will need a token, expiry timestamp, and a valid signature for that upload. The SDK provides a simple method that one can use in their code to generate these authentication parameters.
+
+<em>Note: Any client-side code should never expose The Private API Key. One must always generate these authentications parameters on the server-side</em>
+
+authentication
+
+`authentication_parameters = imagekit.get_authentication_parameters(token, expire)`
+
+Returns
+
+```python
+{
+    "token": "unique_token",
+    "expire": "valid_expiry_timestamp",
+    "signature": "generated_signature"
+}
+```
+
+Both the `token` and `expire` parameters are optional. If not specified, the SDK uses the UUID to generate a random token and internally generates a valid expiry timestamp. The `token` and `expire` used to generate `signature` is part of a response returned by the server.
+
+**Distance calculation between two `pHash` values**
+
+Perceptual hashing allows you to construct a has value that uniquely identifies an input image based on the contents
+of an image. [imagekit.io metadata API](https://docs.imagekit.io/api-reference/metadata-api) returns the `pHash`
+value of an image in the response. You can use this value
+to [find a duplicate or similar image](https://docs.imagekit.io/api-reference/metadata-api#using-phash-to-find-similar-or-duplicate-images)
+by calculating the distance between the two images.
+
+This SDK exposes the `phash_distance` function to calculate the distance between two `pHash` values. It accepts two `pHash`
+hexadecimal
+strings and returns a numeric value indicative of the difference between the two images.
+
+```python
+def calculate_distance():
+    # fetch metadata of two uploaded image files
+    ...
+    # extract pHash strings from both: say 'first_hash' and 'second_hash'
+    ...
+    # calculate the distance between them:
+
+    distance = imagekit.phash_distance(first_hash, second_hash)
+    return distance
+
+```
+
+**Distance calculation examples**
+
+```Python
+imagekit.phash_distance('f06830ca9f1e3e90', 'f06830ca9f1e3e90')
+# output: 0 (same image)
+
+imagekit.phash_distance('2d5ad3936d2e015b', '2d6ed293db36a4fb')
+# output: 17 (similar images)
+
+imagekit.phash_distance('a4a65595ac94518b', '7838873e791f8400')
+# output: 37 (dissimilar images)
+```
+
+**HTTP response metadata of Internal API**
+
+HTTP response metadata of the internal API call can be accessed using the \_response_metadata on the Result object.
+Example:
+
+```Python
+result = imagekit.upload_file(
+    file="<url|base_64|binary>",
+    file_name="my_file_name.jpg",
+)
+
+# Final Result
+print(result)
+print(result.response_metadata.raw)
+print(result.response_metadata.http_status_code)
+print(result.response_metadata.headers)
+```
+
+### Sample Code Instruction
+
+To run `sample` code go to the code samples here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python and run.
+
+```shell
+python sample.py
+```
+
+## Handling errors
+
+Catch and respond to invalid data, internal problems, and more.
+
+ImageKit Python SDK raises exceptions for many reasons, such as not found, invalid parameters, authentication, and
+internal server errors. Therefore, we recommend writing code that gracefully handles all possible API exceptions.
+
+#### Example:
+
+```Python
+from imagekitio.exceptions.BadRequestException import BadRequestException
+from imagekitio.exceptions.UnauthorizedException import UnauthorizedException
+from imagekitio.exceptions.ForbiddenException import ForbiddenException
+from imagekitio.exceptions.TooManyRequestsException import TooManyRequestsException
+from imagekitio.exceptions.InternalServerException import InternalServerException
+from imagekitio.exceptions.PartialSuccessException import PartialSuccessException
+from imagekitio.exceptions.NotFoundException import NotFoundException
+from imagekitio.exceptions.UnknownException import UnknownException
+
+try:
+
+    # Use ImageKit's SDK to make requests...
+    print('Run image kit api')
+except BadRequestException, e:
+    # Missing or Invalid parameters were supplied to Imagekit.io's API
+    print('Status is: ' + e.response_metadata.http_status_code)
+    print('Message is: ' + e.message)
+    print('Headers are: ' + e.response_metadata.headers)
+    print('Raw body is: ' + e.response_metadata.raw)
+except UnauthorizedException, e:
+    print(e)
+except ForbiddenException, e:
+    # No valid API key was provided.
+    print(e)
+except TooManyRequestsException, e:
+    # Can be for the following reasons:
+    # ImageKit could not authenticate your account with the keys provided.
+    # An expired key (public or private) was used with the request.
+    # The account is disabled.
+    # If you use the upload API, the total storage limit (or upload limit) is exceeded.
+    print(e)
+except InternalServerException, e:
+    # Too many requests made to the API too quickly
+    print(e)
+except PartialSuccessException, e:
+    # Something went wrong with ImageKit.io API.
+    print(e)
+except NotFoundException, e:
+    # Error cases on partial success.
+    print(e)
+except UnknownException, e:
+    # If any of the field or parameter is not found in the data
+    print(e)
+
+# Something else happened, which can be unrelated to ImageKit; the reason will be indicated in the message field
+```
+
+## Development
+
+### Tests
+
+Tests are powered by [Tox](https://tox.wiki/en/latest/).
+
+```bash
+$ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
+$ pip install tox
+$ tox
+```
+
+### Sample
+
+#### Get & Install local ImageKit Python SDK
+
+```bash
+$ git clone https://github.com/imagekit-developer/imagekit-python && cd imagekit-python
+$ pip install -e .
+```
+
+#### Get samples
+
+To integrate ImageKit Samples in the Python, the code samples covered here are hosted on GitHub - https://github.com/imagekit-samples/quickstart/tree/master/python.
+
+Open the `python/sample.py` file and replace placeholder credentials with actual values. You can get the value of [URL-endpoint](https://imagekit.io/dashboard#url-endpoints) from your ImageKit dashboard. API keys can be obtained from the [developer](https://imagekit.io/dashboard/developer/api-keys) section in your ImageKit dashboard.
+
+In the `python/sample.py` file, set the following parameters for authentication:
+
+```python
+from imagekitio import ImageKit
+imagekit = ImageKit(
+    private_key='your private_key',
+    public_key='your public_key',
+    url_endpoint = 'your url_endpoint'
+)
+```
+
+To install dependencies that are in the `python/requirements.txt` file, can fire this command to install them:
+
+```shell
+pip install -r python/requirements.txt
+```
+
+Now run `python/sample.py`. If you are using CLI Tool (Terminal/Command prompt), open the project in CLI and execute it.
+
+```shell
+# if not installed already
+pip install imagekitio
+
+# if installing local sdk
+pip install -e <path_to_local_sdk>
+
+# to run sample.py file
+python3 python/sample.py
+```
+
+## Support
+
+For any feedback or to report any issues or general implementation support, please reach out
+to [support@imagekit.io](https://github.com/imagekit-developer/imagekit-python)
+
+## Links
+
+-   [Documentation](https://docs.imagekit.io/)
+
+-   [Main Website](https://imagekit.io/)
+
+## License
+
+Released under the MIT license.
```

### Comparing `imagekitio-3.0.2/imagekitio.egg-info/SOURCES.txt` & `imagekitio-3.1.0/imagekitio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 imagekitio/__init__.py
 imagekitio/client.py
 imagekitio/file.py
 imagekitio/resource.py
 imagekitio/url.py
@@ -76,14 +77,15 @@
 tests/__init__.py
 tests/helpers.py
 tests/test_client.py
 tests/test_custom_metadata_fields_ops.py
 tests/test_files_ops.py
 tests/test_folder_ops.py
 tests/test_generate_url.py
+tests/test_models_results.py
 tests/test_tags_ops.py
 tests/test_utils_calculation.py
 tests/test_utils_formatter.py
 tests/test_utils_utils.py
 tests/dummy_data/__init__.py
 tests/dummy_data/file.py
 tests/dummy_data/urls.py
```

### Comparing `imagekitio-3.0.2/setup.py` & `imagekitio-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements/requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="imagekitio",
-    version="3.0.2",
+    version="3.1.0",
     description="Python wrapper for the ImageKit API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=install_requires,
     url="https://github.com/imagekit-developer/imagekit-python",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `imagekitio-3.0.2/tests/dummy_data/file.py` & `imagekitio-3.1.0/tests/dummy_data/file.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/helpers.py` & `imagekitio-3.1.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_client.py` & `imagekitio-3.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_custom_metadata_fields_ops.py` & `imagekitio-3.1.0/tests/test_custom_metadata_fields_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,96 @@
         self.assertEqual("62aab2cfdb4851833b8f5e64", resp.list[1].id)
         self.assertEqual(
             "http://test.com/v1/customMetadataFields?includeDeleted=true",
             responses.calls[0].request.url,
         )
 
     @responses.activate
+    def test_get_custom_metadata_fields_succeeds_with_additional_attributes_in_response(self):
+        """
+        Tests if get_custom_metadata_fields succeeds with additional responses
+        """
+        URL.API_BASE_URL = "http://test.com"
+        url = "{}/v1/customMetadataFields".format(URL.API_BASE_URL)
+        headers = create_headers_for_test()
+        responses.add(
+            responses.GET,
+            url,
+            body="""[{
+                        "id": "62a9d5f6db485107347bb7f2",
+                        "name": "test10",
+                        "label": "test10",
+                        "schema": {
+                            "type": "Number",
+                            "isValueRequired": false,
+                            "minValue": 10,
+                            "maxValue": 1000,
+                            "currentValue":100
+                        }
+                    }, {
+                        "id": "62aab2cfdb4851833b8f5e64",
+                        "name": "test11",
+                        "label": "test11",
+                        "schema": {
+                            "type": "Number",
+                            "isValueRequired": false,
+                            "minValue": 10,
+                            "maxValue": 1000,
+                            "currentValue":1000
+                        }
+                    }]""",
+            match=[matchers.query_string_matcher("includeDeleted=true")],
+            headers=headers,
+        )
+        resp = self.client.get_custom_metadata_fields(include_deleted=True)
+
+        mock_response_metadata = {
+            "raw": [
+                {
+                    "id": "62a9d5f6db485107347bb7f2",
+                    "name": "test10",
+                    "label": "test10",
+                    "schema": {
+                        "type": "Number",
+                        "isValueRequired": False,
+                        "minValue": 10,
+                        "maxValue": 1000,
+                        "currentValue":100
+                    },
+                },
+                {
+                    "id": "62aab2cfdb4851833b8f5e64",
+                    "name": "test11",
+                    "label": "test11",
+                    "schema": {
+                        "type": "Number",
+                        "isValueRequired": False,
+                        "minValue": 10,
+                        "maxValue": 1000,
+                        "currentValue":1000
+                    },
+                },
+            ],
+            "httpStatusCode": 200,
+            "headers": {
+                "Content-Type": "text/plain",
+                "Accept-Encoding": "gzip, deflate",
+                "Authorization": "Basic ZmFrZTEyMjo=",
+            },
+        }
+
+        self.assertEqual(
+            camel_dict_to_snake_dict(mock_response_metadata),
+            resp.response_metadata.__dict__,
+        )
+        self.assertEqual(resp.list[0].schema.current_value,100)
+        self.assertEqual(resp.list[1].schema.current_value,1000)
+        self.assertEqual(resp.list[0].random,None)
+
+    @responses.activate
     def test_delete_custom_metadata_fields_succeeds(self):
         """
         Tests if delete_custom_metadata_fields succeeds
         """
         URL.API_BASE_URL = "http://test.com"
         url = "{}/v1/customMetadataFields/{}".format(URL.API_BASE_URL, self.field_id)
         headers = create_headers_for_test()
```

### Comparing `imagekitio-3.0.2/tests/test_files_ops.py` & `imagekitio-3.1.0/tests/test_files_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,14 +538,86 @@
         self.assertEqual(resp.embedded_metadata.date_time_created,date_time_created)
 
         # self.assertEqual(request_body, responses.calls[0].request.body)
         # self.assertEqual(
         #     camel_dict_to_snake_dict(mock_response_metadata),
         #     resp.response_metadata.__dict__,
         # )
+    @responses.activate()
+    def test_upload_file_result_on_upload_with_non_breaking_changes_in_response(self):
+        """
+        Tests if  upload succeeds
+        """
+        URL.UPLOAD_BASE_URL = "http://test.com"
+        url = "%s%s" % (URL.UPLOAD_BASE_URL, "/api/v1/files/upload")
+        headers = create_headers_for_test()
+        responses.add(
+            responses.POST,
+            url,
+            body="""{
+                        "fileId": "fake_file_id1234",
+                        "name": "file_name.jpg",
+                        "size": 102117,
+                        "versionInfo": {
+                            "id": "62d670648cdb697522602b45",
+                            "name": "Version 11",
+                            "decription":"Removed Background"
+                        },
+                        "filePath": "/testing-python-folder/file_name.jpg",
+                        "url": "https://ik.imagekit.io/your_imagekit_id/testing-python-folder/file_name.jpg",
+                        "fileType": "image",
+                        "height": 700,
+                        "width": 1050,
+                        "resolution":120,
+                        "thumbnailUrl": "https://ik.imagekit.io/your_imagekit_id/tr:n-ik_ml_thumbnail/testing-python-folder/file_name.jpg",
+                        "tags": [
+                            "abc",
+                            "def"
+                        ],
+                        "AITags": [
+                            {
+                                "name": "Computer",
+                                "confidence": 97.66,
+                                "source": "google-auto-tagging",
+                                "description":"automatically created tag"
+                            },
+                            {
+                                "name": "Personal computer",
+                                "confidence": 94.96,
+                                "source": "google-auto-tagging",
+                                "description":"automatically created tag"
+                            }
+                        ],
+                        "embeddedMetadata":{
+                            "XResolution":1,"YResolution":1,"DateCreated":"2023-06-21T11:49:39.850Z","DateTimeCreated":"2023-06-21T11:49:39.850Z","DPI":120
+                        },
+                        "isPrivateFile": true,
+                        "extensionStatus": {
+                            "remove-bg": "pending",
+                            "google-auto-tagging": "success",
+                            "image-enhancing":"pending"
+                        }
+                    }""",
+            headers=headers,
+        )
+        with open(self.sample_image,"rb") as img:
+            resp = self.client.upload(
+                file=img,
+                file_name="test.jpeg",
+                options=UploadFileRequestOptions(
+                    tags = ["test"],
+                    response_fields=["embedded_metadata"]
+                )
+        )
+        self.assertEqual(resp.embedded_metadata.dpi,120)
+        self.assertEqual(resp.resolution,120)
+        self.assertEqual(resp.ai_tags[0].name,"Computer")
+        self.assertEqual(resp.ai_tags[0].description,"automatically created tag")
+        self.assertEqual(resp.extension_status["image-enhancing"],"pending")
+
 
     def test_upload_fails_without_file_name(self) -> None:
         """Test upload raises error on missing required params"""
         try:
             with open(self.sample_image, mode="rb") as img:
                 imgstr = base64.b64encode(img.read())
             self.client.upload_file(file=imgstr)
@@ -1108,14 +1180,55 @@
         self.assertEqual(["fake_123", "fake_222"], resp.successfully_deleted_file_ids)
         self.assertEqual(
             "http://test.com/v1/files/batch/deleteByFileIds",
             responses.calls[0].request.url,
         )
 
     @responses.activate
+    def test_bulk_file_delete_succeeds_and_recieves_extra_non_breaking_changes_from_apii(self):
+        """Test bulk_delete  on authenticated request
+        this function tests if bulk_file_delete working properly
+        """
+
+        URL.API_BASE_URL = "http://test.com"
+        url = URL.API_BASE_URL + "/v1/files" + URL.BULK_FILE_DELETE
+        headers = {"Content-Type": "application/json"}
+        headers.update(get_auth_headers_for_test())
+
+        responses.add(
+            responses.POST,
+            url,
+            body='{"successfullyDeletedFileIds": ["fake_123"],"nonDeletedFields":["fake_222"]}',
+            headers=headers,
+        )
+
+        resp = self.client.bulk_file_delete(self.bulk_delete_ids)
+
+        mock_response_metadata = {
+            "raw": {"successfullyDeletedFileIds": ["fake_123"],"nonDeletedFields":["fake_222"]},
+            "httpStatusCode": 200,
+            "headers": {
+                "Content-Type": "text/plain, application/json",
+                "Authorization": "Basic ZmFrZTEyMjo=",
+            },
+        }
+        self.assertEqual(
+            '{"fileIds": ["fake_123", "fake_222"]}', responses.calls[0].request.body
+        )
+        self.assertEqual(
+            camel_dict_to_snake_dict(mock_response_metadata),
+            resp.response_metadata.__dict__,
+        )
+        self.assertEqual(["fake_123"], resp.successfully_deleted_file_ids)
+        self.assertEqual(["fake_222"], resp.non_deleted_fields)
+        self.assertEqual(
+            "http://test.com/v1/files/batch/deleteByFileIds",
+            responses.calls[0].request.url,
+        )
+    @responses.activate
     def test_bulk_file_delete_fails_with_404_exception(self) -> None:
         """Test bulk_file_delete raises 404 error"""
 
         URL.API_BASE_URL = "http://test.com"
         url = URL.API_BASE_URL + "/v1/files" + URL.BULK_FILE_DELETE
         headers = {"Content-Type": "application/json"}
         headers.update(get_auth_headers_for_test())
@@ -2743,7 +2856,112 @@
         )
         self.assertEqual("fileId", resp.file_id)
         self.assertEqual("versionId", resp.version_info.id)
         self.assertEqual(
             "http://test.com/v1/files/fax_abx1223/versions/fake_123_version_id/restore",
             responses.calls[0].request.url,
         )
+
+    @responses.activate()
+    def test_get_metadata_with_non_breaking_changes_in_response(self):
+        URL.API_BASE_URL = "http://test.com"
+        url = "{}/v1/files/{}/metadata".format(URL.API_BASE_URL, self.file_id)
+        headers = {"Content-Type": "application/json"}
+        headers.update(create_headers_for_test())
+        responses.add(
+            responses.GET,
+            url,
+            headers=headers,
+            body="""{
+                    "height": 176, 
+                    "width": 287, 
+                    "size": 15869, 
+                    "format": "jpg", 
+                    "hasColorProfile": false, 
+                    "quality": 0, 
+                    "density": 72, 
+                    "hasTransparency": false, 
+                    "exif":{
+                        "gps":{
+                            "GPSVersionId":"1.2",
+                            "latitude":1235.124151355,
+                            "longitude":12315.326236
+                        },
+                        "thumbnail":
+                        {
+                            "compression":12,
+                            "YResolution":1,
+                            "XResolution":1,
+                            "resolutionUnit":"DPI",
+                            "thumbnailOffset":12,
+                            "thumbnailLength":12,
+                            "overallResolution":1
+                        },
+                        "exif": {
+                            "exposureTime":10,
+                            "FNumber":1,
+                            "exposureProgram":null,
+                            "ISO":"2001",
+                            "exifVersion":1.2,
+                            "dateTimeOriginal":null,
+                            "createDate":null,
+                            "shutterSpeedValue":122,
+                            "apertureValue":12,
+                            "exposureCompensation":12,
+                            "meteringMode":null,
+                            "flash":"white",
+                            "focalLength":null,
+                            "subSecTime":null,
+                            "subSecTimeOriginal":null,
+                            "subSecTimeDigitized":null,
+                            "flashpixVersion":null,
+                            "colorSpace":null,
+                            "exifImageWidth":null,
+                            "exifImageHeight":null,
+                            "interopOffset":null,
+                            "focalPlaneXResolution":null,
+                            "focalPlaneYResolution":null,
+                            "focalPlaneResolutionUnit":null,
+                            "customRendered":null,
+                            "exposureMode":null,
+                            "whiteBalance":null,
+                            "sceneCaptureType":null,
+                            "cameraModel":"Canon"
+                        }, 
+                        "image":{
+                            "make":null,
+                            "model":null,
+                            "orientation":null,
+                            "XResolution":null,
+                            "YResolution":null,
+                            "resolutionUnit":null,
+                            "software":null,
+                            "modifyDate":null,
+                            "YCbCrPositioning":null,
+                            "exifOffset":null,
+                            "gpsInfo":"navic",
+                            "cropped":true
+                        },
+                        "interoperability":{
+                            "interopVersion":1.1,
+                            "interopIndex":1.2,
+                            "interopRandom":132
+                        }
+                    }
+                }
+                """,
+        
+        )
+
+        metadataExif = self.client.get_metadata(self.file_id)
+
+        self.assertEqual(metadataExif.exif.interoperability.interop_index,1.2)
+        self.assertEqual(metadataExif.exif.interoperability.interop_random,132)
+        self.assertEqual(metadataExif.exif.image.gps_info,"navic")
+        self.assertEqual(metadataExif.exif.image.cropped,True)
+        self.assertEqual(metadataExif.exif.gps.gps_version_id,["1",".","2"])
+        self.assertEqual(metadataExif.exif.gps.longitude,12315.326236)
+        self.assertEqual(metadataExif.exif.exif.exposure_time,10)
+        self.assertEqual(metadataExif.exif.exif.camera_model,"Canon")
+        self.assertEqual(metadataExif.exif.thumbnail.x_resolution,1)
+        self.assertEqual(metadataExif.exif.thumbnail.overall_resolution,1)
+
```

### Comparing `imagekitio-3.0.2/tests/test_folder_ops.py` & `imagekitio-3.1.0/tests/test_folder_ops.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_generate_url.py` & `imagekitio-3.1.0/tests/test_generate_url.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_tags_ops.py` & `imagekitio-3.1.0/tests/test_tags_ops.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_utils_calculation.py` & `imagekitio-3.1.0/tests/test_utils_calculation.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_utils_formatter.py` & `imagekitio-3.1.0/tests/test_utils_formatter.py`

 * *Files identical despite different names*

### Comparing `imagekitio-3.0.2/tests/test_utils_utils.py` & `imagekitio-3.1.0/tests/test_utils_utils.py`

 * *Files identical despite different names*

