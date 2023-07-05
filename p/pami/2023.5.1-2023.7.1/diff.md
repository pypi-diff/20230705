# Comparing `tmp/pami-2023.5.1.tar.gz` & `tmp/pami-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.5.1.tar", last modified: Tue Jun 20 07:29:48 2023, max compression
+gzip compressed data, was "pami-2023.7.1.tar", last modified: Wed Jul  5 02:40:46 2023, max compression
```

## Comparing `pami-2023.5.1.tar` & `pami-2023.7.1.tar`

### file list

```diff
@@ -1,390 +1,396 @@
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.046296 pami-2023.5.1/
--rw-r--r--   0 likhitha   (505) staff       (20)    35149 2022-05-26 01:58:44.000000 pami-2023.5.1/LICENSE
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.920263 pami-2023.5.1/PAMI/
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.920842 pami-2023.5.1/PAMI/AssociationRules/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.931237 pami-2023.5.1/PAMI/AssociationRules/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)     8001 2023-05-29 07:58:16.000000 pami-2023.5.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     8038 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     8085 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    12384 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/AssociationRules/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6547 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/AssociationRules/basic/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      139 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.931460 pami-2023.5.1/PAMI/correlatedPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.934720 pami-2023.5.1/PAMI/correlatedPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    24412 2023-06-11 11:25:22.000000 pami-2023.5.1/PAMI/correlatedPattern/basic/CPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    25824 2023-06-10 21:46:38.000000 pami-2023.5.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/correlatedPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6055 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.935102 pami-2023.5.1/PAMI/coveragePatterns/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/coveragePatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.937867 pami-2023.5.1/PAMI/coveragePatterns/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    13995 2023-06-10 21:46:38.000000 pami-2023.5.1/PAMI/coveragePatterns/basic/CMine.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    16075 2023-06-10 21:46:38.000000 pami-2023.5.1/PAMI/coveragePatterns/basic/CPPG.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/coveragePatterns/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6938 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/coveragePatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.946364 pami-2023.5.1/PAMI/extras/
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.948771 pami-2023.5.1/PAMI/extras/DF2DB/
--rw-rw-r--   0 likhitha   (505) staff       (20)     2178 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/DF2DB.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     2243 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/DF2DB/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     1607 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/createTDB.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     9942 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/denseDF2DB.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4917 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3607 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3359 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.949258 pami-2023.5.1/PAMI/extras/calculateMISValues/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/calculateMISValues/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3741 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3794 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.951441 pami-2023.5.1/PAMI/extras/dbStats/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/dbStats/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    13043 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    14661 2023-05-30 02:46:24.000000 pami-2023.5.1/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     9364 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    13229 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    10040 2023-05-30 02:47:08.000000 pami-2023.5.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    11775 2023-05-30 02:42:12.000000 pami-2023.5.1/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.952885 pami-2023.5.1/PAMI/extras/fuzzyTransformation/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5195 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5925 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5919 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5803 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.953660 pami-2023.5.1/PAMI/extras/generateDatabase/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/generateDatabase/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     2877 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7092 2023-05-31 04:57:18.000000 pami-2023.5.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3444 2023-05-31 04:55:28.000000 pami-2023.5.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3593 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.956822 pami-2023.5.1/PAMI/extras/graph/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/graph/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     1656 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/graph/dataFrameInToFigures.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     2954 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     1167 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     1753 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     2203 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.956995 pami-2023.5.1/PAMI/extras/image2Database/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.957307 pami-2023.5.1/PAMI/extras/imageProcessing/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/imageProcessing/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4582 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.957618 pami-2023.5.1/PAMI/extras/neighbours/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/neighbours/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     2834 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3031 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/plotPointOnMap.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     3214 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/plotPointOnMap_dump.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     2178 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/scatterPlotSpatialPoints.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     1827 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/topKPatterns.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      473 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.958040 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.960676 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    14656 2023-06-10 21:46:38.000000 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    21185 2023-06-10 21:48:34.000000 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    14992 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6691 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.961090 pami-2023.5.1/PAMI/frequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.968579 pami-2023.5.1/PAMI/frequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    13124 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/basic/Apriori.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    12531 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    13188 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    13480 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    20324 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7733 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.969168 pami-2023.5.1/PAMI/frequentPattern/closed/
--rw-rw-r--   0 likhitha   (505) staff       (20)    19874 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/closed/CHARM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/closed/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6445 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.969968 pami-2023.5.1/PAMI/frequentPattern/cuda/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/cuda/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5744 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     8703 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5582 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.970668 pami-2023.5.1/PAMI/frequentPattern/maximal/
--rw-rw-r--   0 likhitha   (505) staff       (20)    25097 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/maximal/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6436 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.971678 pami-2023.5.1/PAMI/frequentPattern/pyspark/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5605 2023-05-30 02:18:50.000000 pami-2023.5.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    13209 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    11487 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    16147 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.972124 pami-2023.5.1/PAMI/frequentPattern/topk/
--rw-rw-r--   0 likhitha   (505) staff       (20)    14674 2023-06-10 22:08:34.000000 pami-2023.5.1/PAMI/frequentPattern/topk/FAE.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/topk/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4575 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.976188 pami-2023.5.1/PAMI/frequentSpatialPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.978033 pami-2023.5.1/PAMI/frequentSpatialPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    20041 2023-06-11 10:36:52.000000 pami-2023.5.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    19099 2023-06-11 10:36:52.000000 pami-2023.5.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentSpatialPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6680 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/frequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.978188 pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.979130 pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    25239 2023-06-11 10:36:52.000000 pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6635 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.979277 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.980247 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    20750 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    24624 2023-06-11 10:38:46.000000 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6450 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.980396 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.981732 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    23992 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    26791 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6580 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.982038 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.983003 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    23521 2023-06-10 01:56:22.000000 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    25345 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6668 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.983216 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.984629 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    26817 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    32216 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6618 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.985526 pami-2023.5.1/PAMI/geoReferencedFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)    28518 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/geoReferencedFrequentPattern/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5007 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/geoReferencedFrequentPattern/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.985724 pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.989745 pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    19950 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6774 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.989955 pami-2023.5.1/PAMI/highUtilityFrequentPatterns/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityFrequentPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.991582 pami-2023.5.1/PAMI/highUtilityFrequentPatterns/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    35401 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityFrequentPatterns/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6081 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.991746 pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.993436 pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    39910 2023-06-11 10:45:26.000000 pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6181 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.993734 pami-2023.5.1/PAMI/highUtilityPatterns/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.995366 pami-2023.5.1/PAMI/highUtilityPatterns/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    32747 2023-06-11 10:49:44.000000 pami-2023.5.1/PAMI/highUtilityPatterns/basic/EFIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    24847 2023-06-11 10:49:44.000000 pami-2023.5.1/PAMI/highUtilityPatterns/basic/HMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    26567 2023-06-11 10:51:32.000000 pami-2023.5.1/PAMI/highUtilityPatterns/basic/UPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityPatterns/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5053 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.995876 pami-2023.5.1/PAMI/highUtilitySpatialPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6718 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.996836 pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    27632 2023-06-11 10:51:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    34623 2023-06-11 10:53:12.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5955 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.997809 pami-2023.5.1/PAMI/highUtilitySpatialPattern/topk/
--rw-rw-r--   0 likhitha   (505) staff       (20)    35216 2023-06-11 10:53:12.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6625 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:47.997994 pami-2023.5.1/PAMI/localPeriodicPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.004956 pami-2023.5.1/PAMI/localPeriodicPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    32664 2023-06-11 10:55:48.000000 pami-2023.5.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    21999 2023-06-11 10:55:48.000000 pami-2023.5.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    21120 2023-06-11 10:55:48.000000 pami-2023.5.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     8378 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.005227 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.006542 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    23034 2023-06-11 10:58:52.000000 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    22318 2023-06-11 10:58:52.000000 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5913 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.006704 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.007734 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    27316 2023-06-11 10:58:52.000000 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    21102 2023-06-11 10:58:52.000000 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5392 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.007907 pami-2023.5.1/PAMI/partialPeriodicPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.009539 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    50844 2023-06-11 11:03:52.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4195 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    24330 2023-06-11 11:03:52.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    17878 2023-06-11 11:03:52.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5572 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.010128 pami-2023.5.1/PAMI/partialPeriodicPattern/closed/
--rw-rw-r--   0 likhitha   (505) staff       (20)    21069 2023-06-11 11:03:52.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5595 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.010937 pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/
--rw-rw-r--   0 likhitha   (505) staff       (20)    28482 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4261 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.011630 pami-2023.5.1/PAMI/partialPeriodicPattern/timeSeries/
--rw-rw-r--   0 likhitha   (505) staff       (20)    26058 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/timeSeries/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     5550 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.012207 pami-2023.5.1/PAMI/partialPeriodicPattern/topk/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7837 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    17705 2023-06-16 10:18:07.000000 pami-2023.5.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.012744 pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.013689 pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    19876 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6165 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.013975 pami-2023.5.1/PAMI/periodicCorrelatedPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.014887 pami-2023.5.1/PAMI/periodicCorrelatedPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    27518 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6652 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.015074 pami-2023.5.1/PAMI/periodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.017991 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    15591 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    25146 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    24942 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    16311 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    33244 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      726 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6525 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.018935 pami-2023.5.1/PAMI/periodicFrequentPattern/closed/
--rw-rw-r--   0 likhitha   (505) staff       (20)    21540 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6538 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.019460 pami-2023.5.1/PAMI/periodicFrequentPattern/cuda/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    17618 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.020534 pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/
--rw-rw-r--   0 likhitha   (505) staff       (20)    28740 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7873 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.020845 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.021826 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-rw-r--   0 likhitha   (505) staff       (20)    18066 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6898 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.022675 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4583 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    17235 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.023210 pami-2023.5.1/PAMI/recurringPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.024500 pami-2023.5.1/PAMI/recurringPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    26300 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/recurringPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6632 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.024709 pami-2023.5.1/PAMI/relativeFrequentPatterns/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/relativeFrequentPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.025570 pami-2023.5.1/PAMI/relativeFrequentPatterns/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    26260 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/relativeFrequentPatterns/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4261 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/relativeFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.025755 pami-2023.5.1/PAMI/relativeHighUtilityPatterns/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/relativeHighUtilityPatterns/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.027810 pami-2023.5.1/PAMI/relativeHighUtilityPatterns/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    33573 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/relativeHighUtilityPatterns/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7391 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.028159 pami-2023.5.1/PAMI/sequentialPatternMining/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.029217 pami-2023.5.1/PAMI/sequentialPatternMining/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    41062 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6554 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    22592 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.029850 pami-2023.5.1/PAMI/sequentialPatternMining/closed/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6279 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.029969 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.033474 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    16341 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    25169 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    17918 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7258 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.034218 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-rw-r--   0 likhitha   (505) staff       (20)    26386 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7177 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.034415 pami-2023.5.1/PAMI/uncertainFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.038724 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    25974 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    26009 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    18710 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    27060 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    27823 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    25507 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    19046 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4962 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.039005 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)      727 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.040408 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    31127 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)    31329 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6551 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.040587 pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.041630 pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    27481 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6693 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.041819 pami-2023.5.1/PAMI/weightedFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.042749 pami-2023.5.1/PAMI/weightedFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    23852 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     6737 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.042929 pami-2023.5.1/PAMI/weightedFrequentRegularPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.043376 pami-2023.5.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    27228 2023-06-11 11:25:06.000000 pami-2023.5.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     7555 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.043532 pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/
--rw-rw-r--   0 likhitha   (505) staff       (20)        1 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.044615 pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-rw-r--   0 likhitha   (505) staff       (20)    29070 2023-06-11 11:25:04.000000 pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-rw-r--   0 likhitha   (505) staff       (20)        0 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-rw-r--   0 likhitha   (505) staff       (20)     4782 2023-05-05 14:19:32.000000 pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 likhitha   (505) staff       (20)    34708 2023-06-20 07:29:48.045957 pami-2023.5.1/PKG-INFO
--rw-r--r--   0 likhitha   (505) staff       (20)    34124 2023-06-20 07:27:40.000000 pami-2023.5.1/README.md
-drwxr-xr-x   0 likhitha   (505) staff       (20)        0 2023-06-20 07:29:48.045538 pami-2023.5.1/pami.egg-info/
--rw-r--r--   0 likhitha   (505) staff       (20)    34708 2023-06-20 07:29:47.000000 pami-2023.5.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 likhitha   (505) staff       (20)    13278 2023-06-20 07:29:47.000000 pami-2023.5.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 likhitha   (505) staff       (20)        1 2023-06-20 07:29:47.000000 pami-2023.5.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 likhitha   (505) staff       (20)       75 2023-06-20 07:29:47.000000 pami-2023.5.1/pami.egg-info/requires.txt
--rw-r--r--   0 likhitha   (505) staff       (20)        5 2023-06-20 07:29:47.000000 pami-2023.5.1/pami.egg-info/top_level.txt
--rw-r--r--   0 likhitha   (505) staff       (20)       38 2023-06-20 07:29:48.046393 pami-2023.5.1/setup.cfg
--rw-r--r--   0 likhitha   (505) staff       (20)     1205 2023-06-20 07:28:11.000000 pami-2023.5.1/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.068497 pami-2023.7.1/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.1/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.991639 pami-2023.7.1/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.991938 pami-2023.7.1/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.993820 pami-2023.7.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.993985 pami-2023.7.1/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.995945 pami-2023.7.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24412 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.996140 pami-2023.7.1/PAMI/coveragePatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/coveragePatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.997686 pami-2023.7.1/PAMI/coveragePatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.998948 pami-2023.7.1/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.000584 pami-2023.7.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.001023 pami-2023.7.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.002310 pami-2023.7.1/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.004048 pami-2023.7.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.004853 pami-2023.7.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.006183 pami-2023.7.1/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.006385 pami-2023.7.1/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.006747 pami-2023.7.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.007040 pami-2023.7.1/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/scatterPlotSpatialPoints.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.007240 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.008384 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.008684 pami-2023.7.1/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.010529 pami-2023.7.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.011225 pami-2023.7.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.012556 pami-2023.7.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.013238 pami-2023.7.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.014293 pami-2023.7.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.015471 pami-2023.7.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.015605 pami-2023.7.1/PAMI/frequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.016591 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.016800 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.017635 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.017845 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.018942 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.019167 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.020130 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.020436 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.020865 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.021086 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.022205 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.022436 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.023591 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.024431 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.024667 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.025401 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.025636 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.026469 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.027147 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.027990 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.028221 pami-2023.7.1/PAMI/highUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.029468 pami-2023.7.1/PAMI/highUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.029912 pami-2023.7.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.031160 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.031948 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.032177 pami-2023.7.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.033366 pami-2023.7.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.033599 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.034638 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.034855 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.035794 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.036013 pami-2023.7.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.039089 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.039939 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.040890 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.041687 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.042431 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.042854 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.043456 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.043732 pami-2023.7.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.044298 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.044501 pami-2023.7.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.046568 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.047372 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.047787 pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.048739 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.048955 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.049755 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.050428 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.050746 pami-2023.7.1/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.051482 pami-2023.7.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.051699 pami-2023.7.1/PAMI/relativeFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.052434 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.052647 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.053284 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.053503 pami-2023.7.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.054576 pami-2023.7.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.055173 pami-2023.7.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.055260 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.056453 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.057421 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.057658 pami-2023.7.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.062262 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.062509 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.063689 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.063931 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.064605 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.064843 pami-2023.7.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.065590 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.065846 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.066475 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.066736 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.067463 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34817 2023-07-05 02:40:46.068347 pami-2023.7.1/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34213 2023-06-21 07:17:51.000000 pami-2023.7.1/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.068132 pami-2023.7.1/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34817 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13493 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       75 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-05 02:40:46.068543 pami-2023.7.1/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1205 2023-07-05 02:36:58.000000 pami-2023.7.1/setup.py
```

### Comparing `pami-2023.5.1/LICENSE` & `pami-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.7.1/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.7.1/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.7.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/correlatedPattern/__init__.py` & `pami-2023.7.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/correlatedPattern/basic/CPGrowth.py` & `pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py` & `pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.7.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/coveragePatterns/basic/CMine.py` & `pami-2023.7.1/PAMI/coveragePatterns/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/coveragePatterns/basic/CPPG.py` & `pami-2023.7.1/PAMI/coveragePatterns/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/coveragePatterns/basic/abstract.py` & `pami-2023.7.1/PAMI/coveragePatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.7.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.7.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.7.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.7.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.7.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.7.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.7.1/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.7.1/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.7.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.7.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.7.1/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.7.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.7.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.7.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.7.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.7.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.7.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.7.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.7.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.7.1/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.7.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.7.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.7.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.7.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.7.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.7.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/plotPointOnMap.py` & `pami-2023.7.1/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.7.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.7.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/extras/topKPatterns.py` & `pami-2023.7.1/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,14 @@
 """
 
 
 
 
 
 
-
-
-
-from PAMI.faultTolerantFrequentPattern.basic import abstract as _ab
 from PAMI.faultTolerantFrequentPattern.basic import abstract as _fp
 
 _minSup = str()
 _fp._sys.setrecursionlimit(20000)
 
 
 class _Node:
```

### Comparing `pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py` & `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/__init__.py` & `pami-2023.7.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.7.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.7.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.7.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.7.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.7.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.7.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.7.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 
 
 import os
 import csv
 import time
 import numpy as np
-# import pycuda.gpuarray as gpuarray
-# import pycuda.autoinit
-# import psutil
+import pycuda.gpuarray as gpuarray
+import pycuda.autoinit
+import psutil
 
 
 class cudaAprioriGCT:
     __time = 0
     __memRSS = 0
     __memUSS = 0
     __GPU_MEM = 0
```

### Comparing `pami-2023.5.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,45 +22,45 @@
 
 
 
 import os
 import csv
 import time
 import numpy as np
-# import pycuda.gpuarray as gpuarray
-# import pycuda.autoinit
-# import psutil
-# import pycuda.driver as cuda
-# from pycuda.compiler import SourceModule
-# import pycuda
-
-# deviceIntersection = SourceModule("""
-#     __global__ void intersection(int *compareThis, int *compareThat, int *resultStart,
-#                                  int *values, int *result, int resultX, int resultY){
-#         const int tidX = blockIdx.x * blockDim.x + threadIdx.x;
-#         const int tidY = blockIdx.y * blockDim.y + threadIdx.y;
-#         int resultIndex = resultStart[tidX] + tidY;
-#
-#         // ignore if tidX or tidY is out of bounds or if the value comparing with is 0
-#         if (tidX > resultX-1 || tidY > resultY-1 || values[compareThis[tidX] + tidY] == 0) return;
-#
-#         for (int i = 0; i < resultY; i++){
-#             if ( values[compareThat[tidX] + i] == 0) return;
-#             if ( values[compareThis[tidX] + tidY] == values[compareThat[tidX] + i]){
-#                 result[resultIndex] = values[compareThis[tidX] + tidY];
-#                 return;
-#             }
-#         }
-#
-#         //result[resultIndex] = values[compareThis[tidX] + tidY];
-#
-#     }
-#
-# """
-#                                   )
+import pycuda.gpuarray as gpuarray
+import pycuda.autoinit
+import psutil
+import pycuda.driver as cuda
+from pycuda.compiler import SourceModule
+import pycuda
+
+deviceIntersection = SourceModule("""
+    __global__ void intersection(int *compareThis, int *compareThat, int *resultStart,
+                                 int *values, int *result, int resultX, int resultY){
+        const int tidX = blockIdx.x * blockDim.x + threadIdx.x;
+        const int tidY = blockIdx.y * blockDim.y + threadIdx.y;
+        int resultIndex = resultStart[tidX] + tidY;
+
+        // ignore if tidX or tidY is out of bounds or if the value comparing with is 0
+        if (tidX > resultX-1 || tidY > resultY-1 || values[compareThis[tidX] + tidY] == 0) return;
+
+        for (int i = 0; i < resultY; i++){
+            if ( values[compareThat[tidX] + i] == 0) return;
+            if ( values[compareThis[tidX] + tidY] == values[compareThat[tidX] + i]){
+                result[resultIndex] = values[compareThis[tidX] + tidY];
+                return;
+            }
+        }
+
+        //result[resultIndex] = values[compareThis[tidX] + tidY];
+
+    }
+
+"""
+                                  )
 
 
 class cudaAprioriTID:
     __time = 0
     __memRSS = 0
     __memUSS = 0
     __GPU_MEM = 0
```

### Comparing `pami-2023.5.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.7.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import os
 import csv
 import time
 import numpy as np
-# import pycuda.gpuarray as gpuarray
-# import pycuda.autoinit
-# import psutil
+import pycuda.gpuarray as gpuarray
+import pycuda.autoinit
+import psutil
 
 
 class cudaEclatGCT:
     
     __time = 0
     __memRSS = 0
     __memUSS = 0
```

### Comparing `pami-2023.5.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.7.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.7.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.7.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.7.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
-# from pyspark import SparkConf as _SparkConf, SparkContext as _SparkContext
+from pyspark import SparkConf as _SparkConf, SparkContext as _SparkContext
 
 class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
             employ in PAMI
            Attributes:
            ----------
             iFile : str
```

### Comparing `pami-2023.5.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.7.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.7.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentSpatialPattern/__init__.py` & `pami-2023.7.1/PAMI/frequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py` & `pami-2023.7.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py` & `pami-2023.7.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/frequentSpatialPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/frequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentPatterns/__init__.py` & `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py` & `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,18 +207,18 @@
         WriteOut(prefix, prefixLen, item, sumIUtil)
             To Store the patten
 
     Executing the code on terminal :
     --------------------------------
         Format:
 
-            >>> python3 FFIMinerMiner.py <inputFile> <outputFile> <minSup> <separator>
+            >>> python3 FFIMiner.py <inputFile> <outputFile> <minSup> <separator>
         Examples:
 
-            >>> python3  FFIMinerMiner.py sampleTDB.txt output.txt 6  (minSup will be considered in support count or frequency)
+            >>> python3  FFIMiner.py sampleTDB.txt output.txt 6  (minSup will be considered in support count or frequency)
 
 
     Sample run of importing the code:
     ----------------------------------
     .. code-block:: python
 
         from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
```

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py` & `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py` & `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py` & `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py` & `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py` & `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py` & `pami-2023.7.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/geoReferencedFrequentPattern/abstract.py` & `pami-2023.7.1/PAMI/geoReferencedFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py` & `pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py` & `pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py` & `pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py` & `pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityPatterns/basic/EFIM.py` & `pami-2023.7.1/PAMI/highUtilityPatterns/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityPatterns/basic/HMiner.py` & `pami-2023.7.1/PAMI/highUtilityPatterns/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityPatterns/basic/UPGrowth.py` & `pami-2023.7.1/PAMI/highUtilityPatterns/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilityPatterns/basic/abstract.py` & `pami-2023.7.1/PAMI/highUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.7.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py` & `pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,92 +44,92 @@
 
 import os
 import sys
 import csv
 import time
 import psutil
 import numpy as np
-# import pycuda.autoinit
-# import pycuda.driver as cuda
-# from pycuda.compiler import SourceModule
-#
-# supportAndPeriod = SourceModule(r"""
-#
-# __global__ void supportAndPeriod(unsigned long long int *bitArray, // containing transactions
-#                                 unsigned long long int *support, // for support
-#                                 unsigned long long int *period, // for period
-#                                 unsigned long long int *thingsToCompare, // for things to compare
-#                                 unsigned long long int *thingsToCompareIndex, // for things to compare index
-#                                 unsigned long long int numberOfThingsToCompare, // for number of things to compare
-#                                 unsigned long long int numberOfBits, // for number of bits
-#                                 unsigned long long int numberOfElements, // for number of elements
-#                                 unsigned long long int maxPeriod, // for max period
-#                                 unsigned long long int maxTimeStamp){
-#
-#         unsigned long long int threadIDX = blockIdx.x * blockDim.x + threadIdx.x;
-#
-#         if (threadIDX > numberOfThingsToCompare-2) return;
-#
-#         unsigned long long int holder = 0;
-#         unsigned long long int supportCounter = 0;
-#         unsigned long long int periodCounter = 0;
-#         unsigned long long int numbersCounter = 0;
-#         short int bitRepresentation[64];
-#         short int index = numberOfBits - 1;
-#
-#         for(int i = 0; i < numberOfElements; i++){
-#             // intersection
-#             holder = bitArray[thingsToCompare[thingsToCompareIndex[threadIDX]] * numberOfElements + i];
-#             for (int j = thingsToCompareIndex[threadIDX]+1; j < thingsToCompareIndex[threadIDX + 1]; j++){
-#                 holder = holder & bitArray[thingsToCompare[j] * numberOfElements + i];
-#             }
-#
-#             // empty bitRepresentation
-#             for (int j = 0; j < 64; j++){
-#                 bitRepresentation[j] = 0;
-#             }
-#
-#             // conversion to bit representation
-#             index = numberOfBits - 1;
-#             while (holder > 0){
-#                 bitRepresentation[index] = holder % 2;
-#                 holder = holder / 2;
-#                 index--;
-#             }
-#
-#             // counting period
-#             for (int j = 0; j < numberOfBits; j++){
-#                 periodCounter++;
-#                 numbersCounter++;
-#                 if (periodCounter > maxPeriod){
-#                     period[threadIDX] = periodCounter;
-#                     support[threadIDX] = supportCounter;
-#                     return;
-#                 }
-#                 if (bitRepresentation[j] == 1){
-#                     supportCounter++;
-#                     if (periodCounter > period[threadIDX]) period[threadIDX] = periodCounter;
-#                     periodCounter = 0;
-#                 }
-#                 if (numbersCounter == maxTimeStamp){
-#                     support[threadIDX] = supportCounter;
-#                     period[threadIDX] = periodCounter;
-#                     return;
-#                 }
-#             }
-#
-#         }
-#         support[threadIDX] = supportCounter;
-#         period[threadIDX] = periodCounter;
-#         return;
-#
-#     }
-#
-# """
-#                                 )
+import pycuda.autoinit
+import pycuda.driver as cuda
+from pycuda.compiler import SourceModule
+
+supportAndPeriod = SourceModule(r"""
+
+__global__ void supportAndPeriod(unsigned long long int *bitArray, // containing transactions
+                                unsigned long long int *support, // for support
+                                unsigned long long int *period, // for period
+                                unsigned long long int *thingsToCompare, // for things to compare
+                                unsigned long long int *thingsToCompareIndex, // for things to compare index
+                                unsigned long long int numberOfThingsToCompare, // for number of things to compare
+                                unsigned long long int numberOfBits, // for number of bits
+                                unsigned long long int numberOfElements, // for number of elements
+                                unsigned long long int maxPeriod, // for max period
+                                unsigned long long int maxTimeStamp){
+
+        unsigned long long int threadIDX = blockIdx.x * blockDim.x + threadIdx.x;
+
+        if (threadIDX > numberOfThingsToCompare-2) return;
+
+        unsigned long long int holder = 0;
+        unsigned long long int supportCounter = 0;
+        unsigned long long int periodCounter = 0;
+        unsigned long long int numbersCounter = 0;
+        short int bitRepresentation[64];
+        short int index = numberOfBits - 1;
+
+        for(int i = 0; i < numberOfElements; i++){
+            // intersection
+            holder = bitArray[thingsToCompare[thingsToCompareIndex[threadIDX]] * numberOfElements + i];
+            for (int j = thingsToCompareIndex[threadIDX]+1; j < thingsToCompareIndex[threadIDX + 1]; j++){
+                holder = holder & bitArray[thingsToCompare[j] * numberOfElements + i];
+            }
+
+            // empty bitRepresentation
+            for (int j = 0; j < 64; j++){
+                bitRepresentation[j] = 0;
+            }
+
+            // conversion to bit representation
+            index = numberOfBits - 1;
+            while (holder > 0){
+                bitRepresentation[index] = holder % 2;
+                holder = holder / 2;
+                index--;
+            }
+
+            // counting period
+            for (int j = 0; j < numberOfBits; j++){
+                periodCounter++;
+                numbersCounter++;
+                if (periodCounter > maxPeriod){
+                    period[threadIDX] = periodCounter;
+                    support[threadIDX] = supportCounter;
+                    return;
+                }
+                if (bitRepresentation[j] == 1){
+                    supportCounter++;
+                    if (periodCounter > period[threadIDX]) period[threadIDX] = periodCounter;
+                    periodCounter = 0;
+                }
+                if (numbersCounter == maxTimeStamp){
+                    support[threadIDX] = supportCounter;
+                    period[threadIDX] = periodCounter;
+                    return;
+                }
+            }
+
+        }
+        support[threadIDX] = supportCounter;
+        period[threadIDX] = periodCounter;
+        return;
+
+    }
+
+"""
+                                )
 
 
 class gPFMinerBit:
 
     """
     Description:
     ------------
```

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.7.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py` & `pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/relativeFrequentPatterns/basic/abstract.py` & `pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py` & `pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py` & `pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.7.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.7.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.7.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.7.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.7.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.5.1/PKG-INFO` & `pami-2023.7.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,39 @@
-Metadata-Version: 2.1
-Name: pami
-Version: 2023.5.1
-Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayRage/PAMI
-Author: Rage Uday Kiran
-Author-email: uday.rage@gmail.com
-License: GPLv3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 ![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
 [![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
 
 
 # Introduction
-PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referencial/sequence databases across multiple computing platforms.
+PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udayrage.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udayrage.github.io/PAMI/codersManual/index.html
 
 3. Code documentation [PAMI documentation](https://raw.githack.com/udayRage/PAMI/main/htmlDocs/_build/html/index.html)
 
 3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
 
 5. Report issues https://github.com/udayRage/PAMI/issues
   
- __Recent versions__  
+ # Recent versions  
 
+- Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
 # Maintenance
 
   Installation
@@ -61,236 +46,259 @@
   
   Uninstallation
   
        pip uninstall pami 
        
 # Tutorials 
 
-- Click on __"Basic"__ link to view the basic tutorial on using the algorithm. 
-- Click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
-
+## 1. Mining Databases
+### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
-     
+
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-   | Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
-   | FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-   | ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
-   | ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-   | ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+| Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
+| FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
+| ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
+| ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+
+2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-2. Relative Frequent Patterns: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
-    
 | Basic |
 |-------|
 | RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
-    
+
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
-    
-    
-        
+
+
+
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
 | Basic                                                                                                                                                                                                            |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
 | CP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
-    
-5. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
+
+
+### Temporal databases
+
+
+1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
+
+
+2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
+
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
+
+3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
+
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
+| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
+
+4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+
+
+5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+
+6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
+
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+
+### Geo-referenced (or spatiotemporal) databases
+
+1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
-    
-    
-6. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                   |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
-    
-7. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
+2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                        |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
- 
-8. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
-| Basic                                                                                                                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
-    
-9. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                    |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
- | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
-    
-9. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html) 
+| Basic   |
+|---------|
+| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
-| Basic                                                                                                                                                                                                                                    |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
+
+| Basic    |
+|----------|
+| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
-10. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
+
+### Utility databases
+
+1. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
 
 | Basic    |
 |----------|
 | EFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
 | HMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
 | UPGrowth |
 
-11. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
+2. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
 
 | Basic |
 |-------|
 | HUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
-    
-12. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
+
+
+3. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  |
 |--------|
 | SHUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
- 
 
-     
-13. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
+4. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  | topk    |
 |--------|---------|
 | HDSHIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
 | SHUIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
 
-14. Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
-    
-15. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
+5. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
+
+| Basic |
+|-------|
+| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
+
+
+6. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
+
+| Basic |
+|-------|
+| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
+
+
+7. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
 
 | Basic     |
 |-----------|
- | GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
+| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
 
-16. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
+
+8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
 
 | Basic       |
 |-------------|
-| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
-| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
-| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
-    
-17. Partial periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
+| SSWFPGrowth |
 
-| Basic                                                                                                                                                                                                                                      |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
-     
-18. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
+### Fuzzy databases
+1. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
-| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+| Basic                                                                                                                                                                                                                   |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
 
-    
 
-19. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic   |
-|---------|
-| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
-20. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
-    
-| Basic                                                                                                                                                                                                                                 |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+2. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
-21. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
-    
-| Basic      | TopK |
-|------------|------|
-| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
-| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+| Basic                                                                                                                                                                                                                        |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
+
+
+3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
+
+4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                    |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
+
+5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                    |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+
+### Uncertain databases
+
+
+1. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
 
-    
-22. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
-    
 | Basic   | top-k |
 |---------|-------|
 | PUF [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
 | TubeP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
 | TubeS  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
 | UVEclat |       |
-    
-23. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
-     
+
+2. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
+
 | Basic       |
 |-------------|
 | UPFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
 | UPFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
-     
-24. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
-| Basic    |
-|----------|
-| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
-     
-25. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
-    
-| Basic |
-|-------|
-| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
 
-    
-26. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
-    
-| Basic |
-|-------|
-| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
-    
-27. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
-    
+3. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
+
 | Basic |
 |-------|
 | WUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
-    
-28. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
-    
-| Basic     |
-|-----------|
-| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
-    
-    
-29. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
-    
-| Basic       |
-|-------------|
-| SSWFPGrowth |
 
-30. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+### Sequence databases
+
+1. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
- 
- 
-     
- 
+
+### Timeseries databases
+
+
+## 2. Mining Streams
+   __coming soon__    
+
+## 3. Mining Graphs
+__coming soon__
```

### Comparing `pami-2023.5.1/README.md` & `pami-2023.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,56 @@
+Metadata-Version: 2.1
+Name: pami
+Version: 2023.7.1
+Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
+Home-page: https://github.com/udayRage/PAMI
+Author: Rage Uday Kiran
+Author-email: uday.rage@gmail.com
+License: GPLv3
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 ![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
 [![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
 
 
 # Introduction
-PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referencial/sequence databases across multiple computing platforms.
+PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udayrage.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udayrage.github.io/PAMI/codersManual/index.html
 
 3. Code documentation [PAMI documentation](https://raw.githack.com/udayRage/PAMI/main/htmlDocs/_build/html/index.html)
 
 3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
 
 5. Report issues https://github.com/udayRage/PAMI/issues
   
- __Recent versions__  
+ # Recent versions  
 
+- Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
 # Maintenance
 
   Installation
@@ -45,236 +63,261 @@
   
   Uninstallation
   
        pip uninstall pami 
        
 # Tutorials 
 
-- Click on __"Basic"__ link to view the basic tutorial on using the algorithm. 
-- Click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
-
+## 1. Mining Databases
+### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
-     
+
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-   | Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
-   | FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-   | ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
-   | ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-   | ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+| Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
+| FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
+| ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
+| ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+
+2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-2. Relative Frequent Patterns: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
-    
 | Basic |
 |-------|
 | RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
-    
+
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
-    
-    
-        
+
+
+
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
 | Basic                                                                                                                                                                                                            |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
 | CP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
-    
-5. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
+
+
+### Temporal databases
+
+
+1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
+
+
+2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
+
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
+
+3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
+
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
+| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
+
+4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+
+
+5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+
+6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
+
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+
+### Geo-referenced (or spatiotemporal) databases
+
+1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
-    
-    
-6. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                   |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
-    
-7. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
+2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                        |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
- 
-8. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
-| Basic                                                                                                                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
-    
-9. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                    |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
- | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
-    
-9. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html) 
+| Basic   |
+|---------|
+| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
-| Basic                                                                                                                                                                                                                                    |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
-10. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
+| Basic    |
+|----------|
+| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
+
+
+### Utility databases
+
+1. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
 
 | Basic    |
 |----------|
 | EFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
 | HMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
 | UPGrowth |
 
-11. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
+2. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
 
 | Basic |
 |-------|
 | HUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
-    
-12. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
+
+
+3. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  |
 |--------|
 | SHUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
- 
 
-     
-13. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
+4. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  | topk    |
 |--------|---------|
 | HDSHIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
 | SHUIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
 
-14. Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
-    
-15. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
+5. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
+
+| Basic |
+|-------|
+| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
+
+
+6. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
+
+| Basic |
+|-------|
+| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
+
+
+7. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
 
 | Basic     |
 |-----------|
- | GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
+| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
+
 
-16. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
+8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
 
 | Basic       |
 |-------------|
-| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
-| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
-| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
-    
-17. Partial periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
+| SSWFPGrowth |
 
-| Basic                                                                                                                                                                                                                                      |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
-     
-18. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
+### Fuzzy databases
+1. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
-| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+| Basic                                                                                                                                                                                                                   |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
 
-    
 
-19. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic   |
-|---------|
-| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
-20. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
-    
-| Basic                                                                                                                                                                                                                                 |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+2. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
-21. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
-    
-| Basic      | TopK |
-|------------|------|
-| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
-| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+| Basic                                                                                                                                                                                                                        |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
+
+
+3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
+
+4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                    |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
+
+5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                    |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+
+### Uncertain databases
+
+
+1. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
 
-    
-22. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
-    
 | Basic   | top-k |
 |---------|-------|
 | PUF [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
 | TubeP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
 | TubeS  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
 | UVEclat |       |
-    
-23. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
-     
+
+2. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
+
 | Basic       |
 |-------------|
 | UPFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
 | UPFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
-     
-24. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
-| Basic    |
-|----------|
-| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
-     
-25. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
-    
-| Basic |
-|-------|
-| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
 
-    
-26. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
-    
-| Basic |
-|-------|
-| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
-    
-27. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
-    
+3. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
+
 | Basic |
 |-------|
 | WUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
-    
-28. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
-    
-| Basic     |
-|-----------|
-| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
-    
-    
-29. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
-    
-| Basic       |
-|-------------|
-| SSWFPGrowth |
 
-30. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+### Sequence databases
+
+1. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
- 
- 
-     
- 
+
+### Timeseries databases
+
+
+## 2. Mining Streams
+   __coming soon__    
+
+## 3. Mining Graphs
+__coming soon__   
      
      
+
+
```

### Comparing `pami-2023.5.1/pami.egg-info/PKG-INFO` & `pami-2023.7.1/pami.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.5.1
+Version: 2023.7.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayRage/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,31 +25,32 @@
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
 
 
 # Introduction
-PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referencial/sequence databases across multiple computing platforms.
+PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udayrage.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udayrage.github.io/PAMI/codersManual/index.html
 
 3. Code documentation [PAMI documentation](https://raw.githack.com/udayRage/PAMI/main/htmlDocs/_build/html/index.html)
 
 3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
 
 5. Report issues https://github.com/udayRage/PAMI/issues
   
- __Recent versions__  
+ # Recent versions  
 
+- Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
 # Maintenance
 
   Installation
@@ -61,236 +63,261 @@
   
   Uninstallation
   
        pip uninstall pami 
        
 # Tutorials 
 
-- Click on __"Basic"__ link to view the basic tutorial on using the algorithm. 
-- Click on __"Adv"__ link to view the advanced tutorial on using a particular algorithm.
-
+## 1. Mining Databases
+### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
-     
+
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-   | Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
-   | FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-   | ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
-   | ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-   | ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+| Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
+| FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
+| ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
+| ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+
+2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-2. Relative Frequent Patterns: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
-    
 | Basic |
 |-------|
 | RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
-    
+
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
-    
-    
-        
+
+
+
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
 | Basic                                                                                                                                                                                                            |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
 | CP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
-    
-5. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
+
+
+### Temporal databases
+
+
+1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
+
+
+2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
+
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
+
+3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
+
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
+| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
+
+4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+
+
+5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+
+6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
+
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+
+### Geo-referenced (or spatiotemporal) databases
+
+1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
-    
-    
-6. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                   |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
-    
-7. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
+2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                        |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
- 
-8. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
-| Basic                                                                                                                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
-    
-9. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                    |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
- | FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
-    
-9. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html) 
+| Basic   |
+|---------|
+| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
-| Basic                                                                                                                                                                                                                                    |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
-10. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
+| Basic    |
+|----------|
+| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
+
+
+### Utility databases
+
+1. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
 
 | Basic    |
 |----------|
 | EFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
 | HMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
 | UPGrowth |
 
-11. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
+2. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
 
 | Basic |
 |-------|
 | HUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
-    
-12. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
+
+
+3. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  |
 |--------|
 | SHUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
- 
 
-     
-13. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
+4. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  | topk    |
 |--------|---------|
 | HDSHIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
 | SHUIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
 
-14. Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
-    
-15. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
+5. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
+
+| Basic |
+|-------|
+| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
+
+
+6. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
+
+| Basic |
+|-------|
+| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
+
+
+7. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
 
 | Basic     |
 |-----------|
- | GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
+| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
+
 
-16. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
+8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
 
 | Basic       |
 |-------------|
-| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
-| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
-| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
-    
-17. Partial periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
+| SSWFPGrowth |
 
-| Basic                                                                                                                                                                                                                                      |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
-     
-18. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
+### Fuzzy databases
+1. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
-| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+| Basic                                                                                                                                                                                                                   |
+|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
 
-    
 
-19. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
-| Basic   |
-|---------|
-| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
-20. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
-    
-| Basic                                                                                                                                                                                                                                 |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+2. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
-21. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
-    
-| Basic      | TopK |
-|------------|------|
-| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
-| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+| Basic                                                                                                                                                                                                                        |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
+
+
+3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                  |
+|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
+
+4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                    |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
+
+5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
+
+| Basic                                                                                                                                                                                                                                    |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+
+### Uncertain databases
+
+
+1. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
 
-    
-22. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
-    
 | Basic   | top-k |
 |---------|-------|
 | PUF [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
 | TubeP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
 | TubeS  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
 | UVEclat |       |
-    
-23. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
-     
+
+2. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
+
 | Basic       |
 |-------------|
 | UPFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
 | UPFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
-     
-24. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
-| Basic    |
-|----------|
-| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
-     
-25. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
-    
-| Basic |
-|-------|
-| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
 
-    
-26. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
-    
-| Basic |
-|-------|
-| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
-    
-27. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
-    
+3. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
+
 | Basic |
 |-------|
 | WUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
-    
-28. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
-    
-| Basic     |
-|-----------|
-| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
-    
-    
-29. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
-    
-| Basic       |
-|-------------|
-| SSWFPGrowth |
 
-30. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+### Sequence databases
+
+1. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
- 
- 
-     
- 
+
+### Timeseries databases
+
+
+## 2. Mining Streams
+   __coming soon__    
+
+## 3. Mining Graphs
+__coming soon__   
      
      
+
+
```

### Comparing `pami-2023.5.1/pami.egg-info/SOURCES.txt` & `pami-2023.7.1/pami.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 PAMI/extras/uncertaindb_convert.py
 PAMI/extras/DF2DB/DF2DB.py
 PAMI/extras/DF2DB/DF2DBPlus.py
 PAMI/extras/DF2DB/__init__.py
 PAMI/extras/DF2DB/createTDB.py
 PAMI/extras/DF2DB/denseDF2DB.py
 PAMI/extras/DF2DB/denseDF2DBPlus.py
+PAMI/extras/DF2DB/denseDF2DB_dump.py
 PAMI/extras/DF2DB/sparseDF2DB.py
 PAMI/extras/DF2DB/sparseDF2DBPlus.py
 PAMI/extras/calculateMISValues/__init__.py
 PAMI/extras/calculateMISValues/usingBeta.py
 PAMI/extras/calculateMISValues/usingSD.py
 PAMI/extras/dbStats/__init__.py
 PAMI/extras/dbStats/fuzzyDatabaseStats.py
@@ -111,14 +112,17 @@
 PAMI/fuzzyFrequentPatterns/basic/__init__.py
 PAMI/fuzzyFrequentPatterns/basic/abstract.py
 PAMI/fuzzyFrequentSpatialPattern/__init__.py
 PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
 PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
 PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
 PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
 PAMI/fuzzyPeriodicFrequentPattern/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
```

### Comparing `pami-2023.5.1/setup.py` & `pami-2023.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'pami',
-    version = '2023.05.01',
+    version = '2023.07.01',
     author = 'Rage Uday Kiran',
     author_email = 'uday.rage@gmail.com',
     description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages=setuptools.find_packages(),
     url = 'https://github.com/udayRage/PAMI',
```

