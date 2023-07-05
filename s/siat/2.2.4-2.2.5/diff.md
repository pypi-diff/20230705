# Comparing `tmp/siat-2.2.4-py3-none-any.whl.zip` & `tmp/siat-2.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1696568 bytes, number of entries: 120
+Zip file size: 1696578 bytes, number of entries: 120
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Apr-10 11:29 siat/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-Apr-10 11:29 siat/allin.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-10 11:29 siat/alpha_vantage_test.py
 -rw-rw-rw-  2.0 fat    28555 b- defN 23-Apr-10 11:29 siat/assets_liquidity.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-10 11:29 siat/assets_liquidity_test.py
 -rw-rw-rw-  2.0 fat    10110 b- defN 23-Apr-10 11:29 siat/barrons_scraping_test.py
 -rw-rw-rw-  2.0 fat    36597 b- defN 23-Apr-10 11:29 siat/beta_adjustment.py
@@ -81,15 +81,15 @@
 -rw-rw-rw-  2.0 fat    75061 b- defN 23-Apr-10 11:29 siat/risk_evaluation.py
 -rw-rw-rw-  2.0 fat     3731 b- defN 23-Apr-10 11:29 siat/risk_evaluation_test.py
 -rw-rw-rw-  2.0 fat    12304 b- defN 23-Apr-10 11:29 siat/risk_free_rate.py
 -rw-rw-rw-  2.0 fat     4285 b- defN 23-Apr-10 11:29 siat/risk_free_rate_test.py
 -rw-rw-rw-  2.0 fat   101523 b- defN 23-May-27 06:22 siat/sector_china.py
 -rw-rw-rw-  2.0 fat     5843 b- defN 23-Apr-11 14:17 siat/sector_china_test.py
 -rw-rw-rw-  2.0 fat    29185 b- defN 23-May-25 02:36 siat/security_price.py
--rw-rw-rw-  2.0 fat    74003 b- defN 23-Jul-05 02:11 siat/security_prices.py
+-rw-rw-rw-  2.0 fat    74058 b- defN 23-Jul-05 13:33 siat/security_prices.py
 -rw-rw-rw-  2.0 fat    10779 b- defN 23-Apr-10 11:29 siat/security_prices_test.py
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-Apr-10 11:29 siat/setup.py
 -rw-rw-rw-  2.0 fat     1418 b- defN 23-Apr-10 11:29 siat/shenwan index history test.py
 -rw-rw-rw-  2.0 fat   129369 b- defN 23-Jul-04 09:02 siat/stock.py
 -rw-rw-rw-  2.0 fat    31655 b- defN 23-Apr-10 11:29 siat/stock_advice_linear.py
 -rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-10 11:29 siat/stock_base.py
 -rw-rw-rw-  2.0 fat    82785 b- defN 23-Jun-17 02:52 siat/stock_china.py
@@ -111,12 +111,12 @@
 -rw-rw-rw-  2.0 fat   118133 b- defN 23-Apr-10 11:29 siat/translate-20230206.py
 -rw-rw-rw-  2.0 fat   121657 b- defN 23-Apr-10 11:29 siat/translate-20230215.py
 -rw-rw-rw-  2.0 fat   134050 b- defN 23-Jul-04 11:47 siat/translate.py
 -rw-rw-rw-  2.0 fat     3936 b- defN 23-Apr-10 11:29 siat/universal_test.py
 -rw-rw-rw-  2.0 fat    51342 b- defN 23-May-11 00:30 siat/valuation_china.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/valuation_market_china_test.py
 -rw-rw-rw-  2.0 fat    14859 b- defN 23-Apr-10 11:29 siat/var_model_validation.py
--rw-rw-rw-  2.0 fat     1410 b- defN 23-Jul-05 04:02 siat-2.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 04:02 siat-2.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-05 04:02 siat-2.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9602 b- defN 23-Jul-05 04:02 siat-2.2.4.dist-info/RECORD
-120 files, 7751475 bytes uncompressed, 1681928 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     1410 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     9602 b- defN 23-Jul-05 13:43 siat-2.2.5.dist-info/RECORD
+120 files, 7751530 bytes uncompressed, 1681938 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -342,20 +342,20 @@
 
 Filename: siat/valuation_market_china_test.py
 Comment: 
 
 Filename: siat/var_model_validation.py
 Comment: 
 
-Filename: siat-2.2.4.dist-info/METADATA
+Filename: siat-2.2.5.dist-info/METADATA
 Comment: 
 
-Filename: siat-2.2.4.dist-info/WHEEL
+Filename: siat-2.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: siat-2.2.4.dist-info/top_level.txt
+Filename: siat-2.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: siat-2.2.4.dist-info/RECORD
+Filename: siat-2.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siat/security_prices.py

```diff
@@ -233,14 +233,17 @@
     
     pricedf2=remove_timezone(pricedf)
 
 def remove_timezone(pricedf):
     """
     功能：去掉df索引中可能存在的时区信息，避免时区错误
     """
+    if pricedf is None:
+        return pricedf
+    
     pricedf['date_tz']=pricedf.index
     pricedf['date_y4m2d2']=pricedf['date_tz'].astype(str)
     
     import pandas as pd
     pricedf['date']=pricedf['date_y4m2d2'].apply(lambda x: pd.to_datetime(x))
     pricedf['date']=pricedf['date'].apply(lambda x: x.replace(tzinfo=None))   #去掉时区
```

## Comparing `siat-2.2.4.dist-info/METADATA` & `siat-2.2.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siat
-Version: 2.2.4
+Version: 2.2.5
 Summary: Securities Investment Analysis Tools (siat)
 Home-page: https://pypi.org/project/siat/
 Author: Prof. WANG Dehong, Business School, BFSU (北京外国语大学 国际商学院 王德宏 教授)
 Author-email: wdehong2000@163.com
 License: Copyright (C) WANG Dehong, 2023. For educational purpose only!
 Platform: UNKNOWN
 Requires-Dist: pandas-datareader
```

## Comparing `siat-2.2.4.dist-info/RECORD` & `siat-2.2.5.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 siat/risk_evaluation.py,sha256=lCDqCaSEppH0MFPFg-P14IYcF3IJqILbPfDmzf_AfcY,75061
 siat/risk_evaluation_test.py,sha256=YEXM96gKzTfwN4U61AS4Rr1tV7KgUvn4rRC6f3iMw9s,3731
 siat/risk_free_rate.py,sha256=r62zCl1qbI4lJU17GsgM-OmVx9oo3dltXeZVCNd6Uxg,12304
 siat/risk_free_rate_test.py,sha256=CpmhUf8aEAEZeNu4gvWP2Mz2dLoIgBX5bI41vfUBEr8,4285
 siat/sector_china.py,sha256=sHd7nlYWCK0SWAZbu-BLn-3vNPe2E8OFaDFYF67Hoho,101523
 siat/sector_china_test.py,sha256=1wq7ef8Bb_L8F0h0W6FvyBrIcBTEbrTV7hljtpj49U4,5843
 siat/security_price.py,sha256=2oHskgiw41KMGfqtnA0i2YjNNV6cYgtlUK0j3YeuXWs,29185
-siat/security_prices.py,sha256=XcwWos9UpIiCJRU9VJ1wqiPiriVKqt0IPPjsrk8qj3U,74003
+siat/security_prices.py,sha256=1J4SA5tZB4iFrQ91ijUA7jn0kkbAF8Jgc0J__IHq_ow,74058
 siat/security_prices_test.py,sha256=OEphoJ87NPKoNow1QA8EU_5MUYrJF-qKoWKNapVfZNI,10779
 siat/setup.py,sha256=up65rQGLmTBkhtaMLowjoQXYmIsnycnm4g1SYmeQS6o,1335
 siat/shenwan index history test.py,sha256=JCVAzOSEldHalhSFa3pqD8JI_8_djPMQOxpkuYU-Esg,1418
 siat/stock.py,sha256=WaRjLIXpjPl3VoUQ0AWvdtCCHKVP8RNm0ZPtUqOWaYo,129369
 siat/stock_advice_linear.py,sha256=-twT7IGP-NEplkL1WPSACcNJjggRB2j4mlAQCkzOAuo,31655
 siat/stock_base.py,sha256=uISvbRyOGy8p9QREA96CVydgflBkn5L3OXOGKl8oanc,1312
 siat/stock_china.py,sha256=jVSuCWr6TaTx0Y0sgqN-dU9ZL72uKiI_MzvugvH9NaI,82785
@@ -110,11 +110,11 @@
 siat/translate-20230206.py,sha256=-vtI125WyaJhmPotOpDAmclt_XnYVaWU9ByLWZ6FyYE,118133
 siat/translate-20230215.py,sha256=TJgtPE3n8IjljmZ4Pefy8dmHoNdFF-1zpML6BhA9FKE,121657
 siat/translate.py,sha256=pFi_U1_LLzcq6rE9ns0Hr0fLYjzB_n2sGLapdbLlVxw,134050
 siat/universal_test.py,sha256=CDAOffW1Rvs-TcNN5giWVvHMlch1w4dp-w5SIV9jXL0,3936
 siat/valuation_china.py,sha256=gYYXeT9bBPyQ251TCsYlibWcu6JA8x-YOKqLUEeLE7U,51342
 siat/valuation_market_china_test.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/var_model_validation.py,sha256=zB_Skk_tmzIR15l6oAW3am4HBGVIG-eZ8gJhCdXZ8Qw,14859
-siat-2.2.4.dist-info/METADATA,sha256=ijw-WUAKENo0hsIhDB3NqBB030GkxgoXP2OBxda2oVU,1410
-siat-2.2.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-siat-2.2.4.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
-siat-2.2.4.dist-info/RECORD,,
+siat-2.2.5.dist-info/METADATA,sha256=qwkcyHwE6Y30y-PJGL0IyaXLyQ_lNcAI-HRncXH6MNw,1410
+siat-2.2.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+siat-2.2.5.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
+siat-2.2.5.dist-info/RECORD,,
```

