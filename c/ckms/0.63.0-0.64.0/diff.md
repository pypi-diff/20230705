# Comparing `tmp/ckms-0.63.0.tar.gz` & `tmp/ckms-0.64.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckms-0.63.0.tar", last modified: Sun Mar 26 23:04:36 2023, max compression
+gzip compressed data, was "ckms-0.64.0.tar", last modified: Wed Jul  5 15:02:16 2023, max compression
```

## Comparing `ckms-0.63.0.tar` & `ckms-0.64.0.tar`

### file list

```diff
@@ -1,357 +1,358 @@
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.335983 ckms-0.63.0/
--rw-r--r--   0 cochise    (501) staff       (20)      373 2022-07-09 11:28:18.000000 ckms-0.63.0/MANIFEST.in
--rw-r--r--   0 cochise    (501) staff       (20)     2095 2023-03-26 23:04:36.335855 ckms-0.63.0/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)      354 2022-07-09 11:28:18.000000 ckms-0.63.0/README.md
--rw-r--r--   0 cochise    (501) staff       (20)        7 2023-03-26 23:04:16.000000 ckms-0.63.0/VERSION
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.287770 ckms-0.63.0/ckms/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.289960 ckms-0.63.0/ckms/core/
--rw-r--r--   0 cochise    (501) staff       (20)     2059 2023-03-25 23:17:40.000000 ckms-0.63.0/ckms/core/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2452 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/const.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.290295 ckms-0.63.0/ckms/core/exceptions/
--rw-r--r--   0 cochise    (501) staff       (20)      764 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/exceptions/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1554 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/exceptions/malformed.py
--rw-r--r--   0 cochise    (501) staff       (20)     6577 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/keychain.py
--rw-r--r--   0 cochise    (501) staff       (20)    26669 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/keyinspector.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.290679 ckms-0.63.0/ckms/core/local/
--rw-r--r--   0 cochise    (501) staff       (20)    11074 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/core/local/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1912 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/core/local/models.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.293280 ckms-0.63.0/ckms/core/local/types/
--rw-r--r--   0 cochise    (501) staff       (20)     1416 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      994 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/core/local/types/contentencryptionkey.py
--rw-r--r--   0 cochise    (501) staff       (20)     2909 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/edwardscurvekeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     2447 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/ellipticcurvekeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)      742 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/hmac.py
--rw-r--r--   0 cochise    (501) staff       (20)     1095 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/key.py
--rw-r--r--   0 cochise    (501) staff       (20)     1335 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/core/local/types/localkey.py
--rw-r--r--   0 cochise    (501) staff       (20)     1886 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/core/local/types/localkeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     1080 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/parameterlesskey.py
--rw-r--r--   0 cochise    (501) staff       (20)     1961 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/rsakeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     3688 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/core/local/types/symmetrickeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     1128 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/local/types/transientkey.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.296713 ckms-0.63.0/ckms/core/models/
--rw-r--r--   0 cochise    (501) staff       (20)     1533 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2600 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/basekeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     2304 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/certificate.py
--rw-r--r--   0 cochise    (501) staff       (20)     1776 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/contentencryptionkey.py
--rw-r--r--   0 cochise    (501) staff       (20)      973 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/core/models/joseheader_.py
--rw-r--r--   0 cochise    (501) staff       (20)     4769 2022-08-28 17:50:27.000000 ckms-0.63.0/ckms/core/models/joseobject.py
--rw-r--r--   0 cochise    (501) staff       (20)     1383 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/jsonb64.py
--rw-r--r--   0 cochise    (501) staff       (20)     3542 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/jsonwebencryption.py
--rw-r--r--   0 cochise    (501) staff       (20)     7005 2022-08-28 17:51:00.000000 ckms-0.63.0/ckms/core/models/jsonwebencryption_.py
--rw-r--r--   0 cochise    (501) staff       (20)      605 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/jsonwebencryptionbase.py
--rw-r--r--   0 cochise    (501) staff       (20)      707 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/jsonwebencryptionflattened.py
--rw-r--r--   0 cochise    (501) staff       (20)      292 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/jsonwebencryptionrecipient.py
--rw-r--r--   0 cochise    (501) staff       (20)      455 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/jsonwebencryptionwithrecipients.py
--rw-r--r--   0 cochise    (501) staff       (20)     6257 2023-03-26 23:04:13.000000 ckms-0.63.0/ckms/core/models/jsonwebsignature.py
--rw-r--r--   0 cochise    (501) staff       (20)     6927 2023-03-25 23:15:54.000000 ckms-0.63.0/ckms/core/models/keyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     1407 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/octetb64.py
--rw-r--r--   0 cochise    (501) staff       (20)     4247 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/publickeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)     1108 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/recipient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1582 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/remoteblobparams.py
--rw-r--r--   0 cochise    (501) staff       (20)     4114 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/models/signature.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.297124 ckms-0.63.0/ckms/core/provider/
--rw-r--r--   0 cochise    (501) staff       (20)      654 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)    15351 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/core/provider/provider.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.298922 ckms-0.63.0/ckms/core/provider/tests/
--rw-r--r--   0 cochise    (501) staff       (20)     1357 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3553 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/asymmetricsigningtestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     2399 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/baseprovidertestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     3731 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/encryptiontestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     1320 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/josebasetestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     4483 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/joseconsumertestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     7518 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/joseencryptiontestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     5317 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/joseproducertestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)      840 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/providertestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     3315 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/provider/tests/symmetricsigningtestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)      893 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/random.py
--rw-r--r--   0 cochise    (501) staff       (20)     1007 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/core/runlevel.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.299040 ckms-0.63.0/ckms/ext/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.299228 ckms-0.63.0/ckms/ext/asn1/
--rw-r--r--   0 cochise    (501) staff       (20)     3536 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/asn1/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2274 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/asn1/fields.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.299729 ckms-0.63.0/ckms/ext/azure/
--rw-r--r--   0 cochise    (501) staff       (20)      664 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/azure/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3811 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/azure/models.py
--rw-r--r--   0 cochise    (501) staff       (20)     1748 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/azure/provider.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.300164 ckms-0.63.0/ckms/ext/azure/types/
--rw-r--r--   0 cochise    (501) staff       (20)      734 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/azure/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1642 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/azure/types/azureconsumer.py
--rw-r--r--   0 cochise    (501) staff       (20)      731 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/azure/types/iazureprovider.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.300560 ckms-0.63.0/ckms/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)      666 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)    10216 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/ext/google/provider.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.301349 ckms-0.63.0/ckms/ext/google/types/
--rw-r--r--   0 cochise    (501) staff       (20)      832 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/google/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      875 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/google/types/igoogleprovider.py
--rw-r--r--   0 cochise    (501) staff       (20)     6215 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/ext/google/types/keyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)      813 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/google/types/secretmanagerblob.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.301476 ckms-0.63.0/ckms/ext/pkcs/
--rw-r--r--   0 cochise    (501) staff       (20)      759 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/oid.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.302529 ckms-0.63.0/ckms/ext/pkcs/types/
--rw-r--r--   0 cochise    (501) staff       (20)      660 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1095 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/types/attribute.py
--rw-r--r--   0 cochise    (501) staff       (20)     1633 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/types/contentinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)     1439 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/types/issuerandserialnumber.py
--rw-r--r--   0 cochise    (501) staff       (20)     2361 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/types/signeddata.py
--rw-r--r--   0 cochise    (501) staff       (20)     4813 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/pkcs/types/signerinfo.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.284661 ckms-0.63.0/ckms/ext/rfc2459/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.302945 ckms-0.63.0/ckms/ext/rfc2459/types/
--rw-r--r--   0 cochise    (501) staff       (20)      705 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc2459/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2012 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc2459/types/relativedistinguishedname.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.303180 ckms-0.63.0/ckms/ext/rfc3161/
--rw-r--r--   0 cochise    (501) staff       (20)      668 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc3161/oid.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.284808 ckms-0.63.0/ckms/ext/rfc5280/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.304584 ckms-0.63.0/ckms/ext/rfc5280/types/
--rw-r--r--   0 cochise    (501) staff       (20)     1099 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2657 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/algorithmidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1740 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/attribute.py
--rw-r--r--   0 cochise    (501) staff       (20)     1619 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/rdnsequence.py
--rw-r--r--   0 cochise    (501) staff       (20)     1533 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/relativedistinguishedname.py
--rw-r--r--   0 cochise    (501) staff       (20)     1106 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/signaturedigestalgorithmidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      946 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      804 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifiertype.py
--rw-r--r--   0 cochise    (501) staff       (20)     3431 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5280/types/subjectpublickeyinfo.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.284906 ckms-0.63.0/ckms/ext/rfc5480/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.305105 ckms-0.63.0/ckms/ext/rfc5480/types/
--rw-r--r--   0 cochise    (501) staff       (20)      740 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5480/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1239 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5480/types/ecparameters.py
--rw-r--r--   0 cochise    (501) staff       (20)     1092 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5480/types/ellipticcurvetype.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.285003 ckms-0.63.0/ckms/ext/rfc5758/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.305395 ckms-0.63.0/ckms/ext/rfc5758/types/
--rw-r--r--   0 cochise    (501) staff       (20)      714 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5758/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1320 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/rfc5758/types/signaturedigestalgorithmtype.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.306080 ckms-0.63.0/ckms/ext/tsa/
--rw-r--r--   0 cochise    (501) staff       (20)      937 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.306411 ckms-0.63.0/ckms/ext/tsa/certs/
--rw-r--r--   0 cochise    (501) staff       (20)     2416 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/certs/DigiCertTrustedG4RSA4096SHA256TimeStampingCA.crt
--rw-r--r--   0 cochise    (501) staff       (20)     1793 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/certs/digicert_tsa_2021.crt
--rw-r--r--   0 cochise    (501) staff       (20)     3202 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/timestamper.py
--rw-r--r--   0 cochise    (501) staff       (20)     3545 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/timestampingauthority.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.308081 ckms-0.63.0/ckms/ext/tsa/types/
--rw-r--r--   0 cochise    (501) staff       (20)      977 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1279 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/algorithmidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1384 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/messageimprint.py
--rw-r--r--   0 cochise    (501) staff       (20)      822 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/pkifailureinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)      760 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/pkistatus.py
--rw-r--r--   0 cochise    (501) staff       (20)     1989 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/pkistatusinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)      643 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/timestamp.py
--rw-r--r--   0 cochise    (501) staff       (20)      671 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/timestampreq.py
--rw-r--r--   0 cochise    (501) staff       (20)     2251 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/timestampresp.py
--rw-r--r--   0 cochise    (501) staff       (20)     2921 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/timestamptoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     2921 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/types/tstinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)      581 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/tsa/utils.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.285305 ckms-0.63.0/ckms/ext/x509/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.308542 ckms-0.63.0/ckms/ext/x509/types/
--rw-r--r--   0 cochise    (501) staff       (20)      743 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/x509/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1110 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/x509/types/algorithmidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      815 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/x509/types/certificate.py
--rw-r--r--   0 cochise    (501) staff       (20)      650 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/ext/x509/types/tbscertificate.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.310952 ckms-0.63.0/ckms/jose/
--rw-r--r--   0 cochise    (501) staff       (20)     1009 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     6445 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/decoder.py
--rw-r--r--   0 cochise    (501) staff       (20)     4612 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/encoder.py
--rw-r--r--   0 cochise    (501) staff       (20)      781 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/exceptions.py
--rw-r--r--   0 cochise    (501) staff       (20)      941 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/joseheaderset.py
--rw-r--r--   0 cochise    (501) staff       (20)    17752 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/josepayload.py
--rw-r--r--   0 cochise    (501) staff       (20)      833 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/josepayloadcontainer.py
--rw-r--r--   0 cochise    (501) staff       (20)     2181 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/jsonwebkeysetresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)     1095 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/memoryissuercache.py
--rw-r--r--   0 cochise    (501) staff       (20)     1119 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/nullissuercache.py
--rw-r--r--   0 cochise    (501) staff       (20)      896 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/nulltokenconsumer.py
--rw-r--r--   0 cochise    (501) staff       (20)     9965 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/payloadcodec.py
--rw-r--r--   0 cochise    (501) staff       (20)     2355 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/recipient.py
--rw-r--r--   0 cochise    (501) staff       (20)     1005 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/runlevel.py
--rw-r--r--   0 cochise    (501) staff       (20)     2892 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/signature_.py
--rw-r--r--   0 cochise    (501) staff       (20)     4334 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/trustedissuers.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.311288 ckms-0.63.0/ckms/jose/types/
--rw-r--r--   0 cochise    (501) staff       (20)      750 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      882 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/types/baseissuercache.py
--rw-r--r--   0 cochise    (501) staff       (20)      859 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/jose/types/basetokenconsumer.py
--rw-r--r--   0 cochise    (501) staff       (20)       87 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/jose/validator.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.311396 ckms-0.63.0/ckms/lib/
--rw-r--r--   0 cochise    (501) staff       (20)       19 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/lib/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.311816 ckms-0.63.0/ckms/lib/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)      126 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/lib/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2626 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/lib/oauth2/openauthorizationclient.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.312038 ckms-0.63.0/ckms/main/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/main/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      784 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/main/__main__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2756 2023-02-04 23:57:51.000000 ckms-0.63.0/ckms/package.json
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.312313 ckms-0.63.0/ckms/pkix/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1065 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/oid.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.314767 ckms-0.63.0/ckms/pkix/types/
--rw-r--r--   0 cochise    (501) staff       (20)     1122 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1297 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/attribute.py
--rw-r--r--   0 cochise    (501) staff       (20)     2457 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/attributelist.py
--rw-r--r--   0 cochise    (501) staff       (20)     1076 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/basecertificateextension.py
--rw-r--r--   0 cochise    (501) staff       (20)     1439 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/basicconstraints.py
--rw-r--r--   0 cochise    (501) staff       (20)     4704 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/certificateextension.py
--rw-r--r--   0 cochise    (501) staff       (20)     4953 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/certificateextensionsequence.py
--rw-r--r--   0 cochise    (501) staff       (20)     6321 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/certificationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)     2270 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/certificationrequestinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)      711 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/dnsname.py
--rw-r--r--   0 cochise    (501) staff       (20)     1193 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/extendedkeyusagetype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1052 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/generalname.py
--rw-r--r--   0 cochise    (501) staff       (20)     1160 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/ipaddressname.py
--rw-r--r--   0 cochise    (501) staff       (20)     1352 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/name.py
--rw-r--r--   0 cochise    (501) staff       (20)      747 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/pkix/types/uriname.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.324382 ckms-0.63.0/ckms/types/
--rw-r--r--   0 cochise    (501) staff       (20)     4778 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1082 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/aesalgorithmtype.py
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/aeskektype.py
--rw-r--r--   0 cochise    (501) staff       (20)      743 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/aeskeywrapoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     2854 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/aesoperation.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.324874 ckms-0.63.0/ckms/types/algorithm/
--rw-r--r--   0 cochise    (501) staff       (20)     8435 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/algorithm/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4474 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/types/algorithm/base.py
--rw-r--r--   0 cochise    (501) staff       (20)      785 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/algorithm/nullalgorithm.py
--rw-r--r--   0 cochise    (501) staff       (20)      768 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/asymmetricsigningoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     1831 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/audiencetype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1135 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ciphertext.py
--rw-r--r--   0 cochise    (501) staff       (20)     4455 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/claimset.py
--rw-r--r--   0 cochise    (501) staff       (20)     1581 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/cryptographicfailure.py
--rw-r--r--   0 cochise    (501) staff       (20)     1204 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/cryptographypublickeytype.py
--rw-r--r--   0 cochise    (501) staff       (20)     4622 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/data.py
--rw-r--r--   0 cochise    (501) staff       (20)     1470 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/decrypter.py
--rw-r--r--   0 cochise    (501) staff       (20)     2530 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/digest.py
--rw-r--r--   0 cochise    (501) staff       (20)      826 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/edsaoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)      874 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/edwardscurvealgorithmtype.py
--rw-r--r--   0 cochise    (501) staff       (20)      767 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/edwardscurvetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      967 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ellipticcurvealgorithmtype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1437 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ellipticcurveoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)      768 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ellipticcurvetype.py
--rw-r--r--   0 cochise    (501) staff       (20)     2429 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/encrypter.py
--rw-r--r--   0 cochise    (501) staff       (20)      789 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/encryptoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     1227 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/forbiddenoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     1001 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/generatekeyoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     2106 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/generatekeyspec.py
--rw-r--r--   0 cochise    (501) staff       (20)      757 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/hmacalgorithmtype.py
--rw-r--r--   0 cochise    (501) staff       (20)      814 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/hmacoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     2502 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/icontentencryptionkey.py
--rw-r--r--   0 cochise    (501) staff       (20)      810 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ihasher.py
--rw-r--r--   0 cochise    (501) staff       (20)     1221 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ihttpclient.py
--rw-r--r--   0 cochise    (501) staff       (20)      916 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ihttpresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     3324 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ikeychain.py
--rw-r--r--   0 cochise    (501) staff       (20)     2584 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ikeyinspector.py
--rw-r--r--   0 cochise    (501) staff       (20)     2243 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ikeyspecification.py
--rw-r--r--   0 cochise    (501) staff       (20)      976 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/invalidcredential.py
--rw-r--r--   0 cochise    (501) staff       (20)     2150 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/invalidtoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     3000 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/ioperationperformer.py
--rw-r--r--   0 cochise    (501) staff       (20)     6005 2022-09-03 01:59:24.000000 ckms-0.63.0/ckms/types/iprovider.py
--rw-r--r--   0 cochise    (501) staff       (20)     7767 2023-03-13 11:59:00.000000 ckms-0.63.0/ckms/types/jsonwebkey.py
--rw-r--r--   0 cochise    (501) staff       (20)     2808 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/types/jsonwebkeyset.py
--rw-r--r--   0 cochise    (501) staff       (20)     4372 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/jsonwebtoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     1123 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/keyalgorithmtype.py
--rw-r--r--   0 cochise    (501) staff       (20)      863 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/keyoperationtype.py
--rw-r--r--   0 cochise    (501) staff       (20)      682 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/keyusetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      899 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/keywrapoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     3259 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/malformed.py
--rw-r--r--   0 cochise    (501) staff       (20)      826 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/message.py
--rw-r--r--   0 cochise    (501) staff       (20)     4384 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/operation.py
--rw-r--r--   0 cochise    (501) staff       (20)      896 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/plaintext.py
--rw-r--r--   0 cochise    (501) staff       (20)      988 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/rsaalgorithmtype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1574 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/rsaoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)    27072 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/servermetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)     1902 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/signer.py
--rw-r--r--   0 cochise    (501) staff       (20)     1072 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/signingoperation.py
--rw-r--r--   0 cochise    (501) staff       (20)     2719 2022-10-05 17:44:31.000000 ckms-0.63.0/ckms/types/trustissues.py
--rw-r--r--   0 cochise    (501) staff       (20)      716 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/undecryptable.py
--rw-r--r--   0 cochise    (501) staff       (20)     1777 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/types/verifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     2873 2022-08-19 20:55:57.000000 ckms-0.63.0/ckms/utils.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.288589 ckms-0.63.0/ckms.egg-info/
--rw-r--r--   0 cochise    (501) staff       (20)     2095 2023-03-26 23:04:35.000000 ckms-0.63.0/ckms.egg-info/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)     9711 2023-03-26 23:04:36.000000 ckms-0.63.0/ckms.egg-info/SOURCES.txt
--rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-26 23:04:35.000000 ckms-0.63.0/ckms.egg-info/dependency_links.txt
--rw-r--r--   0 cochise    (501) staff       (20)       97 2023-03-26 23:04:36.000000 ckms-0.63.0/ckms.egg-info/entry_points.txt
--rw-r--r--   0 cochise    (501) staff       (20)      724 2023-03-26 23:04:36.000000 ckms-0.63.0/ckms.egg-info/requires.txt
--rw-r--r--   0 cochise    (501) staff       (20)       50 2023-03-26 23:04:36.000000 ckms-0.63.0/ckms.egg-info/top_level.txt
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.286087 ckms-0.63.0/docs/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.324987 ckms-0.63.0/docs/source/
--rw-r--r--   0 cochise    (501) staff       (20)     2410 2022-07-09 11:28:13.000000 ckms-0.63.0/docs/source/conf.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.326628 ckms-0.63.0/examples/
--rw-r--r--   0 cochise    (501) staff       (20)      506 2022-07-09 11:28:16.000000 ckms-0.63.0/examples/google-aes.py
--rw-r--r--   0 cochise    (501) staff       (20)     5422 2022-07-09 11:28:16.000000 ckms-0.63.0/examples/google-kms.py
--rw-r--r--   0 cochise    (501) staff       (20)     1201 2022-07-09 11:28:13.000000 ckms-0.63.0/examples/intro-jose.py
--rw-r--r--   0 cochise    (501) staff       (20)      591 2022-07-09 11:28:13.000000 ckms-0.63.0/examples/intro.py
--rw-r--r--   0 cochise    (501) staff       (20)      887 2022-07-09 11:28:15.000000 ckms-0.63.0/examples/issuers.py
--rw-r--r--   0 cochise    (501) staff       (20)      789 2022-07-09 11:28:16.000000 ckms-0.63.0/examples/local.py
--rw-r--r--   0 cochise    (501) staff       (20)      218 2022-07-09 11:28:15.000000 ckms-0.63.0/examples/oauth2_metadata.py
--rw-r--r--   0 cochise    (501) staff       (20)      153 2022-07-09 11:28:17.000000 ckms-0.63.0/examples/settings.py
--rw-r--r--   0 cochise    (501) staff       (20)       48 2022-07-09 11:28:12.000000 ckms-0.63.0/pyproject.toml
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-26 23:04:36.336017 ckms-0.63.0/setup.cfg
--rw-r--r--   0 cochise    (501) staff       (20)     1274 2022-07-09 11:28:12.000000 ckms-0.63.0/setup.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.326906 ckms-0.63.0/tests/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:12.000000 ckms-0.63.0/tests/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     7435 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.329842 ckms-0.63.0/tests/core/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:15.000000 ckms-0.63.0/tests/core/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4021 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/basedatatestcase.py
--rw-r--r--   0 cochise    (501) staff       (20)     3350 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1625 2022-07-11 07:42:21.000000 ckms-0.63.0/tests/core/test_system_jwk_certificate.py
--rw-r--r--   0 cochise    (501) staff       (20)      940 2022-07-09 11:28:16.000000 ckms-0.63.0/tests/core/test_unit_blob_local.py
--rw-r--r--   0 cochise    (501) staff       (20)      720 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_data.py
--rw-r--r--   0 cochise    (501) staff       (20)     2162 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_digest.py
--rw-r--r--   0 cochise    (501) staff       (20)     2134 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/core/test_unit_jose_consumer_jwcrypto.py
--rw-r--r--   0 cochise    (501) staff       (20)      861 2022-07-09 11:28:16.000000 ckms-0.63.0/tests/core/test_unit_jose_parse.py
--rw-r--r--   0 cochise    (501) staff       (20)     8831 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_keychain.py
--rw-r--r--   0 cochise    (501) staff       (20)     3049 2022-07-09 11:28:15.000000 ckms-0.63.0/tests/core/test_unit_keyinspector.py
--rw-r--r--   0 cochise    (501) staff       (20)      754 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_message.py
--rw-r--r--   0 cochise    (501) staff       (20)     3305 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_models_jose_deserialize.py
--rw-r--r--   0 cochise    (501) staff       (20)     4597 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_models_jwe.py
--rw-r--r--   0 cochise    (501) staff       (20)     4980 2022-07-09 11:28:16.000000 ckms-0.63.0/tests/core/test_unit_provider.py
--rw-r--r--   0 cochise    (501) staff       (20)     6803 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/core/test_unit_provider_local.py
--rw-r--r--   0 cochise    (501) staff       (20)      198 2022-07-09 11:28:16.000000 ckms-0.63.0/tests/core/test_unit_random.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.330040 ckms-0.63.0/tests/ext/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/ext/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.330201 ckms-0.63.0/tests/ext/rfc2986/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/rfc2986/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3850 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/rfc2986/test_unit_csr.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.331714 ckms-0.63.0/tests/ext/tsa/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1378 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)      803 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_accv.py
--rw-r--r--   0 cochise    (501) staff       (20)      807 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_apple.py
--rw-r--r--   0 cochise    (501) staff       (20)      892 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_digicert.py
--rw-r--r--   0 cochise    (501) staff       (20)      844 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_globalsign.py
--rw-r--r--   0 cochise    (501) staff       (20)      797 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_izenpe.py
--rw-r--r--   0 cochise    (501) staff       (20)      810 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_keynectis.py
--rw-r--r--   0 cochise    (501) staff       (20)      823 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_quovadis.py
--rw-r--r--   0 cochise    (501) staff       (20)     1646 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/test_system_timestamper_multi.py
--rw-r--r--   0 cochise    (501) staff       (20)     1255 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/ext/tsa/tsatests.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.331903 ckms-0.63.0/tests/impl/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:13.000000 ckms-0.63.0/tests/impl/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)       19 2022-07-09 11:28:13.000000 ckms-0.63.0/tests/impl/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.332374 ckms-0.63.0/tests/impl/google/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:13.000000 ckms-0.63.0/tests/impl/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3220 2022-07-09 11:28:13.000000 ckms-0.63.0/tests/impl/google/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)      410 2022-07-09 11:28:13.000000 ckms-0.63.0/tests/impl/google/test_integration_signing.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.333505 ckms-0.63.0/tests/jose/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:13.000000 ckms-0.63.0/tests/jose/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2242 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/jose/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1527 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/jose/test_system_trustedissuers_google.py
--rw-r--r--   0 cochise    (501) staff       (20)     4604 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/jose/test_unit_claimset_jwt.py
--rw-r--r--   0 cochise    (501) staff       (20)     3062 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/jose/test_unit_jwcrypto.py
--rw-r--r--   0 cochise    (501) staff       (20)      865 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/jose/test_unit_jwe.py
--rw-r--r--   0 cochise    (501) staff       (20)     1716 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/jose/test_unit_jws.py
--rw-r--r--   0 cochise    (501) staff       (20)     7117 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/jose/test_unit_payloadcodec.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.333798 ckms-0.63.0/tests/providers/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/providers/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.334214 ckms-0.63.0/tests/providers/azure/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/providers/azure/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2170 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/providers/azure/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1448 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/providers/azure/test_system_provider.py
--rw-r--r--   0 cochise    (501) staff       (20)     1758 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/providers/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.335005 ckms-0.63.0/tests/providers/google/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/providers/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     5603 2022-07-09 22:13:41.000000 ckms-0.63.0/tests/providers/google/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1626 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/providers/google/test_system_jwe.py
--rw-r--r--   0 cochise    (501) staff       (20)     1515 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/providers/google/test_system_jws.py
--rw-r--r--   0 cochise    (501) staff       (20)     1452 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/providers/google/test_system_provider.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-26 23:04:36.335593 ckms-0.63.0/tests/types/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1022 2022-07-09 19:16:55.000000 ckms-0.63.0/tests/types/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     1776 2022-07-09 11:28:18.000000 ckms-0.63.0/tests/types/test_unit_jsonwebkey.py
--rw-r--r--   0 cochise    (501) staff       (20)     1650 2022-07-09 11:28:17.000000 ckms-0.63.0/tests/types/test_unit_jsonwebkeyset.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.372083 ckms-0.64.0/
+-rw-r--r--   0 cochise    (501) staff       (20)      373 2022-07-09 11:28:18.000000 ckms-0.64.0/MANIFEST.in
+-rw-r--r--   0 cochise    (501) staff       (20)     2095 2023-07-05 15:02:16.371902 ckms-0.64.0/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)      354 2022-07-09 11:28:18.000000 ckms-0.64.0/README.md
+-rw-r--r--   0 cochise    (501) staff       (20)        7 2023-07-05 14:35:55.000000 ckms-0.64.0/VERSION
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.257350 ckms-0.64.0/ckms/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.261009 ckms-0.64.0/ckms/core/
+-rw-r--r--   0 cochise    (501) staff       (20)     2072 2023-07-05 15:01:31.000000 ckms-0.64.0/ckms/core/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2452 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/const.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.261492 ckms-0.64.0/ckms/core/exceptions/
+-rw-r--r--   0 cochise    (501) staff       (20)      764 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/exceptions/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1554 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/exceptions/malformed.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6577 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/keychain.py
+-rw-r--r--   0 cochise    (501) staff       (20)    26669 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/keyinspector.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.261792 ckms-0.64.0/ckms/core/local/
+-rw-r--r--   0 cochise    (501) staff       (20)    11096 2023-07-05 15:01:00.000000 ckms-0.64.0/ckms/core/local/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1912 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/core/local/models.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.264698 ckms-0.64.0/ckms/core/local/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     1416 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      994 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/core/local/types/contentencryptionkey.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2909 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/edwardscurvekeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2447 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/ellipticcurvekeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)      742 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/hmac.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1095 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/key.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1335 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/core/local/types/localkey.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1886 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/core/local/types/localkeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1080 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/parameterlesskey.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1961 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/rsakeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3688 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/core/local/types/symmetrickeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1128 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/local/types/transientkey.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.269069 ckms-0.64.0/ckms/core/models/
+-rw-r--r--   0 cochise    (501) staff       (20)     1533 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2600 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/basekeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2304 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/certificate.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1776 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/contentencryptionkey.py
+-rw-r--r--   0 cochise    (501) staff       (20)      973 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/core/models/joseheader_.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4769 2022-08-28 17:50:27.000000 ckms-0.64.0/ckms/core/models/joseobject.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1383 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/jsonb64.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3542 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/jsonwebencryption.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7005 2022-08-28 17:51:00.000000 ckms-0.64.0/ckms/core/models/jsonwebencryption_.py
+-rw-r--r--   0 cochise    (501) staff       (20)      605 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/jsonwebencryptionbase.py
+-rw-r--r--   0 cochise    (501) staff       (20)      707 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/jsonwebencryptionflattened.py
+-rw-r--r--   0 cochise    (501) staff       (20)      292 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/jsonwebencryptionrecipient.py
+-rw-r--r--   0 cochise    (501) staff       (20)      455 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/jsonwebencryptionwithrecipients.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6257 2023-03-26 23:04:13.000000 ckms-0.64.0/ckms/core/models/jsonwebsignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6941 2023-07-05 15:01:24.000000 ckms-0.64.0/ckms/core/models/keyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1407 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/octetb64.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4247 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/publickeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1108 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/recipient.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1582 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/remoteblobparams.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4114 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/models/signature.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.275086 ckms-0.64.0/ckms/core/provider/
+-rw-r--r--   0 cochise    (501) staff       (20)      654 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)    15351 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/core/provider/provider.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.277391 ckms-0.64.0/ckms/core/provider/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)     1357 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3553 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/asymmetricsigningtestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2399 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/baseprovidertestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3731 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/encryptiontestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1320 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/josebasetestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4483 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/joseconsumertestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7518 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/joseencryptiontestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5317 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/joseproducertestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)      840 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/providertestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3315 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/provider/tests/symmetricsigningtestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)      893 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/random.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1007 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/core/runlevel.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.277551 ckms-0.64.0/ckms/ext/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.285516 ckms-0.64.0/ckms/ext/asn1/
+-rw-r--r--   0 cochise    (501) staff       (20)     3536 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/asn1/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2274 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/asn1/fields.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.286214 ckms-0.64.0/ckms/ext/azure/
+-rw-r--r--   0 cochise    (501) staff       (20)      664 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/azure/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3811 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/azure/models.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1748 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/azure/provider.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.292048 ckms-0.64.0/ckms/ext/azure/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      734 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/azure/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1642 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/azure/types/azureconsumer.py
+-rw-r--r--   0 cochise    (501) staff       (20)      731 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/azure/types/iazureprovider.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.292586 ckms-0.64.0/ckms/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)      666 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)    10230 2023-07-05 15:01:08.000000 ckms-0.64.0/ckms/ext/google/provider.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.293460 ckms-0.64.0/ckms/ext/google/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      832 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/google/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      875 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/google/types/igoogleprovider.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6215 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/ext/google/types/keyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)      813 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/google/types/secretmanagerblob.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.293606 ckms-0.64.0/ckms/ext/pkcs/
+-rw-r--r--   0 cochise    (501) staff       (20)      759 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/oid.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.302397 ckms-0.64.0/ckms/ext/pkcs/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      660 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1095 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/types/attribute.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1633 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/types/contentinfo.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1439 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/types/issuerandserialnumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2361 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/types/signeddata.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4813 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/pkcs/types/signerinfo.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.252104 ckms-0.64.0/ckms/ext/rfc2459/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.302945 ckms-0.64.0/ckms/ext/rfc2459/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      705 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc2459/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2012 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc2459/types/relativedistinguishedname.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.303170 ckms-0.64.0/ckms/ext/rfc3161/
+-rw-r--r--   0 cochise    (501) staff       (20)      668 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc3161/oid.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.252271 ckms-0.64.0/ckms/ext/rfc5280/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.306866 ckms-0.64.0/ckms/ext/rfc5280/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     1099 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2657 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/algorithmidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1740 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/attribute.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1619 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/rdnsequence.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1533 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/relativedistinguishedname.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1106 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/signaturedigestalgorithmidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      946 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      804 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifiertype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3431 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5280/types/subjectpublickeyinfo.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.252383 ckms-0.64.0/ckms/ext/rfc5480/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.307504 ckms-0.64.0/ckms/ext/rfc5480/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      740 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5480/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1239 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5480/types/ecparameters.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1092 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5480/types/ellipticcurvetype.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.252488 ckms-0.64.0/ckms/ext/rfc5758/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.307858 ckms-0.64.0/ckms/ext/rfc5758/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      714 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5758/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1320 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/rfc5758/types/signaturedigestalgorithmtype.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.308741 ckms-0.64.0/ckms/ext/tsa/
+-rw-r--r--   0 cochise    (501) staff       (20)      937 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.309181 ckms-0.64.0/ckms/ext/tsa/certs/
+-rw-r--r--   0 cochise    (501) staff       (20)     2416 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/certs/DigiCertTrustedG4RSA4096SHA256TimeStampingCA.crt
+-rw-r--r--   0 cochise    (501) staff       (20)     1793 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/certs/digicert_tsa_2021.crt
+-rw-r--r--   0 cochise    (501) staff       (20)     3202 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/timestamper.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3545 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/timestampingauthority.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.311128 ckms-0.64.0/ckms/ext/tsa/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      977 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1279 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/algorithmidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1384 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/messageimprint.py
+-rw-r--r--   0 cochise    (501) staff       (20)      822 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/pkifailureinfo.py
+-rw-r--r--   0 cochise    (501) staff       (20)      760 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/pkistatus.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1989 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/pkistatusinfo.py
+-rw-r--r--   0 cochise    (501) staff       (20)      643 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/timestamp.py
+-rw-r--r--   0 cochise    (501) staff       (20)      671 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/timestampreq.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2251 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/timestampresp.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2921 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/timestamptoken.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2921 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/types/tstinfo.py
+-rw-r--r--   0 cochise    (501) staff       (20)      581 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/tsa/utils.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.252784 ckms-0.64.0/ckms/ext/x509/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.311746 ckms-0.64.0/ckms/ext/x509/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      743 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/x509/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1110 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/x509/types/algorithmidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      815 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/x509/types/certificate.py
+-rw-r--r--   0 cochise    (501) staff       (20)      650 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/ext/x509/types/tbscertificate.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.331302 ckms-0.64.0/ckms/jose/
+-rw-r--r--   0 cochise    (501) staff       (20)     1009 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6445 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/decoder.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4612 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/encoder.py
+-rw-r--r--   0 cochise    (501) staff       (20)      781 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/exceptions.py
+-rw-r--r--   0 cochise    (501) staff       (20)      941 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/joseheaderset.py
+-rw-r--r--   0 cochise    (501) staff       (20)    17752 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/josepayload.py
+-rw-r--r--   0 cochise    (501) staff       (20)      833 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/josepayloadcontainer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2181 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/jsonwebkeysetresolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1095 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/memoryissuercache.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1119 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/nullissuercache.py
+-rw-r--r--   0 cochise    (501) staff       (20)      896 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/nulltokenconsumer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     9965 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/payloadcodec.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2355 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/recipient.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1005 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/runlevel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2892 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/signature_.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4334 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/trustedissuers.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.331765 ckms-0.64.0/ckms/jose/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      750 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      882 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/types/baseissuercache.py
+-rw-r--r--   0 cochise    (501) staff       (20)      859 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/jose/types/basetokenconsumer.py
+-rw-r--r--   0 cochise    (501) staff       (20)       87 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/jose/validator.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.332145 ckms-0.64.0/ckms/lib/
+-rw-r--r--   0 cochise    (501) staff       (20)       19 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/lib/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)    22023 2023-07-05 15:00:21.000000 ckms-0.64.0/ckms/lib/dsnparse.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.332522 ckms-0.64.0/ckms/lib/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)      126 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/lib/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2626 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/lib/oauth2/openauthorizationclient.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.335092 ckms-0.64.0/ckms/main/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/main/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      784 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/main/__main__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2756 2023-07-05 15:01:48.000000 ckms-0.64.0/ckms/package.json
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.335510 ckms-0.64.0/ckms/pkix/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1065 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/oid.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.338640 ckms-0.64.0/ckms/pkix/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     1122 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1297 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/attribute.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2457 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/attributelist.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1076 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/basecertificateextension.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1439 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/basicconstraints.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4704 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/certificateextension.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4953 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/certificateextensionsequence.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6321 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/certificationrequest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2270 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/certificationrequestinfo.py
+-rw-r--r--   0 cochise    (501) staff       (20)      711 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/dnsname.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1193 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/extendedkeyusagetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1052 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/generalname.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1160 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/ipaddressname.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1352 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/name.py
+-rw-r--r--   0 cochise    (501) staff       (20)      747 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/pkix/types/uriname.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.354620 ckms-0.64.0/ckms/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     4778 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1082 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/aesalgorithmtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/aeskektype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      743 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/aeskeywrapoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2854 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/aesoperation.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.355253 ckms-0.64.0/ckms/types/algorithm/
+-rw-r--r--   0 cochise    (501) staff       (20)     8435 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/algorithm/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4474 2022-09-03 01:59:24.000000 ckms-0.64.0/ckms/types/algorithm/base.py
+-rw-r--r--   0 cochise    (501) staff       (20)      785 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/algorithm/nullalgorithm.py
+-rw-r--r--   0 cochise    (501) staff       (20)      768 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/asymmetricsigningoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1831 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/audiencetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1135 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ciphertext.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4455 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/claimset.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1581 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/cryptographicfailure.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1204 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/cryptographypublickeytype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4622 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/data.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1470 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/decrypter.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2530 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/digest.py
+-rw-r--r--   0 cochise    (501) staff       (20)      826 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/edsaoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)      874 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/edwardscurvealgorithmtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      767 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/edwardscurvetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      967 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ellipticcurvealgorithmtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1437 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ellipticcurveoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)      768 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ellipticcurvetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2429 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/encrypter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      789 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/encryptoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1227 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/forbiddenoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1001 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/generatekeyoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2106 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/generatekeyspec.py
+-rw-r--r--   0 cochise    (501) staff       (20)      757 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/hmacalgorithmtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      814 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/hmacoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2502 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/icontentencryptionkey.py
+-rw-r--r--   0 cochise    (501) staff       (20)      810 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ihasher.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1221 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ihttpclient.py
+-rw-r--r--   0 cochise    (501) staff       (20)      916 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ihttpresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3324 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ikeychain.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2584 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ikeyinspector.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2243 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ikeyspecification.py
+-rw-r--r--   0 cochise    (501) staff       (20)      976 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/invalidcredential.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2150 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/invalidtoken.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3000 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/ioperationperformer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6019 2023-07-05 15:00:42.000000 ckms-0.64.0/ckms/types/iprovider.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7767 2023-03-13 11:59:00.000000 ckms-0.64.0/ckms/types/jsonwebkey.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2808 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/types/jsonwebkeyset.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4372 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/jsonwebtoken.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1123 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/keyalgorithmtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      863 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/keyoperationtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      682 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/keyusetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      899 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/keywrapoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3259 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/malformed.py
+-rw-r--r--   0 cochise    (501) staff       (20)      826 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/message.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4384 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/operation.py
+-rw-r--r--   0 cochise    (501) staff       (20)      896 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/plaintext.py
+-rw-r--r--   0 cochise    (501) staff       (20)      988 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/rsaalgorithmtype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1574 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/rsaoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)    27072 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/servermetadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1902 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/signer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1072 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/signingoperation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2719 2022-10-05 17:44:31.000000 ckms-0.64.0/ckms/types/trustissues.py
+-rw-r--r--   0 cochise    (501) staff       (20)      716 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/undecryptable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1777 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/types/verifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2873 2022-08-19 20:55:57.000000 ckms-0.64.0/ckms/utils.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.259431 ckms-0.64.0/ckms.egg-info/
+-rw-r--r--   0 cochise    (501) staff       (20)     2095 2023-07-05 15:02:16.000000 ckms-0.64.0/ckms.egg-info/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)     9732 2023-07-05 15:02:16.000000 ckms-0.64.0/ckms.egg-info/SOURCES.txt
+-rw-r--r--   0 cochise    (501) staff       (20)        1 2023-07-05 15:02:16.000000 ckms-0.64.0/ckms.egg-info/dependency_links.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       97 2023-07-05 15:02:16.000000 ckms-0.64.0/ckms.egg-info/entry_points.txt
+-rw-r--r--   0 cochise    (501) staff       (20)      724 2023-07-05 15:02:16.000000 ckms-0.64.0/ckms.egg-info/requires.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       43 2023-07-05 15:02:16.000000 ckms-0.64.0/ckms.egg-info/top_level.txt
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.253505 ckms-0.64.0/docs/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.356232 ckms-0.64.0/docs/source/
+-rw-r--r--   0 cochise    (501) staff       (20)     2410 2022-07-09 11:28:13.000000 ckms-0.64.0/docs/source/conf.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.358391 ckms-0.64.0/examples/
+-rw-r--r--   0 cochise    (501) staff       (20)      506 2022-07-09 11:28:16.000000 ckms-0.64.0/examples/google-aes.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5422 2022-07-09 11:28:16.000000 ckms-0.64.0/examples/google-kms.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1201 2022-07-09 11:28:13.000000 ckms-0.64.0/examples/intro-jose.py
+-rw-r--r--   0 cochise    (501) staff       (20)      591 2022-07-09 11:28:13.000000 ckms-0.64.0/examples/intro.py
+-rw-r--r--   0 cochise    (501) staff       (20)      887 2022-07-09 11:28:15.000000 ckms-0.64.0/examples/issuers.py
+-rw-r--r--   0 cochise    (501) staff       (20)      789 2022-07-09 11:28:16.000000 ckms-0.64.0/examples/local.py
+-rw-r--r--   0 cochise    (501) staff       (20)      218 2022-07-09 11:28:15.000000 ckms-0.64.0/examples/oauth2_metadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)      153 2022-07-09 11:28:17.000000 ckms-0.64.0/examples/settings.py
+-rw-r--r--   0 cochise    (501) staff       (20)       48 2022-07-09 11:28:12.000000 ckms-0.64.0/pyproject.toml
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-07-05 15:02:16.372124 ckms-0.64.0/setup.cfg
+-rw-r--r--   0 cochise    (501) staff       (20)     1274 2022-07-09 11:28:12.000000 ckms-0.64.0/setup.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.358769 ckms-0.64.0/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:12.000000 ckms-0.64.0/tests/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7435 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/conftest.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.362597 ckms-0.64.0/tests/core/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:15.000000 ckms-0.64.0/tests/core/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4021 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/basedatatestcase.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3350 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1625 2022-07-11 07:42:21.000000 ckms-0.64.0/tests/core/test_system_jwk_certificate.py
+-rw-r--r--   0 cochise    (501) staff       (20)      940 2022-07-09 11:28:16.000000 ckms-0.64.0/tests/core/test_unit_blob_local.py
+-rw-r--r--   0 cochise    (501) staff       (20)      720 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_data.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2162 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_digest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2134 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/core/test_unit_jose_consumer_jwcrypto.py
+-rw-r--r--   0 cochise    (501) staff       (20)      861 2022-07-09 11:28:16.000000 ckms-0.64.0/tests/core/test_unit_jose_parse.py
+-rw-r--r--   0 cochise    (501) staff       (20)     8831 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_keychain.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3049 2022-07-09 11:28:15.000000 ckms-0.64.0/tests/core/test_unit_keyinspector.py
+-rw-r--r--   0 cochise    (501) staff       (20)      754 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_message.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3305 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_models_jose_deserialize.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4597 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_models_jwe.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4980 2022-07-09 11:28:16.000000 ckms-0.64.0/tests/core/test_unit_provider.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6803 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/core/test_unit_provider_local.py
+-rw-r--r--   0 cochise    (501) staff       (20)      198 2022-07-09 11:28:16.000000 ckms-0.64.0/tests/core/test_unit_random.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.362874 ckms-0.64.0/tests/ext/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/ext/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.363070 ckms-0.64.0/tests/ext/rfc2986/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/rfc2986/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3850 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/rfc2986/test_unit_csr.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.365507 ckms-0.64.0/tests/ext/tsa/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1378 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)      803 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_accv.py
+-rw-r--r--   0 cochise    (501) staff       (20)      807 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_apple.py
+-rw-r--r--   0 cochise    (501) staff       (20)      892 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_digicert.py
+-rw-r--r--   0 cochise    (501) staff       (20)      844 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_globalsign.py
+-rw-r--r--   0 cochise    (501) staff       (20)      797 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_izenpe.py
+-rw-r--r--   0 cochise    (501) staff       (20)      810 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_keynectis.py
+-rw-r--r--   0 cochise    (501) staff       (20)      823 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_quovadis.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1646 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/test_system_timestamper_multi.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1255 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/ext/tsa/tsatests.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.365749 ckms-0.64.0/tests/impl/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:13.000000 ckms-0.64.0/tests/impl/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)       19 2022-07-09 11:28:13.000000 ckms-0.64.0/tests/impl/conftest.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.366727 ckms-0.64.0/tests/impl/google/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:13.000000 ckms-0.64.0/tests/impl/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3220 2022-07-09 11:28:13.000000 ckms-0.64.0/tests/impl/google/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)      410 2022-07-09 11:28:13.000000 ckms-0.64.0/tests/impl/google/test_integration_signing.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.368465 ckms-0.64.0/tests/jose/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:13.000000 ckms-0.64.0/tests/jose/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2242 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/jose/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1527 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/jose/test_system_trustedissuers_google.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4604 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/jose/test_unit_claimset_jwt.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3062 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/jose/test_unit_jwcrypto.py
+-rw-r--r--   0 cochise    (501) staff       (20)      865 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/jose/test_unit_jwe.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1716 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/jose/test_unit_jws.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7117 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/jose/test_unit_payloadcodec.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.368960 ckms-0.64.0/tests/providers/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/providers/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.369570 ckms-0.64.0/tests/providers/azure/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/providers/azure/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2170 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/providers/azure/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1448 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/providers/azure/test_system_provider.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1758 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/providers/conftest.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.370838 ckms-0.64.0/tests/providers/google/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/providers/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5603 2022-07-09 22:13:41.000000 ckms-0.64.0/tests/providers/google/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1626 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/providers/google/test_system_jwe.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1515 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/providers/google/test_system_jws.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1452 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/providers/google/test_system_provider.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-07-05 15:02:16.371561 ckms-0.64.0/tests/types/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1022 2022-07-09 19:16:55.000000 ckms-0.64.0/tests/types/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1776 2022-07-09 11:28:18.000000 ckms-0.64.0/tests/types/test_unit_jsonwebkey.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1650 2022-07-09 11:28:17.000000 ckms-0.64.0/tests/types/test_unit_jsonwebkeyset.py
```

### Comparing `ckms-0.63.0/PKG-INFO` & `ckms-0.64.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckms
-Version: 0.63.0
+Version: 0.64.0
 Summary: Enter a description for this Unimatrix package
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `ckms-0.63.0/ckms/core/__init__.py` & `ckms-0.64.0/ckms/core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # type: ignore
 from typing import Any
 
-import dsnparse
-
+from ckms.lib import dsnparse
 from .keychain import get_default_keychain
 from .keychain import Keychain
 from .keyinspector import KeyInspector
 from .provider import Provider
 from .models import RemoteBlobParams as RemoteBlob
 from .models import KeySpecification
```

### Comparing `ckms-0.63.0/ckms/core/const.py` & `ckms-0.64.0/ckms/core/const.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/exceptions/__init__.py` & `ckms-0.64.0/ckms/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/exceptions/malformed.py` & `ckms-0.64.0/ckms/core/exceptions/malformed.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/keychain.py` & `ckms-0.64.0/ckms/core/keychain.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/keyinspector.py` & `ckms-0.64.0/ckms/core/keyinspector.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/__init__.py` & `ckms-0.64.0/ckms/core/local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import functools
 import hmac
 import inspect
 from typing import cast
 from typing import Any
 
 import aiofiles
-import dsnparse
 from ckms.types import CipherText
 from ckms.types import HMACOperation
 from cryptography.exceptions import InvalidSignature
 from cryptography.exceptions import InvalidTag
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric import padding
@@ -32,14 +31,15 @@
 from cryptography.hazmat.primitives.ciphers import algorithms
 from cryptography.hazmat.primitives.ciphers import AEADCipherContext
 from cryptography.hazmat.primitives.keywrap import aes_key_unwrap
 
 import ckms.types
 from ckms import core
 from ckms.core.provider import Provider
+from ckms.lib import dsnparse
 from ckms.utils import bytes_to_number
 from ckms.utils import number_to_bytes
 from .types import HMAC
 from .types import Key
 from .models import KeySpecification
 
 
@@ -72,15 +72,15 @@
         if inspect.isawaitable(result):
             result = await result
         return result
 
 
     def parse_dsn(self, dsn: dsnparse.ParseResult) -> KeySpecification:
         return {
-            **dsn.query, # type: ignore
+            **dsn.query_params, # type: ignore
             'provider': 'local',
             'key': {'path': dsn.path[1:]} # type: ignore
         }
 
     @functools.singledispatchmethod
     def _generate(self, spec: Any) -> Any:
         raise NotImplementedError(repr(spec))
@@ -297,8 +297,8 @@
                 signature=op.signature,
                 data=await op.get_digest(),
                 padding=self.get_padding(op.padding, op.digest),
                 algorithm=utils.Prehashed(self.get_digest_algorithm(op.digest))
             )
             return True
         except InvalidSignature:
-            return False
+            return False
```

### Comparing `ckms-0.63.0/ckms/core/local/models.py` & `ckms-0.64.0/ckms/core/local/models.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/__init__.py` & `ckms-0.64.0/ckms/core/local/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/contentencryptionkey.py` & `ckms-0.64.0/ckms/core/local/types/contentencryptionkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/edwardscurvekeyspecification.py` & `ckms-0.64.0/ckms/core/local/types/edwardscurvekeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/ellipticcurvekeyspecification.py` & `ckms-0.64.0/ckms/core/local/types/ellipticcurvekeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/hmac.py` & `ckms-0.64.0/ckms/core/local/types/hmac.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/key.py` & `ckms-0.64.0/ckms/core/local/types/key.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/localkey.py` & `ckms-0.64.0/ckms/core/local/types/localkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/localkeyspecification.py` & `ckms-0.64.0/ckms/core/local/types/localkeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/parameterlesskey.py` & `ckms-0.64.0/ckms/core/local/types/parameterlesskey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/rsakeyspecification.py` & `ckms-0.64.0/ckms/core/local/types/rsakeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/symmetrickeyspecification.py` & `ckms-0.64.0/ckms/core/local/types/symmetrickeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/local/types/transientkey.py` & `ckms-0.64.0/ckms/core/local/types/transientkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/__init__.py` & `ckms-0.64.0/ckms/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/basekeyspecification.py` & `ckms-0.64.0/ckms/core/models/basekeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/certificate.py` & `ckms-0.64.0/ckms/core/models/certificate.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/contentencryptionkey.py` & `ckms-0.64.0/ckms/core/models/contentencryptionkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/joseheader_.py` & `ckms-0.64.0/ckms/core/models/joseheader_.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/joseobject.py` & `ckms-0.64.0/ckms/core/models/joseobject.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/jsonb64.py` & `ckms-0.64.0/ckms/core/models/jsonb64.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/jsonwebencryption.py` & `ckms-0.64.0/ckms/core/models/jsonwebencryption.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/jsonwebencryption_.py` & `ckms-0.64.0/ckms/core/models/jsonwebencryption_.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/jsonwebencryptionbase.py` & `ckms-0.64.0/ckms/core/models/jsonwebencryptionbase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/jsonwebencryptionflattened.py` & `ckms-0.64.0/ckms/core/models/jsonwebencryptionflattened.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/jsonwebsignature.py` & `ckms-0.64.0/ckms/core/models/jsonwebsignature.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/keyspecification.py` & `ckms-0.64.0/ckms/core/models/keyspecification.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Declares :class:`KeySpecification`."""
 from typing import Any
 from typing import Generator
 
-import dsnparse
 import pydantic
 
 from ckms.core import const
+from ckms.lib import dsnparse
 from ckms.types import Algorithm
 from ckms.types import Decrypter
 from ckms.types import Encrypter
 from ckms.types import IKeyInspector
 from ckms.types import IProvider
 from ckms.types import JSONWebKey
 from ckms.types import KeyOperationType
```

### Comparing `ckms-0.63.0/ckms/core/models/octetb64.py` & `ckms-0.64.0/ckms/core/models/octetb64.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/publickeyspecification.py` & `ckms-0.64.0/ckms/core/models/publickeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/recipient.py` & `ckms-0.64.0/ckms/core/models/recipient.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/remoteblobparams.py` & `ckms-0.64.0/ckms/core/models/remoteblobparams.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/models/signature.py` & `ckms-0.64.0/ckms/core/models/signature.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/__init__.py` & `ckms-0.64.0/ckms/core/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/provider.py` & `ckms-0.64.0/ckms/core/provider/provider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/__init__.py` & `ckms-0.64.0/ckms/core/provider/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/asymmetricsigningtestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/asymmetricsigningtestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/baseprovidertestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/baseprovidertestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/encryptiontestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/encryptiontestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/josebasetestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/josebasetestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/joseconsumertestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/joseconsumertestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/joseencryptiontestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/joseencryptiontestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/joseproducertestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/joseproducertestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/providertestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/providertestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/provider/tests/symmetricsigningtestcase.py` & `ckms-0.64.0/ckms/core/provider/tests/symmetricsigningtestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/random.py` & `ckms-0.64.0/ckms/core/random.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/core/runlevel.py` & `ckms-0.64.0/ckms/core/runlevel.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/asn1/__init__.py` & `ckms-0.64.0/ckms/ext/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/asn1/fields.py` & `ckms-0.64.0/ckms/ext/asn1/fields.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/azure/__init__.py` & `ckms-0.64.0/ckms/ext/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/azure/models.py` & `ckms-0.64.0/ckms/ext/azure/models.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/azure/provider.py` & `ckms-0.64.0/ckms/ext/azure/provider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/azure/types/__init__.py` & `ckms-0.64.0/ckms/ext/azure/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/azure/types/azureconsumer.py` & `ckms-0.64.0/ckms/ext/azure/types/azureconsumer.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/azure/types/iazureprovider.py` & `ckms-0.64.0/ckms/ext/azure/types/iazureprovider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/google/__init__.py` & `ckms-0.64.0/ckms/ext/google/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/google/provider.py` & `ckms-0.64.0/ckms/ext/google/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # type: ignore
 from typing import cast
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 
 import crcmod
-import dsnparse
 import google.auth
 from google.api_core.exceptions import InvalidArgument
 from google.auth.credentials import Credentials
 from google.cloud.kms import AsymmetricDecryptResponse
 from google.cloud.kms import DecryptResponse
 from google.cloud.kms import KeyManagementServiceAsyncClient
 from google.cloud.secretmanager import SecretManagerServiceAsyncClient
 
 from ckms import core
+from ckms.lib import dsnparse
 from ckms.utils import normalize_ec_signature
 from ckms.types import AESOperation
 from ckms.types import CipherText
 from ckms.types import EllipticCurveOperation
 from ckms.types import HMACOperation
 from ckms.types import RSAOperation
 from ckms.types import SigningOperation
```

### Comparing `ckms-0.63.0/ckms/ext/google/types/__init__.py` & `ckms-0.64.0/ckms/ext/google/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/google/types/igoogleprovider.py` & `ckms-0.64.0/ckms/ext/google/types/igoogleprovider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/google/types/keyspecification.py` & `ckms-0.64.0/ckms/ext/google/types/keyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/google/types/secretmanagerblob.py` & `ckms-0.64.0/ckms/ext/google/types/secretmanagerblob.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/oid.py` & `ckms-0.64.0/ckms/ext/pkcs/oid.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/types/__init__.py` & `ckms-0.64.0/ckms/ext/pkcs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/types/attribute.py` & `ckms-0.64.0/ckms/ext/pkcs/types/attribute.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/types/contentinfo.py` & `ckms-0.64.0/ckms/ext/pkcs/types/contentinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/types/issuerandserialnumber.py` & `ckms-0.64.0/ckms/ext/pkcs/types/issuerandserialnumber.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/types/signeddata.py` & `ckms-0.64.0/ckms/ext/pkcs/types/signeddata.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/pkcs/types/signerinfo.py` & `ckms-0.64.0/ckms/ext/pkcs/types/signerinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc2459/types/__init__.py` & `ckms-0.64.0/ckms/ext/rfc2459/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc2459/types/relativedistinguishedname.py` & `ckms-0.64.0/ckms/ext/rfc2459/types/relativedistinguishedname.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc3161/oid.py` & `ckms-0.64.0/ckms/ext/rfc3161/oid.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/__init__.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/algorithmidentifier.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/algorithmidentifier.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/attribute.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/attribute.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/rdnsequence.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/rdnsequence.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/relativedistinguishedname.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/relativedistinguishedname.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/signaturedigestalgorithmidentifier.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/signaturedigestalgorithmidentifier.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifier.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifier.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifiertype.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/subjectpublickeyalgorithmidentifiertype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5280/types/subjectpublickeyinfo.py` & `ckms-0.64.0/ckms/ext/rfc5280/types/subjectpublickeyinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5480/types/__init__.py` & `ckms-0.64.0/ckms/ext/rfc5480/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5480/types/ecparameters.py` & `ckms-0.64.0/ckms/ext/rfc5480/types/ecparameters.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5480/types/ellipticcurvetype.py` & `ckms-0.64.0/ckms/ext/rfc5480/types/ellipticcurvetype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5758/types/__init__.py` & `ckms-0.64.0/ckms/ext/rfc5758/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/rfc5758/types/signaturedigestalgorithmtype.py` & `ckms-0.64.0/ckms/ext/rfc5758/types/signaturedigestalgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/__init__.py` & `ckms-0.64.0/ckms/ext/tsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/certs/DigiCertTrustedG4RSA4096SHA256TimeStampingCA.crt` & `ckms-0.64.0/ckms/ext/tsa/certs/DigiCertTrustedG4RSA4096SHA256TimeStampingCA.crt`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/certs/digicert_tsa_2021.crt` & `ckms-0.64.0/ckms/ext/tsa/certs/digicert_tsa_2021.crt`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/timestamper.py` & `ckms-0.64.0/ckms/ext/tsa/timestamper.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/timestampingauthority.py` & `ckms-0.64.0/ckms/ext/tsa/timestampingauthority.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/__init__.py` & `ckms-0.64.0/ckms/ext/tsa/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/algorithmidentifier.py` & `ckms-0.64.0/ckms/ext/tsa/types/algorithmidentifier.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/messageimprint.py` & `ckms-0.64.0/ckms/ext/tsa/types/messageimprint.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/pkifailureinfo.py` & `ckms-0.64.0/ckms/ext/tsa/types/pkifailureinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/pkistatus.py` & `ckms-0.64.0/ckms/ext/tsa/types/pkistatus.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/pkistatusinfo.py` & `ckms-0.64.0/ckms/ext/tsa/types/pkistatusinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/timestamp.py` & `ckms-0.64.0/ckms/ext/tsa/types/timestamp.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/timestampreq.py` & `ckms-0.64.0/ckms/ext/tsa/types/timestampreq.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/timestampresp.py` & `ckms-0.64.0/ckms/ext/tsa/types/timestampresp.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/timestamptoken.py` & `ckms-0.64.0/ckms/ext/tsa/types/timestamptoken.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/types/tstinfo.py` & `ckms-0.64.0/ckms/ext/tsa/types/tstinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/tsa/utils.py` & `ckms-0.64.0/ckms/ext/tsa/utils.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/x509/types/__init__.py` & `ckms-0.64.0/ckms/ext/x509/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/x509/types/algorithmidentifier.py` & `ckms-0.64.0/ckms/ext/x509/types/algorithmidentifier.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/x509/types/certificate.py` & `ckms-0.64.0/ckms/ext/x509/types/certificate.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/ext/x509/types/tbscertificate.py` & `ckms-0.64.0/ckms/ext/x509/types/tbscertificate.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/__init__.py` & `ckms-0.64.0/ckms/jose/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/decoder.py` & `ckms-0.64.0/ckms/jose/decoder.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/encoder.py` & `ckms-0.64.0/ckms/jose/encoder.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/exceptions.py` & `ckms-0.64.0/ckms/jose/exceptions.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/joseheaderset.py` & `ckms-0.64.0/ckms/jose/joseheaderset.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/josepayload.py` & `ckms-0.64.0/ckms/jose/josepayload.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/josepayloadcontainer.py` & `ckms-0.64.0/ckms/jose/josepayloadcontainer.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/jsonwebkeysetresolver.py` & `ckms-0.64.0/ckms/jose/jsonwebkeysetresolver.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/memoryissuercache.py` & `ckms-0.64.0/ckms/jose/memoryissuercache.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/nullissuercache.py` & `ckms-0.64.0/ckms/jose/nullissuercache.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/nulltokenconsumer.py` & `ckms-0.64.0/ckms/jose/nulltokenconsumer.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/payloadcodec.py` & `ckms-0.64.0/ckms/jose/payloadcodec.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/recipient.py` & `ckms-0.64.0/ckms/jose/recipient.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/runlevel.py` & `ckms-0.64.0/ckms/jose/runlevel.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/signature_.py` & `ckms-0.64.0/ckms/jose/signature_.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/trustedissuers.py` & `ckms-0.64.0/ckms/jose/trustedissuers.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/types/__init__.py` & `ckms-0.64.0/ckms/jose/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/types/baseissuercache.py` & `ckms-0.64.0/ckms/jose/types/baseissuercache.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/jose/types/basetokenconsumer.py` & `ckms-0.64.0/ckms/jose/types/basetokenconsumer.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/lib/oauth2/openauthorizationclient.py` & `ckms-0.64.0/ckms/lib/oauth2/openauthorizationclient.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/main/__main__.py` & `ckms-0.64.0/ckms/main/__main__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/package.json` & `ckms-0.64.0/ckms/package.json`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/oid.py` & `ckms-0.64.0/ckms/pkix/oid.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/__init__.py` & `ckms-0.64.0/ckms/pkix/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/attribute.py` & `ckms-0.64.0/ckms/pkix/types/attribute.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/attributelist.py` & `ckms-0.64.0/ckms/pkix/types/attributelist.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/basecertificateextension.py` & `ckms-0.64.0/ckms/pkix/types/basecertificateextension.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/basicconstraints.py` & `ckms-0.64.0/ckms/pkix/types/basicconstraints.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/certificateextension.py` & `ckms-0.64.0/ckms/pkix/types/certificateextension.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/certificateextensionsequence.py` & `ckms-0.64.0/ckms/pkix/types/certificateextensionsequence.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/certificationrequest.py` & `ckms-0.64.0/ckms/pkix/types/certificationrequest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/certificationrequestinfo.py` & `ckms-0.64.0/ckms/pkix/types/certificationrequestinfo.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/dnsname.py` & `ckms-0.64.0/ckms/pkix/types/dnsname.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/extendedkeyusagetype.py` & `ckms-0.64.0/ckms/pkix/types/extendedkeyusagetype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/generalname.py` & `ckms-0.64.0/ckms/pkix/types/generalname.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/ipaddressname.py` & `ckms-0.64.0/ckms/pkix/types/ipaddressname.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/name.py` & `ckms-0.64.0/ckms/pkix/types/name.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/pkix/types/uriname.py` & `ckms-0.64.0/ckms/pkix/types/uriname.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/__init__.py` & `ckms-0.64.0/ckms/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/aesalgorithmtype.py` & `ckms-0.64.0/ckms/types/aesalgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/aeskeywrapoperation.py` & `ckms-0.64.0/ckms/types/aeskeywrapoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/aesoperation.py` & `ckms-0.64.0/ckms/types/aesoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/algorithm/__init__.py` & `ckms-0.64.0/ckms/types/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/algorithm/base.py` & `ckms-0.64.0/ckms/types/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/algorithm/nullalgorithm.py` & `ckms-0.64.0/ckms/types/algorithm/nullalgorithm.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/asymmetricsigningoperation.py` & `ckms-0.64.0/ckms/types/asymmetricsigningoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/audiencetype.py` & `ckms-0.64.0/ckms/types/audiencetype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ciphertext.py` & `ckms-0.64.0/ckms/types/ciphertext.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/claimset.py` & `ckms-0.64.0/ckms/types/claimset.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/cryptographicfailure.py` & `ckms-0.64.0/ckms/types/cryptographicfailure.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/cryptographypublickeytype.py` & `ckms-0.64.0/ckms/types/cryptographypublickeytype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/data.py` & `ckms-0.64.0/ckms/types/data.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/decrypter.py` & `ckms-0.64.0/ckms/types/decrypter.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/digest.py` & `ckms-0.64.0/ckms/types/digest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/edsaoperation.py` & `ckms-0.64.0/ckms/types/edsaoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/edwardscurvealgorithmtype.py` & `ckms-0.64.0/ckms/types/edwardscurvealgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/edwardscurvetype.py` & `ckms-0.64.0/ckms/types/edwardscurvetype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ellipticcurvealgorithmtype.py` & `ckms-0.64.0/ckms/types/ellipticcurvealgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ellipticcurveoperation.py` & `ckms-0.64.0/ckms/types/ellipticcurveoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ellipticcurvetype.py` & `ckms-0.64.0/ckms/types/ellipticcurvetype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/encrypter.py` & `ckms-0.64.0/ckms/types/encrypter.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/encryptoperation.py` & `ckms-0.64.0/ckms/types/encryptoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/forbiddenoperation.py` & `ckms-0.64.0/ckms/types/forbiddenoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/generatekeyoperation.py` & `ckms-0.64.0/ckms/types/generatekeyoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/generatekeyspec.py` & `ckms-0.64.0/ckms/types/generatekeyspec.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/hmacalgorithmtype.py` & `ckms-0.64.0/ckms/types/hmacalgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/hmacoperation.py` & `ckms-0.64.0/ckms/types/hmacoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/icontentencryptionkey.py` & `ckms-0.64.0/ckms/types/icontentencryptionkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ihasher.py` & `ckms-0.64.0/ckms/types/ihasher.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ihttpclient.py` & `ckms-0.64.0/ckms/types/ihttpclient.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ihttpresponse.py` & `ckms-0.64.0/ckms/types/ihttpresponse.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ikeychain.py` & `ckms-0.64.0/ckms/types/ikeychain.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ikeyinspector.py` & `ckms-0.64.0/ckms/types/ikeyinspector.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ikeyspecification.py` & `ckms-0.64.0/ckms/types/ikeyspecification.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/invalidcredential.py` & `ckms-0.64.0/ckms/types/invalidcredential.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/invalidtoken.py` & `ckms-0.64.0/ckms/types/invalidtoken.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/ioperationperformer.py` & `ckms-0.64.0/ckms/types/ioperationperformer.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/iprovider.py` & `ckms-0.64.0/ckms/types/iprovider.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Generator
 from typing import TypeAlias
 from typing import Union
 
-import dsnparse
 from unimatrix.exceptions import CanonicalException
 
+from ckms.lib import dsnparse
 from .generatekeyoperation import GenerateKeyOperation
 from .ikeyinspector import IKeyInspector
 from .undecryptable import Undecryptable # type: ignore
 
 
 class IProvider:
     __module__: str = 'cbra.types'
```

### Comparing `ckms-0.63.0/ckms/types/jsonwebkey.py` & `ckms-0.64.0/ckms/types/jsonwebkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/jsonwebkeyset.py` & `ckms-0.64.0/ckms/types/jsonwebkeyset.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/jsonwebtoken.py` & `ckms-0.64.0/ckms/types/jsonwebtoken.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/keyalgorithmtype.py` & `ckms-0.64.0/ckms/types/keyalgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/keyoperationtype.py` & `ckms-0.64.0/ckms/types/keyoperationtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/keyusetype.py` & `ckms-0.64.0/ckms/types/keyusetype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/keywrapoperation.py` & `ckms-0.64.0/ckms/types/keywrapoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/malformed.py` & `ckms-0.64.0/ckms/types/malformed.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/message.py` & `ckms-0.64.0/ckms/types/message.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/operation.py` & `ckms-0.64.0/ckms/types/operation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/plaintext.py` & `ckms-0.64.0/ckms/types/plaintext.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/rsaalgorithmtype.py` & `ckms-0.64.0/ckms/types/rsaalgorithmtype.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/rsaoperation.py` & `ckms-0.64.0/ckms/types/rsaoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/servermetadata.py` & `ckms-0.64.0/ckms/types/servermetadata.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/signer.py` & `ckms-0.64.0/ckms/types/signer.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/signingoperation.py` & `ckms-0.64.0/ckms/types/signingoperation.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/trustissues.py` & `ckms-0.64.0/ckms/types/trustissues.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/undecryptable.py` & `ckms-0.64.0/ckms/types/undecryptable.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/types/verifier.py` & `ckms-0.64.0/ckms/types/verifier.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms/utils.py` & `ckms-0.64.0/ckms/utils.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/ckms.egg-info/PKG-INFO` & `ckms-0.64.0/ckms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckms
-Version: 0.63.0
+Version: 0.64.0
 Summary: Enter a description for this Unimatrix package
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `ckms-0.63.0/ckms.egg-info/SOURCES.txt` & `ckms-0.64.0/ckms.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 ckms/jose/signature_.py
 ckms/jose/trustedissuers.py
 ckms/jose/validator.py
 ckms/jose/types/__init__.py
 ckms/jose/types/baseissuercache.py
 ckms/jose/types/basetokenconsumer.py
 ckms/lib/__init__.py
+ckms/lib/dsnparse.py
 ckms/lib/oauth2/__init__.py
 ckms/lib/oauth2/openauthorizationclient.py
 ckms/main/__init__.py
 ckms/main/__main__.py
 ckms/pkix/__init__.py
 ckms/pkix/oid.py
 ckms/pkix/types/__init__.py
```

### Comparing `ckms-0.63.0/ckms.egg-info/requires.txt` & `ckms-0.64.0/ckms.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/docs/source/conf.py` & `ckms-0.64.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/examples/google-kms.py` & `ckms-0.64.0/examples/google-kms.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/examples/intro-jose.py` & `ckms-0.64.0/examples/intro-jose.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/examples/intro.py` & `ckms-0.64.0/examples/intro.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/examples/issuers.py` & `ckms-0.64.0/examples/issuers.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/examples/local.py` & `ckms-0.64.0/examples/local.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/setup.py` & `ckms-0.64.0/setup.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/conftest.py` & `ckms-0.64.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/basedatatestcase.py` & `ckms-0.64.0/tests/core/basedatatestcase.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/conftest.py` & `ckms-0.64.0/tests/core/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_system_jwk_certificate.py` & `ckms-0.64.0/tests/core/test_system_jwk_certificate.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_blob_local.py` & `ckms-0.64.0/tests/core/test_unit_blob_local.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_data.py` & `ckms-0.64.0/tests/core/test_unit_data.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_digest.py` & `ckms-0.64.0/tests/core/test_unit_digest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_jose_consumer_jwcrypto.py` & `ckms-0.64.0/tests/core/test_unit_jose_consumer_jwcrypto.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_jose_parse.py` & `ckms-0.64.0/tests/core/test_unit_jose_parse.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_keychain.py` & `ckms-0.64.0/tests/core/test_unit_keychain.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_keyinspector.py` & `ckms-0.64.0/tests/core/test_unit_keyinspector.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_message.py` & `ckms-0.64.0/tests/core/test_unit_message.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_models_jose_deserialize.py` & `ckms-0.64.0/tests/core/test_unit_models_jose_deserialize.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_models_jwe.py` & `ckms-0.64.0/tests/core/test_unit_models_jwe.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_provider.py` & `ckms-0.64.0/tests/core/test_unit_provider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/core/test_unit_provider_local.py` & `ckms-0.64.0/tests/core/test_unit_provider_local.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/rfc2986/test_unit_csr.py` & `ckms-0.64.0/tests/ext/rfc2986/test_unit_csr.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/conftest.py` & `ckms-0.64.0/tests/ext/tsa/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_accv.py` & `ckms-0.64.0/tests/ext/tsa/test_system_accv.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_apple.py` & `ckms-0.64.0/tests/ext/tsa/test_system_apple.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_digicert.py` & `ckms-0.64.0/tests/ext/tsa/test_system_digicert.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_globalsign.py` & `ckms-0.64.0/tests/ext/tsa/test_system_globalsign.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_izenpe.py` & `ckms-0.64.0/tests/ext/tsa/test_system_izenpe.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_keynectis.py` & `ckms-0.64.0/tests/ext/tsa/test_system_keynectis.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_quovadis.py` & `ckms-0.64.0/tests/ext/tsa/test_system_quovadis.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/test_system_timestamper_multi.py` & `ckms-0.64.0/tests/ext/tsa/test_system_timestamper_multi.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/ext/tsa/tsatests.py` & `ckms-0.64.0/tests/ext/tsa/tsatests.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/impl/google/conftest.py` & `ckms-0.64.0/tests/impl/google/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/conftest.py` & `ckms-0.64.0/tests/jose/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/test_system_trustedissuers_google.py` & `ckms-0.64.0/tests/jose/test_system_trustedissuers_google.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/test_unit_claimset_jwt.py` & `ckms-0.64.0/tests/jose/test_unit_claimset_jwt.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/test_unit_jwcrypto.py` & `ckms-0.64.0/tests/jose/test_unit_jwcrypto.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/test_unit_jwe.py` & `ckms-0.64.0/tests/jose/test_unit_jwe.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/test_unit_jws.py` & `ckms-0.64.0/tests/jose/test_unit_jws.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/jose/test_unit_payloadcodec.py` & `ckms-0.64.0/tests/jose/test_unit_payloadcodec.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/azure/conftest.py` & `ckms-0.64.0/tests/providers/azure/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/azure/test_system_provider.py` & `ckms-0.64.0/tests/providers/azure/test_system_provider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/conftest.py` & `ckms-0.64.0/tests/providers/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/google/conftest.py` & `ckms-0.64.0/tests/providers/google/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/google/test_system_jwe.py` & `ckms-0.64.0/tests/providers/google/test_system_jwe.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/google/test_system_jws.py` & `ckms-0.64.0/tests/providers/google/test_system_jws.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/providers/google/test_system_provider.py` & `ckms-0.64.0/tests/providers/google/test_system_provider.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/types/conftest.py` & `ckms-0.64.0/tests/types/conftest.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/types/test_unit_jsonwebkey.py` & `ckms-0.64.0/tests/types/test_unit_jsonwebkey.py`

 * *Files identical despite different names*

### Comparing `ckms-0.63.0/tests/types/test_unit_jsonwebkeyset.py` & `ckms-0.64.0/tests/types/test_unit_jsonwebkeyset.py`

 * *Files identical despite different names*

