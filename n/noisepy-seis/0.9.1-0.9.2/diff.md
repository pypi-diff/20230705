# Comparing `tmp/noisepy_seis-0.9.1.tar.gz` & `tmp/noisepy_seis-0.9.2.tar.gz`

## Comparing `noisepy_seis-0.9.1.tar` & `noisepy_seis-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112993 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/LICENSE
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/README.md
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 noisepy_seis-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11883 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35007 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/LICENSE
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/README.md
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 noisepy_seis-0.9.2/PKG-INFO
```

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.2/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,17 @@
 # get rough estimate of memory needs to ensure it now below up in S1
 MAX_MEM = 5.0  # maximum memory allowed per core in GB
 
 ##################################################
 # we expect no parameters need to be changed below
 
 
-def download(
-    direc: str,
-    prepro_para: ConfigParameters,
-    client_url_key: str = "SCEDC",
-):
+def download(direc: str, prepro_para: ConfigParameters):
     # client/data center. see https://docs.obspy.org/packages/obspy.clients.fdsn.html for a list
-    client = Client(client_url_key)
+    client = Client(prepro_para.client_url_key)
     chan_list = prepro_para.channels
     sta_list = prepro_para.stations
     executor = ThreadPoolExecutor()
 
     tlog = TimeLogger(logger, logging.INFO)
     t_tot = tlog.reset()
     dlist = os.path.join(direc, "station.csv")  # CSV file for station location info
@@ -238,15 +234,14 @@
                 # continue when there are alreay data for sta A at day X
                 if num_records[ista] == ncomp:
                     logger.info(f"Already have {num_records[ista]} for {sta[ista]}")
                     continue
                 task = executor.submit(
                     download_stream,
                     prepro_para,
-                    client_url_key,
                     inv,
                     net[ista],
                     sta[ista],
                     chan[ista],
                     location[ista],
                     starttime,
                     endtime,
@@ -269,26 +264,25 @@
                     ds.add_waveforms(tr, tag=new_tags)
 
     tlog.log("Total Download", t_tot)
 
 
 def download_stream(
     prepro_para: ConfigParameters,
-    url_key: str,
     inv: obspy.Inventory,
     net: str,
     sta: str,
     chan: str,
     location: str,
     starttime: obspy.UTCDateTime,
     endtime: obspy.UTCDateTime,
     index: int,
 ) -> Tuple[int, obspy.Stream]:
     logger.debug(f"Start download for {sta}.{chan}")
-    client = Client(url_key, timeout=15)
+    client = Client(prepro_para.client_url_key, timeout=15)
     retries = 5
     while retries > 0:
         try:
             tr = client.get_waveforms(
                 network=net,
                 station=sta,
                 channel=chan,
```

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.2/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.2/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,17 +232,24 @@
     parameters = noise_module.cc_parameters(fft_params, coor, tcorr, ncorr, comp)
     return (src_chan, rec_chan, parameters, corr)
 
 
 def preprocess(
     raw_store: RawDataStore, ch: Channel, ch_data: ChannelData, fft_params: ConfigParameters, ts: DateTimeRange
 ) -> obspy.Stream:
+    inv = raw_store.get_inventory(ts, ch.station)
+    ch_inv = inv.select(channel=ch.type.name, time=ts.start_datetime)
+    # if we don't find an inventory when filtering by time, back off and try
+    # without this constraint
+    if len(ch_inv) < 1:
+        ch_inv = inv.select(channel=ch.type.name)
+
     return noise_module.preprocess_raw(
         ch_data.stream.copy(),  # If we don't copy it's not writeable
-        raw_store.get_inventory(ts, ch.station),
+        ch_inv,
         fft_params,
         obspy.UTCDateTime(ts.start_datetime),
         obspy.UTCDateTime(ts.end_datetime),
     )
 
 
 def compute_fft(fft_params: ConfigParameters, ch_data: ChannelData) -> NoiseFFT:
```

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.2/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.2/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.2/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.2/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.2/src/noisepy/seis/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     AUTO_COVARIANCE = "auto_covariance"
     NROOT = "nroot"
     SELECTIVE = "selective"
     ALL = "all"
 
 
 class ConfigParameters(YamlModel):
+    client_url_key: str = "SCEDC"
     start_date: datetime = Field(default=datetime(2019, 1, 1))
     end_date: datetime = Field(default=datetime(2019, 1, 2))
     samp_freq: float = Field(default=20)  # TODO: change this samp_freq for the obspy "sampling_rate"
     cc_len: float = Field(default=1800.0, description="basic unit of data length for fft (sec)")
     # download params.
     # Targeted region/station information: only needed when down_list is False
     lamin: float = Field(default=31, description="Download: minimum latitude")
```

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/main.py` & `noisepy_seis-0.9.2/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.2/src/noisepy/seis/noise_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,6454 +610,6454 @@
 00002610: 706f 6e73 652e 5265 7370 6f6e 7365 2829  ponse.Response()
 00002620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00002630: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
 00002640: 6f72 2822 5468 6520 7265 7370 6f6e 7365  or("The response
 00002650: 2066 6f75 6e64 2069 6e20 7468 6520 696e   found in the in
 00002660: 7665 6e74 6f72 7920 6973 2065 6d70 7479  ventory is empty
 00002670: 2028 6e6f 2073 7461 6765 7329 2120 6162   (no stages)! ab
-00002680: 6f72 7421 2229 0a20 2020 2020 2020 2020  ort!").         
-00002690: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000026a0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 6c6f 6767 6572 2e69 6e66 6f28 2272    logger.info("r
-000026d0: 656d 6f76 696e 6720 7265 7370 6f6e 7365  emoving response
-000026e0: 2066 6f72 2025 7320 7573 696e 6720 696e   for %s using in
-000026f0: 7622 2025 2073 745b 305d 290a 2020 2020  v" % st[0]).    
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 7374 5b30 5d2e 6174 7461 6368 5f72 6573  st[0].attach_res
-00002720: 706f 6e73 6528 696e 7629 0a20 2020 2020  ponse(inv).     
-00002730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002740: 745b 305d 2e72 656d 6f76 655f 7265 7370  t[0].remove_resp
-00002750: 6f6e 7365 286f 7574 7075 743d 726d 5f72  onse(output=rm_r
-00002760: 6573 705f 6f75 742c 2070 7265 5f66 696c  esp_out, pre_fil
-00002770: 743d 7072 655f 6669 6c74 2c20 7761 7465  t=pre_filt, wate
-00002780: 725f 6c65 7665 6c3d 3630 290a 2020 2020  r_level=60).    
-00002790: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000027a0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-000027b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000027c0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-000027d0: 726e 696e 6728 2246 6169 6c65 6420 746f  rning("Failed to
-000027e0: 2072 656d 6f76 6520 7265 7370 6f6e 7365   remove response
-000027f0: 2066 726f 6d20 2573 2e20 5265 7475 726e   from %s. Return
-00002800: 696e 6720 656d 7074 7920 7374 7265 616d  ing empty stream
-00002810: 2e20 2573 2220 2520 2873 745b 305d 2c20  . %s" % (st[0], 
-00002820: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00002830: 2020 2020 2020 2020 7374 203d 205b 5d0a          st = [].
-00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002850: 2020 2020 7265 7475 726e 2073 740a 0a20      return st.. 
-00002860: 2020 2020 2020 2065 6c69 6620 726d 5f72         elif rm_r
-00002870: 6573 7020 3d3d 2022 7370 6563 7472 756d  esp == "spectrum
-00002880: 223a 0a20 2020 2020 2020 2020 2020 206c  ":.            l
-00002890: 6f67 6765 722e 696e 666f 2822 7265 6d6f  ogger.info("remo
-000028a0: 7665 2072 6573 706f 6e73 6520 7573 696e  ve response usin
-000028b0: 6720 7370 6563 7472 756d 2229 0a20 2020  g spectrum").   
-000028c0: 2020 2020 2020 2020 2073 7065 6366 696c           specfil
-000028d0: 6520 3d20 676c 6f62 2e67 6c6f 6228 6f73  e = glob.glob(os
-000028e0: 2e70 6174 682e 6a6f 696e 2872 6573 7064  .path.join(respd
-000028f0: 6972 2c20 222a 2220 2b20 7374 6174 696f  ir, "*" + statio
-00002900: 6e20 2b20 222a 2229 290a 2020 2020 2020  n + "*")).      
-00002910: 2020 2020 2020 6966 206c 656e 2873 7065        if len(spe
-00002920: 6366 696c 6529 203d 3d20 303a 0a20 2020  cfile) == 0:.   
-00002930: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00002940: 7365 2056 616c 7565 4572 726f 7228 226e  se ValueError("n
-00002950: 6f20 7265 7370 6f6e 7365 2073 6570 6374  o response sepct
-00002960: 7275 6d20 666f 756e 6420 666f 7220 2573  rum found for %s
-00002970: 2220 2520 7374 6174 696f 6e29 0a20 2020  " % station).   
-00002980: 2020 2020 2020 2020 2073 7420 3d20 7265           st = re
-00002990: 7370 5f73 7065 6374 7275 6d28 7374 2c20  sp_spectrum(st, 
-000029a0: 7370 6563 6669 6c65 5b30 5d2c 2073 616d  specfile[0], sam
-000029b0: 705f 6672 6571 2c20 7072 655f 6669 6c74  p_freq, pre_filt
-000029c0: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-000029d0: 726d 5f72 6573 7020 3d3d 2022 5245 5350  rm_resp == "RESP
-000029e0: 223a 0a20 2020 2020 2020 2020 2020 206c  ":.            l
-000029f0: 6f67 6765 722e 696e 666f 2822 7265 6d6f  ogger.info("remo
-00002a00: 7665 2072 6573 706f 6e73 6520 7573 696e  ve response usin
-00002a10: 6720 5245 5350 2066 696c 6573 2229 0a20  g RESP files"). 
-00002a20: 2020 2020 2020 2020 2020 2072 6573 7020             resp 
-00002a30: 3d20 676c 6f62 2e67 6c6f 6228 6f73 2e70  = glob.glob(os.p
-00002a40: 6174 682e 6a6f 696e 2872 6573 7064 6972  ath.join(respdir
-00002a50: 2c20 2252 4553 502e 2220 2b20 7374 6174  , "RESP." + stat
-00002a60: 696f 6e20 2b20 222a 2229 290a 2020 2020  ion + "*")).    
-00002a70: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00002a80: 6573 7029 203d 3d20 303a 0a20 2020 2020  esp) == 0:.     
-00002a90: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00002aa0: 2056 616c 7565 4572 726f 7228 226e 6f20   ValueError("no 
-00002ab0: 5245 5350 2066 696c 6573 2066 6f75 6e64  RESP files found
-00002ac0: 2066 6f72 2025 7322 2025 2073 7461 7469   for %s" % stati
-00002ad0: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-00002ae0: 7365 6564 7265 7370 203d 207b 0a20 2020  seedresp = {.   
-00002af0: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
-00002b00: 6c65 6e61 6d65 223a 2072 6573 705b 305d  lename": resp[0]
-00002b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002b20: 2020 2264 6174 6522 3a20 7374 6172 7474    "date": startt
-00002b30: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
-00002b40: 2020 2020 2022 756e 6974 7322 3a20 2244       "units": "D
-00002b50: 4953 222c 0a20 2020 2020 2020 2020 2020  IS",.           
-00002b60: 207d 0a20 2020 2020 2020 2020 2020 2073   }.            s
-00002b70: 742e 7369 6d75 6c61 7465 2870 617a 5f72  t.simulate(paz_r
-00002b80: 656d 6f76 653d 4e6f 6e65 2c20 7072 655f  emove=None, pre_
-00002b90: 6669 6c74 3d70 7265 5f66 696c 742c 2073  filt=pre_filt, s
-00002ba0: 6565 6472 6573 703d 7365 6564 7265 7370  eedresp=seedresp
-00002bb0: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00002bc0: 726d 5f72 6573 7020 3d3d 2022 706f 6c65  rm_resp == "pole
-00002bd0: 737a 6572 6f73 223a 0a20 2020 2020 2020  szeros":.       
-00002be0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00002bf0: 2822 7265 6d6f 7665 2072 6573 706f 6e73  ("remove respons
-00002c00: 6520 7573 696e 6720 706f 6c65 7320 616e  e using poles an
-00002c10: 6420 7a65 726f 7322 290a 2020 2020 2020  d zeros").      
-00002c20: 2020 2020 2020 7061 7a5f 7374 7320 3d20        paz_sts = 
-00002c30: 676c 6f62 2e67 6c6f 6228 6f73 2e70 6174  glob.glob(os.pat
-00002c40: 682e 6a6f 696e 2872 6573 7064 6972 2c20  h.join(respdir, 
-00002c50: 222a 2220 2b20 7374 6174 696f 6e20 2b20  "*" + station + 
-00002c60: 222a 2229 290a 2020 2020 2020 2020 2020  "*")).          
-00002c70: 2020 6966 206c 656e 2870 617a 5f73 7473    if len(paz_sts
-00002c80: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00002c90: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00002ca0: 6c75 6545 7272 6f72 2822 6e6f 2070 6f6c  lueError("no pol
-00002cb0: 6573 7a65 726f 7320 666f 756e 6420 666f  eszeros found fo
-00002cc0: 7220 2573 2220 2520 7374 6174 696f 6e29  r %s" % station)
-00002cd0: 0a20 2020 2020 2020 2020 2020 2073 742e  .            st.
-00002ce0: 7369 6d75 6c61 7465 2870 617a 5f72 656d  simulate(paz_rem
-00002cf0: 6f76 653d 7061 7a5f 7374 735b 305d 2c20  ove=paz_sts[0], 
-00002d00: 7072 655f 6669 6c74 3d70 7265 5f66 696c  pre_filt=pre_fil
-00002d10: 7429 0a0a 2020 2020 2020 2020 656c 7365  t)..        else
-00002d20: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00002d30: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00002d40: 6e6f 2073 7563 6820 6f70 7469 6f6e 2066  no such option f
-00002d50: 6f72 2072 6d5f 7265 7370 2120 706c 6561  or rm_resp! plea
-00002d60: 7365 2064 6f75 626c 6520 6368 6563 6b21  se double check!
-00002d70: 2229 0a0a 2020 2020 6e74 7220 3d20 6f62  ")..    ntr = ob
-00002d80: 7370 792e 5374 7265 616d 2829 0a20 2020  spy.Stream().   
-00002d90: 2023 2074 7269 6d20 6120 636f 6e74 696e   # trim a contin
-00002da0: 6f75 7320 7365 676d 656e 7420 696e 746f  ous segment into
-00002db0: 2075 7365 722d 6465 6669 6e65 6420 7365   user-defined se
-00002dc0: 7175 656e 6365 730a 2020 2020 7374 5b30  quences.    st[0
-00002dd0: 5d2e 7472 696d 280a 2020 2020 2020 2020  ].trim(.        
-00002de0: 7374 6172 7474 696d 653d 7374 6172 7474  starttime=startt
-00002df0: 696d 652c 0a20 2020 2020 2020 2065 6e64  ime,.        end
-00002e00: 7469 6d65 3d65 6e64 7469 6d65 2c0a 2020  time=endtime,.  
-00002e10: 2020 2020 2020 7061 643d 5472 7565 2c0a        pad=True,.
-00002e20: 2020 2020 2020 2020 6669 6c6c 5f76 616c          fill_val
-00002e30: 7565 3d30 2c0a 2020 2020 290a 2020 2020  ue=0,.    ).    
-00002e40: 6e74 722e 6170 7065 6e64 2873 745b 305d  ntr.append(st[0]
-00002e50: 290a 0a20 2020 2072 6574 7572 6e20 6e74  )..    return nt
-00002e60: 720a 0a0a 6465 6620 7374 6174 7332 696e  r...def stats2in
-00002e70: 7628 7374 6174 732c 2070 7265 7072 6f5f  v(stats, prepro_
-00002e80: 7061 7261 2c20 6c6f 6373 3d4e 6f6e 6529  para, locs=None)
-00002e90: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-00002ea0: 6973 2066 756e 6374 696f 6e20 6372 6561  is function crea
-00002eb0: 7465 7320 696e 7665 6e74 6f72 7920 6769  tes inventory gi
-00002ec0: 7665 6e20 7468 6520 7374 6174 7320 7061  ven the stats pa
-00002ed0: 7261 6d65 7465 7273 2069 6e20 616e 206f  rameters in an o
-00002ee0: 6273 7079 2073 7472 6561 6d20 6f72 2061  bspy stream or a
-00002ef0: 2073 7461 7469 6f6e 206c 6973 742e 0a20   station list.. 
-00002f00: 2020 2028 7573 6564 2069 6e20 5330 4229     (used in S0B)
-00002f10: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-00002f20: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-00002f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00002f40: 2020 7374 6174 733a 206f 6273 7079 2074    stats: obspy t
-00002f50: 7261 6365 2073 7461 7473 206f 626a 6563  race stats objec
-00002f60: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
-00002f70: 2073 7461 7469 6f6e 2068 6561 6465 7220   station header 
-00002f80: 696e 666f 0a20 2020 2070 7265 7072 6f5f  info.    prepro_
-00002f90: 7061 7261 3a20 6469 6374 2063 6f6e 7461  para: dict conta
-00002fa0: 696e 696e 6720 6666 7420 7061 7261 6d65  ining fft parame
-00002fb0: 7465 7273 2c20 7375 6368 2061 7320 6672  ters, such as fr
-00002fc0: 6571 7565 6e63 7920 6261 6e64 7320 616e  equency bands an
-00002fd0: 6420 7365 6c65 6374 696f 6e20 666f 7220  d selection for 
-00002fe0: 696e 7374 7275 6d65 6e74 0a20 2020 2072  instrument.    r
-00002ff0: 6573 706f 6e73 6520 7265 6d6f 7661 6c20  esponse removal 
-00003000: 6574 632e 0a20 2020 206c 6f63 733a 2020  etc..    locs:  
-00003010: 7061 6e64 6120 6461 7461 2066 7261 6d65  panda data frame
-00003020: 206f 6620 7468 6520 7374 6174 696f 6e20   of the station 
-00003030: 6c69 7374 2e20 6974 2069 7320 6e65 6564  list. it is need
-00003040: 6564 2066 6f72 2063 6f6e 7665 7269 6e67  ed for convering
-00003050: 206d 696e 6973 6565 6420 6669 6c65 7320   miniseed files 
-00003060: 696e 746f 2041 5344 460a 2020 2020 5245  into ASDF.    RE
-00003070: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-00003080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003090: 2d2d 2d0a 2020 2020 696e 763a 206f 6273  ---.    inv: obs
-000030a0: 7079 2069 6e76 656e 746f 7279 206f 626a  py inventory obj
-000030b0: 6563 7420 6f66 2061 6c6c 2073 7461 7469  ect of all stati
-000030c0: 6f6e 2069 6e66 6f20 746f 2062 6520 7573  on info to be us
-000030d0: 6564 206c 6174 6572 0a20 2020 2022 2222  ed later.    """
-000030e0: 0a20 2020 2073 7461 786d 6c20 3d20 7072  .    staxml = pr
-000030f0: 6570 726f 5f70 6172 615b 2273 7461 7469  epro_para["stati
-00003100: 6f6e 786d 6c22 5d0a 2020 2020 7265 7370  onxml"].    resp
-00003110: 6469 7220 3d20 7072 6570 726f 5f70 6172  dir = prepro_par
-00003120: 615b 2272 6573 7064 6972 225d 0a20 2020  a["respdir"].   
-00003130: 2069 6e70 7574 5f66 6d74 203d 2070 7265   input_fmt = pre
-00003140: 7072 6f5f 7061 7261 5b22 696e 7075 745f  pro_para["input_
-00003150: 666d 7422 5d0a 2020 2020 6966 2073 7461  fmt"].    if sta
-00003160: 786d 6c3a 0a20 2020 2020 2020 2072 6574  xml:.        ret
-00003170: 7572 6e20 7374 6174 7332 496e 765f 7374  urn stats2Inv_st
-00003180: 6178 6d6c 2873 7461 7473 2c20 7265 7370  axml(stats, resp
-00003190: 6469 7229 0a20 2020 2069 6620 696e 7075  dir).    if inpu
-000031a0: 745f 666d 7420 3d3d 2022 7361 6322 3a0a  t_fmt == "sac":.
-000031b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000031c0: 7461 7473 3269 6e76 5f73 6163 2873 7461  tats2inv_sac(sta
-000031d0: 7473 290a 2020 2020 656c 6966 2069 6e70  ts).    elif inp
-000031e0: 7574 5f66 6d74 203d 3d20 226d 7365 6564  ut_fmt == "mseed
-000031f0: 223a 0a20 2020 2020 2020 2072 6574 7572  ":.        retur
-00003200: 6e20 7374 6174 7332 696e 765f 6d73 6565  n stats2inv_msee
-00003210: 6428 7374 6174 732c 206c 6f63 7329 0a0a  d(stats, locs)..
-00003220: 0a64 6566 2073 7461 7473 3249 6e76 5f73  .def stats2Inv_s
-00003230: 7461 786d 6c28 7374 6174 732c 2072 6573  taxml(stats, res
-00003240: 7064 6972 2920 2d3e 2049 6e76 656e 746f  pdir) -> Invento
-00003250: 7279 3a0a 2020 2020 6966 206e 6f74 2072  ry:.    if not r
-00003260: 6573 7064 6972 3a0a 2020 2020 2020 2020  espdir:.        
-00003270: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00003280: 2822 4162 6f72 7421 2073 7461 786d 6c20  ("Abort! staxml 
-00003290: 6973 2073 656c 6563 7465 6420 6275 7420  is selected but 
-000032a0: 6e6f 2064 6972 6563 746f 7279 2069 7320  no directory is 
-000032b0: 6769 7665 6e20 746f 2061 6363 6573 7320  given to access 
-000032c0: 7468 6520 6669 6c65 7322 290a 2020 2020  the files").    
-000032d0: 656c 7365 3a0a 2020 2020 2020 2020 696e  else:.        in
-000032e0: 7666 696c 656c 6973 7420 3d20 676c 6f62  vfilelist = glob
-000032f0: 2e67 6c6f 6228 6f73 2e70 6174 682e 6a6f  .glob(os.path.jo
-00003300: 696e 2872 6573 7064 6972 2c20 222a 2220  in(respdir, "*" 
-00003310: 2b20 7374 6174 732e 7374 6174 696f 6e20  + stats.station 
-00003320: 2b20 222a 2229 290a 2020 2020 2020 2020  + "*")).        
-00003330: 6966 206c 656e 2869 6e76 6669 6c65 6c69  if len(invfileli
-00003340: 7374 2920 3e20 303a 0a20 2020 2020 2020  st) > 0:.       
-00003350: 2020 2020 2069 6e76 6669 6c65 203d 2069       invfile = i
-00003360: 6e76 6669 6c65 6c69 7374 5b30 5d0a 2020  nvfilelist[0].  
-00003370: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00003380: 2869 6e76 6669 6c65 6c69 7374 2920 3e20  (invfilelist) > 
-00003390: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-000033a0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-000033b0: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-000033c0: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2022 5761 726e 696e 6721 204d 6f72 6520   "Warning! More 
-000033f0: 7468 616e 206f 6e65 2053 7461 7469 6f6e  than one Station
-00003400: 584d 4c20 6669 6c65 2077 6173 2066 6f75  XML file was fou
-00003410: 6e64 2066 6f72 2073 7461 7469 6f6e 2025  nd for station %
-00003420: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
-00003430: 2020 2020 2020 2020 2020 2020 2b20 224b              + "K
-00003440: 6565 7069 6e67 2074 6865 2066 6972 7374  eeping the first
-00003450: 2066 696c 6520 696e 206c 6973 742e 220a   file in list.".
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00003480: 2020 2020 2020 2020 2020 2520 7374 6174            % stat
-00003490: 732e 7374 6174 696f 6e0a 2020 2020 2020  s.station.      
-000034a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000034b0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-000034c0: 7468 2e69 7366 696c 6528 7374 7228 696e  th.isfile(str(in
-000034d0: 7666 696c 6529 293a 0a20 2020 2020 2020  vfile)):.       
-000034e0: 2020 2020 2020 2020 2069 6e76 203d 206f           inv = o
-000034f0: 6273 7079 2e72 6561 645f 696e 7665 6e74  bspy.read_invent
-00003500: 6f72 7928 696e 7666 696c 6529 0a20 2020  ory(invfile).   
-00003510: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00003520: 7572 6e20 696e 760a 2020 2020 2020 2020  urn inv.        
-00003530: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003540: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00003550: 6f72 2822 436f 756c 6420 6e6f 7420 6669  or("Could not fi
-00003560: 6e64 2061 2053 7461 7469 6f6e 584d 4c20  nd a StationXML 
-00003570: 6669 6c65 2066 6f72 2073 7461 7469 6f6e  file for station
-00003580: 3a20 2573 2e22 2025 2073 7461 7473 2e73  : %s." % stats.s
-00003590: 7461 7469 6f6e 290a 0a0a 6465 6620 7374  tation)...def st
-000035a0: 6174 7332 696e 765f 7361 6328 7374 6174  ats2inv_sac(stat
-000035b0: 7329 3a0a 2020 2020 696e 7620 3d20 496e  s):.    inv = In
-000035c0: 7665 6e74 6f72 7928 6e65 7477 6f72 6b73  ventory(networks
-000035d0: 3d5b 5d2c 2073 6f75 7263 653d 2268 6f6d  =[], source="hom
-000035e0: 6567 726f 776e 2229 0a20 2020 206e 6574  egrown").    net
-000035f0: 203d 204e 6574 776f 726b 280a 2020 2020   = Network(.    
-00003600: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
-00003610: 6520 6e65 7477 6f72 6b20 636f 6465 2061  e network code a
-00003620: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00003630: 5345 4544 2073 7461 6e64 6172 642e 0a20  SEED standard.. 
-00003640: 2020 2020 2020 2063 6f64 653d 7374 6174         code=stat
-00003650: 732e 6e65 7477 6f72 6b2c 0a20 2020 2020  s.network,.     
-00003660: 2020 2073 7461 7469 6f6e 733d 5b5d 2c0a     stations=[],.
-00003670: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00003680: 696f 6e3d 2263 7265 6174 6564 2066 726f  ion="created fro
-00003690: 6d20 5341 4320 616e 6420 7265 7370 2066  m SAC and resp f
-000036a0: 696c 6573 222c 0a20 2020 2020 2020 2073  iles",.        s
-000036b0: 7461 7274 5f64 6174 653d 7374 6174 732e  tart_date=stats.
-000036c0: 7374 6172 7474 696d 652c 0a20 2020 2029  starttime,.    )
-000036d0: 0a0a 2020 2020 7374 6120 3d20 5374 6174  ..    sta = Stat
-000036e0: 696f 6e28 0a20 2020 2020 2020 2023 2054  ion(.        # T
-000036f0: 6869 7320 6973 2074 6865 2073 7461 7469  his is the stati
-00003700: 6f6e 2063 6f64 6520 6163 636f 7264 696e  on code accordin
-00003710: 6720 746f 2074 6865 2053 4545 4420 7374  g to the SEED st
-00003720: 616e 6461 7264 2e0a 2020 2020 2020 2020  andard..        
-00003730: 636f 6465 3d73 7461 7473 2e73 7461 7469  code=stats.stati
-00003740: 6f6e 2c0a 2020 2020 2020 2020 6c61 7469  on,.        lati
-00003750: 7475 6465 3d73 7461 7473 2e73 6163 5b22  tude=stats.sac["
-00003760: 7374 6c61 225d 2c0a 2020 2020 2020 2020  stla"],.        
-00003770: 6c6f 6e67 6974 7564 653d 7374 6174 732e  longitude=stats.
-00003780: 7361 635b 2273 746c 6f22 5d2c 0a20 2020  sac["stlo"],.   
-00003790: 2020 2020 2065 6c65 7661 7469 6f6e 3d73       elevation=s
-000037a0: 7461 7473 2e73 6163 5b22 7374 656c 225d  tats.sac["stel"]
-000037b0: 2c0a 2020 2020 2020 2020 6372 6561 7469  ,.        creati
-000037c0: 6f6e 5f64 6174 653d 7374 6174 732e 7374  on_date=stats.st
-000037d0: 6172 7474 696d 652c 0a20 2020 2020 2020  arttime,.       
-000037e0: 2073 6974 653d 5369 7465 286e 616d 653d   site=Site(name=
-000037f0: 2246 6972 7374 2073 7461 7469 6f6e 2229  "First station")
-00003800: 2c0a 2020 2020 290a 0a20 2020 2063 6861  ,.    )..    cha
-00003810: 203d 2043 6861 6e6e 656c 280a 2020 2020   = Channel(.    
-00003820: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
-00003830: 6520 6368 616e 6e65 6c20 636f 6465 2061  e channel code a
-00003840: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00003850: 5345 4544 2073 7461 6e64 6172 642e 0a20  SEED standard.. 
-00003860: 2020 2020 2020 2063 6f64 653d 7374 6174         code=stat
-00003870: 732e 6368 616e 6e65 6c2c 0a20 2020 2020  s.channel,.     
-00003880: 2020 2023 2054 6869 7320 6973 2074 6865     # This is the
-00003890: 206c 6f63 6174 696f 6e20 636f 6465 2061   location code a
-000038a0: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-000038b0: 5345 4544 2073 7461 6e64 6172 642e 0a20  SEED standard.. 
-000038c0: 2020 2020 2020 206c 6f63 6174 696f 6e5f         location_
-000038d0: 636f 6465 3d73 7461 7473 2e6c 6f63 6174  code=stats.locat
-000038e0: 696f 6e2c 0a20 2020 2020 2020 2023 204e  ion,.        # N
-000038f0: 6f74 6520 7468 6174 2074 6865 7365 2063  ote that these c
-00003900: 6f6f 7264 696e 6174 6573 2063 616e 2064  oordinates can d
-00003910: 6966 6665 7220 6672 6f6d 2074 6865 2073  iffer from the s
-00003920: 7461 7469 6f6e 2063 6f6f 7264 696e 6174  tation coordinat
-00003930: 6573 2e0a 2020 2020 2020 2020 6c61 7469  es..        lati
-00003940: 7475 6465 3d73 7461 7473 2e73 6163 5b22  tude=stats.sac["
-00003950: 7374 6c61 225d 2c0a 2020 2020 2020 2020  stla"],.        
-00003960: 6c6f 6e67 6974 7564 653d 7374 6174 732e  longitude=stats.
-00003970: 7361 635b 2273 746c 6f22 5d2c 0a20 2020  sac["stlo"],.   
-00003980: 2020 2020 2065 6c65 7661 7469 6f6e 3d73       elevation=s
-00003990: 7461 7473 2e73 6163 5b22 7374 656c 225d  tats.sac["stel"]
-000039a0: 2c0a 2020 2020 2020 2020 6465 7074 683d  ,.        depth=
-000039b0: 2d73 7461 7473 2e73 6163 5b22 7374 656c  -stats.sac["stel
-000039c0: 225d 2c0a 2020 2020 2020 2020 617a 696d  "],.        azim
-000039d0: 7574 683d 7374 6174 732e 7361 635b 2263  uth=stats.sac["c
-000039e0: 6d70 617a 225d 2c0a 2020 2020 2020 2020  mpaz"],.        
-000039f0: 6469 703d 7374 6174 732e 7361 635b 2263  dip=stats.sac["c
-00003a00: 6d70 696e 6322 5d2c 0a20 2020 2020 2020  mpinc"],.       
-00003a10: 2073 616d 706c 655f 7261 7465 3d73 7461   sample_rate=sta
-00003a20: 7473 2e73 616d 706c 696e 675f 7261 7465  ts.sampling_rate
-00003a30: 2c0a 2020 2020 290a 2020 2020 7265 7370  ,.    ).    resp
-00003a40: 6f6e 7365 203d 206f 6273 7079 2e63 6f72  onse = obspy.cor
-00003a50: 652e 696e 7665 6e74 6f72 792e 7265 7370  e.inventory.resp
-00003a60: 6f6e 7365 2e52 6573 706f 6e73 6528 290a  onse.Response().
-00003a70: 0a20 2020 2023 204e 6f77 2074 6965 2069  .    # Now tie i
-00003a80: 7420 616c 6c20 746f 6765 7468 6572 2e0a  t all together..
-00003a90: 2020 2020 6368 612e 7265 7370 6f6e 7365      cha.response
-00003aa0: 203d 2072 6573 706f 6e73 650a 2020 2020   = response.    
-00003ab0: 7374 612e 6368 616e 6e65 6c73 2e61 7070  sta.channels.app
-00003ac0: 656e 6428 6368 6129 0a20 2020 206e 6574  end(cha).    net
-00003ad0: 2e73 7461 7469 6f6e 732e 6170 7065 6e64  .stations.append
-00003ae0: 2873 7461 290a 2020 2020 696e 762e 6e65  (sta).    inv.ne
-00003af0: 7477 6f72 6b73 2e61 7070 656e 6428 6e65  tworks.append(ne
-00003b00: 7429 0a0a 2020 2020 7265 7475 726e 2069  t)..    return i
-00003b10: 6e76 0a0a 0a64 6566 2073 7461 7473 3269  nv...def stats2i
-00003b20: 6e76 5f6d 7365 6564 2873 7461 7473 2c20  nv_mseed(stats, 
-00003b30: 6c6f 6373 3a20 7064 2e44 6174 6146 7261  locs: pd.DataFra
-00003b40: 6d65 2920 2d3e 2049 6e76 656e 746f 7279  me) -> Inventory
-00003b50: 3a0a 2020 2020 696e 7620 3d20 496e 7665  :.    inv = Inve
-00003b60: 6e74 6f72 7928 6e65 7477 6f72 6b73 3d5b  ntory(networks=[
-00003b70: 5d2c 2073 6f75 7263 653d 2268 6f6d 6567  ], source="homeg
-00003b80: 726f 776e 2229 0a20 2020 2069 7374 6120  rown").    ista 
-00003b90: 3d20 6c6f 6373 5b6c 6f63 735b 2273 7461  = locs[locs["sta
-00003ba0: 7469 6f6e 225d 203d 3d20 7374 6174 732e  tion"] == stats.
-00003bb0: 7374 6174 696f 6e5d 2e69 6e64 6578 2e76  station].index.v
-00003bc0: 616c 7565 732e 6173 7479 7065 2822 696e  alues.astype("in
-00003bd0: 7436 3422 295b 305d 0a0a 2020 2020 6e65  t64")[0]..    ne
-00003be0: 7420 3d20 4e65 7477 6f72 6b28 0a20 2020  t = Network(.   
-00003bf0: 2020 2020 2023 2054 6869 7320 6973 2074       # This is t
-00003c00: 6865 206e 6574 776f 726b 2063 6f64 6520  he network code 
-00003c10: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
-00003c20: 2053 4545 4420 7374 616e 6461 7264 2e0a   SEED standard..
-00003c30: 2020 2020 2020 2020 636f 6465 3d6c 6f63          code=loc
-00003c40: 732e 696c 6f63 5b69 7374 615d 5b22 6e65  s.iloc[ista]["ne
-00003c50: 7477 6f72 6b22 5d2c 0a20 2020 2020 2020  twork"],.       
-00003c60: 2073 7461 7469 6f6e 733d 5b5d 2c0a 2020   stations=[],.  
-00003c70: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00003c80: 6e3d 2263 7265 6174 6564 2066 726f 6d20  n="created from 
-00003c90: 5341 4320 616e 6420 7265 7370 2066 696c  SAC and resp fil
-00003ca0: 6573 222c 0a20 2020 2020 2020 2073 7461  es",.        sta
-00003cb0: 7274 5f64 6174 653d 7374 6174 732e 7374  rt_date=stats.st
-00003cc0: 6172 7474 696d 652c 0a20 2020 2029 0a0a  arttime,.    )..
-00003cd0: 2020 2020 7374 6120 3d20 5374 6174 696f      sta = Statio
-00003ce0: 6e28 0a20 2020 2020 2020 2023 2054 6869  n(.        # Thi
-00003cf0: 7320 6973 2074 6865 2073 7461 7469 6f6e  s is the station
-00003d00: 2063 6f64 6520 6163 636f 7264 696e 6720   code according 
-00003d10: 746f 2074 6865 2053 4545 4420 7374 616e  to the SEED stan
-00003d20: 6461 7264 2e0a 2020 2020 2020 2020 636f  dard..        co
-00003d30: 6465 3d6c 6f63 732e 696c 6f63 5b69 7374  de=locs.iloc[ist
-00003d40: 615d 5b22 7374 6174 696f 6e22 5d2c 0a20  a]["station"],. 
-00003d50: 2020 2020 2020 206c 6174 6974 7564 653d         latitude=
-00003d60: 6c6f 6373 2e69 6c6f 635b 6973 7461 5d5b  locs.iloc[ista][
-00003d70: 226c 6174 6974 7564 6522 5d2c 0a20 2020  "latitude"],.   
-00003d80: 2020 2020 206c 6f6e 6769 7475 6465 3d6c       longitude=l
-00003d90: 6f63 732e 696c 6f63 5b69 7374 615d 5b22  ocs.iloc[ista]["
-00003da0: 6c6f 6e67 6974 7564 6522 5d2c 0a20 2020  longitude"],.   
-00003db0: 2020 2020 2065 6c65 7661 7469 6f6e 3d6c       elevation=l
-00003dc0: 6f63 732e 696c 6f63 5b69 7374 615d 5b22  ocs.iloc[ista]["
-00003dd0: 656c 6576 6174 696f 6e22 5d2c 0a20 2020  elevation"],.   
-00003de0: 2020 2020 2063 7265 6174 696f 6e5f 6461       creation_da
-00003df0: 7465 3d73 7461 7473 2e73 7461 7274 7469  te=stats.startti
-00003e00: 6d65 2c0a 2020 2020 2020 2020 7369 7465  me,.        site
-00003e10: 3d53 6974 6528 6e61 6d65 3d22 4669 7273  =Site(name="Firs
-00003e20: 7420 7374 6174 696f 6e22 292c 0a20 2020  t station"),.   
-00003e30: 2029 0a0a 2020 2020 6368 6120 3d20 4368   )..    cha = Ch
-00003e40: 616e 6e65 6c28 0a20 2020 2020 2020 2063  annel(.        c
-00003e50: 6f64 653d 7374 6174 732e 6368 616e 6e65  ode=stats.channe
-00003e60: 6c2c 0a20 2020 2020 2020 206c 6f63 6174  l,.        locat
-00003e70: 696f 6e5f 636f 6465 3d73 7461 7473 2e6c  ion_code=stats.l
-00003e80: 6f63 6174 696f 6e2c 0a20 2020 2020 2020  ocation,.       
-00003e90: 206c 6174 6974 7564 653d 6c6f 6373 2e69   latitude=locs.i
-00003ea0: 6c6f 635b 6973 7461 5d5b 226c 6174 6974  loc[ista]["latit
-00003eb0: 7564 6522 5d2c 0a20 2020 2020 2020 206c  ude"],.        l
-00003ec0: 6f6e 6769 7475 6465 3d6c 6f63 732e 696c  ongitude=locs.il
-00003ed0: 6f63 5b69 7374 615d 5b22 6c6f 6e67 6974  oc[ista]["longit
-00003ee0: 7564 6522 5d2c 0a20 2020 2020 2020 2065  ude"],.        e
-00003ef0: 6c65 7661 7469 6f6e 3d6c 6f63 732e 696c  levation=locs.il
-00003f00: 6f63 5b69 7374 615d 5b22 656c 6576 6174  oc[ista]["elevat
-00003f10: 696f 6e22 5d2c 0a20 2020 2020 2020 2064  ion"],.        d
-00003f20: 6570 7468 3d2d 6c6f 6373 2e69 6c6f 635b  epth=-locs.iloc[
-00003f30: 6973 7461 5d5b 2265 6c65 7661 7469 6f6e  ista]["elevation
-00003f40: 225d 2c0a 2020 2020 2020 2020 617a 696d  "],.        azim
-00003f50: 7574 683d 302c 0a20 2020 2020 2020 2064  uth=0,.        d
-00003f60: 6970 3d30 2c0a 2020 2020 2020 2020 7361  ip=0,.        sa
-00003f70: 6d70 6c65 5f72 6174 653d 7374 6174 732e  mple_rate=stats.
-00003f80: 7361 6d70 6c69 6e67 5f72 6174 652c 0a20  sampling_rate,. 
-00003f90: 2020 2029 0a0a 2020 2020 7265 7370 6f6e     )..    respon
-00003fa0: 7365 203d 206f 6273 7079 2e63 6f72 652e  se = obspy.core.
-00003fb0: 696e 7665 6e74 6f72 792e 7265 7370 6f6e  inventory.respon
-00003fc0: 7365 2e52 6573 706f 6e73 6528 290a 0a20  se.Response().. 
-00003fd0: 2020 2023 204e 6f77 2074 6965 2069 7420     # Now tie it 
-00003fe0: 616c 6c20 746f 6765 7468 6572 2e0a 2020  all together..  
-00003ff0: 2020 6368 612e 7265 7370 6f6e 7365 203d    cha.response =
-00004000: 2072 6573 706f 6e73 650a 2020 2020 7374   response.    st
-00004010: 612e 6368 616e 6e65 6c73 2e61 7070 656e  a.channels.appen
-00004020: 6428 6368 6129 0a20 2020 206e 6574 2e73  d(cha).    net.s
-00004030: 7461 7469 6f6e 732e 6170 7065 6e64 2873  tations.append(s
-00004040: 7461 290a 2020 2020 696e 762e 6e65 7477  ta).    inv.netw
-00004050: 6f72 6b73 2e61 7070 656e 6428 6e65 7429  orks.append(net)
-00004060: 0a0a 2020 2020 7265 7475 726e 2069 6e76  ..    return inv
-00004070: 0a0a 0a64 6566 2073 7461 5f69 6e66 6f5f  ...def sta_info_
-00004080: 6672 6f6d 5f69 6e76 2869 6e76 3a20 6f62  from_inv(inv: ob
-00004090: 7370 792e 636f 7265 2e69 6e76 656e 746f  spy.core.invento
-000040a0: 7279 2e69 6e76 656e 746f 7279 2e49 6e76  ry.inventory.Inv
-000040b0: 656e 746f 7279 293a 0a20 2020 2022 2222  entory):.    """
-000040c0: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
-000040d0: 6f6e 206f 7574 7075 7473 2073 7461 7469  on outputs stati
-000040e0: 6f6e 2069 6e66 6f20 6672 6f6d 2074 6865  on info from the
-000040f0: 206f 6273 7079 2069 6e76 656e 746f 7279   obspy inventory
-00004100: 206f 626a 6563 740a 2020 2020 2875 7365   object.    (use
-00004110: 6420 696e 2053 3042 290a 2020 2020 5041  d in S0B).    PA
-00004120: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
-00004130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004140: 2d2d 2d2d 0a20 2020 2069 6e76 3a20 6f62  ----.    inv: ob
-00004150: 7370 7920 696e 7665 6e74 6f72 7920 6f62  spy inventory ob
-00004160: 6a65 6374 0a20 2020 2052 4554 5552 4e53  ject.    RETURNS
-00004170: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00004180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00004190: 2073 7461 3a20 7374 6174 696f 6e20 6e61   sta: station na
-000041a0: 6d65 0a20 2020 206e 6574 3a20 6e65 746f  me.    net: neto
-000041b0: 7772 6b20 6e61 6d65 0a20 2020 206c 6f6e  wrk name.    lon
-000041c0: 3a20 6c6f 6e67 6974 7564 6520 6f66 2074  : longitude of t
-000041d0: 6865 2073 7461 7469 6f6e 0a20 2020 206c  he station.    l
-000041e0: 6174 3a20 6c61 7469 7475 6465 206f 6620  at: latitude of 
-000041f0: 7468 6520 7374 6174 696f 6e0a 2020 2020  the station.    
-00004200: 656c 763a 2065 6c65 7661 7469 6f6e 206f  elv: elevation o
-00004210: 6620 7468 6520 7374 6174 696f 6e0a 2020  f the station.  
-00004220: 2020 6c6f 6361 7469 6f6e 3a20 6c6f 6361    location: loca
-00004230: 7469 6f6e 2063 6f64 6520 6f66 2074 6865  tion code of the
-00004240: 2073 7461 7469 6f6e 0a20 2020 2022 2222   station.    """
-00004250: 0a20 2020 2023 206c 6f61 6420 6672 6f6d  .    # load from
-00004260: 2073 7461 7469 6f6e 2069 6e76 656e 746f   station invento
-00004270: 7279 0a20 2020 2073 7461 203d 2069 6e76  ry.    sta = inv
-00004280: 5b30 5d5b 305d 2e63 6f64 650a 2020 2020  [0][0].code.    
-00004290: 6e65 7420 3d20 696e 765b 305d 2e63 6f64  net = inv[0].cod
-000042a0: 650a 2020 2020 6c6f 6e20 3d20 696e 765b  e.    lon = inv[
-000042b0: 305d 5b30 5d2e 6c6f 6e67 6974 7564 650a  0][0].longitude.
-000042c0: 2020 2020 6c61 7420 3d20 696e 765b 305d      lat = inv[0]
-000042d0: 5b30 5d2e 6c61 7469 7475 6465 0a20 2020  [0].latitude.   
-000042e0: 2069 6620 696e 765b 305d 5b30 5d2e 656c   if inv[0][0].el
-000042f0: 6576 6174 696f 6e3a 0a20 2020 2020 2020  evation:.       
-00004300: 2065 6c76 203d 2069 6e76 5b30 5d5b 305d   elv = inv[0][0]
-00004310: 2e65 6c65 7661 7469 6f6e 0a20 2020 2065  .elevation.    e
-00004320: 6c73 653a 0a20 2020 2020 2020 2065 6c76  lse:.        elv
-00004330: 203d 2030 2e30 0a0a 2020 2020 6966 2069   = 0.0..    if i
-00004340: 6e76 5b30 5d5b 305d 5b30 5d2e 6c6f 6361  nv[0][0][0].loca
-00004350: 7469 6f6e 5f63 6f64 653a 0a20 2020 2020  tion_code:.     
-00004360: 2020 206c 6f63 6174 696f 6e20 3d20 696e     location = in
-00004370: 765b 305d 5b30 5d5b 305d 2e6c 6f63 6174  v[0][0][0].locat
-00004380: 696f 6e5f 636f 6465 0a20 2020 2065 6c73  ion_code.    els
-00004390: 653a 0a20 2020 2020 2020 206c 6f63 6174  e:.        locat
-000043a0: 696f 6e20 3d20 2230 3022 0a0a 2020 2020  ion = "00"..    
-000043b0: 7265 7475 726e 2073 7461 2c20 6e65 742c  return sta, net,
-000043c0: 206c 6f6e 2c20 6c61 742c 2065 6c76 2c20   lon, lat, elv, 
-000043d0: 6c6f 6361 7469 6f6e 0a0a 0a64 6566 2063  location...def c
-000043e0: 7574 5f74 7261 6365 5f6d 616b 655f 7374  ut_trace_make_st
-000043f0: 6174 2866 635f 7061 7261 3a20 436f 6e66  at(fc_para: Conf
-00004400: 6967 5061 7261 6d65 7465 7273 2c20 6368  igParameters, ch
-00004410: 5f64 6174 613a 2043 6861 6e6e 656c 4461  _data: ChannelDa
-00004420: 7461 293a 0a20 2020 2022 2222 0a20 2020  ta):.    """.   
-00004430: 2074 6869 7320 6675 6e63 7469 6f6e 2063   this function c
-00004440: 7574 7320 636f 6e74 696e 6f75 7320 6e6f  uts continous no
-00004450: 6973 6520 6461 7461 2069 6e74 6f20 7573  ise data into us
-00004460: 6572 2d64 6566 696e 6564 2073 6567 6d65  er-defined segme
-00004470: 6e74 732c 2065 7374 696d 6174 6520 7468  nts, estimate th
-00004480: 6520 7374 6174 6973 7469 6373 206f 660a  e statistics of.
-00004490: 2020 2020 6561 6368 2073 6567 6d65 6e74      each segment
-000044a0: 2061 6e64 206b 6565 7020 7469 6d65 7374   and keep timest
-000044b0: 616d 7020 6f66 2065 6163 6820 7365 676d  amp of each segm
-000044c0: 656e 7420 666f 7220 6c61 7465 7220 7573  ent for later us
-000044d0: 652e 2028 7573 6564 2069 6e20 5331 290a  e. (used in S1).
-000044e0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-000044f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00004500: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
-00004510: 6674 5f70 6172 613a 2041 2064 6963 7469  ft_para: A dicti
-00004520: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
-00004530: 2061 6c6c 2066 6674 2061 6e64 2063 6320   all fft and cc 
-00004540: 7061 7261 6d65 7465 7273 2e0a 2020 2020  parameters..    
-00004550: 736f 7572 6365 3a20 6f62 7370 7920 7374  source: obspy st
-00004560: 7265 616d 206f 626a 6563 740a 2020 2020  ream object.    
-00004570: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
-00004580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004590: 2d2d 2d0a 2020 2020 7472 6163 655f 7374  ---.    trace_st
-000045a0: 6453 3a20 7374 616e 6461 7264 2064 6576  dS: standard dev
-000045b0: 6961 7469 6f6e 206f 6620 7468 6520 6e6f  iation of the no
-000045c0: 6973 6520 616d 706c 6974 7564 6520 6f66  ise amplitude of
-000045d0: 2065 6163 6820 7365 676d 656e 740a 2020   each segment.  
-000045e0: 2020 6461 7461 535f 743a 2020 2020 7469    dataS_t:    ti
-000045f0: 6d65 7374 616d 7073 206f 6620 6561 6368  mestamps of each
-00004600: 2073 6567 6d65 6e74 0a20 2020 2064 6174   segment.    dat
-00004610: 6153 3a20 2020 2020 2032 4420 6d61 7472  aS:      2D matr
-00004620: 6978 206f 6620 7468 6520 7365 676d 656e  ix of the segmen
-00004630: 7465 6420 6461 7461 0a20 2020 2022 2222  ted data.    """
-00004640: 0a20 2020 2023 2064 6566 696e 6520 7265  .    # define re
-00004650: 7475 726e 2076 6172 6961 626c 6573 2066  turn variables f
-00004660: 6972 7374 0a20 2020 2073 6f75 7263 655f  irst.    source_
-00004670: 7061 7261 6d73 203d 205b 5d0a 2020 2020  params = [].    
-00004680: 6461 7461 535f 7420 3d20 5b5d 0a20 2020  dataS_t = [].   
-00004690: 2064 6174 6153 203d 205b 5d0a 0a20 2020   dataS = []..   
-000046a0: 2023 2075 7365 6675 6c20 7061 7261 6d65   # useful parame
-000046b0: 7465 7273 2066 6f72 2074 7261 6365 2073  ters for trace s
-000046c0: 6c69 6469 6e67 0a20 2020 206e 7365 6720  liding.    nseg 
-000046d0: 3d20 696e 7428 6e70 2e66 6c6f 6f72 2828  = int(np.floor((
-000046e0: 6663 5f70 6172 612e 696e 635f 686f 7572  fc_para.inc_hour
-000046f0: 7320 2f20 3234 202a 2038 3634 3030 202d  s / 24 * 86400 -
-00004700: 2066 635f 7061 7261 2e63 635f 6c65 6e29   fc_para.cc_len)
-00004710: 202f 2066 635f 7061 7261 2e73 7465 7029   / fc_para.step)
-00004720: 290a 2020 2020 7370 7320 3d20 696e 7428  ).    sps = int(
-00004730: 6368 5f64 6174 612e 7361 6d70 6c69 6e67  ch_data.sampling
-00004740: 5f72 6174 6529 0a20 2020 2073 7461 7274  _rate).    start
-00004750: 7469 6d65 203d 2063 685f 6461 7461 2e73  time = ch_data.s
-00004760: 7461 7274 5f74 696d 6573 7461 6d70 0a20  tart_timestamp. 
-00004770: 2020 2023 2063 6f70 7920 6461 7461 2069     # copy data i
-00004780: 6e74 6f20 6172 7261 790a 2020 2020 6461  nto array.    da
-00004790: 7461 203d 2063 685f 6461 7461 2e64 6174  ta = ch_data.dat
-000047a0: 610a 0a20 2020 2023 2069 6620 7468 6520  a..    # if the 
-000047b0: 6461 7461 2069 7320 7368 6f72 7465 7220  data is shorter 
-000047c0: 7468 616e 2074 6865 2074 696d 2063 6875  than the tim chu
-000047d0: 6e63 6b2c 2072 6574 7572 6e20 7a65 726f  nck, return zero
-000047e0: 2076 616c 7565 730a 2020 2020 6966 2064   values.    if d
-000047f0: 6174 612e 7369 7a65 203c 2073 7073 202a  ata.size < sps *
-00004800: 2066 635f 7061 7261 2e69 6e63 5f68 6f75   fc_para.inc_hou
-00004810: 7273 202a 2033 3630 303a 0a20 2020 2020  rs * 3600:.     
-00004820: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00004830: 6728 0a20 2020 2020 2020 2020 2020 2066  g(.            f
-00004840: 2254 6865 2064 6174 6120 287b 6461 7461  "The data ({data
-00004850: 2e73 697a 657d 2920 6973 2073 686f 7274  .size}) is short
-00004860: 6572 2074 6861 6e20 7468 6520 7469 6d65  er than the time
-00004870: 2063 6875 6e6b 2028 7b73 7073 2a66 635f   chunk ({sps*fc_
-00004880: 7061 7261 2e69 6e63 5f68 6f75 7273 2a33  para.inc_hours*3
-00004890: 3630 307d 2922 0a20 2020 2020 2020 2020  600})".         
-000048a0: 2020 2022 2c20 7265 7475 726e 696e 6720     ", returning 
-000048b0: 7a65 726f 2076 616c 7565 732e 220a 2020  zero values.".  
-000048c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000048d0: 7265 7475 726e 2073 6f75 7263 655f 7061  return source_pa
-000048e0: 7261 6d73 2c20 6461 7461 535f 742c 2064  rams, dataS_t, d
-000048f0: 6174 6153 0a0a 2020 2020 2320 7374 6174  ataS..    # stat
-00004900: 6973 7469 6320 746f 2064 6574 6563 7420  istic to detect 
-00004910: 7365 676d 656e 7473 2074 6861 7420 6d61  segments that ma
-00004920: 7920 6265 2061 7373 6f63 6961 7465 6420  y be associated 
-00004930: 7769 7468 2065 6172 7468 7175 616b 6573  with earthquakes
-00004940: 0a20 2020 2061 6c6c 5f6d 6164 5320 3d20  .    all_madS = 
-00004950: 6d61 6428 6461 7461 2920 2023 206d 6564  mad(data)  # med
-00004960: 6961 6e20 6162 736f 6c75 7465 2064 6576  ian absolute dev
-00004970: 6961 7469 6f6e 206f 7665 7220 616c 6c20  iation over all 
-00004980: 6e6f 6973 6520 7769 6e64 6f77 0a20 2020  noise window.   
-00004990: 2061 6c6c 5f73 7464 5320 3d20 6e70 2e73   all_stdS = np.s
-000049a0: 7464 2864 6174 6129 2020 2320 7374 616e  td(data)  # stan
-000049b0: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
-000049c0: 7665 7220 616c 6c20 6e6f 6973 6520 7769  ver all noise wi
-000049d0: 6e64 6f77 0a20 2020 2069 6620 616c 6c5f  ndow.    if all_
-000049e0: 6d61 6453 203d 3d20 3020 6f72 2061 6c6c  madS == 0 or all
-000049f0: 5f73 7464 5320 3d3d 2030 206f 7220 6e70  _stdS == 0 or np
-00004a00: 2e69 736e 616e 2861 6c6c 5f6d 6164 5329  .isnan(all_madS)
-00004a10: 206f 7220 6e70 2e69 736e 616e 2861 6c6c   or np.isnan(all
-00004a20: 5f73 7464 5329 3a0a 2020 2020 2020 2020  _stdS):.        
-00004a30: 6c6f 6767 6572 2e64 6562 7567 2822 636f  logger.debug("co
-00004a40: 6e74 696e 7565 2120 6d61 6453 206f 7220  ntinue! madS or 
-00004a50: 7374 6453 2065 7175 616c 7320 746f 2030  stdS equals to 0
-00004a60: 2066 6f72 2025 7322 290a 2020 2020 2020   for %s").      
-00004a70: 2020 7265 7475 726e 2073 6f75 7263 655f    return source_
-00004a80: 7061 7261 6d73 2c20 6461 7461 535f 742c  params, dataS_t,
-00004a90: 2064 6174 6153 0a0a 2020 2020 2320 696e   dataS..    # in
-00004aa0: 6974 6961 6c69 7a65 2076 6172 6961 626c  itialize variabl
-00004ab0: 6573 0a20 2020 206e 7074 7320 3d20 696e  es.    npts = in
-00004ac0: 7428 6663 5f70 6172 612e 6363 5f6c 656e  t(fc_para.cc_len
-00004ad0: 202a 2073 7073 290a 2020 2020 2320 7472   * sps).    # tr
-00004ae0: 6163 655f 6d61 6453 203d 206e 702e 7a65  ace_madS = np.ze
-00004af0: 726f 7328 6e73 6567 2c64 7479 7065 3d6e  ros(nseg,dtype=n
-00004b00: 702e 666c 6f61 7433 3229 0a20 2020 2074  p.float32).    t
-00004b10: 7261 6365 5f73 7464 5320 3d20 6e70 2e7a  race_stdS = np.z
-00004b20: 6572 6f73 286e 7365 672c 2064 7479 7065  eros(nseg, dtype
-00004b30: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
-00004b40: 2064 6174 6153 203d 206e 702e 7a65 726f   dataS = np.zero
-00004b50: 7328 7368 6170 653d 2869 6e74 286e 7365  s(shape=(int(nse
-00004b60: 6729 2c20 696e 7428 6e70 7473 2929 2c20  g), int(npts)), 
-00004b70: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00004b80: 290a 2020 2020 6461 7461 535f 7420 3d20  ).    dataS_t = 
-00004b90: 6e70 2e7a 6572 6f73 286e 7365 672c 2064  np.zeros(nseg, d
-00004ba0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00004bb0: 0a0a 2020 2020 696e 6478 3120 3d20 300a  ..    indx1 = 0.
-00004bc0: 2020 2020 666f 7220 6973 6567 2069 6e20      for iseg in 
-00004bd0: 7261 6e67 6528 6e73 6567 293a 0a20 2020  range(nseg):.   
-00004be0: 2020 2020 2069 6e64 7832 203d 2069 6e64       indx2 = ind
-00004bf0: 7831 202b 206e 7074 730a 2020 2020 2020  x1 + npts.      
-00004c00: 2020 6461 7461 535b 6973 6567 5d20 3d20    dataS[iseg] = 
-00004c10: 6461 7461 5b69 6e64 7831 3a69 6e64 7832  data[indx1:indx2
-00004c20: 5d0a 2020 2020 2020 2020 2320 7472 6163  ].        # trac
-00004c30: 655f 6d61 6453 5b69 7365 675d 203d 2028  e_madS[iseg] = (
-00004c40: 6e70 2e6d 6178 286e 702e 6162 7328 6461  np.max(np.abs(da
-00004c50: 7461 535b 6973 6567 5d29 292f 616c 6c5f  taS[iseg]))/all_
-00004c60: 6d61 6453 290a 2020 2020 2020 2020 7472  madS).        tr
-00004c70: 6163 655f 7374 6453 5b69 7365 675d 203d  ace_stdS[iseg] =
-00004c80: 206e 702e 6d61 7828 6e70 2e61 6273 2864   np.max(np.abs(d
-00004c90: 6174 6153 5b69 7365 675d 2929 202f 2061  ataS[iseg])) / a
-00004ca0: 6c6c 5f73 7464 530a 2020 2020 2020 2020  ll_stdS.        
-00004cb0: 6461 7461 535f 745b 6973 6567 5d20 3d20  dataS_t[iseg] = 
-00004cc0: 7374 6172 7474 696d 6520 2b20 6663 5f70  starttime + fc_p
-00004cd0: 6172 612e 7374 6570 202a 2069 7365 670a  ara.step * iseg.
-00004ce0: 2020 2020 2020 2020 696e 6478 3120 3d20          indx1 = 
-00004cf0: 696e 6478 3120 2b20 696e 7428 6663 5f70  indx1 + int(fc_p
-00004d00: 6172 612e 7374 6570 2920 2a20 7370 730a  ara.step) * sps.
-00004d10: 0a20 2020 2023 2032 4420 6172 7261 7920  .    # 2D array 
-00004d20: 7072 6f63 6573 7369 6e67 0a20 2020 2064  processing.    d
-00004d30: 6174 6153 203d 2064 656d 6561 6e28 6461  ataS = demean(da
-00004d40: 7461 5329 0a20 2020 2064 6174 6153 203d  taS).    dataS =
-00004d50: 2064 6574 7265 6e64 2864 6174 6153 290a   detrend(dataS).
-00004d60: 2020 2020 6461 7461 5320 3d20 7461 7065      dataS = tape
-00004d70: 7228 6461 7461 5329 0a0a 2020 2020 7265  r(dataS)..    re
-00004d80: 7475 726e 2074 7261 6365 5f73 7464 532c  turn trace_stdS,
-00004d90: 2064 6174 6153 5f74 2c20 6461 7461 530a   dataS_t, dataS.
-00004da0: 0a0a 6465 6620 6e6f 6973 655f 7072 6f63  ..def noise_proc
-00004db0: 6573 7369 6e67 2866 6674 5f70 6172 612c  essing(fft_para,
-00004dc0: 2064 6174 6153 293a 0a20 2020 2022 2222   dataS):.    """
-00004dd0: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
-00004de0: 6f6e 2070 6572 666f 726d 7320 7469 6d65  on performs time
-00004df0: 2064 6f6d 6169 6e20 616e 6420 6672 6571   domain and freq
-00004e00: 7565 6e63 7920 646f 6d61 696e 206e 6f72  uency domain nor
-00004e10: 6d61 6c69 7a61 7469 6f6e 2069 6620 6e65  malization if ne
-00004e20: 6564 6564 2e20 696e 2072 6561 6c20 6361  eded. in real ca
-00004e30: 7365 2c20 7765 2070 7265 6665 7220 7573  se, we prefer us
-00004e40: 6520 696e 636c 7564 650a 2020 2020 7468  e include.    th
-00004e50: 6520 6e6f 726d 616c 697a 6174 696f 6e20  e normalization 
-00004e60: 696e 2074 6865 2063 726f 7373 2d63 6f72  in the cross-cor
-00004e70: 7265 616c 7469 6f6e 2073 7465 7073 2062  realtion steps b
-00004e80: 7920 7365 6c65 6374 696e 6720 636f 6865  y selecting cohe
-00004e90: 7265 6e63 7920 6f72 2064 6563 6f6e 0a20  rency or decon. 
-00004ea0: 2020 2028 5072 6965 746f 2065 7420 616c     (Prieto et al
-00004eb0: 2c20 3230 3038 2c20 3230 3039 3b20 4465  , 2008, 2009; De
-00004ec0: 6e6f 6c6c 6520 6574 2061 6c2c 2032 3031  nolle et al, 201
-00004ed0: 3329 0a20 2020 2050 4152 4d41 4554 4552  3).    PARMAETER
-00004ee0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00004ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00004f00: 2020 2020 6666 745f 7061 7261 3a20 6469      fft_para: di
-00004f10: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-00004f20: 696e 6720 616c 6c20 7573 6566 756c 2076  ing all useful v
-00004f30: 6172 6961 626c 6573 2075 7365 6420 666f  ariables used fo
-00004f40: 7220 6666 7420 616e 6420 6363 0a20 2020  r fft and cc.   
-00004f50: 2064 6174 6153 3a20 3244 206d 6174 7269   dataS: 2D matri
-00004f60: 7820 6f66 2061 6c6c 2073 6567 6d65 6e74  x of all segment
-00004f70: 6564 206e 6f69 7365 2064 6174 610a 2020  ed noise data.  
-00004f80: 2020 2320 4f55 5450 5554 2056 4152 4941    # OUTPUT VARIA
-00004f90: 424c 4553 3a0a 2020 2020 736f 7572 6365  BLES:.    source
-00004fa0: 5f77 6869 7465 3a20 3244 206d 6174 7269  _white: 2D matri
-00004fb0: 7820 6f66 2064 6174 6120 7370 6563 7472  x of data spectr
-00004fc0: 610a 2020 2020 2222 220a 2020 2020 2320  a.    """.    # 
-00004fd0: 6c6f 6164 2070 6172 616d 6574 6572 7320  load parameters 
-00004fe0: 6669 7273 740a 2020 2020 7469 6d65 5f6e  first.    time_n
-00004ff0: 6f72 6d20 3d20 6666 745f 7061 7261 5b22  orm = fft_para["
-00005000: 7469 6d65 5f6e 6f72 6d22 5d0a 2020 2020  time_norm"].    
-00005010: 6672 6571 5f6e 6f72 6d20 3d20 6666 745f  freq_norm = fft_
-00005020: 7061 7261 5b22 6672 6571 5f6e 6f72 6d22  para["freq_norm"
-00005030: 5d0a 2020 2020 736d 6f6f 7468 5f4e 203d  ].    smooth_N =
-00005040: 2066 6674 5f70 6172 615b 2273 6d6f 6f74   fft_para["smoot
-00005050: 685f 4e22 5d0a 2020 2020 4e20 3d20 6461  h_N"].    N = da
-00005060: 7461 532e 7368 6170 655b 305d 0a0a 2020  taS.shape[0]..  
-00005070: 2020 2320 2d2d 2d2d 2d2d 746f 206e 6f72    # ------to nor
-00005080: 6d61 6c69 7a65 2069 6e20 7469 6d65 206f  malize in time o
-00005090: 7220 6e6f 742d 2d2d 2d2d 2d0a 2020 2020  r not------.    
-000050a0: 6966 2074 696d 655f 6e6f 726d 2021 3d20  if time_norm != 
-000050b0: 226e 6f22 3a0a 2020 2020 2020 2020 6966  "no":.        if
-000050c0: 2074 696d 655f 6e6f 726d 203d 3d20 226f   time_norm == "o
-000050d0: 6e65 5f62 6974 223a 2020 2320 7369 676e  ne_bit":  # sign
-000050e0: 206e 6f72 6d61 6c69 7a61 7469 6f6e 0a20   normalization. 
-000050f0: 2020 2020 2020 2020 2020 2077 6869 7465             white
-00005100: 203d 206e 702e 7369 676e 2864 6174 6153   = np.sign(dataS
-00005110: 290a 2020 2020 2020 2020 656c 6966 2074  ).        elif t
-00005120: 696d 655f 6e6f 726d 203d 3d20 2272 6d61  ime_norm == "rma
-00005130: 223a 2020 2320 7275 6e6e 696e 6720 6d65  ":  # running me
-00005140: 616e 3a20 6e6f 726d 616c 697a 6174 696f  an: normalizatio
-00005150: 6e20 6f76 6572 2073 6d6f 6f74 6865 6420  n over smoothed 
-00005160: 6162 736f 6c75 7465 2061 7665 7261 6765  absolute average
-00005170: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
-00005180: 7465 203d 206e 702e 7a65 726f 7328 7368  te = np.zeros(sh
-00005190: 6170 653d 6461 7461 532e 7368 6170 652c  ape=dataS.shape,
-000051a0: 2064 7479 7065 3d64 6174 6153 2e64 7479   dtype=dataS.dty
-000051b0: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
-000051c0: 666f 7220 6b6b 6b20 696e 2072 616e 6765  for kkk in range
-000051d0: 284e 293a 0a20 2020 2020 2020 2020 2020  (N):.           
-000051e0: 2020 2020 2077 6869 7465 5b6b 6b6b 2c20       white[kkk, 
-000051f0: 3a5d 203d 2064 6174 6153 5b6b 6b6b 2c20  :] = dataS[kkk, 
-00005200: 3a5d 202f 206d 6f76 696e 675f 6176 6528  :] / moving_ave(
-00005210: 6e70 2e61 6273 2864 6174 6153 5b6b 6b6b  np.abs(dataS[kkk
-00005220: 2c20 3a5d 292c 2073 6d6f 6f74 685f 4e29  , :]), smooth_N)
-00005230: 0a0a 2020 2020 656c 7365 3a20 2023 2064  ..    else:  # d
-00005240: 6f6e 2774 206e 6f72 6d61 6c69 7a65 0a20  on't normalize. 
-00005250: 2020 2020 2020 2077 6869 7465 203d 2064         white = d
-00005260: 6174 6153 0a0a 2020 2020 2320 2d2d 2d2d  ataS..    # ----
-00005270: 2d74 6f20 7768 6974 656e 206f 7220 6e6f  -to whiten or no
-00005280: 742d 2d2d 2d2d 2d0a 2020 2020 6966 2066  t------.    if f
-00005290: 7265 715f 6e6f 726d 2021 3d20 226e 6f22  req_norm != "no"
-000052a0: 3a0a 2020 2020 2020 2020 736f 7572 6365  :.        source
-000052b0: 5f77 6869 7465 203d 2077 6869 7465 6e28  _white = whiten(
-000052c0: 7768 6974 652c 2066 6674 5f70 6172 6129  white, fft_para)
-000052d0: 2020 2320 7768 6974 656e 2061 6e64 2072    # whiten and r
-000052e0: 6574 7572 6e20 4646 540a 2020 2020 656c  eturn FFT.    el
-000052f0: 7365 3a0a 2020 2020 2020 2020 4e66 6674  se:.        Nfft
-00005300: 203d 2069 6e74 286e 6578 745f 6661 7374   = int(next_fast
-00005310: 5f6c 656e 2869 6e74 2864 6174 6153 2e73  _len(int(dataS.s
-00005320: 6861 7065 5b31 5d29 2929 0a20 2020 2020  hape[1]))).     
-00005330: 2020 2073 6f75 7263 655f 7768 6974 6520     source_white 
-00005340: 3d20 7363 6970 792e 6666 7470 6163 6b2e  = scipy.fftpack.
-00005350: 6666 7428 7768 6974 652c 204e 6666 742c  fft(white, Nfft,
-00005360: 2061 7869 733d 3129 2020 2320 7265 7475   axis=1)  # retu
-00005370: 726e 2046 4654 0a0a 2020 2020 7265 7475  rn FFT..    retu
-00005380: 726e 2073 6f75 7263 655f 7768 6974 650a  rn source_white.
-00005390: 0a0a 6465 6620 736d 6f6f 7468 5f73 6f75  ..def smooth_sou
-000053a0: 7263 655f 7370 6563 7428 6363 5f70 6172  rce_spect(cc_par
-000053b0: 612c 2066 6674 3129 3a0a 2020 2020 2222  a, fft1):.    ""
-000053c0: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
-000053d0: 696f 6e20 736d 6f6f 7468 6573 2061 6d70  ion smoothes amp
-000053e0: 6c69 7475 6465 2073 7065 6374 7275 6d20  litude spectrum 
-000053f0: 6f66 2074 6865 2032 4420 7370 6563 7472  of the 2D spectr
-00005400: 616c 206d 6174 7269 782e 2028 7573 6564  al matrix. (used
-00005410: 2069 6e20 5331 290a 2020 2020 5041 5241   in S1).    PARA
-00005420: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-00005430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005440: 2d0a 2020 2020 6363 5f70 6172 613a 2064  -.    cc_para: d
-00005450: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-00005460: 6e69 6e67 2075 7365 6675 6c20 6363 2070  ning useful cc p
-00005470: 6172 616d 6574 6572 730a 2020 2020 6666  arameters.    ff
-00005480: 7431 3a20 2020 2073 6f75 7263 6520 7370  t1:    source sp
-00005490: 6563 7472 756d 206d 6174 7269 780a 0a20  ectrum matrix.. 
-000054a0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-000054b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000054c0: 2d2d 2d2d 2d0a 2020 2020 7366 6674 313a  -----.    sfft1:
-000054d0: 2063 6f6d 706c 6578 206e 756d 7079 2061   complex numpy a
-000054e0: 7272 6179 2077 6974 6820 6e6f 726d 616c  rray with normal
-000054f0: 697a 6564 2073 7065 6374 7275 6d0a 2020  ized spectrum.  
-00005500: 2020 2222 220a 2020 2020 6363 5f6d 6574    """.    cc_met
-00005510: 686f 6420 3d20 6363 5f70 6172 615b 2263  hod = cc_para["c
-00005520: 635f 6d65 7468 6f64 225d 0a20 2020 2073  c_method"].    s
-00005530: 6d6f 6f74 6873 7065 6374 5f4e 203d 2063  moothspect_N = c
-00005540: 635f 7061 7261 5b22 736d 6f6f 7468 7370  c_para["smoothsp
-00005550: 6563 745f 4e22 5d0a 0a20 2020 2069 6620  ect_N"]..    if 
-00005560: 6363 5f6d 6574 686f 6420 3d3d 2022 6465  cc_method == "de
-00005570: 636f 6e76 223a 0a20 2020 2020 2020 2023  conv":.        #
-00005580: 202d 2d2d 2d2d 6e6f 726d 616c 697a 6520   -----normalize 
-00005590: 7369 6e67 6c65 2d73 7461 7469 6f6e 2063  single-station c
-000055a0: 6320 746f 207a 2063 6f6d 706f 6e65 6e74  c to z component
-000055b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7465  -----.        te
-000055c0: 6d70 203d 206d 6f76 696e 675f 6176 6528  mp = moving_ave(
-000055d0: 6e70 2e61 6273 2866 6674 3129 2c20 736d  np.abs(fft1), sm
-000055e0: 6f6f 7468 7370 6563 745f 4e29 0a20 2020  oothspect_N).   
-000055f0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00005600: 2020 2020 2020 7366 6674 3120 3d20 6e70        sfft1 = np
-00005610: 2e63 6f6e 6a28 6666 7431 2920 2f20 7465  .conj(fft1) / te
-00005620: 6d70 2a2a 320a 2020 2020 2020 2020 6578  mp**2.        ex
-00005630: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
-00005640: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00005650: 6520 5661 6c75 6545 7272 6f72 2822 736d  e ValueError("sm
-00005660: 6f6f 7468 6564 2073 7065 6374 7275 6d20  oothed spectrum 
-00005670: 6861 7320 7a65 726f 2076 616c 7565 7322  has zero values"
-00005680: 290a 0a20 2020 2065 6c69 6620 6363 5f6d  )..    elif cc_m
-00005690: 6574 686f 6420 3d3d 2022 636f 6865 7265  ethod == "cohere
-000056a0: 6e63 7922 3a0a 2020 2020 2020 2020 7465  ncy":.        te
-000056b0: 6d70 203d 206d 6f76 696e 675f 6176 6528  mp = moving_ave(
-000056c0: 6e70 2e61 6273 2866 6674 3129 2c20 736d  np.abs(fft1), sm
-000056d0: 6f6f 7468 7370 6563 745f 4e29 0a20 2020  oothspect_N).   
-000056e0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000056f0: 2020 2020 2020 7366 6674 3120 3d20 6e70        sfft1 = np
-00005700: 2e63 6f6e 6a28 6666 7431 2920 2f20 7465  .conj(fft1) / te
-00005710: 6d70 0a20 2020 2020 2020 2065 7863 6570  mp.        excep
-00005720: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
-00005730: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00005740: 616c 7565 4572 726f 7228 2273 6d6f 6f74  alueError("smoot
-00005750: 6865 6420 7370 6563 7472 756d 2068 6173  hed spectrum has
-00005760: 207a 6572 6f20 7661 6c75 6573 2229 0a0a   zero values")..
-00005770: 2020 2020 656c 6966 2063 635f 6d65 7468      elif cc_meth
-00005780: 6f64 203d 3d20 2278 636f 7272 223a 0a20  od == "xcorr":. 
-00005790: 2020 2020 2020 2073 6666 7431 203d 206e         sfft1 = n
-000057a0: 702e 636f 6e6a 2866 6674 3129 0a0a 2020  p.conj(fft1)..  
-000057b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000057c0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000057d0: 2822 6e6f 2063 6f72 7265 6374 696f 6e20  ("no correction 
-000057e0: 636f 7272 656c 6174 696f 6e20 6d65 7468  correlation meth
-000057f0: 6f64 2069 7320 7365 6c65 6374 6564 2061  od is selected a
-00005800: 7420 4c35 3922 290a 0a20 2020 2072 6574  t L59")..    ret
-00005810: 7572 6e20 7366 6674 310a 0a0a 6465 6620  urn sfft1...def 
-00005820: 636f 7272 656c 6174 6528 6666 7431 5f73  correlate(fft1_s
-00005830: 6d6f 6f74 6865 645f 6162 732c 2066 6674  moothed_abs, fft
-00005840: 322c 2044 2c20 4e66 6674 2c20 6461 7461  2, D, Nfft, data
-00005850: 535f 7429 3a0a 2020 2020 2222 220a 2020  S_t):.    """.  
-00005860: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
-00005870: 646f 6573 2074 6865 2063 726f 7373 2d63  does the cross-c
-00005880: 6f72 7265 6c61 7469 6f6e 2069 6e20 6672  orrelation in fr
-00005890: 6571 2064 6f6d 6169 6e20 616e 6420 6861  eq domain and ha
-000058a0: 7320 7468 6520 6f70 7469 6f6e 2074 6f20  s the option to 
-000058b0: 6b65 6570 2073 7562 2d73 7461 636b 7320  keep sub-stacks 
-000058c0: 6f66 0a20 2020 2074 6865 2063 726f 7373  of.    the cross
-000058d0: 2d63 6f72 7265 6c61 7469 6f6e 2069 6620  -correlation if 
-000058e0: 6e65 6564 6564 2e20 6974 2074 616b 6573  needed. it takes
-000058f0: 2061 6476 616e 7461 6765 206f 6620 7468   advantage of th
-00005900: 6520 6c69 6e65 6172 2072 656c 6174 696f  e linear relatio
-00005910: 6e73 6869 7020 6f66 2069 6666 742c 2073  nship of ifft, s
-00005920: 6f20 7468 6174 0a20 2020 2073 7461 636b  o that.    stack
-00005930: 696e 6720 6973 2070 6572 666f 726d 6564  ing is performed
-00005940: 2069 6e20 7370 6563 7472 756d 2064 6f6d   in spectrum dom
-00005950: 6169 6e20 6669 7273 7420 746f 2072 6564  ain first to red
-00005960: 7563 6520 7468 6520 746f 7461 6c20 6e75  uce the total nu
-00005970: 6d62 6572 206f 6620 6966 6674 2e20 2875  mber of ifft. (u
-00005980: 7365 6420 696e 2053 3129 0a20 2020 2050  sed in S1).    P
-00005990: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
-000059a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000059b0: 2d2d 2d2d 0a20 2020 2066 6674 315f 736d  ----.    fft1_sm
-000059c0: 6f6f 7468 6564 5f61 6273 3a20 736d 6f6f  oothed_abs: smoo
-000059d0: 7468 6564 2070 6f77 6572 2073 7065 6374  thed power spect
-000059e0: 7261 6c20 6465 6e73 6974 7920 6f66 2074  ral density of t
-000059f0: 6865 2046 4654 2066 6f72 2074 6865 2073  he FFT for the s
-00005a00: 6f75 7263 6520 7374 6174 696f 6e0a 2020  ource station.  
-00005a10: 2020 6666 7432 3a20 7261 7720 4646 5420    fft2: raw FFT 
-00005a20: 7370 6563 7472 756d 206f 6620 7468 6520  spectrum of the 
-00005a30: 7265 6365 6976 6572 2073 7461 7469 6f6e  receiver station
-00005a40: 0a20 2020 2044 3a20 6469 6374 696f 6e61  .    D: dictiona
-00005a50: 7279 2063 6f6e 7461 696e 696e 6720 666f  ry containing fo
-00005a60: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
-00005a70: 7273 3a0a 2020 2020 2020 2020 6d61 786c  rs:.        maxl
-00005a80: 6167 3a20 206d 6178 696d 756d 206c 6167  ag:  maximum lag
-00005a90: 7320 746f 206b 6565 7020 696e 2074 6865  s to keep in the
-00005aa0: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
-00005ab0: 6f6e 0a20 2020 2020 2020 2064 743a 2020  on.        dt:  
-00005ac0: 2020 2020 7361 6d70 6c69 6e67 2072 6174      sampling rat
-00005ad0: 6520 2869 6e20 7329 0a20 2020 2020 2020  e (in s).       
-00005ae0: 206e 7769 6e3a 2020 2020 6e75 6d62 6572   nwin:    number
-00005af0: 206f 6620 7365 676d 656e 7473 2069 6e20   of segments in 
-00005b00: 7468 6520 3244 206d 6174 7269 780a 2020  the 2D matrix.  
-00005b10: 2020 2020 2020 6d65 7468 6f64 3a20 2063        method:  c
-00005b20: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
-00005b30: 206d 6574 686f 6473 2073 656c 6563 7465   methods selecte
-00005b40: 6420 6279 2074 6865 2075 7365 720a 2020  d by the user.  
-00005b50: 2020 2020 2020 6672 6571 6d69 6e3a 206d        freqmin: m
-00005b60: 696e 696d 756d 2066 7265 7175 656e 6379  inimum frequency
-00005b70: 2028 487a 290a 2020 2020 2020 2020 6672   (Hz).        fr
-00005b80: 6571 6d61 783a 206d 6178 696d 756d 2066  eqmax: maximum f
-00005b90: 7265 7175 656e 6379 2028 487a 290a 2020  requency (Hz).  
-00005ba0: 2020 4e66 6674 3a20 2020 206e 756d 6265    Nfft:    numbe
-00005bb0: 7220 6f66 2066 7265 7175 656e 6379 2070  r of frequency p
-00005bc0: 6f69 6e74 7320 666f 7220 6966 6674 0a20  oints for ifft. 
-00005bd0: 2020 2064 6174 6153 5f74 3a20 6d61 7472     dataS_t: matr
-00005be0: 6978 206f 6620 6461 7465 7469 6d65 206f  ix of datetime o
-00005bf0: 626a 6563 742e 0a0a 2020 2020 5245 5455  bject...    RETU
-00005c00: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
-00005c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00005c20: 2020 2073 5f63 6f72 723a 2031 4420 6f72     s_corr: 1D or
-00005c30: 2032 4420 6d61 7472 6978 206f 6620 7468   2D matrix of th
-00005c40: 6520 6176 6572 6167 6564 206f 7220 7375  e averaged or su
-00005c50: 622d 7374 6163 6b73 206f 6620 6372 6f73  b-stacks of cros
-00005c60: 732d 636f 7272 656c 6174 696f 6e20 6675  s-correlation fu
-00005c70: 6e63 7469 6f6e 7320 696e 2074 696d 6520  nctions in time 
-00005c80: 646f 6d61 696e 0a20 2020 2074 5f63 6f72  domain.    t_cor
-00005c90: 723a 2074 696d 6573 7461 6d70 2066 6f72  r: timestamp for
-00005ca0: 2065 6163 6820 7375 622d 7374 6163 6b20   each sub-stack 
-00005cb0: 6f72 2061 7665 7261 6765 6420 6675 6e63  or averaged func
-00005cc0: 7469 6f6e 0a20 2020 206e 5f63 6f72 723a  tion.    n_corr:
-00005cd0: 206e 756d 6265 7220 6f66 2069 6e63 6c75   number of inclu
-00005ce0: 6465 6420 7365 676d 656e 7473 2066 6f72  ded segments for
-00005cf0: 2065 6163 6820 7375 622d 7374 6163 6b20   each sub-stack 
-00005d00: 6f72 2061 7665 7261 6765 6420 6675 6e63  or averaged func
-00005d10: 7469 6f6e 0a0a 2020 2020 4d4f 4449 4649  tion..    MODIFI
-00005d20: 4341 5449 4f4e 533a 0a20 2020 202d 2d2d  CATIONS:.    ---
-00005d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005d40: 2d2d 0a20 2020 206f 7574 7075 7420 7468  --.    output th
-00005d50: 6520 6c69 6e65 6172 2073 7461 636b 206f  e linear stack o
-00005d60: 6620 6561 6368 2074 696d 6520 6368 756e  f each time chun
-00005d70: 6b20 6576 656e 2077 6865 6e20 7375 6273  k even when subs
-00005d80: 7461 636b 2069 7320 7365 6c65 6374 6564  tack is selected
-00005d90: 2028 6279 2043 6865 6e67 7869 6e20 4041   (by Chengxin @A
-00005da0: 7567 3230 3230 290a 2020 2020 2222 220a  ug2020).    """.
-00005db0: 2020 2020 2320 2d2d 2d2d 6c6f 6164 2070      # ----load p
-00005dc0: 6172 616d 7465 7273 2d2d 2d2d 0a20 2020  aramters----.   
-00005dd0: 2064 7420 3d20 445b 2264 7422 5d0a 2020   dt = D["dt"].  
-00005de0: 2020 6d61 786c 6167 203d 2044 5b22 6d61    maxlag = D["ma
-00005df0: 786c 6167 225d 0a20 2020 206d 6574 686f  xlag"].    metho
-00005e00: 6420 3d20 445b 2263 635f 6d65 7468 6f64  d = D["cc_method
-00005e10: 225d 0a20 2020 2063 635f 6c65 6e20 3d20  "].    cc_len = 
-00005e20: 445b 2263 635f 6c65 6e22 5d0a 2020 2020  D["cc_len"].    
-00005e30: 7375 6273 7461 636b 203d 2044 5b22 7375  substack = D["su
-00005e40: 6273 7461 636b 225d 0a20 2020 2073 7562  bstack"].    sub
-00005e50: 7374 6163 6b5f 6c65 6e20 3d20 445b 2273  stack_len = D["s
-00005e60: 7562 7374 6163 6b5f 6c65 6e22 5d0a 2020  ubstack_len"].  
-00005e70: 2020 736d 6f6f 7468 7370 6563 745f 4e20    smoothspect_N 
-00005e80: 3d20 445b 2273 6d6f 6f74 6873 7065 6374  = D["smoothspect
-00005e90: 5f4e 225d 0a0a 2020 2020 6e77 696e 203d  _N"]..    nwin =
-00005ea0: 2066 6674 315f 736d 6f6f 7468 6564 5f61   fft1_smoothed_a
-00005eb0: 6273 2e73 6861 7065 5b30 5d0a 2020 2020  bs.shape[0].    
-00005ec0: 4e66 6674 3220 3d20 6666 7431 5f73 6d6f  Nfft2 = fft1_smo
-00005ed0: 6f74 6865 645f 6162 732e 7368 6170 655b  othed_abs.shape[
-00005ee0: 315d 0a0a 2020 2020 2320 2d2d 2d2d 2d2d  1]..    # ------
-00005ef0: 636f 6e76 6572 7420 616c 6c20 3244 2061  convert all 2D a
-00005f00: 7272 6179 7320 696e 746f 2031 4420 746f  rrays into 1D to
-00005f10: 2073 7065 6564 2075 702d 2d2d 2d2d 2d2d   speed up-------
-00005f20: 2d0a 2020 2020 636f 7272 203d 206e 702e  -.    corr = np.
-00005f30: 7a65 726f 7328 6e77 696e 202a 204e 6666  zeros(nwin * Nff
-00005f40: 7432 2c20 6474 7970 653d 6e70 2e63 6f6d  t2, dtype=np.com
-00005f50: 706c 6578 3634 290a 2020 2020 636f 7272  plex64).    corr
-00005f60: 203d 2066 6674 315f 736d 6f6f 7468 6564   = fft1_smoothed
-00005f70: 5f61 6273 2e72 6573 6861 7065 280a 2020  _abs.reshape(.  
-00005f80: 2020 2020 2020 6666 7431 5f73 6d6f 6f74        fft1_smoot
-00005f90: 6865 645f 6162 732e 7369 7a65 2c0a 2020  hed_abs.size,.  
-00005fa0: 2020 2920 2a20 6666 7432 2e72 6573 6861    ) * fft2.resha
-00005fb0: 7065 280a 2020 2020 2020 2020 6666 7432  pe(.        fft2
-00005fc0: 2e73 697a 652c 0a20 2020 2029 0a0a 2020  .size,.    )..  
-00005fd0: 2020 6966 206d 6574 686f 6420 3d3d 2022    if method == "
-00005fe0: 636f 6865 7265 6e63 7922 3a0a 2020 2020  coherency":.    
-00005ff0: 2020 2020 7465 6d70 203d 206d 6f76 696e      temp = movin
-00006000: 675f 6176 6528 0a20 2020 2020 2020 2020  g_ave(.         
-00006010: 2020 206e 702e 6162 7328 0a20 2020 2020     np.abs(.     
-00006020: 2020 2020 2020 2020 2020 2066 6674 322e             fft2.
-00006030: 7265 7368 6170 6528 0a20 2020 2020 2020  reshape(.       
-00006040: 2020 2020 2020 2020 2020 2020 2066 6674               fft
-00006050: 322e 7369 7a65 2c0a 2020 2020 2020 2020  2.size,.        
-00006060: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006070: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00006080: 2020 2020 2073 6d6f 6f74 6873 7065 6374       smoothspect
-00006090: 5f4e 2c0a 2020 2020 2020 2020 290a 2020  _N,.        ).  
-000060a0: 2020 2020 2020 636f 7272 202f 3d20 7465        corr /= te
-000060b0: 6d70 0a20 2020 2063 6f72 7220 3d20 636f  mp.    corr = co
-000060c0: 7272 2e72 6573 6861 7065 286e 7769 6e2c  rr.reshape(nwin,
-000060d0: 204e 6666 7432 290a 0a20 2020 2069 6620   Nfft2)..    if 
-000060e0: 7375 6273 7461 636b 3a0a 2020 2020 2020  substack:.      
-000060f0: 2020 6966 2073 7562 7374 6163 6b5f 6c65    if substack_le
-00006100: 6e20 3d3d 2063 635f 6c65 6e3a 0a20 2020  n == cc_len:.   
-00006110: 2020 2020 2020 2020 2023 2063 686f 6f73           # choos
-00006120: 6520 746f 206b 6565 7020 616c 6c20 6666  e to keep all ff
-00006130: 7420 6461 7461 2066 6f72 2061 2064 6179  t data for a day
-00006140: 0a20 2020 2020 2020 2020 2020 2073 5f63  .            s_c
-00006150: 6f72 7220 3d20 6e70 2e7a 6572 6f73 2873  orr = np.zeros(s
-00006160: 6861 7065 3d28 6e77 696e 2c20 4e66 6674  hape=(nwin, Nfft
-00006170: 292c 2064 7479 7065 3d6e 702e 666c 6f61  ), dtype=np.floa
-00006180: 7433 3229 2020 2320 7374 6163 6b65 6420  t32)  # stacked 
-00006190: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
-000061a0: 2020 2020 2020 2020 616d 706d 6178 203d          ampmax =
-000061b0: 206e 702e 7a65 726f 7328 6e77 696e 2c20   np.zeros(nwin, 
-000061c0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-000061d0: 290a 2020 2020 2020 2020 2020 2020 6e5f  ).            n_
-000061e0: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
-000061f0: 6e77 696e 2c20 6474 7970 653d 6e70 2e69  nwin, dtype=np.i
-00006200: 6e74 3136 2920 2023 206e 756d 6265 7220  nt16)  # number 
-00006210: 6f66 2063 6f72 7265 6c61 7469 6f6e 7320  of correlations 
-00006220: 666f 7220 6561 6368 2073 7562 7374 6163  for each substac
-00006230: 6b0a 2020 2020 2020 2020 2020 2020 745f  k.            t_
-00006240: 636f 7272 203d 2064 6174 6153 5f74 2020  corr = dataS_t  
-00006250: 2320 7469 6d65 7374 616d 700a 2020 2020  # timestamp.    
-00006260: 2020 2020 2020 2020 6372 6170 203d 206e          crap = n
-00006270: 702e 7a65 726f 7328 4e66 6674 2c20 6474  p.zeros(Nfft, dt
-00006280: 7970 653d 6e70 2e63 6f6d 706c 6578 3634  ype=np.complex64
-00006290: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-000062a0: 7220 6920 696e 2072 616e 6765 286e 7769  r i in range(nwi
-000062b0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-000062c0: 2020 2020 6e5f 636f 7272 5b69 5d20 3d20      n_corr[i] = 
-000062d0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-000062e0: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
-000062f0: 2063 6f72 725b 692c 203a 5d0a 2020 2020   corr[i, :].    
-00006300: 2020 2020 2020 2020 2020 2020 6372 6170              crap
-00006310: 5b3a 4e66 6674 325d 203d 2063 7261 705b  [:Nfft2] = crap[
-00006320: 3a4e 6666 7432 5d20 2d20 6e70 2e6d 6561  :Nfft2] - np.mea
-00006330: 6e28 6372 6170 5b3a 4e66 6674 325d 2920  n(crap[:Nfft2]) 
-00006340: 2023 2072 656d 6f76 6520 7468 6520 6d65   # remove the me
-00006350: 616e 2069 6e20 6672 6571 2064 6f6d 6169  an in freq domai
-00006360: 6e20 2873 7069 6b65 2061 7420 743d 3029  n (spike at t=0)
-00006370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006380: 2063 7261 705b 2d28 4e66 6674 3229 202b   crap[-(Nfft2) +
-00006390: 2031 203a 5d20 3d20 6e70 2e66 6c69 7028   1 :] = np.flip(
-000063a0: 6e70 2e63 6f6e 6a28 6372 6170 5b31 3a28  np.conj(crap[1:(
-000063b0: 4e66 6674 3229 5d29 2c20 6178 6973 3d30  Nfft2)]), axis=0
-000063c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000063d0: 2020 6372 6170 5b30 5d20 3d20 636f 6d70    crap[0] = comp
-000063e0: 6c65 7828 302c 2030 290a 2020 2020 2020  lex(0, 0).      
-000063f0: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
-00006400: 5b69 2c20 3a5d 203d 206e 702e 7265 616c  [i, :] = np.real
-00006410: 286e 702e 6666 742e 6966 6674 7368 6966  (np.fft.ifftshif
-00006420: 7428 7363 6970 792e 6666 7470 6163 6b2e  t(scipy.fftpack.
-00006430: 6966 6674 2863 7261 702c 204e 6666 742c  ifft(crap, Nfft,
-00006440: 2061 7869 733d 3029 2929 0a0a 2020 2020   axis=0)))..    
-00006450: 2020 2020 2020 2020 2320 7265 6d6f 7665          # remove
-00006460: 2061 626e 6f72 6d61 6c20 6461 7461 0a20   abnormal data. 
-00006470: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
-00006480: 7820 3d20 6e70 2e6d 6178 2873 5f63 6f72  x = np.max(s_cor
-00006490: 722c 2061 7869 733d 3129 0a20 2020 2020  r, axis=1).     
-000064a0: 2020 2020 2020 2074 696e 6478 203d 206e         tindx = n
-000064b0: 702e 7768 6572 6528 2861 6d70 6d61 7820  p.where((ampmax 
-000064c0: 3c20 3230 202a 206e 702e 6d65 6469 616e  < 20 * np.median
-000064d0: 2861 6d70 6d61 7829 2920 2620 2861 6d70  (ampmax)) & (amp
-000064e0: 6d61 7820 3e20 3029 295b 305d 0a20 2020  max > 0))[0].   
-000064f0: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
-00006500: 3d20 735f 636f 7272 5b74 696e 6478 2c20  = s_corr[tindx, 
-00006510: 3a5d 0a20 2020 2020 2020 2020 2020 2074  :].            t
-00006520: 5f63 6f72 7220 3d20 745f 636f 7272 5b74  _corr = t_corr[t
-00006530: 696e 6478 5d0a 2020 2020 2020 2020 2020  indx].          
-00006540: 2020 6e5f 636f 7272 203d 206e 5f63 6f72    n_corr = n_cor
-00006550: 725b 7469 6e64 785d 0a0a 2020 2020 2020  r[tindx]..      
-00006560: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00006570: 2020 2020 2320 6765 7420 7469 6d65 2069      # get time i
-00006580: 6e66 6f72 6d61 7469 6f6e 0a20 2020 2020  nformation.     
-00006590: 2020 2020 2020 2054 746f 7461 6c20 3d20         Ttotal = 
-000065a0: 6461 7461 535f 745b 2d31 5d20 2d20 6461  dataS_t[-1] - da
-000065b0: 7461 535f 745b 305d 2020 2320 746f 7461  taS_t[0]  # tota
-000065c0: 6c20 6475 7261 7469 6f6e 206f 6620 7768  l duration of wh
-000065d0: 6174 2077 6520 6861 7665 206e 6f77 0a20  at we have now. 
-000065e0: 2020 2020 2020 2020 2020 2074 7374 6172             tstar
-000065f0: 7420 3d20 6461 7461 535f 745b 305d 0a0a  t = dataS_t[0]..
-00006600: 2020 2020 2020 2020 2020 2020 6e73 7461              nsta
-00006610: 636b 203d 2069 6e74 286e 702e 726f 756e  ck = int(np.roun
-00006620: 6428 5474 6f74 616c 202f 2073 7562 7374  d(Ttotal / subst
-00006630: 6163 6b5f 6c65 6e29 290a 2020 2020 2020  ack_len)).      
-00006640: 2020 2020 2020 616d 706d 6178 203d 206e        ampmax = n
-00006650: 702e 7a65 726f 7328 6e73 7461 636b 2c20  p.zeros(nstack, 
-00006660: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00006670: 290a 2020 2020 2020 2020 2020 2020 735f  ).            s_
-00006680: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
-00006690: 7368 6170 653d 286e 7374 6163 6b2c 204e  shape=(nstack, N
-000066a0: 6666 7429 2c20 6474 7970 653d 6e70 2e66  fft), dtype=np.f
-000066b0: 6c6f 6174 3332 290a 2020 2020 2020 2020  loat32).        
-000066c0: 2020 2020 6e5f 636f 7272 203d 206e 702e      n_corr = np.
-000066d0: 7a65 726f 7328 6e73 7461 636b 2c20 6474  zeros(nstack, dt
-000066e0: 7970 653d 6e70 2e69 6e74 3136 290a 2020  ype=np.int16).  
-000066f0: 2020 2020 2020 2020 2020 745f 636f 7272            t_corr
-00006700: 203d 206e 702e 7a65 726f 7328 6e73 7461   = np.zeros(nsta
-00006710: 636b 2c20 6474 7970 653d 6e70 2e66 6c6f  ck, dtype=np.flo
-00006720: 6174 3332 290a 2020 2020 2020 2020 2020  at32).          
-00006730: 2020 6372 6170 203d 206e 702e 7a65 726f    crap = np.zero
-00006740: 7328 4e66 6674 2c20 6474 7970 653d 6e70  s(Nfft, dtype=np
-00006750: 2e63 6f6d 706c 6578 3634 290a 0a20 2020  .complex64)..   
-00006760: 2020 2020 2020 2020 2066 6f72 2069 7374           for ist
-00006770: 6163 6b20 696e 2072 616e 6765 286e 7374  ack in range(nst
-00006780: 6163 6b29 3a0a 2020 2020 2020 2020 2020  ack):.          
-00006790: 2020 2020 2020 2320 6669 6e64 2074 6865        # find the
-000067a0: 2069 6e64 6578 6573 206f 6620 616c 6c20   indexes of all 
-000067b0: 6f66 2074 6865 2077 696e 646f 7773 2074  of the windows t
-000067c0: 6861 7420 7374 6172 7420 6f72 2065 6e64  hat start or end
-000067d0: 2077 6974 6869 6e0a 2020 2020 2020 2020   within.        
-000067e0: 2020 2020 2020 2020 6974 696d 6520 3d20          itime = 
-000067f0: 6e70 2e77 6865 7265 2828 6461 7461 535f  np.where((dataS_
-00006800: 7420 3e3d 2074 7374 6172 7429 2026 2028  t >= tstart) & (
-00006810: 6461 7461 535f 7420 3c20 7473 7461 7274  dataS_t < tstart
-00006820: 202b 2073 7562 7374 6163 6b5f 6c65 6e29   + substack_len)
-00006830: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-00006840: 2020 2020 2069 6620 6c65 6e28 6974 696d       if len(itim
-00006850: 6529 203d 3d20 303a 0a20 2020 2020 2020  e) == 0:.       
-00006860: 2020 2020 2020 2020 2020 2020 2074 7374               tst
-00006870: 6172 7420 2b3d 2073 7562 7374 6163 6b5f  art += substack_
-00006880: 6c65 6e0a 2020 2020 2020 2020 2020 2020  len.            
-00006890: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-000068a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000068b0: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
-000068c0: 206e 702e 6d65 616e 2863 6f72 725b 6974   np.mean(corr[it
-000068d0: 696d 652c 203a 5d2c 2061 7869 733d 3029  ime, :], axis=0)
-000068e0: 2020 2320 6c69 6e65 6172 2061 7665 7261    # linear avera
-000068f0: 6765 206f 6620 7468 6520 636f 7272 656c  ge of the correl
-00006900: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-00006910: 2020 2020 2020 6372 6170 5b3a 4e66 6674        crap[:Nfft
-00006920: 325d 203d 2063 7261 705b 3a4e 6666 7432  2] = crap[:Nfft2
-00006930: 5d20 2d20 6e70 2e6d 6561 6e28 6372 6170  ] - np.mean(crap
-00006940: 5b3a 4e66 6674 325d 2920 2023 2072 656d  [:Nfft2])  # rem
-00006950: 6f76 6520 7468 6520 6d65 616e 2069 6e20  ove the mean in 
-00006960: 6672 6571 2064 6f6d 6169 6e20 2873 7069  freq domain (spi
-00006970: 6b65 2061 7420 743d 3029 0a20 2020 2020  ke at t=0).     
-00006980: 2020 2020 2020 2020 2020 2063 7261 705b             crap[
-00006990: 2d28 4e66 6674 3229 202b 2031 203a 5d20  -(Nfft2) + 1 :] 
-000069a0: 3d20 6e70 2e66 6c69 7028 6e70 2e63 6f6e  = np.flip(np.con
-000069b0: 6a28 6372 6170 5b31 3a28 4e66 6674 3229  j(crap[1:(Nfft2)
-000069c0: 5d29 2c20 6178 6973 3d30 290a 2020 2020  ]), axis=0).    
-000069d0: 2020 2020 2020 2020 2020 2020 6372 6170              crap
-000069e0: 5b30 5d20 3d20 636f 6d70 6c65 7828 302c  [0] = complex(0,
-000069f0: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-00006a00: 2020 2020 735f 636f 7272 5b69 7374 6163      s_corr[istac
-00006a10: 6b2c 203a 5d20 3d20 6e70 2e72 6561 6c28  k, :] = np.real(
-00006a20: 6e70 2e66 6674 2e69 6666 7473 6869 6674  np.fft.ifftshift
-00006a30: 2873 6369 7079 2e66 6674 7061 636b 2e69  (scipy.fftpack.i
-00006a40: 6666 7428 6372 6170 2c20 4e66 6674 2c20  fft(crap, Nfft, 
-00006a50: 6178 6973 3d30 2929 290a 2020 2020 2020  axis=0))).      
-00006a60: 2020 2020 2020 2020 2020 6e5f 636f 7272            n_corr
-00006a70: 5b69 7374 6163 6b5d 203d 206c 656e 2869  [istack] = len(i
-00006a80: 7469 6d65 2920 2023 206e 756d 6265 7220  time)  # number 
-00006a90: 6f66 2077 696e 646f 7773 2073 7461 636b  of windows stack
-00006aa0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00006ab0: 2020 745f 636f 7272 5b69 7374 6163 6b5d    t_corr[istack]
-00006ac0: 203d 2074 7374 6172 7420 2023 2073 6176   = tstart  # sav
-00006ad0: 6520 7468 6520 7469 6d65 2073 7461 6d70  e the time stamp
-00006ae0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00006af0: 2020 7473 7461 7274 202b 3d20 7375 6273    tstart += subs
-00006b00: 7461 636b 5f6c 656e 0a20 2020 2020 2020  tack_len.       
-00006b10: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
-00006b20: 2827 636f 7272 656c 6174 696f 6e20 646f  ('correlation do
-00006b30: 6e65 2061 6e64 2073 7461 636b 6564 2061  ne and stacked a
-00006b40: 7420 7469 6d65 2025 7327 2025 2073 7472  t time %s' % str
-00006b50: 2874 5f63 6f72 725b 6973 7461 636b 5d29  (t_corr[istack])
-00006b60: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00006b70: 2072 656d 6f76 6520 6162 6e6f 726d 616c   remove abnormal
-00006b80: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
-00006b90: 2020 616d 706d 6178 203d 206e 702e 6d61    ampmax = np.ma
-00006ba0: 7828 735f 636f 7272 2c20 6178 6973 3d31  x(s_corr, axis=1
-00006bb0: 290a 2020 2020 2020 2020 2020 2020 7469  ).            ti
-00006bc0: 6e64 7820 3d20 6e70 2e77 6865 7265 2828  ndx = np.where((
-00006bd0: 616d 706d 6178 203c 2032 3020 2a20 6e70  ampmax < 20 * np
-00006be0: 2e6d 6564 6961 6e28 616d 706d 6178 2929  .median(ampmax))
-00006bf0: 2026 2028 616d 706d 6178 203e 2030 2929   & (ampmax > 0))
-00006c00: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00006c10: 735f 636f 7272 203d 2073 5f63 6f72 725b  s_corr = s_corr[
-00006c20: 7469 6e64 782c 203a 5d0a 2020 2020 2020  tindx, :].      
-00006c30: 2020 2020 2020 745f 636f 7272 203d 2074        t_corr = t
-00006c40: 5f63 6f72 725b 7469 6e64 785d 0a20 2020  _corr[tindx].   
-00006c50: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
-00006c60: 3d20 6e5f 636f 7272 5b74 696e 6478 5d0a  = n_corr[tindx].
-00006c70: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00006c80: 2020 2023 2061 7665 7261 6765 2064 6169     # average dai
-00006c90: 6c79 2063 726f 7373 2063 6f72 7265 6c61  ly cross correla
-00006ca0: 7469 6f6e 2066 756e 6374 696f 6e73 0a20  tion functions. 
-00006cb0: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
-00006cc0: 6e70 2e6d 6178 2863 6f72 722c 2061 7869  np.max(corr, axi
-00006cd0: 733d 3129 0a20 2020 2020 2020 2074 696e  s=1).        tin
-00006ce0: 6478 203d 206e 702e 7768 6572 6528 2861  dx = np.where((a
-00006cf0: 6d70 6d61 7820 3c20 3230 202a 206e 702e  mpmax < 20 * np.
-00006d00: 6d65 6469 616e 2861 6d70 6d61 7829 2920  median(ampmax)) 
-00006d10: 2620 2861 6d70 6d61 7820 3e20 3029 295b  & (ampmax > 0))[
-00006d20: 305d 0a20 2020 2020 2020 206e 5f63 6f72  0].        n_cor
-00006d30: 7220 3d20 6e77 696e 0a20 2020 2020 2020  r = nwin.       
-00006d40: 2073 5f63 6f72 7220 3d20 6e70 2e7a 6572   s_corr = np.zer
-00006d50: 6f73 284e 6666 742c 2064 7479 7065 3d6e  os(Nfft, dtype=n
-00006d60: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
-00006d70: 2020 2074 5f63 6f72 7220 3d20 6461 7461     t_corr = data
-00006d80: 535f 745b 305d 0a20 2020 2020 2020 2063  S_t[0].        c
-00006d90: 7261 7020 3d20 6e70 2e7a 6572 6f73 284e  rap = np.zeros(N
-00006da0: 6666 742c 2064 7479 7065 3d6e 702e 636f  fft, dtype=np.co
-00006db0: 6d70 6c65 7836 3429 0a20 2020 2020 2020  mplex64).       
-00006dc0: 2063 7261 705b 3a4e 6666 7432 5d20 3d20   crap[:Nfft2] = 
-00006dd0: 6e70 2e6d 6561 6e28 636f 7272 5b74 696e  np.mean(corr[tin
-00006de0: 6478 5d2c 2061 7869 733d 3029 0a20 2020  dx], axis=0).   
-00006df0: 2020 2020 2063 7261 705b 3a4e 6666 7432       crap[:Nfft2
-00006e00: 5d20 3d20 6372 6170 5b3a 4e66 6674 325d  ] = crap[:Nfft2]
-00006e10: 202d 206e 702e 6d65 616e 2863 7261 705b   - np.mean(crap[
-00006e20: 3a4e 6666 7432 5d2c 2061 7869 733d 3029  :Nfft2], axis=0)
-00006e30: 0a20 2020 2020 2020 2063 7261 705b 2d28  .        crap[-(
-00006e40: 4e66 6674 3229 202b 2031 203a 5d20 3d20  Nfft2) + 1 :] = 
-00006e50: 6e70 2e66 6c69 7028 6e70 2e63 6f6e 6a28  np.flip(np.conj(
-00006e60: 6372 6170 5b31 3a28 4e66 6674 3229 5d29  crap[1:(Nfft2)])
-00006e70: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
-00006e80: 2020 735f 636f 7272 203d 206e 702e 7265    s_corr = np.re
-00006e90: 616c 286e 702e 6666 742e 6966 6674 7368  al(np.fft.ifftsh
-00006ea0: 6966 7428 7363 6970 792e 6666 7470 6163  ift(scipy.fftpac
-00006eb0: 6b2e 6966 6674 2863 7261 702c 204e 6666  k.ifft(crap, Nff
-00006ec0: 742c 2061 7869 733d 3029 2929 0a0a 2020  t, axis=0)))..  
-00006ed0: 2020 2320 7472 696d 2074 6865 2043 4346    # trim the CCF
-00006ee0: 7320 696e 205b 2d6d 6178 6c61 6720 6d61  s in [-maxlag ma
-00006ef0: 786c 6167 5d0a 2020 2020 7420 3d20 6e70  xlag].    t = np
-00006f00: 2e61 7261 6e67 6528 2d4e 6666 7432 202b  .arange(-Nfft2 +
-00006f10: 2031 2c20 4e66 6674 3229 202a 2064 740a   1, Nfft2) * dt.
-00006f20: 2020 2020 696e 6420 3d20 6e70 2e77 6865      ind = np.whe
-00006f30: 7265 286e 702e 6162 7328 7429 203c 3d20  re(np.abs(t) <= 
-00006f40: 6d61 786c 6167 295b 305d 0a20 2020 2069  maxlag)[0].    i
-00006f50: 6620 735f 636f 7272 2e6e 6469 6d20 3d3d  f s_corr.ndim ==
-00006f60: 2031 3a0a 2020 2020 2020 2020 735f 636f   1:.        s_co
-00006f70: 7272 203d 2073 5f63 6f72 725b 696e 645d  rr = s_corr[ind]
-00006f80: 0a20 2020 2065 6c69 6620 735f 636f 7272  .    elif s_corr
-00006f90: 2e6e 6469 6d20 3d3d 2032 3a0a 2020 2020  .ndim == 2:.    
-00006fa0: 2020 2020 735f 636f 7272 203d 2073 5f63      s_corr = s_c
-00006fb0: 6f72 725b 3a2c 2069 6e64 5d0a 2020 2020  orr[:, ind].    
-00006fc0: 7265 7475 726e 2073 5f63 6f72 722c 2074  return s_corr, t
-00006fd0: 5f63 6f72 722c 206e 5f63 6f72 720a 0a0a  _corr, n_corr...
-00006fe0: 6465 6620 636f 7272 656c 6174 655f 6e6f  def correlate_no
-00006ff0: 6e6c 696e 6561 725f 7374 6163 6b28 6666  nlinear_stack(ff
-00007000: 7431 5f73 6d6f 6f74 6865 645f 6162 732c  t1_smoothed_abs,
-00007010: 2066 6674 322c 2044 2c20 4e66 6674 2c20   fft2, D, Nfft, 
-00007020: 6461 7461 535f 7429 3a0a 2020 2020 2222  dataS_t):.    ""
-00007030: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
-00007040: 696f 6e20 646f 6573 2074 6865 2063 726f  ion does the cro
-00007050: 7373 2d63 6f72 7265 6c61 7469 6f6e 2069  ss-correlation i
-00007060: 6e20 6672 6571 2064 6f6d 6169 6e20 616e  n freq domain an
-00007070: 6420 6861 7320 7468 6520 6f70 7469 6f6e  d has the option
-00007080: 2074 6f20 6b65 6570 2073 7562 2d73 7461   to keep sub-sta
-00007090: 636b 7320 6f66 0a20 2020 2074 6865 2063  cks of.    the c
-000070a0: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
-000070b0: 2069 6620 6e65 6564 6564 2e20 6974 2074   if needed. it t
-000070c0: 616b 6573 2061 6476 616e 7461 6765 206f  akes advantage o
-000070d0: 6620 7468 6520 6c69 6e65 6172 2072 656c  f the linear rel
-000070e0: 6174 696f 6e73 6869 7020 6f66 2069 6666  ationship of iff
-000070f0: 742c 2073 6f20 7468 6174 0a20 2020 2073  t, so that.    s
-00007100: 7461 636b 696e 6720 6973 2070 6572 666f  tacking is perfo
-00007110: 726d 6564 2069 6e20 7370 6563 7472 756d  rmed in spectrum
-00007120: 2064 6f6d 6169 6e20 6669 7273 7420 746f   domain first to
-00007130: 2072 6564 7563 6520 7468 6520 746f 7461   reduce the tota
-00007140: 6c20 6e75 6d62 6572 206f 6620 6966 6674  l number of ifft
-00007150: 2e20 2875 7365 6420 696e 2053 3129 0a20  . (used in S1). 
-00007160: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-00007170: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00007180: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 6674  --------.    fft
-00007190: 315f 736d 6f6f 7468 6564 5f61 6273 3a20  1_smoothed_abs: 
-000071a0: 736d 6f6f 7468 6564 2070 6f77 6572 2073  smoothed power s
-000071b0: 7065 6374 7261 6c20 6465 6e73 6974 7920  pectral density 
-000071c0: 6f66 2074 6865 2046 4654 2066 6f72 2074  of the FFT for t
-000071d0: 6865 2073 6f75 7263 6520 7374 6174 696f  he source statio
-000071e0: 6e0a 2020 2020 6666 7432 3a20 7261 7720  n.    fft2: raw 
-000071f0: 4646 5420 7370 6563 7472 756d 206f 6620  FFT spectrum of 
-00007200: 7468 6520 7265 6365 6976 6572 2073 7461  the receiver sta
-00007210: 7469 6f6e 0a20 2020 2044 3a20 6469 6374  tion.    D: dict
-00007220: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-00007230: 6720 666f 6c6c 6f77 696e 6720 7061 7261  g following para
-00007240: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-00007250: 6d61 786c 6167 3a20 206d 6178 696d 756d  maxlag:  maximum
-00007260: 206c 6167 7320 746f 206b 6565 7020 696e   lags to keep in
-00007270: 2074 6865 2063 726f 7373 2063 6f72 7265   the cross corre
-00007280: 6c61 7469 6f6e 0a20 2020 2020 2020 2064  lation.        d
-00007290: 743a 2020 2020 2020 7361 6d70 6c69 6e67  t:      sampling
-000072a0: 2072 6174 6520 2869 6e20 7329 0a20 2020   rate (in s).   
-000072b0: 2020 2020 206e 7769 6e3a 2020 2020 6e75       nwin:    nu
-000072c0: 6d62 6572 206f 6620 7365 676d 656e 7473  mber of segments
-000072d0: 2069 6e20 7468 6520 3244 206d 6174 7269   in the 2D matri
-000072e0: 780a 2020 2020 2020 2020 6d65 7468 6f64  x.        method
-000072f0: 3a20 2063 726f 7373 2d63 6f72 7265 6c61  :  cross-correla
-00007300: 7469 6f6e 206d 6574 686f 6473 2073 656c  tion methods sel
-00007310: 6563 7465 6420 6279 2074 6865 2075 7365  ected by the use
-00007320: 720a 2020 2020 2020 2020 6672 6571 6d69  r.        freqmi
-00007330: 6e3a 206d 696e 696d 756d 2066 7265 7175  n: minimum frequ
-00007340: 656e 6379 2028 487a 290a 2020 2020 2020  ency (Hz).      
-00007350: 2020 6672 6571 6d61 783a 206d 6178 696d    freqmax: maxim
-00007360: 756d 2066 7265 7175 656e 6379 2028 487a  um frequency (Hz
-00007370: 290a 2020 2020 4e66 6674 3a20 2020 206e  ).    Nfft:    n
-00007380: 756d 6265 7220 6f66 2066 7265 7175 656e  umber of frequen
-00007390: 6379 2070 6f69 6e74 7320 666f 7220 6966  cy points for if
-000073a0: 6674 0a20 2020 2064 6174 6153 5f74 3a20  ft.    dataS_t: 
-000073b0: 6d61 7472 6978 206f 6620 6461 7465 7469  matrix of dateti
-000073c0: 6d65 206f 626a 6563 742e 0a20 2020 2052  me object..    R
-000073d0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-000073e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000073f0: 2d0a 2020 2020 735f 636f 7272 3a20 3144  -.    s_corr: 1D
-00007400: 206f 7220 3244 206d 6174 7269 7820 6f66   or 2D matrix of
-00007410: 2074 6865 2061 7665 7261 6765 6420 6f72   the averaged or
-00007420: 2073 7562 2d73 7461 636b 7320 6f66 2063   sub-stacks of c
-00007430: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
-00007440: 2066 756e 6374 696f 6e73 2069 6e20 7469   functions in ti
-00007450: 6d65 2064 6f6d 6169 6e0a 2020 2020 745f  me domain.    t_
-00007460: 636f 7272 3a20 7469 6d65 7374 616d 7020  corr: timestamp 
-00007470: 666f 7220 6561 6368 2073 7562 2d73 7461  for each sub-sta
-00007480: 636b 206f 7220 6176 6572 6167 6564 2066  ck or averaged f
-00007490: 756e 6374 696f 6e0a 2020 2020 6e5f 636f  unction.    n_co
-000074a0: 7272 3a20 6e75 6d62 6572 206f 6620 696e  rr: number of in
-000074b0: 636c 7564 6564 2073 6567 6d65 6e74 7320  cluded segments 
-000074c0: 666f 7220 6561 6368 2073 7562 2d73 7461  for each sub-sta
-000074d0: 636b 206f 7220 6176 6572 6167 6564 2066  ck or averaged f
-000074e0: 756e 6374 696f 6e0a 2020 2020 2222 220a  unction.    """.
-000074f0: 2020 2020 2320 2d2d 2d2d 6c6f 6164 2070      # ----load p
-00007500: 6172 616d 7465 7273 2d2d 2d2d 0a20 2020  aramters----.   
-00007510: 2064 7420 3d20 445b 2264 7422 5d0a 2020   dt = D["dt"].  
-00007520: 2020 6d61 786c 6167 203d 2044 5b22 6d61    maxlag = D["ma
-00007530: 786c 6167 225d 0a20 2020 206d 6574 686f  xlag"].    metho
-00007540: 6420 3d20 445b 2263 635f 6d65 7468 6f64  d = D["cc_method
-00007550: 225d 0a20 2020 2063 635f 6c65 6e20 3d20  "].    cc_len = 
-00007560: 445b 2263 635f 6c65 6e22 5d0a 2020 2020  D["cc_len"].    
-00007570: 7375 6273 7461 636b 203d 2044 5b22 7375  substack = D["su
-00007580: 6273 7461 636b 225d 0a20 2020 2073 7461  bstack"].    sta
-00007590: 636b 5f6d 6574 686f 6420 3d20 445b 2273  ck_method = D["s
-000075a0: 7461 636b 5f6d 6574 686f 6422 5d0a 2020  tack_method"].  
-000075b0: 2020 7375 6273 7461 636b 5f6c 656e 203d    substack_len =
-000075c0: 2044 5b22 7375 6273 7461 636b 5f6c 656e   D["substack_len
-000075d0: 225d 0a20 2020 2073 6d6f 6f74 6873 7065  "].    smoothspe
-000075e0: 6374 5f4e 203d 2044 5b22 736d 6f6f 7468  ct_N = D["smooth
-000075f0: 7370 6563 745f 4e22 5d0a 0a20 2020 206e  spect_N"]..    n
-00007600: 7769 6e20 3d20 6666 7431 5f73 6d6f 6f74  win = fft1_smoot
-00007610: 6865 645f 6162 732e 7368 6170 655b 305d  hed_abs.shape[0]
-00007620: 0a20 2020 204e 6666 7432 203d 2066 6674  .    Nfft2 = fft
-00007630: 315f 736d 6f6f 7468 6564 5f61 6273 2e73  1_smoothed_abs.s
-00007640: 6861 7065 5b31 5d0a 0a20 2020 2023 202d  hape[1]..    # -
-00007650: 2d2d 2d2d 2d63 6f6e 7665 7274 2061 6c6c  -----convert all
-00007660: 2032 4420 6172 7261 7973 2069 6e74 6f20   2D arrays into 
-00007670: 3144 2074 6f20 7370 6565 6420 7570 2d2d  1D to speed up--
-00007680: 2d2d 2d2d 2d2d 0a20 2020 2063 6f72 7220  ------.    corr 
-00007690: 3d20 6e70 2e7a 6572 6f73 286e 7769 6e20  = np.zeros(nwin 
-000076a0: 2a20 4e66 6674 322c 2064 7479 7065 3d6e  * Nfft2, dtype=n
-000076b0: 702e 636f 6d70 6c65 7836 3429 0a20 2020  p.complex64).   
-000076c0: 2063 6f72 7220 3d20 6666 7431 5f73 6d6f   corr = fft1_smo
-000076d0: 6f74 6865 645f 6162 732e 7265 7368 6170  othed_abs.reshap
-000076e0: 6528 0a20 2020 2020 2020 2066 6674 315f  e(.        fft1_
-000076f0: 736d 6f6f 7468 6564 5f61 6273 2e73 697a  smoothed_abs.siz
-00007700: 652c 0a20 2020 2029 202a 2066 6674 322e  e,.    ) * fft2.
-00007710: 7265 7368 6170 6528 0a20 2020 2020 2020  reshape(.       
-00007720: 2066 6674 322e 7369 7a65 2c0a 2020 2020   fft2.size,.    
-00007730: 290a 0a20 2020 2023 206e 6f72 6d61 6c69  )..    # normali
-00007740: 7a65 2062 7920 7265 6365 6976 6572 2073  ze by receiver s
-00007750: 7065 6374 7261 6c20 666f 7220 636f 6865  pectral for cohe
-00007760: 7265 6e63 790a 2020 2020 6966 206d 6574  rency.    if met
-00007770: 686f 6420 3d3d 2022 636f 6865 7265 6e63  hod == "coherenc
-00007780: 7922 3a0a 2020 2020 2020 2020 7465 6d70  y":.        temp
-00007790: 203d 206d 6f76 696e 675f 6176 6528 0a20   = moving_ave(. 
-000077a0: 2020 2020 2020 2020 2020 206e 702e 6162             np.ab
-000077b0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-000077c0: 2020 2066 6674 322e 7265 7368 6170 6528     fft2.reshape(
-000077d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000077e0: 2020 2020 2066 6674 322e 7369 7a65 2c0a       fft2.size,.
-000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007800: 290a 2020 2020 2020 2020 2020 2020 292c  ).            ),
-00007810: 0a20 2020 2020 2020 2020 2020 2073 6d6f  .            smo
-00007820: 6f74 6873 7065 6374 5f4e 2c0a 2020 2020  othspect_N,.    
-00007830: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-00007840: 7272 202f 3d20 7465 6d70 0a20 2020 2063  rr /= temp.    c
-00007850: 6f72 7220 3d20 636f 7272 2e72 6573 6861  orr = corr.resha
-00007860: 7065 286e 7769 6e2c 204e 6666 7432 290a  pe(nwin, Nfft2).
-00007870: 0a20 2020 2023 2074 7261 6e73 666f 726d  .    # transform
-00007880: 2062 6163 6b20 746f 2074 696d 6520 646f   back to time do
-00007890: 6d61 696e 2077 6176 6566 6f72 6d73 0a20  main waveforms. 
-000078a0: 2020 2073 5f63 6f72 7220 3d20 6e70 2e7a     s_corr = np.z
-000078b0: 6572 6f73 2873 6861 7065 3d28 6e77 696e  eros(shape=(nwin
-000078c0: 2c20 4e66 6674 292c 2064 7479 7065 3d6e  , Nfft), dtype=n
-000078d0: 702e 666c 6f61 7433 3229 2020 2320 7374  p.float32)  # st
-000078e0: 6163 6b65 6420 636f 7272 656c 6174 696f  acked correlatio
-000078f0: 6e0a 2020 2020 616d 706d 6178 203d 206e  n.    ampmax = n
-00007900: 702e 7a65 726f 7328 6e77 696e 2c20 6474  p.zeros(nwin, dt
-00007910: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-00007920: 2020 2020 6e5f 636f 7272 203d 206e 702e      n_corr = np.
-00007930: 7a65 726f 7328 6e77 696e 2c20 6474 7970  zeros(nwin, dtyp
-00007940: 653d 6e70 2e69 6e74 3136 2920 2023 206e  e=np.int16)  # n
-00007950: 756d 6265 7220 6f66 2063 6f72 7265 6c61  umber of correla
-00007960: 7469 6f6e 7320 666f 7220 6561 6368 2073  tions for each s
-00007970: 7562 7374 6163 6b0a 2020 2020 745f 636f  ubstack.    t_co
-00007980: 7272 203d 2064 6174 6153 5f74 2020 2320  rr = dataS_t  # 
-00007990: 7469 6d65 7374 616d 700a 2020 2020 6372  timestamp.    cr
-000079a0: 6170 203d 206e 702e 7a65 726f 7328 4e66  ap = np.zeros(Nf
-000079b0: 6674 2c20 6474 7970 653d 6e70 2e63 6f6d  ft, dtype=np.com
-000079c0: 706c 6578 3634 290a 2020 2020 666f 7220  plex64).    for 
-000079d0: 6920 696e 2072 616e 6765 286e 7769 6e29  i in range(nwin)
-000079e0: 3a0a 2020 2020 2020 2020 6e5f 636f 7272  :.        n_corr
-000079f0: 5b69 5d20 3d20 310a 2020 2020 2020 2020  [i] = 1.        
-00007a00: 6372 6170 5b3a 4e66 6674 325d 203d 2063  crap[:Nfft2] = c
-00007a10: 6f72 725b 692c 203a 5d0a 2020 2020 2020  orr[i, :].      
-00007a20: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
-00007a30: 2063 7261 705b 3a4e 6666 7432 5d20 2d20   crap[:Nfft2] - 
-00007a40: 6e70 2e6d 6561 6e28 6372 6170 5b3a 4e66  np.mean(crap[:Nf
-00007a50: 6674 325d 2920 2023 2072 656d 6f76 6520  ft2])  # remove 
-00007a60: 7468 6520 6d65 616e 2069 6e20 6672 6571  the mean in freq
-00007a70: 2064 6f6d 6169 6e20 2873 7069 6b65 2061   domain (spike a
-00007a80: 7420 743d 3029 0a20 2020 2020 2020 2063  t t=0).        c
-00007a90: 7261 705b 2d28 4e66 6674 3229 202b 2031  rap[-(Nfft2) + 1
-00007aa0: 203a 5d20 3d20 6e70 2e66 6c69 7028 6e70   :] = np.flip(np
-00007ab0: 2e63 6f6e 6a28 6372 6170 5b31 3a28 4e66  .conj(crap[1:(Nf
-00007ac0: 6674 3229 5d29 2c20 6178 6973 3d30 290a  ft2)]), axis=0).
-00007ad0: 2020 2020 2020 2020 6372 6170 5b30 5d20          crap[0] 
-00007ae0: 3d20 636f 6d70 6c65 7828 302c 2030 290a  = complex(0, 0).
-00007af0: 2020 2020 2020 2020 735f 636f 7272 5b69          s_corr[i
-00007b00: 2c20 3a5d 203d 206e 702e 7265 616c 286e  , :] = np.real(n
-00007b10: 702e 6666 742e 6966 6674 7368 6966 7428  p.fft.ifftshift(
-00007b20: 7363 6970 792e 6666 7470 6163 6b2e 6966  scipy.fftpack.if
-00007b30: 6674 2863 7261 702c 204e 6666 742c 2061  ft(crap, Nfft, a
-00007b40: 7869 733d 3029 2929 0a0a 2020 2020 6e73  xis=0)))..    ns
-00007b50: 5f63 6f72 7220 3d20 735f 636f 7272 0a20  _corr = s_corr. 
-00007b60: 2020 2066 6f72 2069 6969 2069 6e20 7261     for iii in ra
-00007b70: 6e67 6528 6e73 5f63 6f72 722e 7368 6170  nge(ns_corr.shap
-00007b80: 655b 305d 293a 0a20 2020 2020 2020 206e  e[0]):.        n
-00007b90: 735f 636f 7272 5b69 6969 5d20 2f3d 206e  s_corr[iii] /= n
-00007ba0: 702e 6d61 7828 6e70 2e61 6273 286e 735f  p.max(np.abs(ns_
-00007bb0: 636f 7272 5b69 6969 5d29 290a 0a20 2020  corr[iii]))..   
-00007bc0: 2069 6620 7375 6273 7461 636b 3a0a 2020   if substack:.  
-00007bd0: 2020 2020 2020 6966 2073 7562 7374 6163        if substac
-00007be0: 6b5f 6c65 6e20 3d3d 2063 635f 6c65 6e3a  k_len == cc_len:
-00007bf0: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-00007c00: 656d 6f76 6520 6162 6e6f 726d 616c 2064  emove abnormal d
-00007c10: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-00007c20: 616d 706d 6178 203d 206e 702e 6d61 7828  ampmax = np.max(
-00007c30: 735f 636f 7272 2c20 6178 6973 3d31 290a  s_corr, axis=1).
-00007c40: 2020 2020 2020 2020 2020 2020 7469 6e64              tind
-00007c50: 7820 3d20 6e70 2e77 6865 7265 2828 616d  x = np.where((am
-00007c60: 706d 6178 203c 2032 3020 2a20 6e70 2e6d  pmax < 20 * np.m
-00007c70: 6564 6961 6e28 616d 706d 6178 2929 2026  edian(ampmax)) &
-00007c80: 2028 616d 706d 6178 203e 2030 2929 5b30   (ampmax > 0))[0
-00007c90: 5d0a 2020 2020 2020 2020 2020 2020 735f  ].            s_
-00007ca0: 636f 7272 203d 2073 5f63 6f72 725b 7469  corr = s_corr[ti
-00007cb0: 6e64 782c 203a 5d0a 2020 2020 2020 2020  ndx, :].        
-00007cc0: 2020 2020 745f 636f 7272 203d 2074 5f63      t_corr = t_c
-00007cd0: 6f72 725b 7469 6e64 785d 0a20 2020 2020  orr[tindx].     
-00007ce0: 2020 2020 2020 206e 5f63 6f72 7220 3d20         n_corr = 
-00007cf0: 6e5f 636f 7272 5b74 696e 6478 5d0a 0a20  n_corr[tindx].. 
-00007d00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007d10: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
-00007d20: 696d 6520 696e 666f 726d 6174 696f 6e0a  ime information.
-00007d30: 2020 2020 2020 2020 2020 2020 5474 6f74              Ttot
-00007d40: 616c 203d 2064 6174 6153 5f74 5b2d 315d  al = dataS_t[-1]
-00007d50: 202d 2064 6174 6153 5f74 5b30 5d20 2023   - dataS_t[0]  #
-00007d60: 2074 6f74 616c 2064 7572 6174 696f 6e20   total duration 
-00007d70: 6f66 2077 6861 7420 7765 2068 6176 6520  of what we have 
-00007d80: 6e6f 770a 2020 2020 2020 2020 2020 2020  now.            
-00007d90: 7473 7461 7274 203d 2064 6174 6153 5f74  tstart = dataS_t
-00007da0: 5b30 5d0a 0a20 2020 2020 2020 2020 2020  [0]..           
-00007db0: 206e 7374 6163 6b20 3d20 696e 7428 6e70   nstack = int(np
-00007dc0: 2e72 6f75 6e64 2854 746f 7461 6c20 2f20  .round(Ttotal / 
-00007dd0: 7375 6273 7461 636b 5f6c 656e 2929 0a20  substack_len)). 
-00007de0: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
-00007df0: 7820 3d20 6e70 2e7a 6572 6f73 286e 7374  x = np.zeros(nst
-00007e00: 6163 6b2c 2064 7479 7065 3d6e 702e 666c  ack, dtype=np.fl
-00007e10: 6f61 7433 3229 0a20 2020 2020 2020 2020  oat32).         
-00007e20: 2020 2073 5f63 6f72 7220 3d20 6e70 2e7a     s_corr = np.z
-00007e30: 6572 6f73 2873 6861 7065 3d28 6e73 7461  eros(shape=(nsta
-00007e40: 636b 2c20 4e66 6674 292c 2064 7479 7065  ck, Nfft), dtype
-00007e50: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
-00007e60: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
-00007e70: 3d20 6e70 2e7a 6572 6f73 286e 7374 6163  = np.zeros(nstac
-00007e80: 6b2c 2064 7479 7065 3d6e 702e 696e 7429  k, dtype=np.int)
-00007e90: 0a20 2020 2020 2020 2020 2020 2074 5f63  .            t_c
-00007ea0: 6f72 7220 3d20 6e70 2e7a 6572 6f73 286e  orr = np.zeros(n
-00007eb0: 7374 6163 6b2c 2064 7479 7065 3d6e 702e  stack, dtype=np.
-00007ec0: 666c 6f61 7429 0a20 2020 2020 2020 2020  float).         
-00007ed0: 2020 2063 7261 7020 3d20 6e70 2e7a 6572     crap = np.zer
-00007ee0: 6f73 284e 6666 742c 2064 7479 7065 3d6e  os(Nfft, dtype=n
-00007ef0: 702e 636f 6d70 6c65 7836 3429 0a0a 2020  p.complex64)..  
-00007f00: 2020 2020 2020 2020 2020 666f 7220 6973            for is
-00007f10: 7461 636b 2069 6e20 7261 6e67 6528 6e73  tack in range(ns
-00007f20: 7461 636b 293a 0a20 2020 2020 2020 2020  tack):.         
-00007f30: 2020 2020 2020 2023 2066 696e 6420 7468         # find th
-00007f40: 6520 696e 6465 7865 7320 6f66 2061 6c6c  e indexes of all
-00007f50: 206f 6620 7468 6520 7769 6e64 6f77 7320   of the windows 
-00007f60: 7468 6174 2073 7461 7274 206f 7220 656e  that start or en
-00007f70: 6420 7769 7468 696e 0a20 2020 2020 2020  d within.       
-00007f80: 2020 2020 2020 2020 2069 7469 6d65 203d           itime =
-00007f90: 206e 702e 7768 6572 6528 2864 6174 6153   np.where((dataS
-00007fa0: 5f74 203e 3d20 7473 7461 7274 2920 2620  _t >= tstart) & 
-00007fb0: 2864 6174 6153 5f74 203c 2074 7374 6172  (dataS_t < tstar
-00007fc0: 7420 2b20 7375 6273 7461 636b 5f6c 656e  t + substack_len
-00007fd0: 2929 5b30 5d0a 2020 2020 2020 2020 2020  ))[0].          
-00007fe0: 2020 2020 2020 6966 206c 656e 2869 7469        if len(iti
-00007ff0: 6d65 2920 3d3d 2030 3a0a 2020 2020 2020  me) == 0:.      
-00008000: 2020 2020 2020 2020 2020 2020 2020 7473                ts
-00008010: 7461 7274 202b 3d20 7375 6273 7461 636b  tart += substack
-00008020: 5f6c 656e 0a20 2020 2020 2020 2020 2020  _len.           
-00008030: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00008040: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-00008050: 2020 2063 7261 705b 3a4e 6666 7432 5d20     crap[:Nfft2] 
-00008060: 3d20 6e70 2e6d 6561 6e28 636f 7272 5b69  = np.mean(corr[i
-00008070: 7469 6d65 2c20 3a5d 2c20 6178 6973 3d30  time, :], axis=0
-00008080: 2920 2023 206c 696e 6561 7220 6176 6572  )  # linear aver
-00008090: 6167 6520 6f66 2074 6865 2063 6f72 7265  age of the corre
-000080a0: 6c61 7469 6f6e 0a20 2020 2020 2020 2020  lation.         
-000080b0: 2020 2020 2020 2063 7261 705b 3a4e 6666         crap[:Nff
-000080c0: 7432 5d20 3d20 6372 6170 5b3a 4e66 6674  t2] = crap[:Nfft
-000080d0: 325d 202d 206e 702e 6d65 616e 2863 7261  2] - np.mean(cra
-000080e0: 705b 3a4e 6666 7432 5d29 2020 2320 7265  p[:Nfft2])  # re
-000080f0: 6d6f 7665 2074 6865 206d 6561 6e20 696e  move the mean in
-00008100: 2066 7265 7120 646f 6d61 696e 2028 7370   freq domain (sp
-00008110: 696b 6520 6174 2074 3d30 290a 2020 2020  ike at t=0).    
-00008120: 2020 2020 2020 2020 2020 2020 6372 6170              crap
-00008130: 5b2d 284e 6666 7432 2920 2b20 3120 3a5d  [-(Nfft2) + 1 :]
-00008140: 203d 206e 702e 666c 6970 286e 702e 636f   = np.flip(np.co
-00008150: 6e6a 2863 7261 705b 313a 284e 6666 7432  nj(crap[1:(Nfft2
-00008160: 295d 292c 2061 7869 733d 3029 0a20 2020  )]), axis=0).   
-00008170: 2020 2020 2020 2020 2020 2020 2063 7261               cra
-00008180: 705b 305d 203d 2063 6f6d 706c 6578 2830  p[0] = complex(0
-00008190: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
-000081a0: 2020 2020 2073 5f63 6f72 725b 6973 7461       s_corr[ista
-000081b0: 636b 2c20 3a5d 203d 206e 702e 7265 616c  ck, :] = np.real
-000081c0: 286e 702e 6666 742e 6966 6674 7368 6966  (np.fft.ifftshif
-000081d0: 7428 7363 6970 792e 6666 7470 6163 6b2e  t(scipy.fftpack.
-000081e0: 6966 6674 2863 7261 702c 204e 6666 742c  ifft(crap, Nfft,
-000081f0: 2061 7869 733d 3029 2929 0a20 2020 2020   axis=0))).     
-00008200: 2020 2020 2020 2020 2020 206e 5f63 6f72             n_cor
-00008210: 725b 6973 7461 636b 5d20 3d20 6c65 6e28  r[istack] = len(
-00008220: 6974 696d 6529 2020 2320 6e75 6d62 6572  itime)  # number
-00008230: 206f 6620 7769 6e64 6f77 7320 7374 6163   of windows stac
-00008240: 6b73 0a20 2020 2020 2020 2020 2020 2020  ks.             
-00008250: 2020 2074 5f63 6f72 725b 6973 7461 636b     t_corr[istack
-00008260: 5d20 3d20 7473 7461 7274 2020 2320 7361  ] = tstart  # sa
-00008270: 7665 2074 6865 2074 696d 6520 7374 616d  ve the time stam
-00008280: 7073 0a20 2020 2020 2020 2020 2020 2020  ps.             
-00008290: 2020 2074 7374 6172 7420 2b3d 2073 7562     tstart += sub
-000082a0: 7374 6163 6b5f 6c65 6e0a 2020 2020 2020  stack_len.      
-000082b0: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
-000082c0: 7428 2763 6f72 7265 6c61 7469 6f6e 2064  t('correlation d
-000082d0: 6f6e 6520 616e 6420 7374 6163 6b65 6420  one and stacked 
-000082e0: 6174 2074 696d 6520 2573 2720 2520 7374  at time %s' % st
-000082f0: 7228 745f 636f 7272 5b69 7374 6163 6b5d  r(t_corr[istack]
-00008300: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-00008310: 2320 7265 6d6f 7665 2061 626e 6f72 6d61  # remove abnorma
-00008320: 6c20 6461 7461 0a20 2020 2020 2020 2020  l data.         
-00008330: 2020 2061 6d70 6d61 7820 3d20 6e70 2e6d     ampmax = np.m
-00008340: 6178 2873 5f63 6f72 722c 2061 7869 733d  ax(s_corr, axis=
-00008350: 3129 0a20 2020 2020 2020 2020 2020 2074  1).            t
-00008360: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
-00008370: 2861 6d70 6d61 7820 3c20 3230 202a 206e  (ampmax < 20 * n
-00008380: 702e 6d65 6469 616e 2861 6d70 6d61 7829  p.median(ampmax)
-00008390: 2920 2620 2861 6d70 6d61 7820 3e20 3029  ) & (ampmax > 0)
-000083a0: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-000083b0: 2073 5f63 6f72 7220 3d20 735f 636f 7272   s_corr = s_corr
-000083c0: 5b74 696e 6478 2c20 3a5d 0a20 2020 2020  [tindx, :].     
-000083d0: 2020 2020 2020 2074 5f63 6f72 7220 3d20         t_corr = 
-000083e0: 745f 636f 7272 5b74 696e 6478 5d0a 2020  t_corr[tindx].  
-000083f0: 2020 2020 2020 2020 2020 6e5f 636f 7272            n_corr
-00008400: 203d 206e 5f63 6f72 725b 7469 6e64 785d   = n_corr[tindx]
-00008410: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
-00008420: 2020 2020 2320 6176 6572 6167 6520 6461      # average da
-00008430: 696c 7920 6372 6f73 7320 636f 7272 656c  ily cross correl
-00008440: 6174 696f 6e20 6675 6e63 7469 6f6e 730a  ation functions.
-00008450: 2020 2020 2020 2020 6966 2073 7461 636b          if stack
-00008460: 5f6d 6574 686f 6420 3d3d 2053 7461 636b  _method == Stack
-00008470: 4d65 7468 6f64 2e4c 494e 4541 523a 0a20  Method.LINEAR:. 
-00008480: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
-00008490: 7820 3d20 6e70 2e6d 6178 2873 5f63 6f72  x = np.max(s_cor
-000084a0: 722c 2061 7869 733d 3129 0a20 2020 2020  r, axis=1).     
-000084b0: 2020 2020 2020 2074 696e 6478 203d 206e         tindx = n
-000084c0: 702e 7768 6572 6528 2861 6d70 6d61 7820  p.where((ampmax 
-000084d0: 3c20 3230 202a 206e 702e 6d65 6469 616e  < 20 * np.median
-000084e0: 2861 6d70 6d61 7829 2920 2620 2861 6d70  (ampmax)) & (amp
-000084f0: 6d61 7820 3e20 3029 295b 305d 0a20 2020  max > 0))[0].   
-00008500: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
-00008510: 3d20 6e70 2e6d 6561 6e28 735f 636f 7272  = np.mean(s_corr
-00008520: 5b74 696e 6478 5d2c 2061 7869 733d 3029  [tindx], axis=0)
-00008530: 0a20 2020 2020 2020 2020 2020 2074 5f63  .            t_c
-00008540: 6f72 7220 3d20 6461 7461 535f 745b 305d  orr = dataS_t[0]
-00008550: 0a20 2020 2020 2020 2020 2020 206e 5f63  .            n_c
-00008560: 6f72 7220 3d20 6c65 6e28 7469 6e64 7829  orr = len(tindx)
-00008570: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
-00008580: 6163 6b5f 6d65 7468 6f64 203d 3d20 5374  ack_method == St
-00008590: 6163 6b4d 6574 686f 642e 524f 4255 5354  ackMethod.ROBUST
-000085a0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-000085b0: 6767 6572 2e69 6e66 6f28 2264 6f20 726f  gger.info("do ro
-000085c0: 6275 7374 2073 7562 7374 6163 6b69 6e67  bust substacking
-000085d0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-000085e0: 5f63 6f72 7220 3d20 726f 6275 7374 5f73  _corr = robust_s
-000085f0: 7461 636b 2873 5f63 6f72 722c 2030 2e30  tack(s_corr, 0.0
-00008600: 3031 290a 2020 2020 2020 2020 2020 2020  01).            
-00008610: 745f 636f 7272 203d 2064 6174 6153 5f74  t_corr = dataS_t
-00008620: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00008630: 6e5f 636f 7272 203d 206e 7769 6e0a 2020  n_corr = nwin.  
-00008640: 2020 2320 2065 6c69 6620 7374 6163 6b5f    #  elif stack_
-00008650: 6d65 7468 6f64 203d 3d20 2773 656c 6563  method == 'selec
-00008660: 7469 7665 273a 0a20 2020 2023 2020 2020  tive':.    #    
-00008670: 2020 7072 696e 7428 2764 6f20 7365 6c65    print('do sele
-00008680: 6374 6976 6520 7375 6273 7461 636b 696e  ctive substackin
-00008690: 6727 290a 2020 2020 2320 2020 2020 2073  g').    #      s
-000086a0: 5f63 6f72 7220 3d20 7365 6c65 6374 6976  _corr = selectiv
-000086b0: 655f 7374 6163 6b28 735f 636f 7272 2c30  e_stack(s_corr,0
-000086c0: 2e30 3031 290a 2020 2020 2320 2020 2020  .001).    #     
-000086d0: 2074 5f63 6f72 7220 3d20 6461 7461 535f   t_corr = dataS_
-000086e0: 745b 305d 0a20 2020 2023 2020 2020 2020  t[0].    #      
-000086f0: 6e5f 636f 7272 203d 206e 7769 6e0a 0a20  n_corr = nwin.. 
-00008700: 2020 2023 2074 7269 6d20 7468 6520 4343     # trim the CC
-00008710: 4673 2069 6e20 5b2d 6d61 786c 6167 206d  Fs in [-maxlag m
-00008720: 6178 6c61 675d 0a20 2020 2074 203d 206e  axlag].    t = n
-00008730: 702e 6172 616e 6765 282d 4e66 6674 3220  p.arange(-Nfft2 
-00008740: 2b20 312c 204e 6666 7432 2920 2a20 6474  + 1, Nfft2) * dt
-00008750: 0a20 2020 2069 6e64 203d 206e 702e 7768  .    ind = np.wh
-00008760: 6572 6528 6e70 2e61 6273 2874 2920 3c3d  ere(np.abs(t) <=
-00008770: 206d 6178 6c61 6729 5b30 5d0a 2020 2020   maxlag)[0].    
-00008780: 6966 2073 5f63 6f72 722e 6e64 696d 203d  if s_corr.ndim =
-00008790: 3d20 313a 0a20 2020 2020 2020 2073 5f63  = 1:.        s_c
-000087a0: 6f72 7220 3d20 735f 636f 7272 5b69 6e64  orr = s_corr[ind
-000087b0: 5d0a 2020 2020 656c 6966 2073 5f63 6f72  ].    elif s_cor
-000087c0: 722e 6e64 696d 203d 3d20 323a 0a20 2020  r.ndim == 2:.   
-000087d0: 2020 2020 2073 5f63 6f72 7220 3d20 735f       s_corr = s_
-000087e0: 636f 7272 5b3a 2c20 696e 645d 0a20 2020  corr[:, ind].   
-000087f0: 2072 6574 7572 6e20 735f 636f 7272 2c20   return s_corr, 
-00008800: 745f 636f 7272 2c20 6e5f 636f 7272 2c20  t_corr, n_corr, 
-00008810: 6e73 5f63 6f72 725b 3a2c 2069 6e64 5d0a  ns_corr[:, ind].
-00008820: 0a0a 6465 6620 6363 5f70 6172 616d 6574  ..def cc_paramet
-00008830: 6572 7328 6363 5f70 6172 612c 2063 6f6f  ers(cc_para, coo
-00008840: 722c 2074 636f 7272 2c20 6e63 6f72 722c  r, tcorr, ncorr,
-00008850: 2063 6f6d 7029 3a0a 2020 2020 2222 220a   comp):.    """.
-00008860: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-00008870: 6e20 6173 7365 6d62 6c65 7320 7468 6520  n assembles the 
-00008880: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
-00008890: 6865 2063 6320 6675 6e63 7469 6f6e 2c20  he cc function, 
-000088a0: 7768 6963 6820 6973 2075 7365 640a 2020  which is used.  
-000088b0: 2020 7768 656e 2077 7269 7469 6e67 2074    when writing t
-000088c0: 6865 6d20 696e 746f 2041 5344 4620 6669  hem into ASDF fi
-000088d0: 6c65 730a 2020 2020 5041 5241 4d45 5445  les.    PARAMETE
-000088e0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-000088f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00008900: 2020 6363 5f70 6172 613a 2064 6963 7420    cc_para: dict 
-00008910: 636f 6e74 6169 6e69 6e67 2070 6172 616d  containing param
-00008920: 6574 6572 7320 7573 6564 2069 6e20 7468  eters used in th
-00008930: 6520 6666 745f 6363 2073 7465 700a 2020  e fft_cc step.  
-00008940: 2020 636f 6f72 3a20 2020 2064 6963 7420    coor:    dict 
-00008950: 636f 6e74 6169 6e69 6e67 2063 6f6f 7264  containing coord
-00008960: 696e 6174 6573 2069 6e66 6f20 6f66 2074  inates info of t
-00008970: 6865 2073 6f75 7263 6520 616e 6420 7265  he source and re
-00008980: 6365 6976 6572 2073 7461 7469 6f6e 730a  ceiver stations.
-00008990: 2020 2020 7463 6f72 723a 2020 2074 696d      tcorr:   tim
-000089a0: 6573 7461 6d70 206d 6174 7269 780a 2020  estamp matrix.  
-000089b0: 2020 6e63 6f72 723a 2020 206d 6174 7269    ncorr:   matri
-000089c0: 7820 6f66 206e 756d 6265 7220 6f66 2067  x of number of g
-000089d0: 6f6f 6420 7365 676d 656e 7473 2066 6f72  ood segments for
-000089e0: 2065 6163 6820 7375 622d 7374 6163 6b2f   each sub-stack/
-000089f0: 6669 6e61 6c20 7374 6163 6b0a 2020 2020  final stack.    
-00008a00: 636f 6d70 3a20 2020 2032 2063 6861 7261  comp:    2 chara
-00008a10: 6374 6572 2073 7472 696e 6773 2066 6f72  cter strings for
-00008a20: 2074 6865 2063 726f 7373 2063 6f72 7265   the cross corre
-00008a30: 6c61 7469 6f6e 2063 6f6d 706f 6e65 6e74  lation component
-00008a40: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-00008a50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00008a60: 2d2d 2d2d 0a20 2020 2070 6172 616d 6574  ----.    paramet
-00008a70: 6572 733a 2064 6963 7420 636f 6e74 6169  ers: dict contai
-00008a80: 6e69 6e67 2061 626f 7665 2069 6e66 6f20  ning above info 
-00008a90: 7573 6564 2066 6f72 206c 6174 6572 2073  used for later s
-00008aa0: 7461 636b 696e 672f 706c 6f74 7469 6e67  tacking/plotting
-00008ab0: 0a20 2020 2022 2222 0a20 2020 206c 6174  .    """.    lat
-00008ac0: 5320 3d20 636f 6f72 5b22 6c61 7453 225d  S = coor["latS"]
-00008ad0: 0a20 2020 206c 6f6e 5320 3d20 636f 6f72  .    lonS = coor
-00008ae0: 5b22 6c6f 6e53 225d 0a20 2020 206c 6174  ["lonS"].    lat
-00008af0: 5220 3d20 636f 6f72 5b22 6c61 7452 225d  R = coor["latR"]
-00008b00: 0a20 2020 206c 6f6e 5220 3d20 636f 6f72  .    lonR = coor
-00008b10: 5b22 6c6f 6e52 225d 0a20 2020 2064 7420  ["lonR"].    dt 
-00008b20: 3d20 6363 5f70 6172 615b 2264 7422 5d0a  = cc_para["dt"].
-00008b30: 2020 2020 6d61 786c 6167 203d 2063 635f      maxlag = cc_
-00008b40: 7061 7261 5b22 6d61 786c 6167 225d 0a20  para["maxlag"]. 
-00008b50: 2020 2073 7562 7374 6163 6b20 3d20 6363     substack = cc
-00008b60: 5f70 6172 615b 2273 7562 7374 6163 6b22  _para["substack"
-00008b70: 5d0a 2020 2020 6363 5f6d 6574 686f 6420  ].    cc_method 
-00008b80: 3d20 6363 5f70 6172 615b 2263 635f 6d65  = cc_para["cc_me
-00008b90: 7468 6f64 225d 0a0a 2020 2020 6469 7374  thod"]..    dist
-00008ba0: 2c20 617a 692c 2062 617a 203d 206f 6273  , azi, baz = obs
-00008bb0: 7079 2e67 656f 6465 7469 6373 2e62 6173  py.geodetics.bas
-00008bc0: 652e 6770 7332 6469 7374 5f61 7a69 6d75  e.gps2dist_azimu
-00008bd0: 7468 286c 6174 532c 206c 6f6e 532c 206c  th(latS, lonS, l
-00008be0: 6174 522c 206c 6f6e 5229 0a20 2020 2070  atR, lonR).    p
-00008bf0: 6172 616d 6574 6572 7320 3d20 7b0a 2020  arameters = {.  
-00008c00: 2020 2020 2020 2264 7422 3a20 6474 2c0a        "dt": dt,.
-00008c10: 2020 2020 2020 2020 226d 6178 6c61 6722          "maxlag"
-00008c20: 3a20 696e 7428 6d61 786c 6167 292c 0a20  : int(maxlag),. 
-00008c30: 2020 2020 2020 2022 6469 7374 223a 206e         "dist": n
-00008c40: 702e 666c 6f61 7433 3228 6469 7374 202f  p.float32(dist /
-00008c50: 2031 3030 3029 2c0a 2020 2020 2020 2020   1000),.        
-00008c60: 2261 7a69 223a 206e 702e 666c 6f61 7433  "azi": np.float3
-00008c70: 3228 617a 6929 2c0a 2020 2020 2020 2020  2(azi),.        
-00008c80: 2262 617a 223a 206e 702e 666c 6f61 7433  "baz": np.float3
-00008c90: 3228 6261 7a29 2c0a 2020 2020 2020 2020  2(baz),.        
-00008ca0: 226c 6f6e 5322 3a20 6e70 2e66 6c6f 6174  "lonS": np.float
-00008cb0: 3332 286c 6f6e 5329 2c0a 2020 2020 2020  32(lonS),.      
-00008cc0: 2020 226c 6174 5322 3a20 6e70 2e66 6c6f    "latS": np.flo
-00008cd0: 6174 3332 286c 6174 5329 2c0a 2020 2020  at32(latS),.    
-00008ce0: 2020 2020 226c 6f6e 5222 3a20 6e70 2e66      "lonR": np.f
-00008cf0: 6c6f 6174 3332 286c 6f6e 5229 2c0a 2020  loat32(lonR),.  
-00008d00: 2020 2020 2020 226c 6174 5222 3a20 6e70        "latR": np
-00008d10: 2e66 6c6f 6174 3332 286c 6174 5229 2c0a  .float32(latR),.
-00008d20: 2020 2020 2020 2020 226e 676f 6f64 223a          "ngood":
-00008d30: 206e 636f 7272 2c0a 2020 2020 2020 2020   ncorr,.        
-00008d40: 2263 635f 6d65 7468 6f64 223a 2063 635f  "cc_method": cc_
-00008d50: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
-00008d60: 2274 696d 6522 3a20 7463 6f72 722c 0a20  "time": tcorr,. 
-00008d70: 2020 2020 2020 2022 7375 6273 7461 636b         "substack
-00008d80: 223a 2073 7562 7374 6163 6b2c 0a20 2020  ": substack,.   
-00008d90: 2020 2020 2022 636f 6d70 223a 2063 6f6d       "comp": com
-00008da0: 702c 0a20 2020 207d 0a20 2020 2072 6574  p,.    }.    ret
-00008db0: 7572 6e20 7061 7261 6d65 7465 7273 0a0a  urn parameters..
-00008dc0: 0a64 6566 2073 7461 636b 696e 6728 6363  .def stacking(cc
-00008dd0: 5f61 7272 6179 2c20 6363 5f74 696d 652c  _array, cc_time,
-00008de0: 2063 635f 6e67 6f6f 642c 2073 7461 636b   cc_ngood, stack
-00008df0: 5f70 6172 6129 3a0a 2020 2020 2222 220a  _para):.    """.
-00008e00: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-00008e10: 6e20 7374 6163 6b73 2074 6865 2063 726f  n stacks the cro
-00008e20: 7373 2063 6f72 7265 6c61 7469 6f6e 2064  ss correlation d
-00008e30: 6174 6120 6163 636f 7264 696e 6720 746f  ata according to
-00008e40: 2074 6865 2075 7365 722d 6465 6669 6e65   the user-define
-00008e50: 6420 7375 6273 7461 636b 5f6c 656e 2070  d substack_len p
-00008e60: 6172 616d 6574 6572 0a0a 2020 2020 5041  arameter..    PA
-00008e70: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
-00008e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008e90: 2d2d 2d2d 0a20 2020 2063 635f 6172 7261  ----.    cc_arra
-00008ea0: 793a 2032 4420 6e75 6d70 7920 666c 6f61  y: 2D numpy floa
-00008eb0: 7433 3220 6d61 7472 6978 2063 6f6e 7461  t32 matrix conta
-00008ec0: 696e 696e 6720 616c 6c20 7365 676d 656e  ining all segmen
-00008ed0: 7465 6420 6372 6f73 732d 636f 7272 656c  ted cross-correl
-00008ee0: 6174 696f 6e20 6461 7461 0a20 2020 2063  ation data.    c
-00008ef0: 635f 7469 6d65 3a20 2031 4420 6e75 6d70  c_time:  1D nump
-00008f00: 7920 6172 7261 7920 6f66 2074 696d 6573  y array of times
-00008f10: 7461 6d70 7320 666f 7220 6561 6368 2073  tamps for each s
-00008f20: 6567 6d65 6e74 206f 6620 6363 5f61 7272  egment of cc_arr
-00008f30: 6179 0a20 2020 2063 635f 6e67 6f6f 643a  ay.    cc_ngood:
-00008f40: 2031 4420 6e75 6d70 7920 696e 7431 3620   1D numpy int16 
-00008f50: 6d61 7472 6978 2073 686f 7769 6e67 2074  matrix showing t
-00008f60: 6865 206e 756d 6265 7220 6f66 2073 6567  he number of seg
-00008f70: 6d65 6e74 7320 666f 7220 6561 6368 2073  ments for each s
-00008f80: 7562 2d73 7461 636b 2061 6e64 2f6f 7220  ub-stack and/or 
-00008f90: 6675 6c6c 2073 7461 636b 0a20 2020 2073  full stack.    s
-00008fa0: 7461 636b 5f70 6172 613a 2061 2064 6963  tack_para: a dic
-00008fb0: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
-00008fc0: 2073 7461 636b 696e 6720 7061 7261 6d65   stacking parame
-00008fd0: 7465 7273 0a0a 2020 2020 5245 5455 524e  ters..    RETURN
-00008fe0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00008ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00009000: 2020 6363 5f61 7272 6179 2c20 6363 5f6e    cc_array, cc_n
-00009010: 676f 6f64 2c20 6363 5f74 696d 653a 2073  good, cc_time: s
-00009020: 616d 6520 746f 2074 6865 2069 6e70 7574  ame to the input
-00009030: 2070 6172 616d 6574 6572 7320 6275 7420   parameters but 
-00009040: 7769 7468 2061 626e 6f72 6d61 6c20 6372  with abnormal cr
-00009050: 6f73 732d 636f 7272 6561 6c74 696f 6e73  oss-correaltions
-00009060: 2072 656d 6f76 6564 0a20 2020 2061 6c6c   removed.    all
-00009070: 7374 6163 6b73 313a 2031 4420 6d61 7472  stacks1: 1D matr
-00009080: 6978 206f 6620 7374 6163 6b65 6420 6372  ix of stacked cr
-00009090: 6f73 732d 636f 7272 656c 6174 696f 6e20  oss-correlation 
-000090a0: 6675 6e63 7469 6f6e 7320 6f76 6572 2061  functions over a
-000090b0: 6c6c 2074 6865 2073 6567 6d65 6e74 730a  ll the segments.
-000090c0: 2020 2020 6e73 7461 636b 733a 2020 2020      nstacks:    
-000090d0: 6e75 6d62 6572 206f 6620 6f76 6572 616c  number of overal
-000090e0: 6c20 7365 676d 656e 7473 2066 6f72 2074  l segments for t
-000090f0: 6865 2066 696e 616c 2073 7461 636b 730a  he final stacks.
-00009100: 2020 2020 2222 220a 2020 2020 2320 6c6f      """.    # lo
-00009110: 6164 2075 7365 6675 6c20 7061 7261 6d65  ad useful parame
-00009120: 7465 7273 2066 726f 6d20 6469 6374 0a20  ters from dict. 
-00009130: 2020 2073 616d 705f 6672 6571 203d 2073     samp_freq = s
-00009140: 7461 636b 5f70 6172 615b 2273 616d 705f  tack_para["samp_
-00009150: 6672 6571 225d 0a20 2020 2073 6d65 7468  freq"].    smeth
-00009160: 6f64 203d 2073 7461 636b 5f70 6172 615b  od = stack_para[
-00009170: 2273 7461 636b 5f6d 6574 686f 6422 5d0a  "stack_method"].
-00009180: 2020 2020 6e70 7473 203d 2063 635f 6172      npts = cc_ar
-00009190: 7261 792e 7368 6170 655b 315d 0a0a 2020  ray.shape[1]..  
-000091a0: 2020 2320 7265 6d6f 7665 2061 626e 6f72    # remove abnor
-000091b0: 6d61 6c20 6461 7461 0a20 2020 2061 6d70  mal data.    amp
-000091c0: 6d61 7820 3d20 6e70 2e6d 6178 2863 635f  max = np.max(cc_
-000091d0: 6172 7261 792c 2061 7869 733d 3129 0a20  array, axis=1). 
-000091e0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
-000091f0: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
-00009200: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
-00009210: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
-00009220: 3e20 3029 295b 305d 0a20 2020 2069 6620  > 0))[0].    if 
-00009230: 6e6f 7420 6c65 6e28 7469 6e64 7829 3a0a  not len(tindx):.
-00009240: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
-00009250: 7331 203d 205b 5d0a 2020 2020 2020 2020  s1 = [].        
-00009260: 616c 6c73 7461 636b 7332 203d 205b 5d0a  allstacks2 = [].
-00009270: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
-00009280: 7333 203d 205b 5d0a 2020 2020 2020 2020  s3 = [].        
-00009290: 6e73 7461 636b 7320 3d20 300a 2020 2020  nstacks = 0.    
-000092a0: 2020 2020 6363 5f61 7272 6179 203d 205b      cc_array = [
-000092b0: 5d0a 2020 2020 2020 2020 6363 5f6e 676f  ].        cc_ngo
-000092c0: 6f64 203d 205b 5d0a 2020 2020 2020 2020  od = [].        
-000092d0: 6363 5f74 696d 6520 3d20 5b5d 0a20 2020  cc_time = [].   
-000092e0: 2020 2020 2072 6574 7572 6e20 6363 5f61       return cc_a
-000092f0: 7272 6179 2c20 6363 5f6e 676f 6f64 2c20  rray, cc_ngood, 
-00009300: 6363 5f74 696d 652c 2061 6c6c 7374 6163  cc_time, allstac
-00009310: 6b73 312c 2061 6c6c 7374 6163 6b73 322c  ks1, allstacks2,
-00009320: 2061 6c6c 7374 6163 6b73 332c 206e 7374   allstacks3, nst
-00009330: 6163 6b73 0a20 2020 2065 6c73 653a 0a20  acks.    else:. 
-00009340: 2020 2020 2020 2023 2072 656d 6f76 6520         # remove 
-00009350: 6f6e 6573 2077 6974 6820 6261 6420 616d  ones with bad am
-00009360: 706c 6974 7564 650a 2020 2020 2020 2020  plitude.        
-00009370: 6363 5f61 7272 6179 203d 2063 635f 6172  cc_array = cc_ar
-00009380: 7261 795b 7469 6e64 782c 203a 5d0a 2020  ray[tindx, :].  
-00009390: 2020 2020 2020 6363 5f74 696d 6520 3d20        cc_time = 
-000093a0: 6363 5f74 696d 655b 7469 6e64 785d 0a20  cc_time[tindx]. 
-000093b0: 2020 2020 2020 2063 635f 6e67 6f6f 6420         cc_ngood 
-000093c0: 3d20 6363 5f6e 676f 6f64 5b74 696e 6478  = cc_ngood[tindx
-000093d0: 5d0a 0a20 2020 2020 2020 2023 2064 6f20  ]..        # do 
-000093e0: 7374 6163 6b69 6e67 0a20 2020 2020 2020  stacking.       
-000093f0: 2061 6c6c 7374 6163 6b73 3120 3d20 6e70   allstacks1 = np
-00009400: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
-00009410: 7065 3d6e 702e 666c 6f61 7433 3229 0a20  pe=np.float32). 
-00009420: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
-00009430: 3220 3d20 6e70 2e7a 6572 6f73 286e 7074  2 = np.zeros(npt
-00009440: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-00009450: 7433 3229 0a20 2020 2020 2020 2061 6c6c  t32).        all
-00009460: 7374 6163 6b73 3320 3d20 6e70 2e7a 6572  stacks3 = np.zer
-00009470: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
-00009480: 702e 666c 6f61 7433 3229 0a0a 2020 2020  p.float32)..    
-00009490: 2020 2020 6966 2073 6d65 7468 6f64 203d      if smethod =
-000094a0: 3d20 5374 6163 6b4d 6574 686f 642e 4c49  = StackMethod.LI
-000094b0: 4e45 4152 3a0a 2020 2020 2020 2020 2020  NEAR:.          
-000094c0: 2020 616c 6c73 7461 636b 7331 203d 206e    allstacks1 = n
-000094d0: 702e 6d65 616e 2863 635f 6172 7261 792c  p.mean(cc_array,
-000094e0: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-000094f0: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
-00009500: 2053 7461 636b 4d65 7468 6f64 2e50 5753   StackMethod.PWS
-00009510: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
-00009520: 6c73 7461 636b 7331 203d 2070 7773 2863  lstacks1 = pws(c
-00009530: 635f 6172 7261 792c 2073 616d 705f 6672  c_array, samp_fr
-00009540: 6571 290a 2020 2020 2020 2020 656c 6966  eq).        elif
-00009550: 2073 6d65 7468 6f64 203d 3d20 5374 6163   smethod == Stac
-00009560: 6b4d 6574 686f 642e 524f 4255 5354 3a0a  kMethod.ROBUST:.
-00009570: 2020 2020 2020 2020 2020 2020 616c 6c73              alls
-00009580: 7461 636b 7331 2c20 772c 206e 7374 6570  tacks1, w, nstep
-00009590: 203d 2072 6f62 7573 745f 7374 6163 6b28   = robust_stack(
-000095a0: 6363 5f61 7272 6179 2c20 302e 3030 3129  cc_array, 0.001)
-000095b0: 0a20 2020 2020 2020 2065 6c69 6620 736d  .        elif sm
-000095c0: 6574 686f 6420 3d3d 2053 7461 636b 4d65  ethod == StackMe
-000095d0: 7468 6f64 2e41 5554 4f5f 434f 5641 5249  thod.AUTO_COVARI
-000095e0: 414e 4345 3a0a 2020 2020 2020 2020 2020  ANCE:.          
-000095f0: 2020 616c 6c73 7461 636b 7331 203d 2061    allstacks1 = a
-00009600: 6461 7074 6976 655f 6669 6c74 6572 2863  daptive_filter(c
-00009610: 635f 6172 7261 792c 2031 290a 2020 2020  c_array, 1).    
-00009620: 2020 2020 656c 6966 2073 6d65 7468 6f64      elif smethod
-00009630: 203d 3d20 5374 6163 6b4d 6574 686f 642e   == StackMethod.
-00009640: 4e52 4f4f 543a 0a20 2020 2020 2020 2020  NROOT:.         
-00009650: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
-00009660: 6e72 6f6f 745f 7374 6163 6b28 6363 5f61  nroot_stack(cc_a
-00009670: 7272 6179 2c20 3229 0a20 2020 2020 2020  rray, 2).       
-00009680: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
-00009690: 2053 7461 636b 4d65 7468 6f64 2e41 4c4c   StackMethod.ALL
-000096a0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
-000096b0: 6c73 7461 636b 7331 203d 206e 702e 6d65  lstacks1 = np.me
-000096c0: 616e 2863 635f 6172 7261 792c 2061 7869  an(cc_array, axi
-000096d0: 733d 3029 0a20 2020 2020 2020 2020 2020  s=0).           
-000096e0: 2061 6c6c 7374 6163 6b73 3220 3d20 7077   allstacks2 = pw
-000096f0: 7328 6363 5f61 7272 6179 2c20 7361 6d70  s(cc_array, samp
-00009700: 5f66 7265 7129 0a20 2020 2020 2020 2020  _freq).         
-00009710: 2020 2061 6c6c 7374 6163 6b73 332c 2077     allstacks3, w
-00009720: 2c20 6e73 7465 7020 3d20 726f 6275 7374  , nstep = robust
-00009730: 5f73 7461 636b 2863 635f 6172 7261 792c  _stack(cc_array,
-00009740: 2030 2e30 3031 290a 2020 2020 2020 2020   0.001).        
-00009750: 6e73 7461 636b 7320 3d20 6e70 2e73 756d  nstacks = np.sum
-00009760: 2863 635f 6e67 6f6f 6429 0a0a 2020 2020  (cc_ngood)..    
-00009770: 2320 676f 6f64 2074 6f20 7265 7475 726e  # good to return
-00009780: 0a20 2020 2072 6574 7572 6e20 6363 5f61  .    return cc_a
-00009790: 7272 6179 2c20 6363 5f6e 676f 6f64 2c20  rray, cc_ngood, 
-000097a0: 6363 5f74 696d 652c 2061 6c6c 7374 6163  cc_time, allstac
-000097b0: 6b73 312c 2061 6c6c 7374 6163 6b73 322c  ks1, allstacks2,
-000097c0: 2061 6c6c 7374 6163 6b73 332c 206e 7374   allstacks3, nst
-000097d0: 6163 6b73 0a0a 0a64 6566 2073 7461 636b  acks...def stack
-000097e0: 696e 675f 726d 6128 6363 5f61 7272 6179  ing_rma(cc_array
-000097f0: 2c20 6363 5f74 696d 652c 2063 635f 6e67  , cc_time, cc_ng
-00009800: 6f6f 642c 2073 7461 636b 5f70 6172 6129  ood, stack_para)
-00009810: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-00009820: 6973 2066 756e 6374 696f 6e20 7374 6163  is function stac
-00009830: 6b73 2074 6865 2063 726f 7373 2063 6f72  ks the cross cor
-00009840: 7265 6c61 7469 6f6e 2064 6174 6120 6163  relation data ac
-00009850: 636f 7264 696e 6720 746f 2074 6865 2075  cording to the u
-00009860: 7365 722d 6465 6669 6e65 6420 7375 6273  ser-defined subs
-00009870: 7461 636b 5f6c 656e 2070 6172 616d 6574  tack_len paramet
-00009880: 6572 0a20 2020 2050 4152 414d 4554 4552  er.    PARAMETER
-00009890: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-000098a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000098b0: 2020 6363 5f61 7272 6179 3a20 3244 206e    cc_array: 2D n
-000098c0: 756d 7079 2066 6c6f 6174 3332 206d 6174  umpy float32 mat
-000098d0: 7269 7820 636f 6e74 6169 6e69 6e67 2061  rix containing a
-000098e0: 6c6c 2073 6567 6d65 6e74 6564 2063 726f  ll segmented cro
-000098f0: 7373 2d63 6f72 7265 6c61 7469 6f6e 2064  ss-correlation d
-00009900: 6174 610a 2020 2020 6363 5f74 696d 653a  ata.    cc_time:
-00009910: 2020 3144 206e 756d 7079 2061 7272 6179    1D numpy array
-00009920: 206f 6620 7469 6d65 7374 616d 7073 2066   of timestamps f
-00009930: 6f72 2065 6163 6820 7365 676d 656e 7420  or each segment 
-00009940: 6f66 2063 635f 6172 7261 790a 2020 2020  of cc_array.    
-00009950: 6363 5f6e 676f 6f64 3a20 3144 206e 756d  cc_ngood: 1D num
-00009960: 7079 2069 6e74 3136 206d 6174 7269 7820  py int16 matrix 
-00009970: 7368 6f77 696e 6720 7468 6520 6e75 6d62  showing the numb
-00009980: 6572 206f 6620 7365 676d 656e 7473 2066  er of segments f
-00009990: 6f72 2065 6163 6820 7375 622d 7374 6163  or each sub-stac
-000099a0: 6b20 616e 642f 6f72 2066 756c 6c20 7374  k and/or full st
-000099b0: 6163 6b0a 2020 2020 7374 6163 6b5f 7061  ack.    stack_pa
-000099c0: 7261 3a20 6120 6469 6374 2063 6f6e 7461  ra: a dict conta
-000099d0: 696e 696e 6720 616c 6c20 7374 6163 6b69  ining all stacki
-000099e0: 6e67 2070 6172 616d 6574 6572 730a 2020  ng parameters.  
-000099f0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
-00009a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009a10: 2d2d 2d2d 2d0a 2020 2020 6363 5f61 7272  -----.    cc_arr
-00009a20: 6179 2c20 6363 5f6e 676f 6f64 2c20 6363  ay, cc_ngood, cc
-00009a30: 5f74 696d 653a 2073 616d 6520 746f 2074  _time: same to t
-00009a40: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
-00009a50: 6572 7320 6275 7420 7769 7468 2061 626e  ers but with abn
-00009a60: 6f72 6d61 6c20 6372 6f73 732d 636f 7272  ormal cross-corr
-00009a70: 6561 6c74 696f 6e73 2072 656d 6f76 6564  ealtions removed
-00009a80: 0a20 2020 2061 6c6c 7374 6163 6b73 313a  .    allstacks1:
-00009a90: 2031 4420 6d61 7472 6978 206f 6620 7374   1D matrix of st
-00009aa0: 6163 6b65 6420 6372 6f73 732d 636f 7272  acked cross-corr
-00009ab0: 656c 6174 696f 6e20 6675 6e63 7469 6f6e  elation function
-00009ac0: 7320 6f76 6572 2061 6c6c 2074 6865 2073  s over all the s
-00009ad0: 6567 6d65 6e74 730a 2020 2020 6e73 7461  egments.    nsta
-00009ae0: 636b 733a 2020 2020 6e75 6d62 6572 206f  cks:    number o
-00009af0: 6620 6f76 6572 616c 6c20 7365 676d 656e  f overall segmen
-00009b00: 7473 2066 6f72 2074 6865 2066 696e 616c  ts for the final
-00009b10: 2073 7461 636b 730a 2020 2020 2222 220a   stacks.    """.
-00009b20: 2020 2020 2320 6c6f 6164 2075 7365 6675      # load usefu
-00009b30: 6c20 7061 7261 6d65 7465 7273 2066 726f  l parameters fro
-00009b40: 6d20 6469 6374 0a20 2020 2073 616d 705f  m dict.    samp_
-00009b50: 6672 6571 203d 2073 7461 636b 5f70 6172  freq = stack_par
-00009b60: 615b 2273 616d 705f 6672 6571 225d 0a20  a["samp_freq"]. 
-00009b70: 2020 2073 6d65 7468 6f64 203d 2073 7461     smethod = sta
-00009b80: 636b 5f70 6172 615b 2273 7461 636b 5f6d  ck_para["stack_m
-00009b90: 6574 686f 6422 5d0a 2020 2020 726d 615f  ethod"].    rma_
-00009ba0: 7375 6273 7461 636b 203d 2073 7461 636b  substack = stack
-00009bb0: 5f70 6172 615b 2272 6d61 5f73 7562 7374  _para["rma_subst
-00009bc0: 6163 6b22 5d0a 2020 2020 726d 615f 7374  ack"].    rma_st
-00009bd0: 6570 203d 2073 7461 636b 5f70 6172 615b  ep = stack_para[
-00009be0: 2272 6d61 5f73 7465 7022 5d0a 2020 2020  "rma_step"].    
-00009bf0: 7374 6172 745f 6461 7465 203d 2073 7461  start_date = sta
-00009c00: 636b 5f70 6172 615b 2273 7461 7274 5f64  ck_para["start_d
-00009c10: 6174 6522 5d0a 2020 2020 656e 645f 6461  ate"].    end_da
-00009c20: 7465 203d 2073 7461 636b 5f70 6172 615b  te = stack_para[
-00009c30: 2265 6e64 5f64 6174 6522 5d0a 2020 2020  "end_date"].    
-00009c40: 6e70 7473 203d 2063 635f 6172 7261 792e  npts = cc_array.
-00009c50: 7368 6170 655b 315d 0a0a 2020 2020 2320  shape[1]..    # 
-00009c60: 7265 6d6f 7665 2061 626e 6f72 6d61 6c20  remove abnormal 
-00009c70: 6461 7461 0a20 2020 2061 6d70 6d61 7820  data.    ampmax 
-00009c80: 3d20 6e70 2e6d 6178 2863 635f 6172 7261  = np.max(cc_arra
-00009c90: 792c 2061 7869 733d 3129 0a20 2020 2074  y, axis=1).    t
-00009ca0: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
-00009cb0: 2861 6d70 6d61 7820 3c20 3230 202a 206e  (ampmax < 20 * n
-00009cc0: 702e 6d65 6469 616e 2861 6d70 6d61 7829  p.median(ampmax)
-00009cd0: 2920 2620 2861 6d70 6d61 7820 3e20 3029  ) & (ampmax > 0)
-00009ce0: 295b 305d 0a20 2020 2069 6620 6e6f 7420  )[0].    if not 
-00009cf0: 6c65 6e28 7469 6e64 7829 3a0a 2020 2020  len(tindx):.    
-00009d00: 2020 2020 616c 6c73 7461 636b 7331 203d      allstacks1 =
-00009d10: 205b 5d0a 2020 2020 2020 2020 616c 6c73   [].        alls
-00009d20: 7461 636b 7332 203d 205b 5d0a 2020 2020  tacks2 = [].    
-00009d30: 2020 2020 6e73 7461 636b 7320 3d20 300a      nstacks = 0.
-00009d40: 2020 2020 2020 2020 6363 5f61 7272 6179          cc_array
-00009d50: 203d 205b 5d0a 2020 2020 2020 2020 6363   = [].        cc
-00009d60: 5f6e 676f 6f64 203d 205b 5d0a 2020 2020  _ngood = [].    
-00009d70: 2020 2020 6363 5f74 696d 6520 3d20 5b5d      cc_time = []
-00009d80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00009d90: 6363 5f61 7272 6179 2c20 6363 5f6e 676f  cc_array, cc_ngo
-00009da0: 6f64 2c20 6363 5f74 696d 652c 2061 6c6c  od, cc_time, all
-00009db0: 7374 6163 6b73 312c 2061 6c6c 7374 6163  stacks1, allstac
-00009dc0: 6b73 322c 206e 7374 6163 6b73 0a20 2020  ks2, nstacks.   
-00009dd0: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-00009de0: 2072 656d 6f76 6520 6f6e 6573 2077 6974   remove ones wit
-00009df0: 6820 6261 6420 616d 706c 6974 7564 650a  h bad amplitude.
-00009e00: 2020 2020 2020 2020 6363 5f61 7272 6179          cc_array
-00009e10: 203d 2063 635f 6172 7261 795b 7469 6e64   = cc_array[tind
-00009e20: 782c 203a 5d0a 2020 2020 2020 2020 6363  x, :].        cc
-00009e30: 5f74 696d 6520 3d20 6363 5f74 696d 655b  _time = cc_time[
-00009e40: 7469 6e64 785d 0a20 2020 2020 2020 2063  tindx].        c
-00009e50: 635f 6e67 6f6f 6420 3d20 6363 5f6e 676f  c_ngood = cc_ngo
-00009e60: 6f64 5b74 696e 6478 5d0a 0a20 2020 2020  od[tindx]..     
-00009e70: 2020 2023 2064 6f20 7375 6273 7461 636b     # do substack
-00009e80: 730a 2020 2020 2020 2020 6966 2072 6d61  s.        if rma
-00009e90: 5f73 7562 7374 6163 6b3a 0a20 2020 2020  _substack:.     
-00009ea0: 2020 2020 2020 2074 7374 6172 7420 3d20         tstart = 
-00009eb0: 6f62 7370 792e 5554 4344 6174 6554 696d  obspy.UTCDateTim
-00009ec0: 6528 7374 6172 745f 6461 7465 2920 2d20  e(start_date) - 
-00009ed0: 6f62 7370 792e 5554 4344 6174 6554 696d  obspy.UTCDateTim
-00009ee0: 6528 3139 3730 2c20 312c 2031 290a 2020  e(1970, 1, 1).  
-00009ef0: 2020 2020 2020 2020 2020 7465 6e64 203d            tend =
-00009f00: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
-00009f10: 6d65 2865 6e64 5f64 6174 6529 202d 206f  me(end_date) - o
-00009f20: 6273 7079 2e55 5443 4461 7465 5469 6d65  bspy.UTCDateTime
-00009f30: 2831 3937 302c 2031 2c20 3129 0a20 2020  (1970, 1, 1).   
-00009f40: 2020 2020 2020 2020 2074 7469 6d65 203d           ttime =
-00009f50: 2074 7374 6172 740a 2020 2020 2020 2020   tstart.        
-00009f60: 2020 2020 6e73 7461 636b 203d 2069 6e74      nstack = int
-00009f70: 286e 702e 726f 756e 6428 2874 656e 6420  (np.round((tend 
-00009f80: 2d20 7473 7461 7274 2920 2f20 2872 6d61  - tstart) / (rma
-00009f90: 5f73 7465 7020 2a20 3336 3030 2929 290a  _step * 3600))).
-00009fa0: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
-00009fb0: 6172 7261 7920 3d20 6e70 2e7a 6572 6f73  array = np.zeros
-00009fc0: 2873 6861 7065 3d28 6e73 7461 636b 2c20  (shape=(nstack, 
-00009fd0: 6e70 7473 292c 2064 7479 7065 3d6e 702e  npts), dtype=np.
-00009fe0: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
-00009ff0: 2020 2020 206e 6363 5f74 696d 6520 3d20       ncc_time = 
-0000a000: 6e70 2e7a 6572 6f73 286e 7374 6163 6b2c  np.zeros(nstack,
-0000a010: 2064 7479 7065 3d6e 702e 666c 6f61 7429   dtype=np.float)
-0000a020: 0a20 2020 2020 2020 2020 2020 206e 6363  .            ncc
-0000a030: 5f6e 676f 6f64 203d 206e 702e 7a65 726f  _ngood = np.zero
-0000a040: 7328 6e73 7461 636b 2c20 6474 7970 653d  s(nstack, dtype=
-0000a050: 6e70 2e69 6e74 290a 0a20 2020 2020 2020  np.int)..       
-0000a060: 2020 2020 2023 206c 6f6f 7020 7468 726f       # loop thro
-0000a070: 7567 6820 6561 6368 2074 696d 650a 2020  ugh each time.  
-0000a080: 2020 2020 2020 2020 2020 666f 7220 6969            for ii
-0000a090: 2069 6e20 7261 6e67 6528 6e73 7461 636b   in range(nstack
-0000a0a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000a0b0: 2020 2073 696e 6478 203d 206e 702e 7768     sindx = np.wh
-0000a0c0: 6572 6528 2863 635f 7469 6d65 203e 3d20  ere((cc_time >= 
-0000a0d0: 7474 696d 6529 2026 2028 6363 5f74 696d  ttime) & (cc_tim
-0000a0e0: 6520 3c20 7474 696d 6520 2b20 726d 615f  e < ttime + rma_
-0000a0f0: 7375 6273 7461 636b 202a 2033 3630 3029  substack * 3600)
-0000a100: 295b 305d 0a0a 2020 2020 2020 2020 2020  )[0]..          
-0000a110: 2020 2020 2020 2320 7768 656e 2074 6865        # when the
-0000a120: 7265 2061 7265 2064 6174 6120 696e 2074  re are data in t
-0000a130: 6865 2074 696d 6520 7769 6e64 6f77 0a20  he time window. 
-0000a140: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a150: 6620 6c65 6e28 7369 6e64 7829 3a0a 2020  f len(sindx):.  
-0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a170: 2020 6e63 635f 6172 7261 795b 6969 5d20    ncc_array[ii] 
-0000a180: 3d20 6e70 2e6d 6561 6e28 6363 5f61 7272  = np.mean(cc_arr
-0000a190: 6179 5b73 696e 6478 5d2c 2061 7869 733d  ay[sindx], axis=
-0000a1a0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-0000a1b0: 2020 2020 2020 206e 6363 5f74 696d 655b         ncc_time[
-0000a1c0: 6969 5d20 3d20 7474 696d 650a 2020 2020  ii] = ttime.    
-0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 6e63 635f 6e67 6f6f 645b 6969 5d20 3d20  ncc_ngood[ii] = 
-0000a1f0: 6e70 2e73 756d 2863 635f 6e67 6f6f 645b  np.sum(cc_ngood[
-0000a200: 7369 6e64 785d 2c20 6178 6973 3d30 290a  sindx], axis=0).
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a220: 7474 696d 6520 2b3d 2072 6d61 5f73 7465  ttime += rma_ste
-0000a230: 7020 2a20 3336 3030 0a0a 2020 2020 2020  p * 3600..      
-0000a240: 2020 2020 2020 2320 7265 6d6f 7665 2062        # remove b
-0000a250: 6164 206f 6e65 730a 2020 2020 2020 2020  ad ones.        
-0000a260: 2020 2020 7469 6e64 7820 3d20 6e70 2e77      tindx = np.w
-0000a270: 6865 7265 286e 6363 5f6e 676f 6f64 203e  here(ncc_ngood >
-0000a280: 2030 295b 305d 0a20 2020 2020 2020 2020   0)[0].         
-0000a290: 2020 206e 6363 5f61 7272 6179 203d 206e     ncc_array = n
-0000a2a0: 6363 5f61 7272 6179 5b74 696e 6478 5d0a  cc_array[tindx].
-0000a2b0: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
-0000a2c0: 7469 6d65 203d 206e 6363 5f74 696d 655b  time = ncc_time[
-0000a2d0: 7469 6e64 785d 0a20 2020 2020 2020 2020  tindx].         
-0000a2e0: 2020 206e 6363 5f6e 676f 6f64 203d 206e     ncc_ngood = n
-0000a2f0: 6363 5f6e 676f 6f64 5b74 696e 6478 5d0a  cc_ngood[tindx].
-0000a300: 0a20 2020 2020 2020 2023 2064 6f20 7374  .        # do st
-0000a310: 6163 6b69 6e67 0a20 2020 2020 2020 2061  acking.        a
-0000a320: 6c6c 7374 6163 6b73 3120 3d20 6e70 2e7a  llstacks1 = np.z
-0000a330: 6572 6f73 286e 7074 732c 2064 7479 7065  eros(npts, dtype
-0000a340: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
-0000a350: 2020 2020 2061 6c6c 7374 6163 6b73 3220       allstacks2 
-0000a360: 3d20 6e70 2e7a 6572 6f73 286e 7074 732c  = np.zeros(npts,
-0000a370: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-0000a380: 3229 0a20 2020 2020 2020 2061 6c6c 7374  2).        allst
-0000a390: 6163 6b73 3320 3d20 6e70 2e7a 6572 6f73  acks3 = np.zeros
-0000a3a0: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
-0000a3b0: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
-0000a3c0: 2061 6c6c 7374 6163 6b73 3420 3d20 6e70   allstacks4 = np
-0000a3d0: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
-0000a3e0: 7065 3d6e 702e 666c 6f61 7433 3229 0a0a  pe=np.float32)..
-0000a3f0: 2020 2020 2020 2020 6966 2073 6d65 7468          if smeth
-0000a400: 6f64 203d 3d20 5374 6163 6b4d 6574 686f  od == StackMetho
-0000a410: 642e 4c49 4e45 4152 3a0a 2020 2020 2020  d.LINEAR:.      
-0000a420: 2020 2020 2020 616c 6c73 7461 636b 7331        allstacks1
-0000a430: 203d 206e 702e 6d65 616e 2863 635f 6172   = np.mean(cc_ar
-0000a440: 7261 792c 2061 7869 733d 3029 0a20 2020  ray, axis=0).   
-0000a450: 2020 2020 2065 6c69 6620 736d 6574 686f       elif smetho
-0000a460: 6420 3d3d 2053 7461 636b 4d65 7468 6f64  d == StackMethod
-0000a470: 2e50 5753 3a0a 2020 2020 2020 2020 2020  .PWS:.          
-0000a480: 2020 616c 6c73 7461 636b 7331 203d 2070    allstacks1 = p
-0000a490: 7773 2863 635f 6172 7261 792c 2073 616d  ws(cc_array, sam
-0000a4a0: 705f 6672 6571 290a 2020 2020 2020 2020  p_freq).        
-0000a4b0: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
-0000a4c0: 5374 6163 6b4d 6574 686f 642e 524f 4255  StackMethod.ROBU
-0000a4d0: 5354 3a0a 2020 2020 2020 2020 2020 2020  ST:.            
-0000a4e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000a4f0: 2020 616c 6c73 7461 636b 7331 2c0a 2020    allstacks1,.  
-0000a500: 2020 2020 2020 2020 2020 2020 2020 772c                w,
-0000a510: 0a20 2020 2020 2020 2020 2020 2029 203d  .            ) =
-0000a520: 2072 6f62 7573 745f 7374 6163 6b28 6363   robust_stack(cc
-0000a530: 5f61 7272 6179 2c20 302e 3030 3129 0a20  _array, 0.001). 
-0000a540: 2020 2020 2020 2065 6c69 6620 736d 6574         elif smet
-0000a550: 686f 6420 3d3d 2053 7461 636b 4d65 7468  hod == StackMeth
-0000a560: 6f64 2e53 454c 4543 5449 5645 3a0a 2020  od.SELECTIVE:.  
-0000a570: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
-0000a580: 636b 7331 203d 2073 656c 6563 7469 7665  cks1 = selective
-0000a590: 5f73 7461 636b 2863 635f 6172 7261 792c  _stack(cc_array,
-0000a5a0: 2030 2e30 3031 290a 2020 2020 2020 2020   0.001).        
-0000a5b0: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
-0000a5c0: 5374 6163 6b4d 6574 686f 642e 414c 4c3a  StackMethod.ALL:
-0000a5d0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-0000a5e0: 7374 6163 6b73 3120 3d20 6e70 2e6d 6561  stacks1 = np.mea
-0000a5f0: 6e28 6363 5f61 7272 6179 2c20 6178 6973  n(cc_array, axis
-0000a600: 3d30 290a 2020 2020 2020 2020 2020 2020  =0).            
-0000a610: 616c 6c73 7461 636b 7332 203d 2070 7773  allstacks2 = pws
-0000a620: 2863 635f 6172 7261 792c 2073 616d 705f  (cc_array, samp_
-0000a630: 6672 6571 290a 2020 2020 2020 2020 2020  freq).          
-0000a640: 2020 616c 6c73 7461 636b 7333 203d 2072    allstacks3 = r
-0000a650: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
-0000a660: 7272 6179 2c20 302e 3030 3129 0a20 2020  rray, 0.001).   
-0000a670: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
-0000a680: 6b73 3420 3d20 7365 6c65 6374 6976 655f  ks4 = selective_
-0000a690: 7374 6163 6b28 6363 5f61 7272 6179 2c20  stack(cc_array, 
-0000a6a0: 302e 3030 3129 0a20 2020 2020 2020 206e  0.001).        n
-0000a6b0: 7374 6163 6b73 203d 206e 702e 7375 6d28  stacks = np.sum(
-0000a6c0: 6363 5f6e 676f 6f64 290a 0a20 2020 2023  cc_ngood)..    #
-0000a6d0: 2072 6570 6c61 6365 2074 6865 2061 7272   replace the arr
-0000a6e0: 6179 2066 6f72 2073 7562 7374 6163 6b73  ay for substacks
-0000a6f0: 0a20 2020 2069 6620 726d 615f 7375 6273  .    if rma_subs
-0000a700: 7461 636b 3a0a 2020 2020 2020 2020 6363  tack:.        cc
-0000a710: 5f61 7272 6179 203d 206e 6363 5f61 7272  _array = ncc_arr
-0000a720: 6179 0a20 2020 2020 2020 2063 635f 7469  ay.        cc_ti
-0000a730: 6d65 203d 206e 6363 5f74 696d 650a 2020  me = ncc_time.  
-0000a740: 2020 2020 2020 6363 5f6e 676f 6f64 203d        cc_ngood =
-0000a750: 206e 6363 5f6e 676f 6f64 0a0a 2020 2020   ncc_ngood..    
-0000a760: 2320 676f 6f64 2074 6f20 7265 7475 726e  # good to return
-0000a770: 0a20 2020 2072 6574 7572 6e20 280a 2020  .    return (.  
-0000a780: 2020 2020 2020 6363 5f61 7272 6179 2c0a        cc_array,.
-0000a790: 2020 2020 2020 2020 6363 5f6e 676f 6f64          cc_ngood
-0000a7a0: 2c0a 2020 2020 2020 2020 6363 5f74 696d  ,.        cc_tim
-0000a7b0: 652c 0a20 2020 2020 2020 2061 6c6c 7374  e,.        allst
-0000a7c0: 6163 6b73 312c 0a20 2020 2020 2020 2061  acks1,.        a
-0000a7d0: 6c6c 7374 6163 6b73 322c 0a20 2020 2020  llstacks2,.     
-0000a7e0: 2020 2061 6c6c 7374 6163 6b73 332c 0a20     allstacks3,. 
-0000a7f0: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
-0000a800: 342c 0a20 2020 2020 2020 206e 7374 6163  4,.        nstac
-0000a810: 6b73 2c0a 2020 2020 290a 0a0a 6465 6620  ks,.    )...def 
-0000a820: 726f 7461 7469 6f6e 2862 6967 7374 6163  rotation(bigstac
-0000a830: 6b2c 2070 6172 616d 6574 6572 732c 206c  k, parameters, l
-0000a840: 6f63 7329 3a0a 2020 2020 2222 220a 2020  ocs):.    """.  
-0000a850: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
-0000a860: 7472 616e 7366 6572 7320 7468 6520 4772  transfers the Gr
-0000a870: 6565 6e27 7320 7465 6e73 6f72 2066 726f  een's tensor fro
-0000a880: 6d20 6120 452d 4e2d 5a20 7379 7374 656d  m a E-N-Z system
-0000a890: 2069 6e74 6f20 6120 522d 542d 5a20 6f6e   into a R-T-Z on
-0000a8a0: 650a 0a20 2020 2050 4152 414d 4554 4552  e..    PARAMETER
-0000a8b0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-0000a8c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2062  ----------.    b
-0000a8d0: 6967 7374 6163 6b3a 2020 2039 2063 6f6d  igstack:   9 com
-0000a8e0: 706f 6e65 6e74 2047 7265 656e 2773 2074  ponent Green's t
-0000a8f0: 656e 736f 7220 696e 2045 2d4e 2d5a 2073  ensor in E-N-Z s
-0000a900: 7973 7465 6d0a 2020 2020 7061 7261 6d65  ystem.    parame
-0000a910: 7465 7273 3a20 6469 6374 2063 6f6e 7461  ters: dict conta
-0000a920: 696e 696e 6720 616c 6c20 7061 7261 6d65  ining all parame
-0000a930: 7465 7273 2073 6176 6564 2069 6e20 4153  ters saved in AS
-0000a940: 4446 2066 696c 650a 2020 2020 6c6f 6373  DF file.    locs
-0000a950: 3a20 2020 2020 2020 6469 6374 2063 6f6e  :       dict con
-0000a960: 7461 696e 696e 6720 7374 6174 696f 6e20  taining station 
-0000a970: 616e 676c 6520 696e 666f 2066 6f72 2063  angle info for c
-0000a980: 6f72 7265 6374 696f 6e20 7075 7270 6f73  orrection purpos
-0000a990: 650a 2020 2020 5245 5455 524e 533a 0a20  e.    RETURNS:. 
-0000a9a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000a9b0: 2d2d 2d2d 2d2d 0a20 2020 2074 636f 7272  ------.    tcorr
-0000a9c0: 3a20 3920 636f 6d70 6f6e 656e 7420 4772  : 9 component Gr
-0000a9d0: 6565 6e27 7320 7465 6e73 6f72 2069 6e20  een's tensor in 
-0000a9e0: 522d 542d 5a20 7379 7374 656d 0a20 2020  R-T-Z system.   
-0000a9f0: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
-0000aa00: 7061 7261 6d65 7465 7220 6469 630a 2020  parameter dic.  
-0000aa10: 2020 7069 203d 206e 702e 7069 0a20 2020    pi = np.pi.   
-0000aa20: 2061 7a69 203d 2070 6172 616d 6574 6572   azi = parameter
-0000aa30: 735b 2261 7a69 225d 0a20 2020 2062 617a  s["azi"].    baz
-0000aa40: 203d 2070 6172 616d 6574 6572 735b 2262   = parameters["b
-0000aa50: 617a 225d 0a20 2020 206e 636f 6d70 2c20  az"].    ncomp, 
-0000aa60: 6e70 7473 203d 2062 6967 7374 6163 6b2e  npts = bigstack.
-0000aa70: 7368 6170 650a 2020 2020 6966 206e 636f  shape.    if nco
-0000aa80: 6d70 203c 2039 3a0a 2020 2020 2020 2020  mp < 9:.        
-0000aa90: 6c6f 6767 6572 2e64 6562 7567 2822 6372  logger.debug("cr
-0000aaa0: 6170 2064 6964 206e 6f74 2067 6574 2065  ap did not get e
-0000aab0: 6e6f 7567 6820 636f 6d70 6f6e 656e 7473  nough components
-0000aac0: 2229 0a20 2020 2020 2020 2074 636f 7272  ").        tcorr
-0000aad0: 203d 205b 5d0a 2020 2020 2020 2020 7265   = [].        re
-0000aae0: 7475 726e 2074 636f 7272 0a20 2020 2073  turn tcorr.    s
-0000aaf0: 7461 5320 3d20 7061 7261 6d65 7465 7273  taS = parameters
-0000ab00: 5b22 7374 6174 696f 6e5f 736f 7572 6365  ["station_source
-0000ab10: 225d 0a20 2020 2073 7461 5220 3d20 7061  "].    staR = pa
-0000ab20: 7261 6d65 7465 7273 5b22 7374 6174 696f  rameters["statio
-0000ab30: 6e5f 7265 6365 6976 6572 225d 0a0a 2020  n_receiver"]..  
-0000ab40: 2020 6966 206c 656e 286c 6f63 7329 3a0a    if len(locs):.
-0000ab50: 2020 2020 2020 2020 7374 615f 6c69 7374          sta_list
-0000ab60: 203d 206c 6973 7428 6c6f 6373 5b22 7374   = list(locs["st
-0000ab70: 6174 696f 6e22 5d29 0a20 2020 2020 2020  ation"]).       
-0000ab80: 2061 6e67 6c65 7320 3d20 6c69 7374 286c   angles = list(l
-0000ab90: 6f63 735b 2261 6e67 6c65 225d 290a 2020  ocs["angle"]).  
-0000aba0: 2020 2020 2020 2320 6765 7420 7374 6174        # get stat
-0000abb0: 696f 6e20 696e 666f 2066 726f 6d20 7468  ion info from th
-0000abc0: 6520 6e61 6d65 206f 6620 4153 4446 2066  e name of ASDF f
-0000abd0: 696c 650a 2020 2020 2020 2020 696e 6420  ile.        ind 
-0000abe0: 3d20 7374 615f 6c69 7374 2e69 6e64 6578  = sta_list.index
-0000abf0: 2873 7461 5329 0a20 2020 2020 2020 2061  (staS).        a
-0000ac00: 636f 7272 203d 2061 6e67 6c65 735b 696e  corr = angles[in
-0000ac10: 645d 0a20 2020 2020 2020 2069 6e64 203d  d].        ind =
-0000ac20: 2073 7461 5f6c 6973 742e 696e 6465 7828   sta_list.index(
-0000ac30: 7374 6152 290a 2020 2020 2020 2020 6263  staR).        bc
-0000ac40: 6f72 7220 3d20 616e 676c 6573 5b69 6e64  orr = angles[ind
-0000ac50: 5d0a 0a20 2020 2023 202d 2d2d 616e 676c  ]..    # ---angl
-0000ac60: 6573 2074 6f20 6265 2063 6f72 7265 6374  es to be correct
-0000ac70: 6564 2d2d 2d2d 0a20 2020 2069 6620 6c65  ed----.    if le
-0000ac80: 6e28 6c6f 6373 293a 0a20 2020 2020 2020  n(locs):.       
-0000ac90: 2063 6f73 6120 3d20 6e70 2e63 6f73 2828   cosa = np.cos((
-0000aca0: 617a 6920 2b20 6163 6f72 7229 202a 2070  azi + acorr) * p
-0000acb0: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
-0000acc0: 2073 696e 6120 3d20 6e70 2e73 696e 2828   sina = np.sin((
-0000acd0: 617a 6920 2b20 6163 6f72 7229 202a 2070  azi + acorr) * p
-0000ace0: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
-0000acf0: 2063 6f73 6220 3d20 6e70 2e63 6f73 2828   cosb = np.cos((
-0000ad00: 6261 7a20 2b20 6263 6f72 7229 202a 2070  baz + bcorr) * p
-0000ad10: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
-0000ad20: 2073 696e 6220 3d20 6e70 2e73 696e 2828   sinb = np.sin((
-0000ad30: 6261 7a20 2b20 6263 6f72 7229 202a 2070  baz + bcorr) * p
-0000ad40: 6920 2f20 3138 3029 0a20 2020 2065 6c73  i / 180).    els
-0000ad50: 653a 0a20 2020 2020 2020 2063 6f73 6120  e:.        cosa 
-0000ad60: 3d20 6e70 2e63 6f73 2861 7a69 202a 2070  = np.cos(azi * p
-0000ad70: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
-0000ad80: 2073 696e 6120 3d20 6e70 2e73 696e 2861   sina = np.sin(a
-0000ad90: 7a69 202a 2070 6920 2f20 3138 3029 0a20  zi * pi / 180). 
-0000ada0: 2020 2020 2020 2063 6f73 6220 3d20 6e70         cosb = np
-0000adb0: 2e63 6f73 2862 617a 202a 2070 6920 2f20  .cos(baz * pi / 
-0000adc0: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
-0000add0: 6220 3d20 6e70 2e73 696e 2862 617a 202a  b = np.sin(baz *
-0000ade0: 2070 6920 2f20 3138 3029 0a0a 2020 2020   pi / 180)..    
-0000adf0: 2320 7274 7a5f 636f 6d70 6f6e 656e 7473  # rtz_components
-0000ae00: 203d 205b 275a 5227 2c27 5a54 272c 275a   = ['ZR','ZT','Z
-0000ae10: 5a27 2c27 5252 272c 2752 5427 2c27 525a  Z','RR','RT','RZ
-0000ae20: 272c 2754 5227 2c27 5454 272c 2754 5a27  ','TR','TT','TZ'
-0000ae30: 5d0a 2020 2020 7463 6f72 7220 3d20 6e70  ].    tcorr = np
-0000ae40: 2e7a 6572 6f73 2873 6861 7065 3d28 392c  .zeros(shape=(9,
-0000ae50: 206e 7074 7329 2c20 6474 7970 653d 6e70   npts), dtype=np
-0000ae60: 2e66 6c6f 6174 3332 290a 2020 2020 7463  .float32).    tc
-0000ae70: 6f72 725b 305d 203d 202d 636f 7362 202a  orr[0] = -cosb *
-0000ae80: 2062 6967 7374 6163 6b5b 375d 202d 2073   bigstack[7] - s
-0000ae90: 696e 6220 2a20 6269 6773 7461 636b 5b36  inb * bigstack[6
-0000aea0: 5d0a 2020 2020 7463 6f72 725b 315d 203d  ].    tcorr[1] =
-0000aeb0: 2073 696e 6220 2a20 6269 6773 7461 636b   sinb * bigstack
-0000aec0: 5b37 5d20 2d20 636f 7362 202a 2062 6967  [7] - cosb * big
-0000aed0: 7374 6163 6b5b 365d 0a20 2020 2074 636f  stack[6].    tco
-0000aee0: 7272 5b32 5d20 3d20 6269 6773 7461 636b  rr[2] = bigstack
-0000aef0: 5b38 5d0a 2020 2020 7463 6f72 725b 335d  [8].    tcorr[3]
-0000af00: 203d 2028 0a20 2020 2020 2020 202d 636f   = (.        -co
-0000af10: 7361 202a 2063 6f73 6220 2a20 6269 6773  sa * cosb * bigs
-0000af20: 7461 636b 5b34 5d20 2d20 636f 7361 202a  tack[4] - cosa *
-0000af30: 2073 696e 6220 2a20 6269 6773 7461 636b   sinb * bigstack
-0000af40: 5b33 5d20 2d20 7369 6e61 202a 2063 6f73  [3] - sina * cos
-0000af50: 6220 2a20 6269 6773 7461 636b 5b31 5d20  b * bigstack[1] 
-0000af60: 2d20 7369 6e61 202a 2073 696e 6220 2a20  - sina * sinb * 
-0000af70: 6269 6773 7461 636b 5b30 5d0a 2020 2020  bigstack[0].    
-0000af80: 290a 2020 2020 7463 6f72 725b 345d 203d  ).    tcorr[4] =
-0000af90: 2028 0a20 2020 2020 2020 2063 6f73 6120   (.        cosa 
-0000afa0: 2a20 7369 6e62 202a 2062 6967 7374 6163  * sinb * bigstac
-0000afb0: 6b5b 345d 202d 2063 6f73 6120 2a20 636f  k[4] - cosa * co
-0000afc0: 7362 202a 2062 6967 7374 6163 6b5b 335d  sb * bigstack[3]
-0000afd0: 202b 2073 696e 6120 2a20 7369 6e62 202a   + sina * sinb *
-0000afe0: 2062 6967 7374 6163 6b5b 315d 202d 2073   bigstack[1] - s
-0000aff0: 696e 6120 2a20 636f 7362 202a 2062 6967  ina * cosb * big
-0000b000: 7374 6163 6b5b 305d 0a20 2020 2029 0a20  stack[0].    ). 
-0000b010: 2020 2074 636f 7272 5b35 5d20 3d20 636f     tcorr[5] = co
-0000b020: 7361 202a 2062 6967 7374 6163 6b5b 355d  sa * bigstack[5]
-0000b030: 202b 2073 696e 6120 2a20 6269 6773 7461   + sina * bigsta
-0000b040: 636b 5b32 5d0a 2020 2020 7463 6f72 725b  ck[2].    tcorr[
-0000b050: 365d 203d 2028 0a20 2020 2020 2020 2073  6] = (.        s
-0000b060: 696e 6120 2a20 636f 7362 202a 2062 6967  ina * cosb * big
-0000b070: 7374 6163 6b5b 345d 202b 2073 696e 6120  stack[4] + sina 
-0000b080: 2a20 7369 6e62 202a 2062 6967 7374 6163  * sinb * bigstac
-0000b090: 6b5b 335d 202d 2063 6f73 6120 2a20 636f  k[3] - cosa * co
-0000b0a0: 7362 202a 2062 6967 7374 6163 6b5b 315d  sb * bigstack[1]
-0000b0b0: 202d 2063 6f73 6120 2a20 7369 6e62 202a   - cosa * sinb *
-0000b0c0: 2062 6967 7374 6163 6b5b 305d 0a20 2020   bigstack[0].   
-0000b0d0: 2029 0a20 2020 2074 636f 7272 5b37 5d20   ).    tcorr[7] 
-0000b0e0: 3d20 280a 2020 2020 2020 2020 2d73 696e  = (.        -sin
-0000b0f0: 6120 2a20 7369 6e62 202a 2062 6967 7374  a * sinb * bigst
-0000b100: 6163 6b5b 345d 202b 2073 696e 6120 2a20  ack[4] + sina * 
-0000b110: 636f 7362 202a 2062 6967 7374 6163 6b5b  cosb * bigstack[
-0000b120: 335d 202b 2063 6f73 6120 2a20 7369 6e62  3] + cosa * sinb
-0000b130: 202a 2062 6967 7374 6163 6b5b 315d 202d   * bigstack[1] -
-0000b140: 2063 6f73 6120 2a20 636f 7362 202a 2062   cosa * cosb * b
-0000b150: 6967 7374 6163 6b5b 305d 0a20 2020 2029  igstack[0].    )
-0000b160: 0a20 2020 2074 636f 7272 5b38 5d20 3d20  .    tcorr[8] = 
-0000b170: 2d73 696e 6120 2a20 6269 6773 7461 636b  -sina * bigstack
-0000b180: 5b35 5d20 2b20 636f 7361 202a 2062 6967  [5] + cosa * big
-0000b190: 7374 6163 6b5b 325d 0a0a 2020 2020 7265  stack[2]..    re
-0000b1a0: 7475 726e 2074 636f 7272 0a0a 0a23 2323  turn tcorr...###
-0000b1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002680: 6f72 7421 2020 2573 2220 2520 7374 5b30  ort!  %s" % st[0
+00002690: 5d29 0a20 2020 2020 2020 2020 2020 2065  ]).            e
+000026a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000026b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000026c0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000026d0: 6767 6572 2e69 6e66 6f28 2272 656d 6f76  gger.info("remov
+000026e0: 696e 6720 7265 7370 6f6e 7365 2066 6f72  ing response for
+000026f0: 2025 7320 7573 696e 6720 696e 7622 2025   %s using inv" %
+00002700: 2073 745b 305d 290a 2020 2020 2020 2020   st[0]).        
+00002710: 2020 2020 2020 2020 2020 2020 7374 5b30              st[0
+00002720: 5d2e 6174 7461 6368 5f72 6573 706f 6e73  ].attach_respons
+00002730: 6528 696e 7629 0a20 2020 2020 2020 2020  e(inv).         
+00002740: 2020 2020 2020 2020 2020 2073 745b 305d             st[0]
+00002750: 2e72 656d 6f76 655f 7265 7370 6f6e 7365  .remove_response
+00002760: 286f 7574 7075 743d 726d 5f72 6573 705f  (output=rm_resp_
+00002770: 6f75 742c 2070 7265 5f66 696c 743d 7072  out, pre_filt=pr
+00002780: 655f 6669 6c74 2c20 7761 7465 725f 6c65  e_filt, water_le
+00002790: 7665 6c3d 3630 290a 2020 2020 2020 2020  vel=60).        
+000027a0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+000027b0: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+000027e0: 6728 2246 6169 6c65 6420 746f 2072 656d  g("Failed to rem
+000027f0: 6f76 6520 7265 7370 6f6e 7365 2066 726f  ove response fro
+00002800: 6d20 2573 2e20 5265 7475 726e 696e 6720  m %s. Returning 
+00002810: 656d 7074 7920 7374 7265 616d 2e20 2573  empty stream. %s
+00002820: 2220 2520 2873 745b 305d 2c20 6529 290a  " % (st[0], e)).
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 7374 203d 205b 5d0a 2020 2020      st = [].    
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 7265 7475 726e 2073 740a 0a20 2020 2020  return st..     
+00002870: 2020 2065 6c69 6620 726d 5f72 6573 7020     elif rm_resp 
+00002880: 3d3d 2022 7370 6563 7472 756d 223a 0a20  == "spectrum":. 
+00002890: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000028a0: 722e 696e 666f 2822 7265 6d6f 7665 2072  r.info("remove r
+000028b0: 6573 706f 6e73 6520 7573 696e 6720 7370  esponse using sp
+000028c0: 6563 7472 756d 2229 0a20 2020 2020 2020  ectrum").       
+000028d0: 2020 2020 2073 7065 6366 696c 6520 3d20       specfile = 
+000028e0: 676c 6f62 2e67 6c6f 6228 6f73 2e70 6174  glob.glob(os.pat
+000028f0: 682e 6a6f 696e 2872 6573 7064 6972 2c20  h.join(respdir, 
+00002900: 222a 2220 2b20 7374 6174 696f 6e20 2b20  "*" + station + 
+00002910: 222a 2229 290a 2020 2020 2020 2020 2020  "*")).          
+00002920: 2020 6966 206c 656e 2873 7065 6366 696c    if len(specfil
+00002930: 6529 203d 3d20 303a 0a20 2020 2020 2020  e) == 0:.       
+00002940: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00002950: 616c 7565 4572 726f 7228 226e 6f20 7265  alueError("no re
+00002960: 7370 6f6e 7365 2073 6570 6374 7275 6d20  sponse sepctrum 
+00002970: 666f 756e 6420 666f 7220 2573 2220 2520  found for %s" % 
+00002980: 7374 6174 696f 6e29 0a20 2020 2020 2020  station).       
+00002990: 2020 2020 2073 7420 3d20 7265 7370 5f73       st = resp_s
+000029a0: 7065 6374 7275 6d28 7374 2c20 7370 6563  pectrum(st, spec
+000029b0: 6669 6c65 5b30 5d2c 2073 616d 705f 6672  file[0], samp_fr
+000029c0: 6571 2c20 7072 655f 6669 6c74 290a 0a20  eq, pre_filt).. 
+000029d0: 2020 2020 2020 2065 6c69 6620 726d 5f72         elif rm_r
+000029e0: 6573 7020 3d3d 2022 5245 5350 223a 0a20  esp == "RESP":. 
+000029f0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00002a00: 722e 696e 666f 2822 7265 6d6f 7665 2072  r.info("remove r
+00002a10: 6573 706f 6e73 6520 7573 696e 6720 5245  esponse using RE
+00002a20: 5350 2066 696c 6573 2229 0a20 2020 2020  SP files").     
+00002a30: 2020 2020 2020 2072 6573 7020 3d20 676c         resp = gl
+00002a40: 6f62 2e67 6c6f 6228 6f73 2e70 6174 682e  ob.glob(os.path.
+00002a50: 6a6f 696e 2872 6573 7064 6972 2c20 2252  join(respdir, "R
+00002a60: 4553 502e 2220 2b20 7374 6174 696f 6e20  ESP." + station 
+00002a70: 2b20 222a 2229 290a 2020 2020 2020 2020  + "*")).        
+00002a80: 2020 2020 6966 206c 656e 2872 6573 7029      if len(resp)
+00002a90: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00002aa0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00002ab0: 7565 4572 726f 7228 226e 6f20 5245 5350  ueError("no RESP
+00002ac0: 2066 696c 6573 2066 6f75 6e64 2066 6f72   files found for
+00002ad0: 2025 7322 2025 2073 7461 7469 6f6e 290a   %s" % station).
+00002ae0: 2020 2020 2020 2020 2020 2020 7365 6564              seed
+00002af0: 7265 7370 203d 207b 0a20 2020 2020 2020  resp = {.       
+00002b00: 2020 2020 2020 2020 2022 6669 6c65 6e61           "filena
+00002b10: 6d65 223a 2072 6573 705b 305d 2c0a 2020  me": resp[0],.  
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00002b30: 6174 6522 3a20 7374 6172 7474 696d 652c  ate": starttime,
+00002b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b50: 2022 756e 6974 7322 3a20 2244 4953 222c   "units": "DIS",
+00002b60: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00002b70: 2020 2020 2020 2020 2020 2073 742e 7369             st.si
+00002b80: 6d75 6c61 7465 2870 617a 5f72 656d 6f76  mulate(paz_remov
+00002b90: 653d 4e6f 6e65 2c20 7072 655f 6669 6c74  e=None, pre_filt
+00002ba0: 3d70 7265 5f66 696c 742c 2073 6565 6472  =pre_filt, seedr
+00002bb0: 6573 703d 7365 6564 7265 7370 290a 0a20  esp=seedresp).. 
+00002bc0: 2020 2020 2020 2065 6c69 6620 726d 5f72         elif rm_r
+00002bd0: 6573 7020 3d3d 2022 706f 6c65 737a 6572  esp == "poleszer
+00002be0: 6f73 223a 0a20 2020 2020 2020 2020 2020  os":.           
+00002bf0: 206c 6f67 6765 722e 696e 666f 2822 7265   logger.info("re
+00002c00: 6d6f 7665 2072 6573 706f 6e73 6520 7573  move response us
+00002c10: 696e 6720 706f 6c65 7320 616e 6420 7a65  ing poles and ze
+00002c20: 726f 7322 290a 2020 2020 2020 2020 2020  ros").          
+00002c30: 2020 7061 7a5f 7374 7320 3d20 676c 6f62    paz_sts = glob
+00002c40: 2e67 6c6f 6228 6f73 2e70 6174 682e 6a6f  .glob(os.path.jo
+00002c50: 696e 2872 6573 7064 6972 2c20 222a 2220  in(respdir, "*" 
+00002c60: 2b20 7374 6174 696f 6e20 2b20 222a 2229  + station + "*")
+00002c70: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00002c80: 206c 656e 2870 617a 5f73 7473 2920 3d3d   len(paz_sts) ==
+00002c90: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00002ca0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00002cb0: 7272 6f72 2822 6e6f 2070 6f6c 6573 7a65  rror("no polesze
+00002cc0: 726f 7320 666f 756e 6420 666f 7220 2573  ros found for %s
+00002cd0: 2220 2520 7374 6174 696f 6e29 0a20 2020  " % station).   
+00002ce0: 2020 2020 2020 2020 2073 742e 7369 6d75           st.simu
+00002cf0: 6c61 7465 2870 617a 5f72 656d 6f76 653d  late(paz_remove=
+00002d00: 7061 7a5f 7374 735b 305d 2c20 7072 655f  paz_sts[0], pre_
+00002d10: 6669 6c74 3d70 7265 5f66 696c 7429 0a0a  filt=pre_filt)..
+00002d20: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00002d30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00002d40: 5661 6c75 6545 7272 6f72 2822 6e6f 2073  ValueError("no s
+00002d50: 7563 6820 6f70 7469 6f6e 2066 6f72 2072  uch option for r
+00002d60: 6d5f 7265 7370 2120 706c 6561 7365 2064  m_resp! please d
+00002d70: 6f75 626c 6520 6368 6563 6b21 2229 0a0a  ouble check!")..
+00002d80: 2020 2020 6e74 7220 3d20 6f62 7370 792e      ntr = obspy.
+00002d90: 5374 7265 616d 2829 0a20 2020 2023 2074  Stream().    # t
+00002da0: 7269 6d20 6120 636f 6e74 696e 6f75 7320  rim a continous 
+00002db0: 7365 676d 656e 7420 696e 746f 2075 7365  segment into use
+00002dc0: 722d 6465 6669 6e65 6420 7365 7175 656e  r-defined sequen
+00002dd0: 6365 730a 2020 2020 7374 5b30 5d2e 7472  ces.    st[0].tr
+00002de0: 696d 280a 2020 2020 2020 2020 7374 6172  im(.        star
+00002df0: 7474 696d 653d 7374 6172 7474 696d 652c  ttime=starttime,
+00002e00: 0a20 2020 2020 2020 2065 6e64 7469 6d65  .        endtime
+00002e10: 3d65 6e64 7469 6d65 2c0a 2020 2020 2020  =endtime,.      
+00002e20: 2020 7061 643d 5472 7565 2c0a 2020 2020    pad=True,.    
+00002e30: 2020 2020 6669 6c6c 5f76 616c 7565 3d30      fill_value=0
+00002e40: 2c0a 2020 2020 290a 2020 2020 6e74 722e  ,.    ).    ntr.
+00002e50: 6170 7065 6e64 2873 745b 305d 290a 0a20  append(st[0]).. 
+00002e60: 2020 2072 6574 7572 6e20 6e74 720a 0a0a     return ntr...
+00002e70: 6465 6620 7374 6174 7332 696e 7628 7374  def stats2inv(st
+00002e80: 6174 732c 2070 7265 7072 6f5f 7061 7261  ats, prepro_para
+00002e90: 2c20 6c6f 6373 3d4e 6f6e 6529 3a0a 2020  , locs=None):.  
+00002ea0: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
+00002eb0: 756e 6374 696f 6e20 6372 6561 7465 7320  unction creates 
+00002ec0: 696e 7665 6e74 6f72 7920 6769 7665 6e20  inventory given 
+00002ed0: 7468 6520 7374 6174 7320 7061 7261 6d65  the stats parame
+00002ee0: 7465 7273 2069 6e20 616e 206f 6273 7079  ters in an obspy
+00002ef0: 2073 7472 6561 6d20 6f72 2061 2073 7461   stream or a sta
+00002f00: 7469 6f6e 206c 6973 742e 0a20 2020 2028  tion list..    (
+00002f10: 7573 6564 2069 6e20 5330 4229 0a20 2020  used in S0B).   
+00002f20: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
+00002f30: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00002f40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
+00002f50: 6174 733a 206f 6273 7079 2074 7261 6365  ats: obspy trace
+00002f60: 2073 7461 7473 206f 626a 6563 7420 636f   stats object co
+00002f70: 6e74 6169 6e69 6e67 2061 6c6c 2073 7461  ntaining all sta
+00002f80: 7469 6f6e 2068 6561 6465 7220 696e 666f  tion header info
+00002f90: 0a20 2020 2070 7265 7072 6f5f 7061 7261  .    prepro_para
+00002fa0: 3a20 6469 6374 2063 6f6e 7461 696e 696e  : dict containin
+00002fb0: 6720 6666 7420 7061 7261 6d65 7465 7273  g fft parameters
+00002fc0: 2c20 7375 6368 2061 7320 6672 6571 7565  , such as freque
+00002fd0: 6e63 7920 6261 6e64 7320 616e 6420 7365  ncy bands and se
+00002fe0: 6c65 6374 696f 6e20 666f 7220 696e 7374  lection for inst
+00002ff0: 7275 6d65 6e74 0a20 2020 2072 6573 706f  rument.    respo
+00003000: 6e73 6520 7265 6d6f 7661 6c20 6574 632e  nse removal etc.
+00003010: 0a20 2020 206c 6f63 733a 2020 7061 6e64  .    locs:  pand
+00003020: 6120 6461 7461 2066 7261 6d65 206f 6620  a data frame of 
+00003030: 7468 6520 7374 6174 696f 6e20 6c69 7374  the station list
+00003040: 2e20 6974 2069 7320 6e65 6564 6564 2066  . it is needed f
+00003050: 6f72 2063 6f6e 7665 7269 6e67 206d 696e  or convering min
+00003060: 6973 6565 6420 6669 6c65 7320 696e 746f  iseed files into
+00003070: 2041 5344 460a 2020 2020 5245 5455 524e   ASDF.    RETURN
+00003080: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00003090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000030a0: 2020 2020 696e 763a 206f 6273 7079 2069      inv: obspy i
+000030b0: 6e76 656e 746f 7279 206f 626a 6563 7420  nventory object 
+000030c0: 6f66 2061 6c6c 2073 7461 7469 6f6e 2069  of all station i
+000030d0: 6e66 6f20 746f 2062 6520 7573 6564 206c  nfo to be used l
+000030e0: 6174 6572 0a20 2020 2022 2222 0a20 2020  ater.    """.   
+000030f0: 2073 7461 786d 6c20 3d20 7072 6570 726f   staxml = prepro
+00003100: 5f70 6172 615b 2273 7461 7469 6f6e 786d  _para["stationxm
+00003110: 6c22 5d0a 2020 2020 7265 7370 6469 7220  l"].    respdir 
+00003120: 3d20 7072 6570 726f 5f70 6172 615b 2272  = prepro_para["r
+00003130: 6573 7064 6972 225d 0a20 2020 2069 6e70  espdir"].    inp
+00003140: 7574 5f66 6d74 203d 2070 7265 7072 6f5f  ut_fmt = prepro_
+00003150: 7061 7261 5b22 696e 7075 745f 666d 7422  para["input_fmt"
+00003160: 5d0a 2020 2020 6966 2073 7461 786d 6c3a  ].    if staxml:
+00003170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003180: 7374 6174 7332 496e 765f 7374 6178 6d6c  stats2Inv_staxml
+00003190: 2873 7461 7473 2c20 7265 7370 6469 7229  (stats, respdir)
+000031a0: 0a20 2020 2069 6620 696e 7075 745f 666d  .    if input_fm
+000031b0: 7420 3d3d 2022 7361 6322 3a0a 2020 2020  t == "sac":.    
+000031c0: 2020 2020 7265 7475 726e 2073 7461 7473      return stats
+000031d0: 3269 6e76 5f73 6163 2873 7461 7473 290a  2inv_sac(stats).
+000031e0: 2020 2020 656c 6966 2069 6e70 7574 5f66      elif input_f
+000031f0: 6d74 203d 3d20 226d 7365 6564 223a 0a20  mt == "mseed":. 
+00003200: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+00003210: 6174 7332 696e 765f 6d73 6565 6428 7374  ats2inv_mseed(st
+00003220: 6174 732c 206c 6f63 7329 0a0a 0a64 6566  ats, locs)...def
+00003230: 2073 7461 7473 3249 6e76 5f73 7461 786d   stats2Inv_staxm
+00003240: 6c28 7374 6174 732c 2072 6573 7064 6972  l(stats, respdir
+00003250: 2920 2d3e 2049 6e76 656e 746f 7279 3a0a  ) -> Inventory:.
+00003260: 2020 2020 6966 206e 6f74 2072 6573 7064      if not respd
+00003270: 6972 3a0a 2020 2020 2020 2020 7261 6973  ir:.        rais
+00003280: 6520 5661 6c75 6545 7272 6f72 2822 4162  e ValueError("Ab
+00003290: 6f72 7421 2073 7461 786d 6c20 6973 2073  ort! staxml is s
+000032a0: 656c 6563 7465 6420 6275 7420 6e6f 2064  elected but no d
+000032b0: 6972 6563 746f 7279 2069 7320 6769 7665  irectory is give
+000032c0: 6e20 746f 2061 6363 6573 7320 7468 6520  n to access the 
+000032d0: 6669 6c65 7322 290a 2020 2020 656c 7365  files").    else
+000032e0: 3a0a 2020 2020 2020 2020 696e 7666 696c  :.        invfil
+000032f0: 656c 6973 7420 3d20 676c 6f62 2e67 6c6f  elist = glob.glo
+00003300: 6228 6f73 2e70 6174 682e 6a6f 696e 2872  b(os.path.join(r
+00003310: 6573 7064 6972 2c20 222a 2220 2b20 7374  espdir, "*" + st
+00003320: 6174 732e 7374 6174 696f 6e20 2b20 222a  ats.station + "*
+00003330: 2229 290a 2020 2020 2020 2020 6966 206c  ")).        if l
+00003340: 656e 2869 6e76 6669 6c65 6c69 7374 2920  en(invfilelist) 
+00003350: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00003360: 2069 6e76 6669 6c65 203d 2069 6e76 6669   invfile = invfi
+00003370: 6c65 6c69 7374 5b30 5d0a 2020 2020 2020  lelist[0].      
+00003380: 2020 2020 2020 6966 206c 656e 2869 6e76        if len(inv
+00003390: 6669 6c65 6c69 7374 2920 3e20 313a 0a20  filelist) > 1:. 
+000033a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000033b0: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033d0: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+000033e0: 2020 2020 2020 2020 2020 2020 2022 5761               "Wa
+000033f0: 726e 696e 6721 204d 6f72 6520 7468 616e  rning! More than
+00003400: 206f 6e65 2053 7461 7469 6f6e 584d 4c20   one StationXML 
+00003410: 6669 6c65 2077 6173 2066 6f75 6e64 2066  file was found f
+00003420: 6f72 2073 7461 7469 6f6e 2025 732e 220a  or station %s.".
+00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003440: 2020 2020 2020 2020 2b20 224b 6565 7069          + "Keepi
+00003450: 6e67 2074 6865 2066 6972 7374 2066 696c  ng the first fil
+00003460: 6520 696e 206c 6973 742e 220a 2020 2020  e in list.".    
+00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003490: 2020 2020 2020 2520 7374 6174 732e 7374        % stats.st
+000034a0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
+000034b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000034c0: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+000034d0: 7366 696c 6528 7374 7228 696e 7666 696c  sfile(str(invfil
+000034e0: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
+000034f0: 2020 2020 2069 6e76 203d 206f 6273 7079       inv = obspy
+00003500: 2e72 6561 645f 696e 7665 6e74 6f72 7928  .read_inventory(
+00003510: 696e 7666 696c 6529 0a20 2020 2020 2020  invfile).       
+00003520: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003530: 696e 760a 2020 2020 2020 2020 656c 7365  inv.        else
+00003540: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00003550: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00003560: 436f 756c 6420 6e6f 7420 6669 6e64 2061  Could not find a
+00003570: 2053 7461 7469 6f6e 584d 4c20 6669 6c65   StationXML file
+00003580: 2066 6f72 2073 7461 7469 6f6e 3a20 2573   for station: %s
+00003590: 2e22 2025 2073 7461 7473 2e73 7461 7469  ." % stats.stati
+000035a0: 6f6e 290a 0a0a 6465 6620 7374 6174 7332  on)...def stats2
+000035b0: 696e 765f 7361 6328 7374 6174 7329 3a0a  inv_sac(stats):.
+000035c0: 2020 2020 696e 7620 3d20 496e 7665 6e74      inv = Invent
+000035d0: 6f72 7928 6e65 7477 6f72 6b73 3d5b 5d2c  ory(networks=[],
+000035e0: 2073 6f75 7263 653d 2268 6f6d 6567 726f   source="homegro
+000035f0: 776e 2229 0a20 2020 206e 6574 203d 204e  wn").    net = N
+00003600: 6574 776f 726b 280a 2020 2020 2020 2020  etwork(.        
+00003610: 2320 5468 6973 2069 7320 7468 6520 6e65  # This is the ne
+00003620: 7477 6f72 6b20 636f 6465 2061 6363 6f72  twork code accor
+00003630: 6469 6e67 2074 6f20 7468 6520 5345 4544  ding to the SEED
+00003640: 2073 7461 6e64 6172 642e 0a20 2020 2020   standard..     
+00003650: 2020 2063 6f64 653d 7374 6174 732e 6e65     code=stats.ne
+00003660: 7477 6f72 6b2c 0a20 2020 2020 2020 2073  twork,.        s
+00003670: 7461 7469 6f6e 733d 5b5d 2c0a 2020 2020  tations=[],.    
+00003680: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+00003690: 2263 7265 6174 6564 2066 726f 6d20 5341  "created from SA
+000036a0: 4320 616e 6420 7265 7370 2066 696c 6573  C and resp files
+000036b0: 222c 0a20 2020 2020 2020 2073 7461 7274  ",.        start
+000036c0: 5f64 6174 653d 7374 6174 732e 7374 6172  _date=stats.star
+000036d0: 7474 696d 652c 0a20 2020 2029 0a0a 2020  ttime,.    )..  
+000036e0: 2020 7374 6120 3d20 5374 6174 696f 6e28    sta = Station(
+000036f0: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+00003700: 6973 2074 6865 2073 7461 7469 6f6e 2063  is the station c
+00003710: 6f64 6520 6163 636f 7264 696e 6720 746f  ode according to
+00003720: 2074 6865 2053 4545 4420 7374 616e 6461   the SEED standa
+00003730: 7264 2e0a 2020 2020 2020 2020 636f 6465  rd..        code
+00003740: 3d73 7461 7473 2e73 7461 7469 6f6e 2c0a  =stats.station,.
+00003750: 2020 2020 2020 2020 6c61 7469 7475 6465          latitude
+00003760: 3d73 7461 7473 2e73 6163 5b22 7374 6c61  =stats.sac["stla
+00003770: 225d 2c0a 2020 2020 2020 2020 6c6f 6e67  "],.        long
+00003780: 6974 7564 653d 7374 6174 732e 7361 635b  itude=stats.sac[
+00003790: 2273 746c 6f22 5d2c 0a20 2020 2020 2020  "stlo"],.       
+000037a0: 2065 6c65 7661 7469 6f6e 3d73 7461 7473   elevation=stats
+000037b0: 2e73 6163 5b22 7374 656c 225d 2c0a 2020  .sac["stel"],.  
+000037c0: 2020 2020 2020 6372 6561 7469 6f6e 5f64        creation_d
+000037d0: 6174 653d 7374 6174 732e 7374 6172 7474  ate=stats.startt
+000037e0: 696d 652c 0a20 2020 2020 2020 2073 6974  ime,.        sit
+000037f0: 653d 5369 7465 286e 616d 653d 2246 6972  e=Site(name="Fir
+00003800: 7374 2073 7461 7469 6f6e 2229 2c0a 2020  st station"),.  
+00003810: 2020 290a 0a20 2020 2063 6861 203d 2043    )..    cha = C
+00003820: 6861 6e6e 656c 280a 2020 2020 2020 2020  hannel(.        
+00003830: 2320 5468 6973 2069 7320 7468 6520 6368  # This is the ch
+00003840: 616e 6e65 6c20 636f 6465 2061 6363 6f72  annel code accor
+00003850: 6469 6e67 2074 6f20 7468 6520 5345 4544  ding to the SEED
+00003860: 2073 7461 6e64 6172 642e 0a20 2020 2020   standard..     
+00003870: 2020 2063 6f64 653d 7374 6174 732e 6368     code=stats.ch
+00003880: 616e 6e65 6c2c 0a20 2020 2020 2020 2023  annel,.        #
+00003890: 2054 6869 7320 6973 2074 6865 206c 6f63   This is the loc
+000038a0: 6174 696f 6e20 636f 6465 2061 6363 6f72  ation code accor
+000038b0: 6469 6e67 2074 6f20 7468 6520 5345 4544  ding to the SEED
+000038c0: 2073 7461 6e64 6172 642e 0a20 2020 2020   standard..     
+000038d0: 2020 206c 6f63 6174 696f 6e5f 636f 6465     location_code
+000038e0: 3d73 7461 7473 2e6c 6f63 6174 696f 6e2c  =stats.location,
+000038f0: 0a20 2020 2020 2020 2023 204e 6f74 6520  .        # Note 
+00003900: 7468 6174 2074 6865 7365 2063 6f6f 7264  that these coord
+00003910: 696e 6174 6573 2063 616e 2064 6966 6665  inates can diffe
+00003920: 7220 6672 6f6d 2074 6865 2073 7461 7469  r from the stati
+00003930: 6f6e 2063 6f6f 7264 696e 6174 6573 2e0a  on coordinates..
+00003940: 2020 2020 2020 2020 6c61 7469 7475 6465          latitude
+00003950: 3d73 7461 7473 2e73 6163 5b22 7374 6c61  =stats.sac["stla
+00003960: 225d 2c0a 2020 2020 2020 2020 6c6f 6e67  "],.        long
+00003970: 6974 7564 653d 7374 6174 732e 7361 635b  itude=stats.sac[
+00003980: 2273 746c 6f22 5d2c 0a20 2020 2020 2020  "stlo"],.       
+00003990: 2065 6c65 7661 7469 6f6e 3d73 7461 7473   elevation=stats
+000039a0: 2e73 6163 5b22 7374 656c 225d 2c0a 2020  .sac["stel"],.  
+000039b0: 2020 2020 2020 6465 7074 683d 2d73 7461        depth=-sta
+000039c0: 7473 2e73 6163 5b22 7374 656c 225d 2c0a  ts.sac["stel"],.
+000039d0: 2020 2020 2020 2020 617a 696d 7574 683d          azimuth=
+000039e0: 7374 6174 732e 7361 635b 2263 6d70 617a  stats.sac["cmpaz
+000039f0: 225d 2c0a 2020 2020 2020 2020 6469 703d  "],.        dip=
+00003a00: 7374 6174 732e 7361 635b 2263 6d70 696e  stats.sac["cmpin
+00003a10: 6322 5d2c 0a20 2020 2020 2020 2073 616d  c"],.        sam
+00003a20: 706c 655f 7261 7465 3d73 7461 7473 2e73  ple_rate=stats.s
+00003a30: 616d 706c 696e 675f 7261 7465 2c0a 2020  ampling_rate,.  
+00003a40: 2020 290a 2020 2020 7265 7370 6f6e 7365    ).    response
+00003a50: 203d 206f 6273 7079 2e63 6f72 652e 696e   = obspy.core.in
+00003a60: 7665 6e74 6f72 792e 7265 7370 6f6e 7365  ventory.response
+00003a70: 2e52 6573 706f 6e73 6528 290a 0a20 2020  .Response()..   
+00003a80: 2023 204e 6f77 2074 6965 2069 7420 616c   # Now tie it al
+00003a90: 6c20 746f 6765 7468 6572 2e0a 2020 2020  l together..    
+00003aa0: 6368 612e 7265 7370 6f6e 7365 203d 2072  cha.response = r
+00003ab0: 6573 706f 6e73 650a 2020 2020 7374 612e  esponse.    sta.
+00003ac0: 6368 616e 6e65 6c73 2e61 7070 656e 6428  channels.append(
+00003ad0: 6368 6129 0a20 2020 206e 6574 2e73 7461  cha).    net.sta
+00003ae0: 7469 6f6e 732e 6170 7065 6e64 2873 7461  tions.append(sta
+00003af0: 290a 2020 2020 696e 762e 6e65 7477 6f72  ).    inv.networ
+00003b00: 6b73 2e61 7070 656e 6428 6e65 7429 0a0a  ks.append(net)..
+00003b10: 2020 2020 7265 7475 726e 2069 6e76 0a0a      return inv..
+00003b20: 0a64 6566 2073 7461 7473 3269 6e76 5f6d  .def stats2inv_m
+00003b30: 7365 6564 2873 7461 7473 2c20 6c6f 6373  seed(stats, locs
+00003b40: 3a20 7064 2e44 6174 6146 7261 6d65 2920  : pd.DataFrame) 
+00003b50: 2d3e 2049 6e76 656e 746f 7279 3a0a 2020  -> Inventory:.  
+00003b60: 2020 696e 7620 3d20 496e 7665 6e74 6f72    inv = Inventor
+00003b70: 7928 6e65 7477 6f72 6b73 3d5b 5d2c 2073  y(networks=[], s
+00003b80: 6f75 7263 653d 2268 6f6d 6567 726f 776e  ource="homegrown
+00003b90: 2229 0a20 2020 2069 7374 6120 3d20 6c6f  ").    ista = lo
+00003ba0: 6373 5b6c 6f63 735b 2273 7461 7469 6f6e  cs[locs["station
+00003bb0: 225d 203d 3d20 7374 6174 732e 7374 6174  "] == stats.stat
+00003bc0: 696f 6e5d 2e69 6e64 6578 2e76 616c 7565  ion].index.value
+00003bd0: 732e 6173 7479 7065 2822 696e 7436 3422  s.astype("int64"
+00003be0: 295b 305d 0a0a 2020 2020 6e65 7420 3d20  )[0]..    net = 
+00003bf0: 4e65 7477 6f72 6b28 0a20 2020 2020 2020  Network(.       
+00003c00: 2023 2054 6869 7320 6973 2074 6865 206e   # This is the n
+00003c10: 6574 776f 726b 2063 6f64 6520 6163 636f  etwork code acco
+00003c20: 7264 696e 6720 746f 2074 6865 2053 4545  rding to the SEE
+00003c30: 4420 7374 616e 6461 7264 2e0a 2020 2020  D standard..    
+00003c40: 2020 2020 636f 6465 3d6c 6f63 732e 696c      code=locs.il
+00003c50: 6f63 5b69 7374 615d 5b22 6e65 7477 6f72  oc[ista]["networ
+00003c60: 6b22 5d2c 0a20 2020 2020 2020 2073 7461  k"],.        sta
+00003c70: 7469 6f6e 733d 5b5d 2c0a 2020 2020 2020  tions=[],.      
+00003c80: 2020 6465 7363 7269 7074 696f 6e3d 2263    description="c
+00003c90: 7265 6174 6564 2066 726f 6d20 5341 4320  reated from SAC 
+00003ca0: 616e 6420 7265 7370 2066 696c 6573 222c  and resp files",
+00003cb0: 0a20 2020 2020 2020 2073 7461 7274 5f64  .        start_d
+00003cc0: 6174 653d 7374 6174 732e 7374 6172 7474  ate=stats.startt
+00003cd0: 696d 652c 0a20 2020 2029 0a0a 2020 2020  ime,.    )..    
+00003ce0: 7374 6120 3d20 5374 6174 696f 6e28 0a20  sta = Station(. 
+00003cf0: 2020 2020 2020 2023 2054 6869 7320 6973         # This is
+00003d00: 2074 6865 2073 7461 7469 6f6e 2063 6f64   the station cod
+00003d10: 6520 6163 636f 7264 696e 6720 746f 2074  e according to t
+00003d20: 6865 2053 4545 4420 7374 616e 6461 7264  he SEED standard
+00003d30: 2e0a 2020 2020 2020 2020 636f 6465 3d6c  ..        code=l
+00003d40: 6f63 732e 696c 6f63 5b69 7374 615d 5b22  ocs.iloc[ista]["
+00003d50: 7374 6174 696f 6e22 5d2c 0a20 2020 2020  station"],.     
+00003d60: 2020 206c 6174 6974 7564 653d 6c6f 6373     latitude=locs
+00003d70: 2e69 6c6f 635b 6973 7461 5d5b 226c 6174  .iloc[ista]["lat
+00003d80: 6974 7564 6522 5d2c 0a20 2020 2020 2020  itude"],.       
+00003d90: 206c 6f6e 6769 7475 6465 3d6c 6f63 732e   longitude=locs.
+00003da0: 696c 6f63 5b69 7374 615d 5b22 6c6f 6e67  iloc[ista]["long
+00003db0: 6974 7564 6522 5d2c 0a20 2020 2020 2020  itude"],.       
+00003dc0: 2065 6c65 7661 7469 6f6e 3d6c 6f63 732e   elevation=locs.
+00003dd0: 696c 6f63 5b69 7374 615d 5b22 656c 6576  iloc[ista]["elev
+00003de0: 6174 696f 6e22 5d2c 0a20 2020 2020 2020  ation"],.       
+00003df0: 2063 7265 6174 696f 6e5f 6461 7465 3d73   creation_date=s
+00003e00: 7461 7473 2e73 7461 7274 7469 6d65 2c0a  tats.starttime,.
+00003e10: 2020 2020 2020 2020 7369 7465 3d53 6974          site=Sit
+00003e20: 6528 6e61 6d65 3d22 4669 7273 7420 7374  e(name="First st
+00003e30: 6174 696f 6e22 292c 0a20 2020 2029 0a0a  ation"),.    )..
+00003e40: 2020 2020 6368 6120 3d20 4368 616e 6e65      cha = Channe
+00003e50: 6c28 0a20 2020 2020 2020 2063 6f64 653d  l(.        code=
+00003e60: 7374 6174 732e 6368 616e 6e65 6c2c 0a20  stats.channel,. 
+00003e70: 2020 2020 2020 206c 6f63 6174 696f 6e5f         location_
+00003e80: 636f 6465 3d73 7461 7473 2e6c 6f63 6174  code=stats.locat
+00003e90: 696f 6e2c 0a20 2020 2020 2020 206c 6174  ion,.        lat
+00003ea0: 6974 7564 653d 6c6f 6373 2e69 6c6f 635b  itude=locs.iloc[
+00003eb0: 6973 7461 5d5b 226c 6174 6974 7564 6522  ista]["latitude"
+00003ec0: 5d2c 0a20 2020 2020 2020 206c 6f6e 6769  ],.        longi
+00003ed0: 7475 6465 3d6c 6f63 732e 696c 6f63 5b69  tude=locs.iloc[i
+00003ee0: 7374 615d 5b22 6c6f 6e67 6974 7564 6522  sta]["longitude"
+00003ef0: 5d2c 0a20 2020 2020 2020 2065 6c65 7661  ],.        eleva
+00003f00: 7469 6f6e 3d6c 6f63 732e 696c 6f63 5b69  tion=locs.iloc[i
+00003f10: 7374 615d 5b22 656c 6576 6174 696f 6e22  sta]["elevation"
+00003f20: 5d2c 0a20 2020 2020 2020 2064 6570 7468  ],.        depth
+00003f30: 3d2d 6c6f 6373 2e69 6c6f 635b 6973 7461  =-locs.iloc[ista
+00003f40: 5d5b 2265 6c65 7661 7469 6f6e 225d 2c0a  ]["elevation"],.
+00003f50: 2020 2020 2020 2020 617a 696d 7574 683d          azimuth=
+00003f60: 302c 0a20 2020 2020 2020 2064 6970 3d30  0,.        dip=0
+00003f70: 2c0a 2020 2020 2020 2020 7361 6d70 6c65  ,.        sample
+00003f80: 5f72 6174 653d 7374 6174 732e 7361 6d70  _rate=stats.samp
+00003f90: 6c69 6e67 5f72 6174 652c 0a20 2020 2029  ling_rate,.    )
+00003fa0: 0a0a 2020 2020 7265 7370 6f6e 7365 203d  ..    response =
+00003fb0: 206f 6273 7079 2e63 6f72 652e 696e 7665   obspy.core.inve
+00003fc0: 6e74 6f72 792e 7265 7370 6f6e 7365 2e52  ntory.response.R
+00003fd0: 6573 706f 6e73 6528 290a 0a20 2020 2023  esponse()..    #
+00003fe0: 204e 6f77 2074 6965 2069 7420 616c 6c20   Now tie it all 
+00003ff0: 746f 6765 7468 6572 2e0a 2020 2020 6368  together..    ch
+00004000: 612e 7265 7370 6f6e 7365 203d 2072 6573  a.response = res
+00004010: 706f 6e73 650a 2020 2020 7374 612e 6368  ponse.    sta.ch
+00004020: 616e 6e65 6c73 2e61 7070 656e 6428 6368  annels.append(ch
+00004030: 6129 0a20 2020 206e 6574 2e73 7461 7469  a).    net.stati
+00004040: 6f6e 732e 6170 7065 6e64 2873 7461 290a  ons.append(sta).
+00004050: 2020 2020 696e 762e 6e65 7477 6f72 6b73      inv.networks
+00004060: 2e61 7070 656e 6428 6e65 7429 0a0a 2020  .append(net)..  
+00004070: 2020 7265 7475 726e 2069 6e76 0a0a 0a64    return inv...d
+00004080: 6566 2073 7461 5f69 6e66 6f5f 6672 6f6d  ef sta_info_from
+00004090: 5f69 6e76 2869 6e76 3a20 6f62 7370 792e  _inv(inv: obspy.
+000040a0: 636f 7265 2e69 6e76 656e 746f 7279 2e69  core.inventory.i
+000040b0: 6e76 656e 746f 7279 2e49 6e76 656e 746f  nventory.Invento
+000040c0: 7279 293a 0a20 2020 2022 2222 0a20 2020  ry):.    """.   
+000040d0: 2074 6869 7320 6675 6e63 7469 6f6e 206f   this function o
+000040e0: 7574 7075 7473 2073 7461 7469 6f6e 2069  utputs station i
+000040f0: 6e66 6f20 6672 6f6d 2074 6865 206f 6273  nfo from the obs
+00004100: 7079 2069 6e76 656e 746f 7279 206f 626a  py inventory obj
+00004110: 6563 740a 2020 2020 2875 7365 6420 696e  ect.    (used in
+00004120: 2053 3042 290a 2020 2020 5041 5241 4d45   S0B).    PARAME
+00004130: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+00004140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004150: 0a20 2020 2069 6e76 3a20 6f62 7370 7920  .    inv: obspy 
+00004160: 696e 7665 6e74 6f72 7920 6f62 6a65 6374  inventory object
+00004170: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+00004180: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00004190: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 7461  --------.    sta
+000041a0: 3a20 7374 6174 696f 6e20 6e61 6d65 0a20  : station name. 
+000041b0: 2020 206e 6574 3a20 6e65 746f 7772 6b20     net: netowrk 
+000041c0: 6e61 6d65 0a20 2020 206c 6f6e 3a20 6c6f  name.    lon: lo
+000041d0: 6e67 6974 7564 6520 6f66 2074 6865 2073  ngitude of the s
+000041e0: 7461 7469 6f6e 0a20 2020 206c 6174 3a20  tation.    lat: 
+000041f0: 6c61 7469 7475 6465 206f 6620 7468 6520  latitude of the 
+00004200: 7374 6174 696f 6e0a 2020 2020 656c 763a  station.    elv:
+00004210: 2065 6c65 7661 7469 6f6e 206f 6620 7468   elevation of th
+00004220: 6520 7374 6174 696f 6e0a 2020 2020 6c6f  e station.    lo
+00004230: 6361 7469 6f6e 3a20 6c6f 6361 7469 6f6e  cation: location
+00004240: 2063 6f64 6520 6f66 2074 6865 2073 7461   code of the sta
+00004250: 7469 6f6e 0a20 2020 2022 2222 0a20 2020  tion.    """.   
+00004260: 2023 206c 6f61 6420 6672 6f6d 2073 7461   # load from sta
+00004270: 7469 6f6e 2069 6e76 656e 746f 7279 0a20  tion inventory. 
+00004280: 2020 2073 7461 203d 2069 6e76 5b30 5d5b     sta = inv[0][
+00004290: 305d 2e63 6f64 650a 2020 2020 6e65 7420  0].code.    net 
+000042a0: 3d20 696e 765b 305d 2e63 6f64 650a 2020  = inv[0].code.  
+000042b0: 2020 6c6f 6e20 3d20 696e 765b 305d 5b30    lon = inv[0][0
+000042c0: 5d2e 6c6f 6e67 6974 7564 650a 2020 2020  ].longitude.    
+000042d0: 6c61 7420 3d20 696e 765b 305d 5b30 5d2e  lat = inv[0][0].
+000042e0: 6c61 7469 7475 6465 0a20 2020 2069 6620  latitude.    if 
+000042f0: 696e 765b 305d 5b30 5d2e 656c 6576 6174  inv[0][0].elevat
+00004300: 696f 6e3a 0a20 2020 2020 2020 2065 6c76  ion:.        elv
+00004310: 203d 2069 6e76 5b30 5d5b 305d 2e65 6c65   = inv[0][0].ele
+00004320: 7661 7469 6f6e 0a20 2020 2065 6c73 653a  vation.    else:
+00004330: 0a20 2020 2020 2020 2065 6c76 203d 2030  .        elv = 0
+00004340: 2e30 0a0a 2020 2020 6966 2069 6e76 5b30  .0..    if inv[0
+00004350: 5d5b 305d 5b30 5d2e 6c6f 6361 7469 6f6e  ][0][0].location
+00004360: 5f63 6f64 653a 0a20 2020 2020 2020 206c  _code:.        l
+00004370: 6f63 6174 696f 6e20 3d20 696e 765b 305d  ocation = inv[0]
+00004380: 5b30 5d5b 305d 2e6c 6f63 6174 696f 6e5f  [0][0].location_
+00004390: 636f 6465 0a20 2020 2065 6c73 653a 0a20  code.    else:. 
+000043a0: 2020 2020 2020 206c 6f63 6174 696f 6e20         location 
+000043b0: 3d20 2230 3022 0a0a 2020 2020 7265 7475  = "00"..    retu
+000043c0: 726e 2073 7461 2c20 6e65 742c 206c 6f6e  rn sta, net, lon
+000043d0: 2c20 6c61 742c 2065 6c76 2c20 6c6f 6361  , lat, elv, loca
+000043e0: 7469 6f6e 0a0a 0a64 6566 2063 7574 5f74  tion...def cut_t
+000043f0: 7261 6365 5f6d 616b 655f 7374 6174 2866  race_make_stat(f
+00004400: 635f 7061 7261 3a20 436f 6e66 6967 5061  c_para: ConfigPa
+00004410: 7261 6d65 7465 7273 2c20 6368 5f64 6174  rameters, ch_dat
+00004420: 613a 2043 6861 6e6e 656c 4461 7461 293a  a: ChannelData):
+00004430: 0a20 2020 2022 2222 0a20 2020 2074 6869  .    """.    thi
+00004440: 7320 6675 6e63 7469 6f6e 2063 7574 7320  s function cuts 
+00004450: 636f 6e74 696e 6f75 7320 6e6f 6973 6520  continous noise 
+00004460: 6461 7461 2069 6e74 6f20 7573 6572 2d64  data into user-d
+00004470: 6566 696e 6564 2073 6567 6d65 6e74 732c  efined segments,
+00004480: 2065 7374 696d 6174 6520 7468 6520 7374   estimate the st
+00004490: 6174 6973 7469 6373 206f 660a 2020 2020  atistics of.    
+000044a0: 6561 6368 2073 6567 6d65 6e74 2061 6e64  each segment and
+000044b0: 206b 6565 7020 7469 6d65 7374 616d 7020   keep timestamp 
+000044c0: 6f66 2065 6163 6820 7365 676d 656e 7420  of each segment 
+000044d0: 666f 7220 6c61 7465 7220 7573 652e 2028  for later use. (
+000044e0: 7573 6564 2069 6e20 5331 290a 2020 2020  used in S1).    
+000044f0: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+00004500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004510: 2d2d 2d2d 2d2d 0a20 2020 2066 6674 5f70  ------.    fft_p
+00004520: 6172 613a 2041 2064 6963 7469 6f6e 6172  ara: A dictionar
+00004530: 7920 636f 6e74 6169 6e69 6e67 2061 6c6c  y containing all
+00004540: 2066 6674 2061 6e64 2063 6320 7061 7261   fft and cc para
+00004550: 6d65 7465 7273 2e0a 2020 2020 736f 7572  meters..    sour
+00004560: 6365 3a20 6f62 7370 7920 7374 7265 616d  ce: obspy stream
+00004570: 206f 626a 6563 740a 2020 2020 5245 5455   object.    RETU
+00004580: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
+00004590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000045a0: 2020 2020 7472 6163 655f 7374 6453 3a20      trace_stdS: 
+000045b0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+000045c0: 6f6e 206f 6620 7468 6520 6e6f 6973 6520  on of the noise 
+000045d0: 616d 706c 6974 7564 6520 6f66 2065 6163  amplitude of eac
+000045e0: 6820 7365 676d 656e 740a 2020 2020 6461  h segment.    da
+000045f0: 7461 535f 743a 2020 2020 7469 6d65 7374  taS_t:    timest
+00004600: 616d 7073 206f 6620 6561 6368 2073 6567  amps of each seg
+00004610: 6d65 6e74 0a20 2020 2064 6174 6153 3a20  ment.    dataS: 
+00004620: 2020 2020 2032 4420 6d61 7472 6978 206f       2D matrix o
+00004630: 6620 7468 6520 7365 676d 656e 7465 6420  f the segmented 
+00004640: 6461 7461 0a20 2020 2022 2222 0a20 2020  data.    """.   
+00004650: 2023 2064 6566 696e 6520 7265 7475 726e   # define return
+00004660: 2076 6172 6961 626c 6573 2066 6972 7374   variables first
+00004670: 0a20 2020 2073 6f75 7263 655f 7061 7261  .    source_para
+00004680: 6d73 203d 205b 5d0a 2020 2020 6461 7461  ms = [].    data
+00004690: 535f 7420 3d20 5b5d 0a20 2020 2064 6174  S_t = [].    dat
+000046a0: 6153 203d 205b 5d0a 0a20 2020 2023 2075  aS = []..    # u
+000046b0: 7365 6675 6c20 7061 7261 6d65 7465 7273  seful parameters
+000046c0: 2066 6f72 2074 7261 6365 2073 6c69 6469   for trace slidi
+000046d0: 6e67 0a20 2020 206e 7365 6720 3d20 696e  ng.    nseg = in
+000046e0: 7428 6e70 2e66 6c6f 6f72 2828 6663 5f70  t(np.floor((fc_p
+000046f0: 6172 612e 696e 635f 686f 7572 7320 2f20  ara.inc_hours / 
+00004700: 3234 202a 2038 3634 3030 202d 2066 635f  24 * 86400 - fc_
+00004710: 7061 7261 2e63 635f 6c65 6e29 202f 2066  para.cc_len) / f
+00004720: 635f 7061 7261 2e73 7465 7029 290a 2020  c_para.step)).  
+00004730: 2020 7370 7320 3d20 696e 7428 6368 5f64    sps = int(ch_d
+00004740: 6174 612e 7361 6d70 6c69 6e67 5f72 6174  ata.sampling_rat
+00004750: 6529 0a20 2020 2073 7461 7274 7469 6d65  e).    starttime
+00004760: 203d 2063 685f 6461 7461 2e73 7461 7274   = ch_data.start
+00004770: 5f74 696d 6573 7461 6d70 0a20 2020 2023  _timestamp.    #
+00004780: 2063 6f70 7920 6461 7461 2069 6e74 6f20   copy data into 
+00004790: 6172 7261 790a 2020 2020 6461 7461 203d  array.    data =
+000047a0: 2063 685f 6461 7461 2e64 6174 610a 0a20   ch_data.data.. 
+000047b0: 2020 2023 2069 6620 7468 6520 6461 7461     # if the data
+000047c0: 2069 7320 7368 6f72 7465 7220 7468 616e   is shorter than
+000047d0: 2074 6865 2074 696d 2063 6875 6e63 6b2c   the tim chunck,
+000047e0: 2072 6574 7572 6e20 7a65 726f 2076 616c   return zero val
+000047f0: 7565 730a 2020 2020 6966 2064 6174 612e  ues.    if data.
+00004800: 7369 7a65 203c 2073 7073 202a 2066 635f  size < sps * fc_
+00004810: 7061 7261 2e69 6e63 5f68 6f75 7273 202a  para.inc_hours *
+00004820: 2033 3630 303a 0a20 2020 2020 2020 206c   3600:.        l
+00004830: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+00004840: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
+00004850: 2064 6174 6120 287b 6461 7461 2e73 697a   data ({data.siz
+00004860: 657d 2920 6973 2073 686f 7274 6572 2074  e}) is shorter t
+00004870: 6861 6e20 7468 6520 7469 6d65 2063 6875  han the time chu
+00004880: 6e6b 2028 7b73 7073 2a66 635f 7061 7261  nk ({sps*fc_para
+00004890: 2e69 6e63 5f68 6f75 7273 2a33 3630 307d  .inc_hours*3600}
+000048a0: 2922 0a20 2020 2020 2020 2020 2020 2022  )".            "
+000048b0: 2c20 7265 7475 726e 696e 6720 7a65 726f  , returning zero
+000048c0: 2076 616c 7565 732e 220a 2020 2020 2020   values.".      
+000048d0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+000048e0: 726e 2073 6f75 7263 655f 7061 7261 6d73  rn source_params
+000048f0: 2c20 6461 7461 535f 742c 2064 6174 6153  , dataS_t, dataS
+00004900: 0a0a 2020 2020 2320 7374 6174 6973 7469  ..    # statisti
+00004910: 6320 746f 2064 6574 6563 7420 7365 676d  c to detect segm
+00004920: 656e 7473 2074 6861 7420 6d61 7920 6265  ents that may be
+00004930: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00004940: 2065 6172 7468 7175 616b 6573 0a20 2020   earthquakes.   
+00004950: 2061 6c6c 5f6d 6164 5320 3d20 6d61 6428   all_madS = mad(
+00004960: 6461 7461 2920 2023 206d 6564 6961 6e20  data)  # median 
+00004970: 6162 736f 6c75 7465 2064 6576 6961 7469  absolute deviati
+00004980: 6f6e 206f 7665 7220 616c 6c20 6e6f 6973  on over all nois
+00004990: 6520 7769 6e64 6f77 0a20 2020 2061 6c6c  e window.    all
+000049a0: 5f73 7464 5320 3d20 6e70 2e73 7464 2864  _stdS = np.std(d
+000049b0: 6174 6129 2020 2320 7374 616e 6461 7264  ata)  # standard
+000049c0: 2064 6576 6961 7469 6f6e 206f 7665 7220   deviation over 
+000049d0: 616c 6c20 6e6f 6973 6520 7769 6e64 6f77  all noise window
+000049e0: 0a20 2020 2069 6620 616c 6c5f 6d61 6453  .    if all_madS
+000049f0: 203d 3d20 3020 6f72 2061 6c6c 5f73 7464   == 0 or all_std
+00004a00: 5320 3d3d 2030 206f 7220 6e70 2e69 736e  S == 0 or np.isn
+00004a10: 616e 2861 6c6c 5f6d 6164 5329 206f 7220  an(all_madS) or 
+00004a20: 6e70 2e69 736e 616e 2861 6c6c 5f73 7464  np.isnan(all_std
+00004a30: 5329 3a0a 2020 2020 2020 2020 6c6f 6767  S):.        logg
+00004a40: 6572 2e64 6562 7567 2822 636f 6e74 696e  er.debug("contin
+00004a50: 7565 2120 6d61 6453 206f 7220 7374 6453  ue! madS or stdS
+00004a60: 2065 7175 616c 7320 746f 2030 2066 6f72   equals to 0 for
+00004a70: 2025 7322 290a 2020 2020 2020 2020 7265   %s").        re
+00004a80: 7475 726e 2073 6f75 7263 655f 7061 7261  turn source_para
+00004a90: 6d73 2c20 6461 7461 535f 742c 2064 6174  ms, dataS_t, dat
+00004aa0: 6153 0a0a 2020 2020 2320 696e 6974 6961  aS..    # initia
+00004ab0: 6c69 7a65 2076 6172 6961 626c 6573 0a20  lize variables. 
+00004ac0: 2020 206e 7074 7320 3d20 696e 7428 6663     npts = int(fc
+00004ad0: 5f70 6172 612e 6363 5f6c 656e 202a 2073  _para.cc_len * s
+00004ae0: 7073 290a 2020 2020 2320 7472 6163 655f  ps).    # trace_
+00004af0: 6d61 6453 203d 206e 702e 7a65 726f 7328  madS = np.zeros(
+00004b00: 6e73 6567 2c64 7479 7065 3d6e 702e 666c  nseg,dtype=np.fl
+00004b10: 6f61 7433 3229 0a20 2020 2074 7261 6365  oat32).    trace
+00004b20: 5f73 7464 5320 3d20 6e70 2e7a 6572 6f73  _stdS = np.zeros
+00004b30: 286e 7365 672c 2064 7479 7065 3d6e 702e  (nseg, dtype=np.
+00004b40: 666c 6f61 7433 3229 0a20 2020 2064 6174  float32).    dat
+00004b50: 6153 203d 206e 702e 7a65 726f 7328 7368  aS = np.zeros(sh
+00004b60: 6170 653d 2869 6e74 286e 7365 6729 2c20  ape=(int(nseg), 
+00004b70: 696e 7428 6e70 7473 2929 2c20 6474 7970  int(npts)), dtyp
+00004b80: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
+00004b90: 2020 6461 7461 535f 7420 3d20 6e70 2e7a    dataS_t = np.z
+00004ba0: 6572 6f73 286e 7365 672c 2064 7479 7065  eros(nseg, dtype
+00004bb0: 3d6e 702e 666c 6f61 7433 3229 0a0a 2020  =np.float32)..  
+00004bc0: 2020 696e 6478 3120 3d20 300a 2020 2020    indx1 = 0.    
+00004bd0: 666f 7220 6973 6567 2069 6e20 7261 6e67  for iseg in rang
+00004be0: 6528 6e73 6567 293a 0a20 2020 2020 2020  e(nseg):.       
+00004bf0: 2069 6e64 7832 203d 2069 6e64 7831 202b   indx2 = indx1 +
+00004c00: 206e 7074 730a 2020 2020 2020 2020 6461   npts.        da
+00004c10: 7461 535b 6973 6567 5d20 3d20 6461 7461  taS[iseg] = data
+00004c20: 5b69 6e64 7831 3a69 6e64 7832 5d0a 2020  [indx1:indx2].  
+00004c30: 2020 2020 2020 2320 7472 6163 655f 6d61        # trace_ma
+00004c40: 6453 5b69 7365 675d 203d 2028 6e70 2e6d  dS[iseg] = (np.m
+00004c50: 6178 286e 702e 6162 7328 6461 7461 535b  ax(np.abs(dataS[
+00004c60: 6973 6567 5d29 292f 616c 6c5f 6d61 6453  iseg]))/all_madS
+00004c70: 290a 2020 2020 2020 2020 7472 6163 655f  ).        trace_
+00004c80: 7374 6453 5b69 7365 675d 203d 206e 702e  stdS[iseg] = np.
+00004c90: 6d61 7828 6e70 2e61 6273 2864 6174 6153  max(np.abs(dataS
+00004ca0: 5b69 7365 675d 2929 202f 2061 6c6c 5f73  [iseg])) / all_s
+00004cb0: 7464 530a 2020 2020 2020 2020 6461 7461  tdS.        data
+00004cc0: 535f 745b 6973 6567 5d20 3d20 7374 6172  S_t[iseg] = star
+00004cd0: 7474 696d 6520 2b20 6663 5f70 6172 612e  ttime + fc_para.
+00004ce0: 7374 6570 202a 2069 7365 670a 2020 2020  step * iseg.    
+00004cf0: 2020 2020 696e 6478 3120 3d20 696e 6478      indx1 = indx
+00004d00: 3120 2b20 696e 7428 6663 5f70 6172 612e  1 + int(fc_para.
+00004d10: 7374 6570 2920 2a20 7370 730a 0a20 2020  step) * sps..   
+00004d20: 2023 2032 4420 6172 7261 7920 7072 6f63   # 2D array proc
+00004d30: 6573 7369 6e67 0a20 2020 2064 6174 6153  essing.    dataS
+00004d40: 203d 2064 656d 6561 6e28 6461 7461 5329   = demean(dataS)
+00004d50: 0a20 2020 2064 6174 6153 203d 2064 6574  .    dataS = det
+00004d60: 7265 6e64 2864 6174 6153 290a 2020 2020  rend(dataS).    
+00004d70: 6461 7461 5320 3d20 7461 7065 7228 6461  dataS = taper(da
+00004d80: 7461 5329 0a0a 2020 2020 7265 7475 726e  taS)..    return
+00004d90: 2074 7261 6365 5f73 7464 532c 2064 6174   trace_stdS, dat
+00004da0: 6153 5f74 2c20 6461 7461 530a 0a0a 6465  aS_t, dataS...de
+00004db0: 6620 6e6f 6973 655f 7072 6f63 6573 7369  f noise_processi
+00004dc0: 6e67 2866 6674 5f70 6172 612c 2064 6174  ng(fft_para, dat
+00004dd0: 6153 293a 0a20 2020 2022 2222 0a20 2020  aS):.    """.   
+00004de0: 2074 6869 7320 6675 6e63 7469 6f6e 2070   this function p
+00004df0: 6572 666f 726d 7320 7469 6d65 2064 6f6d  erforms time dom
+00004e00: 6169 6e20 616e 6420 6672 6571 7565 6e63  ain and frequenc
+00004e10: 7920 646f 6d61 696e 206e 6f72 6d61 6c69  y domain normali
+00004e20: 7a61 7469 6f6e 2069 6620 6e65 6564 6564  zation if needed
+00004e30: 2e20 696e 2072 6561 6c20 6361 7365 2c20  . in real case, 
+00004e40: 7765 2070 7265 6665 7220 7573 6520 696e  we prefer use in
+00004e50: 636c 7564 650a 2020 2020 7468 6520 6e6f  clude.    the no
+00004e60: 726d 616c 697a 6174 696f 6e20 696e 2074  rmalization in t
+00004e70: 6865 2063 726f 7373 2d63 6f72 7265 616c  he cross-correal
+00004e80: 7469 6f6e 2073 7465 7073 2062 7920 7365  tion steps by se
+00004e90: 6c65 6374 696e 6720 636f 6865 7265 6e63  lecting coherenc
+00004ea0: 7920 6f72 2064 6563 6f6e 0a20 2020 2028  y or decon.    (
+00004eb0: 5072 6965 746f 2065 7420 616c 2c20 3230  Prieto et al, 20
+00004ec0: 3038 2c20 3230 3039 3b20 4465 6e6f 6c6c  08, 2009; Denoll
+00004ed0: 6520 6574 2061 6c2c 2032 3031 3329 0a20  e et al, 2013). 
+00004ee0: 2020 2050 4152 4d41 4554 4552 533a 0a20     PARMAETERS:. 
+00004ef0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00004f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00004f10: 6666 745f 7061 7261 3a20 6469 6374 696f  fft_para: dictio
+00004f20: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00004f30: 616c 6c20 7573 6566 756c 2076 6172 6961  all useful varia
+00004f40: 626c 6573 2075 7365 6420 666f 7220 6666  bles used for ff
+00004f50: 7420 616e 6420 6363 0a20 2020 2064 6174  t and cc.    dat
+00004f60: 6153 3a20 3244 206d 6174 7269 7820 6f66  aS: 2D matrix of
+00004f70: 2061 6c6c 2073 6567 6d65 6e74 6564 206e   all segmented n
+00004f80: 6f69 7365 2064 6174 610a 2020 2020 2320  oise data.    # 
+00004f90: 4f55 5450 5554 2056 4152 4941 424c 4553  OUTPUT VARIABLES
+00004fa0: 3a0a 2020 2020 736f 7572 6365 5f77 6869  :.    source_whi
+00004fb0: 7465 3a20 3244 206d 6174 7269 7820 6f66  te: 2D matrix of
+00004fc0: 2064 6174 6120 7370 6563 7472 610a 2020   data spectra.  
+00004fd0: 2020 2222 220a 2020 2020 2320 6c6f 6164    """.    # load
+00004fe0: 2070 6172 616d 6574 6572 7320 6669 7273   parameters firs
+00004ff0: 740a 2020 2020 7469 6d65 5f6e 6f72 6d20  t.    time_norm 
+00005000: 3d20 6666 745f 7061 7261 5b22 7469 6d65  = fft_para["time
+00005010: 5f6e 6f72 6d22 5d0a 2020 2020 6672 6571  _norm"].    freq
+00005020: 5f6e 6f72 6d20 3d20 6666 745f 7061 7261  _norm = fft_para
+00005030: 5b22 6672 6571 5f6e 6f72 6d22 5d0a 2020  ["freq_norm"].  
+00005040: 2020 736d 6f6f 7468 5f4e 203d 2066 6674    smooth_N = fft
+00005050: 5f70 6172 615b 2273 6d6f 6f74 685f 4e22  _para["smooth_N"
+00005060: 5d0a 2020 2020 4e20 3d20 6461 7461 532e  ].    N = dataS.
+00005070: 7368 6170 655b 305d 0a0a 2020 2020 2320  shape[0]..    # 
+00005080: 2d2d 2d2d 2d2d 746f 206e 6f72 6d61 6c69  ------to normali
+00005090: 7a65 2069 6e20 7469 6d65 206f 7220 6e6f  ze in time or no
+000050a0: 742d 2d2d 2d2d 2d0a 2020 2020 6966 2074  t------.    if t
+000050b0: 696d 655f 6e6f 726d 2021 3d20 226e 6f22  ime_norm != "no"
+000050c0: 3a0a 2020 2020 2020 2020 6966 2074 696d  :.        if tim
+000050d0: 655f 6e6f 726d 203d 3d20 226f 6e65 5f62  e_norm == "one_b
+000050e0: 6974 223a 2020 2320 7369 676e 206e 6f72  it":  # sign nor
+000050f0: 6d61 6c69 7a61 7469 6f6e 0a20 2020 2020  malization.     
+00005100: 2020 2020 2020 2077 6869 7465 203d 206e         white = n
+00005110: 702e 7369 676e 2864 6174 6153 290a 2020  p.sign(dataS).  
+00005120: 2020 2020 2020 656c 6966 2074 696d 655f        elif time_
+00005130: 6e6f 726d 203d 3d20 2272 6d61 223a 2020  norm == "rma":  
+00005140: 2320 7275 6e6e 696e 6720 6d65 616e 3a20  # running mean: 
+00005150: 6e6f 726d 616c 697a 6174 696f 6e20 6f76  normalization ov
+00005160: 6572 2073 6d6f 6f74 6865 6420 6162 736f  er smoothed abso
+00005170: 6c75 7465 2061 7665 7261 6765 0a20 2020  lute average.   
+00005180: 2020 2020 2020 2020 2077 6869 7465 203d           white =
+00005190: 206e 702e 7a65 726f 7328 7368 6170 653d   np.zeros(shape=
+000051a0: 6461 7461 532e 7368 6170 652c 2064 7479  dataS.shape, dty
+000051b0: 7065 3d64 6174 6153 2e64 7479 7065 290a  pe=dataS.dtype).
+000051c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000051d0: 6b6b 6b20 696e 2072 616e 6765 284e 293a  kkk in range(N):
+000051e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051f0: 2077 6869 7465 5b6b 6b6b 2c20 3a5d 203d   white[kkk, :] =
+00005200: 2064 6174 6153 5b6b 6b6b 2c20 3a5d 202f   dataS[kkk, :] /
+00005210: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
+00005220: 6273 2864 6174 6153 5b6b 6b6b 2c20 3a5d  bs(dataS[kkk, :]
+00005230: 292c 2073 6d6f 6f74 685f 4e29 0a0a 2020  ), smooth_N)..  
+00005240: 2020 656c 7365 3a20 2023 2064 6f6e 2774    else:  # don't
+00005250: 206e 6f72 6d61 6c69 7a65 0a20 2020 2020   normalize.     
+00005260: 2020 2077 6869 7465 203d 2064 6174 6153     white = dataS
+00005270: 0a0a 2020 2020 2320 2d2d 2d2d 2d74 6f20  ..    # -----to 
+00005280: 7768 6974 656e 206f 7220 6e6f 742d 2d2d  whiten or not---
+00005290: 2d2d 2d0a 2020 2020 6966 2066 7265 715f  ---.    if freq_
+000052a0: 6e6f 726d 2021 3d20 226e 6f22 3a0a 2020  norm != "no":.  
+000052b0: 2020 2020 2020 736f 7572 6365 5f77 6869        source_whi
+000052c0: 7465 203d 2077 6869 7465 6e28 7768 6974  te = whiten(whit
+000052d0: 652c 2066 6674 5f70 6172 6129 2020 2320  e, fft_para)  # 
+000052e0: 7768 6974 656e 2061 6e64 2072 6574 7572  whiten and retur
+000052f0: 6e20 4646 540a 2020 2020 656c 7365 3a0a  n FFT.    else:.
+00005300: 2020 2020 2020 2020 4e66 6674 203d 2069          Nfft = i
+00005310: 6e74 286e 6578 745f 6661 7374 5f6c 656e  nt(next_fast_len
+00005320: 2869 6e74 2864 6174 6153 2e73 6861 7065  (int(dataS.shape
+00005330: 5b31 5d29 2929 0a20 2020 2020 2020 2073  [1]))).        s
+00005340: 6f75 7263 655f 7768 6974 6520 3d20 7363  ource_white = sc
+00005350: 6970 792e 6666 7470 6163 6b2e 6666 7428  ipy.fftpack.fft(
+00005360: 7768 6974 652c 204e 6666 742c 2061 7869  white, Nfft, axi
+00005370: 733d 3129 2020 2320 7265 7475 726e 2046  s=1)  # return F
+00005380: 4654 0a0a 2020 2020 7265 7475 726e 2073  FT..    return s
+00005390: 6f75 7263 655f 7768 6974 650a 0a0a 6465  ource_white...de
+000053a0: 6620 736d 6f6f 7468 5f73 6f75 7263 655f  f smooth_source_
+000053b0: 7370 6563 7428 6363 5f70 6172 612c 2066  spect(cc_para, f
+000053c0: 6674 3129 3a0a 2020 2020 2222 220a 2020  ft1):.    """.  
+000053d0: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+000053e0: 736d 6f6f 7468 6573 2061 6d70 6c69 7475  smoothes amplitu
+000053f0: 6465 2073 7065 6374 7275 6d20 6f66 2074  de spectrum of t
+00005400: 6865 2032 4420 7370 6563 7472 616c 206d  he 2D spectral m
+00005410: 6174 7269 782e 2028 7573 6564 2069 6e20  atrix. (used in 
+00005420: 5331 290a 2020 2020 5041 5241 4d45 5445  S1).    PARAMETE
+00005430: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+00005440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00005450: 2020 6363 5f70 6172 613a 2064 6963 7469    cc_para: dicti
+00005460: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00005470: 2075 7365 6675 6c20 6363 2070 6172 616d   useful cc param
+00005480: 6574 6572 730a 2020 2020 6666 7431 3a20  eters.    fft1: 
+00005490: 2020 2073 6f75 7263 6520 7370 6563 7472     source spectr
+000054a0: 756d 206d 6174 7269 780a 0a20 2020 2052  um matrix..    R
+000054b0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+000054c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000054d0: 2d0a 2020 2020 7366 6674 313a 2063 6f6d  -.    sfft1: com
+000054e0: 706c 6578 206e 756d 7079 2061 7272 6179  plex numpy array
+000054f0: 2077 6974 6820 6e6f 726d 616c 697a 6564   with normalized
+00005500: 2073 7065 6374 7275 6d0a 2020 2020 2222   spectrum.    ""
+00005510: 220a 2020 2020 6363 5f6d 6574 686f 6420  ".    cc_method 
+00005520: 3d20 6363 5f70 6172 615b 2263 635f 6d65  = cc_para["cc_me
+00005530: 7468 6f64 225d 0a20 2020 2073 6d6f 6f74  thod"].    smoot
+00005540: 6873 7065 6374 5f4e 203d 2063 635f 7061  hspect_N = cc_pa
+00005550: 7261 5b22 736d 6f6f 7468 7370 6563 745f  ra["smoothspect_
+00005560: 4e22 5d0a 0a20 2020 2069 6620 6363 5f6d  N"]..    if cc_m
+00005570: 6574 686f 6420 3d3d 2022 6465 636f 6e76  ethod == "deconv
+00005580: 223a 0a20 2020 2020 2020 2023 202d 2d2d  ":.        # ---
+00005590: 2d2d 6e6f 726d 616c 697a 6520 7369 6e67  --normalize sing
+000055a0: 6c65 2d73 7461 7469 6f6e 2063 6320 746f  le-station cc to
+000055b0: 207a 2063 6f6d 706f 6e65 6e74 2d2d 2d2d   z component----
+000055c0: 2d0a 2020 2020 2020 2020 7465 6d70 203d  -.        temp =
+000055d0: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
+000055e0: 6273 2866 6674 3129 2c20 736d 6f6f 7468  bs(fft1), smooth
+000055f0: 7370 6563 745f 4e29 0a20 2020 2020 2020  spect_N).       
+00005600: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00005610: 2020 7366 6674 3120 3d20 6e70 2e63 6f6e    sfft1 = np.con
+00005620: 6a28 6666 7431 2920 2f20 7465 6d70 2a2a  j(fft1) / temp**
+00005630: 320a 2020 2020 2020 2020 6578 6365 7074  2.        except
+00005640: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
+00005650: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00005660: 6c75 6545 7272 6f72 2822 736d 6f6f 7468  lueError("smooth
+00005670: 6564 2073 7065 6374 7275 6d20 6861 7320  ed spectrum has 
+00005680: 7a65 726f 2076 616c 7565 7322 290a 0a20  zero values").. 
+00005690: 2020 2065 6c69 6620 6363 5f6d 6574 686f     elif cc_metho
+000056a0: 6420 3d3d 2022 636f 6865 7265 6e63 7922  d == "coherency"
+000056b0: 3a0a 2020 2020 2020 2020 7465 6d70 203d  :.        temp =
+000056c0: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
+000056d0: 6273 2866 6674 3129 2c20 736d 6f6f 7468  bs(fft1), smooth
+000056e0: 7370 6563 745f 4e29 0a20 2020 2020 2020  spect_N).       
+000056f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00005700: 2020 7366 6674 3120 3d20 6e70 2e63 6f6e    sfft1 = np.con
+00005710: 6a28 6666 7431 2920 2f20 7465 6d70 0a20  j(fft1) / temp. 
+00005720: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00005730: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+00005740: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00005750: 4572 726f 7228 2273 6d6f 6f74 6865 6420  Error("smoothed 
+00005760: 7370 6563 7472 756d 2068 6173 207a 6572  spectrum has zer
+00005770: 6f20 7661 6c75 6573 2229 0a0a 2020 2020  o values")..    
+00005780: 656c 6966 2063 635f 6d65 7468 6f64 203d  elif cc_method =
+00005790: 3d20 2278 636f 7272 223a 0a20 2020 2020  = "xcorr":.     
+000057a0: 2020 2073 6666 7431 203d 206e 702e 636f     sfft1 = np.co
+000057b0: 6e6a 2866 6674 3129 0a0a 2020 2020 656c  nj(fft1)..    el
+000057c0: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
+000057d0: 6520 5661 6c75 6545 7272 6f72 2822 6e6f  e ValueError("no
+000057e0: 2063 6f72 7265 6374 696f 6e20 636f 7272   correction corr
+000057f0: 656c 6174 696f 6e20 6d65 7468 6f64 2069  elation method i
+00005800: 7320 7365 6c65 6374 6564 2061 7420 4c35  s selected at L5
+00005810: 3922 290a 0a20 2020 2072 6574 7572 6e20  9")..    return 
+00005820: 7366 6674 310a 0a0a 6465 6620 636f 7272  sfft1...def corr
+00005830: 656c 6174 6528 6666 7431 5f73 6d6f 6f74  elate(fft1_smoot
+00005840: 6865 645f 6162 732c 2066 6674 322c 2044  hed_abs, fft2, D
+00005850: 2c20 4e66 6674 2c20 6461 7461 535f 7429  , Nfft, dataS_t)
+00005860: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+00005870: 6973 2066 756e 6374 696f 6e20 646f 6573  is function does
+00005880: 2074 6865 2063 726f 7373 2d63 6f72 7265   the cross-corre
+00005890: 6c61 7469 6f6e 2069 6e20 6672 6571 2064  lation in freq d
+000058a0: 6f6d 6169 6e20 616e 6420 6861 7320 7468  omain and has th
+000058b0: 6520 6f70 7469 6f6e 2074 6f20 6b65 6570  e option to keep
+000058c0: 2073 7562 2d73 7461 636b 7320 6f66 0a20   sub-stacks of. 
+000058d0: 2020 2074 6865 2063 726f 7373 2d63 6f72     the cross-cor
+000058e0: 7265 6c61 7469 6f6e 2069 6620 6e65 6564  relation if need
+000058f0: 6564 2e20 6974 2074 616b 6573 2061 6476  ed. it takes adv
+00005900: 616e 7461 6765 206f 6620 7468 6520 6c69  antage of the li
+00005910: 6e65 6172 2072 656c 6174 696f 6e73 6869  near relationshi
+00005920: 7020 6f66 2069 6666 742c 2073 6f20 7468  p of ifft, so th
+00005930: 6174 0a20 2020 2073 7461 636b 696e 6720  at.    stacking 
+00005940: 6973 2070 6572 666f 726d 6564 2069 6e20  is performed in 
+00005950: 7370 6563 7472 756d 2064 6f6d 6169 6e20  spectrum domain 
+00005960: 6669 7273 7420 746f 2072 6564 7563 6520  first to reduce 
+00005970: 7468 6520 746f 7461 6c20 6e75 6d62 6572  the total number
+00005980: 206f 6620 6966 6674 2e20 2875 7365 6420   of ifft. (used 
+00005990: 696e 2053 3129 0a20 2020 2050 4152 414d  in S1).    PARAM
+000059a0: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+000059b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000059c0: 0a20 2020 2066 6674 315f 736d 6f6f 7468  .    fft1_smooth
+000059d0: 6564 5f61 6273 3a20 736d 6f6f 7468 6564  ed_abs: smoothed
+000059e0: 2070 6f77 6572 2073 7065 6374 7261 6c20   power spectral 
+000059f0: 6465 6e73 6974 7920 6f66 2074 6865 2046  density of the F
+00005a00: 4654 2066 6f72 2074 6865 2073 6f75 7263  FT for the sourc
+00005a10: 6520 7374 6174 696f 6e0a 2020 2020 6666  e station.    ff
+00005a20: 7432 3a20 7261 7720 4646 5420 7370 6563  t2: raw FFT spec
+00005a30: 7472 756d 206f 6620 7468 6520 7265 6365  trum of the rece
+00005a40: 6976 6572 2073 7461 7469 6f6e 0a20 2020  iver station.   
+00005a50: 2044 3a20 6469 6374 696f 6e61 7279 2063   D: dictionary c
+00005a60: 6f6e 7461 696e 696e 6720 666f 6c6c 6f77  ontaining follow
+00005a70: 696e 6720 7061 7261 6d65 7465 7273 3a0a  ing parameters:.
+00005a80: 2020 2020 2020 2020 6d61 786c 6167 3a20          maxlag: 
+00005a90: 206d 6178 696d 756d 206c 6167 7320 746f   maximum lags to
+00005aa0: 206b 6565 7020 696e 2074 6865 2063 726f   keep in the cro
+00005ab0: 7373 2063 6f72 7265 6c61 7469 6f6e 0a20  ss correlation. 
+00005ac0: 2020 2020 2020 2064 743a 2020 2020 2020         dt:      
+00005ad0: 7361 6d70 6c69 6e67 2072 6174 6520 2869  sampling rate (i
+00005ae0: 6e20 7329 0a20 2020 2020 2020 206e 7769  n s).        nwi
+00005af0: 6e3a 2020 2020 6e75 6d62 6572 206f 6620  n:    number of 
+00005b00: 7365 676d 656e 7473 2069 6e20 7468 6520  segments in the 
+00005b10: 3244 206d 6174 7269 780a 2020 2020 2020  2D matrix.      
+00005b20: 2020 6d65 7468 6f64 3a20 2063 726f 7373    method:  cross
+00005b30: 2d63 6f72 7265 6c61 7469 6f6e 206d 6574  -correlation met
+00005b40: 686f 6473 2073 656c 6563 7465 6420 6279  hods selected by
+00005b50: 2074 6865 2075 7365 720a 2020 2020 2020   the user.      
+00005b60: 2020 6672 6571 6d69 6e3a 206d 696e 696d    freqmin: minim
+00005b70: 756d 2066 7265 7175 656e 6379 2028 487a  um frequency (Hz
+00005b80: 290a 2020 2020 2020 2020 6672 6571 6d61  ).        freqma
+00005b90: 783a 206d 6178 696d 756d 2066 7265 7175  x: maximum frequ
+00005ba0: 656e 6379 2028 487a 290a 2020 2020 4e66  ency (Hz).    Nf
+00005bb0: 6674 3a20 2020 206e 756d 6265 7220 6f66  ft:    number of
+00005bc0: 2066 7265 7175 656e 6379 2070 6f69 6e74   frequency point
+00005bd0: 7320 666f 7220 6966 6674 0a20 2020 2064  s for ifft.    d
+00005be0: 6174 6153 5f74 3a20 6d61 7472 6978 206f  ataS_t: matrix o
+00005bf0: 6620 6461 7465 7469 6d65 206f 626a 6563  f datetime objec
+00005c00: 742e 0a0a 2020 2020 5245 5455 524e 533a  t...    RETURNS:
+00005c10: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00005c20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
+00005c30: 5f63 6f72 723a 2031 4420 6f72 2032 4420  _corr: 1D or 2D 
+00005c40: 6d61 7472 6978 206f 6620 7468 6520 6176  matrix of the av
+00005c50: 6572 6167 6564 206f 7220 7375 622d 7374  eraged or sub-st
+00005c60: 6163 6b73 206f 6620 6372 6f73 732d 636f  acks of cross-co
+00005c70: 7272 656c 6174 696f 6e20 6675 6e63 7469  rrelation functi
+00005c80: 6f6e 7320 696e 2074 696d 6520 646f 6d61  ons in time doma
+00005c90: 696e 0a20 2020 2074 5f63 6f72 723a 2074  in.    t_corr: t
+00005ca0: 696d 6573 7461 6d70 2066 6f72 2065 6163  imestamp for eac
+00005cb0: 6820 7375 622d 7374 6163 6b20 6f72 2061  h sub-stack or a
+00005cc0: 7665 7261 6765 6420 6675 6e63 7469 6f6e  veraged function
+00005cd0: 0a20 2020 206e 5f63 6f72 723a 206e 756d  .    n_corr: num
+00005ce0: 6265 7220 6f66 2069 6e63 6c75 6465 6420  ber of included 
+00005cf0: 7365 676d 656e 7473 2066 6f72 2065 6163  segments for eac
+00005d00: 6820 7375 622d 7374 6163 6b20 6f72 2061  h sub-stack or a
+00005d10: 7665 7261 6765 6420 6675 6e63 7469 6f6e  veraged function
+00005d20: 0a0a 2020 2020 4d4f 4449 4649 4341 5449  ..    MODIFICATI
+00005d30: 4f4e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ONS:.    -------
+00005d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00005d50: 2020 206f 7574 7075 7420 7468 6520 6c69     output the li
+00005d60: 6e65 6172 2073 7461 636b 206f 6620 6561  near stack of ea
+00005d70: 6368 2074 696d 6520 6368 756e 6b20 6576  ch time chunk ev
+00005d80: 656e 2077 6865 6e20 7375 6273 7461 636b  en when substack
+00005d90: 2069 7320 7365 6c65 6374 6564 2028 6279   is selected (by
+00005da0: 2043 6865 6e67 7869 6e20 4041 7567 3230   Chengxin @Aug20
+00005db0: 3230 290a 2020 2020 2222 220a 2020 2020  20).    """.    
+00005dc0: 2320 2d2d 2d2d 6c6f 6164 2070 6172 616d  # ----load param
+00005dd0: 7465 7273 2d2d 2d2d 0a20 2020 2064 7420  ters----.    dt 
+00005de0: 3d20 445b 2264 7422 5d0a 2020 2020 6d61  = D["dt"].    ma
+00005df0: 786c 6167 203d 2044 5b22 6d61 786c 6167  xlag = D["maxlag
+00005e00: 225d 0a20 2020 206d 6574 686f 6420 3d20  "].    method = 
+00005e10: 445b 2263 635f 6d65 7468 6f64 225d 0a20  D["cc_method"]. 
+00005e20: 2020 2063 635f 6c65 6e20 3d20 445b 2263     cc_len = D["c
+00005e30: 635f 6c65 6e22 5d0a 2020 2020 7375 6273  c_len"].    subs
+00005e40: 7461 636b 203d 2044 5b22 7375 6273 7461  tack = D["substa
+00005e50: 636b 225d 0a20 2020 2073 7562 7374 6163  ck"].    substac
+00005e60: 6b5f 6c65 6e20 3d20 445b 2273 7562 7374  k_len = D["subst
+00005e70: 6163 6b5f 6c65 6e22 5d0a 2020 2020 736d  ack_len"].    sm
+00005e80: 6f6f 7468 7370 6563 745f 4e20 3d20 445b  oothspect_N = D[
+00005e90: 2273 6d6f 6f74 6873 7065 6374 5f4e 225d  "smoothspect_N"]
+00005ea0: 0a0a 2020 2020 6e77 696e 203d 2066 6674  ..    nwin = fft
+00005eb0: 315f 736d 6f6f 7468 6564 5f61 6273 2e73  1_smoothed_abs.s
+00005ec0: 6861 7065 5b30 5d0a 2020 2020 4e66 6674  hape[0].    Nfft
+00005ed0: 3220 3d20 6666 7431 5f73 6d6f 6f74 6865  2 = fft1_smoothe
+00005ee0: 645f 6162 732e 7368 6170 655b 315d 0a0a  d_abs.shape[1]..
+00005ef0: 2020 2020 2320 2d2d 2d2d 2d2d 636f 6e76      # ------conv
+00005f00: 6572 7420 616c 6c20 3244 2061 7272 6179  ert all 2D array
+00005f10: 7320 696e 746f 2031 4420 746f 2073 7065  s into 1D to spe
+00005f20: 6564 2075 702d 2d2d 2d2d 2d2d 2d0a 2020  ed up--------.  
+00005f30: 2020 636f 7272 203d 206e 702e 7a65 726f    corr = np.zero
+00005f40: 7328 6e77 696e 202a 204e 6666 7432 2c20  s(nwin * Nfft2, 
+00005f50: 6474 7970 653d 6e70 2e63 6f6d 706c 6578  dtype=np.complex
+00005f60: 3634 290a 2020 2020 636f 7272 203d 2066  64).    corr = f
+00005f70: 6674 315f 736d 6f6f 7468 6564 5f61 6273  ft1_smoothed_abs
+00005f80: 2e72 6573 6861 7065 280a 2020 2020 2020  .reshape(.      
+00005f90: 2020 6666 7431 5f73 6d6f 6f74 6865 645f    fft1_smoothed_
+00005fa0: 6162 732e 7369 7a65 2c0a 2020 2020 2920  abs.size,.    ) 
+00005fb0: 2a20 6666 7432 2e72 6573 6861 7065 280a  * fft2.reshape(.
+00005fc0: 2020 2020 2020 2020 6666 7432 2e73 697a          fft2.siz
+00005fd0: 652c 0a20 2020 2029 0a0a 2020 2020 6966  e,.    )..    if
+00005fe0: 206d 6574 686f 6420 3d3d 2022 636f 6865   method == "cohe
+00005ff0: 7265 6e63 7922 3a0a 2020 2020 2020 2020  rency":.        
+00006000: 7465 6d70 203d 206d 6f76 696e 675f 6176  temp = moving_av
+00006010: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
+00006020: 702e 6162 7328 0a20 2020 2020 2020 2020  p.abs(.         
+00006030: 2020 2020 2020 2066 6674 322e 7265 7368         fft2.resh
+00006040: 6170 6528 0a20 2020 2020 2020 2020 2020  ape(.           
+00006050: 2020 2020 2020 2020 2066 6674 322e 7369           fft2.si
+00006060: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+00006070: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00006080: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00006090: 2073 6d6f 6f74 6873 7065 6374 5f4e 2c0a   smoothspect_N,.
+000060a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000060b0: 2020 636f 7272 202f 3d20 7465 6d70 0a20    corr /= temp. 
+000060c0: 2020 2063 6f72 7220 3d20 636f 7272 2e72     corr = corr.r
+000060d0: 6573 6861 7065 286e 7769 6e2c 204e 6666  eshape(nwin, Nff
+000060e0: 7432 290a 0a20 2020 2069 6620 7375 6273  t2)..    if subs
+000060f0: 7461 636b 3a0a 2020 2020 2020 2020 6966  tack:.        if
+00006100: 2073 7562 7374 6163 6b5f 6c65 6e20 3d3d   substack_len ==
+00006110: 2063 635f 6c65 6e3a 0a20 2020 2020 2020   cc_len:.       
+00006120: 2020 2020 2023 2063 686f 6f73 6520 746f       # choose to
+00006130: 206b 6565 7020 616c 6c20 6666 7420 6461   keep all fft da
+00006140: 7461 2066 6f72 2061 2064 6179 0a20 2020  ta for a day.   
+00006150: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
+00006160: 3d20 6e70 2e7a 6572 6f73 2873 6861 7065  = np.zeros(shape
+00006170: 3d28 6e77 696e 2c20 4e66 6674 292c 2064  =(nwin, Nfft), d
+00006180: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00006190: 2020 2320 7374 6163 6b65 6420 636f 7272    # stacked corr
+000061a0: 656c 6174 696f 6e0a 2020 2020 2020 2020  elation.        
+000061b0: 2020 2020 616d 706d 6178 203d 206e 702e      ampmax = np.
+000061c0: 7a65 726f 7328 6e77 696e 2c20 6474 7970  zeros(nwin, dtyp
+000061d0: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
+000061e0: 2020 2020 2020 2020 2020 6e5f 636f 7272            n_corr
+000061f0: 203d 206e 702e 7a65 726f 7328 6e77 696e   = np.zeros(nwin
+00006200: 2c20 6474 7970 653d 6e70 2e69 6e74 3136  , dtype=np.int16
+00006210: 2920 2023 206e 756d 6265 7220 6f66 2063  )  # number of c
+00006220: 6f72 7265 6c61 7469 6f6e 7320 666f 7220  orrelations for 
+00006230: 6561 6368 2073 7562 7374 6163 6b0a 2020  each substack.  
+00006240: 2020 2020 2020 2020 2020 745f 636f 7272            t_corr
+00006250: 203d 2064 6174 6153 5f74 2020 2320 7469   = dataS_t  # ti
+00006260: 6d65 7374 616d 700a 2020 2020 2020 2020  mestamp.        
+00006270: 2020 2020 6372 6170 203d 206e 702e 7a65      crap = np.ze
+00006280: 726f 7328 4e66 6674 2c20 6474 7970 653d  ros(Nfft, dtype=
+00006290: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
+000062a0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000062b0: 696e 2072 616e 6765 286e 7769 6e29 3a0a  in range(nwin):.
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062d0: 6e5f 636f 7272 5b69 5d20 3d20 310a 2020  n_corr[i] = 1.  
+000062e0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+000062f0: 6170 5b3a 4e66 6674 325d 203d 2063 6f72  ap[:Nfft2] = cor
+00006300: 725b 692c 203a 5d0a 2020 2020 2020 2020  r[i, :].        
+00006310: 2020 2020 2020 2020 6372 6170 5b3a 4e66          crap[:Nf
+00006320: 6674 325d 203d 2063 7261 705b 3a4e 6666  ft2] = crap[:Nff
+00006330: 7432 5d20 2d20 6e70 2e6d 6561 6e28 6372  t2] - np.mean(cr
+00006340: 6170 5b3a 4e66 6674 325d 2920 2023 2072  ap[:Nfft2])  # r
+00006350: 656d 6f76 6520 7468 6520 6d65 616e 2069  emove the mean i
+00006360: 6e20 6672 6571 2064 6f6d 6169 6e20 2873  n freq domain (s
+00006370: 7069 6b65 2061 7420 743d 3029 0a20 2020  pike at t=0).   
+00006380: 2020 2020 2020 2020 2020 2020 2063 7261               cra
+00006390: 705b 2d28 4e66 6674 3229 202b 2031 203a  p[-(Nfft2) + 1 :
+000063a0: 5d20 3d20 6e70 2e66 6c69 7028 6e70 2e63  ] = np.flip(np.c
+000063b0: 6f6e 6a28 6372 6170 5b31 3a28 4e66 6674  onj(crap[1:(Nfft
+000063c0: 3229 5d29 2c20 6178 6973 3d30 290a 2020  2)]), axis=0).  
+000063d0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+000063e0: 6170 5b30 5d20 3d20 636f 6d70 6c65 7828  ap[0] = complex(
+000063f0: 302c 2030 290a 2020 2020 2020 2020 2020  0, 0).          
+00006400: 2020 2020 2020 735f 636f 7272 5b69 2c20        s_corr[i, 
+00006410: 3a5d 203d 206e 702e 7265 616c 286e 702e  :] = np.real(np.
+00006420: 6666 742e 6966 6674 7368 6966 7428 7363  fft.ifftshift(sc
+00006430: 6970 792e 6666 7470 6163 6b2e 6966 6674  ipy.fftpack.ifft
+00006440: 2863 7261 702c 204e 6666 742c 2061 7869  (crap, Nfft, axi
+00006450: 733d 3029 2929 0a0a 2020 2020 2020 2020  s=0)))..        
+00006460: 2020 2020 2320 7265 6d6f 7665 2061 626e      # remove abn
+00006470: 6f72 6d61 6c20 6461 7461 0a20 2020 2020  ormal data.     
+00006480: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
+00006490: 6e70 2e6d 6178 2873 5f63 6f72 722c 2061  np.max(s_corr, a
+000064a0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
+000064b0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
+000064c0: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
+000064d0: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
+000064e0: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
+000064f0: 3e20 3029 295b 305d 0a20 2020 2020 2020  > 0))[0].       
+00006500: 2020 2020 2073 5f63 6f72 7220 3d20 735f       s_corr = s_
+00006510: 636f 7272 5b74 696e 6478 2c20 3a5d 0a20  corr[tindx, :]. 
+00006520: 2020 2020 2020 2020 2020 2074 5f63 6f72             t_cor
+00006530: 7220 3d20 745f 636f 7272 5b74 696e 6478  r = t_corr[tindx
+00006540: 5d0a 2020 2020 2020 2020 2020 2020 6e5f  ].            n_
+00006550: 636f 7272 203d 206e 5f63 6f72 725b 7469  corr = n_corr[ti
+00006560: 6e64 785d 0a0a 2020 2020 2020 2020 656c  ndx]..        el
+00006570: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006580: 2320 6765 7420 7469 6d65 2069 6e66 6f72  # get time infor
+00006590: 6d61 7469 6f6e 0a20 2020 2020 2020 2020  mation.         
+000065a0: 2020 2054 746f 7461 6c20 3d20 6461 7461     Ttotal = data
+000065b0: 535f 745b 2d31 5d20 2d20 6461 7461 535f  S_t[-1] - dataS_
+000065c0: 745b 305d 2020 2320 746f 7461 6c20 6475  t[0]  # total du
+000065d0: 7261 7469 6f6e 206f 6620 7768 6174 2077  ration of what w
+000065e0: 6520 6861 7665 206e 6f77 0a20 2020 2020  e have now.     
+000065f0: 2020 2020 2020 2074 7374 6172 7420 3d20         tstart = 
+00006600: 6461 7461 535f 745b 305d 0a0a 2020 2020  dataS_t[0]..    
+00006610: 2020 2020 2020 2020 6e73 7461 636b 203d          nstack =
+00006620: 2069 6e74 286e 702e 726f 756e 6428 5474   int(np.round(Tt
+00006630: 6f74 616c 202f 2073 7562 7374 6163 6b5f  otal / substack_
+00006640: 6c65 6e29 290a 2020 2020 2020 2020 2020  len)).          
+00006650: 2020 616d 706d 6178 203d 206e 702e 7a65    ampmax = np.ze
+00006660: 726f 7328 6e73 7461 636b 2c20 6474 7970  ros(nstack, dtyp
+00006670: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
+00006680: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
+00006690: 203d 206e 702e 7a65 726f 7328 7368 6170   = np.zeros(shap
+000066a0: 653d 286e 7374 6163 6b2c 204e 6666 7429  e=(nstack, Nfft)
+000066b0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+000066c0: 3332 290a 2020 2020 2020 2020 2020 2020  32).            
+000066d0: 6e5f 636f 7272 203d 206e 702e 7a65 726f  n_corr = np.zero
+000066e0: 7328 6e73 7461 636b 2c20 6474 7970 653d  s(nstack, dtype=
+000066f0: 6e70 2e69 6e74 3136 290a 2020 2020 2020  np.int16).      
+00006700: 2020 2020 2020 745f 636f 7272 203d 206e        t_corr = n
+00006710: 702e 7a65 726f 7328 6e73 7461 636b 2c20  p.zeros(nstack, 
+00006720: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00006730: 290a 2020 2020 2020 2020 2020 2020 6372  ).            cr
+00006740: 6170 203d 206e 702e 7a65 726f 7328 4e66  ap = np.zeros(Nf
+00006750: 6674 2c20 6474 7970 653d 6e70 2e63 6f6d  ft, dtype=np.com
+00006760: 706c 6578 3634 290a 0a20 2020 2020 2020  plex64)..       
+00006770: 2020 2020 2066 6f72 2069 7374 6163 6b20       for istack 
+00006780: 696e 2072 616e 6765 286e 7374 6163 6b29  in range(nstack)
+00006790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000067a0: 2020 2320 6669 6e64 2074 6865 2069 6e64    # find the ind
+000067b0: 6578 6573 206f 6620 616c 6c20 6f66 2074  exes of all of t
+000067c0: 6865 2077 696e 646f 7773 2074 6861 7420  he windows that 
+000067d0: 7374 6172 7420 6f72 2065 6e64 2077 6974  start or end wit
+000067e0: 6869 6e0a 2020 2020 2020 2020 2020 2020  hin.            
+000067f0: 2020 2020 6974 696d 6520 3d20 6e70 2e77      itime = np.w
+00006800: 6865 7265 2828 6461 7461 535f 7420 3e3d  here((dataS_t >=
+00006810: 2074 7374 6172 7429 2026 2028 6461 7461   tstart) & (data
+00006820: 535f 7420 3c20 7473 7461 7274 202b 2073  S_t < tstart + s
+00006830: 7562 7374 6163 6b5f 6c65 6e29 295b 305d  ubstack_len))[0]
+00006840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006850: 2069 6620 6c65 6e28 6974 696d 6529 203d   if len(itime) =
+00006860: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00006870: 2020 2020 2020 2020 2074 7374 6172 7420           tstart 
+00006880: 2b3d 2073 7562 7374 6163 6b5f 6c65 6e0a  += substack_len.
+00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068a0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+000068b0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+000068c0: 6170 5b3a 4e66 6674 325d 203d 206e 702e  ap[:Nfft2] = np.
+000068d0: 6d65 616e 2863 6f72 725b 6974 696d 652c  mean(corr[itime,
+000068e0: 203a 5d2c 2061 7869 733d 3029 2020 2320   :], axis=0)  # 
+000068f0: 6c69 6e65 6172 2061 7665 7261 6765 206f  linear average o
+00006900: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
+00006910: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00006920: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
+00006930: 2063 7261 705b 3a4e 6666 7432 5d20 2d20   crap[:Nfft2] - 
+00006940: 6e70 2e6d 6561 6e28 6372 6170 5b3a 4e66  np.mean(crap[:Nf
+00006950: 6674 325d 2920 2023 2072 656d 6f76 6520  ft2])  # remove 
+00006960: 7468 6520 6d65 616e 2069 6e20 6672 6571  the mean in freq
+00006970: 2064 6f6d 6169 6e20 2873 7069 6b65 2061   domain (spike a
+00006980: 7420 743d 3029 0a20 2020 2020 2020 2020  t t=0).         
+00006990: 2020 2020 2020 2063 7261 705b 2d28 4e66         crap[-(Nf
+000069a0: 6674 3229 202b 2031 203a 5d20 3d20 6e70  ft2) + 1 :] = np
+000069b0: 2e66 6c69 7028 6e70 2e63 6f6e 6a28 6372  .flip(np.conj(cr
+000069c0: 6170 5b31 3a28 4e66 6674 3229 5d29 2c20  ap[1:(Nfft2)]), 
+000069d0: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+000069e0: 2020 2020 2020 2020 6372 6170 5b30 5d20          crap[0] 
+000069f0: 3d20 636f 6d70 6c65 7828 302c 2030 290a  = complex(0, 0).
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a10: 735f 636f 7272 5b69 7374 6163 6b2c 203a  s_corr[istack, :
+00006a20: 5d20 3d20 6e70 2e72 6561 6c28 6e70 2e66  ] = np.real(np.f
+00006a30: 6674 2e69 6666 7473 6869 6674 2873 6369  ft.ifftshift(sci
+00006a40: 7079 2e66 6674 7061 636b 2e69 6666 7428  py.fftpack.ifft(
+00006a50: 6372 6170 2c20 4e66 6674 2c20 6178 6973  crap, Nfft, axis
+00006a60: 3d30 2929 290a 2020 2020 2020 2020 2020  =0))).          
+00006a70: 2020 2020 2020 6e5f 636f 7272 5b69 7374        n_corr[ist
+00006a80: 6163 6b5d 203d 206c 656e 2869 7469 6d65  ack] = len(itime
+00006a90: 2920 2023 206e 756d 6265 7220 6f66 2077  )  # number of w
+00006aa0: 696e 646f 7773 2073 7461 636b 730a 2020  indows stacks.  
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 745f                t_
+00006ac0: 636f 7272 5b69 7374 6163 6b5d 203d 2074  corr[istack] = t
+00006ad0: 7374 6172 7420 2023 2073 6176 6520 7468  start  # save th
+00006ae0: 6520 7469 6d65 2073 7461 6d70 730a 2020  e time stamps.  
+00006af0: 2020 2020 2020 2020 2020 2020 2020 7473                ts
+00006b00: 7461 7274 202b 3d20 7375 6273 7461 636b  tart += substack
+00006b10: 5f6c 656e 0a20 2020 2020 2020 2020 2020  _len.           
+00006b20: 2020 2020 2023 2070 7269 6e74 2827 636f       # print('co
+00006b30: 7272 656c 6174 696f 6e20 646f 6e65 2061  rrelation done a
+00006b40: 6e64 2073 7461 636b 6564 2061 7420 7469  nd stacked at ti
+00006b50: 6d65 2025 7327 2025 2073 7472 2874 5f63  me %s' % str(t_c
+00006b60: 6f72 725b 6973 7461 636b 5d29 290a 0a20  orr[istack])).. 
+00006b70: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
+00006b80: 6f76 6520 6162 6e6f 726d 616c 2064 6174  ove abnormal dat
+00006b90: 610a 2020 2020 2020 2020 2020 2020 616d  a.            am
+00006ba0: 706d 6178 203d 206e 702e 6d61 7828 735f  pmax = np.max(s_
+00006bb0: 636f 7272 2c20 6178 6973 3d31 290a 2020  corr, axis=1).  
+00006bc0: 2020 2020 2020 2020 2020 7469 6e64 7820            tindx 
+00006bd0: 3d20 6e70 2e77 6865 7265 2828 616d 706d  = np.where((ampm
+00006be0: 6178 203c 2032 3020 2a20 6e70 2e6d 6564  ax < 20 * np.med
+00006bf0: 6961 6e28 616d 706d 6178 2929 2026 2028  ian(ampmax)) & (
+00006c00: 616d 706d 6178 203e 2030 2929 5b30 5d0a  ampmax > 0))[0].
+00006c10: 2020 2020 2020 2020 2020 2020 735f 636f              s_co
+00006c20: 7272 203d 2073 5f63 6f72 725b 7469 6e64  rr = s_corr[tind
+00006c30: 782c 203a 5d0a 2020 2020 2020 2020 2020  x, :].          
+00006c40: 2020 745f 636f 7272 203d 2074 5f63 6f72    t_corr = t_cor
+00006c50: 725b 7469 6e64 785d 0a20 2020 2020 2020  r[tindx].       
+00006c60: 2020 2020 206e 5f63 6f72 7220 3d20 6e5f       n_corr = n_
+00006c70: 636f 7272 5b74 696e 6478 5d0a 0a20 2020  corr[tindx]..   
+00006c80: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+00006c90: 2061 7665 7261 6765 2064 6169 6c79 2063   average daily c
+00006ca0: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
+00006cb0: 2066 756e 6374 696f 6e73 0a20 2020 2020   functions.     
+00006cc0: 2020 2061 6d70 6d61 7820 3d20 6e70 2e6d     ampmax = np.m
+00006cd0: 6178 2863 6f72 722c 2061 7869 733d 3129  ax(corr, axis=1)
+00006ce0: 0a20 2020 2020 2020 2074 696e 6478 203d  .        tindx =
+00006cf0: 206e 702e 7768 6572 6528 2861 6d70 6d61   np.where((ampma
+00006d00: 7820 3c20 3230 202a 206e 702e 6d65 6469  x < 20 * np.medi
+00006d10: 616e 2861 6d70 6d61 7829 2920 2620 2861  an(ampmax)) & (a
+00006d20: 6d70 6d61 7820 3e20 3029 295b 305d 0a20  mpmax > 0))[0]. 
+00006d30: 2020 2020 2020 206e 5f63 6f72 7220 3d20         n_corr = 
+00006d40: 6e77 696e 0a20 2020 2020 2020 2073 5f63  nwin.        s_c
+00006d50: 6f72 7220 3d20 6e70 2e7a 6572 6f73 284e  orr = np.zeros(N
+00006d60: 6666 742c 2064 7479 7065 3d6e 702e 666c  fft, dtype=np.fl
+00006d70: 6f61 7433 3229 0a20 2020 2020 2020 2074  oat32).        t
+00006d80: 5f63 6f72 7220 3d20 6461 7461 535f 745b  _corr = dataS_t[
+00006d90: 305d 0a20 2020 2020 2020 2063 7261 7020  0].        crap 
+00006da0: 3d20 6e70 2e7a 6572 6f73 284e 6666 742c  = np.zeros(Nfft,
+00006db0: 2064 7479 7065 3d6e 702e 636f 6d70 6c65   dtype=np.comple
+00006dc0: 7836 3429 0a20 2020 2020 2020 2063 7261  x64).        cra
+00006dd0: 705b 3a4e 6666 7432 5d20 3d20 6e70 2e6d  p[:Nfft2] = np.m
+00006de0: 6561 6e28 636f 7272 5b74 696e 6478 5d2c  ean(corr[tindx],
+00006df0: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+00006e00: 2063 7261 705b 3a4e 6666 7432 5d20 3d20   crap[:Nfft2] = 
+00006e10: 6372 6170 5b3a 4e66 6674 325d 202d 206e  crap[:Nfft2] - n
+00006e20: 702e 6d65 616e 2863 7261 705b 3a4e 6666  p.mean(crap[:Nff
+00006e30: 7432 5d2c 2061 7869 733d 3029 0a20 2020  t2], axis=0).   
+00006e40: 2020 2020 2063 7261 705b 2d28 4e66 6674       crap[-(Nfft
+00006e50: 3229 202b 2031 203a 5d20 3d20 6e70 2e66  2) + 1 :] = np.f
+00006e60: 6c69 7028 6e70 2e63 6f6e 6a28 6372 6170  lip(np.conj(crap
+00006e70: 5b31 3a28 4e66 6674 3229 5d29 2c20 6178  [1:(Nfft2)]), ax
+00006e80: 6973 3d30 290a 2020 2020 2020 2020 735f  is=0).        s_
+00006e90: 636f 7272 203d 206e 702e 7265 616c 286e  corr = np.real(n
+00006ea0: 702e 6666 742e 6966 6674 7368 6966 7428  p.fft.ifftshift(
+00006eb0: 7363 6970 792e 6666 7470 6163 6b2e 6966  scipy.fftpack.if
+00006ec0: 6674 2863 7261 702c 204e 6666 742c 2061  ft(crap, Nfft, a
+00006ed0: 7869 733d 3029 2929 0a0a 2020 2020 2320  xis=0)))..    # 
+00006ee0: 7472 696d 2074 6865 2043 4346 7320 696e  trim the CCFs in
+00006ef0: 205b 2d6d 6178 6c61 6720 6d61 786c 6167   [-maxlag maxlag
+00006f00: 5d0a 2020 2020 7420 3d20 6e70 2e61 7261  ].    t = np.ara
+00006f10: 6e67 6528 2d4e 6666 7432 202b 2031 2c20  nge(-Nfft2 + 1, 
+00006f20: 4e66 6674 3229 202a 2064 740a 2020 2020  Nfft2) * dt.    
+00006f30: 696e 6420 3d20 6e70 2e77 6865 7265 286e  ind = np.where(n
+00006f40: 702e 6162 7328 7429 203c 3d20 6d61 786c  p.abs(t) <= maxl
+00006f50: 6167 295b 305d 0a20 2020 2069 6620 735f  ag)[0].    if s_
+00006f60: 636f 7272 2e6e 6469 6d20 3d3d 2031 3a0a  corr.ndim == 1:.
+00006f70: 2020 2020 2020 2020 735f 636f 7272 203d          s_corr =
+00006f80: 2073 5f63 6f72 725b 696e 645d 0a20 2020   s_corr[ind].   
+00006f90: 2065 6c69 6620 735f 636f 7272 2e6e 6469   elif s_corr.ndi
+00006fa0: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
+00006fb0: 735f 636f 7272 203d 2073 5f63 6f72 725b  s_corr = s_corr[
+00006fc0: 3a2c 2069 6e64 5d0a 2020 2020 7265 7475  :, ind].    retu
+00006fd0: 726e 2073 5f63 6f72 722c 2074 5f63 6f72  rn s_corr, t_cor
+00006fe0: 722c 206e 5f63 6f72 720a 0a0a 6465 6620  r, n_corr...def 
+00006ff0: 636f 7272 656c 6174 655f 6e6f 6e6c 696e  correlate_nonlin
+00007000: 6561 725f 7374 6163 6b28 6666 7431 5f73  ear_stack(fft1_s
+00007010: 6d6f 6f74 6865 645f 6162 732c 2066 6674  moothed_abs, fft
+00007020: 322c 2044 2c20 4e66 6674 2c20 6461 7461  2, D, Nfft, data
+00007030: 535f 7429 3a0a 2020 2020 2222 220a 2020  S_t):.    """.  
+00007040: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+00007050: 646f 6573 2074 6865 2063 726f 7373 2d63  does the cross-c
+00007060: 6f72 7265 6c61 7469 6f6e 2069 6e20 6672  orrelation in fr
+00007070: 6571 2064 6f6d 6169 6e20 616e 6420 6861  eq domain and ha
+00007080: 7320 7468 6520 6f70 7469 6f6e 2074 6f20  s the option to 
+00007090: 6b65 6570 2073 7562 2d73 7461 636b 7320  keep sub-stacks 
+000070a0: 6f66 0a20 2020 2074 6865 2063 726f 7373  of.    the cross
+000070b0: 2d63 6f72 7265 6c61 7469 6f6e 2069 6620  -correlation if 
+000070c0: 6e65 6564 6564 2e20 6974 2074 616b 6573  needed. it takes
+000070d0: 2061 6476 616e 7461 6765 206f 6620 7468   advantage of th
+000070e0: 6520 6c69 6e65 6172 2072 656c 6174 696f  e linear relatio
+000070f0: 6e73 6869 7020 6f66 2069 6666 742c 2073  nship of ifft, s
+00007100: 6f20 7468 6174 0a20 2020 2073 7461 636b  o that.    stack
+00007110: 696e 6720 6973 2070 6572 666f 726d 6564  ing is performed
+00007120: 2069 6e20 7370 6563 7472 756d 2064 6f6d   in spectrum dom
+00007130: 6169 6e20 6669 7273 7420 746f 2072 6564  ain first to red
+00007140: 7563 6520 7468 6520 746f 7461 6c20 6e75  uce the total nu
+00007150: 6d62 6572 206f 6620 6966 6674 2e20 2875  mber of ifft. (u
+00007160: 7365 6420 696e 2053 3129 0a20 2020 2050  sed in S1).    P
+00007170: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
+00007180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007190: 2d2d 2d2d 0a20 2020 2066 6674 315f 736d  ----.    fft1_sm
+000071a0: 6f6f 7468 6564 5f61 6273 3a20 736d 6f6f  oothed_abs: smoo
+000071b0: 7468 6564 2070 6f77 6572 2073 7065 6374  thed power spect
+000071c0: 7261 6c20 6465 6e73 6974 7920 6f66 2074  ral density of t
+000071d0: 6865 2046 4654 2066 6f72 2074 6865 2073  he FFT for the s
+000071e0: 6f75 7263 6520 7374 6174 696f 6e0a 2020  ource station.  
+000071f0: 2020 6666 7432 3a20 7261 7720 4646 5420    fft2: raw FFT 
+00007200: 7370 6563 7472 756d 206f 6620 7468 6520  spectrum of the 
+00007210: 7265 6365 6976 6572 2073 7461 7469 6f6e  receiver station
+00007220: 0a20 2020 2044 3a20 6469 6374 696f 6e61  .    D: dictiona
+00007230: 7279 2063 6f6e 7461 696e 696e 6720 666f  ry containing fo
+00007240: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
+00007250: 7273 3a0a 2020 2020 2020 2020 6d61 786c  rs:.        maxl
+00007260: 6167 3a20 206d 6178 696d 756d 206c 6167  ag:  maximum lag
+00007270: 7320 746f 206b 6565 7020 696e 2074 6865  s to keep in the
+00007280: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
+00007290: 6f6e 0a20 2020 2020 2020 2064 743a 2020  on.        dt:  
+000072a0: 2020 2020 7361 6d70 6c69 6e67 2072 6174      sampling rat
+000072b0: 6520 2869 6e20 7329 0a20 2020 2020 2020  e (in s).       
+000072c0: 206e 7769 6e3a 2020 2020 6e75 6d62 6572   nwin:    number
+000072d0: 206f 6620 7365 676d 656e 7473 2069 6e20   of segments in 
+000072e0: 7468 6520 3244 206d 6174 7269 780a 2020  the 2D matrix.  
+000072f0: 2020 2020 2020 6d65 7468 6f64 3a20 2063        method:  c
+00007300: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
+00007310: 206d 6574 686f 6473 2073 656c 6563 7465   methods selecte
+00007320: 6420 6279 2074 6865 2075 7365 720a 2020  d by the user.  
+00007330: 2020 2020 2020 6672 6571 6d69 6e3a 206d        freqmin: m
+00007340: 696e 696d 756d 2066 7265 7175 656e 6379  inimum frequency
+00007350: 2028 487a 290a 2020 2020 2020 2020 6672   (Hz).        fr
+00007360: 6571 6d61 783a 206d 6178 696d 756d 2066  eqmax: maximum f
+00007370: 7265 7175 656e 6379 2028 487a 290a 2020  requency (Hz).  
+00007380: 2020 4e66 6674 3a20 2020 206e 756d 6265    Nfft:    numbe
+00007390: 7220 6f66 2066 7265 7175 656e 6379 2070  r of frequency p
+000073a0: 6f69 6e74 7320 666f 7220 6966 6674 0a20  oints for ifft. 
+000073b0: 2020 2064 6174 6153 5f74 3a20 6d61 7472     dataS_t: matr
+000073c0: 6978 206f 6620 6461 7465 7469 6d65 206f  ix of datetime o
+000073d0: 626a 6563 742e 0a20 2020 2052 4554 5552  bject..    RETUR
+000073e0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+000073f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00007400: 2020 735f 636f 7272 3a20 3144 206f 7220    s_corr: 1D or 
+00007410: 3244 206d 6174 7269 7820 6f66 2074 6865  2D matrix of the
+00007420: 2061 7665 7261 6765 6420 6f72 2073 7562   averaged or sub
+00007430: 2d73 7461 636b 7320 6f66 2063 726f 7373  -stacks of cross
+00007440: 2d63 6f72 7265 6c61 7469 6f6e 2066 756e  -correlation fun
+00007450: 6374 696f 6e73 2069 6e20 7469 6d65 2064  ctions in time d
+00007460: 6f6d 6169 6e0a 2020 2020 745f 636f 7272  omain.    t_corr
+00007470: 3a20 7469 6d65 7374 616d 7020 666f 7220  : timestamp for 
+00007480: 6561 6368 2073 7562 2d73 7461 636b 206f  each sub-stack o
+00007490: 7220 6176 6572 6167 6564 2066 756e 6374  r averaged funct
+000074a0: 696f 6e0a 2020 2020 6e5f 636f 7272 3a20  ion.    n_corr: 
+000074b0: 6e75 6d62 6572 206f 6620 696e 636c 7564  number of includ
+000074c0: 6564 2073 6567 6d65 6e74 7320 666f 7220  ed segments for 
+000074d0: 6561 6368 2073 7562 2d73 7461 636b 206f  each sub-stack o
+000074e0: 7220 6176 6572 6167 6564 2066 756e 6374  r averaged funct
+000074f0: 696f 6e0a 2020 2020 2222 220a 2020 2020  ion.    """.    
+00007500: 2320 2d2d 2d2d 6c6f 6164 2070 6172 616d  # ----load param
+00007510: 7465 7273 2d2d 2d2d 0a20 2020 2064 7420  ters----.    dt 
+00007520: 3d20 445b 2264 7422 5d0a 2020 2020 6d61  = D["dt"].    ma
+00007530: 786c 6167 203d 2044 5b22 6d61 786c 6167  xlag = D["maxlag
+00007540: 225d 0a20 2020 206d 6574 686f 6420 3d20  "].    method = 
+00007550: 445b 2263 635f 6d65 7468 6f64 225d 0a20  D["cc_method"]. 
+00007560: 2020 2063 635f 6c65 6e20 3d20 445b 2263     cc_len = D["c
+00007570: 635f 6c65 6e22 5d0a 2020 2020 7375 6273  c_len"].    subs
+00007580: 7461 636b 203d 2044 5b22 7375 6273 7461  tack = D["substa
+00007590: 636b 225d 0a20 2020 2073 7461 636b 5f6d  ck"].    stack_m
+000075a0: 6574 686f 6420 3d20 445b 2273 7461 636b  ethod = D["stack
+000075b0: 5f6d 6574 686f 6422 5d0a 2020 2020 7375  _method"].    su
+000075c0: 6273 7461 636b 5f6c 656e 203d 2044 5b22  bstack_len = D["
+000075d0: 7375 6273 7461 636b 5f6c 656e 225d 0a20  substack_len"]. 
+000075e0: 2020 2073 6d6f 6f74 6873 7065 6374 5f4e     smoothspect_N
+000075f0: 203d 2044 5b22 736d 6f6f 7468 7370 6563   = D["smoothspec
+00007600: 745f 4e22 5d0a 0a20 2020 206e 7769 6e20  t_N"]..    nwin 
+00007610: 3d20 6666 7431 5f73 6d6f 6f74 6865 645f  = fft1_smoothed_
+00007620: 6162 732e 7368 6170 655b 305d 0a20 2020  abs.shape[0].   
+00007630: 204e 6666 7432 203d 2066 6674 315f 736d   Nfft2 = fft1_sm
+00007640: 6f6f 7468 6564 5f61 6273 2e73 6861 7065  oothed_abs.shape
+00007650: 5b31 5d0a 0a20 2020 2023 202d 2d2d 2d2d  [1]..    # -----
+00007660: 2d63 6f6e 7665 7274 2061 6c6c 2032 4420  -convert all 2D 
+00007670: 6172 7261 7973 2069 6e74 6f20 3144 2074  arrays into 1D t
+00007680: 6f20 7370 6565 6420 7570 2d2d 2d2d 2d2d  o speed up------
+00007690: 2d2d 0a20 2020 2063 6f72 7220 3d20 6e70  --.    corr = np
+000076a0: 2e7a 6572 6f73 286e 7769 6e20 2a20 4e66  .zeros(nwin * Nf
+000076b0: 6674 322c 2064 7479 7065 3d6e 702e 636f  ft2, dtype=np.co
+000076c0: 6d70 6c65 7836 3429 0a20 2020 2063 6f72  mplex64).    cor
+000076d0: 7220 3d20 6666 7431 5f73 6d6f 6f74 6865  r = fft1_smoothe
+000076e0: 645f 6162 732e 7265 7368 6170 6528 0a20  d_abs.reshape(. 
+000076f0: 2020 2020 2020 2066 6674 315f 736d 6f6f         fft1_smoo
+00007700: 7468 6564 5f61 6273 2e73 697a 652c 0a20  thed_abs.size,. 
+00007710: 2020 2029 202a 2066 6674 322e 7265 7368     ) * fft2.resh
+00007720: 6170 6528 0a20 2020 2020 2020 2066 6674  ape(.        fft
+00007730: 322e 7369 7a65 2c0a 2020 2020 290a 0a20  2.size,.    ).. 
+00007740: 2020 2023 206e 6f72 6d61 6c69 7a65 2062     # normalize b
+00007750: 7920 7265 6365 6976 6572 2073 7065 6374  y receiver spect
+00007760: 7261 6c20 666f 7220 636f 6865 7265 6e63  ral for coherenc
+00007770: 790a 2020 2020 6966 206d 6574 686f 6420  y.    if method 
+00007780: 3d3d 2022 636f 6865 7265 6e63 7922 3a0a  == "coherency":.
+00007790: 2020 2020 2020 2020 7465 6d70 203d 206d          temp = m
+000077a0: 6f76 696e 675f 6176 6528 0a20 2020 2020  oving_ave(.     
+000077b0: 2020 2020 2020 206e 702e 6162 7328 0a20         np.abs(. 
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000077d0: 6674 322e 7265 7368 6170 6528 0a20 2020  ft2.reshape(.   
+000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077f0: 2066 6674 322e 7369 7a65 2c0a 2020 2020   fft2.size,.    
+00007800: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00007810: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00007820: 2020 2020 2020 2020 2073 6d6f 6f74 6873           smooths
+00007830: 7065 6374 5f4e 2c0a 2020 2020 2020 2020  pect_N,.        
+00007840: 290a 2020 2020 2020 2020 636f 7272 202f  ).        corr /
+00007850: 3d20 7465 6d70 0a20 2020 2063 6f72 7220  = temp.    corr 
+00007860: 3d20 636f 7272 2e72 6573 6861 7065 286e  = corr.reshape(n
+00007870: 7769 6e2c 204e 6666 7432 290a 0a20 2020  win, Nfft2)..   
+00007880: 2023 2074 7261 6e73 666f 726d 2062 6163   # transform bac
+00007890: 6b20 746f 2074 696d 6520 646f 6d61 696e  k to time domain
+000078a0: 2077 6176 6566 6f72 6d73 0a20 2020 2073   waveforms.    s
+000078b0: 5f63 6f72 7220 3d20 6e70 2e7a 6572 6f73  _corr = np.zeros
+000078c0: 2873 6861 7065 3d28 6e77 696e 2c20 4e66  (shape=(nwin, Nf
+000078d0: 6674 292c 2064 7479 7065 3d6e 702e 666c  ft), dtype=np.fl
+000078e0: 6f61 7433 3229 2020 2320 7374 6163 6b65  oat32)  # stacke
+000078f0: 6420 636f 7272 656c 6174 696f 6e0a 2020  d correlation.  
+00007900: 2020 616d 706d 6178 203d 206e 702e 7a65    ampmax = np.ze
+00007910: 726f 7328 6e77 696e 2c20 6474 7970 653d  ros(nwin, dtype=
+00007920: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
+00007930: 6e5f 636f 7272 203d 206e 702e 7a65 726f  n_corr = np.zero
+00007940: 7328 6e77 696e 2c20 6474 7970 653d 6e70  s(nwin, dtype=np
+00007950: 2e69 6e74 3136 2920 2023 206e 756d 6265  .int16)  # numbe
+00007960: 7220 6f66 2063 6f72 7265 6c61 7469 6f6e  r of correlation
+00007970: 7320 666f 7220 6561 6368 2073 7562 7374  s for each subst
+00007980: 6163 6b0a 2020 2020 745f 636f 7272 203d  ack.    t_corr =
+00007990: 2064 6174 6153 5f74 2020 2320 7469 6d65   dataS_t  # time
+000079a0: 7374 616d 700a 2020 2020 6372 6170 203d  stamp.    crap =
+000079b0: 206e 702e 7a65 726f 7328 4e66 6674 2c20   np.zeros(Nfft, 
+000079c0: 6474 7970 653d 6e70 2e63 6f6d 706c 6578  dtype=np.complex
+000079d0: 3634 290a 2020 2020 666f 7220 6920 696e  64).    for i in
+000079e0: 2072 616e 6765 286e 7769 6e29 3a0a 2020   range(nwin):.  
+000079f0: 2020 2020 2020 6e5f 636f 7272 5b69 5d20        n_corr[i] 
+00007a00: 3d20 310a 2020 2020 2020 2020 6372 6170  = 1.        crap
+00007a10: 5b3a 4e66 6674 325d 203d 2063 6f72 725b  [:Nfft2] = corr[
+00007a20: 692c 203a 5d0a 2020 2020 2020 2020 6372  i, :].        cr
+00007a30: 6170 5b3a 4e66 6674 325d 203d 2063 7261  ap[:Nfft2] = cra
+00007a40: 705b 3a4e 6666 7432 5d20 2d20 6e70 2e6d  p[:Nfft2] - np.m
+00007a50: 6561 6e28 6372 6170 5b3a 4e66 6674 325d  ean(crap[:Nfft2]
+00007a60: 2920 2023 2072 656d 6f76 6520 7468 6520  )  # remove the 
+00007a70: 6d65 616e 2069 6e20 6672 6571 2064 6f6d  mean in freq dom
+00007a80: 6169 6e20 2873 7069 6b65 2061 7420 743d  ain (spike at t=
+00007a90: 3029 0a20 2020 2020 2020 2063 7261 705b  0).        crap[
+00007aa0: 2d28 4e66 6674 3229 202b 2031 203a 5d20  -(Nfft2) + 1 :] 
+00007ab0: 3d20 6e70 2e66 6c69 7028 6e70 2e63 6f6e  = np.flip(np.con
+00007ac0: 6a28 6372 6170 5b31 3a28 4e66 6674 3229  j(crap[1:(Nfft2)
+00007ad0: 5d29 2c20 6178 6973 3d30 290a 2020 2020  ]), axis=0).    
+00007ae0: 2020 2020 6372 6170 5b30 5d20 3d20 636f      crap[0] = co
+00007af0: 6d70 6c65 7828 302c 2030 290a 2020 2020  mplex(0, 0).    
+00007b00: 2020 2020 735f 636f 7272 5b69 2c20 3a5d      s_corr[i, :]
+00007b10: 203d 206e 702e 7265 616c 286e 702e 6666   = np.real(np.ff
+00007b20: 742e 6966 6674 7368 6966 7428 7363 6970  t.ifftshift(scip
+00007b30: 792e 6666 7470 6163 6b2e 6966 6674 2863  y.fftpack.ifft(c
+00007b40: 7261 702c 204e 6666 742c 2061 7869 733d  rap, Nfft, axis=
+00007b50: 3029 2929 0a0a 2020 2020 6e73 5f63 6f72  0)))..    ns_cor
+00007b60: 7220 3d20 735f 636f 7272 0a20 2020 2066  r = s_corr.    f
+00007b70: 6f72 2069 6969 2069 6e20 7261 6e67 6528  or iii in range(
+00007b80: 6e73 5f63 6f72 722e 7368 6170 655b 305d  ns_corr.shape[0]
+00007b90: 293a 0a20 2020 2020 2020 206e 735f 636f  ):.        ns_co
+00007ba0: 7272 5b69 6969 5d20 2f3d 206e 702e 6d61  rr[iii] /= np.ma
+00007bb0: 7828 6e70 2e61 6273 286e 735f 636f 7272  x(np.abs(ns_corr
+00007bc0: 5b69 6969 5d29 290a 0a20 2020 2069 6620  [iii]))..    if 
+00007bd0: 7375 6273 7461 636b 3a0a 2020 2020 2020  substack:.      
+00007be0: 2020 6966 2073 7562 7374 6163 6b5f 6c65    if substack_le
+00007bf0: 6e20 3d3d 2063 635f 6c65 6e3a 0a20 2020  n == cc_len:.   
+00007c00: 2020 2020 2020 2020 2023 2072 656d 6f76           # remov
+00007c10: 6520 6162 6e6f 726d 616c 2064 6174 610a  e abnormal data.
+00007c20: 2020 2020 2020 2020 2020 2020 616d 706d              ampm
+00007c30: 6178 203d 206e 702e 6d61 7828 735f 636f  ax = np.max(s_co
+00007c40: 7272 2c20 6178 6973 3d31 290a 2020 2020  rr, axis=1).    
+00007c50: 2020 2020 2020 2020 7469 6e64 7820 3d20          tindx = 
+00007c60: 6e70 2e77 6865 7265 2828 616d 706d 6178  np.where((ampmax
+00007c70: 203c 2032 3020 2a20 6e70 2e6d 6564 6961   < 20 * np.media
+00007c80: 6e28 616d 706d 6178 2929 2026 2028 616d  n(ampmax)) & (am
+00007c90: 706d 6178 203e 2030 2929 5b30 5d0a 2020  pmax > 0))[0].  
+00007ca0: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
+00007cb0: 203d 2073 5f63 6f72 725b 7469 6e64 782c   = s_corr[tindx,
+00007cc0: 203a 5d0a 2020 2020 2020 2020 2020 2020   :].            
+00007cd0: 745f 636f 7272 203d 2074 5f63 6f72 725b  t_corr = t_corr[
+00007ce0: 7469 6e64 785d 0a20 2020 2020 2020 2020  tindx].         
+00007cf0: 2020 206e 5f63 6f72 7220 3d20 6e5f 636f     n_corr = n_co
+00007d00: 7272 5b74 696e 6478 5d0a 0a20 2020 2020  rr[tindx]..     
+00007d10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007d20: 2020 2020 2023 2067 6574 2074 696d 6520       # get time 
+00007d30: 696e 666f 726d 6174 696f 6e0a 2020 2020  information.    
+00007d40: 2020 2020 2020 2020 5474 6f74 616c 203d          Ttotal =
+00007d50: 2064 6174 6153 5f74 5b2d 315d 202d 2064   dataS_t[-1] - d
+00007d60: 6174 6153 5f74 5b30 5d20 2023 2074 6f74  ataS_t[0]  # tot
+00007d70: 616c 2064 7572 6174 696f 6e20 6f66 2077  al duration of w
+00007d80: 6861 7420 7765 2068 6176 6520 6e6f 770a  hat we have now.
+00007d90: 2020 2020 2020 2020 2020 2020 7473 7461              tsta
+00007da0: 7274 203d 2064 6174 6153 5f74 5b30 5d0a  rt = dataS_t[0].
+00007db0: 0a20 2020 2020 2020 2020 2020 206e 7374  .            nst
+00007dc0: 6163 6b20 3d20 696e 7428 6e70 2e72 6f75  ack = int(np.rou
+00007dd0: 6e64 2854 746f 7461 6c20 2f20 7375 6273  nd(Ttotal / subs
+00007de0: 7461 636b 5f6c 656e 2929 0a20 2020 2020  tack_len)).     
+00007df0: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
+00007e00: 6e70 2e7a 6572 6f73 286e 7374 6163 6b2c  np.zeros(nstack,
+00007e10: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00007e20: 3229 0a20 2020 2020 2020 2020 2020 2073  2).            s
+00007e30: 5f63 6f72 7220 3d20 6e70 2e7a 6572 6f73  _corr = np.zeros
+00007e40: 2873 6861 7065 3d28 6e73 7461 636b 2c20  (shape=(nstack, 
+00007e50: 4e66 6674 292c 2064 7479 7065 3d6e 702e  Nfft), dtype=np.
+00007e60: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
+00007e70: 2020 2020 206e 5f63 6f72 7220 3d20 6e70       n_corr = np
+00007e80: 2e7a 6572 6f73 286e 7374 6163 6b2c 2064  .zeros(nstack, d
+00007e90: 7479 7065 3d6e 702e 696e 7429 0a20 2020  type=np.int).   
+00007ea0: 2020 2020 2020 2020 2074 5f63 6f72 7220           t_corr 
+00007eb0: 3d20 6e70 2e7a 6572 6f73 286e 7374 6163  = np.zeros(nstac
+00007ec0: 6b2c 2064 7479 7065 3d6e 702e 666c 6f61  k, dtype=np.floa
+00007ed0: 7429 0a20 2020 2020 2020 2020 2020 2063  t).            c
+00007ee0: 7261 7020 3d20 6e70 2e7a 6572 6f73 284e  rap = np.zeros(N
+00007ef0: 6666 742c 2064 7479 7065 3d6e 702e 636f  fft, dtype=np.co
+00007f00: 6d70 6c65 7836 3429 0a0a 2020 2020 2020  mplex64)..      
+00007f10: 2020 2020 2020 666f 7220 6973 7461 636b        for istack
+00007f20: 2069 6e20 7261 6e67 6528 6e73 7461 636b   in range(nstack
+00007f30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00007f40: 2020 2023 2066 696e 6420 7468 6520 696e     # find the in
+00007f50: 6465 7865 7320 6f66 2061 6c6c 206f 6620  dexes of all of 
+00007f60: 7468 6520 7769 6e64 6f77 7320 7468 6174  the windows that
+00007f70: 2073 7461 7274 206f 7220 656e 6420 7769   start or end wi
+00007f80: 7468 696e 0a20 2020 2020 2020 2020 2020  thin.           
+00007f90: 2020 2020 2069 7469 6d65 203d 206e 702e       itime = np.
+00007fa0: 7768 6572 6528 2864 6174 6153 5f74 203e  where((dataS_t >
+00007fb0: 3d20 7473 7461 7274 2920 2620 2864 6174  = tstart) & (dat
+00007fc0: 6153 5f74 203c 2074 7374 6172 7420 2b20  aS_t < tstart + 
+00007fd0: 7375 6273 7461 636b 5f6c 656e 2929 5b30  substack_len))[0
+00007fe0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00007ff0: 2020 6966 206c 656e 2869 7469 6d65 2920    if len(itime) 
+00008000: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00008010: 2020 2020 2020 2020 2020 7473 7461 7274            tstart
+00008020: 202b 3d20 7375 6273 7461 636b 5f6c 656e   += substack_len
+00008030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008040: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00008050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008060: 7261 705b 3a4e 6666 7432 5d20 3d20 6e70  rap[:Nfft2] = np
+00008070: 2e6d 6561 6e28 636f 7272 5b69 7469 6d65  .mean(corr[itime
+00008080: 2c20 3a5d 2c20 6178 6973 3d30 2920 2023  , :], axis=0)  #
+00008090: 206c 696e 6561 7220 6176 6572 6167 6520   linear average 
+000080a0: 6f66 2074 6865 2063 6f72 7265 6c61 7469  of the correlati
+000080b0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+000080c0: 2020 2063 7261 705b 3a4e 6666 7432 5d20     crap[:Nfft2] 
+000080d0: 3d20 6372 6170 5b3a 4e66 6674 325d 202d  = crap[:Nfft2] -
+000080e0: 206e 702e 6d65 616e 2863 7261 705b 3a4e   np.mean(crap[:N
+000080f0: 6666 7432 5d29 2020 2320 7265 6d6f 7665  fft2])  # remove
+00008100: 2074 6865 206d 6561 6e20 696e 2066 7265   the mean in fre
+00008110: 7120 646f 6d61 696e 2028 7370 696b 6520  q domain (spike 
+00008120: 6174 2074 3d30 290a 2020 2020 2020 2020  at t=0).        
+00008130: 2020 2020 2020 2020 6372 6170 5b2d 284e          crap[-(N
+00008140: 6666 7432 2920 2b20 3120 3a5d 203d 206e  fft2) + 1 :] = n
+00008150: 702e 666c 6970 286e 702e 636f 6e6a 2863  p.flip(np.conj(c
+00008160: 7261 705b 313a 284e 6666 7432 295d 292c  rap[1:(Nfft2)]),
+00008170: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+00008180: 2020 2020 2020 2020 2063 7261 705b 305d           crap[0]
+00008190: 203d 2063 6f6d 706c 6578 2830 2c20 3029   = complex(0, 0)
+000081a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081b0: 2073 5f63 6f72 725b 6973 7461 636b 2c20   s_corr[istack, 
+000081c0: 3a5d 203d 206e 702e 7265 616c 286e 702e  :] = np.real(np.
+000081d0: 6666 742e 6966 6674 7368 6966 7428 7363  fft.ifftshift(sc
+000081e0: 6970 792e 6666 7470 6163 6b2e 6966 6674  ipy.fftpack.ifft
+000081f0: 2863 7261 702c 204e 6666 742c 2061 7869  (crap, Nfft, axi
+00008200: 733d 3029 2929 0a20 2020 2020 2020 2020  s=0))).         
+00008210: 2020 2020 2020 206e 5f63 6f72 725b 6973         n_corr[is
+00008220: 7461 636b 5d20 3d20 6c65 6e28 6974 696d  tack] = len(itim
+00008230: 6529 2020 2320 6e75 6d62 6572 206f 6620  e)  # number of 
+00008240: 7769 6e64 6f77 7320 7374 6163 6b73 0a20  windows stacks. 
+00008250: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00008260: 5f63 6f72 725b 6973 7461 636b 5d20 3d20  _corr[istack] = 
+00008270: 7473 7461 7274 2020 2320 7361 7665 2074  tstart  # save t
+00008280: 6865 2074 696d 6520 7374 616d 7073 0a20  he time stamps. 
+00008290: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000082a0: 7374 6172 7420 2b3d 2073 7562 7374 6163  start += substac
+000082b0: 6b5f 6c65 6e0a 2020 2020 2020 2020 2020  k_len.          
+000082c0: 2020 2020 2020 2320 7072 696e 7428 2763        # print('c
+000082d0: 6f72 7265 6c61 7469 6f6e 2064 6f6e 6520  orrelation done 
+000082e0: 616e 6420 7374 6163 6b65 6420 6174 2074  and stacked at t
+000082f0: 696d 6520 2573 2720 2520 7374 7228 745f  ime %s' % str(t_
+00008300: 636f 7272 5b69 7374 6163 6b5d 2929 0a0a  corr[istack]))..
+00008310: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00008320: 6d6f 7665 2061 626e 6f72 6d61 6c20 6461  move abnormal da
+00008330: 7461 0a20 2020 2020 2020 2020 2020 2061  ta.            a
+00008340: 6d70 6d61 7820 3d20 6e70 2e6d 6178 2873  mpmax = np.max(s
+00008350: 5f63 6f72 722c 2061 7869 733d 3129 0a20  _corr, axis=1). 
+00008360: 2020 2020 2020 2020 2020 2074 696e 6478             tindx
+00008370: 203d 206e 702e 7768 6572 6528 2861 6d70   = np.where((amp
+00008380: 6d61 7820 3c20 3230 202a 206e 702e 6d65  max < 20 * np.me
+00008390: 6469 616e 2861 6d70 6d61 7829 2920 2620  dian(ampmax)) & 
+000083a0: 2861 6d70 6d61 7820 3e20 3029 295b 305d  (ampmax > 0))[0]
+000083b0: 0a20 2020 2020 2020 2020 2020 2073 5f63  .            s_c
+000083c0: 6f72 7220 3d20 735f 636f 7272 5b74 696e  orr = s_corr[tin
+000083d0: 6478 2c20 3a5d 0a20 2020 2020 2020 2020  dx, :].         
+000083e0: 2020 2074 5f63 6f72 7220 3d20 745f 636f     t_corr = t_co
+000083f0: 7272 5b74 696e 6478 5d0a 2020 2020 2020  rr[tindx].      
+00008400: 2020 2020 2020 6e5f 636f 7272 203d 206e        n_corr = n
+00008410: 5f63 6f72 725b 7469 6e64 785d 0a0a 2020  _corr[tindx]..  
+00008420: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008430: 2320 6176 6572 6167 6520 6461 696c 7920  # average daily 
+00008440: 6372 6f73 7320 636f 7272 656c 6174 696f  cross correlatio
+00008450: 6e20 6675 6e63 7469 6f6e 730a 2020 2020  n functions.    
+00008460: 2020 2020 6966 2073 7461 636b 5f6d 6574      if stack_met
+00008470: 686f 6420 3d3d 2053 7461 636b 4d65 7468  hod == StackMeth
+00008480: 6f64 2e4c 494e 4541 523a 0a20 2020 2020  od.LINEAR:.     
+00008490: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
+000084a0: 6e70 2e6d 6178 2873 5f63 6f72 722c 2061  np.max(s_corr, a
+000084b0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
+000084c0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
+000084d0: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
+000084e0: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
+000084f0: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
+00008500: 3e20 3029 295b 305d 0a20 2020 2020 2020  > 0))[0].       
+00008510: 2020 2020 2073 5f63 6f72 7220 3d20 6e70       s_corr = np
+00008520: 2e6d 6561 6e28 735f 636f 7272 5b74 696e  .mean(s_corr[tin
+00008530: 6478 5d2c 2061 7869 733d 3029 0a20 2020  dx], axis=0).   
+00008540: 2020 2020 2020 2020 2074 5f63 6f72 7220           t_corr 
+00008550: 3d20 6461 7461 535f 745b 305d 0a20 2020  = dataS_t[0].   
+00008560: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
+00008570: 3d20 6c65 6e28 7469 6e64 7829 0a20 2020  = len(tindx).   
+00008580: 2020 2020 2065 6c69 6620 7374 6163 6b5f       elif stack_
+00008590: 6d65 7468 6f64 203d 3d20 5374 6163 6b4d  method == StackM
+000085a0: 6574 686f 642e 524f 4255 5354 3a0a 2020  ethod.ROBUST:.  
+000085b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+000085c0: 2e69 6e66 6f28 2264 6f20 726f 6275 7374  .info("do robust
+000085d0: 2073 7562 7374 6163 6b69 6e67 2229 0a20   substacking"). 
+000085e0: 2020 2020 2020 2020 2020 2073 5f63 6f72             s_cor
+000085f0: 7220 3d20 726f 6275 7374 5f73 7461 636b  r = robust_stack
+00008600: 2873 5f63 6f72 722c 2030 2e30 3031 290a  (s_corr, 0.001).
+00008610: 2020 2020 2020 2020 2020 2020 745f 636f              t_co
+00008620: 7272 203d 2064 6174 6153 5f74 5b30 5d0a  rr = dataS_t[0].
+00008630: 2020 2020 2020 2020 2020 2020 6e5f 636f              n_co
+00008640: 7272 203d 206e 7769 6e0a 2020 2020 2320  rr = nwin.    # 
+00008650: 2065 6c69 6620 7374 6163 6b5f 6d65 7468   elif stack_meth
+00008660: 6f64 203d 3d20 2773 656c 6563 7469 7665  od == 'selective
+00008670: 273a 0a20 2020 2023 2020 2020 2020 7072  ':.    #      pr
+00008680: 696e 7428 2764 6f20 7365 6c65 6374 6976  int('do selectiv
+00008690: 6520 7375 6273 7461 636b 696e 6727 290a  e substacking').
+000086a0: 2020 2020 2320 2020 2020 2073 5f63 6f72      #      s_cor
+000086b0: 7220 3d20 7365 6c65 6374 6976 655f 7374  r = selective_st
+000086c0: 6163 6b28 735f 636f 7272 2c30 2e30 3031  ack(s_corr,0.001
+000086d0: 290a 2020 2020 2320 2020 2020 2074 5f63  ).    #      t_c
+000086e0: 6f72 7220 3d20 6461 7461 535f 745b 305d  orr = dataS_t[0]
+000086f0: 0a20 2020 2023 2020 2020 2020 6e5f 636f  .    #      n_co
+00008700: 7272 203d 206e 7769 6e0a 0a20 2020 2023  rr = nwin..    #
+00008710: 2074 7269 6d20 7468 6520 4343 4673 2069   trim the CCFs i
+00008720: 6e20 5b2d 6d61 786c 6167 206d 6178 6c61  n [-maxlag maxla
+00008730: 675d 0a20 2020 2074 203d 206e 702e 6172  g].    t = np.ar
+00008740: 616e 6765 282d 4e66 6674 3220 2b20 312c  ange(-Nfft2 + 1,
+00008750: 204e 6666 7432 2920 2a20 6474 0a20 2020   Nfft2) * dt.   
+00008760: 2069 6e64 203d 206e 702e 7768 6572 6528   ind = np.where(
+00008770: 6e70 2e61 6273 2874 2920 3c3d 206d 6178  np.abs(t) <= max
+00008780: 6c61 6729 5b30 5d0a 2020 2020 6966 2073  lag)[0].    if s
+00008790: 5f63 6f72 722e 6e64 696d 203d 3d20 313a  _corr.ndim == 1:
+000087a0: 0a20 2020 2020 2020 2073 5f63 6f72 7220  .        s_corr 
+000087b0: 3d20 735f 636f 7272 5b69 6e64 5d0a 2020  = s_corr[ind].  
+000087c0: 2020 656c 6966 2073 5f63 6f72 722e 6e64    elif s_corr.nd
+000087d0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
+000087e0: 2073 5f63 6f72 7220 3d20 735f 636f 7272   s_corr = s_corr
+000087f0: 5b3a 2c20 696e 645d 0a20 2020 2072 6574  [:, ind].    ret
+00008800: 7572 6e20 735f 636f 7272 2c20 745f 636f  urn s_corr, t_co
+00008810: 7272 2c20 6e5f 636f 7272 2c20 6e73 5f63  rr, n_corr, ns_c
+00008820: 6f72 725b 3a2c 2069 6e64 5d0a 0a0a 6465  orr[:, ind]...de
+00008830: 6620 6363 5f70 6172 616d 6574 6572 7328  f cc_parameters(
+00008840: 6363 5f70 6172 612c 2063 6f6f 722c 2074  cc_para, coor, t
+00008850: 636f 7272 2c20 6e63 6f72 722c 2063 6f6d  corr, ncorr, com
+00008860: 7029 3a0a 2020 2020 2222 220a 2020 2020  p):.    """.    
+00008870: 7468 6973 2066 756e 6374 696f 6e20 6173  this function as
+00008880: 7365 6d62 6c65 7320 7468 6520 7061 7261  sembles the para
+00008890: 6d65 7465 7273 2066 6f72 2074 6865 2063  meters for the c
+000088a0: 6320 6675 6e63 7469 6f6e 2c20 7768 6963  c function, whic
+000088b0: 6820 6973 2075 7365 640a 2020 2020 7768  h is used.    wh
+000088c0: 656e 2077 7269 7469 6e67 2074 6865 6d20  en writing them 
+000088d0: 696e 746f 2041 5344 4620 6669 6c65 730a  into ASDF files.
+000088e0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+000088f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00008900: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6363  ---------.    cc
+00008910: 5f70 6172 613a 2064 6963 7420 636f 6e74  _para: dict cont
+00008920: 6169 6e69 6e67 2070 6172 616d 6574 6572  aining parameter
+00008930: 7320 7573 6564 2069 6e20 7468 6520 6666  s used in the ff
+00008940: 745f 6363 2073 7465 700a 2020 2020 636f  t_cc step.    co
+00008950: 6f72 3a20 2020 2064 6963 7420 636f 6e74  or:    dict cont
+00008960: 6169 6e69 6e67 2063 6f6f 7264 696e 6174  aining coordinat
+00008970: 6573 2069 6e66 6f20 6f66 2074 6865 2073  es info of the s
+00008980: 6f75 7263 6520 616e 6420 7265 6365 6976  ource and receiv
+00008990: 6572 2073 7461 7469 6f6e 730a 2020 2020  er stations.    
+000089a0: 7463 6f72 723a 2020 2074 696d 6573 7461  tcorr:   timesta
+000089b0: 6d70 206d 6174 7269 780a 2020 2020 6e63  mp matrix.    nc
+000089c0: 6f72 723a 2020 206d 6174 7269 7820 6f66  orr:   matrix of
+000089d0: 206e 756d 6265 7220 6f66 2067 6f6f 6420   number of good 
+000089e0: 7365 676d 656e 7473 2066 6f72 2065 6163  segments for eac
+000089f0: 6820 7375 622d 7374 6163 6b2f 6669 6e61  h sub-stack/fina
+00008a00: 6c20 7374 6163 6b0a 2020 2020 636f 6d70  l stack.    comp
+00008a10: 3a20 2020 2032 2063 6861 7261 6374 6572  :    2 character
+00008a20: 2073 7472 696e 6773 2066 6f72 2074 6865   strings for the
+00008a30: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
+00008a40: 6f6e 2063 6f6d 706f 6e65 6e74 0a20 2020  on component.   
+00008a50: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+00008a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008a70: 0a20 2020 2070 6172 616d 6574 6572 733a  .    parameters:
+00008a80: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
+00008a90: 2061 626f 7665 2069 6e66 6f20 7573 6564   above info used
+00008aa0: 2066 6f72 206c 6174 6572 2073 7461 636b   for later stack
+00008ab0: 696e 672f 706c 6f74 7469 6e67 0a20 2020  ing/plotting.   
+00008ac0: 2022 2222 0a20 2020 206c 6174 5320 3d20   """.    latS = 
+00008ad0: 636f 6f72 5b22 6c61 7453 225d 0a20 2020  coor["latS"].   
+00008ae0: 206c 6f6e 5320 3d20 636f 6f72 5b22 6c6f   lonS = coor["lo
+00008af0: 6e53 225d 0a20 2020 206c 6174 5220 3d20  nS"].    latR = 
+00008b00: 636f 6f72 5b22 6c61 7452 225d 0a20 2020  coor["latR"].   
+00008b10: 206c 6f6e 5220 3d20 636f 6f72 5b22 6c6f   lonR = coor["lo
+00008b20: 6e52 225d 0a20 2020 2064 7420 3d20 6363  nR"].    dt = cc
+00008b30: 5f70 6172 615b 2264 7422 5d0a 2020 2020  _para["dt"].    
+00008b40: 6d61 786c 6167 203d 2063 635f 7061 7261  maxlag = cc_para
+00008b50: 5b22 6d61 786c 6167 225d 0a20 2020 2073  ["maxlag"].    s
+00008b60: 7562 7374 6163 6b20 3d20 6363 5f70 6172  ubstack = cc_par
+00008b70: 615b 2273 7562 7374 6163 6b22 5d0a 2020  a["substack"].  
+00008b80: 2020 6363 5f6d 6574 686f 6420 3d20 6363    cc_method = cc
+00008b90: 5f70 6172 615b 2263 635f 6d65 7468 6f64  _para["cc_method
+00008ba0: 225d 0a0a 2020 2020 6469 7374 2c20 617a  "]..    dist, az
+00008bb0: 692c 2062 617a 203d 206f 6273 7079 2e67  i, baz = obspy.g
+00008bc0: 656f 6465 7469 6373 2e62 6173 652e 6770  eodetics.base.gp
+00008bd0: 7332 6469 7374 5f61 7a69 6d75 7468 286c  s2dist_azimuth(l
+00008be0: 6174 532c 206c 6f6e 532c 206c 6174 522c  atS, lonS, latR,
+00008bf0: 206c 6f6e 5229 0a20 2020 2070 6172 616d   lonR).    param
+00008c00: 6574 6572 7320 3d20 7b0a 2020 2020 2020  eters = {.      
+00008c10: 2020 2264 7422 3a20 6474 2c0a 2020 2020    "dt": dt,.    
+00008c20: 2020 2020 226d 6178 6c61 6722 3a20 696e      "maxlag": in
+00008c30: 7428 6d61 786c 6167 292c 0a20 2020 2020  t(maxlag),.     
+00008c40: 2020 2022 6469 7374 223a 206e 702e 666c     "dist": np.fl
+00008c50: 6f61 7433 3228 6469 7374 202f 2031 3030  oat32(dist / 100
+00008c60: 3029 2c0a 2020 2020 2020 2020 2261 7a69  0),.        "azi
+00008c70: 223a 206e 702e 666c 6f61 7433 3228 617a  ": np.float32(az
+00008c80: 6929 2c0a 2020 2020 2020 2020 2262 617a  i),.        "baz
+00008c90: 223a 206e 702e 666c 6f61 7433 3228 6261  ": np.float32(ba
+00008ca0: 7a29 2c0a 2020 2020 2020 2020 226c 6f6e  z),.        "lon
+00008cb0: 5322 3a20 6e70 2e66 6c6f 6174 3332 286c  S": np.float32(l
+00008cc0: 6f6e 5329 2c0a 2020 2020 2020 2020 226c  onS),.        "l
+00008cd0: 6174 5322 3a20 6e70 2e66 6c6f 6174 3332  atS": np.float32
+00008ce0: 286c 6174 5329 2c0a 2020 2020 2020 2020  (latS),.        
+00008cf0: 226c 6f6e 5222 3a20 6e70 2e66 6c6f 6174  "lonR": np.float
+00008d00: 3332 286c 6f6e 5229 2c0a 2020 2020 2020  32(lonR),.      
+00008d10: 2020 226c 6174 5222 3a20 6e70 2e66 6c6f    "latR": np.flo
+00008d20: 6174 3332 286c 6174 5229 2c0a 2020 2020  at32(latR),.    
+00008d30: 2020 2020 226e 676f 6f64 223a 206e 636f      "ngood": nco
+00008d40: 7272 2c0a 2020 2020 2020 2020 2263 635f  rr,.        "cc_
+00008d50: 6d65 7468 6f64 223a 2063 635f 6d65 7468  method": cc_meth
+00008d60: 6f64 2c0a 2020 2020 2020 2020 2274 696d  od,.        "tim
+00008d70: 6522 3a20 7463 6f72 722c 0a20 2020 2020  e": tcorr,.     
+00008d80: 2020 2022 7375 6273 7461 636b 223a 2073     "substack": s
+00008d90: 7562 7374 6163 6b2c 0a20 2020 2020 2020  ubstack,.       
+00008da0: 2022 636f 6d70 223a 2063 6f6d 702c 0a20   "comp": comp,. 
+00008db0: 2020 207d 0a20 2020 2072 6574 7572 6e20     }.    return 
+00008dc0: 7061 7261 6d65 7465 7273 0a0a 0a64 6566  parameters...def
+00008dd0: 2073 7461 636b 696e 6728 6363 5f61 7272   stacking(cc_arr
+00008de0: 6179 2c20 6363 5f74 696d 652c 2063 635f  ay, cc_time, cc_
+00008df0: 6e67 6f6f 642c 2073 7461 636b 5f70 6172  ngood, stack_par
+00008e00: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
+00008e10: 7468 6973 2066 756e 6374 696f 6e20 7374  this function st
+00008e20: 6163 6b73 2074 6865 2063 726f 7373 2063  acks the cross c
+00008e30: 6f72 7265 6c61 7469 6f6e 2064 6174 6120  orrelation data 
+00008e40: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+00008e50: 2075 7365 722d 6465 6669 6e65 6420 7375   user-defined su
+00008e60: 6273 7461 636b 5f6c 656e 2070 6172 616d  bstack_len param
+00008e70: 6574 6572 0a0a 2020 2020 5041 5241 4d45  eter..    PARAME
+00008e80: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+00008e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008ea0: 0a20 2020 2063 635f 6172 7261 793a 2032  .    cc_array: 2
+00008eb0: 4420 6e75 6d70 7920 666c 6f61 7433 3220  D numpy float32 
+00008ec0: 6d61 7472 6978 2063 6f6e 7461 696e 696e  matrix containin
+00008ed0: 6720 616c 6c20 7365 676d 656e 7465 6420  g all segmented 
+00008ee0: 6372 6f73 732d 636f 7272 656c 6174 696f  cross-correlatio
+00008ef0: 6e20 6461 7461 0a20 2020 2063 635f 7469  n data.    cc_ti
+00008f00: 6d65 3a20 2031 4420 6e75 6d70 7920 6172  me:  1D numpy ar
+00008f10: 7261 7920 6f66 2074 696d 6573 7461 6d70  ray of timestamp
+00008f20: 7320 666f 7220 6561 6368 2073 6567 6d65  s for each segme
+00008f30: 6e74 206f 6620 6363 5f61 7272 6179 0a20  nt of cc_array. 
+00008f40: 2020 2063 635f 6e67 6f6f 643a 2031 4420     cc_ngood: 1D 
+00008f50: 6e75 6d70 7920 696e 7431 3620 6d61 7472  numpy int16 matr
+00008f60: 6978 2073 686f 7769 6e67 2074 6865 206e  ix showing the n
+00008f70: 756d 6265 7220 6f66 2073 6567 6d65 6e74  umber of segment
+00008f80: 7320 666f 7220 6561 6368 2073 7562 2d73  s for each sub-s
+00008f90: 7461 636b 2061 6e64 2f6f 7220 6675 6c6c  tack and/or full
+00008fa0: 2073 7461 636b 0a20 2020 2073 7461 636b   stack.    stack
+00008fb0: 5f70 6172 613a 2061 2064 6963 7420 636f  _para: a dict co
+00008fc0: 6e74 6169 6e69 6e67 2061 6c6c 2073 7461  ntaining all sta
+00008fd0: 636b 696e 6720 7061 7261 6d65 7465 7273  cking parameters
+00008fe0: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
+00008ff0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00009000: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6363  ---------.    cc
+00009010: 5f61 7272 6179 2c20 6363 5f6e 676f 6f64  _array, cc_ngood
+00009020: 2c20 6363 5f74 696d 653a 2073 616d 6520  , cc_time: same 
+00009030: 746f 2074 6865 2069 6e70 7574 2070 6172  to the input par
+00009040: 616d 6574 6572 7320 6275 7420 7769 7468  ameters but with
+00009050: 2061 626e 6f72 6d61 6c20 6372 6f73 732d   abnormal cross-
+00009060: 636f 7272 6561 6c74 696f 6e73 2072 656d  correaltions rem
+00009070: 6f76 6564 0a20 2020 2061 6c6c 7374 6163  oved.    allstac
+00009080: 6b73 313a 2031 4420 6d61 7472 6978 206f  ks1: 1D matrix o
+00009090: 6620 7374 6163 6b65 6420 6372 6f73 732d  f stacked cross-
+000090a0: 636f 7272 656c 6174 696f 6e20 6675 6e63  correlation func
+000090b0: 7469 6f6e 7320 6f76 6572 2061 6c6c 2074  tions over all t
+000090c0: 6865 2073 6567 6d65 6e74 730a 2020 2020  he segments.    
+000090d0: 6e73 7461 636b 733a 2020 2020 6e75 6d62  nstacks:    numb
+000090e0: 6572 206f 6620 6f76 6572 616c 6c20 7365  er of overall se
+000090f0: 676d 656e 7473 2066 6f72 2074 6865 2066  gments for the f
+00009100: 696e 616c 2073 7461 636b 730a 2020 2020  inal stacks.    
+00009110: 2222 220a 2020 2020 2320 6c6f 6164 2075  """.    # load u
+00009120: 7365 6675 6c20 7061 7261 6d65 7465 7273  seful parameters
+00009130: 2066 726f 6d20 6469 6374 0a20 2020 2073   from dict.    s
+00009140: 616d 705f 6672 6571 203d 2073 7461 636b  amp_freq = stack
+00009150: 5f70 6172 615b 2273 616d 705f 6672 6571  _para["samp_freq
+00009160: 225d 0a20 2020 2073 6d65 7468 6f64 203d  "].    smethod =
+00009170: 2073 7461 636b 5f70 6172 615b 2273 7461   stack_para["sta
+00009180: 636b 5f6d 6574 686f 6422 5d0a 2020 2020  ck_method"].    
+00009190: 6e70 7473 203d 2063 635f 6172 7261 792e  npts = cc_array.
+000091a0: 7368 6170 655b 315d 0a0a 2020 2020 2320  shape[1]..    # 
+000091b0: 7265 6d6f 7665 2061 626e 6f72 6d61 6c20  remove abnormal 
+000091c0: 6461 7461 0a20 2020 2061 6d70 6d61 7820  data.    ampmax 
+000091d0: 3d20 6e70 2e6d 6178 2863 635f 6172 7261  = np.max(cc_arra
+000091e0: 792c 2061 7869 733d 3129 0a20 2020 2074  y, axis=1).    t
+000091f0: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
+00009200: 2861 6d70 6d61 7820 3c20 3230 202a 206e  (ampmax < 20 * n
+00009210: 702e 6d65 6469 616e 2861 6d70 6d61 7829  p.median(ampmax)
+00009220: 2920 2620 2861 6d70 6d61 7820 3e20 3029  ) & (ampmax > 0)
+00009230: 295b 305d 0a20 2020 2069 6620 6e6f 7420  )[0].    if not 
+00009240: 6c65 6e28 7469 6e64 7829 3a0a 2020 2020  len(tindx):.    
+00009250: 2020 2020 616c 6c73 7461 636b 7331 203d      allstacks1 =
+00009260: 205b 5d0a 2020 2020 2020 2020 616c 6c73   [].        alls
+00009270: 7461 636b 7332 203d 205b 5d0a 2020 2020  tacks2 = [].    
+00009280: 2020 2020 616c 6c73 7461 636b 7333 203d      allstacks3 =
+00009290: 205b 5d0a 2020 2020 2020 2020 6e73 7461   [].        nsta
+000092a0: 636b 7320 3d20 300a 2020 2020 2020 2020  cks = 0.        
+000092b0: 6363 5f61 7272 6179 203d 205b 5d0a 2020  cc_array = [].  
+000092c0: 2020 2020 2020 6363 5f6e 676f 6f64 203d        cc_ngood =
+000092d0: 205b 5d0a 2020 2020 2020 2020 6363 5f74   [].        cc_t
+000092e0: 696d 6520 3d20 5b5d 0a20 2020 2020 2020  ime = [].       
+000092f0: 2072 6574 7572 6e20 6363 5f61 7272 6179   return cc_array
+00009300: 2c20 6363 5f6e 676f 6f64 2c20 6363 5f74  , cc_ngood, cc_t
+00009310: 696d 652c 2061 6c6c 7374 6163 6b73 312c  ime, allstacks1,
+00009320: 2061 6c6c 7374 6163 6b73 322c 2061 6c6c   allstacks2, all
+00009330: 7374 6163 6b73 332c 206e 7374 6163 6b73  stacks3, nstacks
+00009340: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00009350: 2020 2023 2072 656d 6f76 6520 6f6e 6573     # remove ones
+00009360: 2077 6974 6820 6261 6420 616d 706c 6974   with bad amplit
+00009370: 7564 650a 2020 2020 2020 2020 6363 5f61  ude.        cc_a
+00009380: 7272 6179 203d 2063 635f 6172 7261 795b  rray = cc_array[
+00009390: 7469 6e64 782c 203a 5d0a 2020 2020 2020  tindx, :].      
+000093a0: 2020 6363 5f74 696d 6520 3d20 6363 5f74    cc_time = cc_t
+000093b0: 696d 655b 7469 6e64 785d 0a20 2020 2020  ime[tindx].     
+000093c0: 2020 2063 635f 6e67 6f6f 6420 3d20 6363     cc_ngood = cc
+000093d0: 5f6e 676f 6f64 5b74 696e 6478 5d0a 0a20  _ngood[tindx].. 
+000093e0: 2020 2020 2020 2023 2064 6f20 7374 6163         # do stac
+000093f0: 6b69 6e67 0a20 2020 2020 2020 2061 6c6c  king.        all
+00009400: 7374 6163 6b73 3120 3d20 6e70 2e7a 6572  stacks1 = np.zer
+00009410: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
+00009420: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
+00009430: 2020 2061 6c6c 7374 6163 6b73 3220 3d20     allstacks2 = 
+00009440: 6e70 2e7a 6572 6f73 286e 7074 732c 2064  np.zeros(npts, d
+00009450: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00009460: 0a20 2020 2020 2020 2061 6c6c 7374 6163  .        allstac
+00009470: 6b73 3320 3d20 6e70 2e7a 6572 6f73 286e  ks3 = np.zeros(n
+00009480: 7074 732c 2064 7479 7065 3d6e 702e 666c  pts, dtype=np.fl
+00009490: 6f61 7433 3229 0a0a 2020 2020 2020 2020  oat32)..        
+000094a0: 6966 2073 6d65 7468 6f64 203d 3d20 5374  if smethod == St
+000094b0: 6163 6b4d 6574 686f 642e 4c49 4e45 4152  ackMethod.LINEAR
+000094c0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+000094d0: 6c73 7461 636b 7331 203d 206e 702e 6d65  lstacks1 = np.me
+000094e0: 616e 2863 635f 6172 7261 792c 2061 7869  an(cc_array, axi
+000094f0: 733d 3029 0a20 2020 2020 2020 2065 6c69  s=0).        eli
+00009500: 6620 736d 6574 686f 6420 3d3d 2053 7461  f smethod == Sta
+00009510: 636b 4d65 7468 6f64 2e50 5753 3a0a 2020  ckMethod.PWS:.  
+00009520: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
+00009530: 636b 7331 203d 2070 7773 2863 635f 6172  cks1 = pws(cc_ar
+00009540: 7261 792c 2073 616d 705f 6672 6571 290a  ray, samp_freq).
+00009550: 2020 2020 2020 2020 656c 6966 2073 6d65          elif sme
+00009560: 7468 6f64 203d 3d20 5374 6163 6b4d 6574  thod == StackMet
+00009570: 686f 642e 524f 4255 5354 3a0a 2020 2020  hod.ROBUST:.    
+00009580: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
+00009590: 7331 2c20 772c 206e 7374 6570 203d 2072  s1, w, nstep = r
+000095a0: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
+000095b0: 7272 6179 2c20 302e 3030 3129 0a20 2020  rray, 0.001).   
+000095c0: 2020 2020 2065 6c69 6620 736d 6574 686f       elif smetho
+000095d0: 6420 3d3d 2053 7461 636b 4d65 7468 6f64  d == StackMethod
+000095e0: 2e41 5554 4f5f 434f 5641 5249 414e 4345  .AUTO_COVARIANCE
+000095f0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+00009600: 6c73 7461 636b 7331 203d 2061 6461 7074  lstacks1 = adapt
+00009610: 6976 655f 6669 6c74 6572 2863 635f 6172  ive_filter(cc_ar
+00009620: 7261 792c 2031 290a 2020 2020 2020 2020  ray, 1).        
+00009630: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
+00009640: 5374 6163 6b4d 6574 686f 642e 4e52 4f4f  StackMethod.NROO
+00009650: 543a 0a20 2020 2020 2020 2020 2020 2061  T:.            a
+00009660: 6c6c 7374 6163 6b73 3120 3d20 6e72 6f6f  llstacks1 = nroo
+00009670: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
+00009680: 2c20 3229 0a20 2020 2020 2020 2065 6c69  , 2).        eli
+00009690: 6620 736d 6574 686f 6420 3d3d 2053 7461  f smethod == Sta
+000096a0: 636b 4d65 7468 6f64 2e41 4c4c 3a0a 2020  ckMethod.ALL:.  
+000096b0: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
+000096c0: 636b 7331 203d 206e 702e 6d65 616e 2863  cks1 = np.mean(c
+000096d0: 635f 6172 7261 792c 2061 7869 733d 3029  c_array, axis=0)
+000096e0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+000096f0: 7374 6163 6b73 3220 3d20 7077 7328 6363  stacks2 = pws(cc
+00009700: 5f61 7272 6179 2c20 7361 6d70 5f66 7265  _array, samp_fre
+00009710: 7129 0a20 2020 2020 2020 2020 2020 2061  q).            a
+00009720: 6c6c 7374 6163 6b73 332c 2077 2c20 6e73  llstacks3, w, ns
+00009730: 7465 7020 3d20 726f 6275 7374 5f73 7461  tep = robust_sta
+00009740: 636b 2863 635f 6172 7261 792c 2030 2e30  ck(cc_array, 0.0
+00009750: 3031 290a 2020 2020 2020 2020 6e73 7461  01).        nsta
+00009760: 636b 7320 3d20 6e70 2e73 756d 2863 635f  cks = np.sum(cc_
+00009770: 6e67 6f6f 6429 0a0a 2020 2020 2320 676f  ngood)..    # go
+00009780: 6f64 2074 6f20 7265 7475 726e 0a20 2020  od to return.   
+00009790: 2072 6574 7572 6e20 6363 5f61 7272 6179   return cc_array
+000097a0: 2c20 6363 5f6e 676f 6f64 2c20 6363 5f74  , cc_ngood, cc_t
+000097b0: 696d 652c 2061 6c6c 7374 6163 6b73 312c  ime, allstacks1,
+000097c0: 2061 6c6c 7374 6163 6b73 322c 2061 6c6c   allstacks2, all
+000097d0: 7374 6163 6b73 332c 206e 7374 6163 6b73  stacks3, nstacks
+000097e0: 0a0a 0a64 6566 2073 7461 636b 696e 675f  ...def stacking_
+000097f0: 726d 6128 6363 5f61 7272 6179 2c20 6363  rma(cc_array, cc
+00009800: 5f74 696d 652c 2063 635f 6e67 6f6f 642c  _time, cc_ngood,
+00009810: 2073 7461 636b 5f70 6172 6129 3a0a 2020   stack_para):.  
+00009820: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
+00009830: 756e 6374 696f 6e20 7374 6163 6b73 2074  unction stacks t
+00009840: 6865 2063 726f 7373 2063 6f72 7265 6c61  he cross correla
+00009850: 7469 6f6e 2064 6174 6120 6163 636f 7264  tion data accord
+00009860: 696e 6720 746f 2074 6865 2075 7365 722d  ing to the user-
+00009870: 6465 6669 6e65 6420 7375 6273 7461 636b  defined substack
+00009880: 5f6c 656e 2070 6172 616d 6574 6572 0a20  _len parameter. 
+00009890: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+000098a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+000098b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6363  ---------.    cc
+000098c0: 5f61 7272 6179 3a20 3244 206e 756d 7079  _array: 2D numpy
+000098d0: 2066 6c6f 6174 3332 206d 6174 7269 7820   float32 matrix 
+000098e0: 636f 6e74 6169 6e69 6e67 2061 6c6c 2073  containing all s
+000098f0: 6567 6d65 6e74 6564 2063 726f 7373 2d63  egmented cross-c
+00009900: 6f72 7265 6c61 7469 6f6e 2064 6174 610a  orrelation data.
+00009910: 2020 2020 6363 5f74 696d 653a 2020 3144      cc_time:  1D
+00009920: 206e 756d 7079 2061 7272 6179 206f 6620   numpy array of 
+00009930: 7469 6d65 7374 616d 7073 2066 6f72 2065  timestamps for e
+00009940: 6163 6820 7365 676d 656e 7420 6f66 2063  ach segment of c
+00009950: 635f 6172 7261 790a 2020 2020 6363 5f6e  c_array.    cc_n
+00009960: 676f 6f64 3a20 3144 206e 756d 7079 2069  good: 1D numpy i
+00009970: 6e74 3136 206d 6174 7269 7820 7368 6f77  nt16 matrix show
+00009980: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
+00009990: 6620 7365 676d 656e 7473 2066 6f72 2065  f segments for e
+000099a0: 6163 6820 7375 622d 7374 6163 6b20 616e  ach sub-stack an
+000099b0: 642f 6f72 2066 756c 6c20 7374 6163 6b0a  d/or full stack.
+000099c0: 2020 2020 7374 6163 6b5f 7061 7261 3a20      stack_para: 
+000099d0: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
+000099e0: 6720 616c 6c20 7374 6163 6b69 6e67 2070  g all stacking p
+000099f0: 6172 616d 6574 6572 730a 2020 2020 5245  arameters.    RE
+00009a00: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+00009a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009a20: 2d0a 2020 2020 6363 5f61 7272 6179 2c20  -.    cc_array, 
+00009a30: 6363 5f6e 676f 6f64 2c20 6363 5f74 696d  cc_ngood, cc_tim
+00009a40: 653a 2073 616d 6520 746f 2074 6865 2069  e: same to the i
+00009a50: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
+00009a60: 6275 7420 7769 7468 2061 626e 6f72 6d61  but with abnorma
+00009a70: 6c20 6372 6f73 732d 636f 7272 6561 6c74  l cross-correalt
+00009a80: 696f 6e73 2072 656d 6f76 6564 0a20 2020  ions removed.   
+00009a90: 2061 6c6c 7374 6163 6b73 313a 2031 4420   allstacks1: 1D 
+00009aa0: 6d61 7472 6978 206f 6620 7374 6163 6b65  matrix of stacke
+00009ab0: 6420 6372 6f73 732d 636f 7272 656c 6174  d cross-correlat
+00009ac0: 696f 6e20 6675 6e63 7469 6f6e 7320 6f76  ion functions ov
+00009ad0: 6572 2061 6c6c 2074 6865 2073 6567 6d65  er all the segme
+00009ae0: 6e74 730a 2020 2020 6e73 7461 636b 733a  nts.    nstacks:
+00009af0: 2020 2020 6e75 6d62 6572 206f 6620 6f76      number of ov
+00009b00: 6572 616c 6c20 7365 676d 656e 7473 2066  erall segments f
+00009b10: 6f72 2074 6865 2066 696e 616c 2073 7461  or the final sta
+00009b20: 636b 730a 2020 2020 2222 220a 2020 2020  cks.    """.    
+00009b30: 2320 6c6f 6164 2075 7365 6675 6c20 7061  # load useful pa
+00009b40: 7261 6d65 7465 7273 2066 726f 6d20 6469  rameters from di
+00009b50: 6374 0a20 2020 2073 616d 705f 6672 6571  ct.    samp_freq
+00009b60: 203d 2073 7461 636b 5f70 6172 615b 2273   = stack_para["s
+00009b70: 616d 705f 6672 6571 225d 0a20 2020 2073  amp_freq"].    s
+00009b80: 6d65 7468 6f64 203d 2073 7461 636b 5f70  method = stack_p
+00009b90: 6172 615b 2273 7461 636b 5f6d 6574 686f  ara["stack_metho
+00009ba0: 6422 5d0a 2020 2020 726d 615f 7375 6273  d"].    rma_subs
+00009bb0: 7461 636b 203d 2073 7461 636b 5f70 6172  tack = stack_par
+00009bc0: 615b 2272 6d61 5f73 7562 7374 6163 6b22  a["rma_substack"
+00009bd0: 5d0a 2020 2020 726d 615f 7374 6570 203d  ].    rma_step =
+00009be0: 2073 7461 636b 5f70 6172 615b 2272 6d61   stack_para["rma
+00009bf0: 5f73 7465 7022 5d0a 2020 2020 7374 6172  _step"].    star
+00009c00: 745f 6461 7465 203d 2073 7461 636b 5f70  t_date = stack_p
+00009c10: 6172 615b 2273 7461 7274 5f64 6174 6522  ara["start_date"
+00009c20: 5d0a 2020 2020 656e 645f 6461 7465 203d  ].    end_date =
+00009c30: 2073 7461 636b 5f70 6172 615b 2265 6e64   stack_para["end
+00009c40: 5f64 6174 6522 5d0a 2020 2020 6e70 7473  _date"].    npts
+00009c50: 203d 2063 635f 6172 7261 792e 7368 6170   = cc_array.shap
+00009c60: 655b 315d 0a0a 2020 2020 2320 7265 6d6f  e[1]..    # remo
+00009c70: 7665 2061 626e 6f72 6d61 6c20 6461 7461  ve abnormal data
+00009c80: 0a20 2020 2061 6d70 6d61 7820 3d20 6e70  .    ampmax = np
+00009c90: 2e6d 6178 2863 635f 6172 7261 792c 2061  .max(cc_array, a
+00009ca0: 7869 733d 3129 0a20 2020 2074 696e 6478  xis=1).    tindx
+00009cb0: 203d 206e 702e 7768 6572 6528 2861 6d70   = np.where((amp
+00009cc0: 6d61 7820 3c20 3230 202a 206e 702e 6d65  max < 20 * np.me
+00009cd0: 6469 616e 2861 6d70 6d61 7829 2920 2620  dian(ampmax)) & 
+00009ce0: 2861 6d70 6d61 7820 3e20 3029 295b 305d  (ampmax > 0))[0]
+00009cf0: 0a20 2020 2069 6620 6e6f 7420 6c65 6e28  .    if not len(
+00009d00: 7469 6e64 7829 3a0a 2020 2020 2020 2020  tindx):.        
+00009d10: 616c 6c73 7461 636b 7331 203d 205b 5d0a  allstacks1 = [].
+00009d20: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
+00009d30: 7332 203d 205b 5d0a 2020 2020 2020 2020  s2 = [].        
+00009d40: 6e73 7461 636b 7320 3d20 300a 2020 2020  nstacks = 0.    
+00009d50: 2020 2020 6363 5f61 7272 6179 203d 205b      cc_array = [
+00009d60: 5d0a 2020 2020 2020 2020 6363 5f6e 676f  ].        cc_ngo
+00009d70: 6f64 203d 205b 5d0a 2020 2020 2020 2020  od = [].        
+00009d80: 6363 5f74 696d 6520 3d20 5b5d 0a20 2020  cc_time = [].   
+00009d90: 2020 2020 2072 6574 7572 6e20 6363 5f61       return cc_a
+00009da0: 7272 6179 2c20 6363 5f6e 676f 6f64 2c20  rray, cc_ngood, 
+00009db0: 6363 5f74 696d 652c 2061 6c6c 7374 6163  cc_time, allstac
+00009dc0: 6b73 312c 2061 6c6c 7374 6163 6b73 322c  ks1, allstacks2,
+00009dd0: 206e 7374 6163 6b73 0a20 2020 2065 6c73   nstacks.    els
+00009de0: 653a 0a20 2020 2020 2020 2023 2072 656d  e:.        # rem
+00009df0: 6f76 6520 6f6e 6573 2077 6974 6820 6261  ove ones with ba
+00009e00: 6420 616d 706c 6974 7564 650a 2020 2020  d amplitude.    
+00009e10: 2020 2020 6363 5f61 7272 6179 203d 2063      cc_array = c
+00009e20: 635f 6172 7261 795b 7469 6e64 782c 203a  c_array[tindx, :
+00009e30: 5d0a 2020 2020 2020 2020 6363 5f74 696d  ].        cc_tim
+00009e40: 6520 3d20 6363 5f74 696d 655b 7469 6e64  e = cc_time[tind
+00009e50: 785d 0a20 2020 2020 2020 2063 635f 6e67  x].        cc_ng
+00009e60: 6f6f 6420 3d20 6363 5f6e 676f 6f64 5b74  ood = cc_ngood[t
+00009e70: 696e 6478 5d0a 0a20 2020 2020 2020 2023  indx]..        #
+00009e80: 2064 6f20 7375 6273 7461 636b 730a 2020   do substacks.  
+00009e90: 2020 2020 2020 6966 2072 6d61 5f73 7562        if rma_sub
+00009ea0: 7374 6163 6b3a 0a20 2020 2020 2020 2020  stack:.         
+00009eb0: 2020 2074 7374 6172 7420 3d20 6f62 7370     tstart = obsp
+00009ec0: 792e 5554 4344 6174 6554 696d 6528 7374  y.UTCDateTime(st
+00009ed0: 6172 745f 6461 7465 2920 2d20 6f62 7370  art_date) - obsp
+00009ee0: 792e 5554 4344 6174 6554 696d 6528 3139  y.UTCDateTime(19
+00009ef0: 3730 2c20 312c 2031 290a 2020 2020 2020  70, 1, 1).      
+00009f00: 2020 2020 2020 7465 6e64 203d 206f 6273        tend = obs
+00009f10: 7079 2e55 5443 4461 7465 5469 6d65 2865  py.UTCDateTime(e
+00009f20: 6e64 5f64 6174 6529 202d 206f 6273 7079  nd_date) - obspy
+00009f30: 2e55 5443 4461 7465 5469 6d65 2831 3937  .UTCDateTime(197
+00009f40: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
+00009f50: 2020 2020 2074 7469 6d65 203d 2074 7374       ttime = tst
+00009f60: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
+00009f70: 6e73 7461 636b 203d 2069 6e74 286e 702e  nstack = int(np.
+00009f80: 726f 756e 6428 2874 656e 6420 2d20 7473  round((tend - ts
+00009f90: 7461 7274 2920 2f20 2872 6d61 5f73 7465  tart) / (rma_ste
+00009fa0: 7020 2a20 3336 3030 2929 290a 2020 2020  p * 3600))).    
+00009fb0: 2020 2020 2020 2020 6e63 635f 6172 7261          ncc_arra
+00009fc0: 7920 3d20 6e70 2e7a 6572 6f73 2873 6861  y = np.zeros(sha
+00009fd0: 7065 3d28 6e73 7461 636b 2c20 6e70 7473  pe=(nstack, npts
+00009fe0: 292c 2064 7479 7065 3d6e 702e 666c 6f61  ), dtype=np.floa
+00009ff0: 7433 3229 0a20 2020 2020 2020 2020 2020  t32).           
+0000a000: 206e 6363 5f74 696d 6520 3d20 6e70 2e7a   ncc_time = np.z
+0000a010: 6572 6f73 286e 7374 6163 6b2c 2064 7479  eros(nstack, dty
+0000a020: 7065 3d6e 702e 666c 6f61 7429 0a20 2020  pe=np.float).   
+0000a030: 2020 2020 2020 2020 206e 6363 5f6e 676f           ncc_ngo
+0000a040: 6f64 203d 206e 702e 7a65 726f 7328 6e73  od = np.zeros(ns
+0000a050: 7461 636b 2c20 6474 7970 653d 6e70 2e69  tack, dtype=np.i
+0000a060: 6e74 290a 0a20 2020 2020 2020 2020 2020  nt)..           
+0000a070: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
+0000a080: 6561 6368 2074 696d 650a 2020 2020 2020  each time.      
+0000a090: 2020 2020 2020 666f 7220 6969 2069 6e20        for ii in 
+0000a0a0: 7261 6e67 6528 6e73 7461 636b 293a 0a20  range(nstack):. 
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a0c0: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
+0000a0d0: 2863 635f 7469 6d65 203e 3d20 7474 696d  (cc_time >= ttim
+0000a0e0: 6529 2026 2028 6363 5f74 696d 6520 3c20  e) & (cc_time < 
+0000a0f0: 7474 696d 6520 2b20 726d 615f 7375 6273  ttime + rma_subs
+0000a100: 7461 636b 202a 2033 3630 3029 295b 305d  tack * 3600))[0]
+0000a110: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a120: 2020 2320 7768 656e 2074 6865 7265 2061    # when there a
+0000a130: 7265 2064 6174 6120 696e 2074 6865 2074  re data in the t
+0000a140: 696d 6520 7769 6e64 6f77 0a20 2020 2020  ime window.     
+0000a150: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000a160: 6e28 7369 6e64 7829 3a0a 2020 2020 2020  n(sindx):.      
+0000a170: 2020 2020 2020 2020 2020 2020 2020 6e63                nc
+0000a180: 635f 6172 7261 795b 6969 5d20 3d20 6e70  c_array[ii] = np
+0000a190: 2e6d 6561 6e28 6363 5f61 7272 6179 5b73  .mean(cc_array[s
+0000a1a0: 696e 6478 5d2c 2061 7869 733d 3029 0a20  indx], axis=0). 
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 2020 206e 6363 5f74 696d 655b 6969 5d20     ncc_time[ii] 
+0000a1d0: 3d20 7474 696d 650a 2020 2020 2020 2020  = ttime.        
+0000a1e0: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
+0000a1f0: 6e67 6f6f 645b 6969 5d20 3d20 6e70 2e73  ngood[ii] = np.s
+0000a200: 756d 2863 635f 6e67 6f6f 645b 7369 6e64  um(cc_ngood[sind
+0000a210: 785d 2c20 6178 6973 3d30 290a 2020 2020  x], axis=0).    
+0000a220: 2020 2020 2020 2020 2020 2020 7474 696d              ttim
+0000a230: 6520 2b3d 2072 6d61 5f73 7465 7020 2a20  e += rma_step * 
+0000a240: 3336 3030 0a0a 2020 2020 2020 2020 2020  3600..          
+0000a250: 2020 2320 7265 6d6f 7665 2062 6164 206f    # remove bad o
+0000a260: 6e65 730a 2020 2020 2020 2020 2020 2020  nes.            
+0000a270: 7469 6e64 7820 3d20 6e70 2e77 6865 7265  tindx = np.where
+0000a280: 286e 6363 5f6e 676f 6f64 203e 2030 295b  (ncc_ngood > 0)[
+0000a290: 305d 0a20 2020 2020 2020 2020 2020 206e  0].            n
+0000a2a0: 6363 5f61 7272 6179 203d 206e 6363 5f61  cc_array = ncc_a
+0000a2b0: 7272 6179 5b74 696e 6478 5d0a 2020 2020  rray[tindx].    
+0000a2c0: 2020 2020 2020 2020 6e63 635f 7469 6d65          ncc_time
+0000a2d0: 203d 206e 6363 5f74 696d 655b 7469 6e64   = ncc_time[tind
+0000a2e0: 785d 0a20 2020 2020 2020 2020 2020 206e  x].            n
+0000a2f0: 6363 5f6e 676f 6f64 203d 206e 6363 5f6e  cc_ngood = ncc_n
+0000a300: 676f 6f64 5b74 696e 6478 5d0a 0a20 2020  good[tindx]..   
+0000a310: 2020 2020 2023 2064 6f20 7374 6163 6b69       # do stacki
+0000a320: 6e67 0a20 2020 2020 2020 2061 6c6c 7374  ng.        allst
+0000a330: 6163 6b73 3120 3d20 6e70 2e7a 6572 6f73  acks1 = np.zeros
+0000a340: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
+0000a350: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
+0000a360: 2061 6c6c 7374 6163 6b73 3220 3d20 6e70   allstacks2 = np
+0000a370: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
+0000a380: 7065 3d6e 702e 666c 6f61 7433 3229 0a20  pe=np.float32). 
+0000a390: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
+0000a3a0: 3320 3d20 6e70 2e7a 6572 6f73 286e 7074  3 = np.zeros(npt
+0000a3b0: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
+0000a3c0: 7433 3229 0a20 2020 2020 2020 2061 6c6c  t32).        all
+0000a3d0: 7374 6163 6b73 3420 3d20 6e70 2e7a 6572  stacks4 = np.zer
+0000a3e0: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
+0000a3f0: 702e 666c 6f61 7433 3229 0a0a 2020 2020  p.float32)..    
+0000a400: 2020 2020 6966 2073 6d65 7468 6f64 203d      if smethod =
+0000a410: 3d20 5374 6163 6b4d 6574 686f 642e 4c49  = StackMethod.LI
+0000a420: 4e45 4152 3a0a 2020 2020 2020 2020 2020  NEAR:.          
+0000a430: 2020 616c 6c73 7461 636b 7331 203d 206e    allstacks1 = n
+0000a440: 702e 6d65 616e 2863 635f 6172 7261 792c  p.mean(cc_array,
+0000a450: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+0000a460: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
+0000a470: 2053 7461 636b 4d65 7468 6f64 2e50 5753   StackMethod.PWS
+0000a480: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+0000a490: 6c73 7461 636b 7331 203d 2070 7773 2863  lstacks1 = pws(c
+0000a4a0: 635f 6172 7261 792c 2073 616d 705f 6672  c_array, samp_fr
+0000a4b0: 6571 290a 2020 2020 2020 2020 656c 6966  eq).        elif
+0000a4c0: 2073 6d65 7468 6f64 203d 3d20 5374 6163   smethod == Stac
+0000a4d0: 6b4d 6574 686f 642e 524f 4255 5354 3a0a  kMethod.ROBUST:.
+0000a4e0: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+0000a500: 6c73 7461 636b 7331 2c0a 2020 2020 2020  lstacks1,.      
+0000a510: 2020 2020 2020 2020 2020 772c 0a20 2020            w,.   
+0000a520: 2020 2020 2020 2020 2029 203d 2072 6f62           ) = rob
+0000a530: 7573 745f 7374 6163 6b28 6363 5f61 7272  ust_stack(cc_arr
+0000a540: 6179 2c20 302e 3030 3129 0a20 2020 2020  ay, 0.001).     
+0000a550: 2020 2065 6c69 6620 736d 6574 686f 6420     elif smethod 
+0000a560: 3d3d 2053 7461 636b 4d65 7468 6f64 2e53  == StackMethod.S
+0000a570: 454c 4543 5449 5645 3a0a 2020 2020 2020  ELECTIVE:.      
+0000a580: 2020 2020 2020 616c 6c73 7461 636b 7331        allstacks1
+0000a590: 203d 2073 656c 6563 7469 7665 5f73 7461   = selective_sta
+0000a5a0: 636b 2863 635f 6172 7261 792c 2030 2e30  ck(cc_array, 0.0
+0000a5b0: 3031 290a 2020 2020 2020 2020 656c 6966  01).        elif
+0000a5c0: 2073 6d65 7468 6f64 203d 3d20 5374 6163   smethod == Stac
+0000a5d0: 6b4d 6574 686f 642e 414c 4c3a 0a20 2020  kMethod.ALL:.   
+0000a5e0: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
+0000a5f0: 6b73 3120 3d20 6e70 2e6d 6561 6e28 6363  ks1 = np.mean(cc
+0000a600: 5f61 7272 6179 2c20 6178 6973 3d30 290a  _array, axis=0).
+0000a610: 2020 2020 2020 2020 2020 2020 616c 6c73              alls
+0000a620: 7461 636b 7332 203d 2070 7773 2863 635f  tacks2 = pws(cc_
+0000a630: 6172 7261 792c 2073 616d 705f 6672 6571  array, samp_freq
+0000a640: 290a 2020 2020 2020 2020 2020 2020 616c  ).            al
+0000a650: 6c73 7461 636b 7333 203d 2072 6f62 7573  lstacks3 = robus
+0000a660: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
+0000a670: 2c20 302e 3030 3129 0a20 2020 2020 2020  , 0.001).       
+0000a680: 2020 2020 2061 6c6c 7374 6163 6b73 3420       allstacks4 
+0000a690: 3d20 7365 6c65 6374 6976 655f 7374 6163  = selective_stac
+0000a6a0: 6b28 6363 5f61 7272 6179 2c20 302e 3030  k(cc_array, 0.00
+0000a6b0: 3129 0a20 2020 2020 2020 206e 7374 6163  1).        nstac
+0000a6c0: 6b73 203d 206e 702e 7375 6d28 6363 5f6e  ks = np.sum(cc_n
+0000a6d0: 676f 6f64 290a 0a20 2020 2023 2072 6570  good)..    # rep
+0000a6e0: 6c61 6365 2074 6865 2061 7272 6179 2066  lace the array f
+0000a6f0: 6f72 2073 7562 7374 6163 6b73 0a20 2020  or substacks.   
+0000a700: 2069 6620 726d 615f 7375 6273 7461 636b   if rma_substack
+0000a710: 3a0a 2020 2020 2020 2020 6363 5f61 7272  :.        cc_arr
+0000a720: 6179 203d 206e 6363 5f61 7272 6179 0a20  ay = ncc_array. 
+0000a730: 2020 2020 2020 2063 635f 7469 6d65 203d         cc_time =
+0000a740: 206e 6363 5f74 696d 650a 2020 2020 2020   ncc_time.      
+0000a750: 2020 6363 5f6e 676f 6f64 203d 206e 6363    cc_ngood = ncc
+0000a760: 5f6e 676f 6f64 0a0a 2020 2020 2320 676f  _ngood..    # go
+0000a770: 6f64 2074 6f20 7265 7475 726e 0a20 2020  od to return.   
+0000a780: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
+0000a790: 2020 6363 5f61 7272 6179 2c0a 2020 2020    cc_array,.    
+0000a7a0: 2020 2020 6363 5f6e 676f 6f64 2c0a 2020      cc_ngood,.  
+0000a7b0: 2020 2020 2020 6363 5f74 696d 652c 0a20        cc_time,. 
+0000a7c0: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
+0000a7d0: 312c 0a20 2020 2020 2020 2061 6c6c 7374  1,.        allst
+0000a7e0: 6163 6b73 322c 0a20 2020 2020 2020 2061  acks2,.        a
+0000a7f0: 6c6c 7374 6163 6b73 332c 0a20 2020 2020  llstacks3,.     
+0000a800: 2020 2061 6c6c 7374 6163 6b73 342c 0a20     allstacks4,. 
+0000a810: 2020 2020 2020 206e 7374 6163 6b73 2c0a         nstacks,.
+0000a820: 2020 2020 290a 0a0a 6465 6620 726f 7461      )...def rota
+0000a830: 7469 6f6e 2862 6967 7374 6163 6b2c 2070  tion(bigstack, p
+0000a840: 6172 616d 6574 6572 732c 206c 6f63 7329  arameters, locs)
+0000a850: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+0000a860: 6973 2066 756e 6374 696f 6e20 7472 616e  is function tran
+0000a870: 7366 6572 7320 7468 6520 4772 6565 6e27  sfers the Green'
+0000a880: 7320 7465 6e73 6f72 2066 726f 6d20 6120  s tensor from a 
+0000a890: 452d 4e2d 5a20 7379 7374 656d 2069 6e74  E-N-Z system int
+0000a8a0: 6f20 6120 522d 542d 5a20 6f6e 650a 0a20  o a R-T-Z one.. 
+0000a8b0: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+0000a8c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000a8d0: 2d2d 2d2d 2d2d 0a20 2020 2062 6967 7374  ------.    bigst
+0000a8e0: 6163 6b3a 2020 2039 2063 6f6d 706f 6e65  ack:   9 compone
+0000a8f0: 6e74 2047 7265 656e 2773 2074 656e 736f  nt Green's tenso
+0000a900: 7220 696e 2045 2d4e 2d5a 2073 7973 7465  r in E-N-Z syste
+0000a910: 6d0a 2020 2020 7061 7261 6d65 7465 7273  m.    parameters
+0000a920: 3a20 6469 6374 2063 6f6e 7461 696e 696e  : dict containin
+0000a930: 6720 616c 6c20 7061 7261 6d65 7465 7273  g all parameters
+0000a940: 2073 6176 6564 2069 6e20 4153 4446 2066   saved in ASDF f
+0000a950: 696c 650a 2020 2020 6c6f 6373 3a20 2020  ile.    locs:   
+0000a960: 2020 2020 6469 6374 2063 6f6e 7461 696e      dict contain
+0000a970: 696e 6720 7374 6174 696f 6e20 616e 676c  ing station angl
+0000a980: 6520 696e 666f 2066 6f72 2063 6f72 7265  e info for corre
+0000a990: 6374 696f 6e20 7075 7270 6f73 650a 2020  ction purpose.  
+0000a9a0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
+0000a9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a9c0: 2d2d 0a20 2020 2074 636f 7272 3a20 3920  --.    tcorr: 9 
+0000a9d0: 636f 6d70 6f6e 656e 7420 4772 6565 6e27  component Green'
+0000a9e0: 7320 7465 6e73 6f72 2069 6e20 522d 542d  s tensor in R-T-
+0000a9f0: 5a20 7379 7374 656d 0a20 2020 2022 2222  Z system.    """
+0000aa00: 0a20 2020 2023 206c 6f61 6420 7061 7261  .    # load para
+0000aa10: 6d65 7465 7220 6469 630a 2020 2020 7069  meter dic.    pi
+0000aa20: 203d 206e 702e 7069 0a20 2020 2061 7a69   = np.pi.    azi
+0000aa30: 203d 2070 6172 616d 6574 6572 735b 2261   = parameters["a
+0000aa40: 7a69 225d 0a20 2020 2062 617a 203d 2070  zi"].    baz = p
+0000aa50: 6172 616d 6574 6572 735b 2262 617a 225d  arameters["baz"]
+0000aa60: 0a20 2020 206e 636f 6d70 2c20 6e70 7473  .    ncomp, npts
+0000aa70: 203d 2062 6967 7374 6163 6b2e 7368 6170   = bigstack.shap
+0000aa80: 650a 2020 2020 6966 206e 636f 6d70 203c  e.    if ncomp <
+0000aa90: 2039 3a0a 2020 2020 2020 2020 6c6f 6767   9:.        logg
+0000aaa0: 6572 2e64 6562 7567 2822 6372 6170 2064  er.debug("crap d
+0000aab0: 6964 206e 6f74 2067 6574 2065 6e6f 7567  id not get enoug
+0000aac0: 6820 636f 6d70 6f6e 656e 7473 2229 0a20  h components"). 
+0000aad0: 2020 2020 2020 2074 636f 7272 203d 205b         tcorr = [
+0000aae0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+0000aaf0: 2074 636f 7272 0a20 2020 2073 7461 5320   tcorr.    staS 
+0000ab00: 3d20 7061 7261 6d65 7465 7273 5b22 7374  = parameters["st
+0000ab10: 6174 696f 6e5f 736f 7572 6365 225d 0a20  ation_source"]. 
+0000ab20: 2020 2073 7461 5220 3d20 7061 7261 6d65     staR = parame
+0000ab30: 7465 7273 5b22 7374 6174 696f 6e5f 7265  ters["station_re
+0000ab40: 6365 6976 6572 225d 0a0a 2020 2020 6966  ceiver"]..    if
+0000ab50: 206c 656e 286c 6f63 7329 3a0a 2020 2020   len(locs):.    
+0000ab60: 2020 2020 7374 615f 6c69 7374 203d 206c      sta_list = l
+0000ab70: 6973 7428 6c6f 6373 5b22 7374 6174 696f  ist(locs["statio
+0000ab80: 6e22 5d29 0a20 2020 2020 2020 2061 6e67  n"]).        ang
+0000ab90: 6c65 7320 3d20 6c69 7374 286c 6f63 735b  les = list(locs[
+0000aba0: 2261 6e67 6c65 225d 290a 2020 2020 2020  "angle"]).      
+0000abb0: 2020 2320 6765 7420 7374 6174 696f 6e20    # get station 
+0000abc0: 696e 666f 2066 726f 6d20 7468 6520 6e61  info from the na
+0000abd0: 6d65 206f 6620 4153 4446 2066 696c 650a  me of ASDF file.
+0000abe0: 2020 2020 2020 2020 696e 6420 3d20 7374          ind = st
+0000abf0: 615f 6c69 7374 2e69 6e64 6578 2873 7461  a_list.index(sta
+0000ac00: 5329 0a20 2020 2020 2020 2061 636f 7272  S).        acorr
+0000ac10: 203d 2061 6e67 6c65 735b 696e 645d 0a20   = angles[ind]. 
+0000ac20: 2020 2020 2020 2069 6e64 203d 2073 7461         ind = sta
+0000ac30: 5f6c 6973 742e 696e 6465 7828 7374 6152  _list.index(staR
+0000ac40: 290a 2020 2020 2020 2020 6263 6f72 7220  ).        bcorr 
+0000ac50: 3d20 616e 676c 6573 5b69 6e64 5d0a 0a20  = angles[ind].. 
+0000ac60: 2020 2023 202d 2d2d 616e 676c 6573 2074     # ---angles t
+0000ac70: 6f20 6265 2063 6f72 7265 6374 6564 2d2d  o be corrected--
+0000ac80: 2d2d 0a20 2020 2069 6620 6c65 6e28 6c6f  --.    if len(lo
+0000ac90: 6373 293a 0a20 2020 2020 2020 2063 6f73  cs):.        cos
+0000aca0: 6120 3d20 6e70 2e63 6f73 2828 617a 6920  a = np.cos((azi 
+0000acb0: 2b20 6163 6f72 7229 202a 2070 6920 2f20  + acorr) * pi / 
+0000acc0: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
+0000acd0: 6120 3d20 6e70 2e73 696e 2828 617a 6920  a = np.sin((azi 
+0000ace0: 2b20 6163 6f72 7229 202a 2070 6920 2f20  + acorr) * pi / 
+0000acf0: 3138 3029 0a20 2020 2020 2020 2063 6f73  180).        cos
+0000ad00: 6220 3d20 6e70 2e63 6f73 2828 6261 7a20  b = np.cos((baz 
+0000ad10: 2b20 6263 6f72 7229 202a 2070 6920 2f20  + bcorr) * pi / 
+0000ad20: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
+0000ad30: 6220 3d20 6e70 2e73 696e 2828 6261 7a20  b = np.sin((baz 
+0000ad40: 2b20 6263 6f72 7229 202a 2070 6920 2f20  + bcorr) * pi / 
+0000ad50: 3138 3029 0a20 2020 2065 6c73 653a 0a20  180).    else:. 
+0000ad60: 2020 2020 2020 2063 6f73 6120 3d20 6e70         cosa = np
+0000ad70: 2e63 6f73 2861 7a69 202a 2070 6920 2f20  .cos(azi * pi / 
+0000ad80: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
+0000ad90: 6120 3d20 6e70 2e73 696e 2861 7a69 202a  a = np.sin(azi *
+0000ada0: 2070 6920 2f20 3138 3029 0a20 2020 2020   pi / 180).     
+0000adb0: 2020 2063 6f73 6220 3d20 6e70 2e63 6f73     cosb = np.cos
+0000adc0: 2862 617a 202a 2070 6920 2f20 3138 3029  (baz * pi / 180)
+0000add0: 0a20 2020 2020 2020 2073 696e 6220 3d20  .        sinb = 
+0000ade0: 6e70 2e73 696e 2862 617a 202a 2070 6920  np.sin(baz * pi 
+0000adf0: 2f20 3138 3029 0a0a 2020 2020 2320 7274  / 180)..    # rt
+0000ae00: 7a5f 636f 6d70 6f6e 656e 7473 203d 205b  z_components = [
+0000ae10: 275a 5227 2c27 5a54 272c 275a 5a27 2c27  'ZR','ZT','ZZ','
+0000ae20: 5252 272c 2752 5427 2c27 525a 272c 2754  RR','RT','RZ','T
+0000ae30: 5227 2c27 5454 272c 2754 5a27 5d0a 2020  R','TT','TZ'].  
+0000ae40: 2020 7463 6f72 7220 3d20 6e70 2e7a 6572    tcorr = np.zer
+0000ae50: 6f73 2873 6861 7065 3d28 392c 206e 7074  os(shape=(9, npt
+0000ae60: 7329 2c20 6474 7970 653d 6e70 2e66 6c6f  s), dtype=np.flo
+0000ae70: 6174 3332 290a 2020 2020 7463 6f72 725b  at32).    tcorr[
+0000ae80: 305d 203d 202d 636f 7362 202a 2062 6967  0] = -cosb * big
+0000ae90: 7374 6163 6b5b 375d 202d 2073 696e 6220  stack[7] - sinb 
+0000aea0: 2a20 6269 6773 7461 636b 5b36 5d0a 2020  * bigstack[6].  
+0000aeb0: 2020 7463 6f72 725b 315d 203d 2073 696e    tcorr[1] = sin
+0000aec0: 6220 2a20 6269 6773 7461 636b 5b37 5d20  b * bigstack[7] 
+0000aed0: 2d20 636f 7362 202a 2062 6967 7374 6163  - cosb * bigstac
+0000aee0: 6b5b 365d 0a20 2020 2074 636f 7272 5b32  k[6].    tcorr[2
+0000aef0: 5d20 3d20 6269 6773 7461 636b 5b38 5d0a  ] = bigstack[8].
+0000af00: 2020 2020 7463 6f72 725b 335d 203d 2028      tcorr[3] = (
+0000af10: 0a20 2020 2020 2020 202d 636f 7361 202a  .        -cosa *
+0000af20: 2063 6f73 6220 2a20 6269 6773 7461 636b   cosb * bigstack
+0000af30: 5b34 5d20 2d20 636f 7361 202a 2073 696e  [4] - cosa * sin
+0000af40: 6220 2a20 6269 6773 7461 636b 5b33 5d20  b * bigstack[3] 
+0000af50: 2d20 7369 6e61 202a 2063 6f73 6220 2a20  - sina * cosb * 
+0000af60: 6269 6773 7461 636b 5b31 5d20 2d20 7369  bigstack[1] - si
+0000af70: 6e61 202a 2073 696e 6220 2a20 6269 6773  na * sinb * bigs
+0000af80: 7461 636b 5b30 5d0a 2020 2020 290a 2020  tack[0].    ).  
+0000af90: 2020 7463 6f72 725b 345d 203d 2028 0a20    tcorr[4] = (. 
+0000afa0: 2020 2020 2020 2063 6f73 6120 2a20 7369         cosa * si
+0000afb0: 6e62 202a 2062 6967 7374 6163 6b5b 345d  nb * bigstack[4]
+0000afc0: 202d 2063 6f73 6120 2a20 636f 7362 202a   - cosa * cosb *
+0000afd0: 2062 6967 7374 6163 6b5b 335d 202b 2073   bigstack[3] + s
+0000afe0: 696e 6120 2a20 7369 6e62 202a 2062 6967  ina * sinb * big
+0000aff0: 7374 6163 6b5b 315d 202d 2073 696e 6120  stack[1] - sina 
+0000b000: 2a20 636f 7362 202a 2062 6967 7374 6163  * cosb * bigstac
+0000b010: 6b5b 305d 0a20 2020 2029 0a20 2020 2074  k[0].    ).    t
+0000b020: 636f 7272 5b35 5d20 3d20 636f 7361 202a  corr[5] = cosa *
+0000b030: 2062 6967 7374 6163 6b5b 355d 202b 2073   bigstack[5] + s
+0000b040: 696e 6120 2a20 6269 6773 7461 636b 5b32  ina * bigstack[2
+0000b050: 5d0a 2020 2020 7463 6f72 725b 365d 203d  ].    tcorr[6] =
+0000b060: 2028 0a20 2020 2020 2020 2073 696e 6120   (.        sina 
+0000b070: 2a20 636f 7362 202a 2062 6967 7374 6163  * cosb * bigstac
+0000b080: 6b5b 345d 202b 2073 696e 6120 2a20 7369  k[4] + sina * si
+0000b090: 6e62 202a 2062 6967 7374 6163 6b5b 335d  nb * bigstack[3]
+0000b0a0: 202d 2063 6f73 6120 2a20 636f 7362 202a   - cosa * cosb *
+0000b0b0: 2062 6967 7374 6163 6b5b 315d 202d 2063   bigstack[1] - c
+0000b0c0: 6f73 6120 2a20 7369 6e62 202a 2062 6967  osa * sinb * big
+0000b0d0: 7374 6163 6b5b 305d 0a20 2020 2029 0a20  stack[0].    ). 
+0000b0e0: 2020 2074 636f 7272 5b37 5d20 3d20 280a     tcorr[7] = (.
+0000b0f0: 2020 2020 2020 2020 2d73 696e 6120 2a20          -sina * 
+0000b100: 7369 6e62 202a 2062 6967 7374 6163 6b5b  sinb * bigstack[
+0000b110: 345d 202b 2073 696e 6120 2a20 636f 7362  4] + sina * cosb
+0000b120: 202a 2062 6967 7374 6163 6b5b 335d 202b   * bigstack[3] +
+0000b130: 2063 6f73 6120 2a20 7369 6e62 202a 2062   cosa * sinb * b
+0000b140: 6967 7374 6163 6b5b 315d 202d 2063 6f73  igstack[1] - cos
+0000b150: 6120 2a20 636f 7362 202a 2062 6967 7374  a * cosb * bigst
+0000b160: 6163 6b5b 305d 0a20 2020 2029 0a20 2020  ack[0].    ).   
+0000b170: 2074 636f 7272 5b38 5d20 3d20 2d73 696e   tcorr[8] = -sin
+0000b180: 6120 2a20 6269 6773 7461 636b 5b35 5d20  a * bigstack[5] 
+0000b190: 2b20 636f 7361 202a 2062 6967 7374 6163  + cosa * bigstac
+0000b1a0: 6b5b 325d 0a0a 2020 2020 7265 7475 726e  k[2]..    return
+0000b1b0: 2074 636f 7272 0a0a 0a23 2323 2323 2323   tcorr...#######
 0000b1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000b1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b1e0: 230a 2323 2323 2323 2323 2323 2323 2323  #.##############
-0000b1f0: 2055 5449 4c49 5459 2046 554e 4354 494f   UTILITY FUNCTIO
-0000b200: 4e53 2023 2323 2323 2323 2323 2323 2323  NS #############
-0000b210: 2323 2323 2323 0a23 2323 2323 2323 2323  ######.#########
-0000b220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b1e0: 2323 2323 2323 2323 2323 2323 230a 2323  #############.##
+0000b1f0: 2323 2323 2323 2323 2323 2323 2055 5449  ############ UTI
+0000b200: 4c49 5459 2046 554e 4354 494f 4e53 2023  LITY FUNCTIONS #
+0000b210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b220: 2323 0a23 2323 2323 2323 2323 2323 2323  ##.#############
 0000b230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b240: 2323 2323 2323 2323 2323 230a 0a0a 6465  ###########...de
-0000b250: 6620 6368 6563 6b5f 7361 6d70 6c65 5f67  f check_sample_g
-0000b260: 6170 7328 7374 7265 616d 3a20 6f62 7370  aps(stream: obsp
-0000b270: 792e 5374 7265 616d 2c20 7374 6172 7474  y.Stream, startt
-0000b280: 696d 653a 206f 6273 7079 2e55 5443 4461  ime: obspy.UTCDa
-0000b290: 7465 5469 6d65 2c20 656e 6474 696d 653a  teTime, endtime:
-0000b2a0: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
-0000b2b0: 6d65 293a 0a20 2020 2022 2222 0a20 2020  me):.    """.   
-0000b2c0: 2074 6869 7320 6675 6e63 7469 6f6e 2063   this function c
-0000b2d0: 6865 636b 7320 7361 6d70 6c69 6e67 2072  hecks sampling r
-0000b2e0: 6174 6520 616e 6420 6669 6e64 2067 6170  ate and find gap
-0000b2f0: 7320 6f66 2061 6c6c 2074 7261 6365 7320  s of all traces 
-0000b300: 696e 2073 7472 6561 6d2e 0a20 2020 2050  in stream..    P
-0000b310: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
-0000b320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b330: 0a20 2020 2073 7472 6561 6d3a 206f 6273  .    stream: obs
-0000b340: 7079 2073 7472 6561 6d20 6f62 6a65 6374  py stream object
-0000b350: 2e0a 2020 2020 6461 7465 5f69 6e66 6f3a  ..    date_info:
-0000b360: 2064 6963 7420 6f66 2073 7461 7274 696e   dict of startin
-0000b370: 6720 616e 6420 656e 6469 6e67 2074 696d  g and ending tim
-0000b380: 6520 6f66 2074 6865 2073 7472 6561 6d0a  e of the stream.
-0000b390: 0a20 2020 2052 4554 5552 454e 533a 0a20  .    RETURENS:. 
-0000b3a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000b3b0: 2d2d 2d2d 0a20 2020 2073 7472 6561 6d3a  ----.    stream:
-0000b3c0: 204c 6973 7420 6f66 2067 6f6f 6420 7472   List of good tr
-0000b3d0: 6163 6573 2069 6e20 7468 6520 7374 7265  aces in the stre
-0000b3e0: 616d 0a20 2020 2022 2222 0a20 2020 2023  am.    """.    #
-0000b3f0: 2072 656d 6f76 6520 656d 7074 792f 6269   remove empty/bi
-0000b400: 6720 7472 6163 6573 0a20 2020 2069 6620  g traces.    if 
-0000b410: 6c65 6e28 7374 7265 616d 2920 3d3d 2030  len(stream) == 0
-0000b420: 206f 7220 6c65 6e28 7374 7265 616d 2920   or len(stream) 
-0000b430: 3e20 3130 303a 0a20 2020 2020 2020 2073  > 100:.        s
-0000b440: 7472 6561 6d20 3d20 5b5d 0a20 2020 2020  tream = [].     
-0000b450: 2020 2072 6574 7572 6e20 7374 7265 616d     return stream
-0000b460: 0a0a 2020 2020 2320 7265 6d6f 7665 2074  ..    # remove t
-0000b470: 7261 6365 7320 7769 7468 2062 6967 2067  races with big g
-0000b480: 6170 730a 2020 2020 6966 2070 6f72 7469  aps.    if porti
-0000b490: 6f6e 5f67 6170 7328 7374 7265 616d 2c20  on_gaps(stream, 
-0000b4a0: 7374 6172 7474 696d 652c 2065 6e64 7469  starttime, endti
-0000b4b0: 6d65 2920 3e20 302e 333a 0a20 2020 2020  me) > 0.3:.     
-0000b4c0: 2020 2073 7472 6561 6d20 3d20 5b5d 0a20     stream = []. 
-0000b4d0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-0000b4e0: 7265 616d 0a0a 2020 2020 6672 6571 7320  ream..    freqs 
-0000b4f0: 3d20 5b5d 0a20 2020 2066 6f72 2074 7220  = [].    for tr 
-0000b500: 696e 2073 7472 6561 6d3a 0a20 2020 2020  in stream:.     
-0000b510: 2020 2066 7265 7173 2e61 7070 656e 6428     freqs.append(
-0000b520: 696e 7428 7472 2e73 7461 7473 2e73 616d  int(tr.stats.sam
-0000b530: 706c 696e 675f 7261 7465 2929 0a20 2020  pling_rate)).   
-0000b540: 2066 7265 7120 3d20 6d61 7828 6672 6571   freq = max(freq
-0000b550: 7329 0a20 2020 2066 6f72 2074 7220 696e  s).    for tr in
-0000b560: 2073 7472 6561 6d3a 0a20 2020 2020 2020   stream:.       
-0000b570: 2069 6620 696e 7428 7472 2e73 7461 7473   if int(tr.stats
-0000b580: 2e73 616d 706c 696e 675f 7261 7465 2920  .sampling_rate) 
-0000b590: 213d 2066 7265 713a 0a20 2020 2020 2020  != freq:.       
-0000b5a0: 2020 2020 2073 7472 6561 6d2e 7265 6d6f       stream.remo
-0000b5b0: 7665 2874 7229 0a20 2020 2020 2020 2069  ve(tr).        i
-0000b5c0: 6620 7472 2e73 7461 7473 2e6e 7074 7320  f tr.stats.npts 
-0000b5d0: 3c20 3130 3a0a 2020 2020 2020 2020 2020  < 10:.          
-0000b5e0: 2020 7374 7265 616d 2e72 656d 6f76 6528    stream.remove(
-0000b5f0: 7472 290a 0a20 2020 2072 6574 7572 6e20  tr)..    return 
-0000b600: 7374 7265 616d 0a0a 0a64 6566 2070 6f72  stream...def por
-0000b610: 7469 6f6e 5f67 6170 7328 7374 7265 616d  tion_gaps(stream
-0000b620: 2c20 7374 6172 7474 696d 653a 206f 6273  , starttime: obs
-0000b630: 7079 2e55 5443 4461 7465 5469 6d65 2c20  py.UTCDateTime, 
-0000b640: 656e 6474 696d 653a 206f 6273 7079 2e55  endtime: obspy.U
-0000b650: 5443 4461 7465 5469 6d65 293a 0a20 2020  TCDateTime):.   
-0000b660: 2022 2222 0a20 2020 2074 6869 7320 6675   """.    this fu
-0000b670: 6e63 7469 6f6e 2074 7261 636b 7320 7468  nction tracks th
-0000b680: 6520 6761 7073 2028 6e70 7473 2920 6672  e gaps (npts) fr
-0000b690: 6f6d 2074 6865 2061 6363 756d 756c 6174  om the accumulat
-0000b6a0: 6564 2064 6966 6665 7265 6e63 6520 6265  ed difference be
-0000b6b0: 7477 6565 6e20 7374 6172 7474 696d 6520  tween starttime 
-0000b6c0: 616e 6420 656e 6474 696d 650a 2020 2020  and endtime.    
-0000b6d0: 6f66 2065 6163 6820 7374 7265 616d 2074  of each stream t
-0000b6e0: 7261 6365 2e20 6974 2072 656d 6f76 6573  race. it removes
-0000b6f0: 2074 7261 6365 2077 6974 6820 6761 7020   trace with gap 
-0000b700: 6c65 6e67 7468 203e 2033 3025 206f 6620  length > 30% of 
-0000b710: 7472 6163 6520 7369 7a65 2e0a 2020 2020  trace size..    
-0000b720: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
-0000b730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b740: 2d2d 2d0a 2020 2020 7374 7265 616d 3a20  ---.    stream: 
-0000b750: 6f62 7370 7920 7374 7265 616d 206f 626a  obspy stream obj
-0000b760: 6563 740a 2020 2020 6461 7465 5f69 6e66  ect.    date_inf
-0000b770: 6f3a 2064 6963 7420 6f66 2073 7461 7274  o: dict of start
-0000b780: 696e 6720 616e 6420 656e 6469 6e67 2074  ing and ending t
-0000b790: 696d 6520 6f66 2074 6865 2073 7472 6561  ime of the strea
-0000b7a0: 6d0a 0a20 2020 2052 4554 5552 4e53 3a0a  m..    RETURNS:.
-0000b7b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000b7c0: 2d2d 2d2d 2d0a 2020 2020 7067 6170 733a  -----.    pgaps:
-0000b7d0: 2070 726f 706f 7274 696f 6e20 6f66 2067   proportion of g
-0000b7e0: 6170 732f 616c 6c5f 7074 7320 696e 2073  aps/all_pts in s
-0000b7f0: 7472 6561 6d0a 2020 2020 2222 220a 2020  tream.    """.  
-0000b800: 2020 2320 6964 6561 6c20 6475 7261 7469    # ideal durati
-0000b810: 6f6e 206f 6620 6461 7461 0a20 2020 206e  on of data.    n
-0000b820: 7074 7320 3d20 2865 6e64 7469 6d65 202d  pts = (endtime -
-0000b830: 2073 7461 7274 7469 6d65 2920 2a20 7374   starttime) * st
-0000b840: 7265 616d 5b30 5d2e 7374 6174 732e 7361  ream[0].stats.sa
-0000b850: 6d70 6c69 6e67 5f72 6174 650a 0a20 2020  mpling_rate..   
-0000b860: 2070 6761 7073 203d 2030 0a20 2020 2023   pgaps = 0.    #
-0000b870: 206c 6f6f 7020 7468 726f 7567 6820 616c   loop through al
-0000b880: 6c20 7472 6163 6520 746f 2061 6363 756d  l trace to accum
-0000b890: 756c 6174 6520 6761 7073 0a20 2020 2066  ulate gaps.    f
-0000b8a0: 6f72 2069 6920 696e 2072 616e 6765 286c  or ii in range(l
-0000b8b0: 656e 2873 7472 6561 6d29 202d 2031 293a  en(stream) - 1):
-0000b8c0: 0a20 2020 2020 2020 2070 6761 7073 202b  .        pgaps +
-0000b8d0: 3d20 2873 7472 6561 6d5b 6969 202b 2031  = (stream[ii + 1
-0000b8e0: 5d2e 7374 6174 732e 7374 6172 7474 696d  ].stats.starttim
-0000b8f0: 6520 2d20 7374 7265 616d 5b69 695d 2e73  e - stream[ii].s
-0000b900: 7461 7473 2e65 6e64 7469 6d65 2920 2a20  tats.endtime) * 
-0000b910: 7374 7265 616d 5b69 695d 2e73 7461 7473  stream[ii].stats
-0000b920: 2e73 616d 706c 696e 675f 7261 7465 0a20  .sampling_rate. 
-0000b930: 2020 2069 6620 6e70 7473 2021 3d20 303a     if npts != 0:
-0000b940: 0a20 2020 2020 2020 2070 6761 7073 203d  .        pgaps =
-0000b950: 2070 6761 7073 202f 206e 7074 730a 2020   pgaps / npts.  
-0000b960: 2020 6966 206e 7074 7320 3d3d 2030 3a0a    if npts == 0:.
-0000b970: 2020 2020 2020 2020 7067 6170 7320 3d20          pgaps = 
-0000b980: 310a 2020 2020 7265 7475 726e 2070 6761  1.    return pga
-0000b990: 7073 0a0a 0a40 6a69 7428 2266 6c6f 6174  ps...@jit("float
-0000b9a0: 3332 5b3a 5d28 666c 6f61 7433 325b 3a5d  32[:](float32[:]
-0000b9b0: 2c66 6c6f 6174 3332 2922 290a 6465 6620  ,float32)").def 
-0000b9c0: 7365 676d 656e 745f 696e 7465 7270 6f6c  segment_interpol
-0000b9d0: 6174 6528 7369 6731 2c20 6e66 7269 6329  ate(sig1, nfric)
-0000b9e0: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-0000b9f0: 6973 2066 756e 6374 696f 6e20 696e 7465  is function inte
-0000ba00: 7270 6f6c 6174 6573 2074 6865 2064 6174  rpolates the dat
-0000ba10: 6120 746f 2065 6e73 7572 6520 616c 6c20  a to ensure all 
-0000ba20: 706f 696e 7473 206c 6f63 6174 6564 206f  points located o
-0000ba30: 6e20 696e 7465 7267 6572 2074 696d 6573  n interger times
-0000ba40: 206f 6620 7468 650a 2020 2020 7361 6d70   of the.    samp
-0000ba50: 6c69 6e67 2072 6174 6520 2865 2e67 2e2c  ling rate (e.g.,
-0000ba60: 2073 7461 7274 7469 6d65 203d 2030 303a   starttime = 00:
-0000ba70: 3030 3a30 302e 3031 352c 2064 656c 7461  00:00.015, delta
-0000ba80: 203d 2030 2e30 352e 290a 2020 2020 5041   = 0.05.).    PA
-0000ba90: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
-0000baa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bab0: 2d2d 2d2d 0a20 2020 2073 6967 313a 2020  ----.    sig1:  
-0000bac0: 7365 6973 6d69 6320 7265 636f 7264 696e  seismic recordin
-0000bad0: 6773 2069 6e20 6120 3144 2061 7272 6179  gs in a 1D array
-0000bae0: 0a20 2020 206e 6672 6963 3a20 7468 6520  .    nfric: the 
-0000baf0: 616d 6f75 6e74 206f 6620 7469 6d65 2064  amount of time d
-0000bb00: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
-0000bb10: 6e20 7468 6520 706f 696e 7420 616e 6420  n the point and 
-0000bb20: 7468 6520 6164 6a61 6365 6e74 2061 7373  the adjacent ass
-0000bb30: 756d 6564 2073 616d 706c 6573 0a20 2020  umed samples.   
-0000bb40: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-0000bb50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bb60: 2d2d 2d2d 0a20 2020 2073 6967 323a 2020  ----.    sig2:  
-0000bb70: 696e 7465 7270 6f6c 6174 6564 2073 6569  interpolated sei
-0000bb80: 736d 6963 2072 6563 6f72 6469 6e67 7320  smic recordings 
-0000bb90: 6f6e 2074 6865 2073 616d 706c 696e 6720  on the sampling 
-0000bba0: 706f 696e 7473 0a20 2020 2022 2222 0a20  points.    """. 
-0000bbb0: 2020 206e 7074 7320 3d20 6c65 6e28 7369     npts = len(si
-0000bbc0: 6731 290a 2020 2020 7369 6732 203d 206e  g1).    sig2 = n
-0000bbd0: 702e 7a65 726f 7328 6e70 7473 2c20 6474  p.zeros(npts, dt
-0000bbe0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-0000bbf0: 0a20 2020 2023 202d 2d2d 2d69 6e73 7465  .    # ----inste
-0000bc00: 6164 206f 6620 7368 6966 7469 6e67 2c20  ad of shifting, 
-0000bc10: 646f 2061 2069 6e74 6572 706f 6c61 7469  do a interpolati
-0000bc20: 6f6e 2d2d 2d2d 2d2d 0a20 2020 2066 6f72  on------.    for
-0000bc30: 2069 6920 696e 2072 616e 6765 286e 7074   ii in range(npt
-0000bc40: 7329 3a0a 2020 2020 2020 2020 2320 2d2d  s):.        # --
-0000bc50: 2d2d 6465 616c 2077 6974 6820 6564 6765  --deal with edge
-0000bc60: 732d 2d2d 2d2d 0a20 2020 2020 2020 2069  s-----.        i
-0000bc70: 6620 6969 203d 3d20 3020 6f72 2069 6920  f ii == 0 or ii 
-0000bc80: 3d3d 206e 7074 7320 2d20 313a 0a20 2020  == npts - 1:.   
-0000bc90: 2020 2020 2020 2020 2073 6967 325b 6969           sig2[ii
-0000bca0: 5d20 3d20 7369 6731 5b69 695d 0a20 2020  ] = sig1[ii].   
-0000bcb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000bcc0: 2020 2020 2020 2023 202d 2d2d 2d2d 2d69         # ------i
-0000bcd0: 6e74 6572 706f 6c61 7465 2075 7369 6e67  nterpolate using
-0000bce0: 2061 2068 6174 2066 756e 6374 696f 6e2d   a hat function-
-0000bcf0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2020  -----.          
-0000bd00: 2020 7369 6732 5b69 695d 203d 2028 3120    sig2[ii] = (1 
-0000bd10: 2d20 6e66 7269 6329 202a 2073 6967 315b  - nfric) * sig1[
-0000bd20: 6969 202b 2031 5d20 2b20 6e66 7269 6320  ii + 1] + nfric 
-0000bd30: 2a20 7369 6731 5b69 695d 0a0a 2020 2020  * sig1[ii]..    
-0000bd40: 7265 7475 726e 2073 6967 320a 0a0a 6465  return sig2...de
-0000bd50: 6620 7265 7370 5f73 7065 6374 7275 6d28  f resp_spectrum(
-0000bd60: 736f 7572 6365 2c20 7265 7370 5f66 696c  source, resp_fil
-0000bd70: 652c 2064 6f77 6e73 616d 705f 6672 6571  e, downsamp_freq
-0000bd80: 2c20 7072 655f 6669 6c74 3d4e 6f6e 6529  , pre_filt=None)
-0000bd90: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-0000bda0: 6973 2066 756e 6374 696f 6e20 7265 6d6f  is function remo
-0000bdb0: 7665 7320 7468 6520 696e 7374 7275 6d65  ves the instrume
-0000bdc0: 6e74 2072 6573 706f 6e73 6520 7573 696e  nt response usin
-0000bdd0: 6720 7265 7370 6f6e 7365 2073 7065 6374  g response spect
-0000bde0: 7275 6d20 6672 6f6d 2065 7661 6c72 6573  rum from evalres
-0000bdf0: 702e 0a20 2020 2074 6865 2072 6573 706f  p..    the respo
-0000be00: 6e73 6520 7370 6563 7472 756d 2069 7320  nse spectrum is 
-0000be10: 6576 616c 7561 7465 6420 6261 7365 6420  evaluated based 
-0000be20: 6f6e 2052 4553 502f 505a 2066 696c 6573  on RESP/PZ files
-0000be30: 2062 6566 6f72 6520 696e 7665 7274 6564   before inverted
-0000be40: 2075 7369 6e67 2074 6865 206f 6273 7079   using the obspy
-0000be50: 0a20 2020 2066 756e 6374 696f 6e20 6f66  .    function of
-0000be60: 2069 6e76 6572 745f 7370 6563 7472 756d   invert_spectrum
-0000be70: 2e20 6120 6d6f 6475 6c65 206f 6620 6372  . a module of cr
-0000be80: 6561 7465 5f72 6573 702e 7079 2069 7320  eate_resp.py is 
-0000be90: 7072 6f76 6964 6564 2069 6e20 6469 7265  provided in dire
-0000bea0: 6374 6f72 7920 6f66 2027 6164 6469 7469  ctory of 'additi
-0000beb0: 6f6e 616c 5f6d 6f64 756c 6573 270a 2020  onal_modules'.  
-0000bec0: 2020 746f 2063 7265 6174 6520 7468 6520    to create the 
-0000bed0: 7265 7370 6f6e 7365 2073 7065 6374 7275  response spectru
-0000bee0: 6d0a 2020 2020 5041 5241 4d45 5445 5253  m.    PARAMETERS
-0000bef0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-0000bf00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0000bf10: 2073 6f75 7263 653a 206f 6273 7079 2073   source: obspy s
-0000bf20: 7472 6561 6d20 6f62 6a65 6374 206f 6620  tream object of 
-0000bf30: 7461 7267 6574 6564 206e 6f69 7365 2064  targeted noise d
-0000bf40: 6174 610a 2020 2020 7265 7370 5f66 696c  ata.    resp_fil
-0000bf50: 653a 206e 756d 7079 2064 6174 6120 6669  e: numpy data fi
-0000bf60: 6c65 206f 6620 7265 7370 6f6e 7365 2073  le of response s
-0000bf70: 7065 6374 7275 6d0a 2020 2020 646f 776e  pectrum.    down
-0000bf80: 7361 6d70 5f66 7265 713a 2073 616d 706c  samp_freq: sampl
-0000bf90: 696e 6720 7261 7465 206f 6620 7468 6520  ing rate of the 
-0000bfa0: 736f 7572 6365 2064 6174 610a 2020 2020  source data.    
-0000bfb0: 7072 655f 6669 6c74 3a20 7072 652d 6465  pre_filt: pre-de
-0000bfc0: 6669 6e65 6420 6669 6c74 6572 2070 6172  fined filter par
-0000bfd0: 616d 6574 6572 730a 2020 2020 5245 5455  ameters.    RETU
-0000bfe0: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
-0000bff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000c000: 2020 2020 736f 7572 6365 3a20 6f62 7370      source: obsp
-0000c010: 7920 7374 7265 616d 206f 626a 6563 7420  y stream object 
-0000c020: 6f66 206e 6f69 7365 2064 6174 6120 7769  of noise data wi
-0000c030: 7468 2069 6e73 7472 756d 656e 7420 7265  th instrument re
-0000c040: 7370 6f6e 7365 2072 656d 6f76 6564 0a20  sponse removed. 
-0000c050: 2020 2022 2222 0a20 2020 2023 202d 2d2d     """.    # ---
-0000c060: 2d2d 2d2d 2d72 6573 705f 6669 6c65 2069  -----resp_file i
-0000c070: 7320 7468 6520 696e 7665 7274 6564 2073  s the inverted s
-0000c080: 7065 6374 7275 6d20 7265 7370 6f6e 7365  pectrum response
-0000c090: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7265  ---------.    re
-0000c0a0: 7370 7a20 3d20 6e70 2e6c 6f61 6428 7265  spz = np.load(re
-0000c0b0: 7370 5f66 696c 6529 0a20 2020 206e 7265  sp_file).    nre
-0000c0c0: 7370 7a20 3d20 7265 7370 7a5b 315d 5b3a  spz = respz[1][:
-0000c0d0: 5d0a 2020 2020 7370 6563 5f66 7265 7120  ].    spec_freq 
-0000c0e0: 3d20 6d61 7828 7265 7370 7a5b 305d 290a  = max(respz[0]).
-0000c0f0: 0a20 2020 2023 202d 2d2d 2d2d 2d2d 6f6e  .    # -------on
-0000c100: 2063 7572 7265 6e74 2074 7261 6365 2d2d   current trace--
-0000c110: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 6666  --------.    nff
-0000c120: 7420 3d20 5f6e 7074 7332 6e66 6674 2873  t = _npts2nfft(s
-0000c130: 6f75 7263 655b 305d 2e73 7461 7473 2e6e  ource[0].stats.n
-0000c140: 7074 7329 0a20 2020 2073 7073 203d 2069  pts).    sps = i
-0000c150: 6e74 2873 6f75 7263 655b 305d 2e73 7461  nt(source[0].sta
-0000c160: 7473 2e73 616d 706c 696e 675f 7261 7465  ts.sampling_rate
-0000c170: 290a 0a20 2020 2023 202d 2d2d 2d2d 2d2d  )..    # -------
-0000c180: 2d2d 646f 2074 6865 2069 6e74 6572 706f  --do the interpo
-0000c190: 6c61 7469 6f6e 2069 6620 6e65 6564 6564  lation if needed
-0000c1a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6620  --------.    if 
-0000c1b0: 7370 6563 5f66 7265 7120 3c20 302e 3520  spec_freq < 0.5 
-0000c1c0: 2a20 7370 733a 0a20 2020 2020 2020 2072  * sps:.        r
-0000c1d0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000c1e0: 2273 7065 6374 7275 6d20 6669 6c65 2068  "spectrum file h
-0000c1f0: 6173 2070 6561 6b20 6672 6571 2073 6d61  as peak freq sma
-0000c200: 6c6c 6572 2074 6861 6e20 7468 6520 6461  ller than the da
-0000c210: 7461 2c20 6162 6f72 7421 2229 0a20 2020  ta, abort!").   
-0000c220: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
-0000c230: 6e64 7820 3d20 6e70 2e77 6865 7265 2872  ndx = np.where(r
-0000c240: 6573 707a 5b30 5d20 3c3d 2030 2e35 202a  espz[0] <= 0.5 *
-0000c250: 2073 7073 290a 2020 2020 2020 2020 6e66   sps).        nf
-0000c260: 7265 7120 3d20 6e70 2e6c 696e 7370 6163  req = np.linspac
-0000c270: 6528 302c 2030 2e35 202a 2073 7073 2c20  e(0, 0.5 * sps, 
-0000c280: 6e66 6674 202f 2f20 3220 2b20 3129 0a20  nfft // 2 + 1). 
-0000c290: 2020 2020 2020 206e 7265 7370 7a20 3d20         nrespz = 
-0000c2a0: 6e70 2e69 6e74 6572 7028 6e66 7265 712c  np.interp(nfreq,
-0000c2b0: 206e 702e 7265 616c 2872 6573 707a 5b30   np.real(respz[0
-0000c2c0: 5d5b 696e 6478 5d29 2c20 7265 7370 7a5b  ][indx]), respz[
-0000c2d0: 315d 5b69 6e64 785d 290a 0a20 2020 2023  1][indx])..    #
-0000c2e0: 202d 2d2d 2d64 6f20 696e 7465 7270 6f6c   ----do interpol
-0000c2f0: 6174 696f 6e20 6966 206e 6563 6573 7361  ation if necessa
-0000c300: 7279 2d2d 2d2d 2d0a 2020 2020 736f 7572  ry-----.    sour
-0000c310: 6365 5f73 7065 6374 203d 206e 702e 6666  ce_spect = np.ff
-0000c320: 742e 7266 6674 2873 6f75 7263 655b 305d  t.rfft(source[0]
-0000c330: 2e64 6174 612c 206e 3d6e 6666 7429 0a0a  .data, n=nfft)..
-0000c340: 2020 2020 2320 2d2d 2d2d 2d6e 7265 7370      # -----nresp
-0000c350: 7a20 6973 2069 6e76 6572 7365 6420 2877  z is inversed (w
-0000c360: 6174 6572 2d6c 6576 656c 6564 2920 7370  ater-leveled) sp
-0000c370: 6563 7472 756d 2d2d 2d2d 2d0a 2020 2020  ectrum-----.    
-0000c380: 736f 7572 6365 5f73 7065 6374 202a 3d20  source_spect *= 
-0000c390: 6e72 6573 707a 0a20 2020 2073 6f75 7263  nrespz.    sourc
-0000c3a0: 655b 305d 2e64 6174 6120 3d20 6e70 2e66  e[0].data = np.f
-0000c3b0: 6674 2e69 7266 6674 2873 6f75 7263 655f  ft.irfft(source_
-0000c3c0: 7370 6563 7429 5b30 203a 2073 6f75 7263  spect)[0 : sourc
-0000c3d0: 655b 305d 2e73 7461 7473 2e6e 7074 735d  e[0].stats.npts]
-0000c3e0: 0a0a 2020 2020 6966 2070 7265 5f66 696c  ..    if pre_fil
-0000c3f0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-0000c400: 2020 2020 2020 2073 6f75 7263 655b 305d         source[0]
-0000c410: 2e64 6174 6120 3d20 6e70 2e66 6c6f 6174  .data = np.float
-0000c420: 3332 280a 2020 2020 2020 2020 2020 2020  32(.            
-0000c430: 6261 6e64 7061 7373 280a 2020 2020 2020  bandpass(.      
-0000c440: 2020 2020 2020 2020 2020 736f 7572 6365            source
-0000c450: 5b30 5d2e 6461 7461 2c0a 2020 2020 2020  [0].data,.      
-0000c460: 2020 2020 2020 2020 2020 7072 655f 6669            pre_fi
-0000c470: 6c74 5b30 5d2c 0a20 2020 2020 2020 2020  lt[0],.         
-0000c480: 2020 2020 2020 2070 7265 5f66 696c 745b         pre_filt[
-0000c490: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
-0000c4a0: 2020 2020 2064 663d 7370 732c 0a20 2020       df=sps,.   
-0000c4b0: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
-0000c4c0: 6e65 7273 3d34 2c0a 2020 2020 2020 2020  ners=4,.        
-0000c4d0: 2020 2020 2020 2020 7a65 726f 7068 6173          zerophas
-0000c4e0: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
-0000c4f0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
-0000c500: 0a20 2020 2072 6574 7572 6e20 736f 7572  .    return sour
-0000c510: 6365 0a0a 0a64 6566 206d 6164 2861 7272  ce...def mad(arr
-0000c520: 293a 0a20 2020 2022 2222 0a20 2020 204d  ):.    """.    M
-0000c530: 6564 6961 6e20 4162 736f 6c75 7465 2044  edian Absolute D
-0000c540: 6576 6961 7469 6f6e 3a20 4d41 4420 3d20  eviation: MAD = 
-0000c550: 6d65 6469 616e 287c 5869 2d20 6d65 6469  median(|Xi- medi
-0000c560: 616e 2858 297c 290a 2020 2020 5041 5241  an(X)|).    PARA
-0000c570: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-0000c580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000c590: 2020 2020 6172 723a 206e 756d 7079 2e6e      arr: numpy.n
-0000c5a0: 6461 7272 6179 2c20 7365 6973 6d69 6320  darray, seismic 
-0000c5b0: 7472 6163 6520 6461 7461 2061 7272 6179  trace data array
-0000c5c0: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-0000c5d0: 2020 6461 7461 3a20 4d65 6469 616e 2041    data: Median A
-0000c5e0: 6273 6f6c 7574 6520 4465 7669 6174 696f  bsolute Deviatio
-0000c5f0: 6e20 6f66 2064 6174 610a 2020 2020 2222  n of data.    ""
-0000c600: 220a 2020 2020 6966 206e 6f74 206e 702e  ".    if not np.
-0000c610: 6d61 2e69 735f 6d61 736b 6564 2861 7272  ma.is_masked(arr
-0000c620: 293a 0a20 2020 2020 2020 206d 6564 203d  ):.        med =
-0000c630: 206e 702e 6d65 6469 616e 2861 7272 290a   np.median(arr).
-0000c640: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
-0000c650: 702e 6d65 6469 616e 286e 702e 6162 7328  p.median(np.abs(
-0000c660: 6172 7220 2d20 6d65 6429 290a 2020 2020  arr - med)).    
-0000c670: 656c 7365 3a0a 2020 2020 2020 2020 6d65  else:.        me
-0000c680: 6420 3d20 6e70 2e6d 612e 6d65 6469 616e  d = np.ma.median
-0000c690: 2861 7272 290a 2020 2020 2020 2020 6461  (arr).        da
-0000c6a0: 7461 203d 206e 702e 6d61 2e6d 6564 6961  ta = np.ma.media
-0000c6b0: 6e28 6e70 2e6d 612e 6162 7328 6172 7220  n(np.ma.abs(arr 
-0000c6c0: 2d20 6d65 6429 290a 2020 2020 7265 7475  - med)).    retu
-0000c6d0: 726e 2064 6174 610a 0a0a 6465 6620 6465  rn data...def de
-0000c6e0: 7472 656e 6428 6461 7461 293a 0a20 2020  trend(data):.   
-0000c6f0: 2022 2222 0a20 2020 2074 6869 7320 6675   """.    this fu
-0000c700: 6e63 7469 6f6e 2072 656d 6f76 6573 2074  nction removes t
-0000c710: 6865 2073 6967 6e61 6c20 7472 656e 6420  he signal trend 
-0000c720: 6261 7365 6420 6f6e 2051 5220 6465 636f  based on QR deco
-0000c730: 6d70 6f73 696f 6e0a 2020 2020 4e4f 5445  mposion.    NOTE
-0000c740: 3a20 5152 2069 7320 6120 6c6f 7420 6661  : QR is a lot fa
-0000c750: 7374 6572 2074 6861 6e20 7468 6520 6c65  ster than the le
-0000c760: 6173 7420 7371 7561 7265 2069 6e76 6572  ast square inver
-0000c770: 7369 6f6e 2075 7365 6420 6279 0a20 2020  sion used by.   
-0000c780: 2073 6369 7079 2028 616c 736f 2069 6e20   scipy (also in 
-0000c790: 6f62 7370 7929 2e0a 2020 2020 5041 5241  obspy)..    PARA
-0000c7a0: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-0000c7b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c7c0: 2d0a 2020 2020 6461 7461 3a20 696e 7075  -.    data: inpu
-0000c7d0: 7420 6461 7461 206d 6174 7269 780a 2020  t data matrix.  
-0000c7e0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
-0000c7f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c800: 2d2d 2d2d 0a20 2020 2064 6174 613a 2064  ----.    data: d
-0000c810: 6174 6120 6d61 7472 6978 2077 6974 6820  ata matrix with 
-0000c820: 7472 656e 6420 7265 6d6f 7665 640a 2020  trend removed.  
-0000c830: 2020 2222 220a 2020 2020 2320 6e64 6174    """.    # ndat
-0000c840: 6120 3d20 6e70 2e7a 6572 6f73 2873 6861  a = np.zeros(sha
-0000c850: 7065 3d64 6174 612e 7368 6170 652c 6474  pe=data.shape,dt
-0000c860: 7970 653d 6461 7461 2e64 7479 7065 290a  ype=data.dtype).
-0000c870: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
-0000c880: 203d 3d20 313a 0a20 2020 2020 2020 206e   == 1:.        n
-0000c890: 7074 7320 3d20 6461 7461 2e73 6861 7065  pts = data.shape
-0000c8a0: 5b30 5d0a 2020 2020 2020 2020 5820 3d20  [0].        X = 
-0000c8b0: 6e70 2e6f 6e65 7328 286e 7074 732c 2032  np.ones((npts, 2
-0000c8c0: 2929 0a20 2020 2020 2020 2058 5b3a 2c20  )).        X[:, 
-0000c8d0: 305d 203d 206e 702e 6172 616e 6765 2830  0] = np.arange(0
-0000c8e0: 2c20 6e70 7473 2920 2f20 6e70 7473 0a20  , npts) / npts. 
-0000c8f0: 2020 2020 2020 2051 2c20 5220 3d20 6e70         Q, R = np
-0000c900: 2e6c 696e 616c 672e 7172 2858 290a 2020  .linalg.qr(X).  
-0000c910: 2020 2020 2020 7271 203d 206e 702e 646f        rq = np.do
-0000c920: 7428 6e70 2e6c 696e 616c 672e 696e 7628  t(np.linalg.inv(
-0000c930: 5229 2c20 512e 7472 616e 7370 6f73 6528  R), Q.transpose(
-0000c940: 2929 0a20 2020 2020 2020 2063 6f65 6666  )).        coeff
-0000c950: 203d 206e 702e 646f 7428 7271 2c20 6461   = np.dot(rq, da
-0000c960: 7461 290a 2020 2020 2020 2020 6461 7461  ta).        data
-0000c970: 203d 2064 6174 6120 2d20 6e70 2e64 6f74   = data - np.dot
-0000c980: 2858 2c20 636f 6566 6629 0a20 2020 2065  (X, coeff).    e
-0000c990: 6c69 6620 6461 7461 2e6e 6469 6d20 3d3d  lif data.ndim ==
-0000c9a0: 2032 3a0a 2020 2020 2020 2020 6e70 7473   2:.        npts
-0000c9b0: 203d 2064 6174 612e 7368 6170 655b 315d   = data.shape[1]
-0000c9c0: 0a20 2020 2020 2020 2058 203d 206e 702e  .        X = np.
-0000c9d0: 6f6e 6573 2828 6e70 7473 2c20 3229 290a  ones((npts, 2)).
-0000c9e0: 2020 2020 2020 2020 585b 3a2c 2030 5d20          X[:, 0] 
-0000c9f0: 3d20 6e70 2e61 7261 6e67 6528 302c 206e  = np.arange(0, n
-0000ca00: 7074 7329 202f 206e 7074 730a 2020 2020  pts) / npts.    
-0000ca10: 2020 2020 512c 2052 203d 206e 702e 6c69      Q, R = np.li
-0000ca20: 6e61 6c67 2e71 7228 5829 0a20 2020 2020  nalg.qr(X).     
-0000ca30: 2020 2072 7120 3d20 6e70 2e64 6f74 286e     rq = np.dot(n
-0000ca40: 702e 6c69 6e61 6c67 2e69 6e76 2852 292c  p.linalg.inv(R),
-0000ca50: 2051 2e74 7261 6e73 706f 7365 2829 290a   Q.transpose()).
-0000ca60: 2020 2020 2020 2020 666f 7220 6969 2069          for ii i
-0000ca70: 6e20 7261 6e67 6528 6461 7461 2e73 6861  n range(data.sha
-0000ca80: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
-0000ca90: 2020 2020 636f 6566 6620 3d20 6e70 2e64      coeff = np.d
-0000caa0: 6f74 2872 712c 2064 6174 615b 6969 5d29  ot(rq, data[ii])
-0000cab0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000cac0: 615b 6969 5d20 3d20 6461 7461 5b69 695d  a[ii] = data[ii]
-0000cad0: 202d 206e 702e 646f 7428 582c 2063 6f65   - np.dot(X, coe
-0000cae0: 6666 290a 2020 2020 7265 7475 726e 2064  ff).    return d
-0000caf0: 6174 610a 0a0a 6465 6620 6465 6d65 616e  ata...def demean
-0000cb00: 2864 6174 6129 3a0a 2020 2020 2222 220a  (data):.    """.
-0000cb10: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-0000cb20: 6e20 7265 6d6f 7665 2074 6865 206d 6561  n remove the mea
-0000cb30: 6e20 6f66 2074 6865 2073 6967 6e61 6c0a  n of the signal.
-0000cb40: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-0000cb50: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000cb60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6461  ---------.    da
-0000cb70: 7461 3a20 696e 7075 7420 6461 7461 206d  ta: input data m
-0000cb80: 6174 7269 780a 2020 2020 5245 5455 524e  atrix.    RETURN
-0000cb90: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-0000cba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0000cbb0: 2064 6174 613a 2064 6174 6120 6d61 7472   data: data matr
-0000cbc0: 6978 2077 6974 6820 6d65 616e 2072 656d  ix with mean rem
-0000cbd0: 6f76 6564 0a20 2020 2022 2222 0a20 2020  oved.    """.   
-0000cbe0: 2023 206e 6461 7461 203d 206e 702e 7a65   # ndata = np.ze
-0000cbf0: 726f 7328 7368 6170 653d 6461 7461 2e73  ros(shape=data.s
-0000cc00: 6861 7065 2c64 7479 7065 3d64 6174 612e  hape,dtype=data.
-0000cc10: 6474 7970 6529 0a20 2020 2069 6620 6461  dtype).    if da
-0000cc20: 7461 2e6e 6469 6d20 3d3d 2031 3a0a 2020  ta.ndim == 1:.  
-0000cc30: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0000cc40: 6120 2d20 6e70 2e6d 6561 6e28 6461 7461  a - np.mean(data
-0000cc50: 290a 2020 2020 656c 6966 2064 6174 612e  ).    elif data.
-0000cc60: 6e64 696d 203d 3d20 323a 0a20 2020 2020  ndim == 2:.     
-0000cc70: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
-0000cc80: 6765 2864 6174 612e 7368 6170 655b 305d  ge(data.shape[0]
-0000cc90: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-0000cca0: 6174 615b 6969 5d20 3d20 6461 7461 5b69  ata[ii] = data[i
-0000ccb0: 695d 202d 206e 702e 6d65 616e 2864 6174  i] - np.mean(dat
-0000ccc0: 615b 6969 5d29 0a20 2020 2072 6574 7572  a[ii]).    retur
-0000ccd0: 6e20 6461 7461 0a0a 0a64 6566 2074 6170  n data...def tap
-0000cce0: 6572 2864 6174 6129 3a0a 2020 2020 2222  er(data):.    ""
-0000ccf0: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
-0000cd00: 696f 6e20 6170 706c 6965 7320 6120 636f  ion applies a co
-0000cd10: 7369 6e65 2074 6170 6572 2075 7369 6e67  sine taper using
-0000cd20: 206f 6273 7079 2066 756e 6374 696f 6e73   obspy functions
-0000cd30: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-0000cd40: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000cd50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
-0000cd60: 6174 613a 2069 6e70 7574 2064 6174 6120  ata: input data 
-0000cd70: 6d61 7472 6978 0a20 2020 2052 4554 5552  matrix.    RETUR
-0000cd80: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-0000cd90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000cda0: 2020 6461 7461 3a20 6461 7461 206d 6174    data: data mat
-0000cdb0: 7269 7820 7769 7468 2074 6170 6572 2061  rix with taper a
-0000cdc0: 7070 6c69 6564 0a20 2020 2022 2222 0a20  pplied.    """. 
-0000cdd0: 2020 2023 206e 6461 7461 203d 206e 702e     # ndata = np.
-0000cde0: 7a65 726f 7328 7368 6170 653d 6461 7461  zeros(shape=data
-0000cdf0: 2e73 6861 7065 2c64 7479 7065 3d64 6174  .shape,dtype=dat
-0000ce00: 612e 6474 7970 6529 0a20 2020 2069 6620  a.dtype).    if 
-0000ce10: 6461 7461 2e6e 6469 6d20 3d3d 2031 3a0a  data.ndim == 1:.
-0000ce20: 2020 2020 2020 2020 6e70 7473 203d 2064          npts = d
-0000ce30: 6174 612e 7368 6170 655b 305d 0a20 2020  ata.shape[0].   
-0000ce40: 2020 2020 2023 2077 696e 646f 7720 6c65       # window le
-0000ce50: 6e67 7468 0a20 2020 2020 2020 2069 6620  ngth.        if 
-0000ce60: 6e70 7473 202a 2030 2e30 3520 3e20 3230  npts * 0.05 > 20
-0000ce70: 3a0a 2020 2020 2020 2020 2020 2020 776c  :.            wl
-0000ce80: 656e 203d 2032 300a 2020 2020 2020 2020  en = 20.        
-0000ce90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000cea0: 2020 776c 656e 203d 206e 7074 7320 2a20    wlen = npts * 
-0000ceb0: 302e 3035 0a20 2020 2020 2020 2023 2074  0.05.        # t
-0000cec0: 6170 6572 2076 616c 7565 730a 2020 2020  aper values.    
-0000ced0: 2020 2020 6675 6e63 203d 205f 6765 745f      func = _get_
-0000cee0: 6675 6e63 7469 6f6e 5f66 726f 6d5f 656e  function_from_en
-0000cef0: 7472 795f 706f 696e 7428 2274 6170 6572  try_point("taper
-0000cf00: 222c 2022 6861 6e6e 2229 0a20 2020 2020  ", "hann").     
-0000cf10: 2020 2069 6620 3220 2a20 776c 656e 203d     if 2 * wlen =
-0000cf20: 3d20 6e70 7473 3a0a 2020 2020 2020 2020  = npts:.        
-0000cf30: 2020 2020 7461 7065 725f 7369 6465 7320      taper_sides 
-0000cf40: 3d20 6675 6e63 2832 202a 2077 6c65 6e29  = func(2 * wlen)
-0000cf50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000cf60: 2020 2020 2020 2020 2020 2074 6170 6572             taper
-0000cf70: 5f73 6964 6573 203d 2066 756e 6328 3220  _sides = func(2 
-0000cf80: 2a20 776c 656e 202b 2031 290a 2020 2020  * wlen + 1).    
-0000cf90: 2020 2020 2320 7461 7065 7220 7769 6e64      # taper wind
-0000cfa0: 6f77 0a20 2020 2020 2020 2077 696e 203d  ow.        win =
-0000cfb0: 206e 702e 6873 7461 636b 280a 2020 2020   np.hstack(.    
-0000cfc0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-0000cfd0: 2020 2020 2020 2020 2020 7461 7065 725f            taper_
-0000cfe0: 7369 6465 735b 3a77 6c65 6e5d 2c0a 2020  sides[:wlen],.  
-0000cff0: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-0000d000: 2e6f 6e65 7328 6e70 7473 202d 2032 202a  .ones(npts - 2 *
-0000d010: 2077 6c65 6e29 2c0a 2020 2020 2020 2020   wlen),.        
-0000d020: 2020 2020 2020 2020 7461 7065 725f 7369          taper_si
-0000d030: 6465 735b 6c65 6e28 7461 7065 725f 7369  des[len(taper_si
-0000d040: 6465 7329 202d 2077 6c65 6e20 3a5d 2c0a  des) - wlen :],.
-0000d050: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000d060: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000d070: 6461 7461 202a 3d20 7769 6e0a 2020 2020  data *= win.    
-0000d080: 656c 6966 2064 6174 612e 6e64 696d 203d  elif data.ndim =
-0000d090: 3d20 323a 0a20 2020 2020 2020 206e 7074  = 2:.        npt
-0000d0a0: 7320 3d20 6461 7461 2e73 6861 7065 5b31  s = data.shape[1
-0000d0b0: 5d0a 2020 2020 2020 2020 2320 7769 6e64  ].        # wind
-0000d0c0: 6f77 206c 656e 6774 680a 2020 2020 2020  ow length.      
-0000d0d0: 2020 6966 206e 7074 7320 2a20 302e 3035    if npts * 0.05
-0000d0e0: 203e 2032 303a 0a20 2020 2020 2020 2020   > 20:.         
-0000d0f0: 2020 2077 6c65 6e20 3d20 3230 0a20 2020     wlen = 20.   
-0000d100: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000d110: 2020 2020 2020 2077 6c65 6e20 3d20 6e70         wlen = np
-0000d120: 7473 202a 2030 2e30 350a 2020 2020 2020  ts * 0.05.      
-0000d130: 2020 2320 7461 7065 7220 7661 6c75 6573    # taper values
-0000d140: 0a20 2020 2020 2020 2066 756e 6320 3d20  .        func = 
-0000d150: 5f67 6574 5f66 756e 6374 696f 6e5f 6672  _get_function_fr
-0000d160: 6f6d 5f65 6e74 7279 5f70 6f69 6e74 2822  om_entry_point("
-0000d170: 7461 7065 7222 2c20 2268 616e 6e22 290a  taper", "hann").
-0000d180: 2020 2020 2020 2020 6966 2032 202a 2077          if 2 * w
-0000d190: 6c65 6e20 3d3d 206e 7074 733a 0a20 2020  len == npts:.   
-0000d1a0: 2020 2020 2020 2020 2074 6170 6572 5f73           taper_s
-0000d1b0: 6964 6573 203d 2066 756e 6328 3220 2a20  ides = func(2 * 
-0000d1c0: 776c 656e 290a 2020 2020 2020 2020 656c  wlen).        el
-0000d1d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d1e0: 7461 7065 725f 7369 6465 7320 3d20 6675  taper_sides = fu
-0000d1f0: 6e63 2832 202a 2077 6c65 6e20 2b20 3129  nc(2 * wlen + 1)
-0000d200: 0a20 2020 2020 2020 2023 2074 6170 6572  .        # taper
-0000d210: 2077 696e 646f 770a 2020 2020 2020 2020   window.        
-0000d220: 7769 6e20 3d20 6e70 2e68 7374 6163 6b28  win = np.hstack(
-0000d230: 0a20 2020 2020 2020 2020 2020 2028 0a20  .            (. 
-0000d240: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000d250: 6170 6572 5f73 6964 6573 5b3a 776c 656e  aper_sides[:wlen
-0000d260: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000d270: 2020 206e 702e 6f6e 6573 286e 7074 7320     np.ones(npts 
-0000d280: 2d20 3220 2a20 776c 656e 292c 0a20 2020  - 2 * wlen),.   
-0000d290: 2020 2020 2020 2020 2020 2020 2074 6170               tap
-0000d2a0: 6572 5f73 6964 6573 5b6c 656e 2874 6170  er_sides[len(tap
-0000d2b0: 6572 5f73 6964 6573 2920 2d20 776c 656e  er_sides) - wlen
-0000d2c0: 203a 5d2c 0a20 2020 2020 2020 2020 2020   :],.           
-0000d2d0: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
-0000d2e0: 2020 2020 2066 6f72 2069 6920 696e 2072       for ii in r
-0000d2f0: 616e 6765 2864 6174 612e 7368 6170 655b  ange(data.shape[
-0000d300: 305d 293a 0a20 2020 2020 2020 2020 2020  0]):.           
-0000d310: 2064 6174 615b 6969 5d20 2a3d 2077 696e   data[ii] *= win
-0000d320: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
-0000d330: 0a0a 0a23 2040 6a69 7428 6e6f 7079 7468  ...# @jit(nopyth
-0000d340: 6f6e 203d 2054 7275 6529 0a0a 0a23 2063  on = True)...# c
-0000d350: 6861 6e67 6520 7468 6520 6d6f 7669 6e67  hange the moving
-0000d360: 2061 7665 7261 6765 2063 616c 6375 6c61   average calcula
-0000d370: 7469 6f6e 2074 6f20 7461 6b65 2061 7320  tion to take as 
-0000d380: 696e 7075 7420 4e20 7468 6520 6675 6c6c  input N the full
-0000d390: 2077 696e 646f 7720 6c65 6e67 7468 2074   window length t
-0000d3a0: 6f20 736d 6f6f 7468 0a64 6566 206d 6f76  o smooth.def mov
-0000d3b0: 696e 675f 6176 6528 412c 204e 293a 0a20  ing_ave(A, N):. 
-0000d3c0: 2020 2022 2222 0a20 2020 2041 6c74 6572     """.    Alter
-0000d3d0: 6e61 7469 7665 2066 756e 6374 696f 6e20  native function 
-0000d3e0: 666f 7220 6d6f 7669 6e67 2061 7665 7261  for moving avera
-0000d3f0: 6765 2066 6f72 2061 6e20 6172 7261 792e  ge for an array.
-0000d400: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-0000d410: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000d420: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2041  ----------.    A
-0000d430: 3a20 312d 4420 6172 7261 7920 6f66 2064  : 1-D array of d
-0000d440: 6174 6120 746f 2062 6520 736d 6f6f 7468  ata to be smooth
-0000d450: 6564 0a20 2020 204e 3a20 696e 7465 6765  ed.    N: intege
-0000d460: 722c 2069 7420 6465 6669 6e65 7320 7468  r, it defines th
-0000d470: 6520 6675 6c6c 2121 2077 696e 646f 7720  e full!! window 
-0000d480: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
-0000d490: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-0000d4a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000d4b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 423a 2031  -------.    B: 1
-0000d4c0: 2d44 2061 7272 6179 2077 6974 6820 736d  -D array with sm
-0000d4d0: 6f6f 7468 6564 2064 6174 610a 2020 2020  oothed data.    
-0000d4e0: 2222 220a 2020 2020 2320 6465 6669 6e65  """.    # define
-0000d4f0: 7320 616e 2061 7272 6179 2077 6974 6820  s an array with 
-0000d500: 4e20 6578 7472 6120 7361 6d70 6c65 7320  N extra samples 
-0000d510: 6174 2065 6974 6865 7220 7369 6465 0a20  at either side. 
-0000d520: 2020 2074 656d 7020 3d20 6e70 2e7a 6572     temp = np.zer
-0000d530: 6f73 286c 656e 2841 2920 2b20 3220 2a20  os(len(A) + 2 * 
-0000d540: 4e29 0a20 2020 2023 2073 6574 2074 6865  N).    # set the
-0000d550: 2063 656e 7472 616c 2070 6f72 7469 6f6e   central portion
-0000d560: 206f 6620 7468 6520 6172 7261 7920 746f   of the array to
-0000d570: 2041 0a20 2020 2074 656d 705b 4e3a 2d4e   A.    temp[N:-N
-0000d580: 5d20 3d20 410a 2020 2020 2320 6c65 6164  ] = A.    # lead
-0000d590: 696e 6720 7361 6d70 6c65 733a 2065 7175  ing samples: equ
-0000d5a0: 616c 2074 6f20 6669 7273 7420 7361 6d70  al to first samp
-0000d5b0: 6c65 206f 6620 6163 7475 616c 2061 7272  le of actual arr
-0000d5c0: 6179 0a20 2020 2074 656d 705b 303a 4e5d  ay.    temp[0:N]
-0000d5d0: 203d 2074 656d 705b 4e5d 0a20 2020 2023   = temp[N].    #
-0000d5e0: 2074 7261 696c 696e 6720 7361 6d70 6c65   trailing sample
-0000d5f0: 733a 2045 7175 616c 2074 6f20 6c61 7374  s: Equal to last
-0000d600: 2073 616d 706c 6520 6f66 2061 6374 7561   sample of actua
-0000d610: 6c20 6172 7261 790a 2020 2020 7465 6d70  l array.    temp
-0000d620: 5b2d 4e3a 5d20 3d20 7465 6d70 5b2d 4e20  [-N:] = temp[-N 
-0000d630: 2d20 315d 0a20 2020 2023 2063 6f6e 766f  - 1].    # convo
-0000d640: 6c76 6520 7769 7468 2061 2062 6f78 6361  lve with a boxca
-0000d650: 7220 616e 6420 6e6f 726d 616c 697a 652c  r and normalize,
-0000d660: 2061 6e64 2075 7365 206f 6e6c 7920 6365   and use only ce
-0000d670: 6e74 7261 6c20 706f 7274 696f 6e20 6f66  ntral portion of
-0000d680: 2074 6865 2072 6573 756c 740a 2020 2020   the result.    
-0000d690: 2320 7769 7468 206c 656e 6774 6820 6571  # with length eq
-0000d6a0: 7561 6c20 746f 2074 6865 206f 7269 6769  ual to the origi
-0000d6b0: 6e61 6c20 6172 7261 792c 2064 6973 6361  nal array, disca
-0000d6c0: 7264 696e 6720 7468 6520 6164 6465 6420  rding the added 
-0000d6d0: 6c65 6164 696e 6720 616e 6420 7472 6169  leading and trai
-0000d6e0: 6c69 6e67 2073 616d 706c 6573 0a20 2020  ling samples.   
-0000d6f0: 2042 203d 206e 702e 636f 6e76 6f6c 7665   B = np.convolve
-0000d700: 2874 656d 702c 206e 702e 6f6e 6573 284e  (temp, np.ones(N
-0000d710: 2920 2f20 4e2c 206d 6f64 653d 2273 616d  ) / N, mode="sam
-0000d720: 6522 295b 4e3a 2d4e 5d0a 2020 2020 7265  e")[N:-N].    re
-0000d730: 7475 726e 2042 0a0a 0a23 2063 6861 6e67  turn B...# chang
-0000d740: 6520 7468 6520 6d6f 7669 6e67 2061 7665  e the moving ave
-0000d750: 7261 6765 2063 616c 6375 6c61 7469 6f6e  rage calculation
-0000d760: 2074 6f20 7461 6b65 2061 7320 696e 7075   to take as inpu
-0000d770: 7420 4e20 7468 6520 6675 6c6c 2077 696e  t N the full win
-0000d780: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
-0000d790: 6f6f 7468 0a64 6566 206d 6f76 696e 675f  ooth.def moving_
-0000d7a0: 6176 655f 3244 2841 2c20 4e29 3a0a 2020  ave_2D(A, N):.  
-0000d7b0: 2020 2222 220a 2020 2020 416c 7465 726e    """.    Altern
-0000d7c0: 6174 6976 6520 6675 6e63 7469 6f6e 2066  ative function f
-0000d7d0: 6f72 206d 6f76 696e 6720 6176 6572 6167  or moving averag
-0000d7e0: 6520 666f 7220 616e 2061 7272 6179 2e0a  e for an array..
-0000d7f0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-0000d800: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000d810: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 413a  ---------.    A:
-0000d820: 2032 2d44 2061 7272 6179 206f 6620 6461   2-D array of da
-0000d830: 7461 2074 6f20 6265 2073 6d6f 6f74 6865  ta to be smoothe
-0000d840: 640a 2020 2020 4e3a 2069 6e74 6567 6572  d.    N: integer
-0000d850: 2c20 6974 2064 6566 696e 6573 2074 6865  , it defines the
-0000d860: 2066 756c 6c21 2120 7769 6e64 6f77 206c   full!! window l
-0000d870: 656e 6774 6820 746f 2073 6d6f 6f74 680a  ength to smooth.
-0000d880: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-0000d890: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000d8a0: 2d2d 2d2d 2d2d 0a20 2020 2042 3a20 322d  ------.    B: 2-
-0000d8b0: 4420 6172 7261 7920 7769 7468 2073 6d6f  D array with smo
-0000d8c0: 6f74 6865 6420 6461 7461 0a20 2020 2022  othed data.    "
-0000d8d0: 2222 0a20 2020 206e 7463 2c20 6e73 7074  "".    ntc, nspt
-0000d8e0: 203d 2041 2e73 6861 7065 0a20 2020 2023   = A.shape.    #
-0000d8f0: 2064 6566 696e 6573 2061 6e20 6172 7261   defines an arra
-0000d900: 7920 7769 7468 204e 2065 7874 7261 2073  y with N extra s
-0000d910: 616d 706c 6573 2061 7420 6569 7468 6572  amples at either
-0000d920: 2073 6964 650a 2020 2020 7465 6d70 203d   side.    temp =
-0000d930: 206e 702e 7a65 726f 7328 5b6e 7463 2c20   np.zeros([ntc, 
-0000d940: 6e73 7074 202b 2032 202a 204e 5d29 0a20  nspt + 2 * N]). 
-0000d950: 2020 2023 2073 6574 2074 6865 2063 656e     # set the cen
-0000d960: 7472 616c 2070 6f72 7469 6f6e 206f 6620  tral portion of 
-0000d970: 7468 6520 6172 7261 7920 746f 2041 0a20  the array to A. 
-0000d980: 2020 2074 656d 705b 3a2c 204e 3a2d 4e5d     temp[:, N:-N]
-0000d990: 203d 2041 0a20 2020 2023 206c 6561 6469   = A.    # leadi
-0000d9a0: 6e67 2073 616d 706c 6573 3a20 6571 7561  ng samples: equa
-0000d9b0: 6c20 746f 2066 6972 7374 2073 616d 706c  l to first sampl
-0000d9c0: 6520 6f66 2061 6374 7561 6c20 6172 7261  e of actual arra
-0000d9d0: 790a 2020 2020 7465 6d70 5b3a 2c20 303a  y.    temp[:, 0:
-0000d9e0: 4e5d 203d 206e 702e 7265 7065 6174 286e  N] = np.repeat(n
-0000d9f0: 702e 6578 7061 6e64 5f64 696d 7328 7465  p.expand_dims(te
-0000da00: 6d70 5b3a 2c20 4e5d 2c20 6178 6973 3d2d  mp[:, N], axis=-
-0000da10: 3129 2c20 4e2c 2061 7869 733d 2d31 290a  1), N, axis=-1).
-0000da20: 2020 2020 2320 7472 6169 6c69 6e67 2073      # trailing s
-0000da30: 616d 706c 6573 3a20 4571 7561 6c20 746f  amples: Equal to
-0000da40: 206c 6173 7420 7361 6d70 6c65 206f 6620   last sample of 
-0000da50: 6163 7475 616c 2061 7272 6179 0a20 2020  actual array.   
-0000da60: 2074 656d 705b 3a2c 202d 4e3a 5d20 3d20   temp[:, -N:] = 
-0000da70: 6e70 2e72 6570 6561 7428 6e70 2e65 7870  np.repeat(np.exp
-0000da80: 616e 645f 6469 6d73 2874 656d 705b 3a2c  and_dims(temp[:,
-0000da90: 202d 4e20 2d20 315d 2c20 6178 6973 3d2d   -N - 1], axis=-
-0000daa0: 3129 2c20 4e2c 2061 7869 733d 2d31 290a  1), N, axis=-1).
-0000dab0: 2020 2020 2320 636f 6e76 6f6c 7665 2077      # convolve w
-0000dac0: 6974 6820 6120 626f 7863 6172 2061 6e64  ith a boxcar and
-0000dad0: 206e 6f72 6d61 6c69 7a65 2c20 616e 6420   normalize, and 
-0000dae0: 7573 6520 6f6e 6c79 2063 656e 7472 616c  use only central
-0000daf0: 2070 6f72 7469 6f6e 206f 6620 7468 6520   portion of the 
-0000db00: 7265 7375 6c74 0a20 2020 2023 2077 6974  result.    # wit
-0000db10: 6820 6c65 6e67 7468 2065 7175 616c 2074  h length equal t
-0000db20: 6f20 7468 6520 6f72 6967 696e 616c 2061  o the original a
-0000db30: 7272 6179 2c20 6469 7363 6172 6469 6e67  rray, discarding
-0000db40: 2074 6865 2061 6464 6564 206c 6561 6469   the added leadi
-0000db50: 6e67 2061 6e64 2074 7261 696c 696e 6720  ng and trailing 
-0000db60: 7361 6d70 6c65 730a 2020 2020 4220 3d20  samples.    B = 
-0000db70: 7363 6970 792e 7369 676e 616c 2e63 6f6e  scipy.signal.con
-0000db80: 766f 6c76 6532 6428 7465 6d70 2c20 6e70  volve2d(temp, np
-0000db90: 2e65 7870 616e 645f 6469 6d73 286e 702e  .expand_dims(np.
-0000dba0: 6f6e 6573 284e 2920 2f20 4e2c 2061 7869  ones(N) / N, axi
-0000dbb0: 733d 3029 2c20 6d6f 6465 3d22 7361 6d65  s=0), mode="same
-0000dbc0: 2229 5b3a 2c20 4e3a 2d4e 5d0a 2020 2020  ")[:, N:-N].    
-0000dbd0: 7265 7475 726e 2042 0a0a 0a64 6566 2072  return B...def r
-0000dbe0: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
-0000dbf0: 7272 6179 2c20 6570 7369 6c6f 6e29 3a0a  rray, epsilon):.
-0000dc00: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
-0000dc10: 2069 7320 6120 726f 6275 7374 2073 7461   is a robust sta
-0000dc20: 636b 696e 6720 616c 676f 7269 7468 6d20  cking algorithm 
-0000dc30: 6465 7363 7269 6265 6420 696e 2050 616c  described in Pal
-0000dc40: 7669 7320 616e 6420 5665 726e 6f6e 2032  vis and Vernon 2
-0000dc50: 3031 300a 0a20 2020 2050 4152 414d 4554  010..    PARAMET
-0000dc60: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
-0000dc70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000dc80: 2020 2020 6363 5f61 7272 6179 3a20 6e75      cc_array: nu
-0000dc90: 6d70 792e 6e64 6172 7261 7920 636f 6e74  mpy.ndarray cont
-0000dca0: 6169 6e73 2074 6865 2032 4420 6372 6f73  ains the 2D cros
-0000dcb0: 7320 636f 7272 656c 6174 696f 6e20 6d61  s correlation ma
-0000dcc0: 7472 6978 0a20 2020 2065 7073 696c 6f6e  trix.    epsilon
-0000dcd0: 3a20 7265 7369 6475 616c 2074 6872 6568  : residual threh
-0000dce0: 6f6c 6420 746f 2071 7569 7420 7468 6520  old to quit the 
-0000dcf0: 6974 6572 6174 696f 6e0a 2020 2020 5245  iteration.    RE
-0000dd00: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-0000dd10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000dd20: 2d0a 2020 2020 6e65 7773 7461 636b 3a20  -.    newstack: 
-0000dd30: 6e75 6d70 7920 7665 6374 6f72 2063 6f6e  numpy vector con
-0000dd40: 7461 696e 7320 7468 6520 7374 6163 6b65  tains the stacke
-0000dd50: 6420 6372 6f73 7320 636f 7272 656c 6174  d cross correlat
-0000dd60: 696f 6e0a 0a20 2020 2057 7269 7474 656e  ion..    Written
-0000dd70: 2062 7920 4d61 7269 6e65 2044 656e 6f6c   by Marine Denol
-0000dd80: 6c65 0a20 2020 2022 2222 0a20 2020 2072  le.    """.    r
-0000dd90: 6573 203d 2039 6539 2020 2320 7265 7369  es = 9e9  # resi
-0000dda0: 6475 616c 730a 2020 2020 7720 3d20 6e70  duals.    w = np
-0000ddb0: 2e6f 6e65 7328 6363 5f61 7272 6179 2e73  .ones(cc_array.s
-0000ddc0: 6861 7065 5b30 5d29 0a20 2020 206e 7374  hape[0]).    nst
-0000ddd0: 6570 203d 2030 0a20 2020 206e 6577 7374  ep = 0.    newst
-0000dde0: 6163 6b20 3d20 6e70 2e6d 6564 6961 6e28  ack = np.median(
-0000ddf0: 6363 5f61 7272 6179 2c20 6178 6973 3d30  cc_array, axis=0
-0000de00: 290a 2020 2020 7768 696c 6520 7265 7320  ).    while res 
-0000de10: 3e20 6570 7369 6c6f 6e3a 0a20 2020 2020  > epsilon:.     
-0000de20: 2020 2073 7461 636b 203d 206e 6577 7374     stack = newst
-0000de30: 6163 6b0a 2020 2020 2020 2020 666f 7220  ack.        for 
-0000de40: 6920 696e 2072 616e 6765 2863 635f 6172  i in range(cc_ar
-0000de50: 7261 792e 7368 6170 655b 305d 293a 0a20  ray.shape[0]):. 
-0000de60: 2020 2020 2020 2020 2020 2063 7261 7020             crap 
-0000de70: 3d20 6e70 2e6d 756c 7469 706c 7928 7374  = np.multiply(st
-0000de80: 6163 6b2c 2063 635f 6172 7261 795b 692c  ack, cc_array[i,
-0000de90: 203a 5d2e 5429 0a20 2020 2020 2020 2020   :].T).         
-0000dea0: 2020 2063 7261 705f 646f 7420 3d20 6e70     crap_dot = np
-0000deb0: 2e73 756d 2863 7261 7029 0a20 2020 2020  .sum(crap).     
-0000dec0: 2020 2020 2020 2064 695f 6e6f 726d 203d         di_norm =
-0000ded0: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-0000dee0: 6363 5f61 7272 6179 5b69 2c20 3a5d 290a  cc_array[i, :]).
-0000def0: 2020 2020 2020 2020 2020 2020 7269 203d              ri =
-0000df00: 2063 635f 6172 7261 795b 692c 203a 5d20   cc_array[i, :] 
-0000df10: 2d20 6372 6170 5f64 6f74 202a 2073 7461  - crap_dot * sta
-0000df20: 636b 0a20 2020 2020 2020 2020 2020 2072  ck.            r
-0000df30: 695f 6e6f 726d 203d 206e 702e 6c69 6e61  i_norm = np.lina
-0000df40: 6c67 2e6e 6f72 6d28 7269 290a 2020 2020  lg.norm(ri).    
-0000df50: 2020 2020 2020 2020 775b 695d 203d 206e          w[i] = n
-0000df60: 702e 6162 7328 6372 6170 5f64 6f74 2920  p.abs(crap_dot) 
-0000df70: 2f20 6469 5f6e 6f72 6d20 2f20 7269 5f6e  / di_norm / ri_n
-0000df80: 6f72 6d20 2023 202f 6c65 6e28 6363 5f61  orm  # /len(cc_a
-0000df90: 7272 6179 5b3a 2c31 5d29 0a20 2020 2020  rray[:,1]).     
-0000dfa0: 2020 2023 2070 7269 6e74 2877 290a 2020     # print(w).  
-0000dfb0: 2020 2020 2020 7720 3d20 7720 2f20 6e70        w = w / np
-0000dfc0: 2e73 756d 2877 290a 2020 2020 2020 2020  .sum(w).        
-0000dfd0: 6e65 7773 7461 636b 203d 206e 702e 7375  newstack = np.su
-0000dfe0: 6d28 2877 202a 2063 635f 6172 7261 792e  m((w * cc_array.
-0000dff0: 5429 2e54 2c20 6178 6973 3d30 2920 2023  T).T, axis=0)  #
-0000e000: 202f 6c65 6e28 6363 5f61 7272 6179 5b3a   /len(cc_array[:
-0000e010: 2c31 5d29 0a20 2020 2020 2020 2072 6573  ,1]).        res
-0000e020: 203d 206e 702e 6c69 6e61 6c67 2e6e 6f72   = np.linalg.nor
-0000e030: 6d28 6e65 7773 7461 636b 202d 2073 7461  m(newstack - sta
-0000e040: 636b 2c20 6f72 643d 3129 202f 206e 702e  ck, ord=1) / np.
-0000e050: 6c69 6e61 6c67 2e6e 6f72 6d28 6e65 7773  linalg.norm(news
-0000e060: 7461 636b 2920 2f20 6c65 6e28 6363 5f61  tack) / len(cc_a
-0000e070: 7272 6179 5b3a 2c20 315d 290a 2020 2020  rray[:, 1]).    
-0000e080: 2020 2020 6e73 7465 7020 2b3d 2031 0a20      nstep += 1. 
-0000e090: 2020 2020 2020 2069 6620 6e73 7465 7020         if nstep 
-0000e0a0: 3e20 3130 3a0a 2020 2020 2020 2020 2020  > 10:.          
-0000e0b0: 2020 7265 7475 726e 206e 6577 7374 6163    return newstac
-0000e0c0: 6b2c 2077 2c20 6e73 7465 700a 2020 2020  k, w, nstep.    
-0000e0d0: 7265 7475 726e 206e 6577 7374 6163 6b2c  return newstack,
-0000e0e0: 2077 2c20 6e73 7465 700a 0a0a 6465 6620   w, nstep...def 
-0000e0f0: 7365 6c65 6374 6976 655f 7374 6163 6b28  selective_stack(
-0000e100: 6363 5f61 7272 6179 2c20 6570 7369 6c6f  cc_array, epsilo
-0000e110: 6e29 3a0a 2020 2020 2222 220a 2020 2020  n):.    """.    
-0000e120: 7468 6973 2069 7320 6120 7365 6c65 6374  this is a select
-0000e130: 6976 6520 7374 6163 6b69 6e67 2061 6c67  ive stacking alg
-0000e140: 6f72 6974 686d 2064 6576 656c 6f70 6564  orithm developed
-0000e150: 2062 7920 4a61 7265 6420 4272 7961 6e2e   by Jared Bryan.
-0000e160: 0a0a 2020 2020 5041 5241 4d45 5445 5253  ..    PARAMETERS
-0000e170: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-0000e180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0000e190: 2063 635f 6172 7261 793a 206e 756d 7079   cc_array: numpy
-0000e1a0: 2e6e 6461 7272 6179 2063 6f6e 7461 696e  .ndarray contain
-0000e1b0: 7320 7468 6520 3244 2063 726f 7373 2063  s the 2D cross c
-0000e1c0: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
-0000e1d0: 780a 2020 2020 6570 7369 6c6f 6e3a 2072  x.    epsilon: r
-0000e1e0: 6573 6964 7561 6c20 7468 7265 686f 6c64  esidual threhold
-0000e1f0: 2074 6f20 7175 6974 2074 6865 2069 7465   to quit the ite
-0000e200: 7261 7469 6f6e 0a20 2020 2052 4554 5552  ration.    RETUR
-0000e210: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-0000e220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0000e230: 2020 206e 6577 7374 6163 6b3a 206e 756d     newstack: num
-0000e240: 7079 2076 6563 746f 7220 636f 6e74 6169  py vector contai
-0000e250: 6e73 2074 6865 2073 7461 636b 6564 2063  ns the stacked c
-0000e260: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
-0000e270: 0a0a 2020 2020 5772 6974 7465 6e20 6279  ..    Written by
-0000e280: 204d 6172 696e 6520 4465 6e6f 6c6c 650a   Marine Denolle.
-0000e290: 2020 2020 2222 220a 2020 2020 6363 203d      """.    cc =
-0000e2a0: 206e 702e 6f6e 6573 2863 635f 6172 7261   np.ones(cc_arra
-0000e2b0: 792e 7368 6170 655b 305d 290a 2020 2020  y.shape[0]).    
-0000e2c0: 6e65 7773 7461 636b 203d 206e 702e 6d65  newstack = np.me
-0000e2d0: 616e 2863 635f 6172 7261 792c 2061 7869  an(cc_array, axi
-0000e2e0: 733d 3029 0a20 2020 2066 6f72 2069 2069  s=0).    for i i
-0000e2f0: 6e20 7261 6e67 6528 6363 5f61 7272 6179  n range(cc_array
-0000e300: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
-0000e310: 2020 2020 6363 5b69 5d20 3d20 6e70 2e73      cc[i] = np.s
-0000e320: 756d 286e 702e 6d75 6c74 6970 6c79 286e  um(np.multiply(n
-0000e330: 6577 7374 6163 6b2c 2063 635f 6172 7261  ewstack, cc_arra
-0000e340: 795b 692c 203a 5d2e 5429 290a 2020 2020  y[i, :].T)).    
-0000e350: 696b 203d 206e 702e 7768 6572 6528 6363  ik = np.where(cc
-0000e360: 203e 3d20 6570 7369 6c6f 6e29 5b30 5d0a   >= epsilon)[0].
-0000e370: 2020 2020 6e65 7773 7461 636b 203d 206e      newstack = n
-0000e380: 702e 6d65 616e 2863 635f 6172 7261 795b  p.mean(cc_array[
-0000e390: 696b 2c20 3a5d 2c20 6178 6973 3d30 290a  ik, :], axis=0).
-0000e3a0: 0a20 2020 2072 6574 7572 6e20 6e65 7773  .    return news
-0000e3b0: 7461 636b 2c20 6363 0a0a 0a64 6566 2077  tack, cc...def w
-0000e3c0: 6869 7465 6e5f 3144 2874 696d 6573 6572  hiten_1D(timeser
-0000e3d0: 6965 732c 2066 6674 5f70 6172 612c 206e  ies, fft_para, n
-0000e3e0: 5f74 6170 6572 293a 0a20 2020 2022 2222  _taper):.    """
-0000e3f0: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
-0000e400: 6f6e 2074 616b 6573 2061 2031 2d64 696d  on takes a 1-dim
-0000e410: 656e 7369 6f6e 616c 2074 696d 6573 6572  ensional timeser
-0000e420: 6965 7320 6172 7261 792c 2074 7261 6e73  ies array, trans
-0000e430: 666f 726d 7320 746f 2066 7265 7175 656e  forms to frequen
-0000e440: 6379 2064 6f6d 6169 6e20 7573 696e 6720  cy domain using 
-0000e450: 6666 742c 0a20 2020 2077 6869 7465 6e73  fft,.    whitens
-0000e460: 2074 6865 2061 6d70 6c69 7475 6465 206f   the amplitude o
-0000e470: 6620 7468 6520 7370 6563 7472 756d 2069  f the spectrum i
-0000e480: 6e20 6672 6571 7565 6e63 7920 646f 6d61  n frequency doma
-0000e490: 696e 2062 6574 7765 656e 202a 6672 6571  in between *freq
-0000e4a0: 6d69 6e2a 2061 6e64 202a 6672 6571 6d61  min* and *freqma
-0000e4b0: 782a 0a20 2020 2061 6e64 2072 6574 7572  x*.    and retur
-0000e4c0: 6e73 2074 6865 2077 6869 7465 6e65 6420  ns the whitened 
-0000e4d0: 6666 742e 0a20 2020 2050 4152 414d 4554  fft..    PARAMET
-0000e4e0: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
-0000e4f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000e500: 2020 2020 6461 7461 3a20 6e75 6d70 792e      data: numpy.
-0000e510: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
-0000e520: 2074 6865 2031 4420 7469 6d65 2073 6572   the 1D time ser
-0000e530: 6965 7320 746f 2077 6869 7465 6e0a 2020  ies to whiten.  
-0000e540: 2020 6666 745f 7061 7261 3a20 6469 6374    fft_para: dict
-0000e550: 2063 6f6e 7461 696e 696e 6720 616c 6c20   containing all 
-0000e560: 6666 745f 6363 2070 6172 616d 6574 6572  fft_cc parameter
-0000e570: 7320 7375 6368 2061 730a 2020 2020 2020  s such as.      
-0000e580: 2020 6474 3a20 5468 6520 7361 6d70 6c69    dt: The sampli
-0000e590: 6e67 2073 7061 6365 206f 6620 7468 6520  ng space of the 
-0000e5a0: 6064 6174 6160 0a20 2020 2020 2020 2066  `data`.        f
-0000e5b0: 7265 716d 696e 3a20 5468 6520 6c6f 7765  reqmin: The lowe
-0000e5c0: 7220 6672 6571 7565 6e63 7920 626f 756e  r frequency boun
-0000e5d0: 640a 2020 2020 2020 2020 6672 6571 6d61  d.        freqma
-0000e5e0: 783a 2054 6865 2075 7070 6572 2066 7265  x: The upper fre
-0000e5f0: 7175 656e 6379 2062 6f75 6e64 0a20 2020  quency bound.   
-0000e600: 2020 2020 2073 6d6f 6f74 685f 4e3a 2069       smooth_N: i
-0000e610: 6e74 6567 6572 2c20 6974 2064 6566 696e  nteger, it defin
-0000e620: 6573 2074 6865 2068 616c 6620 7769 6e64  es the half wind
-0000e630: 6f77 206c 656e 6774 6820 746f 2073 6d6f  ow length to smo
-0000e640: 6f74 680a 2020 2020 2020 2020 6e5f 7461  oth.        n_ta
-0000e650: 7065 722c 206f 7074 696f 6e61 6c3a 2069  per, optional: i
-0000e660: 6e74 6567 6572 2c20 6465 6669 6e65 2074  nteger, define t
-0000e670: 6865 2077 6964 7468 206f 6620 7468 6520  he width of the 
-0000e680: 7461 7065 7220 696e 2073 616d 706c 6573  taper in samples
-0000e690: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-0000e6a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000e6b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2046 4654  --------.    FFT
-0000e6c0: 5261 7753 6967 6e3a 206e 756d 7079 2e6e  RawSign: numpy.n
-0000e6d0: 6461 7272 6179 2063 6f6e 7461 696e 7320  darray contains 
-0000e6e0: 7468 6520 4646 5420 6f66 2074 6865 2077  the FFT of the w
-0000e6f0: 6869 7465 6e65 6420 696e 7075 7420 7472  hitened input tr
-0000e700: 6163 6520 6265 7477 6565 6e20 7468 6520  ace between the 
-0000e710: 6672 6571 7565 6e63 7920 626f 756e 6473  frequency bounds
-0000e720: 0a20 2020 2022 2222 0a20 2020 2023 206c  .    """.    # l
-0000e730: 6f61 6420 7061 7261 6d65 7465 7273 0a20  oad parameters. 
-0000e740: 2020 2064 656c 7461 203d 2066 6674 5f70     delta = fft_p
-0000e750: 6172 615b 2264 7422 5d0a 2020 2020 6672  ara["dt"].    fr
-0000e760: 6571 6d69 6e20 3d20 6666 745f 7061 7261  eqmin = fft_para
-0000e770: 5b22 6672 6571 6d69 6e22 5d0a 2020 2020  ["freqmin"].    
-0000e780: 6672 6571 6d61 7820 3d20 6666 745f 7061  freqmax = fft_pa
-0000e790: 7261 5b22 6672 6571 6d61 7822 5d0a 2020  ra["freqmax"].  
-0000e7a0: 2020 736d 6f6f 7468 5f4e 203d 2066 6674    smooth_N = fft
-0000e7b0: 5f70 6172 615b 2273 6d6f 6f74 685f 4e22  _para["smooth_N"
-0000e7c0: 5d0a 0a20 2020 206e 6666 7420 3d20 6e65  ]..    nfft = ne
-0000e7d0: 7874 5f66 6173 745f 6c65 6e28 6c65 6e28  xt_fast_len(len(
-0000e7e0: 7469 6d65 7365 7269 6573 2929 0a20 2020  timeseries)).   
-0000e7f0: 2073 7065 6320 3d20 6e70 2e66 6674 2e66   spec = np.fft.f
-0000e800: 6674 2874 696d 6573 6572 6965 732c 206e  ft(timeseries, n
-0000e810: 6666 7429 0a20 2020 2066 7265 7120 3d20  fft).    freq = 
-0000e820: 6e70 2e66 6674 2e66 6674 6672 6571 286e  np.fft.fftfreq(n
-0000e830: 6666 742c 2064 3d64 656c 7461 290a 0a20  fft, d=delta).. 
-0000e840: 2020 2069 7830 203d 206e 702e 6172 676d     ix0 = np.argm
-0000e850: 696e 286e 702e 6162 7328 6672 6571 202d  in(np.abs(freq -
-0000e860: 2066 7265 716d 696e 2929 0a20 2020 2069   freqmin)).    i
-0000e870: 7831 203d 206e 702e 6172 676d 696e 286e  x1 = np.argmin(n
-0000e880: 702e 6162 7328 6672 6571 202d 2066 7265  p.abs(freq - fre
-0000e890: 716d 6178 2929 0a0a 2020 2020 6966 2069  qmax))..    if i
-0000e8a0: 7831 202b 206e 5f74 6170 6572 203e 206e  x1 + n_taper > n
-0000e8b0: 6666 743a 0a20 2020 2020 2020 2069 7831  fft:.        ix1
-0000e8c0: 3120 3d20 6e66 6674 0a20 2020 2065 6c73  1 = nfft.    els
-0000e8d0: 653a 0a20 2020 2020 2020 2069 7831 3120  e:.        ix11 
-0000e8e0: 3d20 6978 3120 2b20 6e5f 7461 7065 720a  = ix1 + n_taper.
-0000e8f0: 0a20 2020 2069 6620 6978 3020 2d20 6e5f  .    if ix0 - n_
-0000e900: 7461 7065 7220 3c20 303a 0a20 2020 2020  taper < 0:.     
-0000e910: 2020 2069 7830 3020 3d20 300a 2020 2020     ix00 = 0.    
-0000e920: 656c 7365 3a0a 2020 2020 2020 2020 6978  else:.        ix
-0000e930: 3030 203d 2069 7830 202d 206e 5f74 6170  00 = ix0 - n_tap
-0000e940: 6572 0a0a 2020 2020 7370 6563 5f6f 7574  er..    spec_out
-0000e950: 203d 2073 7065 632e 636f 7079 2829 0a20   = spec.copy(). 
-0000e960: 2020 2073 7065 635f 6f75 745b 303a 6978     spec_out[0:ix
-0000e970: 3030 5d20 3d20 302e 3020 2b20 302e 306a  00] = 0.0 + 0.0j
-0000e980: 0a20 2020 2073 7065 635f 6f75 745b 6978  .    spec_out[ix
-0000e990: 3131 3a5d 203d 2030 2e30 202b 2030 2e30  11:] = 0.0 + 0.0
-0000e9a0: 6a0a 0a20 2020 2069 6620 736d 6f6f 7468  j..    if smooth
-0000e9b0: 5f4e 203c 3d20 313a 0a20 2020 2020 2020  _N <= 1:.       
-0000e9c0: 2073 7065 635f 6f75 745b 6978 3030 3a69   spec_out[ix00:i
-0000e9d0: 7831 315d 203d 206e 702e 6578 7028 312e  x11] = np.exp(1.
-0000e9e0: 306a 202a 206e 702e 616e 676c 6528 7370  0j * np.angle(sp
-0000e9f0: 6563 5f6f 7574 5b69 7830 303a 6978 3131  ec_out[ix00:ix11
-0000ea00: 5d29 290a 2020 2020 656c 7365 3a0a 2020  ])).    else:.  
-0000ea10: 2020 2020 2020 7370 6563 5f6f 7574 5b69        spec_out[i
-0000ea20: 7830 303a 6978 3131 5d20 2f3d 206d 6f76  x00:ix11] /= mov
-0000ea30: 696e 675f 6176 6528 6e70 2e61 6273 2873  ing_ave(np.abs(s
-0000ea40: 7065 635f 6f75 745b 6978 3030 3a69 7831  pec_out[ix00:ix1
-0000ea50: 315d 292c 2073 6d6f 6f74 685f 4e29 0a0a  1]), smooth_N)..
-0000ea60: 2020 2020 7820 3d20 6e70 2e6c 696e 7370      x = np.linsp
-0000ea70: 6163 6528 6e70 2e70 6920 2f20 322e 302c  ace(np.pi / 2.0,
-0000ea80: 206e 702e 7069 2c20 6978 3020 2d20 6978   np.pi, ix0 - ix
-0000ea90: 3030 290a 2020 2020 7370 6563 5f6f 7574  00).    spec_out
-0000eaa0: 5b69 7830 303a 6978 305d 202a 3d20 6e70  [ix00:ix0] *= np
-0000eab0: 2e63 6f73 2878 2920 2a2a 2032 0a0a 2020  .cos(x) ** 2..  
-0000eac0: 2020 7820 3d20 6e70 2e6c 696e 7370 6163    x = np.linspac
-0000ead0: 6528 302e 302c 206e 702e 7069 202f 2032  e(0.0, np.pi / 2
-0000eae0: 2e30 2c20 6978 3131 202d 2069 7831 290a  .0, ix11 - ix1).
-0000eaf0: 2020 2020 7370 6563 5f6f 7574 5b69 7831      spec_out[ix1
-0000eb00: 3a69 7831 315d 202a 3d20 6e70 2e63 6f73  :ix11] *= np.cos
-0000eb10: 2878 2920 2a2a 2032 0a0a 2020 2020 7265  (x) ** 2..    re
-0000eb20: 7475 726e 2073 7065 635f 6f75 740a 0a0a  turn spec_out...
-0000eb30: 6465 6620 7768 6974 656e 5f32 4428 7469  def whiten_2D(ti
-0000eb40: 6d65 7365 7269 6573 2c20 6666 745f 7061  meseries, fft_pa
-0000eb50: 7261 2c20 6e5f 7461 7065 7229 3a0a 2020  ra, n_taper):.  
-0000eb60: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
-0000eb70: 756e 6374 696f 6e20 7461 6b65 7320 6120  unction takes a 
-0000eb80: 322d 6469 6d65 6e73 696f 6e61 6c20 7469  2-dimensional ti
-0000eb90: 6d65 7365 7269 6573 2061 7272 6179 2c20  meseries array, 
-0000eba0: 7472 616e 7366 6f72 6d73 2074 6f20 6672  transforms to fr
-0000ebb0: 6571 7565 6e63 7920 646f 6d61 696e 2075  equency domain u
-0000ebc0: 7369 6e67 2066 6674 2c0a 2020 2020 7768  sing fft,.    wh
-0000ebd0: 6974 656e 7320 7468 6520 616d 706c 6974  itens the amplit
-0000ebe0: 7564 6520 6f66 2074 6865 2073 7065 6374  ude of the spect
-0000ebf0: 7275 6d20 696e 2066 7265 7175 656e 6379  rum in frequency
-0000ec00: 2064 6f6d 6169 6e20 6265 7477 6565 6e20   domain between 
-0000ec10: 2a66 7265 716d 696e 2a20 616e 6420 2a66  *freqmin* and *f
-0000ec20: 7265 716d 6178 2a0a 2020 2020 616e 6420  reqmax*.    and 
-0000ec30: 7265 7475 726e 7320 7468 6520 7768 6974  returns the whit
-0000ec40: 656e 6564 2066 6674 2e0a 2020 2020 5041  ened fft..    PA
-0000ec50: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
-0000ec60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ec70: 2d2d 2d2d 0a20 2020 2064 6174 613a 206e  ----.    data: n
-0000ec80: 756d 7079 2e6e 6461 7272 6179 2063 6f6e  umpy.ndarray con
-0000ec90: 7461 696e 7320 7468 6520 3144 2074 696d  tains the 1D tim
-0000eca0: 6520 7365 7269 6573 2074 6f20 7768 6974  e series to whit
-0000ecb0: 656e 0a20 2020 2066 6674 5f70 6172 613a  en.    fft_para:
-0000ecc0: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
-0000ecd0: 2061 6c6c 2066 6674 5f63 6320 7061 7261   all fft_cc para
-0000ece0: 6d65 7465 7273 2073 7563 6820 6173 0a20  meters such as. 
-0000ecf0: 2020 2020 2020 2064 743a 2054 6865 2073         dt: The s
-0000ed00: 616d 706c 696e 6720 7370 6163 6520 6f66  ampling space of
-0000ed10: 2074 6865 2060 6461 7461 600a 2020 2020   the `data`.    
-0000ed20: 2020 2020 6672 6571 6d69 6e3a 2054 6865      freqmin: The
-0000ed30: 206c 6f77 6572 2066 7265 7175 656e 6379   lower frequency
-0000ed40: 2062 6f75 6e64 0a20 2020 2020 2020 2066   bound.        f
-0000ed50: 7265 716d 6178 3a20 5468 6520 7570 7065  reqmax: The uppe
-0000ed60: 7220 6672 6571 7565 6e63 7920 626f 756e  r frequency boun
-0000ed70: 640a 2020 2020 2020 2020 736d 6f6f 7468  d.        smooth
-0000ed80: 5f4e 3a20 696e 7465 6765 722c 2069 7420  _N: integer, it 
-0000ed90: 6465 6669 6e65 7320 7468 6520 6861 6c66  defines the half
-0000eda0: 2077 696e 646f 7720 6c65 6e67 7468 2074   window length t
-0000edb0: 6f20 736d 6f6f 7468 0a20 2020 2020 2020  o smooth.       
-0000edc0: 206e 5f74 6170 6572 2c20 6f70 7469 6f6e   n_taper, option
-0000edd0: 616c 3a20 696e 7465 6765 722c 2064 6566  al: integer, def
-0000ede0: 696e 6520 7468 6520 7769 6474 6820 6f66  ine the width of
-0000edf0: 2074 6865 2074 6170 6572 2069 6e20 7361   the taper in sa
-0000ee00: 6d70 6c65 730a 2020 2020 5245 5455 524e  mples.    RETURN
-0000ee10: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-0000ee20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000ee30: 2020 4646 5452 6177 5369 676e 3a20 6e75    FFTRawSign: nu
-0000ee40: 6d70 792e 6e64 6172 7261 7920 636f 6e74  mpy.ndarray cont
-0000ee50: 6169 6e73 2074 6865 2046 4654 206f 6620  ains the FFT of 
-0000ee60: 7468 6520 7768 6974 656e 6564 2069 6e70  the whitened inp
-0000ee70: 7574 2074 7261 6365 2062 6574 7765 656e  ut trace between
-0000ee80: 2074 6865 2066 7265 7175 656e 6379 2062   the frequency b
-0000ee90: 6f75 6e64 730a 2020 2020 2222 220a 2020  ounds.    """.  
-0000eea0: 2020 2320 6c6f 6164 2070 6172 616d 6574    # load paramet
-0000eeb0: 6572 730a 2020 2020 6465 6c74 6120 3d20  ers.    delta = 
-0000eec0: 6666 745f 7061 7261 5b22 6474 225d 0a20  fft_para["dt"]. 
-0000eed0: 2020 2066 7265 716d 696e 203d 2066 6674     freqmin = fft
-0000eee0: 5f70 6172 615b 2266 7265 716d 696e 225d  _para["freqmin"]
-0000eef0: 0a20 2020 2066 7265 716d 6178 203d 2066  .    freqmax = f
-0000ef00: 6674 5f70 6172 615b 2266 7265 716d 6178  ft_para["freqmax
-0000ef10: 225d 0a20 2020 2073 6d6f 6f74 685f 4e20  "].    smooth_N 
-0000ef20: 3d20 6666 745f 7061 7261 5b22 736d 6f6f  = fft_para["smoo
-0000ef30: 7468 5f4e 225d 0a0a 2020 2020 6e66 6674  th_N"]..    nfft
-0000ef40: 203d 206e 6578 745f 6661 7374 5f6c 656e   = next_fast_len
-0000ef50: 2874 696d 6573 6572 6965 732e 7368 6170  (timeseries.shap
-0000ef60: 655b 315d 290a 2020 2020 7370 6563 203d  e[1]).    spec =
-0000ef70: 206e 702e 6666 742e 6666 746e 2874 696d   np.fft.fftn(tim
-0000ef80: 6573 6572 6965 732c 2073 3d5b 6e66 6674  eseries, s=[nfft
-0000ef90: 5d29 0a20 2020 2066 7265 7120 3d20 6e70  ]).    freq = np
-0000efa0: 2e66 6674 2e66 6674 6672 6571 286e 6666  .fft.fftfreq(nff
-0000efb0: 742c 2064 3d64 656c 7461 290a 0a20 2020  t, d=delta)..   
-0000efc0: 2069 7830 203d 206e 702e 6172 676d 696e   ix0 = np.argmin
-0000efd0: 286e 702e 6162 7328 6672 6571 202d 2066  (np.abs(freq - f
-0000efe0: 7265 716d 696e 2929 0a20 2020 2069 7831  reqmin)).    ix1
-0000eff0: 203d 206e 702e 6172 676d 696e 286e 702e   = np.argmin(np.
-0000f000: 6162 7328 6672 6571 202d 2066 7265 716d  abs(freq - freqm
-0000f010: 6178 2929 0a0a 2020 2020 6966 2069 7831  ax))..    if ix1
-0000f020: 202b 206e 5f74 6170 6572 203e 206e 6666   + n_taper > nff
-0000f030: 743a 0a20 2020 2020 2020 2069 7831 3120  t:.        ix11 
-0000f040: 3d20 6e66 6674 0a20 2020 2065 6c73 653a  = nfft.    else:
-0000f050: 0a20 2020 2020 2020 2069 7831 3120 3d20  .        ix11 = 
-0000f060: 6978 3120 2b20 6e5f 7461 7065 720a 0a20  ix1 + n_taper.. 
-0000f070: 2020 2069 6620 6978 3020 2d20 6e5f 7461     if ix0 - n_ta
-0000f080: 7065 7220 3c20 303a 0a20 2020 2020 2020  per < 0:.       
-0000f090: 2069 7830 3020 3d20 300a 2020 2020 656c   ix00 = 0.    el
-0000f0a0: 7365 3a0a 2020 2020 2020 2020 6978 3030  se:.        ix00
-0000f0b0: 203d 2069 7830 202d 206e 5f74 6170 6572   = ix0 - n_taper
-0000f0c0: 0a0a 2020 2020 7370 6563 5f6f 7574 203d  ..    spec_out =
-0000f0d0: 2073 7065 632e 636f 7079 2829 2020 2320   spec.copy()  # 
-0000f0e0: 6d61 7920 6265 2069 6e63 6f6e 7665 6e69  may be inconveni
-0000f0f0: 656e 7420 6475 6520 746f 2068 6967 6865  ent due to highe
-0000f100: 7220 6d65 6d6f 7279 2075 7361 6765 0a20  r memory usage. 
-0000f110: 2020 2073 7065 635f 6f75 745b 3a2c 2030     spec_out[:, 0
-0000f120: 3a69 7830 305d 203d 2030 2e30 202b 2030  :ix00] = 0.0 + 0
-0000f130: 2e30 6a0a 2020 2020 7370 6563 5f6f 7574  .0j.    spec_out
-0000f140: 5b3a 2c20 6978 3131 3a5d 203d 2030 2e30  [:, ix11:] = 0.0
-0000f150: 202b 2030 2e30 6a0a 0a20 2020 2069 6620   + 0.0j..    if 
-0000f160: 736d 6f6f 7468 5f4e 203c 3d20 313a 0a20  smooth_N <= 1:. 
-0000f170: 2020 2020 2020 2073 7065 635f 6f75 745b         spec_out[
-0000f180: 3a2c 2069 7830 303a 6978 3131 5d20 3d20  :, ix00:ix11] = 
-0000f190: 6e70 2e65 7870 2831 2e30 6a20 2a20 6e70  np.exp(1.0j * np
-0000f1a0: 2e61 6e67 6c65 2873 7065 635f 6f75 745b  .angle(spec_out[
-0000f1b0: 3a2c 2069 7830 303a 6978 3131 5d29 290a  :, ix00:ix11])).
-0000f1c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f1d0: 2020 7370 6563 5f6f 7574 5b3a 2c20 6978    spec_out[:, ix
-0000f1e0: 3030 3a69 7831 315d 202f 3d20 6d6f 7669  00:ix11] /= movi
-0000f1f0: 6e67 5f61 7665 5f32 4428 6e70 2e61 6273  ng_ave_2D(np.abs
-0000f200: 2873 7065 635f 6f75 745b 3a2c 2069 7830  (spec_out[:, ix0
-0000f210: 303a 6978 3131 5d29 2c20 736d 6f6f 7468  0:ix11]), smooth
-0000f220: 5f4e 290a 0a20 2020 2078 203d 206e 702e  _N)..    x = np.
-0000f230: 6c69 6e73 7061 6365 286e 702e 7069 202f  linspace(np.pi /
-0000f240: 2032 2e30 2c20 6e70 2e70 692c 2069 7830   2.0, np.pi, ix0
-0000f250: 202d 2069 7830 3029 0a20 2020 2073 7065   - ix00).    spe
-0000f260: 635f 6f75 745b 3a2c 2069 7830 303a 6978  c_out[:, ix00:ix
-0000f270: 305d 202a 3d20 6e70 2e63 6f73 2878 2920  0] *= np.cos(x) 
-0000f280: 2a2a 2032 0a0a 2020 2020 7820 3d20 6e70  ** 2..    x = np
-0000f290: 2e6c 696e 7370 6163 6528 302e 302c 206e  .linspace(0.0, n
-0000f2a0: 702e 7069 202f 2032 2e30 2c20 6978 3131  p.pi / 2.0, ix11
-0000f2b0: 202d 2069 7831 290a 2020 2020 7370 6563   - ix1).    spec
-0000f2c0: 5f6f 7574 5b3a 2c20 6978 313a 6978 3131  _out[:, ix1:ix11
-0000f2d0: 5d20 2a3d 206e 702e 636f 7328 7829 202a  ] *= np.cos(x) *
-0000f2e0: 2a20 320a 0a20 2020 2072 6574 7572 6e20  * 2..    return 
-0000f2f0: 7370 6563 5f6f 7574 0a0a 0a64 6566 2077  spec_out...def w
-0000f300: 6869 7465 6e28 6461 7461 2c20 6666 745f  hiten(data, fft_
-0000f310: 7061 7261 2c20 6e5f 7461 7065 723d 3130  para, n_taper=10
-0000f320: 3029 3a0a 2020 2020 2222 220a 2020 2020  0):.    """.    
-0000f330: 5468 6973 2066 756e 6374 696f 6e20 7461  This function ta
-0000f340: 6b65 7320 6120 7469 6d65 7365 7269 6573  kes a timeseries
-0000f350: 2061 7272 6179 2c20 7472 616e 7366 6f72   array, transfor
-0000f360: 6d73 2074 6f20 6672 6571 7565 6e63 7920  ms to frequency 
-0000f370: 646f 6d61 696e 2075 7369 6e67 2066 6674  domain using fft
-0000f380: 2c0a 2020 2020 7768 6974 656e 7320 7468  ,.    whitens th
-0000f390: 6520 616d 706c 6974 7564 6520 6f66 2074  e amplitude of t
-0000f3a0: 6865 2073 7065 6374 7275 6d20 696e 2066  he spectrum in f
-0000f3b0: 7265 7175 656e 6379 2064 6f6d 6169 6e20  requency domain 
-0000f3c0: 6265 7477 6565 6e20 2a66 7265 716d 696e  between *freqmin
-0000f3d0: 2a20 616e 6420 2a66 7265 716d 6178 2a0a  * and *freqmax*.
-0000f3e0: 2020 2020 616e 6420 7265 7475 726e 7320      and returns 
-0000f3f0: 7468 6520 7768 6974 656e 6564 2066 6674  the whitened fft
-0000f400: 2e0a 2020 2020 5041 5241 4d45 5445 5253  ..    PARAMETERS
-0000f410: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-0000f420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0000f430: 2064 6174 613a 206e 756d 7079 2e6e 6461   data: numpy.nda
-0000f440: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
-0000f450: 6520 3144 2074 696d 6520 7365 7269 6573  e 1D time series
-0000f460: 2074 6f20 7768 6974 656e 0a20 2020 2066   to whiten.    f
-0000f470: 6674 5f70 6172 613a 2064 6963 7420 636f  ft_para: dict co
-0000f480: 6e74 6169 6e69 6e67 2061 6c6c 2066 6674  ntaining all fft
-0000f490: 5f63 6320 7061 7261 6d65 7465 7273 2073  _cc parameters s
-0000f4a0: 7563 6820 6173 0a20 2020 2020 2020 2064  uch as.        d
-0000f4b0: 743a 2054 6865 2073 616d 706c 696e 6720  t: The sampling 
-0000f4c0: 7370 6163 6520 6f66 2074 6865 2060 6461  space of the `da
-0000f4d0: 7461 600a 2020 2020 2020 2020 6672 6571  ta`.        freq
-0000f4e0: 6d69 6e3a 2054 6865 206c 6f77 6572 2066  min: The lower f
-0000f4f0: 7265 7175 656e 6379 2062 6f75 6e64 0a20  requency bound. 
-0000f500: 2020 2020 2020 2066 7265 716d 6178 3a20         freqmax: 
-0000f510: 5468 6520 7570 7065 7220 6672 6571 7565  The upper freque
-0000f520: 6e63 7920 626f 756e 640a 2020 2020 2020  ncy bound.      
-0000f530: 2020 736d 6f6f 7468 5f4e 3a20 696e 7465    smooth_N: inte
-0000f540: 6765 722c 2069 7420 6465 6669 6e65 7320  ger, it defines 
-0000f550: 7468 6520 6861 6c66 2077 696e 646f 7720  the half window 
-0000f560: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
-0000f570: 0a20 2020 2020 2020 2066 7265 715f 6e6f  .        freq_no
-0000f580: 726d 3a20 7768 6974 656e 696e 6720 6d65  rm: whitening me
-0000f590: 7468 6f64 2062 6574 7765 656e 2027 6f6e  thod between 'on
-0000f5a0: 652d 6269 7427 2061 6e64 2027 524d 4127  e-bit' and 'RMA'
-0000f5b0: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-0000f5c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000f5d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2046 4654  --------.    FFT
-0000f5e0: 5261 7753 6967 6e3a 206e 756d 7079 2e6e  RawSign: numpy.n
-0000f5f0: 6461 7272 6179 2063 6f6e 7461 696e 7320  darray contains 
-0000f600: 7468 6520 4646 5420 6f66 2074 6865 2077  the FFT of the w
-0000f610: 6869 7465 6e65 6420 696e 7075 7420 7472  hitened input tr
-0000f620: 6163 6520 6265 7477 6565 6e20 7468 6520  ace between the 
-0000f630: 6672 6571 7565 6e63 7920 626f 756e 6473  frequency bounds
-0000f640: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
-0000f650: 5370 6565 6420 7570 2046 4654 2062 7920  Speed up FFT by 
-0000f660: 7061 6464 696e 6720 746f 206f 7074 696d  padding to optim
-0000f670: 616c 2073 697a 6520 666f 7220 4646 5450  al size for FFTP
-0000f680: 4143 4b0a 2020 2020 6966 2064 6174 612e  ACK.    if data.
-0000f690: 6e64 696d 203d 3d20 313a 0a20 2020 2020  ndim == 1:.     
-0000f6a0: 2020 2046 4654 5261 7753 6967 6e20 3d20     FFTRawSign = 
-0000f6b0: 7768 6974 656e 5f31 4428 6461 7461 2c20  whiten_1D(data, 
-0000f6c0: 6666 745f 7061 7261 2c20 6e5f 7461 7065  fft_para, n_tape
-0000f6d0: 7229 0a20 2020 2020 2020 2023 2041 5252  r).        # ARR
-0000f6e0: 5f4f 5554 3a20 4f6e 6c79 2066 6f72 2063  _OUT: Only for c
-0000f6f0: 6f6e 7369 7374 656e 6379 2077 6974 6820  onsistency with 
-0000f700: 6e6f 6973 6570 7920 6170 7072 6f61 6368  noisepy approach
-0000f710: 206f 6620 686f 6c64 696e 6720 7468 6520   of holding the 
-0000f720: 6675 6c6c 0a20 2020 2020 2020 2023 2073  full.        # s
-0000f730: 7065 6374 7275 6d20 286e 6f74 206a 7573  pectrum (not jus
-0000f740: 7420 3020 616e 6420 706f 7369 7469 7665  t 0 and positive
-0000f750: 2066 7265 712e 2070 6172 7429 0a20 2020   freq. part).   
-0000f760: 2020 2020 2061 7272 5f6f 7574 203d 206e       arr_out = n
-0000f770: 702e 7a65 726f 7328 2846 4654 5261 7753  p.zeros((FFTRawS
-0000f780: 6967 6e2e 7368 6170 655b 305d 202d 2031  ign.shape[0] - 1
-0000f790: 2920 2a20 3220 2b20 312c 2064 7479 7065  ) * 2 + 1, dtype
-0000f7a0: 3d63 6f6d 706c 6578 290a 2020 2020 2020  =complex).      
-0000f7b0: 2020 6172 725f 6f75 745b 3020 3a20 4646    arr_out[0 : FF
-0000f7c0: 5452 6177 5369 676e 2e73 6861 7065 5b30  TRawSign.shape[0
-0000f7d0: 5d5d 203d 2046 4654 5261 7753 6967 6e0a  ]] = FFTRawSign.
-0000f7e0: 2020 2020 2020 2020 6172 725f 6f75 745b          arr_out[
-0000f7f0: 4646 5452 6177 5369 676e 2e73 6861 7065  FFTRawSign.shape
-0000f800: 5b30 5d20 3a5d 203d 2046 4654 5261 7753  [0] :] = FFTRawS
-0000f810: 6967 6e5b 313a 5d2e 636f 6e6a 7567 6174  ign[1:].conjugat
-0000f820: 6528 295b 3a3a 2d31 5d0a 0a20 2020 2065  e()[::-1]..    e
-0000f830: 6c69 6620 6461 7461 2e6e 6469 6d20 3d3d  lif data.ndim ==
-0000f840: 2032 3a0a 2020 2020 2020 2020 4646 5452   2:.        FFTR
-0000f850: 6177 5369 676e 203d 2077 6869 7465 6e5f  awSign = whiten_
-0000f860: 3244 2864 6174 612c 2066 6674 5f70 6172  2D(data, fft_par
-0000f870: 612c 206e 5f74 6170 6572 290a 2020 2020  a, n_taper).    
-0000f880: 2020 2020 6172 725f 6f75 7420 3d20 6e70      arr_out = np
-0000f890: 2e7a 6572 6f73 2828 4646 5452 6177 5369  .zeros((FFTRawSi
-0000f8a0: 676e 2e73 6861 7065 5b30 5d2c 2028 4646  gn.shape[0], (FF
-0000f8b0: 5452 6177 5369 676e 2e73 6861 7065 5b31  TRawSign.shape[1
-0000f8c0: 5d20 2d20 3129 202a 2032 202b 2031 292c  ] - 1) * 2 + 1),
-0000f8d0: 2064 7479 7065 3d63 6f6d 706c 6578 290a   dtype=complex).
-0000f8e0: 2020 2020 2020 2020 6172 725f 6f75 745b          arr_out[
-0000f8f0: 3a2c 2046 4654 5261 7753 6967 6e2e 7368  :, FFTRawSign.sh
-0000f900: 6170 655b 315d 203a 5d20 3d20 4646 5452  ape[1] :] = FFTR
-0000f910: 6177 5369 676e 5b3a 2c20 313a 5d2e 636f  awSign[:, 1:].co
-0000f920: 6e6a 7567 6174 6528 295b 3a3a 2d31 5d0a  njugate()[::-1].
-0000f930: 2020 2020 7265 7475 726e 2046 4654 5261      return FFTRa
-0000f940: 7753 6967 6e0a 0a0a 6465 6620 6164 6170  wSign...def adap
-0000f950: 7469 7665 5f66 696c 7465 7228 6172 722c  tive_filter(arr,
-0000f960: 2067 293a 0a20 2020 2022 2222 0a20 2020   g):.    """.   
-0000f970: 2074 6865 2061 6461 7074 6976 6520 636f   the adaptive co
-0000f980: 7661 7269 616e 6365 2066 696c 7465 7220  variance filter 
-0000f990: 746f 2065 6e68 616e 6365 2063 6f68 6572  to enhance coher
-0000f9a0: 656e 7420 7369 676e 616c 732e 2046 656c  ent signals. Fel
-0000f9b0: 6c6f 7773 2074 6865 206d 6574 686f 6420  lows the method 
-0000f9c0: 6f66 0a20 2020 204e 616b 6174 6120 6574  of.    Nakata et
-0000f9d0: 2061 6c2e 2c20 3230 3135 2028 4170 7065   al., 2015 (Appe
-0000f9e0: 6e64 6978 2042 290a 0a20 2020 2074 6865  ndix B)..    the
-0000f9f0: 2066 696c 7465 7265 6420 7369 676e 616c   filtered signal
-0000fa00: 205b 7831 5d20 6973 2067 6976 656e 2062   [x1] is given b
-0000fa10: 7920 7831 203d 2069 6666 7428 502a 7831  y x1 = ifft(P*x1
-0000fa20: 2877 2929 2077 6865 7265 2078 3120 6973  (w)) where x1 is
-0000fa30: 2074 6865 2066 6674 6564 2073 7065 6374   the ffted spect
-0000fa40: 7261 0a20 2020 2061 6e64 2050 2069 7320  ra.    and P is 
-0000fa50: 7468 6520 6669 6c74 6572 2e20 5020 6973  the filter. P is
-0000fa60: 2063 6f6e 7374 7275 6374 6564 2062 7920   constructed by 
-0000fa70: 7573 696e 6720 7468 6520 7465 6d70 6f72  using the tempor
-0000fa80: 616c 2063 6f76 6172 6961 6e63 6520 6d61  al covariance ma
-0000fa90: 7472 6978 2e0a 0a20 2020 2050 4152 414d  trix...    PARAM
-0000faa0: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
-0000fab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fac0: 2d0a 2020 2020 6172 723a 206e 756d 7079  -.    arr: numpy
-0000fad0: 2e6e 6461 7272 6179 2063 6f6e 7461 696e  .ndarray contain
-0000fae0: 7320 7468 6520 3244 2074 7261 6365 7320  s the 2D traces 
-0000faf0: 6f66 2064 6169 6c79 2f68 6f75 726c 7920  of daily/hourly 
-0000fb00: 6372 6f73 732d 636f 7272 656c 6174 696f  cross-correlatio
-0000fb10: 6e20 6675 6e63 7469 6f6e 730a 2020 2020  n functions.    
-0000fb20: 673a 2061 2070 6f73 6974 6976 6520 6e75  g: a positive nu
-0000fb30: 6d62 6572 2074 6f20 6164 6a75 7374 2074  mber to adjust t
-0000fb40: 6865 2066 696c 7465 7220 6861 7273 686e  he filter harshn
-0000fb50: 6573 730a 2020 2020 5245 5455 524e 533a  ess.    RETURNS:
-0000fb60: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000fb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-0000fb80: 6e61 7272 3a20 6e75 6d70 7920 7665 6374  narr: numpy vect
-0000fb90: 6f72 2063 6f6e 7461 696e 7320 7468 6520  or contains the 
-0000fba0: 7374 6163 6b65 6420 6372 6f73 7320 636f  stacked cross co
-0000fbb0: 7272 656c 6174 696f 6e20 6675 6e63 7469  rrelation functi
-0000fbc0: 6f6e 0a20 2020 2022 2222 0a20 2020 2069  on.    """.    i
-0000fbd0: 6620 6172 722e 6e64 696d 203d 3d20 313a  f arr.ndim == 1:
-0000fbe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fbf0: 6172 720a 2020 2020 4e2c 204d 203d 2061  arr.    N, M = a
-0000fc00: 7272 2e73 6861 7065 0a20 2020 204e 6666  rr.shape.    Nff
-0000fc10: 7420 3d20 6e65 7874 5f66 6173 745f 6c65  t = next_fast_le
-0000fc20: 6e28 4d29 0a0a 2020 2020 2320 6666 7420  n(M)..    # fft 
-0000fc30: 7468 6520 3244 2061 7272 6179 0a20 2020  the 2D array.   
-0000fc40: 2073 7065 6320 3d20 7363 6970 792e 6666   spec = scipy.ff
-0000fc50: 7470 6163 6b2e 6666 7428 6172 722c 2061  tpack.fft(arr, a
-0000fc60: 7869 733d 312c 206e 3d4e 6666 7429 5b3a  xis=1, n=Nfft)[:
-0000fc70: 2c20 3a4d 5d0a 0a20 2020 2023 206d 616b  , :M]..    # mak
-0000fc80: 6520 6372 6f73 732d 7370 6563 7472 6d20  e cross-spectrm 
-0000fc90: 6d61 7472 6978 0a20 2020 2063 7370 6563  matrix.    cspec
-0000fca0: 203d 206e 702e 7a65 726f 7328 7368 6170   = np.zeros(shap
-0000fcb0: 653d 284e 202a 204e 2c20 4d29 2c20 6474  e=(N * N, M), dt
-0000fcc0: 7970 653d 6e70 2e63 6f6d 706c 6578 3634  ype=np.complex64
-0000fcd0: 290a 2020 2020 666f 7220 6969 2069 6e20  ).    for ii in 
-0000fce0: 7261 6e67 6528 4e29 3a0a 2020 2020 2020  range(N):.      
-0000fcf0: 2020 666f 7220 6a6a 2069 6e20 7261 6e67    for jj in rang
-0000fd00: 6528 4e29 3a0a 2020 2020 2020 2020 2020  e(N):.          
-0000fd10: 2020 6b6b 203d 2069 6920 2a20 4e20 2b20    kk = ii * N + 
-0000fd20: 6a6a 0a20 2020 2020 2020 2020 2020 2063  jj.            c
-0000fd30: 7370 6563 5b6b 6b5d 203d 2073 7065 635b  spec[kk] = spec[
-0000fd40: 6969 5d20 2a20 6e70 2e63 6f6e 6a75 6761  ii] * np.conjuga
-0000fd50: 7465 2873 7065 635b 6a6a 5d29 0a0a 2020  te(spec[jj])..  
-0000fd60: 2020 5331 203d 206e 702e 7a65 726f 7328    S1 = np.zeros(
-0000fd70: 4d2c 2064 7479 7065 3d6e 702e 636f 6d70  M, dtype=np.comp
-0000fd80: 6c65 7836 3429 0a20 2020 2053 3220 3d20  lex64).    S2 = 
-0000fd90: 6e70 2e7a 6572 6f73 284d 2c20 6474 7970  np.zeros(M, dtyp
-0000fda0: 653d 6e70 2e63 6f6d 706c 6578 3634 290a  e=np.complex64).
-0000fdb0: 2020 2020 2320 636f 6e73 7472 7563 7420      # construct 
-0000fdc0: 7468 6520 6669 6c74 6572 2050 0a20 2020  the filter P.   
-0000fdd0: 2066 6f72 2069 6920 696e 2072 616e 6765   for ii in range
-0000fde0: 284e 293a 0a20 2020 2020 2020 206d 6d20  (N):.        mm 
-0000fdf0: 3d20 6969 202a 204e 202b 2069 690a 2020  = ii * N + ii.  
-0000fe00: 2020 2020 2020 5332 202b 3d20 6373 7065        S2 += cspe
-0000fe10: 635b 6d6d 5d0a 2020 2020 2020 2020 666f  c[mm].        fo
-0000fe20: 7220 6a6a 2069 6e20 7261 6e67 6528 4e29  r jj in range(N)
-0000fe30: 3a0a 2020 2020 2020 2020 2020 2020 6b6b  :.            kk
-0000fe40: 203d 2069 6920 2a20 4e20 2b20 6a6a 0a20   = ii * N + jj. 
-0000fe50: 2020 2020 2020 2020 2020 2053 3120 2b3d             S1 +=
-0000fe60: 2063 7370 6563 5b6b 6b5d 0a0a 2020 2020   cspec[kk]..    
-0000fe70: 7020 3d20 6e70 2e70 6f77 6572 2828 5331  p = np.power((S1
-0000fe80: 202d 2053 3229 202f 2028 5332 202a 2028   - S2) / (S2 * (
-0000fe90: 4e20 2d20 3129 292c 2067 290a 0a20 2020  N - 1)), g)..   
-0000fea0: 2023 206d 616b 6520 6966 6674 0a20 2020   # make ifft.   
-0000feb0: 206e 6172 7220 3d20 6e70 2e72 6561 6c28   narr = np.real(
-0000fec0: 7363 6970 792e 6666 7470 6163 6b2e 6966  scipy.fftpack.if
-0000fed0: 6674 286e 702e 6d75 6c74 6970 6c79 2870  ft(np.multiply(p
-0000fee0: 2c20 7370 6563 292c 204e 6666 742c 2061  , spec), Nfft, a
-0000fef0: 7869 733d 3129 5b3a 2c20 3a4d 5d29 0a20  xis=1)[:, :M]). 
-0000ff00: 2020 2072 6574 7572 6e20 6e70 2e6d 6561     return np.mea
-0000ff10: 6e28 6e61 7272 2c20 6178 6973 3d30 290a  n(narr, axis=0).
-0000ff20: 0a0a 6465 6620 7077 7328 6172 722c 2073  ..def pws(arr, s
-0000ff30: 616d 706c 696e 675f 7261 7465 2c20 706f  ampling_rate, po
-0000ff40: 7765 723d 322c 2070 7773 5f74 696d 6567  wer=2, pws_timeg
-0000ff50: 6174 653d 352e 3029 3a0a 2020 2020 2222  ate=5.0):.    ""
-0000ff60: 220a 2020 2020 5065 7266 6f72 6d73 2070  ".    Performs p
-0000ff70: 6861 7365 2d77 6569 6768 7465 6420 7374  hase-weighted st
-0000ff80: 6163 6b20 6f6e 2061 7272 6179 206f 6620  ack on array of 
-0000ff90: 7469 6d65 2073 6572 6965 732e 204d 6f64  time series. Mod
-0000ffa0: 6966 6965 6420 6f6e 2074 6865 206e 6f69  ified on the noi
-0000ffb0: 7365 2066 756e 6374 696f 6e20 6279 2054  se function by T
-0000ffc0: 696d 2043 6c69 6d65 6e74 732e 0a20 2020  im Climents..   
-0000ffd0: 2046 6f6c 6c6f 7773 206d 6574 686f 6473   Follows methods
-0000ffe0: 206f 6620 5363 6869 6d6d 656c 2061 6e64   of Schimmel and
-0000fff0: 2050 6175 6c73 7365 6e2c 2031 3939 372e   Paulssen, 1997.
-00010000: 0a20 2020 2049 6620 7328 7429 2069 7320  .    If s(t) is 
-00010010: 7469 6d65 2073 6572 6965 7320 6461 7461  time series data
-00010020: 2028 7365 6973 6d6f 6772 616d 2c20 6f72   (seismogram, or
-00010030: 2063 726f 7373 2d63 6f72 7265 6c61 7469   cross-correlati
-00010040: 6f6e 292c 0a20 2020 2053 2874 2920 3d20  on),.    S(t) = 
-00010050: 7328 7429 202b 2069 2a48 2873 2874 2929  s(t) + i*H(s(t))
-00010060: 2c20 7768 6572 6520 4828 7328 7429 2920  , where H(s(t)) 
-00010070: 6973 2048 696c 6265 7274 2074 7261 6e73  is Hilbert trans
-00010080: 666f 726d 206f 6620 7328 7429 0a20 2020  form of s(t).   
-00010090: 2053 2874 2920 3d20 7328 7429 202b 2069   S(t) = s(t) + i
-000100a0: 2a48 2873 2874 2929 203d 2041 2874 292a  *H(s(t)) = A(t)*
-000100b0: 6578 7028 692a 7068 6928 7429 292c 2077  exp(i*phi(t)), w
-000100c0: 6865 7265 0a20 2020 2041 2874 2920 6973  here.    A(t) is
-000100d0: 2065 6e76 656c 6f70 6520 6f66 2073 2874   envelope of s(t
-000100e0: 2920 616e 6420 7068 6928 7429 2069 7320  ) and phi(t) is 
-000100f0: 7068 6173 6520 6f66 2073 2874 290a 2020  phase of s(t).  
-00010100: 2020 5068 6173 652d 7765 6967 6874 6564    Phase-weighted
-00010110: 2073 7461 636b 2c20 6728 7429 2c20 6973   stack, g(t), is
-00010120: 2074 6865 6e3a 0a20 2020 2067 2874 2920   then:.    g(t) 
-00010130: 3d20 312f 4e20 7375 6d20 6a20 3d20 313a  = 1/N sum j = 1:
-00010140: 4e20 735f 6a28 7429 202a 207c 2031 2f4e  N s_j(t) * | 1/N
-00010150: 2073 756d 206b 203d 2031 3a4e 2065 7870   sum k = 1:N exp
-00010160: 5b69 202a 2070 6869 5f6b 2874 295d 7c5e  [i * phi_k(t)]|^
-00010170: 760a 2020 2020 7768 6572 6520 4e20 6973  v.    where N is
-00010180: 206e 756d 6265 7220 6f66 2074 7261 6365   number of trace
-00010190: 7320 7573 6564 2c20 7620 6973 2073 6861  s used, v is sha
-000101a0: 7270 6e65 7373 206f 6620 7068 6173 652d  rpness of phase-
-000101b0: 7765 6967 6874 6564 2073 7461 636b 0a0a  weighted stack..
-000101c0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-000101d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-000101e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6172  ---------.    ar
-000101f0: 723a 204e 206c 656e 6774 6820 6172 7261  r: N length arra
-00010200: 7920 6f66 2074 696d 6520 7365 7269 6573  y of time series
-00010210: 2064 6174 6120 286e 756d 7079 2e6e 6461   data (numpy.nda
-00010220: 7272 6179 290a 2020 2020 7361 6d70 6c69  rray).    sampli
-00010230: 6e67 5f72 6174 653a 2073 616d 706c 696e  ng_rate: samplin
-00010240: 6720 7261 7465 206f 6620 7469 6d65 2073  g rate of time s
-00010250: 6572 6965 7320 6172 7220 2869 6e74 290a  eries arr (int).
-00010260: 2020 2020 706f 7765 723a 2065 7870 6f6e      power: expon
-00010270: 656e 7420 666f 7220 7068 6173 6520 7374  ent for phase st
-00010280: 6163 6b20 2869 6e74 290a 2020 2020 7077  ack (int).    pw
-00010290: 735f 7469 6d65 6761 7465 3a20 6e75 6d62  s_timegate: numb
-000102a0: 6572 206f 6620 7365 636f 6e64 7320 746f  er of seconds to
-000102b0: 2073 6d6f 6f74 6820 7068 6173 6520 7374   smooth phase st
-000102c0: 6163 6b20 2866 6c6f 6174 290a 0a20 2020  ack (float)..   
-000102d0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-000102e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000102f0: 2d2d 2d0a 2020 2020 7765 6967 6874 6564  ---.    weighted
-00010300: 3a20 5068 6173 6520 7765 6967 6874 6564  : Phase weighted
-00010310: 2073 7461 636b 206f 6620 7469 6d65 2073   stack of time s
-00010320: 6572 6965 7320 6461 7461 2028 6e75 6d70  eries data (nump
-00010330: 792e 6e64 6172 7261 7929 0a20 2020 2022  y.ndarray).    "
-00010340: 2222 0a0a 2020 2020 6966 2061 7272 2e6e  ""..    if arr.n
-00010350: 6469 6d20 3d3d 2031 3a0a 2020 2020 2020  dim == 1:.      
-00010360: 2020 7265 7475 726e 2061 7272 0a20 2020    return arr.   
-00010370: 204e 2c20 4d20 3d20 6172 722e 7368 6170   N, M = arr.shap
-00010380: 650a 2020 2020 616e 616c 7974 6963 203d  e.    analytic =
-00010390: 2068 696c 6265 7274 2861 7272 2c20 6178   hilbert(arr, ax
-000103a0: 6973 3d31 2c20 4e3d 6e65 7874 5f66 6173  is=1, N=next_fas
-000103b0: 745f 6c65 6e28 4d29 295b 3a2c 203a 4d5d  t_len(M))[:, :M]
-000103c0: 0a20 2020 2070 6861 7365 203d 206e 702e  .    phase = np.
-000103d0: 616e 676c 6528 616e 616c 7974 6963 290a  angle(analytic).
-000103e0: 2020 2020 7068 6173 655f 7374 6163 6b20      phase_stack 
-000103f0: 3d20 6e70 2e6d 6561 6e28 6e70 2e65 7870  = np.mean(np.exp
-00010400: 2831 6a20 2a20 7068 6173 6529 2c20 6178  (1j * phase), ax
-00010410: 6973 3d30 290a 2020 2020 7068 6173 655f  is=0).    phase_
-00010420: 7374 6163 6b20 3d20 6e70 2e61 6273 2870  stack = np.abs(p
-00010430: 6861 7365 5f73 7461 636b 2920 2a2a 2028  hase_stack) ** (
-00010440: 706f 7765 7229 0a0a 2020 2020 2320 736d  power)..    # sm
-00010450: 6f6f 7468 696e 670a 2020 2020 2320 7469  oothing.    # ti
-00010460: 6d65 6761 7465 5f73 616d 706c 6573 203d  megate_samples =
-00010470: 2069 6e74 2870 7773 5f74 696d 6567 6174   int(pws_timegat
-00010480: 6520 2a20 7361 6d70 6c69 6e67 5f72 6174  e * sampling_rat
-00010490: 6529 0a20 2020 2023 2070 6861 7365 5f73  e).    # phase_s
-000104a0: 7461 636b 203d 206d 6f76 696e 675f 6176  tack = moving_av
-000104b0: 6528 7068 6173 655f 7374 6163 6b2c 7469  e(phase_stack,ti
-000104c0: 6d65 6761 7465 5f73 616d 706c 6573 290a  megate_samples).
-000104d0: 2020 2020 7765 6967 6874 6564 203d 206e      weighted = n
-000104e0: 702e 6d75 6c74 6970 6c79 2861 7272 2c20  p.multiply(arr, 
-000104f0: 7068 6173 655f 7374 6163 6b29 0a20 2020  phase_stack).   
-00010500: 2072 6574 7572 6e20 6e70 2e6d 6561 6e28   return np.mean(
-00010510: 7765 6967 6874 6564 2c20 6178 6973 3d30  weighted, axis=0
-00010520: 290a 0a0a 6465 6620 6e72 6f6f 745f 7374  )...def nroot_st
-00010530: 6163 6b28 6363 5f61 7272 6179 2c20 706f  ack(cc_array, po
-00010540: 7765 7229 3a0a 2020 2020 2222 220a 2020  wer):.    """.  
-00010550: 2020 7468 6973 2069 7320 6e74 682d 726f    this is nth-ro
-00010560: 6f74 2073 7461 636b 696e 6720 616c 676f  ot stacking algo
-00010570: 7269 7468 6d20 7472 616e 736c 6174 6564  rithm translated
-00010580: 2062 6173 6564 206f 6e20 7468 6520 6d61   based on the ma
-00010590: 746c 6162 2066 756e 6374 696f 6e0a 2020  tlab function.  
-000105a0: 2020 6672 6f6d 2068 7474 7073 3a2f 2f67    from https://g
-000105b0: 6974 6875 622e 636f 6d2f 7874 7961 6e67  ithub.com/xtyang
-000105c0: 7073 702f 5365 6973 5374 6163 6b20 2862  psp/SeisStack (b
-000105d0: 7920 5869 616f 7461 6f20 5961 6e67 3b20  y Xiaotao Yang; 
-000105e0: 666f 6c6c 6f77 7320 7468 650a 2020 2020  follows the.    
-000105f0: 7265 6665 7265 6e63 6520 6f66 204d 696c  reference of Mil
-00010600: 6c65 742c 2046 2065 7420 616c 2e2c 2032  let, F et al., 2
-00010610: 3031 3920 4a47 5229 0a0a 2020 2020 5061  019 JGR)..    Pa
-00010620: 7261 6d65 7465 7273 3a0a 2020 2020 2d2d  rameters:.    --
-00010630: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
-00010640: 635f 6172 7261 793a 206e 756d 7079 2e6e  c_array: numpy.n
-00010650: 6461 7272 6179 2063 6f6e 7461 696e 7320  darray contains 
-00010660: 7468 6520 3244 2063 726f 7373 2063 6f72  the 2D cross cor
-00010670: 7265 6c61 7469 6f6e 206d 6174 7269 780a  relation matrix.
-00010680: 2020 2020 706f 7765 723a 206e 702e 696e      power: np.in
-00010690: 742c 206e 7468 2072 6f6f 7420 666f 7220  t, nth root for 
-000106a0: 7468 6520 7374 6163 6b69 6e67 0a0a 2020  the stacking..  
-000106b0: 2020 5265 7475 726e 733a 0a20 2020 202d    Returns:.    -
-000106c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-000106d0: 6e73 7461 636b 3a20 6e70 2e6e 6461 7272  nstack: np.ndarr
-000106e0: 6179 2c20 6669 6e61 6c20 7374 6163 6b65  ay, final stacke
-000106f0: 6420 7761 7665 666f 726d 730a 0a20 2020  d waveforms..   
-00010700: 2057 7269 7474 656e 2062 7920 4368 656e   Written by Chen
-00010710: 6778 696e 204a 6961 6e67 2040 414e 5520  gxin Jiang @ANU 
-00010720: 284d 6179 3230 3230 290a 2020 2020 2222  (May2020).    ""
-00010730: 220a 2020 2020 6966 2063 635f 6172 7261  ".    if cc_arra
-00010740: 792e 6e64 696d 203d 3d20 313a 0a20 2020  y.ndim == 1:.   
-00010750: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00010760: 6728 2232 4420 6d61 7472 6978 2069 7320  g("2D matrix is 
-00010770: 6e65 6564 6564 2066 6f72 206e 726f 6f74  needed for nroot
-00010780: 5f73 7461 636b 2229 0a20 2020 2020 2020  _stack").       
-00010790: 2072 6574 7572 6e20 6363 5f61 7272 6179   return cc_array
-000107a0: 0a20 2020 204e 2c20 4d20 3d20 6363 5f61  .    N, M = cc_a
-000107b0: 7272 6179 2e73 6861 7065 0a20 2020 2064  rray.shape.    d
-000107c0: 6f75 7420 3d20 6e70 2e7a 6572 6f73 284d  out = np.zeros(M
-000107d0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-000107e0: 3332 290a 0a20 2020 2023 2063 6f6e 7374  32)..    # const
-000107f0: 7275 6374 2079 0a20 2020 2066 6f72 2069  ruct y.    for i
-00010800: 6920 696e 2072 616e 6765 284e 293a 0a20  i in range(N):. 
-00010810: 2020 2020 2020 2064 6174 203d 2063 635f         dat = cc_
-00010820: 6172 7261 795b 6969 2c20 3a5d 0a20 2020  array[ii, :].   
-00010830: 2020 2020 2064 6f75 7420 2b3d 206e 702e       dout += np.
-00010840: 7369 676e 2864 6174 2920 2a20 6e70 2e61  sign(dat) * np.a
-00010850: 6273 2864 6174 2920 2a2a 2028 3120 2f20  bs(dat) ** (1 / 
-00010860: 706f 7765 7229 0a20 2020 2064 6f75 7420  power).    dout 
-00010870: 2f3d 204e 0a0a 2020 2020 2320 7468 6520  /= N..    # the 
-00010880: 6669 6e61 6c20 7374 6163 6b65 6420 7761  final stacked wa
-00010890: 7665 666f 726d 0a20 2020 206e 7374 6163  veform.    nstac
-000108a0: 6b20 3d20 646f 7574 202a 206e 702e 6162  k = dout * np.ab
-000108b0: 7328 646f 7574 2920 2a2a 2028 706f 7765  s(dout) ** (powe
-000108c0: 7220 2d20 3129 0a0a 2020 2020 7265 7475  r - 1)..    retu
-000108d0: 726e 206e 7374 6163 6b0a 0a0a 6465 6620  rn nstack...def 
-000108e0: 7365 6c65 6374 6976 655f 7374 6163 6b28  selective_stack(
-000108f0: 6363 5f61 7272 6179 2c20 6570 7369 6c6f  cc_array, epsilo
-00010900: 6e2c 2063 635f 7468 293a 2020 2320 6e6f  n, cc_th):  # no
-00010910: 7161 3a20 4638 3131 0a20 2020 2022 2222  qa: F811.    """
-00010920: 0a20 2020 2074 6869 7320 6973 2061 2073  .    this is a s
-00010930: 656c 6563 7469 7665 2073 7461 636b 696e  elective stackin
-00010940: 6720 616c 676f 7269 7468 6d20 6465 7665  g algorithm deve
-00010950: 6c6f 7065 6420 6279 204a 6172 6564 2042  loped by Jared B
-00010960: 7279 616e 2f4b 7572 616d 6120 4f6b 7562  ryan/Kurama Okub
-00010970: 6f2e 0a0a 2020 2020 5041 5241 4d45 5445  o...    PARAMETE
-00010980: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-00010990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-000109a0: 2020 2063 635f 6172 7261 793a 206e 756d     cc_array: num
-000109b0: 7079 2e6e 6461 7272 6179 2063 6f6e 7461  py.ndarray conta
-000109c0: 696e 7320 7468 6520 3244 2063 726f 7373  ins the 2D cross
-000109d0: 2063 6f72 7265 6c61 7469 6f6e 206d 6174   correlation mat
-000109e0: 7269 780a 2020 2020 6570 7369 6c6f 6e3a  rix.    epsilon:
-000109f0: 2072 6573 6964 7561 6c20 7468 7265 686f   residual threho
-00010a00: 6c64 2074 6f20 7175 6974 2074 6865 2069  ld to quit the i
-00010a10: 7465 7261 7469 6f6e 0a20 2020 2063 635f  teration.    cc_
-00010a20: 7468 3a20 6e75 6d70 792e 666c 6f61 742c  th: numpy.float,
-00010a30: 2074 6872 6573 686f 6c64 206f 6620 636f   threshold of co
-00010a40: 7272 656c 6174 696f 6e20 636f 6566 6669  rrelation coeffi
-00010a50: 6369 656e 7420 746f 2062 6520 7365 6c65  cient to be sele
-00010a60: 6374 6564 0a0a 2020 2020 5245 5455 524e  cted..    RETURN
-00010a70: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00010a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00010a90: 2020 6e65 7773 7461 636b 3a20 6e75 6d70    newstack: nump
-00010aa0: 7920 7665 6374 6f72 2063 6f6e 7461 696e  y vector contain
-00010ab0: 7320 7468 6520 7374 6163 6b65 6420 6372  s the stacked cr
-00010ac0: 6f73 7320 636f 7272 656c 6174 696f 6e0a  oss correlation.
-00010ad0: 2020 2020 6e73 7465 703a 206e 702e 696e      nstep: np.in
-00010ae0: 742c 2074 6f74 616c 206e 756d 6265 7220  t, total number 
-00010af0: 6f66 2069 7465 7261 7469 6f6e 7320 666f  of iterations fo
-00010b00: 7220 7468 6520 7374 6163 6b69 6e67 0a0a  r the stacking..
-00010b10: 2020 2020 4f72 6967 696e 616c 6c79 2072      Originally r
-00010b20: 6974 7465 6e20 6279 204d 6172 696e 6520  itten by Marine 
-00010b30: 4465 6e6f 6c6c 650a 2020 2020 4d6f 6469  Denolle.    Modi
-00010b40: 6669 6564 2062 7920 4368 656e 6778 696e  fied by Chengxin
-00010b50: 204a 6961 6e67 2040 4861 7276 6172 6420   Jiang @Harvard 
-00010b60: 284f 6374 3230 3230 290a 2020 2020 2222  (Oct2020).    ""
-00010b70: 220a 2020 2020 6966 2063 635f 6172 7261  ".    if cc_arra
-00010b80: 792e 6e64 696d 203d 3d20 313a 0a20 2020  y.ndim == 1:.   
-00010b90: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00010ba0: 6728 2232 4420 6d61 7472 6978 2069 7320  g("2D matrix is 
-00010bb0: 6e65 6564 6564 2066 6f72 206e 726f 6f74  needed for nroot
-00010bc0: 5f73 7461 636b 2229 0a20 2020 2020 2020  _stack").       
-00010bd0: 2072 6574 7572 6e20 6363 5f61 7272 6179   return cc_array
-00010be0: 0a20 2020 204e 2c20 4d20 3d20 6363 5f61  .    N, M = cc_a
-00010bf0: 7272 6179 2e73 6861 7065 0a0a 2020 2020  rray.shape..    
-00010c00: 7265 7320 3d20 3965 3920 2023 2072 6573  res = 9e9  # res
-00010c10: 6964 7561 6c73 0a20 2020 2063 6f66 203d  iduals.    cof =
-00010c20: 206e 702e 7a65 726f 7328 4e2c 2064 7479   np.zeros(N, dty
-00010c30: 7065 3d6e 702e 666c 6f61 7433 3229 0a20  pe=np.float32). 
-00010c40: 2020 206e 6577 7374 6163 6b20 3d20 6e70     newstack = np
-00010c50: 2e6d 6561 6e28 6363 5f61 7272 6179 2c20  .mean(cc_array, 
-00010c60: 6178 6973 3d30 290a 0a20 2020 206e 7374  axis=0)..    nst
-00010c70: 6570 203d 2030 0a20 2020 2023 2073 7461  ep = 0.    # sta
-00010c80: 7274 2069 7465 7261 7469 6f6e 0a20 2020  rt iteration.   
-00010c90: 2077 6869 6c65 2072 6573 203e 2065 7073   while res > eps
-00010ca0: 696c 6f6e 3a0a 2020 2020 2020 2020 666f  ilon:.        fo
-00010cb0: 7220 6969 2069 6e20 7261 6e67 6528 4e29  r ii in range(N)
-00010cc0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00010cd0: 665b 6969 5d20 3d20 6e70 2e63 6f72 7263  f[ii] = np.corrc
-00010ce0: 6f65 6628 6e65 7773 7461 636b 2c20 6363  oef(newstack, cc
-00010cf0: 5f61 7272 6179 5b69 692c 203a 5d29 5b30  _array[ii, :])[0
-00010d00: 2c20 315d 0a0a 2020 2020 2020 2020 2320  , 1]..        # 
-00010d10: 6669 6e64 2067 6f6f 6420 7761 7665 666f  find good wavefo
-00010d20: 726d 730a 2020 2020 2020 2020 696e 6478  rms.        indx
-00010d30: 203d 206e 702e 7768 6572 6528 636f 6620   = np.where(cof 
-00010d40: 3e3d 2063 635f 7468 295b 305d 0a20 2020  >= cc_th)[0].   
-00010d50: 2020 2020 2069 6620 6e6f 7420 6c65 6e28       if not len(
-00010d60: 696e 6478 293a 0a20 2020 2020 2020 2020  indx):.         
-00010d70: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00010d80: 726f 7228 2263 616e 6e6f 7420 6669 6e64  ror("cannot find
-00010d90: 2067 6f6f 6420 7761 7665 666f 726d 7320   good waveforms 
-00010da0: 696e 7369 6465 2073 656c 6563 7469 7665  inside selective
-00010db0: 2073 7461 636b 696e 6722 290a 2020 2020   stacking").    
-00010dc0: 2020 2020 6f6c 6473 7461 636b 203d 206e      oldstack = n
-00010dd0: 6577 7374 6163 6b0a 2020 2020 2020 2020  ewstack.        
-00010de0: 6e65 7773 7461 636b 203d 206e 702e 6d65  newstack = np.me
-00010df0: 616e 2863 635f 6172 7261 795b 696e 6478  an(cc_array[indx
-00010e00: 5d2c 2061 7869 733d 3029 0a20 2020 2020  ], axis=0).     
-00010e10: 2020 2072 6573 203d 206e 702e 6c69 6e61     res = np.lina
-00010e20: 6c67 2e6e 6f72 6d28 6e65 7773 7461 636b  lg.norm(newstack
-00010e30: 202d 206f 6c64 7374 6163 6b29 202f 2028   - oldstack) / (
-00010e40: 6e70 2e6c 696e 616c 672e 6e6f 726d 286e  np.linalg.norm(n
-00010e50: 6577 7374 6163 6b29 202a 204d 290a 2020  ewstack) * M).  
-00010e60: 2020 2020 2020 6e73 7465 7020 2b3d 2031        nstep += 1
-00010e70: 0a0a 2020 2020 7265 7475 726e 206e 6577  ..    return new
-00010e80: 7374 6163 6b2c 206e 7374 6570 0a0a 0a64  stack, nstep...d
-00010e90: 6566 2067 6574 5f63 6328 7331 2c20 735f  ef get_cc(s1, s_
-00010ea0: 7265 6629 3a0a 2020 2020 2320 7265 7475  ref):.    # retu
-00010eb0: 726e 7320 7468 6520 636f 7272 656c 6174  rns the correlat
-00010ec0: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
-00010ed0: 6265 7477 6565 6e20 7761 7665 666f 726d  between waveform
-00010ee0: 7320 696e 2073 3120 6167 6169 6e73 7420  s in s1 against 
-00010ef0: 7265 6665 7265 6e63 650a 2020 2020 2320  reference.    # 
-00010f00: 7761 7665 666f 726d 2073 5f72 6566 2e0a  waveform s_ref..
-00010f10: 2020 2020 230a 2020 2020 6363 203d 206e      #.    cc = n
-00010f20: 702e 7a65 726f 7328 7331 2e73 6861 7065  p.zeros(s1.shape
-00010f30: 5b30 5d29 0a20 2020 2073 5f72 6566 5f6e  [0]).    s_ref_n
-00010f40: 6f72 6d20 3d20 6e70 2e6c 696e 616c 672e  orm = np.linalg.
-00010f50: 6e6f 726d 2873 5f72 6566 290a 2020 2020  norm(s_ref).    
-00010f60: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00010f70: 312e 7368 6170 655b 305d 293a 0a20 2020  1.shape[0]):.   
-00010f80: 2020 2020 2063 635b 695d 203d 206e 702e       cc[i] = np.
-00010f90: 7375 6d28 6e70 2e6d 756c 7469 706c 7928  sum(np.multiply(
-00010fa0: 7331 5b69 2c20 3a5d 2c20 735f 7265 6629  s1[i, :], s_ref)
-00010fb0: 2920 2f20 6e70 2e6c 696e 616c 672e 6e6f  ) / np.linalg.no
-00010fc0: 726d 2873 315b 692c 203a 5d29 202f 2073  rm(s1[i, :]) / s
-00010fd0: 5f72 6566 5f6e 6f72 6d0a 2020 2020 7265  _ref_norm.    re
-00010fe0: 7475 726e 2063 630a 0a0a 2323 2323 2323  turn cc...######
-00010ff0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b250: 2323 2323 2323 230a 0a0a 6465 6620 6368  #######...def ch
+0000b260: 6563 6b5f 7361 6d70 6c65 5f67 6170 7328  eck_sample_gaps(
+0000b270: 7374 7265 616d 3a20 6f62 7370 792e 5374  stream: obspy.St
+0000b280: 7265 616d 2c20 7374 6172 7474 696d 653a  ream, starttime:
+0000b290: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
+0000b2a0: 6d65 2c20 656e 6474 696d 653a 206f 6273  me, endtime: obs
+0000b2b0: 7079 2e55 5443 4461 7465 5469 6d65 293a  py.UTCDateTime):
+0000b2c0: 0a20 2020 2022 2222 0a20 2020 2074 6869  .    """.    thi
+0000b2d0: 7320 6675 6e63 7469 6f6e 2063 6865 636b  s function check
+0000b2e0: 7320 7361 6d70 6c69 6e67 2072 6174 6520  s sampling rate 
+0000b2f0: 616e 6420 6669 6e64 2067 6170 7320 6f66  and find gaps of
+0000b300: 2061 6c6c 2074 7261 6365 7320 696e 2073   all traces in s
+0000b310: 7472 6561 6d2e 0a20 2020 2050 4152 414d  tream..    PARAM
+0000b320: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+0000b330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000b340: 2073 7472 6561 6d3a 206f 6273 7079 2073   stream: obspy s
+0000b350: 7472 6561 6d20 6f62 6a65 6374 2e0a 2020  tream object..  
+0000b360: 2020 6461 7465 5f69 6e66 6f3a 2064 6963    date_info: dic
+0000b370: 7420 6f66 2073 7461 7274 696e 6720 616e  t of starting an
+0000b380: 6420 656e 6469 6e67 2074 696d 6520 6f66  d ending time of
+0000b390: 2074 6865 2073 7472 6561 6d0a 0a20 2020   the stream..   
+0000b3a0: 2052 4554 5552 454e 533a 0a20 2020 202d   RETURENS:.    -
+0000b3b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b3c0: 0a20 2020 2073 7472 6561 6d3a 204c 6973  .    stream: Lis
+0000b3d0: 7420 6f66 2067 6f6f 6420 7472 6163 6573  t of good traces
+0000b3e0: 2069 6e20 7468 6520 7374 7265 616d 0a20   in the stream. 
+0000b3f0: 2020 2022 2222 0a20 2020 2023 2072 656d     """.    # rem
+0000b400: 6f76 6520 656d 7074 792f 6269 6720 7472  ove empty/big tr
+0000b410: 6163 6573 0a20 2020 2069 6620 6c65 6e28  aces.    if len(
+0000b420: 7374 7265 616d 2920 3d3d 2030 206f 7220  stream) == 0 or 
+0000b430: 6c65 6e28 7374 7265 616d 2920 3e20 3130  len(stream) > 10
+0000b440: 303a 0a20 2020 2020 2020 2073 7472 6561  0:.        strea
+0000b450: 6d20 3d20 5b5d 0a20 2020 2020 2020 2072  m = [].        r
+0000b460: 6574 7572 6e20 7374 7265 616d 0a0a 2020  eturn stream..  
+0000b470: 2020 2320 7265 6d6f 7665 2074 7261 6365    # remove trace
+0000b480: 7320 7769 7468 2062 6967 2067 6170 730a  s with big gaps.
+0000b490: 2020 2020 6966 2070 6f72 7469 6f6e 5f67      if portion_g
+0000b4a0: 6170 7328 7374 7265 616d 2c20 7374 6172  aps(stream, star
+0000b4b0: 7474 696d 652c 2065 6e64 7469 6d65 2920  ttime, endtime) 
+0000b4c0: 3e20 302e 333a 0a20 2020 2020 2020 2073  > 0.3:.        s
+0000b4d0: 7472 6561 6d20 3d20 5b5d 0a20 2020 2020  tream = [].     
+0000b4e0: 2020 2072 6574 7572 6e20 7374 7265 616d     return stream
+0000b4f0: 0a0a 2020 2020 6672 6571 7320 3d20 5b5d  ..    freqs = []
+0000b500: 0a20 2020 2066 6f72 2074 7220 696e 2073  .    for tr in s
+0000b510: 7472 6561 6d3a 0a20 2020 2020 2020 2066  tream:.        f
+0000b520: 7265 7173 2e61 7070 656e 6428 696e 7428  reqs.append(int(
+0000b530: 7472 2e73 7461 7473 2e73 616d 706c 696e  tr.stats.samplin
+0000b540: 675f 7261 7465 2929 0a20 2020 2066 7265  g_rate)).    fre
+0000b550: 7120 3d20 6d61 7828 6672 6571 7329 0a20  q = max(freqs). 
+0000b560: 2020 2066 6f72 2074 7220 696e 2073 7472     for tr in str
+0000b570: 6561 6d3a 0a20 2020 2020 2020 2069 6620  eam:.        if 
+0000b580: 696e 7428 7472 2e73 7461 7473 2e73 616d  int(tr.stats.sam
+0000b590: 706c 696e 675f 7261 7465 2920 213d 2066  pling_rate) != f
+0000b5a0: 7265 713a 0a20 2020 2020 2020 2020 2020  req:.           
+0000b5b0: 2073 7472 6561 6d2e 7265 6d6f 7665 2874   stream.remove(t
+0000b5c0: 7229 0a20 2020 2020 2020 2069 6620 7472  r).        if tr
+0000b5d0: 2e73 7461 7473 2e6e 7074 7320 3c20 3130  .stats.npts < 10
+0000b5e0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+0000b5f0: 7265 616d 2e72 656d 6f76 6528 7472 290a  ream.remove(tr).
+0000b600: 0a20 2020 2072 6574 7572 6e20 7374 7265  .    return stre
+0000b610: 616d 0a0a 0a64 6566 2070 6f72 7469 6f6e  am...def portion
+0000b620: 5f67 6170 7328 7374 7265 616d 2c20 7374  _gaps(stream, st
+0000b630: 6172 7474 696d 653a 206f 6273 7079 2e55  arttime: obspy.U
+0000b640: 5443 4461 7465 5469 6d65 2c20 656e 6474  TCDateTime, endt
+0000b650: 696d 653a 206f 6273 7079 2e55 5443 4461  ime: obspy.UTCDa
+0000b660: 7465 5469 6d65 293a 0a20 2020 2022 2222  teTime):.    """
+0000b670: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+0000b680: 6f6e 2074 7261 636b 7320 7468 6520 6761  on tracks the ga
+0000b690: 7073 2028 6e70 7473 2920 6672 6f6d 2074  ps (npts) from t
+0000b6a0: 6865 2061 6363 756d 756c 6174 6564 2064  he accumulated d
+0000b6b0: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
+0000b6c0: 6e20 7374 6172 7474 696d 6520 616e 6420  n starttime and 
+0000b6d0: 656e 6474 696d 650a 2020 2020 6f66 2065  endtime.    of e
+0000b6e0: 6163 6820 7374 7265 616d 2074 7261 6365  ach stream trace
+0000b6f0: 2e20 6974 2072 656d 6f76 6573 2074 7261  . it removes tra
+0000b700: 6365 2077 6974 6820 6761 7020 6c65 6e67  ce with gap leng
+0000b710: 7468 203e 2033 3025 206f 6620 7472 6163  th > 30% of trac
+0000b720: 6520 7369 7a65 2e0a 2020 2020 5041 5241  e size..    PARA
+0000b730: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+0000b740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0000b750: 2020 2020 7374 7265 616d 3a20 6f62 7370      stream: obsp
+0000b760: 7920 7374 7265 616d 206f 626a 6563 740a  y stream object.
+0000b770: 2020 2020 6461 7465 5f69 6e66 6f3a 2064      date_info: d
+0000b780: 6963 7420 6f66 2073 7461 7274 696e 6720  ict of starting 
+0000b790: 616e 6420 656e 6469 6e67 2074 696d 6520  and ending time 
+0000b7a0: 6f66 2074 6865 2073 7472 6561 6d0a 0a20  of the stream.. 
+0000b7b0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+0000b7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b7d0: 2d0a 2020 2020 7067 6170 733a 2070 726f  -.    pgaps: pro
+0000b7e0: 706f 7274 696f 6e20 6f66 2067 6170 732f  portion of gaps/
+0000b7f0: 616c 6c5f 7074 7320 696e 2073 7472 6561  all_pts in strea
+0000b800: 6d0a 2020 2020 2222 220a 2020 2020 2320  m.    """.    # 
+0000b810: 6964 6561 6c20 6475 7261 7469 6f6e 206f  ideal duration o
+0000b820: 6620 6461 7461 0a20 2020 206e 7074 7320  f data.    npts 
+0000b830: 3d20 2865 6e64 7469 6d65 202d 2073 7461  = (endtime - sta
+0000b840: 7274 7469 6d65 2920 2a20 7374 7265 616d  rttime) * stream
+0000b850: 5b30 5d2e 7374 6174 732e 7361 6d70 6c69  [0].stats.sampli
+0000b860: 6e67 5f72 6174 650a 0a20 2020 2070 6761  ng_rate..    pga
+0000b870: 7073 203d 2030 0a20 2020 2023 206c 6f6f  ps = 0.    # loo
+0000b880: 7020 7468 726f 7567 6820 616c 6c20 7472  p through all tr
+0000b890: 6163 6520 746f 2061 6363 756d 756c 6174  ace to accumulat
+0000b8a0: 6520 6761 7073 0a20 2020 2066 6f72 2069  e gaps.    for i
+0000b8b0: 6920 696e 2072 616e 6765 286c 656e 2873  i in range(len(s
+0000b8c0: 7472 6561 6d29 202d 2031 293a 0a20 2020  tream) - 1):.   
+0000b8d0: 2020 2020 2070 6761 7073 202b 3d20 2873       pgaps += (s
+0000b8e0: 7472 6561 6d5b 6969 202b 2031 5d2e 7374  tream[ii + 1].st
+0000b8f0: 6174 732e 7374 6172 7474 696d 6520 2d20  ats.starttime - 
+0000b900: 7374 7265 616d 5b69 695d 2e73 7461 7473  stream[ii].stats
+0000b910: 2e65 6e64 7469 6d65 2920 2a20 7374 7265  .endtime) * stre
+0000b920: 616d 5b69 695d 2e73 7461 7473 2e73 616d  am[ii].stats.sam
+0000b930: 706c 696e 675f 7261 7465 0a20 2020 2069  pling_rate.    i
+0000b940: 6620 6e70 7473 2021 3d20 303a 0a20 2020  f npts != 0:.   
+0000b950: 2020 2020 2070 6761 7073 203d 2070 6761       pgaps = pga
+0000b960: 7073 202f 206e 7074 730a 2020 2020 6966  ps / npts.    if
+0000b970: 206e 7074 7320 3d3d 2030 3a0a 2020 2020   npts == 0:.    
+0000b980: 2020 2020 7067 6170 7320 3d20 310a 2020      pgaps = 1.  
+0000b990: 2020 7265 7475 726e 2070 6761 7073 0a0a    return pgaps..
+0000b9a0: 0a40 6a69 7428 2266 6c6f 6174 3332 5b3a  .@jit("float32[:
+0000b9b0: 5d28 666c 6f61 7433 325b 3a5d 2c66 6c6f  ](float32[:],flo
+0000b9c0: 6174 3332 2922 290a 6465 6620 7365 676d  at32)").def segm
+0000b9d0: 656e 745f 696e 7465 7270 6f6c 6174 6528  ent_interpolate(
+0000b9e0: 7369 6731 2c20 6e66 7269 6329 3a0a 2020  sig1, nfric):.  
+0000b9f0: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
+0000ba00: 756e 6374 696f 6e20 696e 7465 7270 6f6c  unction interpol
+0000ba10: 6174 6573 2074 6865 2064 6174 6120 746f  ates the data to
+0000ba20: 2065 6e73 7572 6520 616c 6c20 706f 696e   ensure all poin
+0000ba30: 7473 206c 6f63 6174 6564 206f 6e20 696e  ts located on in
+0000ba40: 7465 7267 6572 2074 696d 6573 206f 6620  terger times of 
+0000ba50: 7468 650a 2020 2020 7361 6d70 6c69 6e67  the.    sampling
+0000ba60: 2072 6174 6520 2865 2e67 2e2c 2073 7461   rate (e.g., sta
+0000ba70: 7274 7469 6d65 203d 2030 303a 3030 3a30  rttime = 00:00:0
+0000ba80: 302e 3031 352c 2064 656c 7461 203d 2030  0.015, delta = 0
+0000ba90: 2e30 352e 290a 2020 2020 5041 5241 4d45  .05.).    PARAME
+0000baa0: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+0000bab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bac0: 0a20 2020 2073 6967 313a 2020 7365 6973  .    sig1:  seis
+0000bad0: 6d69 6320 7265 636f 7264 696e 6773 2069  mic recordings i
+0000bae0: 6e20 6120 3144 2061 7272 6179 0a20 2020  n a 1D array.   
+0000baf0: 206e 6672 6963 3a20 7468 6520 616d 6f75   nfric: the amou
+0000bb00: 6e74 206f 6620 7469 6d65 2064 6966 6665  nt of time diffe
+0000bb10: 7265 6e63 6520 6265 7477 6565 6e20 7468  rence between th
+0000bb20: 6520 706f 696e 7420 616e 6420 7468 6520  e point and the 
+0000bb30: 6164 6a61 6365 6e74 2061 7373 756d 6564  adjacent assumed
+0000bb40: 2073 616d 706c 6573 0a20 2020 2052 4554   samples.    RET
+0000bb50: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
+0000bb60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bb70: 0a20 2020 2073 6967 323a 2020 696e 7465  .    sig2:  inte
+0000bb80: 7270 6f6c 6174 6564 2073 6569 736d 6963  rpolated seismic
+0000bb90: 2072 6563 6f72 6469 6e67 7320 6f6e 2074   recordings on t
+0000bba0: 6865 2073 616d 706c 696e 6720 706f 696e  he sampling poin
+0000bbb0: 7473 0a20 2020 2022 2222 0a20 2020 206e  ts.    """.    n
+0000bbc0: 7074 7320 3d20 6c65 6e28 7369 6731 290a  pts = len(sig1).
+0000bbd0: 2020 2020 7369 6732 203d 206e 702e 7a65      sig2 = np.ze
+0000bbe0: 726f 7328 6e70 7473 2c20 6474 7970 653d  ros(npts, dtype=
+0000bbf0: 6e70 2e66 6c6f 6174 3332 290a 0a20 2020  np.float32)..   
+0000bc00: 2023 202d 2d2d 2d69 6e73 7465 6164 206f   # ----instead o
+0000bc10: 6620 7368 6966 7469 6e67 2c20 646f 2061  f shifting, do a
+0000bc20: 2069 6e74 6572 706f 6c61 7469 6f6e 2d2d   interpolation--
+0000bc30: 2d2d 2d2d 0a20 2020 2066 6f72 2069 6920  ----.    for ii 
+0000bc40: 696e 2072 616e 6765 286e 7074 7329 3a0a  in range(npts):.
+0000bc50: 2020 2020 2020 2020 2320 2d2d 2d2d 6465          # ----de
+0000bc60: 616c 2077 6974 6820 6564 6765 732d 2d2d  al with edges---
+0000bc70: 2d2d 0a20 2020 2020 2020 2069 6620 6969  --.        if ii
+0000bc80: 203d 3d20 3020 6f72 2069 6920 3d3d 206e   == 0 or ii == n
+0000bc90: 7074 7320 2d20 313a 0a20 2020 2020 2020  pts - 1:.       
+0000bca0: 2020 2020 2073 6967 325b 6969 5d20 3d20       sig2[ii] = 
+0000bcb0: 7369 6731 5b69 695d 0a20 2020 2020 2020  sig1[ii].       
+0000bcc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000bcd0: 2020 2023 202d 2d2d 2d2d 2d69 6e74 6572     # ------inter
+0000bce0: 706f 6c61 7465 2075 7369 6e67 2061 2068  polate using a h
+0000bcf0: 6174 2066 756e 6374 696f 6e2d 2d2d 2d2d  at function-----
+0000bd00: 2d0a 2020 2020 2020 2020 2020 2020 7369  -.            si
+0000bd10: 6732 5b69 695d 203d 2028 3120 2d20 6e66  g2[ii] = (1 - nf
+0000bd20: 7269 6329 202a 2073 6967 315b 6969 202b  ric) * sig1[ii +
+0000bd30: 2031 5d20 2b20 6e66 7269 6320 2a20 7369   1] + nfric * si
+0000bd40: 6731 5b69 695d 0a0a 2020 2020 7265 7475  g1[ii]..    retu
+0000bd50: 726e 2073 6967 320a 0a0a 6465 6620 7265  rn sig2...def re
+0000bd60: 7370 5f73 7065 6374 7275 6d28 736f 7572  sp_spectrum(sour
+0000bd70: 6365 2c20 7265 7370 5f66 696c 652c 2064  ce, resp_file, d
+0000bd80: 6f77 6e73 616d 705f 6672 6571 2c20 7072  ownsamp_freq, pr
+0000bd90: 655f 6669 6c74 3d4e 6f6e 6529 3a0a 2020  e_filt=None):.  
+0000bda0: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
+0000bdb0: 756e 6374 696f 6e20 7265 6d6f 7665 7320  unction removes 
+0000bdc0: 7468 6520 696e 7374 7275 6d65 6e74 2072  the instrument r
+0000bdd0: 6573 706f 6e73 6520 7573 696e 6720 7265  esponse using re
+0000bde0: 7370 6f6e 7365 2073 7065 6374 7275 6d20  sponse spectrum 
+0000bdf0: 6672 6f6d 2065 7661 6c72 6573 702e 0a20  from evalresp.. 
+0000be00: 2020 2074 6865 2072 6573 706f 6e73 6520     the response 
+0000be10: 7370 6563 7472 756d 2069 7320 6576 616c  spectrum is eval
+0000be20: 7561 7465 6420 6261 7365 6420 6f6e 2052  uated based on R
+0000be30: 4553 502f 505a 2066 696c 6573 2062 6566  ESP/PZ files bef
+0000be40: 6f72 6520 696e 7665 7274 6564 2075 7369  ore inverted usi
+0000be50: 6e67 2074 6865 206f 6273 7079 0a20 2020  ng the obspy.   
+0000be60: 2066 756e 6374 696f 6e20 6f66 2069 6e76   function of inv
+0000be70: 6572 745f 7370 6563 7472 756d 2e20 6120  ert_spectrum. a 
+0000be80: 6d6f 6475 6c65 206f 6620 6372 6561 7465  module of create
+0000be90: 5f72 6573 702e 7079 2069 7320 7072 6f76  _resp.py is prov
+0000bea0: 6964 6564 2069 6e20 6469 7265 6374 6f72  ided in director
+0000beb0: 7920 6f66 2027 6164 6469 7469 6f6e 616c  y of 'additional
+0000bec0: 5f6d 6f64 756c 6573 270a 2020 2020 746f  _modules'.    to
+0000bed0: 2063 7265 6174 6520 7468 6520 7265 7370   create the resp
+0000bee0: 6f6e 7365 2073 7065 6374 7275 6d0a 2020  onse spectrum.  
+0000bef0: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+0000bf00: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000bf10: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 6f75  --------.    sou
+0000bf20: 7263 653a 206f 6273 7079 2073 7472 6561  rce: obspy strea
+0000bf30: 6d20 6f62 6a65 6374 206f 6620 7461 7267  m object of targ
+0000bf40: 6574 6564 206e 6f69 7365 2064 6174 610a  eted noise data.
+0000bf50: 2020 2020 7265 7370 5f66 696c 653a 206e      resp_file: n
+0000bf60: 756d 7079 2064 6174 6120 6669 6c65 206f  umpy data file o
+0000bf70: 6620 7265 7370 6f6e 7365 2073 7065 6374  f response spect
+0000bf80: 7275 6d0a 2020 2020 646f 776e 7361 6d70  rum.    downsamp
+0000bf90: 5f66 7265 713a 2073 616d 706c 696e 6720  _freq: sampling 
+0000bfa0: 7261 7465 206f 6620 7468 6520 736f 7572  rate of the sour
+0000bfb0: 6365 2064 6174 610a 2020 2020 7072 655f  ce data.    pre_
+0000bfc0: 6669 6c74 3a20 7072 652d 6465 6669 6e65  filt: pre-define
+0000bfd0: 6420 6669 6c74 6572 2070 6172 616d 6574  d filter paramet
+0000bfe0: 6572 730a 2020 2020 5245 5455 524e 533a  ers.    RETURNS:
+0000bff0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000c000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000c010: 736f 7572 6365 3a20 6f62 7370 7920 7374  source: obspy st
+0000c020: 7265 616d 206f 626a 6563 7420 6f66 206e  ream object of n
+0000c030: 6f69 7365 2064 6174 6120 7769 7468 2069  oise data with i
+0000c040: 6e73 7472 756d 656e 7420 7265 7370 6f6e  nstrument respon
+0000c050: 7365 2072 656d 6f76 6564 0a20 2020 2022  se removed.    "
+0000c060: 2222 0a20 2020 2023 202d 2d2d 2d2d 2d2d  "".    # -------
+0000c070: 2d72 6573 705f 6669 6c65 2069 7320 7468  -resp_file is th
+0000c080: 6520 696e 7665 7274 6564 2073 7065 6374  e inverted spect
+0000c090: 7275 6d20 7265 7370 6f6e 7365 2d2d 2d2d  rum response----
+0000c0a0: 2d2d 2d2d 2d0a 2020 2020 7265 7370 7a20  -----.    respz 
+0000c0b0: 3d20 6e70 2e6c 6f61 6428 7265 7370 5f66  = np.load(resp_f
+0000c0c0: 696c 6529 0a20 2020 206e 7265 7370 7a20  ile).    nrespz 
+0000c0d0: 3d20 7265 7370 7a5b 315d 5b3a 5d0a 2020  = respz[1][:].  
+0000c0e0: 2020 7370 6563 5f66 7265 7120 3d20 6d61    spec_freq = ma
+0000c0f0: 7828 7265 7370 7a5b 305d 290a 0a20 2020  x(respz[0])..   
+0000c100: 2023 202d 2d2d 2d2d 2d2d 6f6e 2063 7572   # -------on cur
+0000c110: 7265 6e74 2074 7261 6365 2d2d 2d2d 2d2d  rent trace------
+0000c120: 2d2d 2d2d 0a20 2020 206e 6666 7420 3d20  ----.    nfft = 
+0000c130: 5f6e 7074 7332 6e66 6674 2873 6f75 7263  _npts2nfft(sourc
+0000c140: 655b 305d 2e73 7461 7473 2e6e 7074 7329  e[0].stats.npts)
+0000c150: 0a20 2020 2073 7073 203d 2069 6e74 2873  .    sps = int(s
+0000c160: 6f75 7263 655b 305d 2e73 7461 7473 2e73  ource[0].stats.s
+0000c170: 616d 706c 696e 675f 7261 7465 290a 0a20  ampling_rate).. 
+0000c180: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 646f     # ---------do
+0000c190: 2074 6865 2069 6e74 6572 706f 6c61 7469   the interpolati
+0000c1a0: 6f6e 2069 6620 6e65 6564 6564 2d2d 2d2d  on if needed----
+0000c1b0: 2d2d 2d2d 0a20 2020 2069 6620 7370 6563  ----.    if spec
+0000c1c0: 5f66 7265 7120 3c20 302e 3520 2a20 7370  _freq < 0.5 * sp
+0000c1d0: 733a 0a20 2020 2020 2020 2072 6169 7365  s:.        raise
+0000c1e0: 2056 616c 7565 4572 726f 7228 2273 7065   ValueError("spe
+0000c1f0: 6374 7275 6d20 6669 6c65 2068 6173 2070  ctrum file has p
+0000c200: 6561 6b20 6672 6571 2073 6d61 6c6c 6572  eak freq smaller
+0000c210: 2074 6861 6e20 7468 6520 6461 7461 2c20   than the data, 
+0000c220: 6162 6f72 7421 2229 0a20 2020 2065 6c73  abort!").    els
+0000c230: 653a 0a20 2020 2020 2020 2069 6e64 7820  e:.        indx 
+0000c240: 3d20 6e70 2e77 6865 7265 2872 6573 707a  = np.where(respz
+0000c250: 5b30 5d20 3c3d 2030 2e35 202a 2073 7073  [0] <= 0.5 * sps
+0000c260: 290a 2020 2020 2020 2020 6e66 7265 7120  ).        nfreq 
+0000c270: 3d20 6e70 2e6c 696e 7370 6163 6528 302c  = np.linspace(0,
+0000c280: 2030 2e35 202a 2073 7073 2c20 6e66 6674   0.5 * sps, nfft
+0000c290: 202f 2f20 3220 2b20 3129 0a20 2020 2020   // 2 + 1).     
+0000c2a0: 2020 206e 7265 7370 7a20 3d20 6e70 2e69     nrespz = np.i
+0000c2b0: 6e74 6572 7028 6e66 7265 712c 206e 702e  nterp(nfreq, np.
+0000c2c0: 7265 616c 2872 6573 707a 5b30 5d5b 696e  real(respz[0][in
+0000c2d0: 6478 5d29 2c20 7265 7370 7a5b 315d 5b69  dx]), respz[1][i
+0000c2e0: 6e64 785d 290a 0a20 2020 2023 202d 2d2d  ndx])..    # ---
+0000c2f0: 2d64 6f20 696e 7465 7270 6f6c 6174 696f  -do interpolatio
+0000c300: 6e20 6966 206e 6563 6573 7361 7279 2d2d  n if necessary--
+0000c310: 2d2d 2d0a 2020 2020 736f 7572 6365 5f73  ---.    source_s
+0000c320: 7065 6374 203d 206e 702e 6666 742e 7266  pect = np.fft.rf
+0000c330: 6674 2873 6f75 7263 655b 305d 2e64 6174  ft(source[0].dat
+0000c340: 612c 206e 3d6e 6666 7429 0a0a 2020 2020  a, n=nfft)..    
+0000c350: 2320 2d2d 2d2d 2d6e 7265 7370 7a20 6973  # -----nrespz is
+0000c360: 2069 6e76 6572 7365 6420 2877 6174 6572   inversed (water
+0000c370: 2d6c 6576 656c 6564 2920 7370 6563 7472  -leveled) spectr
+0000c380: 756d 2d2d 2d2d 2d0a 2020 2020 736f 7572  um-----.    sour
+0000c390: 6365 5f73 7065 6374 202a 3d20 6e72 6573  ce_spect *= nres
+0000c3a0: 707a 0a20 2020 2073 6f75 7263 655b 305d  pz.    source[0]
+0000c3b0: 2e64 6174 6120 3d20 6e70 2e66 6674 2e69  .data = np.fft.i
+0000c3c0: 7266 6674 2873 6f75 7263 655f 7370 6563  rfft(source_spec
+0000c3d0: 7429 5b30 203a 2073 6f75 7263 655b 305d  t)[0 : source[0]
+0000c3e0: 2e73 7461 7473 2e6e 7074 735d 0a0a 2020  .stats.npts]..  
+0000c3f0: 2020 6966 2070 7265 5f66 696c 7420 6973    if pre_filt is
+0000c400: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000c410: 2020 2073 6f75 7263 655b 305d 2e64 6174     source[0].dat
+0000c420: 6120 3d20 6e70 2e66 6c6f 6174 3332 280a  a = np.float32(.
+0000c430: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+0000c440: 7061 7373 280a 2020 2020 2020 2020 2020  pass(.          
+0000c450: 2020 2020 2020 736f 7572 6365 5b30 5d2e        source[0].
+0000c460: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+0000c470: 2020 2020 2020 7072 655f 6669 6c74 5b30        pre_filt[0
+0000c480: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000c490: 2020 2070 7265 5f66 696c 745b 2d31 5d2c     pre_filt[-1],
+0000c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4b0: 2064 663d 7370 732c 0a20 2020 2020 2020   df=sps,.       
+0000c4c0: 2020 2020 2020 2020 2063 6f72 6e65 7273           corners
+0000c4d0: 3d34 2c0a 2020 2020 2020 2020 2020 2020  =4,.            
+0000c4e0: 2020 2020 7a65 726f 7068 6173 653d 5472      zerophase=Tr
+0000c4f0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000c500: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+0000c510: 2072 6574 7572 6e20 736f 7572 6365 0a0a   return source..
+0000c520: 0a64 6566 206d 6164 2861 7272 293a 0a20  .def mad(arr):. 
+0000c530: 2020 2022 2222 0a20 2020 204d 6564 6961     """.    Media
+0000c540: 6e20 4162 736f 6c75 7465 2044 6576 6961  n Absolute Devia
+0000c550: 7469 6f6e 3a20 4d41 4420 3d20 6d65 6469  tion: MAD = medi
+0000c560: 616e 287c 5869 2d20 6d65 6469 616e 2858  an(|Xi- median(X
+0000c570: 297c 290a 2020 2020 5041 5241 4d45 5445  )|).    PARAMETE
+0000c580: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+0000c590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000c5a0: 6172 723a 206e 756d 7079 2e6e 6461 7272  arr: numpy.ndarr
+0000c5b0: 6179 2c20 7365 6973 6d69 6320 7472 6163  ay, seismic trac
+0000c5c0: 6520 6461 7461 2061 7272 6179 0a20 2020  e data array.   
+0000c5d0: 2052 4554 5552 4e53 3a0a 2020 2020 6461   RETURNS:.    da
+0000c5e0: 7461 3a20 4d65 6469 616e 2041 6273 6f6c  ta: Median Absol
+0000c5f0: 7574 6520 4465 7669 6174 696f 6e20 6f66  ute Deviation of
+0000c600: 2064 6174 610a 2020 2020 2222 220a 2020   data.    """.  
+0000c610: 2020 6966 206e 6f74 206e 702e 6d61 2e69    if not np.ma.i
+0000c620: 735f 6d61 736b 6564 2861 7272 293a 0a20  s_masked(arr):. 
+0000c630: 2020 2020 2020 206d 6564 203d 206e 702e         med = np.
+0000c640: 6d65 6469 616e 2861 7272 290a 2020 2020  median(arr).    
+0000c650: 2020 2020 6461 7461 203d 206e 702e 6d65      data = np.me
+0000c660: 6469 616e 286e 702e 6162 7328 6172 7220  dian(np.abs(arr 
+0000c670: 2d20 6d65 6429 290a 2020 2020 656c 7365  - med)).    else
+0000c680: 3a0a 2020 2020 2020 2020 6d65 6420 3d20  :.        med = 
+0000c690: 6e70 2e6d 612e 6d65 6469 616e 2861 7272  np.ma.median(arr
+0000c6a0: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+0000c6b0: 206e 702e 6d61 2e6d 6564 6961 6e28 6e70   np.ma.median(np
+0000c6c0: 2e6d 612e 6162 7328 6172 7220 2d20 6d65  .ma.abs(arr - me
+0000c6d0: 6429 290a 2020 2020 7265 7475 726e 2064  d)).    return d
+0000c6e0: 6174 610a 0a0a 6465 6620 6465 7472 656e  ata...def detren
+0000c6f0: 6428 6461 7461 293a 0a20 2020 2022 2222  d(data):.    """
+0000c700: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+0000c710: 6f6e 2072 656d 6f76 6573 2074 6865 2073  on removes the s
+0000c720: 6967 6e61 6c20 7472 656e 6420 6261 7365  ignal trend base
+0000c730: 6420 6f6e 2051 5220 6465 636f 6d70 6f73  d on QR decompos
+0000c740: 696f 6e0a 2020 2020 4e4f 5445 3a20 5152  ion.    NOTE: QR
+0000c750: 2069 7320 6120 6c6f 7420 6661 7374 6572   is a lot faster
+0000c760: 2074 6861 6e20 7468 6520 6c65 6173 7420   than the least 
+0000c770: 7371 7561 7265 2069 6e76 6572 7369 6f6e  square inversion
+0000c780: 2075 7365 6420 6279 0a20 2020 2073 6369   used by.    sci
+0000c790: 7079 2028 616c 736f 2069 6e20 6f62 7370  py (also in obsp
+0000c7a0: 7929 2e0a 2020 2020 5041 5241 4d45 5445  y)..    PARAMETE
+0000c7b0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+0000c7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000c7d0: 2020 6461 7461 3a20 696e 7075 7420 6461    data: input da
+0000c7e0: 7461 206d 6174 7269 780a 2020 2020 5245  ta matrix.    RE
+0000c7f0: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+0000c800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c810: 0a20 2020 2064 6174 613a 2064 6174 6120  .    data: data 
+0000c820: 6d61 7472 6978 2077 6974 6820 7472 656e  matrix with tren
+0000c830: 6420 7265 6d6f 7665 640a 2020 2020 2222  d removed.    ""
+0000c840: 220a 2020 2020 2320 6e64 6174 6120 3d20  ".    # ndata = 
+0000c850: 6e70 2e7a 6572 6f73 2873 6861 7065 3d64  np.zeros(shape=d
+0000c860: 6174 612e 7368 6170 652c 6474 7970 653d  ata.shape,dtype=
+0000c870: 6461 7461 2e64 7479 7065 290a 2020 2020  data.dtype).    
+0000c880: 6966 2064 6174 612e 6e64 696d 203d 3d20  if data.ndim == 
+0000c890: 313a 0a20 2020 2020 2020 206e 7074 7320  1:.        npts 
+0000c8a0: 3d20 6461 7461 2e73 6861 7065 5b30 5d0a  = data.shape[0].
+0000c8b0: 2020 2020 2020 2020 5820 3d20 6e70 2e6f          X = np.o
+0000c8c0: 6e65 7328 286e 7074 732c 2032 2929 0a20  nes((npts, 2)). 
+0000c8d0: 2020 2020 2020 2058 5b3a 2c20 305d 203d         X[:, 0] =
+0000c8e0: 206e 702e 6172 616e 6765 2830 2c20 6e70   np.arange(0, np
+0000c8f0: 7473 2920 2f20 6e70 7473 0a20 2020 2020  ts) / npts.     
+0000c900: 2020 2051 2c20 5220 3d20 6e70 2e6c 696e     Q, R = np.lin
+0000c910: 616c 672e 7172 2858 290a 2020 2020 2020  alg.qr(X).      
+0000c920: 2020 7271 203d 206e 702e 646f 7428 6e70    rq = np.dot(np
+0000c930: 2e6c 696e 616c 672e 696e 7628 5229 2c20  .linalg.inv(R), 
+0000c940: 512e 7472 616e 7370 6f73 6528 2929 0a20  Q.transpose()). 
+0000c950: 2020 2020 2020 2063 6f65 6666 203d 206e         coeff = n
+0000c960: 702e 646f 7428 7271 2c20 6461 7461 290a  p.dot(rq, data).
+0000c970: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0000c980: 6174 6120 2d20 6e70 2e64 6f74 2858 2c20  ata - np.dot(X, 
+0000c990: 636f 6566 6629 0a20 2020 2065 6c69 6620  coeff).    elif 
+0000c9a0: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
+0000c9b0: 2020 2020 2020 2020 6e70 7473 203d 2064          npts = d
+0000c9c0: 6174 612e 7368 6170 655b 315d 0a20 2020  ata.shape[1].   
+0000c9d0: 2020 2020 2058 203d 206e 702e 6f6e 6573       X = np.ones
+0000c9e0: 2828 6e70 7473 2c20 3229 290a 2020 2020  ((npts, 2)).    
+0000c9f0: 2020 2020 585b 3a2c 2030 5d20 3d20 6e70      X[:, 0] = np
+0000ca00: 2e61 7261 6e67 6528 302c 206e 7074 7329  .arange(0, npts)
+0000ca10: 202f 206e 7074 730a 2020 2020 2020 2020   / npts.        
+0000ca20: 512c 2052 203d 206e 702e 6c69 6e61 6c67  Q, R = np.linalg
+0000ca30: 2e71 7228 5829 0a20 2020 2020 2020 2072  .qr(X).        r
+0000ca40: 7120 3d20 6e70 2e64 6f74 286e 702e 6c69  q = np.dot(np.li
+0000ca50: 6e61 6c67 2e69 6e76 2852 292c 2051 2e74  nalg.inv(R), Q.t
+0000ca60: 7261 6e73 706f 7365 2829 290a 2020 2020  ranspose()).    
+0000ca70: 2020 2020 666f 7220 6969 2069 6e20 7261      for ii in ra
+0000ca80: 6e67 6528 6461 7461 2e73 6861 7065 5b30  nge(data.shape[0
+0000ca90: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+0000caa0: 636f 6566 6620 3d20 6e70 2e64 6f74 2872  coeff = np.dot(r
+0000cab0: 712c 2064 6174 615b 6969 5d29 0a20 2020  q, data[ii]).   
+0000cac0: 2020 2020 2020 2020 2064 6174 615b 6969           data[ii
+0000cad0: 5d20 3d20 6461 7461 5b69 695d 202d 206e  ] = data[ii] - n
+0000cae0: 702e 646f 7428 582c 2063 6f65 6666 290a  p.dot(X, coeff).
+0000caf0: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
+0000cb00: 0a0a 6465 6620 6465 6d65 616e 2864 6174  ..def demean(dat
+0000cb10: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
+0000cb20: 7468 6973 2066 756e 6374 696f 6e20 7265  this function re
+0000cb30: 6d6f 7665 2074 6865 206d 6561 6e20 6f66  move the mean of
+0000cb40: 2074 6865 2073 6967 6e61 6c0a 2020 2020   the signal.    
+0000cb50: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+0000cb60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cb70: 2d2d 2d2d 2d0a 2020 2020 6461 7461 3a20  -----.    data: 
+0000cb80: 696e 7075 7420 6461 7461 206d 6174 7269  input data matri
+0000cb90: 780a 2020 2020 5245 5455 524e 533a 0a20  x.    RETURNS:. 
+0000cba0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000cbb0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
+0000cbc0: 613a 2064 6174 6120 6d61 7472 6978 2077  a: data matrix w
+0000cbd0: 6974 6820 6d65 616e 2072 656d 6f76 6564  ith mean removed
+0000cbe0: 0a20 2020 2022 2222 0a20 2020 2023 206e  .    """.    # n
+0000cbf0: 6461 7461 203d 206e 702e 7a65 726f 7328  data = np.zeros(
+0000cc00: 7368 6170 653d 6461 7461 2e73 6861 7065  shape=data.shape
+0000cc10: 2c64 7479 7065 3d64 6174 612e 6474 7970  ,dtype=data.dtyp
+0000cc20: 6529 0a20 2020 2069 6620 6461 7461 2e6e  e).    if data.n
+0000cc30: 6469 6d20 3d3d 2031 3a0a 2020 2020 2020  dim == 1:.      
+0000cc40: 2020 6461 7461 203d 2064 6174 6120 2d20    data = data - 
+0000cc50: 6e70 2e6d 6561 6e28 6461 7461 290a 2020  np.mean(data).  
+0000cc60: 2020 656c 6966 2064 6174 612e 6e64 696d    elif data.ndim
+0000cc70: 203d 3d20 323a 0a20 2020 2020 2020 2066   == 2:.        f
+0000cc80: 6f72 2069 6920 696e 2072 616e 6765 2864  or ii in range(d
+0000cc90: 6174 612e 7368 6170 655b 305d 293a 0a20  ata.shape[0]):. 
+0000cca0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0000ccb0: 6969 5d20 3d20 6461 7461 5b69 695d 202d  ii] = data[ii] -
+0000ccc0: 206e 702e 6d65 616e 2864 6174 615b 6969   np.mean(data[ii
+0000ccd0: 5d29 0a20 2020 2072 6574 7572 6e20 6461  ]).    return da
+0000cce0: 7461 0a0a 0a64 6566 2074 6170 6572 2864  ta...def taper(d
+0000ccf0: 6174 6129 3a0a 2020 2020 2222 220a 2020  ata):.    """.  
+0000cd00: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+0000cd10: 6170 706c 6965 7320 6120 636f 7369 6e65  applies a cosine
+0000cd20: 2074 6170 6572 2075 7369 6e67 206f 6273   taper using obs
+0000cd30: 7079 2066 756e 6374 696f 6e73 0a20 2020  py functions.   
+0000cd40: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
+0000cd50: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000cd60: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 613a  ------.    data:
+0000cd70: 2069 6e70 7574 2064 6174 6120 6d61 7472   input data matr
+0000cd80: 6978 0a20 2020 2052 4554 5552 4e53 3a0a  ix.    RETURNS:.
+0000cd90: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000cda0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6461  ---------.    da
+0000cdb0: 7461 3a20 6461 7461 206d 6174 7269 7820  ta: data matrix 
+0000cdc0: 7769 7468 2074 6170 6572 2061 7070 6c69  with taper appli
+0000cdd0: 6564 0a20 2020 2022 2222 0a20 2020 2023  ed.    """.    #
+0000cde0: 206e 6461 7461 203d 206e 702e 7a65 726f   ndata = np.zero
+0000cdf0: 7328 7368 6170 653d 6461 7461 2e73 6861  s(shape=data.sha
+0000ce00: 7065 2c64 7479 7065 3d64 6174 612e 6474  pe,dtype=data.dt
+0000ce10: 7970 6529 0a20 2020 2069 6620 6461 7461  ype).    if data
+0000ce20: 2e6e 6469 6d20 3d3d 2031 3a0a 2020 2020  .ndim == 1:.    
+0000ce30: 2020 2020 6e70 7473 203d 2064 6174 612e      npts = data.
+0000ce40: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
+0000ce50: 2023 2077 696e 646f 7720 6c65 6e67 7468   # window length
+0000ce60: 0a20 2020 2020 2020 2069 6620 6e70 7473  .        if npts
+0000ce70: 202a 2030 2e30 3520 3e20 3230 3a0a 2020   * 0.05 > 20:.  
+0000ce80: 2020 2020 2020 2020 2020 776c 656e 203d            wlen =
+0000ce90: 2032 300a 2020 2020 2020 2020 656c 7365   20.        else
+0000cea0: 3a0a 2020 2020 2020 2020 2020 2020 776c  :.            wl
+0000ceb0: 656e 203d 206e 7074 7320 2a20 302e 3035  en = npts * 0.05
+0000cec0: 0a20 2020 2020 2020 2023 2074 6170 6572  .        # taper
+0000ced0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+0000cee0: 6675 6e63 203d 205f 6765 745f 6675 6e63  func = _get_func
+0000cef0: 7469 6f6e 5f66 726f 6d5f 656e 7472 795f  tion_from_entry_
+0000cf00: 706f 696e 7428 2274 6170 6572 222c 2022  point("taper", "
+0000cf10: 6861 6e6e 2229 0a20 2020 2020 2020 2069  hann").        i
+0000cf20: 6620 3220 2a20 776c 656e 203d 3d20 6e70  f 2 * wlen == np
+0000cf30: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0000cf40: 7461 7065 725f 7369 6465 7320 3d20 6675  taper_sides = fu
+0000cf50: 6e63 2832 202a 2077 6c65 6e29 0a20 2020  nc(2 * wlen).   
+0000cf60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000cf70: 2020 2020 2020 2074 6170 6572 5f73 6964         taper_sid
+0000cf80: 6573 203d 2066 756e 6328 3220 2a20 776c  es = func(2 * wl
+0000cf90: 656e 202b 2031 290a 2020 2020 2020 2020  en + 1).        
+0000cfa0: 2320 7461 7065 7220 7769 6e64 6f77 0a20  # taper window. 
+0000cfb0: 2020 2020 2020 2077 696e 203d 206e 702e         win = np.
+0000cfc0: 6873 7461 636b 280a 2020 2020 2020 2020  hstack(.        
+0000cfd0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+0000cfe0: 2020 2020 2020 7461 7065 725f 7369 6465        taper_side
+0000cff0: 735b 3a77 6c65 6e5d 2c0a 2020 2020 2020  s[:wlen],.      
+0000d000: 2020 2020 2020 2020 2020 6e70 2e6f 6e65            np.one
+0000d010: 7328 6e70 7473 202d 2032 202a 2077 6c65  s(npts - 2 * wle
+0000d020: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
+0000d030: 2020 2020 7461 7065 725f 7369 6465 735b      taper_sides[
+0000d040: 6c65 6e28 7461 7065 725f 7369 6465 7329  len(taper_sides)
+0000d050: 202d 2077 6c65 6e20 3a5d 2c0a 2020 2020   - wlen :],.    
+0000d060: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d070: 2020 290a 2020 2020 2020 2020 6461 7461    ).        data
+0000d080: 202a 3d20 7769 6e0a 2020 2020 656c 6966   *= win.    elif
+0000d090: 2064 6174 612e 6e64 696d 203d 3d20 323a   data.ndim == 2:
+0000d0a0: 0a20 2020 2020 2020 206e 7074 7320 3d20  .        npts = 
+0000d0b0: 6461 7461 2e73 6861 7065 5b31 5d0a 2020  data.shape[1].  
+0000d0c0: 2020 2020 2020 2320 7769 6e64 6f77 206c        # window l
+0000d0d0: 656e 6774 680a 2020 2020 2020 2020 6966  ength.        if
+0000d0e0: 206e 7074 7320 2a20 302e 3035 203e 2032   npts * 0.05 > 2
+0000d0f0: 303a 0a20 2020 2020 2020 2020 2020 2077  0:.            w
+0000d100: 6c65 6e20 3d20 3230 0a20 2020 2020 2020  len = 20.       
+0000d110: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d120: 2020 2077 6c65 6e20 3d20 6e70 7473 202a     wlen = npts *
+0000d130: 2030 2e30 350a 2020 2020 2020 2020 2320   0.05.        # 
+0000d140: 7461 7065 7220 7661 6c75 6573 0a20 2020  taper values.   
+0000d150: 2020 2020 2066 756e 6320 3d20 5f67 6574       func = _get
+0000d160: 5f66 756e 6374 696f 6e5f 6672 6f6d 5f65  _function_from_e
+0000d170: 6e74 7279 5f70 6f69 6e74 2822 7461 7065  ntry_point("tape
+0000d180: 7222 2c20 2268 616e 6e22 290a 2020 2020  r", "hann").    
+0000d190: 2020 2020 6966 2032 202a 2077 6c65 6e20      if 2 * wlen 
+0000d1a0: 3d3d 206e 7074 733a 0a20 2020 2020 2020  == npts:.       
+0000d1b0: 2020 2020 2074 6170 6572 5f73 6964 6573       taper_sides
+0000d1c0: 203d 2066 756e 6328 3220 2a20 776c 656e   = func(2 * wlen
+0000d1d0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000d1e0: 2020 2020 2020 2020 2020 2020 7461 7065              tape
+0000d1f0: 725f 7369 6465 7320 3d20 6675 6e63 2832  r_sides = func(2
+0000d200: 202a 2077 6c65 6e20 2b20 3129 0a20 2020   * wlen + 1).   
+0000d210: 2020 2020 2023 2074 6170 6572 2077 696e       # taper win
+0000d220: 646f 770a 2020 2020 2020 2020 7769 6e20  dow.        win 
+0000d230: 3d20 6e70 2e68 7374 6163 6b28 0a20 2020  = np.hstack(.   
+0000d240: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+0000d250: 2020 2020 2020 2020 2020 2074 6170 6572             taper
+0000d260: 5f73 6964 6573 5b3a 776c 656e 5d2c 0a20  _sides[:wlen],. 
+0000d270: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000d280: 702e 6f6e 6573 286e 7074 7320 2d20 3220  p.ones(npts - 2 
+0000d290: 2a20 776c 656e 292c 0a20 2020 2020 2020  * wlen),.       
+0000d2a0: 2020 2020 2020 2020 2074 6170 6572 5f73           taper_s
+0000d2b0: 6964 6573 5b6c 656e 2874 6170 6572 5f73  ides[len(taper_s
+0000d2c0: 6964 6573 2920 2d20 776c 656e 203a 5d2c  ides) - wlen :],
+0000d2d0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d2e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d2f0: 2066 6f72 2069 6920 696e 2072 616e 6765   for ii in range
+0000d300: 2864 6174 612e 7368 6170 655b 305d 293a  (data.shape[0]):
+0000d310: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000d320: 615b 6969 5d20 2a3d 2077 696e 0a20 2020  a[ii] *= win.   
+0000d330: 2072 6574 7572 6e20 6461 7461 0a0a 0a23   return data...#
+0000d340: 2040 6a69 7428 6e6f 7079 7468 6f6e 203d   @jit(nopython =
+0000d350: 2054 7275 6529 0a0a 0a23 2063 6861 6e67   True)...# chang
+0000d360: 6520 7468 6520 6d6f 7669 6e67 2061 7665  e the moving ave
+0000d370: 7261 6765 2063 616c 6375 6c61 7469 6f6e  rage calculation
+0000d380: 2074 6f20 7461 6b65 2061 7320 696e 7075   to take as inpu
+0000d390: 7420 4e20 7468 6520 6675 6c6c 2077 696e  t N the full win
+0000d3a0: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
+0000d3b0: 6f6f 7468 0a64 6566 206d 6f76 696e 675f  ooth.def moving_
+0000d3c0: 6176 6528 412c 204e 293a 0a20 2020 2022  ave(A, N):.    "
+0000d3d0: 2222 0a20 2020 2041 6c74 6572 6e61 7469  "".    Alternati
+0000d3e0: 7665 2066 756e 6374 696f 6e20 666f 7220  ve function for 
+0000d3f0: 6d6f 7669 6e67 2061 7665 7261 6765 2066  moving average f
+0000d400: 6f72 2061 6e20 6172 7261 792e 0a20 2020  or an array..   
+0000d410: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
+0000d420: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000d430: 2d2d 2d2d 2d2d 0a20 2020 2041 3a20 312d  ------.    A: 1-
+0000d440: 4420 6172 7261 7920 6f66 2064 6174 6120  D array of data 
+0000d450: 746f 2062 6520 736d 6f6f 7468 6564 0a20  to be smoothed. 
+0000d460: 2020 204e 3a20 696e 7465 6765 722c 2069     N: integer, i
+0000d470: 7420 6465 6669 6e65 7320 7468 6520 6675  t defines the fu
+0000d480: 6c6c 2121 2077 696e 646f 7720 6c65 6e67  ll!! window leng
+0000d490: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
+0000d4a0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000d4b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d4c0: 2d2d 2d0a 2020 2020 423a 2031 2d44 2061  ---.    B: 1-D a
+0000d4d0: 7272 6179 2077 6974 6820 736d 6f6f 7468  rray with smooth
+0000d4e0: 6564 2064 6174 610a 2020 2020 2222 220a  ed data.    """.
+0000d4f0: 2020 2020 2320 6465 6669 6e65 7320 616e      # defines an
+0000d500: 2061 7272 6179 2077 6974 6820 4e20 6578   array with N ex
+0000d510: 7472 6120 7361 6d70 6c65 7320 6174 2065  tra samples at e
+0000d520: 6974 6865 7220 7369 6465 0a20 2020 2074  ither side.    t
+0000d530: 656d 7020 3d20 6e70 2e7a 6572 6f73 286c  emp = np.zeros(l
+0000d540: 656e 2841 2920 2b20 3220 2a20 4e29 0a20  en(A) + 2 * N). 
+0000d550: 2020 2023 2073 6574 2074 6865 2063 656e     # set the cen
+0000d560: 7472 616c 2070 6f72 7469 6f6e 206f 6620  tral portion of 
+0000d570: 7468 6520 6172 7261 7920 746f 2041 0a20  the array to A. 
+0000d580: 2020 2074 656d 705b 4e3a 2d4e 5d20 3d20     temp[N:-N] = 
+0000d590: 410a 2020 2020 2320 6c65 6164 696e 6720  A.    # leading 
+0000d5a0: 7361 6d70 6c65 733a 2065 7175 616c 2074  samples: equal t
+0000d5b0: 6f20 6669 7273 7420 7361 6d70 6c65 206f  o first sample o
+0000d5c0: 6620 6163 7475 616c 2061 7272 6179 0a20  f actual array. 
+0000d5d0: 2020 2074 656d 705b 303a 4e5d 203d 2074     temp[0:N] = t
+0000d5e0: 656d 705b 4e5d 0a20 2020 2023 2074 7261  emp[N].    # tra
+0000d5f0: 696c 696e 6720 7361 6d70 6c65 733a 2045  iling samples: E
+0000d600: 7175 616c 2074 6f20 6c61 7374 2073 616d  qual to last sam
+0000d610: 706c 6520 6f66 2061 6374 7561 6c20 6172  ple of actual ar
+0000d620: 7261 790a 2020 2020 7465 6d70 5b2d 4e3a  ray.    temp[-N:
+0000d630: 5d20 3d20 7465 6d70 5b2d 4e20 2d20 315d  ] = temp[-N - 1]
+0000d640: 0a20 2020 2023 2063 6f6e 766f 6c76 6520  .    # convolve 
+0000d650: 7769 7468 2061 2062 6f78 6361 7220 616e  with a boxcar an
+0000d660: 6420 6e6f 726d 616c 697a 652c 2061 6e64  d normalize, and
+0000d670: 2075 7365 206f 6e6c 7920 6365 6e74 7261   use only centra
+0000d680: 6c20 706f 7274 696f 6e20 6f66 2074 6865  l portion of the
+0000d690: 2072 6573 756c 740a 2020 2020 2320 7769   result.    # wi
+0000d6a0: 7468 206c 656e 6774 6820 6571 7561 6c20  th length equal 
+0000d6b0: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+0000d6c0: 6172 7261 792c 2064 6973 6361 7264 696e  array, discardin
+0000d6d0: 6720 7468 6520 6164 6465 6420 6c65 6164  g the added lead
+0000d6e0: 696e 6720 616e 6420 7472 6169 6c69 6e67  ing and trailing
+0000d6f0: 2073 616d 706c 6573 0a20 2020 2042 203d   samples.    B =
+0000d700: 206e 702e 636f 6e76 6f6c 7665 2874 656d   np.convolve(tem
+0000d710: 702c 206e 702e 6f6e 6573 284e 2920 2f20  p, np.ones(N) / 
+0000d720: 4e2c 206d 6f64 653d 2273 616d 6522 295b  N, mode="same")[
+0000d730: 4e3a 2d4e 5d0a 2020 2020 7265 7475 726e  N:-N].    return
+0000d740: 2042 0a0a 0a23 2063 6861 6e67 6520 7468   B...# change th
+0000d750: 6520 6d6f 7669 6e67 2061 7665 7261 6765  e moving average
+0000d760: 2063 616c 6375 6c61 7469 6f6e 2074 6f20   calculation to 
+0000d770: 7461 6b65 2061 7320 696e 7075 7420 4e20  take as input N 
+0000d780: 7468 6520 6675 6c6c 2077 696e 646f 7720  the full window 
+0000d790: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
+0000d7a0: 0a64 6566 206d 6f76 696e 675f 6176 655f  .def moving_ave_
+0000d7b0: 3244 2841 2c20 4e29 3a0a 2020 2020 2222  2D(A, N):.    ""
+0000d7c0: 220a 2020 2020 416c 7465 726e 6174 6976  ".    Alternativ
+0000d7d0: 6520 6675 6e63 7469 6f6e 2066 6f72 206d  e function for m
+0000d7e0: 6f76 696e 6720 6176 6572 6167 6520 666f  oving average fo
+0000d7f0: 7220 616e 2061 7272 6179 2e0a 2020 2020  r an array..    
+0000d800: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+0000d810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d820: 2d2d 2d2d 2d0a 2020 2020 413a 2032 2d44  -----.    A: 2-D
+0000d830: 2061 7272 6179 206f 6620 6461 7461 2074   array of data t
+0000d840: 6f20 6265 2073 6d6f 6f74 6865 640a 2020  o be smoothed.  
+0000d850: 2020 4e3a 2069 6e74 6567 6572 2c20 6974    N: integer, it
+0000d860: 2064 6566 696e 6573 2074 6865 2066 756c   defines the ful
+0000d870: 6c21 2120 7769 6e64 6f77 206c 656e 6774  l!! window lengt
+0000d880: 6820 746f 2073 6d6f 6f74 680a 2020 2020  h to smooth.    
+0000d890: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+0000d8a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d8b0: 2d2d 0a20 2020 2042 3a20 322d 4420 6172  --.    B: 2-D ar
+0000d8c0: 7261 7920 7769 7468 2073 6d6f 6f74 6865  ray with smoothe
+0000d8d0: 6420 6461 7461 0a20 2020 2022 2222 0a20  d data.    """. 
+0000d8e0: 2020 206e 7463 2c20 6e73 7074 203d 2041     ntc, nspt = A
+0000d8f0: 2e73 6861 7065 0a20 2020 2023 2064 6566  .shape.    # def
+0000d900: 696e 6573 2061 6e20 6172 7261 7920 7769  ines an array wi
+0000d910: 7468 204e 2065 7874 7261 2073 616d 706c  th N extra sampl
+0000d920: 6573 2061 7420 6569 7468 6572 2073 6964  es at either sid
+0000d930: 650a 2020 2020 7465 6d70 203d 206e 702e  e.    temp = np.
+0000d940: 7a65 726f 7328 5b6e 7463 2c20 6e73 7074  zeros([ntc, nspt
+0000d950: 202b 2032 202a 204e 5d29 0a20 2020 2023   + 2 * N]).    #
+0000d960: 2073 6574 2074 6865 2063 656e 7472 616c   set the central
+0000d970: 2070 6f72 7469 6f6e 206f 6620 7468 6520   portion of the 
+0000d980: 6172 7261 7920 746f 2041 0a20 2020 2074  array to A.    t
+0000d990: 656d 705b 3a2c 204e 3a2d 4e5d 203d 2041  emp[:, N:-N] = A
+0000d9a0: 0a20 2020 2023 206c 6561 6469 6e67 2073  .    # leading s
+0000d9b0: 616d 706c 6573 3a20 6571 7561 6c20 746f  amples: equal to
+0000d9c0: 2066 6972 7374 2073 616d 706c 6520 6f66   first sample of
+0000d9d0: 2061 6374 7561 6c20 6172 7261 790a 2020   actual array.  
+0000d9e0: 2020 7465 6d70 5b3a 2c20 303a 4e5d 203d    temp[:, 0:N] =
+0000d9f0: 206e 702e 7265 7065 6174 286e 702e 6578   np.repeat(np.ex
+0000da00: 7061 6e64 5f64 696d 7328 7465 6d70 5b3a  pand_dims(temp[:
+0000da10: 2c20 4e5d 2c20 6178 6973 3d2d 3129 2c20  , N], axis=-1), 
+0000da20: 4e2c 2061 7869 733d 2d31 290a 2020 2020  N, axis=-1).    
+0000da30: 2320 7472 6169 6c69 6e67 2073 616d 706c  # trailing sampl
+0000da40: 6573 3a20 4571 7561 6c20 746f 206c 6173  es: Equal to las
+0000da50: 7420 7361 6d70 6c65 206f 6620 6163 7475  t sample of actu
+0000da60: 616c 2061 7272 6179 0a20 2020 2074 656d  al array.    tem
+0000da70: 705b 3a2c 202d 4e3a 5d20 3d20 6e70 2e72  p[:, -N:] = np.r
+0000da80: 6570 6561 7428 6e70 2e65 7870 616e 645f  epeat(np.expand_
+0000da90: 6469 6d73 2874 656d 705b 3a2c 202d 4e20  dims(temp[:, -N 
+0000daa0: 2d20 315d 2c20 6178 6973 3d2d 3129 2c20  - 1], axis=-1), 
+0000dab0: 4e2c 2061 7869 733d 2d31 290a 2020 2020  N, axis=-1).    
+0000dac0: 2320 636f 6e76 6f6c 7665 2077 6974 6820  # convolve with 
+0000dad0: 6120 626f 7863 6172 2061 6e64 206e 6f72  a boxcar and nor
+0000dae0: 6d61 6c69 7a65 2c20 616e 6420 7573 6520  malize, and use 
+0000daf0: 6f6e 6c79 2063 656e 7472 616c 2070 6f72  only central por
+0000db00: 7469 6f6e 206f 6620 7468 6520 7265 7375  tion of the resu
+0000db10: 6c74 0a20 2020 2023 2077 6974 6820 6c65  lt.    # with le
+0000db20: 6e67 7468 2065 7175 616c 2074 6f20 7468  ngth equal to th
+0000db30: 6520 6f72 6967 696e 616c 2061 7272 6179  e original array
+0000db40: 2c20 6469 7363 6172 6469 6e67 2074 6865  , discarding the
+0000db50: 2061 6464 6564 206c 6561 6469 6e67 2061   added leading a
+0000db60: 6e64 2074 7261 696c 696e 6720 7361 6d70  nd trailing samp
+0000db70: 6c65 730a 2020 2020 4220 3d20 7363 6970  les.    B = scip
+0000db80: 792e 7369 676e 616c 2e63 6f6e 766f 6c76  y.signal.convolv
+0000db90: 6532 6428 7465 6d70 2c20 6e70 2e65 7870  e2d(temp, np.exp
+0000dba0: 616e 645f 6469 6d73 286e 702e 6f6e 6573  and_dims(np.ones
+0000dbb0: 284e 2920 2f20 4e2c 2061 7869 733d 3029  (N) / N, axis=0)
+0000dbc0: 2c20 6d6f 6465 3d22 7361 6d65 2229 5b3a  , mode="same")[:
+0000dbd0: 2c20 4e3a 2d4e 5d0a 2020 2020 7265 7475  , N:-N].    retu
+0000dbe0: 726e 2042 0a0a 0a64 6566 2072 6f62 7573  rn B...def robus
+0000dbf0: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
+0000dc00: 2c20 6570 7369 6c6f 6e29 3a0a 2020 2020  , epsilon):.    
+0000dc10: 2222 220a 2020 2020 7468 6973 2069 7320  """.    this is 
+0000dc20: 6120 726f 6275 7374 2073 7461 636b 696e  a robust stackin
+0000dc30: 6720 616c 676f 7269 7468 6d20 6465 7363  g algorithm desc
+0000dc40: 7269 6265 6420 696e 2050 616c 7669 7320  ribed in Palvis 
+0000dc50: 616e 6420 5665 726e 6f6e 2032 3031 300a  and Vernon 2010.
+0000dc60: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+0000dc70: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000dc80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000dc90: 6363 5f61 7272 6179 3a20 6e75 6d70 792e  cc_array: numpy.
+0000dca0: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
+0000dcb0: 2074 6865 2032 4420 6372 6f73 7320 636f   the 2D cross co
+0000dcc0: 7272 656c 6174 696f 6e20 6d61 7472 6978  rrelation matrix
+0000dcd0: 0a20 2020 2065 7073 696c 6f6e 3a20 7265  .    epsilon: re
+0000dce0: 7369 6475 616c 2074 6872 6568 6f6c 6420  sidual threhold 
+0000dcf0: 746f 2071 7569 7420 7468 6520 6974 6572  to quit the iter
+0000dd00: 6174 696f 6e0a 2020 2020 5245 5455 524e  ation.    RETURN
+0000dd10: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000dd20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000dd30: 2020 6e65 7773 7461 636b 3a20 6e75 6d70    newstack: nump
+0000dd40: 7920 7665 6374 6f72 2063 6f6e 7461 696e  y vector contain
+0000dd50: 7320 7468 6520 7374 6163 6b65 6420 6372  s the stacked cr
+0000dd60: 6f73 7320 636f 7272 656c 6174 696f 6e0a  oss correlation.
+0000dd70: 0a20 2020 2057 7269 7474 656e 2062 7920  .    Written by 
+0000dd80: 4d61 7269 6e65 2044 656e 6f6c 6c65 0a20  Marine Denolle. 
+0000dd90: 2020 2022 2222 0a20 2020 2072 6573 203d     """.    res =
+0000dda0: 2039 6539 2020 2320 7265 7369 6475 616c   9e9  # residual
+0000ddb0: 730a 2020 2020 7720 3d20 6e70 2e6f 6e65  s.    w = np.one
+0000ddc0: 7328 6363 5f61 7272 6179 2e73 6861 7065  s(cc_array.shape
+0000ddd0: 5b30 5d29 0a20 2020 206e 7374 6570 203d  [0]).    nstep =
+0000dde0: 2030 0a20 2020 206e 6577 7374 6163 6b20   0.    newstack 
+0000ddf0: 3d20 6e70 2e6d 6564 6961 6e28 6363 5f61  = np.median(cc_a
+0000de00: 7272 6179 2c20 6178 6973 3d30 290a 2020  rray, axis=0).  
+0000de10: 2020 7768 696c 6520 7265 7320 3e20 6570    while res > ep
+0000de20: 7369 6c6f 6e3a 0a20 2020 2020 2020 2073  silon:.        s
+0000de30: 7461 636b 203d 206e 6577 7374 6163 6b0a  tack = newstack.
+0000de40: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000de50: 2072 616e 6765 2863 635f 6172 7261 792e   range(cc_array.
+0000de60: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
+0000de70: 2020 2020 2020 2063 7261 7020 3d20 6e70         crap = np
+0000de80: 2e6d 756c 7469 706c 7928 7374 6163 6b2c  .multiply(stack,
+0000de90: 2063 635f 6172 7261 795b 692c 203a 5d2e   cc_array[i, :].
+0000dea0: 5429 0a20 2020 2020 2020 2020 2020 2063  T).            c
+0000deb0: 7261 705f 646f 7420 3d20 6e70 2e73 756d  rap_dot = np.sum
+0000dec0: 2863 7261 7029 0a20 2020 2020 2020 2020  (crap).         
+0000ded0: 2020 2064 695f 6e6f 726d 203d 206e 702e     di_norm = np.
+0000dee0: 6c69 6e61 6c67 2e6e 6f72 6d28 6363 5f61  linalg.norm(cc_a
+0000def0: 7272 6179 5b69 2c20 3a5d 290a 2020 2020  rray[i, :]).    
+0000df00: 2020 2020 2020 2020 7269 203d 2063 635f          ri = cc_
+0000df10: 6172 7261 795b 692c 203a 5d20 2d20 6372  array[i, :] - cr
+0000df20: 6170 5f64 6f74 202a 2073 7461 636b 0a20  ap_dot * stack. 
+0000df30: 2020 2020 2020 2020 2020 2072 695f 6e6f             ri_no
+0000df40: 726d 203d 206e 702e 6c69 6e61 6c67 2e6e  rm = np.linalg.n
+0000df50: 6f72 6d28 7269 290a 2020 2020 2020 2020  orm(ri).        
+0000df60: 2020 2020 775b 695d 203d 206e 702e 6162      w[i] = np.ab
+0000df70: 7328 6372 6170 5f64 6f74 2920 2f20 6469  s(crap_dot) / di
+0000df80: 5f6e 6f72 6d20 2f20 7269 5f6e 6f72 6d20  _norm / ri_norm 
+0000df90: 2023 202f 6c65 6e28 6363 5f61 7272 6179   # /len(cc_array
+0000dfa0: 5b3a 2c31 5d29 0a20 2020 2020 2020 2023  [:,1]).        #
+0000dfb0: 2070 7269 6e74 2877 290a 2020 2020 2020   print(w).      
+0000dfc0: 2020 7720 3d20 7720 2f20 6e70 2e73 756d    w = w / np.sum
+0000dfd0: 2877 290a 2020 2020 2020 2020 6e65 7773  (w).        news
+0000dfe0: 7461 636b 203d 206e 702e 7375 6d28 2877  tack = np.sum((w
+0000dff0: 202a 2063 635f 6172 7261 792e 5429 2e54   * cc_array.T).T
+0000e000: 2c20 6178 6973 3d30 2920 2023 202f 6c65  , axis=0)  # /le
+0000e010: 6e28 6363 5f61 7272 6179 5b3a 2c31 5d29  n(cc_array[:,1])
+0000e020: 0a20 2020 2020 2020 2072 6573 203d 206e  .        res = n
+0000e030: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6e65  p.linalg.norm(ne
+0000e040: 7773 7461 636b 202d 2073 7461 636b 2c20  wstack - stack, 
+0000e050: 6f72 643d 3129 202f 206e 702e 6c69 6e61  ord=1) / np.lina
+0000e060: 6c67 2e6e 6f72 6d28 6e65 7773 7461 636b  lg.norm(newstack
+0000e070: 2920 2f20 6c65 6e28 6363 5f61 7272 6179  ) / len(cc_array
+0000e080: 5b3a 2c20 315d 290a 2020 2020 2020 2020  [:, 1]).        
+0000e090: 6e73 7465 7020 2b3d 2031 0a20 2020 2020  nstep += 1.     
+0000e0a0: 2020 2069 6620 6e73 7465 7020 3e20 3130     if nstep > 10
+0000e0b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e0c0: 7475 726e 206e 6577 7374 6163 6b2c 2077  turn newstack, w
+0000e0d0: 2c20 6e73 7465 700a 2020 2020 7265 7475  , nstep.    retu
+0000e0e0: 726e 206e 6577 7374 6163 6b2c 2077 2c20  rn newstack, w, 
+0000e0f0: 6e73 7465 700a 0a0a 6465 6620 7365 6c65  nstep...def sele
+0000e100: 6374 6976 655f 7374 6163 6b28 6363 5f61  ctive_stack(cc_a
+0000e110: 7272 6179 2c20 6570 7369 6c6f 6e29 3a0a  rray, epsilon):.
+0000e120: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
+0000e130: 2069 7320 6120 7365 6c65 6374 6976 6520   is a selective 
+0000e140: 7374 6163 6b69 6e67 2061 6c67 6f72 6974  stacking algorit
+0000e150: 686d 2064 6576 656c 6f70 6564 2062 7920  hm developed by 
+0000e160: 4a61 7265 6420 4272 7961 6e2e 0a0a 2020  Jared Bryan...  
+0000e170: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+0000e180: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000e190: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 635f  --------.    cc_
+0000e1a0: 6172 7261 793a 206e 756d 7079 2e6e 6461  array: numpy.nda
+0000e1b0: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
+0000e1c0: 6520 3244 2063 726f 7373 2063 6f72 7265  e 2D cross corre
+0000e1d0: 6c61 7469 6f6e 206d 6174 7269 780a 2020  lation matrix.  
+0000e1e0: 2020 6570 7369 6c6f 6e3a 2072 6573 6964    epsilon: resid
+0000e1f0: 7561 6c20 7468 7265 686f 6c64 2074 6f20  ual threhold to 
+0000e200: 7175 6974 2074 6865 2069 7465 7261 7469  quit the iterati
+0000e210: 6f6e 0a20 2020 2052 4554 5552 4e53 3a0a  on.    RETURNS:.
+0000e220: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000e230: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
+0000e240: 6577 7374 6163 6b3a 206e 756d 7079 2076  ewstack: numpy v
+0000e250: 6563 746f 7220 636f 6e74 6169 6e73 2074  ector contains t
+0000e260: 6865 2073 7461 636b 6564 2063 726f 7373  he stacked cross
+0000e270: 2063 6f72 7265 6c61 7469 6f6e 0a0a 2020   correlation..  
+0000e280: 2020 5772 6974 7465 6e20 6279 204d 6172    Written by Mar
+0000e290: 696e 6520 4465 6e6f 6c6c 650a 2020 2020  ine Denolle.    
+0000e2a0: 2222 220a 2020 2020 6363 203d 206e 702e  """.    cc = np.
+0000e2b0: 6f6e 6573 2863 635f 6172 7261 792e 7368  ones(cc_array.sh
+0000e2c0: 6170 655b 305d 290a 2020 2020 6e65 7773  ape[0]).    news
+0000e2d0: 7461 636b 203d 206e 702e 6d65 616e 2863  tack = np.mean(c
+0000e2e0: 635f 6172 7261 792c 2061 7869 733d 3029  c_array, axis=0)
+0000e2f0: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+0000e300: 6e67 6528 6363 5f61 7272 6179 2e73 6861  nge(cc_array.sha
+0000e310: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
+0000e320: 6363 5b69 5d20 3d20 6e70 2e73 756d 286e  cc[i] = np.sum(n
+0000e330: 702e 6d75 6c74 6970 6c79 286e 6577 7374  p.multiply(newst
+0000e340: 6163 6b2c 2063 635f 6172 7261 795b 692c  ack, cc_array[i,
+0000e350: 203a 5d2e 5429 290a 2020 2020 696b 203d   :].T)).    ik =
+0000e360: 206e 702e 7768 6572 6528 6363 203e 3d20   np.where(cc >= 
+0000e370: 6570 7369 6c6f 6e29 5b30 5d0a 2020 2020  epsilon)[0].    
+0000e380: 6e65 7773 7461 636b 203d 206e 702e 6d65  newstack = np.me
+0000e390: 616e 2863 635f 6172 7261 795b 696b 2c20  an(cc_array[ik, 
+0000e3a0: 3a5d 2c20 6178 6973 3d30 290a 0a20 2020  :], axis=0)..   
+0000e3b0: 2072 6574 7572 6e20 6e65 7773 7461 636b   return newstack
+0000e3c0: 2c20 6363 0a0a 0a64 6566 2077 6869 7465  , cc...def white
+0000e3d0: 6e5f 3144 2874 696d 6573 6572 6965 732c  n_1D(timeseries,
+0000e3e0: 2066 6674 5f70 6172 612c 206e 5f74 6170   fft_para, n_tap
+0000e3f0: 6572 293a 0a20 2020 2022 2222 0a20 2020  er):.    """.   
+0000e400: 2054 6869 7320 6675 6e63 7469 6f6e 2074   This function t
+0000e410: 616b 6573 2061 2031 2d64 696d 656e 7369  akes a 1-dimensi
+0000e420: 6f6e 616c 2074 696d 6573 6572 6965 7320  onal timeseries 
+0000e430: 6172 7261 792c 2074 7261 6e73 666f 726d  array, transform
+0000e440: 7320 746f 2066 7265 7175 656e 6379 2064  s to frequency d
+0000e450: 6f6d 6169 6e20 7573 696e 6720 6666 742c  omain using fft,
+0000e460: 0a20 2020 2077 6869 7465 6e73 2074 6865  .    whitens the
+0000e470: 2061 6d70 6c69 7475 6465 206f 6620 7468   amplitude of th
+0000e480: 6520 7370 6563 7472 756d 2069 6e20 6672  e spectrum in fr
+0000e490: 6571 7565 6e63 7920 646f 6d61 696e 2062  equency domain b
+0000e4a0: 6574 7765 656e 202a 6672 6571 6d69 6e2a  etween *freqmin*
+0000e4b0: 2061 6e64 202a 6672 6571 6d61 782a 0a20   and *freqmax*. 
+0000e4c0: 2020 2061 6e64 2072 6574 7572 6e73 2074     and returns t
+0000e4d0: 6865 2077 6869 7465 6e65 6420 6666 742e  he whitened fft.
+0000e4e0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+0000e4f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000e500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000e510: 6461 7461 3a20 6e75 6d70 792e 6e64 6172  data: numpy.ndar
+0000e520: 7261 7920 636f 6e74 6169 6e73 2074 6865  ray contains the
+0000e530: 2031 4420 7469 6d65 2073 6572 6965 7320   1D time series 
+0000e540: 746f 2077 6869 7465 6e0a 2020 2020 6666  to whiten.    ff
+0000e550: 745f 7061 7261 3a20 6469 6374 2063 6f6e  t_para: dict con
+0000e560: 7461 696e 696e 6720 616c 6c20 6666 745f  taining all fft_
+0000e570: 6363 2070 6172 616d 6574 6572 7320 7375  cc parameters su
+0000e580: 6368 2061 730a 2020 2020 2020 2020 6474  ch as.        dt
+0000e590: 3a20 5468 6520 7361 6d70 6c69 6e67 2073  : The sampling s
+0000e5a0: 7061 6365 206f 6620 7468 6520 6064 6174  pace of the `dat
+0000e5b0: 6160 0a20 2020 2020 2020 2066 7265 716d  a`.        freqm
+0000e5c0: 696e 3a20 5468 6520 6c6f 7765 7220 6672  in: The lower fr
+0000e5d0: 6571 7565 6e63 7920 626f 756e 640a 2020  equency bound.  
+0000e5e0: 2020 2020 2020 6672 6571 6d61 783a 2054        freqmax: T
+0000e5f0: 6865 2075 7070 6572 2066 7265 7175 656e  he upper frequen
+0000e600: 6379 2062 6f75 6e64 0a20 2020 2020 2020  cy bound.       
+0000e610: 2073 6d6f 6f74 685f 4e3a 2069 6e74 6567   smooth_N: integ
+0000e620: 6572 2c20 6974 2064 6566 696e 6573 2074  er, it defines t
+0000e630: 6865 2068 616c 6620 7769 6e64 6f77 206c  he half window l
+0000e640: 656e 6774 6820 746f 2073 6d6f 6f74 680a  ength to smooth.
+0000e650: 2020 2020 2020 2020 6e5f 7461 7065 722c          n_taper,
+0000e660: 206f 7074 696f 6e61 6c3a 2069 6e74 6567   optional: integ
+0000e670: 6572 2c20 6465 6669 6e65 2074 6865 2077  er, define the w
+0000e680: 6964 7468 206f 6620 7468 6520 7461 7065  idth of the tape
+0000e690: 7220 696e 2073 616d 706c 6573 0a20 2020  r in samples.   
+0000e6a0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000e6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e6c0: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
+0000e6d0: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
+0000e6e0: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+0000e6f0: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
+0000e700: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
+0000e710: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
+0000e720: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
+0000e730: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
+0000e740: 7061 7261 6d65 7465 7273 0a20 2020 2064  parameters.    d
+0000e750: 656c 7461 203d 2066 6674 5f70 6172 615b  elta = fft_para[
+0000e760: 2264 7422 5d0a 2020 2020 6672 6571 6d69  "dt"].    freqmi
+0000e770: 6e20 3d20 6666 745f 7061 7261 5b22 6672  n = fft_para["fr
+0000e780: 6571 6d69 6e22 5d0a 2020 2020 6672 6571  eqmin"].    freq
+0000e790: 6d61 7820 3d20 6666 745f 7061 7261 5b22  max = fft_para["
+0000e7a0: 6672 6571 6d61 7822 5d0a 2020 2020 736d  freqmax"].    sm
+0000e7b0: 6f6f 7468 5f4e 203d 2066 6674 5f70 6172  ooth_N = fft_par
+0000e7c0: 615b 2273 6d6f 6f74 685f 4e22 5d0a 0a20  a["smooth_N"].. 
+0000e7d0: 2020 206e 6666 7420 3d20 6e65 7874 5f66     nfft = next_f
+0000e7e0: 6173 745f 6c65 6e28 6c65 6e28 7469 6d65  ast_len(len(time
+0000e7f0: 7365 7269 6573 2929 0a20 2020 2073 7065  series)).    spe
+0000e800: 6320 3d20 6e70 2e66 6674 2e66 6674 2874  c = np.fft.fft(t
+0000e810: 696d 6573 6572 6965 732c 206e 6666 7429  imeseries, nfft)
+0000e820: 0a20 2020 2066 7265 7120 3d20 6e70 2e66  .    freq = np.f
+0000e830: 6674 2e66 6674 6672 6571 286e 6666 742c  ft.fftfreq(nfft,
+0000e840: 2064 3d64 656c 7461 290a 0a20 2020 2069   d=delta)..    i
+0000e850: 7830 203d 206e 702e 6172 676d 696e 286e  x0 = np.argmin(n
+0000e860: 702e 6162 7328 6672 6571 202d 2066 7265  p.abs(freq - fre
+0000e870: 716d 696e 2929 0a20 2020 2069 7831 203d  qmin)).    ix1 =
+0000e880: 206e 702e 6172 676d 696e 286e 702e 6162   np.argmin(np.ab
+0000e890: 7328 6672 6571 202d 2066 7265 716d 6178  s(freq - freqmax
+0000e8a0: 2929 0a0a 2020 2020 6966 2069 7831 202b  ))..    if ix1 +
+0000e8b0: 206e 5f74 6170 6572 203e 206e 6666 743a   n_taper > nfft:
+0000e8c0: 0a20 2020 2020 2020 2069 7831 3120 3d20  .        ix11 = 
+0000e8d0: 6e66 6674 0a20 2020 2065 6c73 653a 0a20  nfft.    else:. 
+0000e8e0: 2020 2020 2020 2069 7831 3120 3d20 6978         ix11 = ix
+0000e8f0: 3120 2b20 6e5f 7461 7065 720a 0a20 2020  1 + n_taper..   
+0000e900: 2069 6620 6978 3020 2d20 6e5f 7461 7065   if ix0 - n_tape
+0000e910: 7220 3c20 303a 0a20 2020 2020 2020 2069  r < 0:.        i
+0000e920: 7830 3020 3d20 300a 2020 2020 656c 7365  x00 = 0.    else
+0000e930: 3a0a 2020 2020 2020 2020 6978 3030 203d  :.        ix00 =
+0000e940: 2069 7830 202d 206e 5f74 6170 6572 0a0a   ix0 - n_taper..
+0000e950: 2020 2020 7370 6563 5f6f 7574 203d 2073      spec_out = s
+0000e960: 7065 632e 636f 7079 2829 0a20 2020 2073  pec.copy().    s
+0000e970: 7065 635f 6f75 745b 303a 6978 3030 5d20  pec_out[0:ix00] 
+0000e980: 3d20 302e 3020 2b20 302e 306a 0a20 2020  = 0.0 + 0.0j.   
+0000e990: 2073 7065 635f 6f75 745b 6978 3131 3a5d   spec_out[ix11:]
+0000e9a0: 203d 2030 2e30 202b 2030 2e30 6a0a 0a20   = 0.0 + 0.0j.. 
+0000e9b0: 2020 2069 6620 736d 6f6f 7468 5f4e 203c     if smooth_N <
+0000e9c0: 3d20 313a 0a20 2020 2020 2020 2073 7065  = 1:.        spe
+0000e9d0: 635f 6f75 745b 6978 3030 3a69 7831 315d  c_out[ix00:ix11]
+0000e9e0: 203d 206e 702e 6578 7028 312e 306a 202a   = np.exp(1.0j *
+0000e9f0: 206e 702e 616e 676c 6528 7370 6563 5f6f   np.angle(spec_o
+0000ea00: 7574 5b69 7830 303a 6978 3131 5d29 290a  ut[ix00:ix11])).
+0000ea10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ea20: 2020 7370 6563 5f6f 7574 5b69 7830 303a    spec_out[ix00:
+0000ea30: 6978 3131 5d20 2f3d 206d 6f76 696e 675f  ix11] /= moving_
+0000ea40: 6176 6528 6e70 2e61 6273 2873 7065 635f  ave(np.abs(spec_
+0000ea50: 6f75 745b 6978 3030 3a69 7831 315d 292c  out[ix00:ix11]),
+0000ea60: 2073 6d6f 6f74 685f 4e29 0a0a 2020 2020   smooth_N)..    
+0000ea70: 7820 3d20 6e70 2e6c 696e 7370 6163 6528  x = np.linspace(
+0000ea80: 6e70 2e70 6920 2f20 322e 302c 206e 702e  np.pi / 2.0, np.
+0000ea90: 7069 2c20 6978 3020 2d20 6978 3030 290a  pi, ix0 - ix00).
+0000eaa0: 2020 2020 7370 6563 5f6f 7574 5b69 7830      spec_out[ix0
+0000eab0: 303a 6978 305d 202a 3d20 6e70 2e63 6f73  0:ix0] *= np.cos
+0000eac0: 2878 2920 2a2a 2032 0a0a 2020 2020 7820  (x) ** 2..    x 
+0000ead0: 3d20 6e70 2e6c 696e 7370 6163 6528 302e  = np.linspace(0.
+0000eae0: 302c 206e 702e 7069 202f 2032 2e30 2c20  0, np.pi / 2.0, 
+0000eaf0: 6978 3131 202d 2069 7831 290a 2020 2020  ix11 - ix1).    
+0000eb00: 7370 6563 5f6f 7574 5b69 7831 3a69 7831  spec_out[ix1:ix1
+0000eb10: 315d 202a 3d20 6e70 2e63 6f73 2878 2920  1] *= np.cos(x) 
+0000eb20: 2a2a 2032 0a0a 2020 2020 7265 7475 726e  ** 2..    return
+0000eb30: 2073 7065 635f 6f75 740a 0a0a 6465 6620   spec_out...def 
+0000eb40: 7768 6974 656e 5f32 4428 7469 6d65 7365  whiten_2D(timese
+0000eb50: 7269 6573 2c20 6666 745f 7061 7261 2c20  ries, fft_para, 
+0000eb60: 6e5f 7461 7065 7229 3a0a 2020 2020 2222  n_taper):.    ""
+0000eb70: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
+0000eb80: 696f 6e20 7461 6b65 7320 6120 322d 6469  ion takes a 2-di
+0000eb90: 6d65 6e73 696f 6e61 6c20 7469 6d65 7365  mensional timese
+0000eba0: 7269 6573 2061 7272 6179 2c20 7472 616e  ries array, tran
+0000ebb0: 7366 6f72 6d73 2074 6f20 6672 6571 7565  sforms to freque
+0000ebc0: 6e63 7920 646f 6d61 696e 2075 7369 6e67  ncy domain using
+0000ebd0: 2066 6674 2c0a 2020 2020 7768 6974 656e   fft,.    whiten
+0000ebe0: 7320 7468 6520 616d 706c 6974 7564 6520  s the amplitude 
+0000ebf0: 6f66 2074 6865 2073 7065 6374 7275 6d20  of the spectrum 
+0000ec00: 696e 2066 7265 7175 656e 6379 2064 6f6d  in frequency dom
+0000ec10: 6169 6e20 6265 7477 6565 6e20 2a66 7265  ain between *fre
+0000ec20: 716d 696e 2a20 616e 6420 2a66 7265 716d  qmin* and *freqm
+0000ec30: 6178 2a0a 2020 2020 616e 6420 7265 7475  ax*.    and retu
+0000ec40: 726e 7320 7468 6520 7768 6974 656e 6564  rns the whitened
+0000ec50: 2066 6674 2e0a 2020 2020 5041 5241 4d45   fft..    PARAME
+0000ec60: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+0000ec70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ec80: 0a20 2020 2064 6174 613a 206e 756d 7079  .    data: numpy
+0000ec90: 2e6e 6461 7272 6179 2063 6f6e 7461 696e  .ndarray contain
+0000eca0: 7320 7468 6520 3144 2074 696d 6520 7365  s the 1D time se
+0000ecb0: 7269 6573 2074 6f20 7768 6974 656e 0a20  ries to whiten. 
+0000ecc0: 2020 2066 6674 5f70 6172 613a 2064 6963     fft_para: dic
+0000ecd0: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
+0000ece0: 2066 6674 5f63 6320 7061 7261 6d65 7465   fft_cc paramete
+0000ecf0: 7273 2073 7563 6820 6173 0a20 2020 2020  rs such as.     
+0000ed00: 2020 2064 743a 2054 6865 2073 616d 706c     dt: The sampl
+0000ed10: 696e 6720 7370 6163 6520 6f66 2074 6865  ing space of the
+0000ed20: 2060 6461 7461 600a 2020 2020 2020 2020   `data`.        
+0000ed30: 6672 6571 6d69 6e3a 2054 6865 206c 6f77  freqmin: The low
+0000ed40: 6572 2066 7265 7175 656e 6379 2062 6f75  er frequency bou
+0000ed50: 6e64 0a20 2020 2020 2020 2066 7265 716d  nd.        freqm
+0000ed60: 6178 3a20 5468 6520 7570 7065 7220 6672  ax: The upper fr
+0000ed70: 6571 7565 6e63 7920 626f 756e 640a 2020  equency bound.  
+0000ed80: 2020 2020 2020 736d 6f6f 7468 5f4e 3a20        smooth_N: 
+0000ed90: 696e 7465 6765 722c 2069 7420 6465 6669  integer, it defi
+0000eda0: 6e65 7320 7468 6520 6861 6c66 2077 696e  nes the half win
+0000edb0: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
+0000edc0: 6f6f 7468 0a20 2020 2020 2020 206e 5f74  ooth.        n_t
+0000edd0: 6170 6572 2c20 6f70 7469 6f6e 616c 3a20  aper, optional: 
+0000ede0: 696e 7465 6765 722c 2064 6566 696e 6520  integer, define 
+0000edf0: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+0000ee00: 2074 6170 6572 2069 6e20 7361 6d70 6c65   taper in sample
+0000ee10: 730a 2020 2020 5245 5455 524e 533a 0a20  s.    RETURNS:. 
+0000ee20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000ee30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 4646  ---------.    FF
+0000ee40: 5452 6177 5369 676e 3a20 6e75 6d70 792e  TRawSign: numpy.
+0000ee50: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
+0000ee60: 2074 6865 2046 4654 206f 6620 7468 6520   the FFT of the 
+0000ee70: 7768 6974 656e 6564 2069 6e70 7574 2074  whitened input t
+0000ee80: 7261 6365 2062 6574 7765 656e 2074 6865  race between the
+0000ee90: 2066 7265 7175 656e 6379 2062 6f75 6e64   frequency bound
+0000eea0: 730a 2020 2020 2222 220a 2020 2020 2320  s.    """.    # 
+0000eeb0: 6c6f 6164 2070 6172 616d 6574 6572 730a  load parameters.
+0000eec0: 2020 2020 6465 6c74 6120 3d20 6666 745f      delta = fft_
+0000eed0: 7061 7261 5b22 6474 225d 0a20 2020 2066  para["dt"].    f
+0000eee0: 7265 716d 696e 203d 2066 6674 5f70 6172  reqmin = fft_par
+0000eef0: 615b 2266 7265 716d 696e 225d 0a20 2020  a["freqmin"].   
+0000ef00: 2066 7265 716d 6178 203d 2066 6674 5f70   freqmax = fft_p
+0000ef10: 6172 615b 2266 7265 716d 6178 225d 0a20  ara["freqmax"]. 
+0000ef20: 2020 2073 6d6f 6f74 685f 4e20 3d20 6666     smooth_N = ff
+0000ef30: 745f 7061 7261 5b22 736d 6f6f 7468 5f4e  t_para["smooth_N
+0000ef40: 225d 0a0a 2020 2020 6e66 6674 203d 206e  "]..    nfft = n
+0000ef50: 6578 745f 6661 7374 5f6c 656e 2874 696d  ext_fast_len(tim
+0000ef60: 6573 6572 6965 732e 7368 6170 655b 315d  eseries.shape[1]
+0000ef70: 290a 2020 2020 7370 6563 203d 206e 702e  ).    spec = np.
+0000ef80: 6666 742e 6666 746e 2874 696d 6573 6572  fft.fftn(timeser
+0000ef90: 6965 732c 2073 3d5b 6e66 6674 5d29 0a20  ies, s=[nfft]). 
+0000efa0: 2020 2066 7265 7120 3d20 6e70 2e66 6674     freq = np.fft
+0000efb0: 2e66 6674 6672 6571 286e 6666 742c 2064  .fftfreq(nfft, d
+0000efc0: 3d64 656c 7461 290a 0a20 2020 2069 7830  =delta)..    ix0
+0000efd0: 203d 206e 702e 6172 676d 696e 286e 702e   = np.argmin(np.
+0000efe0: 6162 7328 6672 6571 202d 2066 7265 716d  abs(freq - freqm
+0000eff0: 696e 2929 0a20 2020 2069 7831 203d 206e  in)).    ix1 = n
+0000f000: 702e 6172 676d 696e 286e 702e 6162 7328  p.argmin(np.abs(
+0000f010: 6672 6571 202d 2066 7265 716d 6178 2929  freq - freqmax))
+0000f020: 0a0a 2020 2020 6966 2069 7831 202b 206e  ..    if ix1 + n
+0000f030: 5f74 6170 6572 203e 206e 6666 743a 0a20  _taper > nfft:. 
+0000f040: 2020 2020 2020 2069 7831 3120 3d20 6e66         ix11 = nf
+0000f050: 6674 0a20 2020 2065 6c73 653a 0a20 2020  ft.    else:.   
+0000f060: 2020 2020 2069 7831 3120 3d20 6978 3120       ix11 = ix1 
+0000f070: 2b20 6e5f 7461 7065 720a 0a20 2020 2069  + n_taper..    i
+0000f080: 6620 6978 3020 2d20 6e5f 7461 7065 7220  f ix0 - n_taper 
+0000f090: 3c20 303a 0a20 2020 2020 2020 2069 7830  < 0:.        ix0
+0000f0a0: 3020 3d20 300a 2020 2020 656c 7365 3a0a  0 = 0.    else:.
+0000f0b0: 2020 2020 2020 2020 6978 3030 203d 2069          ix00 = i
+0000f0c0: 7830 202d 206e 5f74 6170 6572 0a0a 2020  x0 - n_taper..  
+0000f0d0: 2020 7370 6563 5f6f 7574 203d 2073 7065    spec_out = spe
+0000f0e0: 632e 636f 7079 2829 2020 2320 6d61 7920  c.copy()  # may 
+0000f0f0: 6265 2069 6e63 6f6e 7665 6e69 656e 7420  be inconvenient 
+0000f100: 6475 6520 746f 2068 6967 6865 7220 6d65  due to higher me
+0000f110: 6d6f 7279 2075 7361 6765 0a20 2020 2073  mory usage.    s
+0000f120: 7065 635f 6f75 745b 3a2c 2030 3a69 7830  pec_out[:, 0:ix0
+0000f130: 305d 203d 2030 2e30 202b 2030 2e30 6a0a  0] = 0.0 + 0.0j.
+0000f140: 2020 2020 7370 6563 5f6f 7574 5b3a 2c20      spec_out[:, 
+0000f150: 6978 3131 3a5d 203d 2030 2e30 202b 2030  ix11:] = 0.0 + 0
+0000f160: 2e30 6a0a 0a20 2020 2069 6620 736d 6f6f  .0j..    if smoo
+0000f170: 7468 5f4e 203c 3d20 313a 0a20 2020 2020  th_N <= 1:.     
+0000f180: 2020 2073 7065 635f 6f75 745b 3a2c 2069     spec_out[:, i
+0000f190: 7830 303a 6978 3131 5d20 3d20 6e70 2e65  x00:ix11] = np.e
+0000f1a0: 7870 2831 2e30 6a20 2a20 6e70 2e61 6e67  xp(1.0j * np.ang
+0000f1b0: 6c65 2873 7065 635f 6f75 745b 3a2c 2069  le(spec_out[:, i
+0000f1c0: 7830 303a 6978 3131 5d29 290a 2020 2020  x00:ix11])).    
+0000f1d0: 656c 7365 3a0a 2020 2020 2020 2020 7370  else:.        sp
+0000f1e0: 6563 5f6f 7574 5b3a 2c20 6978 3030 3a69  ec_out[:, ix00:i
+0000f1f0: 7831 315d 202f 3d20 6d6f 7669 6e67 5f61  x11] /= moving_a
+0000f200: 7665 5f32 4428 6e70 2e61 6273 2873 7065  ve_2D(np.abs(spe
+0000f210: 635f 6f75 745b 3a2c 2069 7830 303a 6978  c_out[:, ix00:ix
+0000f220: 3131 5d29 2c20 736d 6f6f 7468 5f4e 290a  11]), smooth_N).
+0000f230: 0a20 2020 2078 203d 206e 702e 6c69 6e73  .    x = np.lins
+0000f240: 7061 6365 286e 702e 7069 202f 2032 2e30  pace(np.pi / 2.0
+0000f250: 2c20 6e70 2e70 692c 2069 7830 202d 2069  , np.pi, ix0 - i
+0000f260: 7830 3029 0a20 2020 2073 7065 635f 6f75  x00).    spec_ou
+0000f270: 745b 3a2c 2069 7830 303a 6978 305d 202a  t[:, ix00:ix0] *
+0000f280: 3d20 6e70 2e63 6f73 2878 2920 2a2a 2032  = np.cos(x) ** 2
+0000f290: 0a0a 2020 2020 7820 3d20 6e70 2e6c 696e  ..    x = np.lin
+0000f2a0: 7370 6163 6528 302e 302c 206e 702e 7069  space(0.0, np.pi
+0000f2b0: 202f 2032 2e30 2c20 6978 3131 202d 2069   / 2.0, ix11 - i
+0000f2c0: 7831 290a 2020 2020 7370 6563 5f6f 7574  x1).    spec_out
+0000f2d0: 5b3a 2c20 6978 313a 6978 3131 5d20 2a3d  [:, ix1:ix11] *=
+0000f2e0: 206e 702e 636f 7328 7829 202a 2a20 320a   np.cos(x) ** 2.
+0000f2f0: 0a20 2020 2072 6574 7572 6e20 7370 6563  .    return spec
+0000f300: 5f6f 7574 0a0a 0a64 6566 2077 6869 7465  _out...def white
+0000f310: 6e28 6461 7461 2c20 6666 745f 7061 7261  n(data, fft_para
+0000f320: 2c20 6e5f 7461 7065 723d 3130 3029 3a0a  , n_taper=100):.
+0000f330: 2020 2020 2222 220a 2020 2020 5468 6973      """.    This
+0000f340: 2066 756e 6374 696f 6e20 7461 6b65 7320   function takes 
+0000f350: 6120 7469 6d65 7365 7269 6573 2061 7272  a timeseries arr
+0000f360: 6179 2c20 7472 616e 7366 6f72 6d73 2074  ay, transforms t
+0000f370: 6f20 6672 6571 7565 6e63 7920 646f 6d61  o frequency doma
+0000f380: 696e 2075 7369 6e67 2066 6674 2c0a 2020  in using fft,.  
+0000f390: 2020 7768 6974 656e 7320 7468 6520 616d    whitens the am
+0000f3a0: 706c 6974 7564 6520 6f66 2074 6865 2073  plitude of the s
+0000f3b0: 7065 6374 7275 6d20 696e 2066 7265 7175  pectrum in frequ
+0000f3c0: 656e 6379 2064 6f6d 6169 6e20 6265 7477  ency domain betw
+0000f3d0: 6565 6e20 2a66 7265 716d 696e 2a20 616e  een *freqmin* an
+0000f3e0: 6420 2a66 7265 716d 6178 2a0a 2020 2020  d *freqmax*.    
+0000f3f0: 616e 6420 7265 7475 726e 7320 7468 6520  and returns the 
+0000f400: 7768 6974 656e 6564 2066 6674 2e0a 2020  whitened fft..  
+0000f410: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+0000f420: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000f430: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
+0000f440: 613a 206e 756d 7079 2e6e 6461 7272 6179  a: numpy.ndarray
+0000f450: 2063 6f6e 7461 696e 7320 7468 6520 3144   contains the 1D
+0000f460: 2074 696d 6520 7365 7269 6573 2074 6f20   time series to 
+0000f470: 7768 6974 656e 0a20 2020 2066 6674 5f70  whiten.    fft_p
+0000f480: 6172 613a 2064 6963 7420 636f 6e74 6169  ara: dict contai
+0000f490: 6e69 6e67 2061 6c6c 2066 6674 5f63 6320  ning all fft_cc 
+0000f4a0: 7061 7261 6d65 7465 7273 2073 7563 6820  parameters such 
+0000f4b0: 6173 0a20 2020 2020 2020 2064 743a 2054  as.        dt: T
+0000f4c0: 6865 2073 616d 706c 696e 6720 7370 6163  he sampling spac
+0000f4d0: 6520 6f66 2074 6865 2060 6461 7461 600a  e of the `data`.
+0000f4e0: 2020 2020 2020 2020 6672 6571 6d69 6e3a          freqmin:
+0000f4f0: 2054 6865 206c 6f77 6572 2066 7265 7175   The lower frequ
+0000f500: 656e 6379 2062 6f75 6e64 0a20 2020 2020  ency bound.     
+0000f510: 2020 2066 7265 716d 6178 3a20 5468 6520     freqmax: The 
+0000f520: 7570 7065 7220 6672 6571 7565 6e63 7920  upper frequency 
+0000f530: 626f 756e 640a 2020 2020 2020 2020 736d  bound.        sm
+0000f540: 6f6f 7468 5f4e 3a20 696e 7465 6765 722c  ooth_N: integer,
+0000f550: 2069 7420 6465 6669 6e65 7320 7468 6520   it defines the 
+0000f560: 6861 6c66 2077 696e 646f 7720 6c65 6e67  half window leng
+0000f570: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
+0000f580: 2020 2020 2066 7265 715f 6e6f 726d 3a20       freq_norm: 
+0000f590: 7768 6974 656e 696e 6720 6d65 7468 6f64  whitening method
+0000f5a0: 2062 6574 7765 656e 2027 6f6e 652d 6269   between 'one-bi
+0000f5b0: 7427 2061 6e64 2027 524d 4127 0a20 2020  t' and 'RMA'.   
+0000f5c0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000f5d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000f5e0: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
+0000f5f0: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
+0000f600: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+0000f610: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
+0000f620: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
+0000f630: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
+0000f640: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
+0000f650: 2022 2222 0a0a 2020 2020 2320 5370 6565   """..    # Spee
+0000f660: 6420 7570 2046 4654 2062 7920 7061 6464  d up FFT by padd
+0000f670: 696e 6720 746f 206f 7074 696d 616c 2073  ing to optimal s
+0000f680: 697a 6520 666f 7220 4646 5450 4143 4b0a  ize for FFTPACK.
+0000f690: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
+0000f6a0: 203d 3d20 313a 0a20 2020 2020 2020 2046   == 1:.        F
+0000f6b0: 4654 5261 7753 6967 6e20 3d20 7768 6974  FTRawSign = whit
+0000f6c0: 656e 5f31 4428 6461 7461 2c20 6666 745f  en_1D(data, fft_
+0000f6d0: 7061 7261 2c20 6e5f 7461 7065 7229 0a20  para, n_taper). 
+0000f6e0: 2020 2020 2020 2023 2041 5252 5f4f 5554         # ARR_OUT
+0000f6f0: 3a20 4f6e 6c79 2066 6f72 2063 6f6e 7369  : Only for consi
+0000f700: 7374 656e 6379 2077 6974 6820 6e6f 6973  stency with nois
+0000f710: 6570 7920 6170 7072 6f61 6368 206f 6620  epy approach of 
+0000f720: 686f 6c64 696e 6720 7468 6520 6675 6c6c  holding the full
+0000f730: 0a20 2020 2020 2020 2023 2073 7065 6374  .        # spect
+0000f740: 7275 6d20 286e 6f74 206a 7573 7420 3020  rum (not just 0 
+0000f750: 616e 6420 706f 7369 7469 7665 2066 7265  and positive fre
+0000f760: 712e 2070 6172 7429 0a20 2020 2020 2020  q. part).       
+0000f770: 2061 7272 5f6f 7574 203d 206e 702e 7a65   arr_out = np.ze
+0000f780: 726f 7328 2846 4654 5261 7753 6967 6e2e  ros((FFTRawSign.
+0000f790: 7368 6170 655b 305d 202d 2031 2920 2a20  shape[0] - 1) * 
+0000f7a0: 3220 2b20 312c 2064 7479 7065 3d63 6f6d  2 + 1, dtype=com
+0000f7b0: 706c 6578 290a 2020 2020 2020 2020 6172  plex).        ar
+0000f7c0: 725f 6f75 745b 3020 3a20 4646 5452 6177  r_out[0 : FFTRaw
+0000f7d0: 5369 676e 2e73 6861 7065 5b30 5d5d 203d  Sign.shape[0]] =
+0000f7e0: 2046 4654 5261 7753 6967 6e0a 2020 2020   FFTRawSign.    
+0000f7f0: 2020 2020 6172 725f 6f75 745b 4646 5452      arr_out[FFTR
+0000f800: 6177 5369 676e 2e73 6861 7065 5b30 5d20  awSign.shape[0] 
+0000f810: 3a5d 203d 2046 4654 5261 7753 6967 6e5b  :] = FFTRawSign[
+0000f820: 313a 5d2e 636f 6e6a 7567 6174 6528 295b  1:].conjugate()[
+0000f830: 3a3a 2d31 5d0a 0a20 2020 2065 6c69 6620  ::-1]..    elif 
+0000f840: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
+0000f850: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
+0000f860: 676e 203d 2077 6869 7465 6e5f 3244 2864  gn = whiten_2D(d
+0000f870: 6174 612c 2066 6674 5f70 6172 612c 206e  ata, fft_para, n
+0000f880: 5f74 6170 6572 290a 2020 2020 2020 2020  _taper).        
+0000f890: 6172 725f 6f75 7420 3d20 6e70 2e7a 6572  arr_out = np.zer
+0000f8a0: 6f73 2828 4646 5452 6177 5369 676e 2e73  os((FFTRawSign.s
+0000f8b0: 6861 7065 5b30 5d2c 2028 4646 5452 6177  hape[0], (FFTRaw
+0000f8c0: 5369 676e 2e73 6861 7065 5b31 5d20 2d20  Sign.shape[1] - 
+0000f8d0: 3129 202a 2032 202b 2031 292c 2064 7479  1) * 2 + 1), dty
+0000f8e0: 7065 3d63 6f6d 706c 6578 290a 2020 2020  pe=complex).    
+0000f8f0: 2020 2020 6172 725f 6f75 745b 3a2c 2046      arr_out[:, F
+0000f900: 4654 5261 7753 6967 6e2e 7368 6170 655b  FTRawSign.shape[
+0000f910: 315d 203a 5d20 3d20 4646 5452 6177 5369  1] :] = FFTRawSi
+0000f920: 676e 5b3a 2c20 313a 5d2e 636f 6e6a 7567  gn[:, 1:].conjug
+0000f930: 6174 6528 295b 3a3a 2d31 5d0a 2020 2020  ate()[::-1].    
+0000f940: 7265 7475 726e 2046 4654 5261 7753 6967  return FFTRawSig
+0000f950: 6e0a 0a0a 6465 6620 6164 6170 7469 7665  n...def adaptive
+0000f960: 5f66 696c 7465 7228 6172 722c 2067 293a  _filter(arr, g):
+0000f970: 0a20 2020 2022 2222 0a20 2020 2074 6865  .    """.    the
+0000f980: 2061 6461 7074 6976 6520 636f 7661 7269   adaptive covari
+0000f990: 616e 6365 2066 696c 7465 7220 746f 2065  ance filter to e
+0000f9a0: 6e68 616e 6365 2063 6f68 6572 656e 7420  nhance coherent 
+0000f9b0: 7369 676e 616c 732e 2046 656c 6c6f 7773  signals. Fellows
+0000f9c0: 2074 6865 206d 6574 686f 6420 6f66 0a20   the method of. 
+0000f9d0: 2020 204e 616b 6174 6120 6574 2061 6c2e     Nakata et al.
+0000f9e0: 2c20 3230 3135 2028 4170 7065 6e64 6978  , 2015 (Appendix
+0000f9f0: 2042 290a 0a20 2020 2074 6865 2066 696c   B)..    the fil
+0000fa00: 7465 7265 6420 7369 676e 616c 205b 7831  tered signal [x1
+0000fa10: 5d20 6973 2067 6976 656e 2062 7920 7831  ] is given by x1
+0000fa20: 203d 2069 6666 7428 502a 7831 2877 2929   = ifft(P*x1(w))
+0000fa30: 2077 6865 7265 2078 3120 6973 2074 6865   where x1 is the
+0000fa40: 2066 6674 6564 2073 7065 6374 7261 0a20   ffted spectra. 
+0000fa50: 2020 2061 6e64 2050 2069 7320 7468 6520     and P is the 
+0000fa60: 6669 6c74 6572 2e20 5020 6973 2063 6f6e  filter. P is con
+0000fa70: 7374 7275 6374 6564 2062 7920 7573 696e  structed by usin
+0000fa80: 6720 7468 6520 7465 6d70 6f72 616c 2063  g the temporal c
+0000fa90: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000faa0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
+0000fab0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000fac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000fad0: 2020 6172 723a 206e 756d 7079 2e6e 6461    arr: numpy.nda
+0000fae0: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
+0000faf0: 6520 3244 2074 7261 6365 7320 6f66 2064  e 2D traces of d
+0000fb00: 6169 6c79 2f68 6f75 726c 7920 6372 6f73  aily/hourly cros
+0000fb10: 732d 636f 7272 656c 6174 696f 6e20 6675  s-correlation fu
+0000fb20: 6e63 7469 6f6e 730a 2020 2020 673a 2061  nctions.    g: a
+0000fb30: 2070 6f73 6974 6976 6520 6e75 6d62 6572   positive number
+0000fb40: 2074 6f20 6164 6a75 7374 2074 6865 2066   to adjust the f
+0000fb50: 696c 7465 7220 6861 7273 686e 6573 730a  ilter harshness.
+0000fb60: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+0000fb70: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000fb80: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e61 7272  -------.    narr
+0000fb90: 3a20 6e75 6d70 7920 7665 6374 6f72 2063  : numpy vector c
+0000fba0: 6f6e 7461 696e 7320 7468 6520 7374 6163  ontains the stac
+0000fbb0: 6b65 6420 6372 6f73 7320 636f 7272 656c  ked cross correl
+0000fbc0: 6174 696f 6e20 6675 6e63 7469 6f6e 0a20  ation function. 
+0000fbd0: 2020 2022 2222 0a20 2020 2069 6620 6172     """.    if ar
+0000fbe0: 722e 6e64 696d 203d 3d20 313a 0a20 2020  r.ndim == 1:.   
+0000fbf0: 2020 2020 2072 6574 7572 6e20 6172 720a       return arr.
+0000fc00: 2020 2020 4e2c 204d 203d 2061 7272 2e73      N, M = arr.s
+0000fc10: 6861 7065 0a20 2020 204e 6666 7420 3d20  hape.    Nfft = 
+0000fc20: 6e65 7874 5f66 6173 745f 6c65 6e28 4d29  next_fast_len(M)
+0000fc30: 0a0a 2020 2020 2320 6666 7420 7468 6520  ..    # fft the 
+0000fc40: 3244 2061 7272 6179 0a20 2020 2073 7065  2D array.    spe
+0000fc50: 6320 3d20 7363 6970 792e 6666 7470 6163  c = scipy.fftpac
+0000fc60: 6b2e 6666 7428 6172 722c 2061 7869 733d  k.fft(arr, axis=
+0000fc70: 312c 206e 3d4e 6666 7429 5b3a 2c20 3a4d  1, n=Nfft)[:, :M
+0000fc80: 5d0a 0a20 2020 2023 206d 616b 6520 6372  ]..    # make cr
+0000fc90: 6f73 732d 7370 6563 7472 6d20 6d61 7472  oss-spectrm matr
+0000fca0: 6978 0a20 2020 2063 7370 6563 203d 206e  ix.    cspec = n
+0000fcb0: 702e 7a65 726f 7328 7368 6170 653d 284e  p.zeros(shape=(N
+0000fcc0: 202a 204e 2c20 4d29 2c20 6474 7970 653d   * N, M), dtype=
+0000fcd0: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
+0000fce0: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
+0000fcf0: 6528 4e29 3a0a 2020 2020 2020 2020 666f  e(N):.        fo
+0000fd00: 7220 6a6a 2069 6e20 7261 6e67 6528 4e29  r jj in range(N)
+0000fd10: 3a0a 2020 2020 2020 2020 2020 2020 6b6b  :.            kk
+0000fd20: 203d 2069 6920 2a20 4e20 2b20 6a6a 0a20   = ii * N + jj. 
+0000fd30: 2020 2020 2020 2020 2020 2063 7370 6563             cspec
+0000fd40: 5b6b 6b5d 203d 2073 7065 635b 6969 5d20  [kk] = spec[ii] 
+0000fd50: 2a20 6e70 2e63 6f6e 6a75 6761 7465 2873  * np.conjugate(s
+0000fd60: 7065 635b 6a6a 5d29 0a0a 2020 2020 5331  pec[jj])..    S1
+0000fd70: 203d 206e 702e 7a65 726f 7328 4d2c 2064   = np.zeros(M, d
+0000fd80: 7479 7065 3d6e 702e 636f 6d70 6c65 7836  type=np.complex6
+0000fd90: 3429 0a20 2020 2053 3220 3d20 6e70 2e7a  4).    S2 = np.z
+0000fda0: 6572 6f73 284d 2c20 6474 7970 653d 6e70  eros(M, dtype=np
+0000fdb0: 2e63 6f6d 706c 6578 3634 290a 2020 2020  .complex64).    
+0000fdc0: 2320 636f 6e73 7472 7563 7420 7468 6520  # construct the 
+0000fdd0: 6669 6c74 6572 2050 0a20 2020 2066 6f72  filter P.    for
+0000fde0: 2069 6920 696e 2072 616e 6765 284e 293a   ii in range(N):
+0000fdf0: 0a20 2020 2020 2020 206d 6d20 3d20 6969  .        mm = ii
+0000fe00: 202a 204e 202b 2069 690a 2020 2020 2020   * N + ii.      
+0000fe10: 2020 5332 202b 3d20 6373 7065 635b 6d6d    S2 += cspec[mm
+0000fe20: 5d0a 2020 2020 2020 2020 666f 7220 6a6a  ].        for jj
+0000fe30: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
+0000fe40: 2020 2020 2020 2020 2020 6b6b 203d 2069            kk = i
+0000fe50: 6920 2a20 4e20 2b20 6a6a 0a20 2020 2020  i * N + jj.     
+0000fe60: 2020 2020 2020 2053 3120 2b3d 2063 7370         S1 += csp
+0000fe70: 6563 5b6b 6b5d 0a0a 2020 2020 7020 3d20  ec[kk]..    p = 
+0000fe80: 6e70 2e70 6f77 6572 2828 5331 202d 2053  np.power((S1 - S
+0000fe90: 3229 202f 2028 5332 202a 2028 4e20 2d20  2) / (S2 * (N - 
+0000fea0: 3129 292c 2067 290a 0a20 2020 2023 206d  1)), g)..    # m
+0000feb0: 616b 6520 6966 6674 0a20 2020 206e 6172  ake ifft.    nar
+0000fec0: 7220 3d20 6e70 2e72 6561 6c28 7363 6970  r = np.real(scip
+0000fed0: 792e 6666 7470 6163 6b2e 6966 6674 286e  y.fftpack.ifft(n
+0000fee0: 702e 6d75 6c74 6970 6c79 2870 2c20 7370  p.multiply(p, sp
+0000fef0: 6563 292c 204e 6666 742c 2061 7869 733d  ec), Nfft, axis=
+0000ff00: 3129 5b3a 2c20 3a4d 5d29 0a20 2020 2072  1)[:, :M]).    r
+0000ff10: 6574 7572 6e20 6e70 2e6d 6561 6e28 6e61  eturn np.mean(na
+0000ff20: 7272 2c20 6178 6973 3d30 290a 0a0a 6465  rr, axis=0)...de
+0000ff30: 6620 7077 7328 6172 722c 2073 616d 706c  f pws(arr, sampl
+0000ff40: 696e 675f 7261 7465 2c20 706f 7765 723d  ing_rate, power=
+0000ff50: 322c 2070 7773 5f74 696d 6567 6174 653d  2, pws_timegate=
+0000ff60: 352e 3029 3a0a 2020 2020 2222 220a 2020  5.0):.    """.  
+0000ff70: 2020 5065 7266 6f72 6d73 2070 6861 7365    Performs phase
+0000ff80: 2d77 6569 6768 7465 6420 7374 6163 6b20  -weighted stack 
+0000ff90: 6f6e 2061 7272 6179 206f 6620 7469 6d65  on array of time
+0000ffa0: 2073 6572 6965 732e 204d 6f64 6966 6965   series. Modifie
+0000ffb0: 6420 6f6e 2074 6865 206e 6f69 7365 2066  d on the noise f
+0000ffc0: 756e 6374 696f 6e20 6279 2054 696d 2043  unction by Tim C
+0000ffd0: 6c69 6d65 6e74 732e 0a20 2020 2046 6f6c  liments..    Fol
+0000ffe0: 6c6f 7773 206d 6574 686f 6473 206f 6620  lows methods of 
+0000fff0: 5363 6869 6d6d 656c 2061 6e64 2050 6175  Schimmel and Pau
+00010000: 6c73 7365 6e2c 2031 3939 372e 0a20 2020  lssen, 1997..   
+00010010: 2049 6620 7328 7429 2069 7320 7469 6d65   If s(t) is time
+00010020: 2073 6572 6965 7320 6461 7461 2028 7365   series data (se
+00010030: 6973 6d6f 6772 616d 2c20 6f72 2063 726f  ismogram, or cro
+00010040: 7373 2d63 6f72 7265 6c61 7469 6f6e 292c  ss-correlation),
+00010050: 0a20 2020 2053 2874 2920 3d20 7328 7429  .    S(t) = s(t)
+00010060: 202b 2069 2a48 2873 2874 2929 2c20 7768   + i*H(s(t)), wh
+00010070: 6572 6520 4828 7328 7429 2920 6973 2048  ere H(s(t)) is H
+00010080: 696c 6265 7274 2074 7261 6e73 666f 726d  ilbert transform
+00010090: 206f 6620 7328 7429 0a20 2020 2053 2874   of s(t).    S(t
+000100a0: 2920 3d20 7328 7429 202b 2069 2a48 2873  ) = s(t) + i*H(s
+000100b0: 2874 2929 203d 2041 2874 292a 6578 7028  (t)) = A(t)*exp(
+000100c0: 692a 7068 6928 7429 292c 2077 6865 7265  i*phi(t)), where
+000100d0: 0a20 2020 2041 2874 2920 6973 2065 6e76  .    A(t) is env
+000100e0: 656c 6f70 6520 6f66 2073 2874 2920 616e  elope of s(t) an
+000100f0: 6420 7068 6928 7429 2069 7320 7068 6173  d phi(t) is phas
+00010100: 6520 6f66 2073 2874 290a 2020 2020 5068  e of s(t).    Ph
+00010110: 6173 652d 7765 6967 6874 6564 2073 7461  ase-weighted sta
+00010120: 636b 2c20 6728 7429 2c20 6973 2074 6865  ck, g(t), is the
+00010130: 6e3a 0a20 2020 2067 2874 2920 3d20 312f  n:.    g(t) = 1/
+00010140: 4e20 7375 6d20 6a20 3d20 313a 4e20 735f  N sum j = 1:N s_
+00010150: 6a28 7429 202a 207c 2031 2f4e 2073 756d  j(t) * | 1/N sum
+00010160: 206b 203d 2031 3a4e 2065 7870 5b69 202a   k = 1:N exp[i *
+00010170: 2070 6869 5f6b 2874 295d 7c5e 760a 2020   phi_k(t)]|^v.  
+00010180: 2020 7768 6572 6520 4e20 6973 206e 756d    where N is num
+00010190: 6265 7220 6f66 2074 7261 6365 7320 7573  ber of traces us
+000101a0: 6564 2c20 7620 6973 2073 6861 7270 6e65  ed, v is sharpne
+000101b0: 7373 206f 6620 7068 6173 652d 7765 6967  ss of phase-weig
+000101c0: 6874 6564 2073 7461 636b 0a0a 2020 2020  hted stack..    
+000101d0: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+000101e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000101f0: 2d2d 2d2d 2d0a 2020 2020 6172 723a 204e  -----.    arr: N
+00010200: 206c 656e 6774 6820 6172 7261 7920 6f66   length array of
+00010210: 2074 696d 6520 7365 7269 6573 2064 6174   time series dat
+00010220: 6120 286e 756d 7079 2e6e 6461 7272 6179  a (numpy.ndarray
+00010230: 290a 2020 2020 7361 6d70 6c69 6e67 5f72  ).    sampling_r
+00010240: 6174 653a 2073 616d 706c 696e 6720 7261  ate: sampling ra
+00010250: 7465 206f 6620 7469 6d65 2073 6572 6965  te of time serie
+00010260: 7320 6172 7220 2869 6e74 290a 2020 2020  s arr (int).    
+00010270: 706f 7765 723a 2065 7870 6f6e 656e 7420  power: exponent 
+00010280: 666f 7220 7068 6173 6520 7374 6163 6b20  for phase stack 
+00010290: 2869 6e74 290a 2020 2020 7077 735f 7469  (int).    pws_ti
+000102a0: 6d65 6761 7465 3a20 6e75 6d62 6572 206f  megate: number o
+000102b0: 6620 7365 636f 6e64 7320 746f 2073 6d6f  f seconds to smo
+000102c0: 6f74 6820 7068 6173 6520 7374 6163 6b20  oth phase stack 
+000102d0: 2866 6c6f 6174 290a 0a20 2020 2052 4554  (float)..    RET
+000102e0: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
+000102f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00010300: 2020 2020 7765 6967 6874 6564 3a20 5068      weighted: Ph
+00010310: 6173 6520 7765 6967 6874 6564 2073 7461  ase weighted sta
+00010320: 636b 206f 6620 7469 6d65 2073 6572 6965  ck of time serie
+00010330: 7320 6461 7461 2028 6e75 6d70 792e 6e64  s data (numpy.nd
+00010340: 6172 7261 7929 0a20 2020 2022 2222 0a0a  array).    """..
+00010350: 2020 2020 6966 2061 7272 2e6e 6469 6d20      if arr.ndim 
+00010360: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
+00010370: 7475 726e 2061 7272 0a20 2020 204e 2c20  turn arr.    N, 
+00010380: 4d20 3d20 6172 722e 7368 6170 650a 2020  M = arr.shape.  
+00010390: 2020 616e 616c 7974 6963 203d 2068 696c    analytic = hil
+000103a0: 6265 7274 2861 7272 2c20 6178 6973 3d31  bert(arr, axis=1
+000103b0: 2c20 4e3d 6e65 7874 5f66 6173 745f 6c65  , N=next_fast_le
+000103c0: 6e28 4d29 295b 3a2c 203a 4d5d 0a20 2020  n(M))[:, :M].   
+000103d0: 2070 6861 7365 203d 206e 702e 616e 676c   phase = np.angl
+000103e0: 6528 616e 616c 7974 6963 290a 2020 2020  e(analytic).    
+000103f0: 7068 6173 655f 7374 6163 6b20 3d20 6e70  phase_stack = np
+00010400: 2e6d 6561 6e28 6e70 2e65 7870 2831 6a20  .mean(np.exp(1j 
+00010410: 2a20 7068 6173 6529 2c20 6178 6973 3d30  * phase), axis=0
+00010420: 290a 2020 2020 7068 6173 655f 7374 6163  ).    phase_stac
+00010430: 6b20 3d20 6e70 2e61 6273 2870 6861 7365  k = np.abs(phase
+00010440: 5f73 7461 636b 2920 2a2a 2028 706f 7765  _stack) ** (powe
+00010450: 7229 0a0a 2020 2020 2320 736d 6f6f 7468  r)..    # smooth
+00010460: 696e 670a 2020 2020 2320 7469 6d65 6761  ing.    # timega
+00010470: 7465 5f73 616d 706c 6573 203d 2069 6e74  te_samples = int
+00010480: 2870 7773 5f74 696d 6567 6174 6520 2a20  (pws_timegate * 
+00010490: 7361 6d70 6c69 6e67 5f72 6174 6529 0a20  sampling_rate). 
+000104a0: 2020 2023 2070 6861 7365 5f73 7461 636b     # phase_stack
+000104b0: 203d 206d 6f76 696e 675f 6176 6528 7068   = moving_ave(ph
+000104c0: 6173 655f 7374 6163 6b2c 7469 6d65 6761  ase_stack,timega
+000104d0: 7465 5f73 616d 706c 6573 290a 2020 2020  te_samples).    
+000104e0: 7765 6967 6874 6564 203d 206e 702e 6d75  weighted = np.mu
+000104f0: 6c74 6970 6c79 2861 7272 2c20 7068 6173  ltiply(arr, phas
+00010500: 655f 7374 6163 6b29 0a20 2020 2072 6574  e_stack).    ret
+00010510: 7572 6e20 6e70 2e6d 6561 6e28 7765 6967  urn np.mean(weig
+00010520: 6874 6564 2c20 6178 6973 3d30 290a 0a0a  hted, axis=0)...
+00010530: 6465 6620 6e72 6f6f 745f 7374 6163 6b28  def nroot_stack(
+00010540: 6363 5f61 7272 6179 2c20 706f 7765 7229  cc_array, power)
+00010550: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+00010560: 6973 2069 7320 6e74 682d 726f 6f74 2073  is is nth-root s
+00010570: 7461 636b 696e 6720 616c 676f 7269 7468  tacking algorith
+00010580: 6d20 7472 616e 736c 6174 6564 2062 6173  m translated bas
+00010590: 6564 206f 6e20 7468 6520 6d61 746c 6162  ed on the matlab
+000105a0: 2066 756e 6374 696f 6e0a 2020 2020 6672   function.    fr
+000105b0: 6f6d 2068 7474 7073 3a2f 2f67 6974 6875  om https://githu
+000105c0: 622e 636f 6d2f 7874 7961 6e67 7073 702f  b.com/xtyangpsp/
+000105d0: 5365 6973 5374 6163 6b20 2862 7920 5869  SeisStack (by Xi
+000105e0: 616f 7461 6f20 5961 6e67 3b20 666f 6c6c  aotao Yang; foll
+000105f0: 6f77 7320 7468 650a 2020 2020 7265 6665  ows the.    refe
+00010600: 7265 6e63 6520 6f66 204d 696c 6c65 742c  rence of Millet,
+00010610: 2046 2065 7420 616c 2e2c 2032 3031 3920   F et al., 2019 
+00010620: 4a47 5229 0a0a 2020 2020 5061 7261 6d65  JGR)..    Parame
+00010630: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
+00010640: 2d2d 2d2d 2d2d 0a20 2020 2063 635f 6172  ------.    cc_ar
+00010650: 7261 793a 206e 756d 7079 2e6e 6461 7272  ray: numpy.ndarr
+00010660: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+00010670: 3244 2063 726f 7373 2063 6f72 7265 6c61  2D cross correla
+00010680: 7469 6f6e 206d 6174 7269 780a 2020 2020  tion matrix.    
+00010690: 706f 7765 723a 206e 702e 696e 742c 206e  power: np.int, n
+000106a0: 7468 2072 6f6f 7420 666f 7220 7468 6520  th root for the 
+000106b0: 7374 6163 6b69 6e67 0a0a 2020 2020 5265  stacking..    Re
+000106c0: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
+000106d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e73 7461  -------.    nsta
+000106e0: 636b 3a20 6e70 2e6e 6461 7272 6179 2c20  ck: np.ndarray, 
+000106f0: 6669 6e61 6c20 7374 6163 6b65 6420 7761  final stacked wa
+00010700: 7665 666f 726d 730a 0a20 2020 2057 7269  veforms..    Wri
+00010710: 7474 656e 2062 7920 4368 656e 6778 696e  tten by Chengxin
+00010720: 204a 6961 6e67 2040 414e 5520 284d 6179   Jiang @ANU (May
+00010730: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
+00010740: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
+00010750: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+00010760: 206c 6f67 6765 722e 6465 6275 6728 2232   logger.debug("2
+00010770: 4420 6d61 7472 6978 2069 7320 6e65 6564  D matrix is need
+00010780: 6564 2066 6f72 206e 726f 6f74 5f73 7461  ed for nroot_sta
+00010790: 636b 2229 0a20 2020 2020 2020 2072 6574  ck").        ret
+000107a0: 7572 6e20 6363 5f61 7272 6179 0a20 2020  urn cc_array.   
+000107b0: 204e 2c20 4d20 3d20 6363 5f61 7272 6179   N, M = cc_array
+000107c0: 2e73 6861 7065 0a20 2020 2064 6f75 7420  .shape.    dout 
+000107d0: 3d20 6e70 2e7a 6572 6f73 284d 2c20 6474  = np.zeros(M, dt
+000107e0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
+000107f0: 0a20 2020 2023 2063 6f6e 7374 7275 6374  .    # construct
+00010800: 2079 0a20 2020 2066 6f72 2069 6920 696e   y.    for ii in
+00010810: 2072 616e 6765 284e 293a 0a20 2020 2020   range(N):.     
+00010820: 2020 2064 6174 203d 2063 635f 6172 7261     dat = cc_arra
+00010830: 795b 6969 2c20 3a5d 0a20 2020 2020 2020  y[ii, :].       
+00010840: 2064 6f75 7420 2b3d 206e 702e 7369 676e   dout += np.sign
+00010850: 2864 6174 2920 2a20 6e70 2e61 6273 2864  (dat) * np.abs(d
+00010860: 6174 2920 2a2a 2028 3120 2f20 706f 7765  at) ** (1 / powe
+00010870: 7229 0a20 2020 2064 6f75 7420 2f3d 204e  r).    dout /= N
+00010880: 0a0a 2020 2020 2320 7468 6520 6669 6e61  ..    # the fina
+00010890: 6c20 7374 6163 6b65 6420 7761 7665 666f  l stacked wavefo
+000108a0: 726d 0a20 2020 206e 7374 6163 6b20 3d20  rm.    nstack = 
+000108b0: 646f 7574 202a 206e 702e 6162 7328 646f  dout * np.abs(do
+000108c0: 7574 2920 2a2a 2028 706f 7765 7220 2d20  ut) ** (power - 
+000108d0: 3129 0a0a 2020 2020 7265 7475 726e 206e  1)..    return n
+000108e0: 7374 6163 6b0a 0a0a 6465 6620 7365 6c65  stack...def sele
+000108f0: 6374 6976 655f 7374 6163 6b28 6363 5f61  ctive_stack(cc_a
+00010900: 7272 6179 2c20 6570 7369 6c6f 6e2c 2063  rray, epsilon, c
+00010910: 635f 7468 293a 2020 2320 6e6f 7161 3a20  c_th):  # noqa: 
+00010920: 4638 3131 0a20 2020 2022 2222 0a20 2020  F811.    """.   
+00010930: 2074 6869 7320 6973 2061 2073 656c 6563   this is a selec
+00010940: 7469 7665 2073 7461 636b 696e 6720 616c  tive stacking al
+00010950: 676f 7269 7468 6d20 6465 7665 6c6f 7065  gorithm develope
+00010960: 6420 6279 204a 6172 6564 2042 7279 616e  d by Jared Bryan
+00010970: 2f4b 7572 616d 6120 4f6b 7562 6f2e 0a0a  /Kurama Okubo...
+00010980: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+00010990: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+000109a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
+000109b0: 635f 6172 7261 793a 206e 756d 7079 2e6e  c_array: numpy.n
+000109c0: 6461 7272 6179 2063 6f6e 7461 696e 7320  darray contains 
+000109d0: 7468 6520 3244 2063 726f 7373 2063 6f72  the 2D cross cor
+000109e0: 7265 6c61 7469 6f6e 206d 6174 7269 780a  relation matrix.
+000109f0: 2020 2020 6570 7369 6c6f 6e3a 2072 6573      epsilon: res
+00010a00: 6964 7561 6c20 7468 7265 686f 6c64 2074  idual threhold t
+00010a10: 6f20 7175 6974 2074 6865 2069 7465 7261  o quit the itera
+00010a20: 7469 6f6e 0a20 2020 2063 635f 7468 3a20  tion.    cc_th: 
+00010a30: 6e75 6d70 792e 666c 6f61 742c 2074 6872  numpy.float, thr
+00010a40: 6573 686f 6c64 206f 6620 636f 7272 656c  eshold of correl
+00010a50: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
+00010a60: 7420 746f 2062 6520 7365 6c65 6374 6564  t to be selected
+00010a70: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
+00010a80: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00010a90: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6e65  ---------.    ne
+00010aa0: 7773 7461 636b 3a20 6e75 6d70 7920 7665  wstack: numpy ve
+00010ab0: 6374 6f72 2063 6f6e 7461 696e 7320 7468  ctor contains th
+00010ac0: 6520 7374 6163 6b65 6420 6372 6f73 7320  e stacked cross 
+00010ad0: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
+00010ae0: 6e73 7465 703a 206e 702e 696e 742c 2074  nstep: np.int, t
+00010af0: 6f74 616c 206e 756d 6265 7220 6f66 2069  otal number of i
+00010b00: 7465 7261 7469 6f6e 7320 666f 7220 7468  terations for th
+00010b10: 6520 7374 6163 6b69 6e67 0a0a 2020 2020  e stacking..    
+00010b20: 4f72 6967 696e 616c 6c79 2072 6974 7465  Originally ritte
+00010b30: 6e20 6279 204d 6172 696e 6520 4465 6e6f  n by Marine Deno
+00010b40: 6c6c 650a 2020 2020 4d6f 6469 6669 6564  lle.    Modified
+00010b50: 2062 7920 4368 656e 6778 696e 204a 6961   by Chengxin Jia
+00010b60: 6e67 2040 4861 7276 6172 6420 284f 6374  ng @Harvard (Oct
+00010b70: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
+00010b80: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
+00010b90: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+00010ba0: 206c 6f67 6765 722e 6465 6275 6728 2232   logger.debug("2
+00010bb0: 4420 6d61 7472 6978 2069 7320 6e65 6564  D matrix is need
+00010bc0: 6564 2066 6f72 206e 726f 6f74 5f73 7461  ed for nroot_sta
+00010bd0: 636b 2229 0a20 2020 2020 2020 2072 6574  ck").        ret
+00010be0: 7572 6e20 6363 5f61 7272 6179 0a20 2020  urn cc_array.   
+00010bf0: 204e 2c20 4d20 3d20 6363 5f61 7272 6179   N, M = cc_array
+00010c00: 2e73 6861 7065 0a0a 2020 2020 7265 7320  .shape..    res 
+00010c10: 3d20 3965 3920 2023 2072 6573 6964 7561  = 9e9  # residua
+00010c20: 6c73 0a20 2020 2063 6f66 203d 206e 702e  ls.    cof = np.
+00010c30: 7a65 726f 7328 4e2c 2064 7479 7065 3d6e  zeros(N, dtype=n
+00010c40: 702e 666c 6f61 7433 3229 0a20 2020 206e  p.float32).    n
+00010c50: 6577 7374 6163 6b20 3d20 6e70 2e6d 6561  ewstack = np.mea
+00010c60: 6e28 6363 5f61 7272 6179 2c20 6178 6973  n(cc_array, axis
+00010c70: 3d30 290a 0a20 2020 206e 7374 6570 203d  =0)..    nstep =
+00010c80: 2030 0a20 2020 2023 2073 7461 7274 2069   0.    # start i
+00010c90: 7465 7261 7469 6f6e 0a20 2020 2077 6869  teration.    whi
+00010ca0: 6c65 2072 6573 203e 2065 7073 696c 6f6e  le res > epsilon
+00010cb0: 3a0a 2020 2020 2020 2020 666f 7220 6969  :.        for ii
+00010cc0: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
+00010cd0: 2020 2020 2020 2020 2020 636f 665b 6969            cof[ii
+00010ce0: 5d20 3d20 6e70 2e63 6f72 7263 6f65 6628  ] = np.corrcoef(
+00010cf0: 6e65 7773 7461 636b 2c20 6363 5f61 7272  newstack, cc_arr
+00010d00: 6179 5b69 692c 203a 5d29 5b30 2c20 315d  ay[ii, :])[0, 1]
+00010d10: 0a0a 2020 2020 2020 2020 2320 6669 6e64  ..        # find
+00010d20: 2067 6f6f 6420 7761 7665 666f 726d 730a   good waveforms.
+00010d30: 2020 2020 2020 2020 696e 6478 203d 206e          indx = n
+00010d40: 702e 7768 6572 6528 636f 6620 3e3d 2063  p.where(cof >= c
+00010d50: 635f 7468 295b 305d 0a20 2020 2020 2020  c_th)[0].       
+00010d60: 2069 6620 6e6f 7420 6c65 6e28 696e 6478   if not len(indx
+00010d70: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00010d80: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00010d90: 2263 616e 6e6f 7420 6669 6e64 2067 6f6f  "cannot find goo
+00010da0: 6420 7761 7665 666f 726d 7320 696e 7369  d waveforms insi
+00010db0: 6465 2073 656c 6563 7469 7665 2073 7461  de selective sta
+00010dc0: 636b 696e 6722 290a 2020 2020 2020 2020  cking").        
+00010dd0: 6f6c 6473 7461 636b 203d 206e 6577 7374  oldstack = newst
+00010de0: 6163 6b0a 2020 2020 2020 2020 6e65 7773  ack.        news
+00010df0: 7461 636b 203d 206e 702e 6d65 616e 2863  tack = np.mean(c
+00010e00: 635f 6172 7261 795b 696e 6478 5d2c 2061  c_array[indx], a
+00010e10: 7869 733d 3029 0a20 2020 2020 2020 2072  xis=0).        r
+00010e20: 6573 203d 206e 702e 6c69 6e61 6c67 2e6e  es = np.linalg.n
+00010e30: 6f72 6d28 6e65 7773 7461 636b 202d 206f  orm(newstack - o
+00010e40: 6c64 7374 6163 6b29 202f 2028 6e70 2e6c  ldstack) / (np.l
+00010e50: 696e 616c 672e 6e6f 726d 286e 6577 7374  inalg.norm(newst
+00010e60: 6163 6b29 202a 204d 290a 2020 2020 2020  ack) * M).      
+00010e70: 2020 6e73 7465 7020 2b3d 2031 0a0a 2020    nstep += 1..  
+00010e80: 2020 7265 7475 726e 206e 6577 7374 6163    return newstac
+00010e90: 6b2c 206e 7374 6570 0a0a 0a64 6566 2067  k, nstep...def g
+00010ea0: 6574 5f63 6328 7331 2c20 735f 7265 6629  et_cc(s1, s_ref)
+00010eb0: 3a0a 2020 2020 2320 7265 7475 726e 7320  :.    # returns 
+00010ec0: 7468 6520 636f 7272 656c 6174 696f 6e20  the correlation 
+00010ed0: 636f 6566 6669 6369 656e 7420 6265 7477  coefficient betw
+00010ee0: 6565 6e20 7761 7665 666f 726d 7320 696e  een waveforms in
+00010ef0: 2073 3120 6167 6169 6e73 7420 7265 6665   s1 against refe
+00010f00: 7265 6e63 650a 2020 2020 2320 7761 7665  rence.    # wave
+00010f10: 666f 726d 2073 5f72 6566 2e0a 2020 2020  form s_ref..    
+00010f20: 230a 2020 2020 6363 203d 206e 702e 7a65  #.    cc = np.ze
+00010f30: 726f 7328 7331 2e73 6861 7065 5b30 5d29  ros(s1.shape[0])
+00010f40: 0a20 2020 2073 5f72 6566 5f6e 6f72 6d20  .    s_ref_norm 
+00010f50: 3d20 6e70 2e6c 696e 616c 672e 6e6f 726d  = np.linalg.norm
+00010f60: 2873 5f72 6566 290a 2020 2020 666f 7220  (s_ref).    for 
+00010f70: 6920 696e 2072 616e 6765 2873 312e 7368  i in range(s1.sh
+00010f80: 6170 655b 305d 293a 0a20 2020 2020 2020  ape[0]):.       
+00010f90: 2063 635b 695d 203d 206e 702e 7375 6d28   cc[i] = np.sum(
+00010fa0: 6e70 2e6d 756c 7469 706c 7928 7331 5b69  np.multiply(s1[i
+00010fb0: 2c20 3a5d 2c20 735f 7265 6629 2920 2f20  , :], s_ref)) / 
+00010fc0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2873  np.linalg.norm(s
+00010fd0: 315b 692c 203a 5d29 202f 2073 5f72 6566  1[i, :]) / s_ref
+00010fe0: 5f6e 6f72 6d0a 2020 2020 7265 7475 726e  _norm.    return
+00010ff0: 2063 630a 0a0a 2323 2323 2323 2323 2323   cc...##########
 00011000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00011010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011020: 2323 0a23 2323 2323 2323 2323 2323 2323  ##.#############
-00011030: 2323 2320 4d4f 4e49 544f 5249 4e47 2046  ### MONITORING F
-00011040: 554e 4354 494f 4e53 2023 2323 2323 2323  UNCTIONS #######
-00011050: 2323 2323 2323 2323 2323 230a 2323 2323  ###########.####
-00011060: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00011020: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
+00011030: 2323 2323 2323 2323 2323 2323 2323 2320  ############### 
+00011040: 4d4f 4e49 544f 5249 4e47 2046 554e 4354  MONITORING FUNCT
+00011050: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
+00011060: 2323 2323 2323 230a 2323 2323 2323 2323  #######.########
 00011070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00011080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011090: 2323 2323 0a0a 2222 220a 6120 636f 6d70  ####..""".a comp
-000110a0: 696c 6174 696f 6e20 6f66 2061 6c6c 2061  ilation of all a
-000110b0: 7661 696c 6162 6c65 2063 6f72 6520 6675  vailable core fu
-000110c0: 6e63 7469 6f6e 7320 666f 7220 636f 6d70  nctions for comp
-000110d0: 7574 696e 6720 7068 6173 6520 6465 6c61  uting phase dela
-000110e0: 7973 2062 6173 6564 206f 6e20 616d 6269  ys based on ambi
-000110f0: 656e 7420 6e6f 6973 6520 696e 7465 7266  ent noise interf
-00011100: 6572 6f6d 6574 7279 0a0a 7175 6963 6b20  erometry..quick 
-00011110: 696e 6465 7820 6f66 2064 762f 7620 6d65  index of dv/v me
-00011120: 7468 6f64 733a 0a31 2920 7374 7265 7463  thods:.1) stretc
-00011130: 6869 6e67 2028 7469 6d65 2073 7472 6574  hing (time stret
-00011140: 6368 696e 673b 2057 6561 7665 7220 6574  ching; Weaver et
-00011150: 2061 6c20 2832 3031 3129 290a 3229 2064   al (2011)).2) d
-00011160: 7477 5f64 7676 2028 4479 6e61 6d69 6320  tw_dvv (Dynamic 
-00011170: 5469 6d65 2057 6172 7069 6e67 3b20 4d69  Time Warping; Mi
-00011180: 6b65 7365 6c6c 2065 7420 616c 2e20 3230  kesell et al. 20
-00011190: 3135 290a 3329 206d 7763 735f 6476 7620  15).3) mwcs_dvv 
-000111a0: 284d 6f76 696e 6720 5769 6e64 6f77 2043  (Moving Window C
-000111b0: 726f 7373 2053 7065 6374 7275 6d3b 2043  ross Spectrum; C
-000111c0: 6c61 726b 2065 7420 616c 2e2c 2032 3031  lark et al., 201
-000111d0: 3129 0a34 2920 6d77 6363 5f64 7676 2028  1).4) mwcc_dvv (
-000111e0: 4d6f 7669 6e67 2057 696e 646f 7720 4372  Moving Window Cr
-000111f0: 6f73 7320 436f 7272 656c 6174 696f 6e3b  oss Correlation;
-00011200: 2053 6e69 6564 6572 2065 7420 616c 2e2c   Snieder et al.,
-00011210: 2032 3031 3229 0a35 2920 7774 735f 6476   2012).5) wts_dv
-00011220: 7620 2857 6176 656c 6574 2053 7472 6563  v (Wavelet Strec
-00011230: 6869 6e67 3b20 5975 616e 2065 7420 616c  hing; Yuan et al
-00011240: 2e2c 2069 6e20 7072 6570 290a 3629 2077  ., in prep).6) w
-00011250: 7873 5f64 7676 2028 5761 7665 6c65 7420  xs_dvv (Wavelet 
-00011260: 5872 6f73 7320 5370 6563 7472 756d 3b20  Xross Spectrum; 
-00011270: 4d61 6f20 6574 2061 6c2e 2c20 3230 3139  Mao et al., 2019
-00011280: 290a 3729 2077 6477 5f64 7676 2028 5761  ).7) wdw_dvv (Wa
-00011290: 7665 6c65 7420 4479 6e61 6d69 6320 5761  velet Dynamic Wa
-000112a0: 7270 696e 673b 2059 7561 6e20 6574 2061  rping; Yuan et a
-000112b0: 6c2e 2c20 696e 2070 7265 7029 0a22 2222  l., in prep)."""
-000112c0: 0a0a 0a64 6566 2073 7472 6574 6368 696e  ...def stretchin
-000112d0: 6728 7265 662c 2063 7572 2c20 6476 5f72  g(ref, cur, dv_r
-000112e0: 616e 6765 2c20 6e62 7472 6961 6c2c 2070  ange, nbtrial, p
-000112f0: 6172 6129 3a0a 2020 2020 2222 220a 2020  ara):.    """.  
-00011300: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00011310: 636f 6d70 6172 6573 2074 6865 2052 6566  compares the Ref
-00011320: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
-00011330: 746f 2073 7472 6574 6368 6564 2f63 6f6d  to stretched/com
-00011340: 7072 6573 7365 6420 6375 7272 656e 7420  pressed current 
-00011350: 7761 7665 666f 726d 7320 746f 2067 6574  waveforms to get
-00011360: 2074 6865 0a20 2020 2072 656c 6174 6976   the.    relativ
-00011370: 6520 7365 6973 6d69 6320 7665 6c6f 6369  e seismic veloci
-00011380: 7479 2076 6172 6961 7469 6f6e 2028 616e  ty variation (an
-00011390: 6420 6173 736f 6369 6174 6564 2065 7272  d associated err
-000113a0: 6f72 292e 0a20 2020 2049 7420 616c 736f  or)..    It also
-000113b0: 2063 6f6d 7075 7465 7320 7468 6520 636f   computes the co
-000113c0: 7272 656c 6174 696f 6e20 636f 6566 6669  rrelation coeffi
-000113d0: 6369 656e 7420 6265 7477 6565 6e20 7468  cient between th
-000113e0: 6520 5265 6665 7265 6e63 6520 7761 7665  e Reference wave
-000113f0: 666f 726d 2061 6e64 2074 6865 2063 7572  form and the cur
-00011400: 7265 6e74 2077 6176 6566 6f72 6d2e 0a0a  rent waveform...
-00011410: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-00011420: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00011430: 2d2d 2d2d 0a20 2020 2072 6566 3a20 5265  ----.    ref: Re
-00011440: 6665 7265 6e63 6520 7761 7665 666f 726d  ference waveform
-00011450: 2028 6e70 2e6e 6461 7272 6179 2c20 7369   (np.ndarray, si
-00011460: 7a65 204e 290a 2020 2020 6375 723a 2043  ze N).    cur: C
-00011470: 7572 7265 6e74 2077 6176 6566 6f72 6d20  urrent waveform 
-00011480: 286e 702e 6e64 6172 7261 792c 2073 697a  (np.ndarray, siz
-00011490: 6520 4e29 0a20 2020 2064 765f 7261 6e67  e N).    dv_rang
-000114a0: 653a 2061 6273 6f6c 7574 6520 626f 756e  e: absolute boun
-000114b0: 6420 666f 7220 7468 6520 7665 6c6f 6369  d for the veloci
-000114c0: 7479 2076 6172 6961 7469 6f6e 3b20 6578  ty variation; ex
-000114d0: 616d 706c 653a 2064 763d 302e 3033 2066  ample: dv=0.03 f
-000114e0: 6f72 205b 2d33 2c33 5d25 0a20 2020 206f  or [-3,3]%.    o
-000114f0: 6620 7265 6c61 7469 7665 2076 656c 6f63  f relative veloc
-00011500: 6974 7920 6368 616e 6765 2028 2766 6c6f  ity change ('flo
-00011510: 6174 2729 0a20 2020 206e 6274 7269 616c  at').    nbtrial
-00011520: 3a20 6e75 6d62 6572 206f 6620 7374 7265  : number of stre
-00011530: 7463 6869 6e67 2063 6f65 6666 6963 6965  tching coefficie
-00011540: 6e74 2062 6574 7765 656e 2064 766d 696e  nt between dvmin
-00011550: 2061 6e64 2064 766d 6178 2c20 6e6f 206e   and dvmax, no n
-00011560: 6565 6420 746f 2062 6520 6869 6768 6572  eed to be higher
-00011570: 2074 6861 6e20 3130 3020 2028 2766 6c6f   than 100  ('flo
-00011580: 6174 2729 0a20 2020 2070 6172 613a 2076  at').    para: v
-00011590: 6563 746f 7220 6f66 2074 6865 2069 6e64  ector of the ind
-000115a0: 6963 6573 206f 6620 7468 6520 6375 7220  ices of the cur 
-000115b0: 616e 6420 7265 6620 7769 6e64 6f77 7320  and ref windows 
-000115c0: 6f6e 2077 6963 6820 796f 7520 7761 6e74  on wich you want
-000115d0: 2074 6f20 646f 2074 6865 206d 6561 7375   to do the measu
-000115e0: 7265 6d65 6e74 730a 2020 2020 286e 702e  rements.    (np.
-000115f0: 6e64 6172 7261 792c 2073 697a 6520 746d  ndarray, size tm
-00011600: 696e 2a64 656c 7461 3a74 6d61 782a 6465  in*delta:tmax*de
-00011610: 6c74 6129 0a20 2020 2046 6f72 2065 7272  lta).    For err
-00011620: 6f72 2063 6f6d 7075 7461 7469 6f6e 2c20  or computation, 
-00011630: 7765 206e 6565 6420 7061 7261 6d65 7465  we need paramete
-00011640: 7273 3a0a 2020 2020 2020 2020 666d 696e  rs:.        fmin
-00011650: 3a20 6d69 6e69 6d75 6d20 6672 6571 7565  : minimum freque
-00011660: 6e63 7920 6f66 2074 6865 2064 6174 610a  ncy of the data.
-00011670: 2020 2020 2020 2020 666d 6178 3a20 6d61          fmax: ma
-00011680: 7869 6d75 6d20 6672 6571 7565 6e63 7920  ximum frequency 
-00011690: 6f66 2074 6865 2064 6174 610a 2020 2020  of the data.    
-000116a0: 2020 2020 746d 696e 3a20 6d69 6e69 6d75      tmin: minimu
-000116b0: 6d20 7469 6d65 2077 696e 646f 7720 7768  m time window wh
-000116c0: 6572 6520 7468 6520 6476 2f76 2069 7320  ere the dv/v is 
-000116d0: 636f 6d70 7574 6564 0a20 2020 2020 2020  computed.       
-000116e0: 2074 6d61 783a 206d 6178 696d 756d 2074   tmax: maximum t
-000116f0: 696d 6520 7769 6e64 6f77 2077 6865 7265  ime window where
-00011700: 2074 6865 2064 762f 7620 6973 2063 6f6d   the dv/v is com
-00011710: 7075 7465 640a 2020 2020 5245 5455 524e  puted.    RETURN
-00011720: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00011730: 2d2d 2d2d 2d2d 2d0a 2020 2020 6476 3a20  -------.    dv: 
-00011740: 5265 6c61 7469 7665 2076 656c 6f63 6974  Relative velocit
-00011750: 7920 6368 616e 6765 2064 762f 7620 2869  y change dv/v (i
-00011760: 6e20 2529 0a20 2020 2063 633a 2063 6f72  n %).    cc: cor
-00011770: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
-00011780: 6965 6e74 2062 6574 7765 656e 2074 6865  ient between the
-00011790: 2072 6566 6572 656e 6365 2077 6176 6566   reference wavef
-000117a0: 6f72 6d20 616e 6420 7468 6520 6265 7374  orm and the best
-000117b0: 2073 7472 6574 6368 6564 2f63 6f6d 7072   stretched/compr
-000117c0: 6573 7365 6420 6375 7272 656e 7420 7761  essed current wa
-000117d0: 7665 666f 726d 0a20 2020 2063 6470 3a20  veform.    cdp: 
-000117e0: 636f 7272 656c 6174 696f 6e20 636f 6566  correlation coef
-000117f0: 6669 6369 656e 7420 6265 7477 6565 6e20  ficient between 
-00011800: 7468 6520 7265 6665 7265 6e63 6520 7761  the reference wa
-00011810: 7665 666f 726d 2061 6e64 2074 6865 2069  veform and the i
-00011820: 6e69 7469 616c 2063 7572 7265 6e74 2077  nitial current w
-00011830: 6176 6566 6f72 6d0a 2020 2020 6572 726f  aveform.    erro
-00011840: 723a 2045 7272 6f72 7320 696e 2074 6865  r: Errors in the
-00011850: 2064 762f 7620 6d65 6173 7572 656d 656e   dv/v measuremen
-00011860: 7473 2062 6173 6564 206f 6e20 5765 6176  ts based on Weav
-00011870: 6572 2065 7420 616c 2028 3230 3131 292c  er et al (2011),
-00011880: 0a20 2020 204f 6e20 7468 6520 7072 6563  .    On the prec
-00011890: 6973 696f 6e20 6f66 206e 6f69 7365 2d63  ision of noise-c
-000118a0: 6f72 7265 6c61 7469 6f6e 2069 6e74 6572  orrelation inter
-000118b0: 6665 726f 6d65 7472 792c 2047 656f 7068  ferometry, Geoph
-000118c0: 7973 2e20 4a2e 2049 6e74 2e2c 2031 3835  ys. J. Int., 185
-000118d0: 2833 290a 0a20 2020 204e 6f74 653a 2054  (3)..    Note: T
-000118e0: 6865 2063 6f64 6520 6669 7273 7420 6669  he code first fi
-000118f0: 6e64 7320 7468 6520 6265 7374 2063 6f72  nds the best cor
-00011900: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
-00011910: 6965 6e74 2062 6574 7765 656e 2074 6865  ient between the
-00011920: 2052 6566 6572 656e 6365 2077 6176 6566   Reference wavef
-00011930: 6f72 6d20 616e 640a 2020 2020 7468 6520  orm and.    the 
-00011940: 7374 7265 7463 6865 642f 636f 6d70 7265  stretched/compre
-00011950: 7373 6564 2063 7572 7265 6e74 2077 6176  ssed current wav
-00011960: 6566 6f72 6d20 616d 6f6e 6720 7468 6520  eform among the 
-00011970: 226e 6274 7269 616c 2220 7661 6c75 6573  "nbtrial" values
-00011980: 2e0a 2020 2020 4120 7265 6669 6e65 6420  ..    A refined 
-00011990: 616e 616c 7973 6973 2069 7320 7468 656e  analysis is then
-000119a0: 2070 6572 666f 726d 6564 2061 726f 756e   performed aroun
-000119b0: 6420 7468 6973 2076 616c 7565 2074 6f20  d this value to 
-000119c0: 6f62 7461 696e 2061 206d 6f72 6520 7072  obtain a more pr
-000119d0: 6563 6973 6520 6476 2f76 206d 6561 7375  ecise dv/v measu
-000119e0: 7265 6d65 6e74 202e 0a0a 2020 2020 4f72  rement ...    Or
-000119f0: 6967 696e 616c 6c79 2062 7920 4c2e 2056  iginally by L. V
-00011a00: 6965 6e73 2030 342f 3236 2f32 3031 3820  iens 04/26/2018 
-00011a10: 2856 6965 6e73 2065 7420 616c 2e2c 2032  (Viens et al., 2
-00011a20: 3031 3820 4a47 5229 0a20 2020 206d 6f64  018 JGR).    mod
-00011a30: 6966 6965 6420 6279 2043 6865 6e67 7869  ified by Chengxi
-00011a40: 6e20 4a69 616e 670a 2020 2020 2222 220a  n Jiang.    """.
-00011a50: 2020 2020 2320 6c6f 6164 2063 6f6d 6d6f      # load commo
-00011a60: 6e20 7661 7269 6162 6c65 7320 6672 6f6d  n variables from
-00011a70: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
-00011a80: 7477 696e 203d 2070 6172 615b 2274 7769  twin = para["twi
-00011a90: 6e22 5d0a 2020 2020 6672 6571 203d 2070  n"].    freq = p
-00011aa0: 6172 615b 2266 7265 7122 5d0a 2020 2020  ara["freq"].    
-00011ab0: 6474 203d 2070 6172 615b 2264 7422 5d0a  dt = para["dt"].
-00011ac0: 2020 2020 746d 696e 203d 206e 702e 6d69      tmin = np.mi
-00011ad0: 6e28 7477 696e 290a 2020 2020 746d 6178  n(twin).    tmax
-00011ae0: 203d 206e 702e 6d61 7828 7477 696e 290a   = np.max(twin).
-00011af0: 2020 2020 666d 696e 203d 206e 702e 6d69      fmin = np.mi
-00011b00: 6e28 6672 6571 290a 2020 2020 666d 6178  n(freq).    fmax
-00011b10: 203d 206e 702e 6d61 7828 6672 6571 290a   = np.max(freq).
-00011b20: 2020 2020 7476 6563 203d 206e 702e 6172      tvec = np.ar
-00011b30: 616e 6765 2874 6d69 6e2c 2074 6d61 782c  ange(tmin, tmax,
-00011b40: 2064 7429 0a0a 2020 2020 2320 6d61 6b65   dt)..    # make
-00011b50: 2075 7365 6675 6c20 6f6e 6520 666f 7220   useful one for 
-00011b60: 6d65 6173 7572 656d 656e 7473 0a20 2020  measurements.   
-00011b70: 2064 766d 696e 203d 202d 6e70 2e61 6273   dvmin = -np.abs
-00011b80: 2864 765f 7261 6e67 6529 0a20 2020 2064  (dv_range).    d
-00011b90: 766d 6178 203d 206e 702e 6162 7328 6476  vmax = np.abs(dv
-00011ba0: 5f72 616e 6765 290a 2020 2020 4570 7320  _range).    Eps 
-00011bb0: 3d20 3120 2b20 286e 702e 6c69 6e73 7061  = 1 + (np.linspa
-00011bc0: 6365 2864 766d 696e 2c20 6476 6d61 782c  ce(dvmin, dvmax,
-00011bd0: 206e 6274 7269 616c 2929 0a20 2020 2063   nbtrial)).    c
-00011be0: 6f66 203d 206e 702e 7a65 726f 7328 4570  of = np.zeros(Ep
-00011bf0: 732e 7368 6170 652c 2064 7479 7065 3d6e  s.shape, dtype=n
-00011c00: 702e 666c 6f61 7433 3229 0a0a 2020 2020  p.float32)..    
-00011c10: 2320 5365 7420 6f66 2073 7472 6574 6368  # Set of stretch
-00011c20: 6564 2f63 6f6d 7072 6573 7365 6420 6375  ed/compressed cu
-00011c30: 7272 656e 7420 7761 7665 666f 726d 730a  rrent waveforms.
-00011c40: 2020 2020 666f 7220 6969 2069 6e20 7261      for ii in ra
-00011c50: 6e67 6528 6c65 6e28 4570 7329 293a 0a20  nge(len(Eps)):. 
-00011c60: 2020 2020 2020 206e 7420 3d20 7476 6563         nt = tvec
-00011c70: 202a 2045 7073 5b69 695d 0a20 2020 2020   * Eps[ii].     
-00011c80: 2020 2073 203d 206e 702e 696e 7465 7270     s = np.interp
-00011c90: 2878 3d74 7665 632c 2078 703d 6e74 2c20  (x=tvec, xp=nt, 
-00011ca0: 6670 3d63 7572 290a 2020 2020 2020 2020  fp=cur).        
-00011cb0: 7761 7665 666f 726d 5f72 6566 203d 2072  waveform_ref = r
-00011cc0: 6566 0a20 2020 2020 2020 2077 6176 6566  ef.        wavef
-00011cd0: 6f72 6d5f 6375 7220 3d20 730a 2020 2020  orm_cur = s.    
-00011ce0: 2020 2020 636f 665b 6969 5d20 3d20 6e70      cof[ii] = np
-00011cf0: 2e63 6f72 7263 6f65 6628 7761 7665 666f  .corrcoef(wavefo
-00011d00: 726d 5f72 6566 2c20 7761 7665 666f 726d  rm_ref, waveform
-00011d10: 5f63 7572 295b 302c 2031 5d0a 0a20 2020  _cur)[0, 1]..   
-00011d20: 2063 6470 203d 206e 702e 636f 7272 636f   cdp = np.corrco
-00011d30: 6566 2863 7572 2c20 7265 6629 5b30 2c20  ef(cur, ref)[0, 
-00011d40: 315d 2020 2320 636f 7272 656c 6174 696f  1]  # correlatio
-00011d50: 6e20 636f 6566 6669 6369 656e 7420 6265  n coefficient be
-00011d60: 7477 6565 6e20 7468 6520 7265 6665 7265  tween the refere
-00011d70: 6e63 6520 616e 6420 696e 6974 6961 6c20  nce and initial 
-00011d80: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
-00011d90: 730a 0a20 2020 2023 2066 696e 6420 7468  s..    # find th
-00011da0: 6520 6d61 7869 6d75 6d20 636f 7272 656c  e maximum correl
-00011db0: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
-00011dc0: 740a 2020 2020 696d 6178 203d 206e 702e  t.    imax = np.
-00011dd0: 6e61 6e61 7267 6d61 7828 636f 6629 0a20  nanargmax(cof). 
-00011de0: 2020 2069 6620 696d 6178 203e 3d20 6c65     if imax >= le
-00011df0: 6e28 4570 7329 202d 2032 3a0a 2020 2020  n(Eps) - 2:.    
-00011e00: 2020 2020 696d 6178 203d 2069 6d61 7820      imax = imax 
-00011e10: 2d20 320a 2020 2020 6966 2069 6d61 7820  - 2.    if imax 
-00011e20: 3c3d 2032 3a0a 2020 2020 2020 2020 696d  <= 2:.        im
-00011e30: 6178 203d 2069 6d61 7820 2b20 320a 0a20  ax = imax + 2.. 
-00011e40: 2020 2023 2050 726f 6365 6564 2074 6f20     # Proceed to 
-00011e50: 7468 6520 7365 636f 6e64 2073 7465 7020  the second step 
-00011e60: 746f 2067 6574 2061 206d 6f72 6520 7072  to get a more pr
-00011e70: 6563 6973 6520 6476 2f76 206d 6561 7375  ecise dv/v measu
-00011e80: 7265 6d65 6e74 0a20 2020 2064 7466 696e  rement.    dtfin
-00011e90: 6572 203d 206e 702e 6c69 6e73 7061 6365  er = np.linspace
-00011ea0: 2845 7073 5b69 6d61 7820 2d20 325d 2c20  (Eps[imax - 2], 
-00011eb0: 4570 735b 696d 6178 202b 2032 5d2c 2031  Eps[imax + 2], 1
-00011ec0: 3030 290a 2020 2020 6e63 6f66 203d 206e  00).    ncof = n
-00011ed0: 702e 7a65 726f 7328 6474 6669 6e65 722e  p.zeros(dtfiner.
-00011ee0: 7368 6170 652c 2064 7479 7065 3d6e 702e  shape, dtype=np.
-00011ef0: 666c 6f61 7433 3229 0a20 2020 2066 6f72  float32).    for
-00011f00: 2069 6920 696e 2072 616e 6765 286c 656e   ii in range(len
-00011f10: 2864 7466 696e 6572 2929 3a0a 2020 2020  (dtfiner)):.    
-00011f20: 2020 2020 6e74 203d 2074 7665 6320 2a20      nt = tvec * 
-00011f30: 6474 6669 6e65 725b 6969 5d0a 2020 2020  dtfiner[ii].    
-00011f40: 2020 2020 7320 3d20 6e70 2e69 6e74 6572      s = np.inter
-00011f50: 7028 783d 7476 6563 2c20 7870 3d6e 742c  p(x=tvec, xp=nt,
-00011f60: 2066 703d 6375 7229 0a20 2020 2020 2020   fp=cur).       
-00011f70: 2077 6176 6566 6f72 6d5f 7265 6620 3d20   waveform_ref = 
-00011f80: 7265 660a 2020 2020 2020 2020 7761 7665  ref.        wave
-00011f90: 666f 726d 5f63 7572 203d 2073 0a20 2020  form_cur = s.   
-00011fa0: 2020 2020 206e 636f 665b 6969 5d20 3d20       ncof[ii] = 
-00011fb0: 6e70 2e63 6f72 7263 6f65 6628 7761 7665  np.corrcoef(wave
-00011fc0: 666f 726d 5f72 6566 2c20 7761 7665 666f  form_ref, wavefo
-00011fd0: 726d 5f63 7572 295b 302c 2031 5d0a 0a20  rm_cur)[0, 1].. 
-00011fe0: 2020 2063 6320 3d20 6e70 2e6d 6178 286e     cc = np.max(n
-00011ff0: 636f 6629 2020 2320 4669 6e64 206d 6178  cof)  # Find max
-00012000: 696d 756d 2063 6f72 7265 6c61 7469 6f6e  imum correlation
-00012010: 2063 6f65 6666 6963 6965 6e74 206f 6620   coefficient of 
-00012020: 7468 6520 7265 6669 6e65 6420 2061 6e61  the refined  ana
-00012030: 6c79 7369 730a 2020 2020 6476 203d 2031  lysis.    dv = 1
-00012040: 3030 2e30 202a 2064 7466 696e 6572 5b6e  00.0 * dtfiner[n
-00012050: 702e 6172 676d 6178 286e 636f 6629 5d20  p.argmax(ncof)] 
-00012060: 2d20 3130 3020 2023 204d 756c 7469 706c  - 100  # Multipl
-00012070: 7920 6279 2031 3030 2074 6f20 636f 6e76  y by 100 to conv
-00012080: 6572 7420 746f 2070 6572 6365 6e74 6167  ert to percentag
-00012090: 6520 2845 7073 696c 6f6e 203d 202d 6474  e (Epsilon = -dt
-000120a0: 2f74 203d 2064 762f 7629 0a0a 2020 2020  /t = dv/v)..    
-000120b0: 2320 4572 726f 7220 636f 6d70 7574 6174  # Error computat
-000120c0: 696f 6e20 6261 7365 6420 6f6e 2057 6561  ion based on Wea
-000120d0: 7665 7220 6574 2061 6c20 2832 3031 3129  ver et al (2011)
-000120e0: 2c20 4f6e 2074 6865 2070 7265 6369 7369  , On the precisi
-000120f0: 6f6e 206f 6620 6e6f 6973 652d 636f 7272  on of noise-corr
-00012100: 656c 6174 696f 6e0a 2020 2020 2320 696e  elation.    # in
-00012110: 7465 7266 6572 6f6d 6574 7279 2c20 4765  terferometry, Ge
-00012120: 6f70 6879 732e 204a 2e20 496e 742e 2c20  ophys. J. Int., 
-00012130: 3138 3528 3329 0a20 2020 2054 203d 2031  185(3).    T = 1
-00012140: 202f 2028 666d 6178 202d 2066 6d69 6e29   / (fmax - fmin)
-00012150: 0a20 2020 2058 203d 2063 630a 2020 2020  .    X = cc.    
-00012160: 7763 203d 206e 702e 7069 202a 2028 666d  wc = np.pi * (fm
-00012170: 696e 202b 2066 6d61 7829 0a20 2020 2074  in + fmax).    t
-00012180: 3120 3d20 6e70 2e6d 696e 285b 746d 696e  1 = np.min([tmin
-00012190: 2c20 746d 6178 5d29 0a20 2020 2074 3220  , tmax]).    t2 
-000121a0: 3d20 6e70 2e6d 6178 285b 746d 696e 2c20  = np.max([tmin, 
-000121b0: 746d 6178 5d29 0a20 2020 2065 7272 6f72  tmax]).    error
-000121c0: 203d 2031 3030 202a 2028 0a20 2020 2020   = 100 * (.     
-000121d0: 2020 206e 702e 7371 7274 2831 202d 2058     np.sqrt(1 - X
-000121e0: 2a2a 3229 202f 2028 3220 2a20 5829 202a  **2) / (2 * X) *
-000121f0: 206e 702e 7371 7274 2828 3620 2a20 6e70   np.sqrt((6 * np
-00012200: 2e73 7172 7428 6e70 2e70 6920 2f20 3229  .sqrt(np.pi / 2)
-00012210: 202a 2054 2920 2f20 2877 632a 2a32 202a   * T) / (wc**2 *
-00012220: 2028 7432 2a2a 3320 2d20 7431 2a2a 3329   (t2**3 - t1**3)
-00012230: 2929 0a20 2020 2029 0a0a 2020 2020 7265  )).    )..    re
-00012240: 7475 726e 2064 762c 2065 7272 6f72 2c20  turn dv, error, 
-00012250: 6363 2c20 6364 700a 0a0a 6465 6620 7374  cc, cdp...def st
-00012260: 7265 7463 6869 6e67 5f76 6563 7428 7265  retching_vect(re
-00012270: 662c 2063 7572 2c20 6476 5f72 616e 6765  f, cur, dv_range
-00012280: 2c20 6e62 7472 6961 6c2c 2070 6172 6129  , nbtrial, para)
-00012290: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-000122a0: 6973 2066 756e 6374 696f 6e20 636f 6d70  is function comp
-000122b0: 6172 6573 2074 6865 2052 6566 6572 656e  ares the Referen
-000122c0: 6365 2077 6176 6566 6f72 6d20 746f 2073  ce waveform to s
-000122d0: 7472 6574 6368 6564 2f63 6f6d 7072 6573  tretched/compres
-000122e0: 7365 6420 6375 7272 656e 7420 7761 7665  sed current wave
-000122f0: 666f 726d 730a 2020 2020 746f 2067 6574  forms.    to get
-00012300: 2074 6865 2072 656c 6174 6976 6520 7365   the relative se
-00012310: 6973 6d69 6320 7665 6c6f 6369 7479 2076  ismic velocity v
-00012320: 6172 6961 7469 6f6e 2028 616e 6420 6173  ariation (and as
-00012330: 736f 6369 6174 6564 2065 7272 6f72 292e  sociated error).
-00012340: 0a20 2020 2049 7420 616c 736f 2063 6f6d  .    It also com
-00012350: 7075 7465 7320 7468 6520 636f 7272 656c  putes the correl
-00012360: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
-00012370: 7420 6265 7477 6565 6e20 7468 6520 5265  t between the Re
-00012380: 6665 7265 6e63 6520 7761 7665 666f 726d  ference waveform
-00012390: 2061 6e64 2074 6865 2063 7572 7265 6e74   and the current
-000123a0: 2077 6176 6566 6f72 6d2e 0a0a 2020 2020   waveform...    
-000123b0: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
-000123c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000123d0: 0a20 2020 2072 6566 3a20 5265 6665 7265  .    ref: Refere
-000123e0: 6e63 6520 7761 7665 666f 726d 2028 6e70  nce waveform (np
-000123f0: 2e6e 6461 7272 6179 2c20 7369 7a65 204e  .ndarray, size N
-00012400: 290a 2020 2020 6375 723a 2043 7572 7265  ).    cur: Curre
-00012410: 6e74 2077 6176 6566 6f72 6d20 286e 702e  nt waveform (np.
-00012420: 6e64 6172 7261 792c 2073 697a 6520 4e29  ndarray, size N)
-00012430: 0a20 2020 2064 765f 7261 6e67 653a 2061  .    dv_range: a
-00012440: 6273 6f6c 7574 6520 626f 756e 6420 666f  bsolute bound fo
-00012450: 7220 7468 6520 7665 6c6f 6369 7479 2076  r the velocity v
-00012460: 6172 6961 7469 6f6e 3b20 6578 616d 706c  ariation; exampl
-00012470: 653a 2064 763d 302e 3033 2066 6f72 205b  e: dv=0.03 for [
-00012480: 2d33 2c33 5d25 0a20 2020 206f 6620 7265  -3,3]%.    of re
-00012490: 6c61 7469 7665 2076 656c 6f63 6974 7920  lative velocity 
-000124a0: 6368 616e 6765 2028 2766 6c6f 6174 2729  change ('float')
-000124b0: 0a20 2020 206e 6274 7269 616c 3a20 6e75  .    nbtrial: nu
-000124c0: 6d62 6572 206f 6620 7374 7265 7463 6869  mber of stretchi
-000124d0: 6e67 2063 6f65 6666 6963 6965 6e74 2062  ng coefficient b
-000124e0: 6574 7765 656e 2064 766d 696e 2061 6e64  etween dvmin and
-000124f0: 2064 766d 6178 2c20 6e6f 206e 6565 6420   dvmax, no need 
-00012500: 746f 2062 6520 6869 6768 6572 2074 6861  to be higher tha
-00012510: 6e20 3130 3020 2028 2766 6c6f 6174 2729  n 100  ('float')
-00012520: 0a20 2020 2070 6172 613a 2076 6563 746f  .    para: vecto
-00012530: 7220 6f66 2074 6865 2069 6e64 6963 6573  r of the indices
-00012540: 206f 6620 7468 6520 6375 7220 616e 6420   of the cur and 
-00012550: 7265 6620 7769 6e64 6f77 7320 6f6e 2077  ref windows on w
-00012560: 6963 6820 796f 7520 7761 6e74 2074 6f20  ich you want to 
-00012570: 646f 2074 6865 0a20 2020 206d 6561 7375  do the.    measu
-00012580: 7265 6d65 6e74 7320 286e 702e 6e64 6172  rements (np.ndar
-00012590: 7261 792c 2073 697a 6520 746d 696e 2a64  ray, size tmin*d
-000125a0: 656c 7461 3a74 6d61 782a 6465 6c74 6129  elta:tmax*delta)
-000125b0: 0a20 2020 2046 6f72 2065 7272 6f72 2063  .    For error c
-000125c0: 6f6d 7075 7461 7469 6f6e 2c20 7765 206e  omputation, we n
-000125d0: 6565 6420 7061 7261 6d65 7465 7273 3a0a  eed parameters:.
-000125e0: 2020 2020 2020 2020 666d 696e 3a20 6d69          fmin: mi
-000125f0: 6e69 6d75 6d20 6672 6571 7565 6e63 7920  nimum frequency 
-00012600: 6f66 2074 6865 2064 6174 610a 2020 2020  of the data.    
-00012610: 2020 2020 666d 6178 3a20 6d61 7869 6d75      fmax: maximu
-00012620: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
-00012630: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
-00012640: 746d 696e 3a20 6d69 6e69 6d75 6d20 7469  tmin: minimum ti
-00012650: 6d65 2077 696e 646f 7720 7768 6572 6520  me window where 
-00012660: 7468 6520 6476 2f76 2069 7320 636f 6d70  the dv/v is comp
-00012670: 7574 6564 0a20 2020 2020 2020 2074 6d61  uted.        tma
-00012680: 783a 206d 6178 696d 756d 2074 696d 6520  x: maximum time 
-00012690: 7769 6e64 6f77 2077 6865 7265 2074 6865  window where the
-000126a0: 2064 762f 7620 6973 2063 6f6d 7075 7465   dv/v is compute
-000126b0: 640a 2020 2020 5245 5455 524e 533a 0a20  d.    RETURNS:. 
-000126c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-000126d0: 2d2d 2d0a 2020 2020 6476 3a20 5265 6c61  ---.    dv: Rela
-000126e0: 7469 7665 2076 656c 6f63 6974 7920 6368  tive velocity ch
-000126f0: 616e 6765 2064 762f 7620 2869 6e20 2529  ange dv/v (in %)
-00012700: 0a20 2020 2063 633a 2063 6f72 7265 6c61  .    cc: correla
-00012710: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
-00012720: 2062 6574 7765 656e 2074 6865 2072 6566   between the ref
-00012730: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
-00012740: 616e 6420 7468 6520 6265 7374 2073 7472  and the best str
-00012750: 6574 6368 6564 2f63 6f6d 7072 6573 7365  etched/compresse
-00012760: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
-00012770: 726d 0a20 2020 2063 6470 3a20 636f 7272  rm.    cdp: corr
-00012780: 656c 6174 696f 6e20 636f 6566 6669 6369  elation coeffici
-00012790: 656e 7420 6265 7477 6565 6e20 7468 6520  ent between the 
-000127a0: 7265 6665 7265 6e63 6520 7761 7665 666f  reference wavefo
-000127b0: 726d 2061 6e64 2074 6865 2069 6e69 7469  rm and the initi
-000127c0: 616c 2063 7572 7265 6e74 2077 6176 6566  al current wavef
-000127d0: 6f72 6d0a 2020 2020 6572 726f 723a 2045  orm.    error: E
-000127e0: 7272 6f72 7320 696e 2074 6865 2064 762f  rrors in the dv/
-000127f0: 7620 6d65 6173 7572 656d 656e 7473 2062  v measurements b
-00012800: 6173 6564 206f 6e20 5765 6176 6572 2065  ased on Weaver e
-00012810: 7420 616c 2028 3230 3131 292c 204f 6e20  t al (2011), On 
-00012820: 7468 6520 7072 6563 6973 696f 6e0a 2020  the precision.  
-00012830: 2020 6f66 206e 6f69 7365 2d63 6f72 7265    of noise-corre
-00012840: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
-00012850: 6d65 7472 792c 2047 656f 7068 7973 2e20  metry, Geophys. 
-00012860: 4a2e 2049 6e74 2e2c 2031 3835 2833 290a  J. Int., 185(3).
-00012870: 0a20 2020 204e 6f74 653a 2054 6865 2063  .    Note: The c
-00012880: 6f64 6520 6669 7273 7420 6669 6e64 7320  ode first finds 
-00012890: 7468 6520 6265 7374 2063 6f72 7265 6c61  the best correla
-000128a0: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
-000128b0: 2062 6574 7765 656e 2074 6865 2052 6566   between the Ref
-000128c0: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
-000128d0: 616e 640a 2020 2020 7468 6520 7374 7265  and.    the stre
-000128e0: 7463 6865 642f 636f 6d70 7265 7373 6564  tched/compressed
-000128f0: 2063 7572 7265 6e74 2077 6176 6566 6f72   current wavefor
-00012900: 6d20 616d 6f6e 6720 7468 6520 226e 6274  m among the "nbt
-00012910: 7269 616c 2220 7661 6c75 6573 2e0a 2020  rial" values..  
-00012920: 2020 4120 7265 6669 6e65 6420 616e 616c    A refined anal
-00012930: 7973 6973 2069 7320 7468 656e 2070 6572  ysis is then per
-00012940: 666f 726d 6564 2061 726f 756e 6420 7468  formed around th
-00012950: 6973 2076 616c 7565 2074 6f20 6f62 7461  is value to obta
-00012960: 696e 2061 206d 6f72 6520 7072 6563 6973  in a more precis
-00012970: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
-00012980: 6e74 202e 0a0a 2020 2020 4f72 6967 696e  nt ...    Origin
-00012990: 616c 6c79 2062 7920 4c2e 2056 6965 6e73  ally by L. Viens
-000129a0: 2030 342f 3236 2f32 3031 3820 2856 6965   04/26/2018 (Vie
-000129b0: 6e73 2065 7420 616c 2e2c 2032 3031 3820  ns et al., 2018 
-000129c0: 4a47 5229 0a20 2020 206d 6f64 6966 6965  JGR).    modifie
-000129d0: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
-000129e0: 616e 670a 2020 2020 6d6f 6469 6669 6564  ang.    modified
-000129f0: 2062 7920 4c61 7572 6120 4572 6d65 7274   by Laura Ermert
-00012a00: 3a20 7665 6374 6f72 697a 6564 2076 6572  : vectorized ver
-00012a10: 7369 6f6e 0a20 2020 2022 2222 0a20 2020  sion.    """.   
-00012a20: 2023 206c 6f61 6420 636f 6d6d 6f6e 2076   # load common v
-00012a30: 6172 6961 626c 6573 2066 726f 6d20 6469  ariables from di
-00012a40: 6374 696f 6e61 7279 0a20 2020 2074 7769  ctionary.    twi
-00012a50: 6e20 3d20 7061 7261 5b22 7477 696e 225d  n = para["twin"]
-00012a60: 0a20 2020 2066 7265 7120 3d20 7061 7261  .    freq = para
-00012a70: 5b22 6672 6571 225d 0a20 2020 2064 7420  ["freq"].    dt 
-00012a80: 3d20 7061 7261 5b22 6474 225d 0a20 2020  = para["dt"].   
-00012a90: 2074 6d69 6e20 3d20 6e70 2e6d 696e 2874   tmin = np.min(t
-00012aa0: 7769 6e29 0a20 2020 2074 6d61 7820 3d20  win).    tmax = 
-00012ab0: 6e70 2e6d 6178 2874 7769 6e29 0a20 2020  np.max(twin).   
-00012ac0: 2066 6d69 6e20 3d20 6e70 2e6d 696e 2866   fmin = np.min(f
-00012ad0: 7265 7129 0a20 2020 2066 6d61 7820 3d20  req).    fmax = 
-00012ae0: 6e70 2e6d 6178 2866 7265 7129 0a20 2020  np.max(freq).   
-00012af0: 2074 7665 6320 3d20 6e70 2e61 7261 6e67   tvec = np.arang
-00012b00: 6528 746d 696e 2c20 746d 6178 2c20 6474  e(tmin, tmax, dt
-00012b10: 290a 0a20 2020 2023 206d 616b 6520 7573  )..    # make us
-00012b20: 6566 756c 206f 6e65 2066 6f72 206d 6561  eful one for mea
-00012b30: 7375 7265 6d65 6e74 730a 2020 2020 6476  surements.    dv
-00012b40: 6d69 6e20 3d20 2d6e 702e 6162 7328 6476  min = -np.abs(dv
-00012b50: 5f72 616e 6765 290a 2020 2020 6476 6d61  _range).    dvma
-00012b60: 7820 3d20 6e70 2e61 6273 2864 765f 7261  x = np.abs(dv_ra
-00012b70: 6e67 6529 0a20 2020 2045 7073 203d 2031  nge).    Eps = 1
-00012b80: 202b 2028 6e70 2e6c 696e 7370 6163 6528   + (np.linspace(
-00012b90: 6476 6d69 6e2c 2064 766d 6178 2c20 6e62  dvmin, dvmax, nb
-00012ba0: 7472 6961 6c29 290a 2020 2020 6364 7020  trial)).    cdp 
-00012bb0: 3d20 6e70 2e63 6f72 7263 6f65 6628 6375  = np.corrcoef(cu
-00012bc0: 722c 2072 6566 295b 302c 2031 5d20 2023  r, ref)[0, 1]  #
-00012bd0: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
-00012be0: 6666 6963 6965 6e74 2062 6574 7765 656e  fficient between
-00012bf0: 2074 6865 2072 6566 6572 656e 6365 2061   the reference a
-00012c00: 6e64 2069 6e69 7469 616c 2063 7572 7265  nd initial curre
-00012c10: 6e74 2077 6176 6566 6f72 6d73 0a20 2020  nt waveforms.   
-00012c20: 2077 6176 6566 6f72 6d73 203d 206e 702e   waveforms = np.
-00012c30: 7a65 726f 7328 286e 6274 7269 616c 202b  zeros((nbtrial +
-00012c40: 2031 2c20 6c65 6e28 7265 6629 2929 0a20   1, len(ref))). 
-00012c50: 2020 2077 6176 6566 6f72 6d73 5b30 2c20     waveforms[0, 
-00012c60: 3a5d 203d 2072 6566 0a0a 2020 2020 2320  :] = ref..    # 
-00012c70: 5365 7420 6f66 2073 7472 6574 6368 6564  Set of stretched
-00012c80: 2f63 6f6d 7072 6573 7365 6420 6375 7272  /compressed curr
-00012c90: 656e 7420 7761 7665 666f 726d 730a 2020  ent waveforms.  
-00012ca0: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
-00012cb0: 6528 6e62 7472 6961 6c29 3a0a 2020 2020  e(nbtrial):.    
-00012cc0: 2020 2020 6e74 203d 2074 7665 6320 2a20      nt = tvec * 
-00012cd0: 4570 735b 6969 5d0a 2020 2020 2020 2020  Eps[ii].        
-00012ce0: 7320 3d20 6e70 2e69 6e74 6572 7028 783d  s = np.interp(x=
-00012cf0: 7476 6563 2c20 7870 3d6e 742c 2066 703d  tvec, xp=nt, fp=
-00012d00: 6375 7229 0a20 2020 2020 2020 2077 6176  cur).        wav
-00012d10: 6566 6f72 6d73 5b69 6920 2b20 312c 203a  eforms[ii + 1, :
-00012d20: 5d20 3d20 730a 2020 2020 636f 6620 3d20  ] = s.    cof = 
-00012d30: 6e70 2e63 6f72 7263 6f65 6628 7761 7665  np.corrcoef(wave
-00012d40: 666f 726d 7329 5b30 5d5b 313a 5d0a 0a20  forms)[0][1:].. 
-00012d50: 2020 2023 2066 696e 6420 7468 6520 6d61     # find the ma
-00012d60: 7869 6d75 6d20 636f 7272 656c 6174 696f  ximum correlatio
-00012d70: 6e20 636f 6566 6669 6369 656e 740a 2020  n coefficient.  
-00012d80: 2020 696d 6178 203d 206e 702e 6e61 6e61    imax = np.nana
-00012d90: 7267 6d61 7828 636f 6629 0a20 2020 2069  rgmax(cof).    i
-00012da0: 6620 696d 6178 203e 3d20 6c65 6e28 4570  f imax >= len(Ep
-00012db0: 7329 202d 2032 3a0a 2020 2020 2020 2020  s) - 2:.        
-00012dc0: 696d 6178 203d 2069 6d61 7820 2d20 320a  imax = imax - 2.
-00012dd0: 2020 2020 6966 2069 6d61 7820 3c20 323a      if imax < 2:
-00012de0: 0a20 2020 2020 2020 2069 6d61 7820 3d20  .        imax = 
-00012df0: 696d 6178 202b 2032 0a0a 2020 2020 2320  imax + 2..    # 
-00012e00: 5072 6f63 6565 6420 746f 2074 6865 2073  Proceed to the s
-00012e10: 6563 6f6e 6420 7374 6570 2074 6f20 6765  econd step to ge
-00012e20: 7420 6120 6d6f 7265 2070 7265 6369 7365  t a more precise
-00012e30: 2064 762f 7620 6d65 6173 7572 656d 656e   dv/v measuremen
-00012e40: 740a 2020 2020 6474 6669 6e65 7220 3d20  t.    dtfiner = 
-00012e50: 6e70 2e6c 696e 7370 6163 6528 4570 735b  np.linspace(Eps[
-00012e60: 696d 6178 202d 2032 5d2c 2045 7073 5b69  imax - 2], Eps[i
-00012e70: 6d61 7820 2b20 325d 2c20 6e62 7472 6961  max + 2], nbtria
-00012e80: 6c29 0a20 2020 2023 206e 636f 6620 2020  l).    # ncof   
-00012e90: 203d 206e 702e 7a65 726f 7328 6474 6669   = np.zeros(dtfi
-00012ea0: 6e65 722e 7368 6170 652c 6474 7970 653d  ner.shape,dtype=
-00012eb0: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
-00012ec0: 7761 7665 666f 726d 7320 3d20 6e70 2e7a  waveforms = np.z
-00012ed0: 6572 6f73 2828 6e62 7472 6961 6c20 2b20  eros((nbtrial + 
-00012ee0: 312c 206c 656e 2872 6566 2929 290a 2020  1, len(ref))).  
-00012ef0: 2020 7761 7665 666f 726d 735b 302c 203a    waveforms[0, :
-00012f00: 5d20 3d20 7265 660a 2020 2020 666f 7220  ] = ref.    for 
-00012f10: 6969 2069 6e20 7261 6e67 6528 6c65 6e28  ii in range(len(
-00012f20: 6474 6669 6e65 7229 293a 0a20 2020 2020  dtfiner)):.     
-00012f30: 2020 206e 7420 3d20 7476 6563 202a 2064     nt = tvec * d
-00012f40: 7466 696e 6572 5b69 695d 0a20 2020 2020  tfiner[ii].     
-00012f50: 2020 2073 203d 206e 702e 696e 7465 7270     s = np.interp
-00012f60: 2878 3d74 7665 632c 2078 703d 6e74 2c20  (x=tvec, xp=nt, 
-00012f70: 6670 3d63 7572 290a 2020 2020 2020 2020  fp=cur).        
-00012f80: 7761 7665 666f 726d 735b 6969 202b 2031  waveforms[ii + 1
-00012f90: 2c20 3a5d 203d 2073 0a20 2020 206e 636f  , :] = s.    nco
-00012fa0: 6620 3d20 6e70 2e63 6f72 7263 6f65 6628  f = np.corrcoef(
-00012fb0: 7761 7665 666f 726d 7329 5b30 5d5b 313a  waveforms)[0][1:
-00012fc0: 5d0a 2020 2020 6363 203d 206e 702e 6d61  ].    cc = np.ma
-00012fd0: 7828 6e63 6f66 2920 2023 2046 696e 6420  x(ncof)  # Find 
-00012fe0: 6d61 7869 6d75 6d20 636f 7272 656c 6174  maximum correlat
-00012ff0: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
-00013000: 6f66 2074 6865 2072 6566 696e 6564 2020  of the refined  
-00013010: 616e 616c 7973 6973 0a20 2020 2064 7620  analysis.    dv 
-00013020: 3d20 3130 302e 3020 2a20 6474 6669 6e65  = 100.0 * dtfine
-00013030: 725b 6e70 2e61 7267 6d61 7828 6e63 6f66  r[np.argmax(ncof
-00013040: 295d 202d 2031 3030 2020 2320 4d75 6c74  )] - 100  # Mult
-00013050: 6970 6c79 2062 7920 3130 3020 746f 2063  iply by 100 to c
-00013060: 6f6e 7665 7274 2074 6f20 7065 7263 656e  onvert to percen
-00013070: 7461 6765 2028 4570 7369 6c6f 6e20 3d20  tage (Epsilon = 
-00013080: 2d64 742f 7420 3d20 6476 2f76 290a 0a20  -dt/t = dv/v).. 
-00013090: 2020 2023 2045 7272 6f72 2063 6f6d 7075     # Error compu
-000130a0: 7461 7469 6f6e 2062 6173 6564 206f 6e20  tation based on 
-000130b0: 5765 6176 6572 2065 7420 616c 2028 3230  Weaver et al (20
-000130c0: 3131 292c 204f 6e20 7468 6520 7072 6563  11), On the prec
-000130d0: 6973 696f 6e20 6f66 206e 6f69 7365 2d63  ision of noise-c
-000130e0: 6f72 7265 6c61 7469 6f6e 2069 6e74 6572  orrelation inter
-000130f0: 6665 726f 6d65 7472 792c 0a20 2020 2023  ferometry,.    #
-00013100: 2047 656f 7068 7973 2e20 4a2e 2049 6e74   Geophys. J. Int
-00013110: 2e2c 2031 3835 2833 290a 2020 2020 5420  ., 185(3).    T 
-00013120: 3d20 3120 2f20 2866 6d61 7820 2d20 666d  = 1 / (fmax - fm
-00013130: 696e 290a 2020 2020 5820 3d20 6363 0a20  in).    X = cc. 
-00013140: 2020 2077 6320 3d20 6e70 2e70 6920 2a20     wc = np.pi * 
-00013150: 2866 6d69 6e20 2b20 666d 6178 290a 2020  (fmin + fmax).  
-00013160: 2020 7431 203d 206e 702e 6d69 6e28 5b74    t1 = np.min([t
-00013170: 6d69 6e2c 2074 6d61 785d 290a 2020 2020  min, tmax]).    
-00013180: 7432 203d 206e 702e 6d61 7828 5b74 6d69  t2 = np.max([tmi
-00013190: 6e2c 2074 6d61 785d 290a 2020 2020 6572  n, tmax]).    er
-000131a0: 726f 7220 3d20 3130 3020 2a20 280a 2020  ror = 100 * (.  
-000131b0: 2020 2020 2020 6e70 2e73 7172 7428 3120        np.sqrt(1 
-000131c0: 2d20 582a 2a32 2920 2f20 2832 202a 2058  - X**2) / (2 * X
-000131d0: 2920 2a20 6e70 2e73 7172 7428 2836 202a  ) * np.sqrt((6 *
-000131e0: 206e 702e 7371 7274 286e 702e 7069 202f   np.sqrt(np.pi /
-000131f0: 2032 2920 2a20 5429 202f 2028 7763 2a2a   2) * T) / (wc**
-00013200: 3220 2a20 2874 322a 2a33 202d 2074 312a  2 * (t2**3 - t1*
-00013210: 2a33 2929 290a 2020 2020 290a 0a20 2020  *3))).    )..   
-00013220: 2072 6574 7572 6e20 6476 2c20 6572 726f   return dv, erro
-00013230: 722c 2063 632c 2063 6470 0a0a 0a64 6566  r, cc, cdp...def
-00013240: 2064 7477 5f64 7676 2872 6566 2c20 6375   dtw_dvv(ref, cu
-00013250: 722c 2070 6172 612c 206d 6178 4c61 672c  r, para, maxLag,
-00013260: 2062 2c20 6469 7265 6374 696f 6e29 3a0a   b, direction):.
-00013270: 2020 2020 2222 220a 2020 2020 4479 6e61      """.    Dyna
-00013280: 6d69 6320 7469 6d65 2077 6172 7069 6e67  mic time warping
-00013290: 2066 6f72 2064 762f 7620 6573 7469 6d61   for dv/v estima
-000132a0: 7469 6f6e 2e0a 0a20 2020 2050 4152 414d  tion...    PARAM
-000132b0: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
-000132c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-000132d0: 7265 6620 3a20 7265 6665 7265 6e63 6520  ref : reference 
-000132e0: 7369 676e 616c 2028 6e70 2e61 7272 6179  signal (np.array
-000132f0: 2c20 7369 7a65 204e 290a 2020 2020 6375  , size N).    cu
-00013300: 7220 3a20 6375 7272 656e 7420 7369 676e  r : current sign
-00013310: 616c 2028 6e70 2e61 7272 6179 2c20 7369  al (np.array, si
-00013320: 7a65 204e 290a 2020 2020 7061 7261 3a20  ze N).    para: 
-00013330: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
-00013340: 7573 6566 756c 2070 6172 616d 6574 6572  useful parameter
-00013350: 7320 6162 6f75 7420 7468 6520 6461 7461  s about the data
-00013360: 2077 696e 646f 7720 616e 6420 7461 7267   window and targ
-00013370: 6574 6564 2066 7265 7175 656e 6379 0a20  eted frequency. 
-00013380: 2020 206d 6178 4c61 6720 3a20 6d61 7820     maxLag : max 
-00013390: 6e75 6d62 6572 206f 6620 706f 696e 7473  number of points
-000133a0: 2074 6f20 7365 6172 6368 2066 6f72 7761   to search forwa
-000133b0: 7264 2061 6e64 2062 6163 6b77 6172 642e  rd and backward.
-000133c0: 0a20 2020 2020 2020 2020 2020 2053 7567  .            Sug
-000133d0: 6765 7374 2073 6574 7469 6e67 2069 7420  gest setting it 
-000133e0: 6c61 7267 6572 2069 6620 7769 6e64 6f77  larger if window
-000133f0: 2069 7320 7365 7420 6c61 7267 6572 2e0a   is set larger..
-00013400: 2020 2020 6220 3a20 622d 7661 6c75 6520      b : b-value 
-00013410: 746f 206c 696d 6974 2073 7472 6169 6e2c  to limit strain,
-00013420: 2077 6869 6368 2069 7320 746f 206c 696d   which is to lim
-00013430: 6974 2074 6865 206d 6178 696d 756d 2076  it the maximum v
-00013440: 656c 6f63 6974 7920 7065 7274 7572 6261  elocity perturba
-00013450: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-00013460: 2020 5365 6520 6571 7561 7469 6f6e 2031    See equation 1
-00013470: 3120 696e 2028 4d69 6b65 7365 6c6c 2065  1 in (Mikesell e
-00013480: 7420 616c 2e20 3230 3135 290a 2020 2020  t al. 2015).    
-00013490: 6469 7265 6374 696f 6e3a 2064 6972 6563  direction: direc
-000134a0: 7469 6f6e 2074 6f20 6163 6375 6d75 6c61  tion to accumula
-000134b0: 7465 2065 7272 6f72 7320 2831 3d66 6f72  te errors (1=for
-000134c0: 7761 7264 2c20 2d31 3d62 6163 6b77 6172  ward, -1=backwar
-000134d0: 6429 0a20 2020 2052 4554 5552 4e53 3a0a  d).    RETURNS:.
-000134e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-000134f0: 2d2d 2d2d 2d2d 0a20 2020 202d 6d30 203a  ------.    -m0 :
-00013500: 2065 7374 696d 6174 6564 2064 762f 760a   estimated dv/v.
-00013510: 2020 2020 656d 3020 3a20 6572 726f 7220      em0 : error 
-00013520: 6f66 2064 762f 7620 6573 7469 6d61 7469  of dv/v estimati
-00013530: 6f6e 0a0a 2020 2020 4f72 6967 696e 616c  on..    Original
-00013540: 2062 7920 4469 2059 616e 670a 2020 2020   by Di Yang.    
-00013550: 4c61 7374 206d 6f64 6966 6965 6420 6279  Last modified by
-00013560: 2044 796c 616e 204d 696b 6573 656c 6c20   Dylan Mikesell 
-00013570: 2832 3520 4665 622e 2032 3031 3529 0a20  (25 Feb. 2015). 
-00013580: 2020 2054 7261 6e73 6c61 7465 6420 746f     Translated to
-00013590: 2070 7974 686f 6e20 6279 2054 696d 2043   python by Tim C
-000135a0: 6c65 6d65 6e74 7320 2831 3720 4175 672e  lements (17 Aug.
-000135b0: 2032 3031 3829 0a20 2020 2022 2222 0a20   2018).    """. 
-000135c0: 2020 2074 7769 6e20 3d20 7061 7261 5b22     twin = para["
-000135d0: 7477 696e 225d 0a20 2020 2064 7420 3d20  twin"].    dt = 
-000135e0: 7061 7261 5b22 6474 225d 0a20 2020 2074  para["dt"].    t
-000135f0: 6d69 6e20 3d20 6e70 2e6d 696e 2874 7769  min = np.min(twi
-00013600: 6e29 0a20 2020 2074 6d61 7820 3d20 6e70  n).    tmax = np
-00013610: 2e6d 6178 2874 7769 6e29 0a20 2020 2074  .max(twin).    t
-00013620: 7665 6374 203d 206e 702e 6172 616e 6765  vect = np.arange
-00013630: 2874 6d69 6e2c 2074 6d61 782c 2064 7429  (tmin, tmax, dt)
-00013640: 0a0a 2020 2020 2320 7365 7475 7020 6f74  ..    # setup ot
-00013650: 6865 7220 7061 7261 6d65 7465 7273 0a20  her parameters. 
-00013660: 2020 206e 7074 7320 3d20 6c65 6e28 7265     npts = len(re
-00013670: 6629 2020 2320 6e75 6d62 6572 206f 6620  f)  # number of 
-00013680: 7469 6d65 2073 616d 706c 6573 0a0a 2020  time samples..  
-00013690: 2020 2320 636f 6d70 7574 6520 6572 726f    # compute erro
-000136a0: 7220 6675 6e63 7469 6f6e 206f 7665 7220  r function over 
-000136b0: 6c61 6773 2c20 7768 6963 6820 6973 2069  lags, which is i
-000136c0: 6e64 6570 656e 6465 6e74 206f 6620 7374  ndependent of st
-000136d0: 7261 696e 206c 696d 6974 2027 6227 2e0a  rain limit 'b'..
-000136e0: 2020 2020 6572 7220 3d20 636f 6d70 7574      err = comput
-000136f0: 6545 7272 6f72 4675 6e63 7469 6f6e 2863  eErrorFunction(c
-00013700: 7572 2c20 7265 662c 206e 7074 732c 206d  ur, ref, npts, m
-00013710: 6178 4c61 6729 0a0a 2020 2020 2320 6469  axLag)..    # di
-00013720: 7265 6374 696f 6e20 746f 2061 6363 756d  rection to accum
-00013730: 756c 6174 6520 6572 726f 7273 2028 313d  ulate errors (1=
-00013740: 666f 7277 6172 642c 202d 313d 6261 636b  forward, -1=back
-00013750: 7761 7264 290a 2020 2020 6469 7374 203d  ward).    dist =
-00013760: 2061 6363 756d 756c 6174 6545 7272 6f72   accumulateError
-00013770: 4675 6e63 7469 6f6e 2864 6972 6563 7469  Function(directi
-00013780: 6f6e 2c20 6572 722c 206e 7074 732c 206d  on, err, npts, m
-00013790: 6178 4c61 672c 2062 290a 2020 2020 7374  axLag, b).    st
-000137a0: 6261 7220 3d20 6261 636b 7472 6163 6b44  bar = backtrackD
-000137b0: 6973 7461 6e63 6546 756e 6374 696f 6e28  istanceFunction(
-000137c0: 2d31 202a 2064 6972 6563 7469 6f6e 2c20  -1 * direction, 
-000137d0: 6469 7374 2c20 6572 722c 202d 6d61 784c  dist, err, -maxL
-000137e0: 6167 2c20 6229 0a20 2020 2073 7462 6172  ag, b).    stbar
-000137f0: 5469 6d65 203d 2073 7462 6172 202a 2064  Time = stbar * d
-00013800: 7420 2023 2063 6f6e 7665 7274 2066 726f  t  # convert fro
-00013810: 6d20 7361 6d70 6c65 7320 746f 2074 696d  m samples to tim
-00013820: 650a 0a20 2020 2023 2063 7574 2074 6865  e..    # cut the
-00013830: 2066 6972 7374 2061 6e64 206c 6173 7420   first and last 
-00013840: 3525 2066 6f72 2062 6574 7465 7220 7265  5% for better re
-00013850: 6772 6573 7369 6f6e 0a20 2020 2069 6e64  gression.    ind
-00013860: 7820 3d20 6e70 2e77 6865 7265 2828 7476  x = np.where((tv
-00013870: 6563 7420 3e3d 2030 2e30 3520 2a20 6e70  ect >= 0.05 * np
-00013880: 7473 202a 2064 7429 2026 2028 7476 6563  ts * dt) & (tvec
-00013890: 7420 3c3d 2030 2e39 3520 2a20 6e70 7473  t <= 0.95 * npts
-000138a0: 202a 2064 7429 295b 305d 0a0a 2020 2020   * dt))[0]..    
-000138b0: 2320 6c69 6e65 6172 2072 6567 7265 7373  # linear regress
-000138c0: 696f 6e20 746f 2067 6574 2064 762f 760a  ion to get dv/v.
-000138d0: 2020 2020 6966 206e 7074 7320 3e20 323a      if npts > 2:
-000138e0: 0a20 2020 2020 2020 2023 2077 6569 6768  .        # weigh
-000138f0: 7473 0a20 2020 2020 2020 2077 203d 206e  ts.        w = n
-00013900: 702e 6f6e 6573 286e 7074 7329 0a20 2020  p.ones(npts).   
-00013910: 2020 2020 2023 206d 2c20 612c 2065 6d2c       # m, a, em,
-00013920: 2065 6120 3d20 6c69 6e65 6172 5f72 6567   ea = linear_reg
-00013930: 7265 7373 696f 6e28 7469 6d65 5f61 7869  ression(time_axi
-00013940: 735b 696e 6478 5d2c 2064 656c 7461 5f74  s[indx], delta_t
-00013950: 5b69 6e64 785d 2c20 772c 2069 6e74 6572  [indx], w, inter
-00013960: 6365 7074 5f6f 7269 6769 6e3d 4661 6c73  cept_origin=Fals
-00013970: 6529 0a20 2020 2020 2020 206d 302c 2065  e).        m0, e
-00013980: 6d30 203d 206c 696e 6561 725f 7265 6772  m0 = linear_regr
-00013990: 6573 7369 6f6e 280a 2020 2020 2020 2020  ession(.        
-000139a0: 2020 2020 7476 6563 742e 666c 6174 7465      tvect.flatte
-000139b0: 6e28 295b 696e 6478 5d2c 0a20 2020 2020  n()[indx],.     
-000139c0: 2020 2020 2020 2073 7462 6172 5469 6d65         stbarTime
-000139d0: 2e66 6c61 7474 656e 2829 5b69 6e64 785d  .flatten()[indx]
-000139e0: 2c0a 2020 2020 2020 2020 2020 2020 772e  ,.            w.
-000139f0: 666c 6174 7465 6e28 295b 696e 6478 5d2c  flatten()[indx],
-00013a00: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-00013a10: 6572 6365 7074 5f6f 7269 6769 6e3d 5472  ercept_origin=Tr
-00013a20: 7565 2c0a 2020 2020 2020 2020 290a 0a20  ue,.        ).. 
-00013a30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013a40: 206c 6f67 6765 722e 6465 6275 6728 226e   logger.debug("n
-00013a50: 6f74 2065 6e6f 7567 6820 706f 696e 7473  ot enough points
-00013a60: 2074 6f20 6573 7469 6d61 7465 2064 762f   to estimate dv/
-00013a70: 7620 666f 7220 6474 7722 290a 2020 2020  v for dtw").    
-00013a80: 2020 2020 6d30 203d 2030 0a20 2020 2020      m0 = 0.     
-00013a90: 2020 2065 6d30 203d 2030 0a0a 2020 2020     em0 = 0..    
-00013aa0: 7265 7475 726e 206d 3020 2a20 3130 302c  return m0 * 100,
-00013ab0: 2065 6d30 202a 2031 3030 2c20 6469 7374   em0 * 100, dist
-00013ac0: 0a0a 0a64 6566 206d 7763 735f 6476 7628  ...def mwcs_dvv(
-00013ad0: 7265 662c 2063 7572 2c20 6d6f 7669 6e67  ref, cur, moving
-00013ae0: 5f77 696e 646f 775f 6c65 6e67 7468 2c20  _window_length, 
-00013af0: 736c 6964 655f 7374 6570 2c20 7061 7261  slide_step, para
-00013b00: 2c20 736d 6f6f 7468 696e 675f 6861 6c66  , smoothing_half
-00013b10: 5f77 696e 3d35 293a 0a20 2020 2022 2222  _win=5):.    """
-00013b20: 0a20 2020 204d 6f76 696e 6720 5769 6e64  .    Moving Wind
-00013b30: 6f77 2043 726f 7373 2053 7065 6374 7275  ow Cross Spectru
-00013b40: 6d20 6d65 7468 6f64 2074 6f20 6d65 6173  m method to meas
-00013b50: 7572 6520 6476 2f76 2028 7265 6c79 696e  ure dv/v (relyin
-00013b60: 6720 6f6e 2070 6869 3d32 2a70 692a 662a  g on phi=2*pi*f*
-00013b70: 7420 696e 2066 7265 7120 646f 6d61 696e  t in freq domain
-00013b80: 290a 0a20 2020 2050 4152 414d 4554 4552  )..    PARAMETER
-00013b90: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00013ba0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 663a  -------.    ref:
-00013bb0: 2052 6566 6572 656e 6365 2077 6176 6566   Reference wavef
-00013bc0: 6f72 6d20 286e 702e 6e64 6172 7261 792c  orm (np.ndarray,
-00013bd0: 2073 697a 6520 4e29 0a20 2020 2063 7572   size N).    cur
-00013be0: 3a20 4375 7272 656e 7420 7761 7665 666f  : Current wavefo
-00013bf0: 726d 2028 6e70 2e6e 6461 7272 6179 2c20  rm (np.ndarray, 
-00013c00: 7369 7a65 204e 290a 2020 2020 6d6f 7669  size N).    movi
-00013c10: 6e67 5f77 696e 646f 775f 6c65 6e67 7468  ng_window_length
-00013c20: 3a20 6d6f 7669 6e67 2077 696e 646f 7720  : moving window 
-00013c30: 6c65 6e67 7468 2074 6f20 6361 6c63 756c  length to calcul
-00013c40: 6174 6520 6372 6f73 732d 7370 6563 7472  ate cross-spectr
-00013c50: 756d 2028 6e70 2e66 6c6f 6174 2c20 696e  um (np.float, in
-00013c60: 2073 6563 290a 2020 2020 736c 6964 655f   sec).    slide_
-00013c70: 7374 6570 3a20 7374 6570 7320 696e 2074  step: steps in t
-00013c80: 696d 6520 746f 2073 6869 6674 2074 6865  ime to shift the
-00013c90: 206d 6f76 696e 6720 7769 6e64 6f77 2028   moving window (
-00013ca0: 6e70 2e66 6c6f 6174 2c20 696e 2073 6563  np.float, in sec
-00013cb0: 6f6e 6473 290a 2020 2020 7061 7261 3a20  onds).    para: 
-00013cc0: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
-00013cd0: 6720 7061 7261 6d65 7465 7273 2061 626f  g parameters abo
-00013ce0: 7574 2069 6e70 7574 2064 6174 6120 7769  ut input data wi
-00013cf0: 6e64 6f77 2061 6e64 2066 7265 7175 656e  ndow and frequen
-00013d00: 6379 2069 6e66 6f2c 2069 6e63 6c75 6469  cy info, includi
-00013d10: 6e67 0a20 2020 2020 2020 2064 656c 7461  ng.        delta
-00013d20: 2d3e 5468 6520 7361 6d70 6c69 6e67 2072  ->The sampling r
-00013d30: 6174 6520 6f66 2074 6865 2069 6e70 7574  ate of the input
-00013d40: 2074 696d 6573 6572 6965 7320 2869 6e20   timeseries (in 
-00013d50: 487a 290a 2020 2020 2020 2020 7769 6e64  Hz).        wind
-00013d60: 6f77 2d3e 2054 6865 2074 6172 6765 7420  ow-> The target 
-00013d70: 7769 6e64 6f77 2066 6f72 206d 6561 7375  window for measu
-00013d80: 7269 6e67 2064 742f 740a 2020 2020 2020  ring dt/t.      
-00013d90: 2020 6672 6571 2d3e 2054 6865 2066 7265    freq-> The fre
-00013da0: 7175 656e 6379 2062 6f75 6e64 2074 6f20  quency bound to 
-00013db0: 636f 6d70 7574 6520 7468 6520 6465 7068  compute the deph
-00013dc0: 6173 696e 6720 2869 6e20 487a 290a 2020  asing (in Hz).  
-00013dd0: 2020 2020 2020 746d 696e 3a20 5468 6520        tmin: The 
-00013de0: 6c65 6674 6d6f 7374 2074 696d 6520 6c61  leftmost time la
-00013df0: 6720 2875 7365 6420 746f 2063 6f6d 7075  g (used to compu
-00013e00: 7465 2074 6865 2022 7469 6d65 206c 6167  te the "time lag
-00013e10: 7320 6172 7261 7922 290a 2020 2020 736d  s array").    sm
-00013e20: 6f6f 7468 696e 675f 6861 6c66 5f77 696e  oothing_half_win
-00013e30: 3a20 4966 2064 6966 6665 7265 6e74 2066  : If different f
-00013e40: 726f 6d20 302c 2064 6566 696e 6573 2074  rom 0, defines t
-00013e50: 6865 2068 616c 6620 6c65 6e67 7468 206f  he half length o
-00013e60: 6620 7468 6520 736d 6f6f 7468 696e 6720  f the smoothing 
-00013e70: 6861 6e6e 696e 6720 7769 6e64 6f77 2e0a  hanning window..
-00013e80: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-00013e90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00013ea0: 2d2d 2d2d 0a20 2020 2074 696d 655f 6178  ----.    time_ax
-00013eb0: 6973 3a20 7468 6520 6365 6e74 7261 6c20  is: the central 
-00013ec0: 7469 6d65 7320 6f66 2074 6865 2077 696e  times of the win
-00013ed0: 646f 7773 2e0a 2020 2020 6465 6c74 615f  dows..    delta_
-00013ee0: 743a 2064 740a 2020 2020 6465 6c74 615f  t: dt.    delta_
-00013ef0: 6572 723a 6572 726f 720a 2020 2020 6465  err:error.    de
-00013f00: 6c74 615f 6d63 6f68 3a20 6d65 616e 2063  lta_mcoh: mean c
-00013f10: 6f68 6572 656e 6365 0a0a 2020 2020 436f  oherence..    Co
-00013f20: 7069 6564 2066 726f 6d20 4d53 4e6f 6973  pied from MSNois
-00013f30: 6520 2868 7474 7073 3a2f 2f67 6974 6875  e (https://githu
-00013f40: 622e 636f 6d2f 524f 4265 6c67 6975 6d2f  b.com/ROBelgium/
-00013f50: 4d53 4e6f 6973 652f 7472 6565 2f6d 6173  MSNoise/tree/mas
-00013f60: 7465 722f 6d73 6e6f 6973 6529 0a20 2020  ter/msnoise).   
-00013f70: 204d 6f64 6966 6965 6420 6279 2043 6865   Modified by Che
-00013f80: 6e67 7869 6e20 4a69 616e 670a 2020 2020  ngxin Jiang.    
-00013f90: 2222 220a 2020 2020 2320 636f 6d6d 6f6e  """.    # common
-00013fa0: 2076 6172 6961 626c 6573 0a20 2020 2074   variables.    t
-00013fb0: 7769 6e20 3d20 7061 7261 5b22 7477 696e  win = para["twin
-00013fc0: 225d 0a20 2020 2066 7265 7120 3d20 7061  "].    freq = pa
-00013fd0: 7261 5b22 6672 6571 225d 0a20 2020 2064  ra["freq"].    d
-00013fe0: 7420 3d20 7061 7261 5b22 6474 225d 0a20  t = para["dt"]. 
-00013ff0: 2020 2074 6d69 6e20 3d20 6e70 2e6d 696e     tmin = np.min
-00014000: 2874 7769 6e29 0a20 2020 2066 6d69 6e20  (twin).    fmin 
-00014010: 3d20 6e70 2e6d 696e 2866 7265 7129 0a20  = np.min(freq). 
-00014020: 2020 2066 6d61 7820 3d20 6e70 2e6d 6178     fmax = np.max
-00014030: 2866 7265 7129 0a0a 2020 2020 2320 7061  (freq)..    # pa
-00014040: 7261 6d65 7465 7220 696e 6974 6961 6c69  rameter initiali
-00014050: 7a65 0a20 2020 2064 656c 7461 5f74 203d  ze.    delta_t =
-00014060: 205b 5d0a 2020 2020 6465 6c74 615f 6572   [].    delta_er
-00014070: 7220 3d20 5b5d 0a20 2020 2064 656c 7461  r = [].    delta
-00014080: 5f6d 636f 6820 3d20 5b5d 0a20 2020 2074  _mcoh = [].    t
-00014090: 696d 655f 6178 6973 203d 205b 5d0a 0a20  ime_axis = [].. 
-000140a0: 2020 2023 2069 6e66 6f20 6f6e 2074 6865     # info on the
-000140b0: 206d 6f76 696e 6720 7769 6e64 6f77 0a20   moving window. 
-000140c0: 2020 2077 696e 646f 775f 6c65 6e67 7468     window_length
-000140d0: 5f73 616d 706c 6573 203d 206e 702e 696e  _samples = np.in
-000140e0: 7428 6d6f 7669 6e67 5f77 696e 646f 775f  t(moving_window_
-000140f0: 6c65 6e67 7468 202f 2064 7429 0a20 2020  length / dt).   
-00014100: 2070 6164 6420 3d20 696e 7428 3220 2a2a   padd = int(2 **
-00014110: 2028 6e65 7874 706f 7732 2877 696e 646f   (nextpow2(windo
-00014120: 775f 6c65 6e67 7468 5f73 616d 706c 6573  w_length_samples
-00014130: 2920 2b20 3229 290a 2020 2020 636f 756e  ) + 2)).    coun
-00014140: 7420 3d20 300a 2020 2020 7470 203d 2063  t = 0.    tp = c
-00014150: 6f73 696e 655f 7461 7065 7228 7769 6e64  osine_taper(wind
-00014160: 6f77 5f6c 656e 6774 685f 7361 6d70 6c65  ow_length_sample
-00014170: 732c 2030 2e31 3529 0a0a 2020 2020 6d69  s, 0.15)..    mi
-00014180: 6e69 6e64 203d 2030 0a20 2020 206d 6178  nind = 0.    max
-00014190: 696e 6420 3d20 7769 6e64 6f77 5f6c 656e  ind = window_len
-000141a0: 6774 685f 7361 6d70 6c65 730a 0a20 2020  gth_samples..   
-000141b0: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
-000141c0: 616c 6c20 7375 622d 7769 6e64 6f77 730a  all sub-windows.
-000141d0: 2020 2020 7768 696c 6520 6d61 7869 6e64      while maxind
-000141e0: 203c 3d20 6c65 6e28 7265 6629 3a0a 2020   <= len(ref):.  
-000141f0: 2020 2020 2020 6363 6920 3d20 6375 725b        cci = cur[
-00014200: 6d69 6e69 6e64 3a6d 6178 696e 645d 0a20  minind:maxind]. 
-00014210: 2020 2020 2020 2063 6369 203d 2073 6369         cci = sci
-00014220: 7079 2e73 6967 6e61 6c2e 6465 7472 656e  py.signal.detren
-00014230: 6428 6363 692c 2074 7970 653d 226c 696e  d(cci, type="lin
-00014240: 6561 7222 290a 2020 2020 2020 2020 6363  ear").        cc
-00014250: 6920 2a3d 2074 700a 0a20 2020 2020 2020  i *= tp..       
-00014260: 2063 7269 203d 2072 6566 5b6d 696e 696e   cri = ref[minin
-00014270: 643a 6d61 7869 6e64 5d0a 2020 2020 2020  d:maxind].      
-00014280: 2020 6372 6920 3d20 7363 6970 792e 7369    cri = scipy.si
-00014290: 676e 616c 2e64 6574 7265 6e64 2863 7269  gnal.detrend(cri
-000142a0: 2c20 7479 7065 3d22 6c69 6e65 6172 2229  , type="linear")
-000142b0: 0a20 2020 2020 2020 2063 7269 202a 3d20  .        cri *= 
-000142c0: 7470 0a0a 2020 2020 2020 2020 6d69 6e69  tp..        mini
-000142d0: 6e64 202b 3d20 696e 7428 736c 6964 655f  nd += int(slide_
-000142e0: 7374 6570 202f 2064 7429 0a20 2020 2020  step / dt).     
-000142f0: 2020 206d 6178 696e 6420 2b3d 2069 6e74     maxind += int
-00014300: 2873 6c69 6465 5f73 7465 7020 2f20 6474  (slide_step / dt
-00014310: 290a 0a20 2020 2020 2020 2023 2064 6f20  )..        # do 
-00014320: 6666 740a 2020 2020 2020 2020 6663 7572  fft.        fcur
-00014330: 203d 2073 6369 7079 2e66 6674 7061 636b   = scipy.fftpack
-00014340: 2e66 6674 2863 6369 2c20 6e3d 7061 6464  .fft(cci, n=padd
-00014350: 295b 3a20 7061 6464 202f 2f20 325d 0a20  )[: padd // 2]. 
-00014360: 2020 2020 2020 2066 7265 6620 3d20 7363         fref = sc
-00014370: 6970 792e 6666 7470 6163 6b2e 6666 7428  ipy.fftpack.fft(
-00014380: 6372 692c 206e 3d70 6164 6429 5b3a 2070  cri, n=padd)[: p
-00014390: 6164 6420 2f2f 2032 5d0a 0a20 2020 2020  add // 2]..     
-000143a0: 2020 2066 6375 7232 203d 206e 702e 7265     fcur2 = np.re
-000143b0: 616c 2866 6375 7229 202a 2a20 3220 2b20  al(fcur) ** 2 + 
-000143c0: 6e70 2e69 6d61 6728 6663 7572 2920 2a2a  np.imag(fcur) **
-000143d0: 2032 0a20 2020 2020 2020 2066 7265 6632   2.        fref2
-000143e0: 203d 206e 702e 7265 616c 2866 7265 6629   = np.real(fref)
-000143f0: 202a 2a20 3220 2b20 6e70 2e69 6d61 6728   ** 2 + np.imag(
-00014400: 6672 6566 2920 2a2a 2032 0a0a 2020 2020  fref) ** 2..    
-00014410: 2020 2020 2320 6765 7420 6372 6f73 732d      # get cross-
-00014420: 7370 6563 7472 756d 2026 2064 6f20 6669  spectrum & do fi
-00014430: 6c74 6572 696e 670a 2020 2020 2020 2020  ltering.        
-00014440: 5820 3d20 6672 6566 202a 2028 6663 7572  X = fref * (fcur
-00014450: 2e63 6f6e 6a28 2929 0a20 2020 2020 2020  .conj()).       
-00014460: 2069 6620 736d 6f6f 7468 696e 675f 6861   if smoothing_ha
-00014470: 6c66 5f77 696e 2021 3d20 303a 0a20 2020  lf_win != 0:.   
-00014480: 2020 2020 2020 2020 2064 6375 7220 3d20           dcur = 
-00014490: 6e70 2e73 7172 7428 736d 6f6f 7468 2866  np.sqrt(smooth(f
-000144a0: 6375 7232 2c20 7769 6e64 6f77 3d22 6861  cur2, window="ha
-000144b0: 6e6e 696e 6722 2c20 6861 6c66 5f77 696e  nning", half_win
-000144c0: 3d73 6d6f 6f74 6869 6e67 5f68 616c 665f  =smoothing_half_
-000144d0: 7769 6e29 290a 2020 2020 2020 2020 2020  win)).          
-000144e0: 2020 6472 6566 203d 206e 702e 7371 7274    dref = np.sqrt
-000144f0: 2873 6d6f 6f74 6828 6672 6566 322c 2077  (smooth(fref2, w
-00014500: 696e 646f 773d 2268 616e 6e69 6e67 222c  indow="hanning",
-00014510: 2068 616c 665f 7769 6e3d 736d 6f6f 7468   half_win=smooth
-00014520: 696e 675f 6861 6c66 5f77 696e 2929 0a20  ing_half_win)). 
-00014530: 2020 2020 2020 2020 2020 2058 203d 2073             X = s
-00014540: 6d6f 6f74 6828 582c 2077 696e 646f 773d  mooth(X, window=
-00014550: 2268 616e 6e69 6e67 222c 2068 616c 665f  "hanning", half_
-00014560: 7769 6e3d 736d 6f6f 7468 696e 675f 6861  win=smoothing_ha
-00014570: 6c66 5f77 696e 290a 2020 2020 2020 2020  lf_win).        
-00014580: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014590: 2020 6463 7572 203d 206e 702e 7371 7274    dcur = np.sqrt
-000145a0: 2866 6375 7232 290a 2020 2020 2020 2020  (fcur2).        
-000145b0: 2020 2020 6472 6566 203d 206e 702e 7371      dref = np.sq
-000145c0: 7274 2866 7265 6632 290a 0a20 2020 2020  rt(fref2)..     
-000145d0: 2020 2064 6373 203d 206e 702e 6162 7328     dcs = np.abs(
-000145e0: 5829 0a0a 2020 2020 2020 2020 2320 4669  X)..        # Fi
-000145f0: 6e64 2074 6865 2076 616c 7565 7320 7468  nd the values th
-00014600: 6520 6672 6571 7565 6e63 7920 7261 6e67  e frequency rang
-00014610: 6520 6f66 2069 6e74 6572 6573 740a 2020  e of interest.  
-00014620: 2020 2020 2020 6672 6571 5f76 6563 203d        freq_vec =
-00014630: 2073 6369 7079 2e66 6674 7061 636b 2e66   scipy.fftpack.f
-00014640: 6674 6672 6571 286c 656e 2858 2920 2a20  ftfreq(len(X) * 
-00014650: 322c 2064 7429 5b3a 2070 6164 6420 2f2f  2, dt)[: padd //
-00014660: 2032 5d0a 2020 2020 2020 2020 696e 6465   2].        inde
-00014670: 785f 7261 6e67 6520 3d20 6e70 2e61 7267  x_range = np.arg
-00014680: 7768 6572 6528 6e70 2e6c 6f67 6963 616c  where(np.logical
-00014690: 5f61 6e64 2866 7265 715f 7665 6320 3e3d  _and(freq_vec >=
-000146a0: 2066 6d69 6e2c 2066 7265 715f 7665 6320   fmin, freq_vec 
-000146b0: 3c3d 2066 6d61 7829 290a 0a20 2020 2020  <= fmax))..     
-000146c0: 2020 2023 2047 6574 2043 6f68 6572 656e     # Get Coheren
-000146d0: 6365 2061 6e64 2069 7473 206d 6561 6e20  ce and its mean 
-000146e0: 7661 6c75 650a 2020 2020 2020 2020 636f  value.        co
-000146f0: 6820 3d20 6765 7443 6f68 6572 656e 6365  h = getCoherence
-00014700: 2864 6373 2c20 6472 6566 2c20 6463 7572  (dcs, dref, dcur
-00014710: 290a 2020 2020 2020 2020 6d63 6f68 203d  ).        mcoh =
-00014720: 206e 702e 6d65 616e 2863 6f68 5b69 6e64   np.mean(coh[ind
-00014730: 6578 5f72 616e 6765 5d29 0a0a 2020 2020  ex_range])..    
-00014740: 2020 2020 2320 4765 7420 5765 6967 6874      # Get Weight
-00014750: 730a 2020 2020 2020 2020 7720 3d20 312e  s.        w = 1.
-00014760: 3020 2f20 2831 2e30 202f 2028 636f 685b  0 / (1.0 / (coh[
-00014770: 696e 6465 785f 7261 6e67 655d 202a 2a20  index_range] ** 
-00014780: 3229 202d 2031 2e30 290a 2020 2020 2020  2) - 1.0).      
-00014790: 2020 775b 636f 685b 696e 6465 785f 7261    w[coh[index_ra
-000147a0: 6e67 655d 203e 3d20 302e 3939 5d20 3d20  nge] >= 0.99] = 
-000147b0: 312e 3020 2f20 2831 2e30 202f 2030 2e39  1.0 / (1.0 / 0.9
-000147c0: 3830 3120 2d20 312e 3029 0a20 2020 2020  801 - 1.0).     
-000147d0: 2020 2077 203d 206e 702e 7371 7274 2877     w = np.sqrt(w
-000147e0: 202a 206e 702e 7371 7274 2864 6373 5b69   * np.sqrt(dcs[i
-000147f0: 6e64 6578 5f72 616e 6765 5d29 290a 2020  ndex_range])).  
-00014800: 2020 2020 2020 7720 3d20 6e70 2e72 6561        w = np.rea
-00014810: 6c28 7729 0a0a 2020 2020 2020 2020 2320  l(w)..        # 
-00014820: 4672 6571 7565 6e63 7920 6172 7261 793a  Frequency array:
-00014830: 0a20 2020 2020 2020 2076 203d 206e 702e  .        v = np.
-00014840: 7265 616c 2866 7265 715f 7665 635b 696e  real(freq_vec[in
-00014850: 6465 785f 7261 6e67 655d 2920 2a20 3220  dex_range]) * 2 
-00014860: 2a20 6e70 2e70 690a 0a20 2020 2020 2020  * np.pi..       
-00014870: 2023 2050 6861 7365 3a0a 2020 2020 2020   # Phase:.      
-00014880: 2020 7068 6920 3d20 6e70 2e61 6e67 6c65    phi = np.angle
-00014890: 2858 290a 2020 2020 2020 2020 7068 695b  (X).        phi[
-000148a0: 305d 203d 2030 2e30 0a20 2020 2020 2020  0] = 0.0.       
-000148b0: 2070 6869 203d 206e 702e 756e 7772 6170   phi = np.unwrap
-000148c0: 2870 6869 290a 2020 2020 2020 2020 7068  (phi).        ph
-000148d0: 6920 3d20 7068 695b 696e 6465 785f 7261  i = phi[index_ra
-000148e0: 6e67 655d 0a0a 2020 2020 2020 2020 2320  nge]..        # 
-000148f0: 4361 6c63 756c 6174 6520 7468 6520 736c  Calculate the sl
-00014900: 6f70 6520 7769 7468 2061 2077 6569 6768  ope with a weigh
-00014910: 7465 6420 6c65 6173 7420 7371 7561 7265  ted least square
-00014920: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
-00014930: 6f6e 0a20 2020 2020 2020 2023 2066 6f72  on.        # for
-00014940: 6365 6420 7468 726f 7567 6820 7468 6520  ced through the 
-00014950: 6f72 6967 696e 3b20 7765 6967 6874 7320  origin; weights 
-00014960: 666f 7220 7468 6520 574c 5320 6d75 7374  for the WLS must
-00014970: 2062 6520 7468 6520 7661 7269 616e 6365   be the variance
-00014980: 2021 0a20 2020 2020 2020 206d 2c20 656d   !.        m, em
-00014990: 203d 206c 696e 6561 725f 7265 6772 6573   = linear_regres
-000149a0: 7369 6f6e 2876 2e66 6c61 7474 656e 2829  sion(v.flatten()
-000149b0: 2c20 7068 692e 666c 6174 7465 6e28 292c  , phi.flatten(),
-000149c0: 2077 2e66 6c61 7474 656e 2829 290a 2020   w.flatten()).  
-000149d0: 2020 2020 2020 6465 6c74 615f 742e 6170        delta_t.ap
-000149e0: 7065 6e64 286d 290a 0a20 2020 2020 2020  pend(m)..       
-000149f0: 2023 2070 7269 6e74 2070 6869 2e73 6861   # print phi.sha
-00014a00: 7065 2c20 762e 7368 6170 652c 2077 2e73  pe, v.shape, w.s
-00014a10: 6861 7065 0a20 2020 2020 2020 2065 203d  hape.        e =
-00014a20: 206e 702e 7375 6d28 2870 6869 202d 206d   np.sum((phi - m
-00014a30: 202a 2076 2920 2a2a 2032 2920 2f20 286e   * v) ** 2) / (n
-00014a40: 702e 7369 7a65 2876 2920 2d20 3129 0a20  p.size(v) - 1). 
-00014a50: 2020 2020 2020 2073 3278 3220 3d20 6e70         s2x2 = np
-00014a60: 2e73 756d 2876 2a2a 3220 2a20 772a 2a32  .sum(v**2 * w**2
-00014a70: 290a 2020 2020 2020 2020 7378 3220 3d20  ).        sx2 = 
-00014a80: 6e70 2e73 756d 2877 202a 2076 2a2a 3229  np.sum(w * v**2)
-00014a90: 0a20 2020 2020 2020 2065 203d 206e 702e  .        e = np.
-00014aa0: 7371 7274 2865 202a 2073 3278 3220 2f20  sqrt(e * s2x2 / 
-00014ab0: 7378 322a 2a32 290a 0a20 2020 2020 2020  sx2**2)..       
-00014ac0: 2064 656c 7461 5f65 7272 2e61 7070 656e   delta_err.appen
-00014ad0: 6428 6529 0a20 2020 2020 2020 2064 656c  d(e).        del
-00014ae0: 7461 5f6d 636f 682e 6170 7065 6e64 286e  ta_mcoh.append(n
-00014af0: 702e 7265 616c 286d 636f 6829 290a 2020  p.real(mcoh)).  
-00014b00: 2020 2020 2020 7469 6d65 5f61 7869 732e        time_axis.
-00014b10: 6170 7065 6e64 2874 6d69 6e20 2b20 6d6f  append(tmin + mo
-00014b20: 7669 6e67 5f77 696e 646f 775f 6c65 6e67  ving_window_leng
-00014b30: 7468 202f 2032 2e30 202b 2063 6f75 6e74  th / 2.0 + count
-00014b40: 202a 2073 6c69 6465 5f73 7465 7029 0a20   * slide_step). 
-00014b50: 2020 2020 2020 2063 6f75 6e74 202b 3d20         count += 
-00014b60: 310a 0a20 2020 2020 2020 2064 656c 2066  1..        del f
-00014b70: 6375 722c 2066 7265 660a 2020 2020 2020  cur, fref.      
-00014b80: 2020 6465 6c20 580a 2020 2020 2020 2020    del X.        
-00014b90: 6465 6c20 6672 6571 5f76 6563 0a20 2020  del freq_vec.   
-00014ba0: 2020 2020 2064 656c 2069 6e64 6578 5f72       del index_r
-00014bb0: 616e 6765 0a20 2020 2020 2020 2064 656c  ange.        del
-00014bc0: 2077 2c20 762c 2065 2c20 7332 7832 2c20   w, v, e, s2x2, 
-00014bd0: 7378 322c 206d 2c20 656d 0a0a 2020 2020  sx2, m, em..    
-00014be0: 6966 206d 6178 696e 6420 3e20 6c65 6e28  if maxind > len(
-00014bf0: 6375 7229 202b 2069 6e74 2873 6c69 6465  cur) + int(slide
-00014c00: 5f73 7465 7020 2f20 6474 293a 0a20 2020  _step / dt):.   
-00014c10: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00014c20: 6728 2254 6865 206c 6173 7420 7769 6e64  g("The last wind
-00014c30: 6f77 2077 6173 2074 6f6f 2073 6d61 6c6c  ow was too small
-00014c40: 2c20 6275 7420 7761 7320 636f 6d70 7574  , but was comput
-00014c50: 6564 2229 0a0a 2020 2020 2320 656e 7375  ed")..    # ensu
-00014c60: 7265 2061 6c6c 206d 6174 7269 7820 6172  re all matrix ar
-00014c70: 6520 6e70 2061 7272 6179 0a20 2020 2064  e np array.    d
-00014c80: 656c 7461 5f74 203d 206e 702e 6172 7261  elta_t = np.arra
-00014c90: 7928 6465 6c74 615f 7429 0a20 2020 2064  y(delta_t).    d
-00014ca0: 656c 7461 5f65 7272 203d 206e 702e 6172  elta_err = np.ar
-00014cb0: 7261 7928 6465 6c74 615f 6572 7229 0a20  ray(delta_err). 
-00014cc0: 2020 2064 656c 7461 5f6d 636f 6820 3d20     delta_mcoh = 
-00014cd0: 6e70 2e61 7272 6179 2864 656c 7461 5f6d  np.array(delta_m
-00014ce0: 636f 6829 0a20 2020 2074 696d 655f 6178  coh).    time_ax
-00014cf0: 6973 203d 206e 702e 6172 7261 7928 7469  is = np.array(ti
-00014d00: 6d65 5f61 7869 7329 0a0a 2020 2020 2320  me_axis)..    # 
-00014d10: 7265 6164 7920 666f 7220 6c69 6e65 6172  ready for linear
-00014d20: 2072 6567 7265 7373 696f 6e0a 2020 2020   regression.    
-00014d30: 6465 6c74 615f 6d69 6e63 686f 203d 2030  delta_mincho = 0
-00014d40: 2e36 350a 2020 2020 6465 6c74 615f 6d61  .65.    delta_ma
-00014d50: 7865 7272 203d 2030 2e31 0a20 2020 2064  xerr = 0.1.    d
-00014d60: 656c 7461 5f6d 6178 6474 203d 2030 2e31  elta_maxdt = 0.1
-00014d70: 0a20 2020 2069 6e64 7831 203d 206e 702e  .    indx1 = np.
-00014d80: 7768 6572 6528 6465 6c74 615f 6d63 6f68  where(delta_mcoh
-00014d90: 203e 2064 656c 7461 5f6d 696e 6368 6f29   > delta_mincho)
-00014da0: 0a20 2020 2069 6e64 7832 203d 206e 702e  .    indx2 = np.
-00014db0: 7768 6572 6528 6465 6c74 615f 6572 7220  where(delta_err 
-00014dc0: 3c20 6465 6c74 615f 6d61 7865 7272 290a  < delta_maxerr).
-00014dd0: 2020 2020 696e 6478 3320 3d20 6e70 2e77      indx3 = np.w
-00014de0: 6865 7265 2864 656c 7461 5f74 203c 2064  here(delta_t < d
-00014df0: 656c 7461 5f6d 6178 6474 290a 0a20 2020  elta_maxdt)..   
-00014e00: 2023 202d 2d2d 2d2d 6669 6e64 2067 6f6f   # -----find goo
-00014e10: 6420 6474 206d 6561 7375 7265 6d65 6e74  d dt measurement
-00014e20: 732d 2d2d 2d2d 0a20 2020 2069 6e64 7820  s-----.    indx 
-00014e30: 3d20 6e70 2e69 6e74 6572 7365 6374 3164  = np.intersect1d
-00014e40: 2869 6e64 7831 2c20 696e 6478 3229 0a20  (indx1, indx2). 
-00014e50: 2020 2069 6e64 7820 3d20 6e70 2e69 6e74     indx = np.int
-00014e60: 6572 7365 6374 3164 2869 6e64 782c 2069  ersect1d(indx, i
-00014e70: 6e64 7833 290a 0a20 2020 2069 6620 6c65  ndx3)..    if le
-00014e80: 6e28 696e 6478 2920 3e20 323a 0a20 2020  n(indx) > 2:.   
-00014e90: 2020 2020 2023 202d 2d2d 2d65 7374 696d       # ----estim
-00014ea0: 6174 6520 7765 6967 6874 2066 6f72 2072  ate weight for r
-00014eb0: 6567 7265 7373 696f 6e2d 2d2d 2d0a 2020  egression----.  
-00014ec0: 2020 2020 2020 7720 3d20 3120 2f20 6465        w = 1 / de
-00014ed0: 6c74 615f 6572 725b 696e 6478 5d0a 2020  lta_err[indx].  
-00014ee0: 2020 2020 2020 775b 7e6e 702e 6973 6669        w[~np.isfi
-00014ef0: 6e69 7465 2877 295d 203d 2031 2e30 0a0a  nite(w)] = 1.0..
-00014f00: 2020 2020 2020 2020 2320 2d2d 2d2d 2d2d          # ------
-00014f10: 2d2d 2d64 6f20 6c69 6e65 6172 2072 6567  ---do linear reg
-00014f20: 7265 7373 696f 6e2d 2d2d 2d2d 2d2d 2d2d  ression---------
-00014f30: 2d2d 0a20 2020 2020 2020 2023 206d 2c20  --.        # m, 
-00014f40: 612c 2065 6d2c 2065 6120 3d20 6c69 6e65  a, em, ea = line
-00014f50: 6172 5f72 6567 7265 7373 696f 6e28 7469  ar_regression(ti
-00014f60: 6d65 5f61 7869 735b 696e 6478 5d2c 2064  me_axis[indx], d
-00014f70: 656c 7461 5f74 5b69 6e64 785d 2c20 772c  elta_t[indx], w,
-00014f80: 2069 6e74 6572 6365 7074 5f6f 7269 6769   intercept_origi
-00014f90: 6e3d 4661 6c73 6529 0a20 2020 2020 2020  n=False).       
-00014fa0: 206d 302c 2065 6d30 203d 206c 696e 6561   m0, em0 = linea
-00014fb0: 725f 7265 6772 6573 7369 6f6e 2874 696d  r_regression(tim
-00014fc0: 655f 6178 6973 5b69 6e64 785d 2c20 6465  e_axis[indx], de
-00014fd0: 6c74 615f 745b 696e 6478 5d2c 2077 2c20  lta_t[indx], w, 
-00014fe0: 696e 7465 7263 6570 745f 6f72 6967 696e  intercept_origin
-00014ff0: 3d54 7275 6529 0a0a 2020 2020 656c 7365  =True)..    else
-00015000: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
-00015010: 2e64 6562 7567 2822 6e6f 7420 656e 6f75  .debug("not enou
-00015020: 6768 2070 6f69 6e74 7320 746f 2065 7374  gh points to est
-00015030: 696d 6174 6520 6476 2f76 2066 6f72 206d  imate dv/v for m
-00015040: 7763 7322 290a 2020 2020 2020 2020 6d30  wcs").        m0
-00015050: 203d 2030 0a20 2020 2020 2020 2065 6d30   = 0.        em0
-00015060: 203d 2030 0a0a 2020 2020 7265 7475 726e   = 0..    return
-00015070: 202d 6d30 202a 2031 3030 2c20 656d 3020   -m0 * 100, em0 
-00015080: 2a20 3130 300a 0a0a 6465 6620 5743 435f  * 100...def WCC_
-00015090: 6476 7628 7265 662c 2063 7572 2c20 6d6f  dvv(ref, cur, mo
-000150a0: 7669 6e67 5f77 696e 646f 775f 6c65 6e67  ving_window_leng
-000150b0: 7468 2c20 736c 6964 655f 7374 6570 2c20  th, slide_step, 
-000150c0: 7061 7261 293a 0a20 2020 2022 2222 0a20  para):.    """. 
-000150d0: 2020 2057 696e 646f 7765 6420 6372 6f73     Windowed cros
-000150e0: 7320 636f 7272 656c 6174 696f 6e20 2857  s correlation (W
-000150f0: 4343 2920 666f 7220 6474 206f 7220 6476  CC) for dt or dv
-00015100: 2f76 206d 6573 7572 656d 656e 7420 2853  /v mesurement (S
-00015110: 6e69 6564 6572 2065 7420 616c 2e20 3230  nieder et al. 20
-00015120: 3132 290a 0a20 2020 2050 6172 616d 6574  12)..    Paramet
-00015130: 6572 733a 0a20 2020 202d 2d2d 2d2d 2d2d  ers:.    -------
-00015140: 2d2d 2d2d 0a20 2020 2072 6566 3a20 5468  ----.    ref: Th
-00015150: 6520 2252 6566 6572 656e 6365 2220 7469  e "Reference" ti
-00015160: 6d65 7365 7269 6573 0a20 2020 2063 7572  meseries.    cur
-00015170: 3a20 5468 6520 2243 7572 7265 6e74 2220  : The "Current" 
-00015180: 7469 6d65 7365 7269 6573 0a20 2020 206d  timeseries.    m
-00015190: 6f76 696e 675f 7769 6e64 6f77 5f6c 656e  oving_window_len
-000151a0: 6774 683a 2054 6865 206d 6f76 696e 6720  gth: The moving 
-000151b0: 7769 6e64 6f77 206c 656e 6774 6820 2869  window length (i
-000151c0: 6e20 7365 636f 6e64 7329 0a20 2020 2073  n seconds).    s
-000151d0: 6c69 6465 5f73 7465 703a 2054 6865 2073  lide_step: The s
-000151e0: 7465 7020 746f 206a 756d 7020 666f 7220  tep to jump for 
-000151f0: 7468 6520 6d6f 7669 6e67 2077 696e 646f  the moving windo
-00015200: 7720 2869 6e20 7365 636f 6e64 7329 0a20  w (in seconds). 
-00015210: 2020 2070 6172 613a 2061 2064 6963 7420     para: a dict 
-00015220: 636f 6e74 6169 6e69 6e67 2066 7265 712f  containing freq/
-00015230: 7469 6d65 2069 6e66 6f20 6f66 2074 6865  time info of the
-00015240: 2064 6174 6120 6d61 7472 6978 0a0a 2020   data matrix..  
-00015250: 2020 5265 7475 726e 733a 0a20 2020 202d    Returns:.    -
-00015260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00015270: 7469 6d65 5f61 7869 733a 2063 656e 7472  time_axis: centr
-00015280: 616c 2074 696d 6573 206f 6620 7468 6520  al times of the 
-00015290: 6d6f 7669 6e67 2077 696e 646f 770a 2020  moving window.  
-000152a0: 2020 6465 6c74 615f 743a 2064 740a 2020    delta_t: dt.  
-000152b0: 2020 6465 6c74 615f 6572 723a 2065 7272    delta_err: err
-000152c0: 6f72 0a20 2020 2064 656c 7461 5f6d 636f  or.    delta_mco
-000152d0: 683a 206d 6561 6e20 636f 6865 7265 6e63  h: mean coherenc
-000152e0: 6520 666f 7220 6561 6368 2077 696e 646f  e for each windo
-000152f0: 770a 0a20 2020 2057 7269 7474 656e 2062  w..    Written b
-00015300: 7920 436f 6e67 636f 6e67 2059 7561 6e20  y Congcong Yuan 
-00015310: 2831 204a 756c 792c 2032 3031 3929 0a20  (1 July, 2019). 
-00015320: 2020 2022 2222 0a20 2020 2023 2063 6f6d     """.    # com
-00015330: 6d6f 6e20 7661 7269 6162 6c65 730a 2020  mon variables.  
-00015340: 2020 7477 696e 203d 2070 6172 615b 2274    twin = para["t
-00015350: 7769 6e22 5d0a 2020 2020 6474 203d 2070  win"].    dt = p
-00015360: 6172 615b 2264 7422 5d0a 2020 2020 746d  ara["dt"].    tm
-00015370: 696e 203d 206e 702e 6d69 6e28 7477 696e  in = np.min(twin
-00015380: 290a 0a20 2020 2023 2070 6172 616d 6574  )..    # paramet
-00015390: 6572 2069 6e69 7469 616c 697a 650a 2020  er initialize.  
-000153a0: 2020 6465 6c74 615f 7420 3d20 5b5d 0a20    delta_t = []. 
-000153b0: 2020 2064 656c 7461 5f74 5f63 6f65 6620     delta_t_coef 
-000153c0: 3d20 5b5d 0a20 2020 2074 696d 655f 6178  = [].    time_ax
-000153d0: 6973 203d 205b 5d0a 0a20 2020 2023 2069  is = []..    # i
-000153e0: 6e66 6f20 6f6e 2074 6865 206d 6f76 696e  nfo on the movin
-000153f0: 6720 7769 6e64 6f77 0a20 2020 2077 696e  g window.    win
-00015400: 646f 775f 6c65 6e67 7468 5f73 616d 706c  dow_length_sampl
-00015410: 6573 203d 206e 702e 696e 7428 6d6f 7669  es = np.int(movi
-00015420: 6e67 5f77 696e 646f 775f 6c65 6e67 7468  ng_window_length
-00015430: 202f 2064 7429 0a20 2020 2063 6f75 6e74   / dt).    count
-00015440: 203d 2030 0a20 2020 2074 7020 3d20 636f   = 0.    tp = co
-00015450: 7369 6e65 5f74 6170 6572 2877 696e 646f  sine_taper(windo
-00015460: 775f 6c65 6e67 7468 5f73 616d 706c 6573  w_length_samples
-00015470: 2c20 302e 3135 290a 0a20 2020 206d 696e  , 0.15)..    min
-00015480: 696e 6420 3d20 300a 2020 2020 6d61 7869  ind = 0.    maxi
-00015490: 6e64 203d 2077 696e 646f 775f 6c65 6e67  nd = window_leng
-000154a0: 7468 5f73 616d 706c 6573 0a0a 2020 2020  th_samples..    
-000154b0: 2320 6c6f 6f70 2074 6872 6f75 6768 2061  # loop through a
-000154c0: 6c6c 2073 7562 2d77 696e 646f 7773 0a20  ll sub-windows. 
-000154d0: 2020 2077 6869 6c65 206d 6178 696e 6420     while maxind 
-000154e0: 3c3d 206c 656e 2872 6566 293a 0a20 2020  <= len(ref):.   
-000154f0: 2020 2020 2063 6369 203d 2063 7572 5b6d       cci = cur[m
-00015500: 696e 696e 643a 6d61 7869 6e64 5d0a 2020  inind:maxind].  
-00015510: 2020 2020 2020 6363 6920 3d20 7363 6970        cci = scip
-00015520: 792e 7369 676e 616c 2e64 6574 7265 6e64  y.signal.detrend
-00015530: 2863 6369 2c20 7479 7065 3d22 6c69 6e65  (cci, type="line
-00015540: 6172 2229 0a20 2020 2020 2020 2063 6369  ar").        cci
-00015550: 202a 3d20 7470 0a0a 2020 2020 2020 2020   *= tp..        
-00015560: 6372 6920 3d20 7265 665b 6d69 6e69 6e64  cri = ref[minind
-00015570: 3a6d 6178 696e 645d 0a20 2020 2020 2020  :maxind].       
-00015580: 2063 7269 203d 2073 6369 7079 2e73 6967   cri = scipy.sig
-00015590: 6e61 6c2e 6465 7472 656e 6428 6372 692c  nal.detrend(cri,
-000155a0: 2074 7970 653d 226c 696e 6561 7222 290a   type="linear").
-000155b0: 2020 2020 2020 2020 6372 6920 2a3d 2074          cri *= t
-000155c0: 700a 0a20 2020 2020 2020 206d 696e 696e  p..        minin
-000155d0: 6420 2b3d 2069 6e74 2873 6c69 6465 5f73  d += int(slide_s
-000155e0: 7465 7020 2f20 6474 290a 2020 2020 2020  tep / dt).      
-000155f0: 2020 6d61 7869 6e64 202b 3d20 696e 7428    maxind += int(
-00015600: 736c 6964 655f 7374 6570 202f 2064 7429  slide_step / dt)
-00015610: 0a0a 2020 2020 2020 2020 2320 6e6f 726d  ..        # norm
-00015620: 616c 697a 6520 7369 676e 616c 7320 6265  alize signals be
-00015630: 666f 7265 2063 726f 7373 2063 6f72 7265  fore cross corre
-00015640: 6c61 7469 6f6e 0a20 2020 2020 2020 2063  lation.        c
-00015650: 6369 203d 2028 6363 6920 2d20 6363 692e  ci = (cci - cci.
-00015660: 6d65 616e 2829 2920 2f20 6363 692e 7374  mean()) / cci.st
-00015670: 6428 290a 2020 2020 2020 2020 6372 6920  d().        cri 
-00015680: 3d20 2863 7269 202d 2063 7269 2e6d 6561  = (cri - cri.mea
-00015690: 6e28 2929 202f 2063 7269 2e73 7464 2829  n()) / cri.std()
-000156a0: 0a0a 2020 2020 2020 2020 2320 6765 7420  ..        # get 
-000156b0: 6d61 7869 6d75 6d20 636f 7272 656c 6174  maximum correlat
-000156c0: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
-000156d0: 616e 6420 6974 7320 696e 6465 780a 2020  and its index.  
-000156e0: 2020 2020 2020 6363 3220 3d20 6e70 2e63        cc2 = np.c
-000156f0: 6f72 7265 6c61 7465 2863 6369 2c20 6372  orrelate(cci, cr
-00015700: 692c 206d 6f64 653d 2273 616d 6522 290a  i, mode="same").
-00015710: 2020 2020 2020 2020 6363 3220 3d20 6363          cc2 = cc
-00015720: 3220 2f20 6e70 2e73 7172 7428 2863 6369  2 / np.sqrt((cci
-00015730: 2a2a 3229 2e73 756d 2829 202a 2028 6372  **2).sum() * (cr
-00015740: 692a 2a32 292e 7375 6d28 2929 0a0a 2020  i**2).sum())..  
-00015750: 2020 2020 2020 696d 6178 6363 3220 3d20        imaxcc2 = 
-00015760: 6e70 2e77 6865 7265 2863 6332 203d 3d20  np.where(cc2 == 
-00015770: 6e70 2e6d 6178 2863 6332 2929 5b30 5d0a  np.max(cc2))[0].
-00015780: 2020 2020 2020 2020 6d61 7863 6332 203d          maxcc2 =
-00015790: 206e 702e 6d61 7828 6363 3229 0a0a 2020   np.max(cc2)..  
-000157a0: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
-000157b0: 7469 6d65 2073 6869 6674 0a20 2020 2020  time shift.     
-000157c0: 2020 206d 203d 2028 696d 6178 6363 3220     m = (imaxcc2 
-000157d0: 2d20 2828 6d61 7869 6e64 202d 206d 696e  - ((maxind - min
-000157e0: 696e 6429 202f 2f20 3229 2920 2a20 6474  ind) // 2)) * dt
-000157f0: 0a20 2020 2020 2020 2064 656c 7461 5f74  .        delta_t
-00015800: 2e61 7070 656e 6428 6d29 0a20 2020 2020  .append(m).     
-00015810: 2020 2064 656c 7461 5f74 5f63 6f65 662e     delta_t_coef.
-00015820: 6170 7065 6e64 286d 6178 6363 3229 0a0a  append(maxcc2)..
-00015830: 2020 2020 2020 2020 7469 6d65 5f61 7869          time_axi
-00015840: 732e 6170 7065 6e64 2874 6d69 6e20 2b20  s.append(tmin + 
-00015850: 6d6f 7669 6e67 5f77 696e 646f 775f 6c65  moving_window_le
-00015860: 6e67 7468 202f 2032 2e30 202b 2063 6f75  ngth / 2.0 + cou
-00015870: 6e74 202a 2073 6c69 6465 5f73 7465 7029  nt * slide_step)
-00015880: 0a20 2020 2020 2020 2063 6f75 6e74 202b  .        count +
-00015890: 3d20 310a 0a20 2020 2064 656c 2063 6369  = 1..    del cci
-000158a0: 2c20 6372 692c 2063 6332 2c20 696d 6178  , cri, cc2, imax
-000158b0: 6363 322c 206d 6178 6363 320a 2020 2020  cc2, maxcc2.    
-000158c0: 6465 6c20 6d0a 0a20 2020 2069 6620 6d61  del m..    if ma
-000158d0: 7869 6e64 203e 206c 656e 2863 7572 2920  xind > len(cur) 
-000158e0: 2b20 696e 7428 736c 6964 655f 7374 6570  + int(slide_step
-000158f0: 202f 2064 7429 3a0a 2020 2020 2020 2020   / dt):.        
-00015900: 6c6f 6767 6572 2e64 6562 7567 2822 5468  logger.debug("Th
-00015910: 6520 6c61 7374 2077 696e 646f 7720 7761  e last window wa
-00015920: 7320 746f 6f20 736d 616c 6c2c 2062 7574  s too small, but
-00015930: 2077 6173 2063 6f6d 7075 7465 6422 290a   was computed").
-00015940: 0a20 2020 2064 656c 7461 5f74 203d 206e  .    delta_t = n
-00015950: 702e 6172 7261 7928 6465 6c74 615f 7429  p.array(delta_t)
-00015960: 0a20 2020 2064 656c 7461 5f74 5f63 6f65  .    delta_t_coe
-00015970: 6620 3d20 6e70 2e61 7272 6179 2864 656c  f = np.array(del
-00015980: 7461 5f74 5f63 6f65 6629 0a20 2020 2074  ta_t_coef).    t
-00015990: 696d 655f 6178 6973 203d 206e 702e 6172  ime_axis = np.ar
-000159a0: 7261 7928 7469 6d65 5f61 7869 7329 0a0a  ray(time_axis)..
-000159b0: 2020 2020 2320 6c69 6e65 6172 2072 6567      # linear reg
-000159c0: 7265 7373 696f 6e20 746f 2067 6574 2064  ression to get d
-000159d0: 762f 760a 2020 2020 6966 2063 6f75 6e74  v/v.    if count
-000159e0: 203e 2032 3a0a 2020 2020 2020 2020 2320   > 2:.        # 
-000159f0: 7369 6d70 6c65 2077 6569 6768 740a 2020  simple weight.  
-00015a00: 2020 2020 2020 7720 3d20 6e70 2e6f 6e65        w = np.one
-00015a10: 7328 636f 756e 7429 0a20 2020 2020 2020  s(count).       
-00015a20: 2023 206d 2c20 612c 2065 6d2c 2065 6120   # m, a, em, ea 
-00015a30: 3d20 6c69 6e65 6172 5f72 6567 7265 7373  = linear_regress
-00015a40: 696f 6e28 7469 6d65 5f61 7869 735b 696e  ion(time_axis[in
-00015a50: 6478 5d2c 2064 656c 7461 5f74 5b69 6e64  dx], delta_t[ind
-00015a60: 785d 2c20 772c 2069 6e74 6572 6365 7074  x], w, intercept
-00015a70: 5f6f 7269 6769 6e3d 4661 6c73 6529 0a20  _origin=False). 
-00015a80: 2020 2020 2020 206d 302c 2065 6d30 203d         m0, em0 =
-00015a90: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
-00015aa0: 6f6e 2874 696d 655f 6178 6973 2e66 6c61  on(time_axis.fla
-00015ab0: 7474 656e 2829 2c20 6465 6c74 615f 742e  tten(), delta_t.
-00015ac0: 666c 6174 7465 6e28 292c 2077 2e66 6c61  flatten(), w.fla
-00015ad0: 7474 656e 2829 2c20 696e 7465 7263 6570  tten(), intercep
-00015ae0: 745f 6f72 6967 696e 3d54 7275 6529 0a0a  t_origin=True)..
-00015af0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015b00: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00015b10: 6e6f 7420 656e 6f75 6768 2070 6f69 6e74  not enough point
-00015b20: 7320 746f 2065 7374 696d 6174 6520 6476  s to estimate dv
-00015b30: 2f76 2066 6f72 2077 6363 2229 0a20 2020  /v for wcc").   
-00015b40: 2020 2020 206d 3020 3d20 300a 2020 2020       m0 = 0.    
-00015b50: 2020 2020 656d 3020 3d20 300a 0a20 2020      em0 = 0..   
-00015b60: 2072 6574 7572 6e20 2d6d 3020 2a20 3130   return -m0 * 10
-00015b70: 302c 2065 6d30 202a 2031 3030 0a0a 0a64  0, em0 * 100...d
-00015b80: 6566 2077 7873 5f64 7676 280a 2020 2020  ef wxs_dvv(.    
-00015b90: 7265 662c 0a20 2020 2063 7572 2c0a 2020  ref,.    cur,.  
-00015ba0: 2020 616c 6c66 7265 712c 0a20 2020 2070    allfreq,.    p
-00015bb0: 6172 612c 0a20 2020 2064 6a3d 3120 2f20  ara,.    dj=1 / 
-00015bc0: 3132 2c0a 2020 2020 7330 3d2d 312c 0a20  12,.    s0=-1,. 
-00015bd0: 2020 204a 3d2d 312c 0a20 2020 2073 6967     J=-1,.    sig
-00015be0: 3d46 616c 7365 2c0a 2020 2020 7776 6e3d  =False,.    wvn=
-00015bf0: 226d 6f72 6c65 7422 2c0a 2020 2020 756e  "morlet",.    un
-00015c00: 7772 6170 666c 6167 3d46 616c 7365 2c0a  wrapflag=False,.
-00015c10: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
-00015c20: 6f6d 7075 7465 2064 7420 6f72 2064 762f  ompute dt or dv/
-00015c30: 7620 696e 2074 696d 6520 616e 6420 6672  v in time and fr
-00015c40: 6571 7565 6e63 7920 646f 6d61 696e 2066  equency domain f
-00015c50: 726f 6d20 7761 7665 6c65 7420 6372 6f73  rom wavelet cros
-00015c60: 7320 7370 6563 7472 756d 2028 7778 7329  s spectrum (wxs)
-00015c70: 2e0a 2020 2020 666f 7220 616c 6c20 6672  ..    for all fr
-00015c80: 6571 7565 6369 6573 2069 6e20 616e 2069  equecies in an i
-00015c90: 6e74 6572 6573 7420 7261 6e67 650a 0a20  nterest range.. 
-00015ca0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00015cb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00015cc0: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
-00015cd0: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
-00015ce0: 7269 6573 2028 6e75 6d70 792e 6e64 6172  ries (numpy.ndar
-00015cf0: 7261 7929 0a20 2020 2063 7572 3a20 5468  ray).    cur: Th
-00015d00: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
-00015d10: 7365 7269 6573 2028 6e75 6d70 792e 6e64  series (numpy.nd
-00015d20: 6172 7261 7929 0a20 2020 2061 6c6c 6672  array).    allfr
-00015d30: 6571 3a20 6120 626f 6f6c 656e 2076 6172  eq: a boolen var
-00015d40: 6961 626c 6520 746f 206d 616b 6520 6d65  iable to make me
-00015d50: 6173 7572 656d 656e 7473 206f 6e20 616c  asurements on al
-00015d60: 6c20 6672 6571 7565 6e63 7920 7261 6e67  l frequency rang
-00015d70: 6520 6f72 206e 6f74 0a20 2020 2070 6172  e or not.    par
-00015d80: 613a 2061 2064 6963 7420 636f 6e74 6169  a: a dict contai
-00015d90: 6e69 6e67 2066 7265 712f 7469 6d65 2069  ning freq/time i
-00015da0: 6e66 6f20 6f66 2074 6865 2064 6174 6120  nfo of the data 
-00015db0: 6d61 7472 6978 0a20 2020 2064 6a2c 2073  matrix.    dj, s
-00015dc0: 302c 204a 2c20 7369 672c 2077 766e 3a20  0, J, sig, wvn: 
-00015dd0: 636f 6d6d 6f6e 2070 6172 616d 6574 6572  common parameter
-00015de0: 7320 7573 6564 2069 6e20 2777 6176 656c  s used in 'wavel
-00015df0: 6574 2e77 6374 270a 2020 2020 756e 7772  et.wct'.    unwr
-00015e00: 6170 666c 6167 3a20 5472 7565 202d 2075  apflag: True - u
-00015e10: 6e77 7261 7020 7068 6173 6520 6465 6c61  nwrap phase dela
-00015e20: 7973 2e20 4465 6661 756c 7420 6973 2046  ys. Default is F
-00015e30: 616c 7365 0a0a 2020 2020 5245 5455 524e  alse..    RETURN
-00015e40: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00015e50: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6476  ---------.    dv
-00015e60: 762a 3130 3020 3a20 6573 7469 6d61 7465  v*100 : estimate
-00015e70: 6420 6476 2f76 2069 6e20 250a 2020 2020  d dv/v in %.    
-00015e80: 6572 722a 3130 3020 3a20 6572 726f 7220  err*100 : error 
-00015e90: 6f66 2064 762f 7620 6573 7469 6d61 7469  of dv/v estimati
-00015ea0: 6f6e 2069 6e20 250a 0a20 2020 204f 7269  on in %..    Ori
-00015eb0: 6769 6e61 6c6c 7920 7772 6974 7465 6e20  ginally written 
-00015ec0: 6279 2054 696d 2043 6c65 6d65 6e74 7320  by Tim Clements 
-00015ed0: 2831 204d 6172 6368 2c20 3230 3139 290a  (1 March, 2019).
-00015ee0: 2020 2020 4d6f 6469 6669 6564 2062 7920      Modified by 
-00015ef0: 436f 6e67 636f 6e67 2059 7561 6e20 2833  Congcong Yuan (3
-00015f00: 3020 4a75 6e65 2c20 3230 3139 2920 6261  0 June, 2019) ba
-00015f10: 7365 6420 6f6e 2028 4d61 6f20 6574 2061  sed on (Mao et a
-00015f20: 6c2e 2032 3031 3929 2e0a 2020 2020 5570  l. 2019)..    Up
-00015f30: 6461 7465 6420 6279 2043 6865 6e67 7869  dated by Chengxi
-00015f40: 6e20 4a69 616e 6720 2831 3020 4f63 742c  n Jiang (10 Oct,
-00015f50: 2032 3031 3929 2074 6f20 6d65 7267 6520   2019) to merge 
-00015f60: 7468 6520 6675 6e63 7469 6f6e 616c 6974  the functionalit
-00015f70: 7920 666f 7220 6d65 7375 7265 6d65 6e74  y for mesurement
-00015f80: 730a 2020 2020 6163 726f 7373 2061 6c6c  s.    across all
-00015f90: 2066 7265 7175 656e 6379 2061 6e64 206f   frequency and o
-00015fa0: 6e65 2066 7265 7120 7261 6e67 650a 2020  ne freq range.  
-00015fb0: 2020 2222 220a 2020 2020 2320 636f 6d6d    """.    # comm
-00015fc0: 6f6e 2076 6172 6961 626c 6573 0a20 2020  on variables.   
-00015fd0: 2074 7769 6e20 3d20 7061 7261 5b22 7477   twin = para["tw
-00015fe0: 696e 225d 0a20 2020 2066 7265 7120 3d20  in"].    freq = 
-00015ff0: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
-00016000: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
-00016010: 0a20 2020 2074 6d69 6e20 3d20 6e70 2e6d  .    tmin = np.m
-00016020: 696e 2874 7769 6e29 0a20 2020 2074 6d61  in(twin).    tma
-00016030: 7820 3d20 6e70 2e6d 6178 2874 7769 6e29  x = np.max(twin)
-00016040: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
-00016050: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
-00016060: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
-00016070: 0a20 2020 2074 7665 6320 3d20 6e70 2e61  .    tvec = np.a
-00016080: 7261 6e67 6528 746d 696e 2c20 746d 6178  range(tmin, tmax
-00016090: 2c20 6474 290a 2020 2020 6e70 7473 203d  , dt).    npts =
-000160a0: 206c 656e 2874 7665 6329 0a0a 2020 2020   len(tvec)..    
-000160b0: 2320 7065 7266 6f72 6d20 6372 6f73 7320  # perform cross 
-000160c0: 636f 6865 7265 6e74 2061 6e61 6c79 7369  coherent analysi
-000160d0: 732c 206d 6f64 6966 6965 6420 6672 6f6d  s, modified from
-000160e0: 2066 756e 6374 696f 6e20 2777 6176 656c   function 'wavel
-000160f0: 6574 2e63 7774 270a 2020 2020 5743 542c  et.cwt'.    WCT,
-00016100: 2061 5743 542c 2063 6f69 2c20 6672 6571   aWCT, coi, freq
-00016110: 2c20 7369 6720 3d20 7763 745f 6d6f 6469  , sig = wct_modi
-00016120: 6669 6564 2872 6566 2c20 6375 722c 2064  fied(ref, cur, d
-00016130: 742c 2064 6a3d 646a 2c20 7330 3d73 302c  t, dj=dj, s0=s0,
-00016140: 204a 3d4a 2c20 7369 673d 7369 672c 2077   J=J, sig=sig, w
-00016150: 6176 656c 6574 3d77 766e 2c20 6e6f 726d  avelet=wvn, norm
-00016160: 616c 697a 653d 5472 7565 290a 0a20 2020  alize=True)..   
-00016170: 2069 6620 756e 7772 6170 666c 6167 3a0a   if unwrapflag:.
-00016180: 2020 2020 2020 2020 7068 6173 6520 3d20          phase = 
-00016190: 6e70 2e75 6e77 7261 7028 6157 4354 2c20  np.unwrap(aWCT, 
-000161a0: 6178 6973 3d2d 3129 2020 2320 6178 6973  axis=-1)  # axis
-000161b0: 3d30 2c20 7570 7772 6170 2061 6c6f 6e67  =0, upwrap along
-000161c0: 2074 696d 653b 2061 7869 733d 2d31 2c20   time; axis=-1, 
-000161d0: 756e 7772 6170 2061 6c6f 6e67 2066 7265  unwrap along fre
-000161e0: 7175 656e 6379 0a20 2020 2065 6c73 653a  quency.    else:
-000161f0: 0a20 2020 2020 2020 2070 6861 7365 203d  .        phase =
-00016200: 2061 5743 540a 0a20 2020 2023 207a 6572   aWCT..    # zer
-00016210: 6f20 6f75 7420 6461 7461 206f 7574 7369  o out data outsi
-00016220: 6465 2066 7265 7175 656e 6379 2062 616e  de frequency ban
-00016230: 640a 2020 2020 6966 2028 666d 6178 203e  d.    if (fmax >
-00016240: 206e 702e 6d61 7828 6672 6571 2929 207c   np.max(freq)) |
-00016250: 2028 666d 6178 203c 3d20 666d 696e 293a   (fmax <= fmin):
-00016260: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00016270: 616c 7565 4572 726f 7228 2241 626f 7274  alueError("Abort
-00016280: 3a20 696e 7075 7420 6672 6571 7565 6e63  : input frequenc
-00016290: 7920 6f75 7420 6f66 206c 696d 6974 7321  y out of limits!
-000162a0: 2229 0a20 2020 2065 6c73 653a 0a20 2020  ").    else:.   
-000162b0: 2020 2020 2066 7265 715f 696e 6469 6e20       freq_indin 
-000162c0: 3d20 6e70 2e77 6865 7265 2828 6672 6571  = np.where((freq
-000162d0: 203e 3d20 666d 696e 2920 2620 2866 7265   >= fmin) & (fre
-000162e0: 7120 3c3d 2066 6d61 7829 295b 305d 0a0a  q <= fmax))[0]..
-000162f0: 2020 2020 2320 666f 6c6c 6f77 204d 5743      # follow MWC
-00016300: 5320 746f 2064 6f20 7477 6f20 7374 6570  S to do two step
-00016310: 7320 6f66 206c 696e 6561 7220 7265 6772  s of linear regr
-00016320: 6573 7369 6f6e 0a20 2020 2069 6620 6e6f  ession.    if no
-00016330: 7420 616c 6c66 7265 713a 0a20 2020 2020  t allfreq:.     
-00016340: 2020 2064 656c 7461 5f74 5f6d 2c20 6465     delta_t_m, de
-00016350: 6c74 615f 745f 756e 6320 3d20 6e70 2e7a  lta_t_unc = np.z
-00016360: 6572 6f73 286e 7074 732c 2064 7479 7065  eros(npts, dtype
-00016370: 3d6e 702e 666c 6f61 7433 3229 2c20 6e70  =np.float32), np
-00016380: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
-00016390: 7065 3d6e 702e 666c 6f61 7433 3229 0a20  pe=np.float32). 
-000163a0: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
-000163b0: 7468 6520 7476 6563 2069 7320 7468 6520  the tvec is the 
-000163c0: 7469 6d65 2077 696e 646f 7720 746f 206d  time window to m
-000163d0: 6561 7375 7265 2064 740a 2020 2020 2020  easure dt.      
-000163e0: 2020 666f 7220 6974 2069 6e20 7261 6e67    for it in rang
-000163f0: 6528 6e70 7473 293a 0a20 2020 2020 2020  e(npts):.       
-00016400: 2020 2020 2077 203d 2031 202f 2057 4354       w = 1 / WCT
-00016410: 5b66 7265 715f 696e 6469 6e2c 2069 745d  [freq_indin, it]
-00016420: 0a20 2020 2020 2020 2020 2020 2077 5b7e  .            w[~
-00016430: 6e70 2e69 7366 696e 6974 6528 7729 5d20  np.isfinite(w)] 
-00016440: 3d20 312e 300a 2020 2020 2020 2020 2020  = 1.0.          
-00016450: 2020 6465 6c74 615f 745f 6d5b 6974 5d2c    delta_t_m[it],
-00016460: 2064 656c 7461 5f74 5f75 6e63 5b69 745d   delta_t_unc[it]
-00016470: 203d 206c 696e 6561 725f 7265 6772 6573   = linear_regres
-00016480: 7369 6f6e 2866 7265 715b 6672 6571 5f69  sion(freq[freq_i
-00016490: 6e64 696e 5d20 2a20 3220 2a20 6e70 2e70  ndin] * 2 * np.p
-000164a0: 692c 2070 6861 7365 5b66 7265 715f 696e  i, phase[freq_in
-000164b0: 6469 6e2c 2069 745d 2c20 7729 0a0a 2020  din, it], w)..  
-000164c0: 2020 2020 2020 2320 6e65 7720 7765 6967        # new weig
-000164d0: 6874 7320 666f 7220 7265 6772 6573 7369  hts for regressi
-000164e0: 6f6e 0a20 2020 2020 2020 2077 3220 3d20  on.        w2 = 
-000164f0: 3120 2f20 6e70 2e6d 6561 6e28 5743 545b  1 / np.mean(WCT[
-00016500: 6672 6571 5f69 6e64 696e 2c20 3a5d 2c20  freq_indin, :], 
-00016510: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
-00016520: 7732 5b7e 6e70 2e69 7366 696e 6974 6528  w2[~np.isfinite(
-00016530: 7732 295d 203d 2031 2e30 0a0a 2020 2020  w2)] = 1.0..    
-00016540: 2020 2020 2320 6e6f 7720 7573 6520 6474      # now use dt
-00016550: 2061 6e64 2074 2074 6f20 6765 7420 6476   and t to get dv
-00016560: 2f76 0a20 2020 2020 2020 2069 6620 6c65  /v.        if le
-00016570: 6e28 7732 2920 3e20 323a 0a20 2020 2020  n(w2) > 2:.     
-00016580: 2020 2020 2020 2069 6620 6e6f 7420 6e70         if not np
-00016590: 2e61 6e79 2864 656c 7461 5f74 5f6d 293a  .any(delta_t_m):
-000165a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165b0: 2064 7676 2c20 6572 7220 3d20 6e70 2e6e   dvv, err = np.n
-000165c0: 616e 2c20 6e70 2e6e 616e 0a20 2020 2020  an, np.nan.     
-000165d0: 2020 2020 2020 206d 2c20 656d 203d 206c         m, em = l
-000165e0: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
-000165f0: 2874 7665 632c 2064 656c 7461 5f74 5f6d  (tvec, delta_t_m
-00016600: 2c20 7732 2c20 696e 7465 7263 6570 745f  , w2, intercept_
-00016610: 6f72 6967 696e 3d54 7275 6529 0a20 2020  origin=True).   
-00016620: 2020 2020 2020 2020 2064 7676 2c20 6572           dvv, er
-00016630: 7220 3d20 2d6d 2c20 656d 0a20 2020 2020  r = -m, em.     
-00016640: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00016650: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00016660: 6728 226e 6f74 2065 6e6f 7567 6820 706f  g("not enough po
-00016670: 696e 7473 2074 6f20 6573 7469 6d61 7465  ints to estimate
-00016680: 2064 762f 7620 666f 7220 7774 7322 290a   dv/v for wts").
-00016690: 2020 2020 2020 2020 2020 2020 6476 762c              dvv,
-000166a0: 2065 7272 203d 206e 702e 6e61 6e2c 206e   err = np.nan, n
-000166b0: 702e 6e61 6e0a 0a20 2020 2020 2020 2072  p.nan..        r
-000166c0: 6574 7572 6e20 6476 7620 2a20 3130 302c  eturn dvv * 100,
-000166d0: 2065 7272 202a 2031 3030 0a0a 2020 2020   err * 100..    
-000166e0: 2320 636f 6e76 6572 7420 7068 6173 6520  # convert phase 
-000166f0: 6469 7265 6374 6c79 2074 6f20 6465 6c74  directly to delt
-00016700: 615f 7420 666f 7220 616c 6c20 6672 6571  a_t for all freq
-00016710: 7565 6e63 6965 730a 2020 2020 656c 7365  uencies.    else
-00016720: 3a0a 2020 2020 2020 2020 2320 636f 6e76  :.        # conv
-00016730: 6572 7420 7068 6173 6520 6465 6c61 7920  ert phase delay 
-00016740: 746f 2074 696d 6520 6465 6c61 790a 2020  to time delay.  
-00016750: 2020 2020 2020 6465 6c74 615f 7420 3d20        delta_t = 
-00016760: 7068 6173 6520 2f20 2832 202a 206e 702e  phase / (2 * np.
-00016770: 7069 202a 2066 7265 715b 3a2c 204e 6f6e  pi * freq[:, Non
-00016780: 655d 2920 2023 206e 6f72 6d61 6c69 7a65  e])  # normalize
-00016790: 2070 6861 7365 2062 7920 2832 2a70 692a   phase by (2*pi*
-000167a0: 6672 6571 7565 6e63 7929 0a20 2020 2020  frequency).     
-000167b0: 2020 2064 7676 2c20 6572 7220 3d20 6e70     dvv, err = np
-000167c0: 2e7a 6572 6f73 2866 7265 715f 696e 6469  .zeros(freq_indi
-000167d0: 6e2e 7368 6170 6529 2c20 6e70 2e7a 6572  n.shape), np.zer
-000167e0: 6f73 2866 7265 715f 696e 6469 6e2e 7368  os(freq_indin.sh
-000167f0: 6170 6529 0a0a 2020 2020 2020 2020 2320  ape)..        # 
-00016800: 6c6f 6f70 2074 6872 6f75 6768 2066 7265  loop through fre
-00016810: 7120 666f 7220 6c69 6e65 6172 2072 6567  q for linear reg
-00016820: 7265 7373 696f 6e0a 2020 2020 2020 2020  ression.        
-00016830: 666f 7220 6969 2c20 6966 7265 7120 696e  for ii, ifreq in
-00016840: 2065 6e75 6d65 7261 7465 2866 7265 715f   enumerate(freq_
-00016850: 696e 6469 6e29 3a0a 2020 2020 2020 2020  indin):.        
-00016860: 2020 2020 6966 206c 656e 2874 7665 6329      if len(tvec)
-00016870: 203e 2032 3a0a 2020 2020 2020 2020 2020   > 2:.          
-00016880: 2020 2020 2020 6966 206e 6f74 206e 702e        if not np.
-00016890: 616e 7928 6465 6c74 615f 745b 6966 7265  any(delta_t[ifre
-000168a0: 715d 293a 0a20 2020 2020 2020 2020 2020  q]):.           
-000168b0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000168c0: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-000168d0: 2020 2023 2068 6f77 2074 6f20 6265 7474     # how to bett
-000168e0: 6572 2061 7070 726f 6163 6820 7468 6520  er approach the 
-000168f0: 756e 6365 7274 6169 6e74 7920 6f66 2064  uncertainty of d
-00016900: 656c 7461 5f74 0a20 2020 2020 2020 2020  elta_t.         
-00016910: 2020 2020 2020 2077 203d 2031 202f 2057         w = 1 / W
-00016920: 4354 5b69 6672 6571 5d0a 2020 2020 2020  CT[ifreq].      
-00016930: 2020 2020 2020 2020 2020 775b 7e6e 702e            w[~np.
-00016940: 6973 6669 6e69 7465 2877 295d 203d 2031  isfinite(w)] = 1
-00016950: 2e30 0a0a 2020 2020 2020 2020 2020 2020  .0..            
-00016960: 2020 2020 2320 6d2c 2061 2c20 656d 2c20      # m, a, em, 
-00016970: 6561 203d 206c 696e 6561 725f 7265 6772  ea = linear_regr
-00016980: 6573 7369 6f6e 2874 696d 655f 6178 6973  ession(time_axis
-00016990: 5b69 6e64 785d 2c20 6465 6c74 615f 745b  [indx], delta_t[
-000169a0: 696e 6478 5d2c 2077 2c20 696e 7465 7263  indx], w, interc
-000169b0: 6570 745f 6f72 6967 696e 3d46 616c 7365  ept_origin=False
-000169c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000169d0: 2020 6d2c 2065 6d20 3d20 6c69 6e65 6172    m, em = linear
-000169e0: 5f72 6567 7265 7373 696f 6e28 7476 6563  _regression(tvec
-000169f0: 2c20 6465 6c74 615f 745b 6966 7265 715d  , delta_t[ifreq]
-00016a00: 2c20 772c 2069 6e74 6572 6365 7074 5f6f  , w, intercept_o
-00016a10: 7269 6769 6e3d 5472 7565 290a 2020 2020  rigin=True).    
-00016a20: 2020 2020 2020 2020 2020 2020 6476 765b              dvv[
-00016a30: 6969 5d2c 2065 7272 5b69 695d 203d 202d  ii], err[ii] = -
-00016a40: 6d2c 2065 6d0a 2020 2020 2020 2020 2020  m, em.          
-00016a50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00016a60: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00016a70: 6562 7567 2822 6e6f 7420 656e 6f75 6768  ebug("not enough
-00016a80: 2070 6f69 6e74 7320 746f 2065 7374 696d   points to estim
-00016a90: 6174 6520 6476 2f76 2066 6f72 2077 7473  ate dv/v for wts
-00016aa0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00016ab0: 2020 2064 7676 5b69 695d 2c20 6572 725b     dvv[ii], err[
-00016ac0: 6969 5d20 3d20 6e70 2e6e 616e 2c20 6e70  ii] = np.nan, np
-00016ad0: 2e6e 616e 0a0a 2020 2020 2020 2020 7265  .nan..        re
-00016ae0: 7475 726e 2066 7265 715b 6672 6571 5f69  turn freq[freq_i
-00016af0: 6e64 696e 5d2c 2064 7676 202a 2031 3030  ndin], dvv * 100
-00016b00: 2c20 6572 7220 2a20 3130 300a 0a0a 6465  , err * 100...de
-00016b10: 6620 7774 735f 6476 7628 0a20 2020 2072  f wts_dvv(.    r
-00016b20: 6566 2c0a 2020 2020 6375 722c 0a20 2020  ef,.    cur,.   
-00016b30: 2061 6c6c 6672 6571 2c0a 2020 2020 7061   allfreq,.    pa
-00016b40: 7261 2c0a 2020 2020 6476 5f72 616e 6765  ra,.    dv_range
-00016b50: 2c0a 2020 2020 6e62 7472 6961 6c2c 0a20  ,.    nbtrial,. 
-00016b60: 2020 2064 6a3d 3120 2f20 3132 2c0a 2020     dj=1 / 12,.  
-00016b70: 2020 7330 3d2d 312c 0a20 2020 204a 3d2d    s0=-1,.    J=-
-00016b80: 312c 0a20 2020 2077 766e 3d22 6d6f 726c  1,.    wvn="morl
-00016b90: 6574 222c 0a20 2020 206e 6f72 6d61 6c69  et",.    normali
-00016ba0: 7a65 3d54 7275 652c 0a29 3a0a 2020 2020  ze=True,.):.    
-00016bb0: 2222 220a 2020 2020 4170 706c 7920 7374  """.    Apply st
-00016bc0: 7265 7463 6869 6e67 206d 6574 686f 6420  retching method 
-00016bd0: 746f 2063 6f6e 7469 6e75 6f75 7320 7761  to continuous wa
-00016be0: 7665 6c65 7420 7472 616e 7366 6f72 6d61  velet transforma
-00016bf0: 7469 6f6e 2028 4357 5429 206f 6620 7369  tion (CWT) of si
-00016c00: 676e 616c 730a 2020 2020 666f 7220 616c  gnals.    for al
-00016c10: 6c20 6672 6571 7565 6369 6573 2069 6e20  l frequecies in 
-00016c20: 616e 2069 6e74 6572 6573 7420 7261 6e67  an interest rang
-00016c30: 650a 0a20 2020 2050 6172 616d 6574 6572  e..    Parameter
-00016c40: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00016c50: 2d2d 2d2d 0a20 2020 2072 6566 3a20 5468  ----.    ref: Th
-00016c60: 6520 2252 6566 6572 656e 6365 2220 7469  e "Reference" ti
-00016c70: 6d65 7365 7269 6573 2028 6e75 6d70 792e  meseries (numpy.
-00016c80: 6e64 6172 7261 7929 0a20 2020 2063 7572  ndarray).    cur
-00016c90: 3a20 5468 6520 2243 7572 7265 6e74 2220  : The "Current" 
-00016ca0: 7469 6d65 7365 7269 6573 2028 6e75 6d70  timeseries (nump
-00016cb0: 792e 6e64 6172 7261 7929 0a20 2020 2061  y.ndarray).    a
-00016cc0: 6c6c 6672 6571 3a20 6120 626f 6f6c 656e  llfreq: a boolen
-00016cd0: 2076 6172 6961 626c 6520 746f 206d 616b   variable to mak
-00016ce0: 6520 6d65 6173 7572 656d 656e 7473 206f  e measurements o
-00016cf0: 6e20 616c 6c20 6672 6571 7565 6e63 7920  n all frequency 
-00016d00: 7261 6e67 6520 6f72 206e 6f74 0a20 2020  range or not.   
-00016d10: 2070 6172 613a 2061 2064 6963 7420 636f   para: a dict co
-00016d20: 6e74 6169 6e69 6e67 2066 7265 712f 7469  ntaining freq/ti
-00016d30: 6d65 2069 6e66 6f20 6f66 2074 6865 2064  me info of the d
-00016d40: 6174 6120 6d61 7472 6978 0a20 2020 2064  ata matrix.    d
-00016d50: 765f 7261 6e67 653a 2061 6273 6f6c 7574  v_range: absolut
-00016d60: 6520 626f 756e 6420 666f 7220 7468 6520  e bound for the 
-00016d70: 7665 6c6f 6369 7479 2076 6172 6961 7469  velocity variati
-00016d80: 6f6e 3b20 6578 616d 706c 653a 2064 763d  on; example: dv=
-00016d90: 302e 3033 2066 6f72 205b 2d33 2c33 5d25  0.03 for [-3,3]%
-00016da0: 0a20 2020 206f 6620 7265 6c61 7469 7665  .    of relative
-00016db0: 2076 656c 6f63 6974 7920 6368 616e 6765   velocity change
-00016dc0: 2028 666c 6f61 7429 0a20 2020 206e 6274   (float).    nbt
-00016dd0: 7269 616c 3a20 6e75 6d62 6572 206f 6620  rial: number of 
-00016de0: 7374 7265 7463 6869 6e67 2063 6f65 6666  stretching coeff
-00016df0: 6963 6965 6e74 2062 6574 7765 656e 2064  icient between d
-00016e00: 766d 696e 2061 6e64 2064 766d 6178 2c20  vmin and dvmax, 
-00016e10: 6e6f 206e 6565 6420 746f 2062 6520 6869  no need to be hi
-00016e20: 6768 6572 2074 6861 6e20 3130 3020 2028  gher than 100  (
-00016e30: 666c 6f61 7429 0a20 2020 2064 6a2c 2073  float).    dj, s
-00016e40: 302c 204a 2c20 7369 672c 2077 766e 3a20  0, J, sig, wvn: 
-00016e50: 636f 6d6d 6f6e 2070 6172 616d 6574 6572  common parameter
-00016e60: 7320 7573 6564 2069 6e20 2777 6176 656c  s used in 'wavel
-00016e70: 6574 2e77 6374 270a 2020 2020 6e6f 726d  et.wct'.    norm
-00016e80: 616c 697a 653a 206e 6f72 6d61 6c69 7a65  alize: normalize
-00016e90: 2074 6865 2077 6176 656c 6574 2073 7065   the wavelet spe
-00016ea0: 6374 7275 6d20 6f72 206e 6f74 2e20 4465  ctrum or not. De
-00016eb0: 6661 756c 7420 6973 2054 7275 650a 0a20  fault is True.. 
-00016ec0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-00016ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016ee0: 2d2d 0a20 2020 2064 7676 3a20 6573 7469  --.    dvv: esti
-00016ef0: 6d61 7465 6420 6476 2f76 0a20 2020 2065  mated dv/v.    e
-00016f00: 7272 3a20 6572 726f 7220 6f66 2064 762f  rr: error of dv/
-00016f10: 7620 6573 7469 6d61 7469 6f6e 0a0a 2020  v estimation..  
-00016f20: 2020 5772 6974 7465 6e20 6279 2043 6f6e    Written by Con
-00016f30: 6763 6f6e 6720 5975 616e 2028 3330 204a  gcong Yuan (30 J
-00016f40: 756e 2c20 3230 3139 290a 2020 2020 2222  un, 2019).    ""
-00016f50: 220a 2020 2020 2320 636f 6d6d 6f6e 2076  ".    # common v
-00016f60: 6172 6961 626c 6573 0a20 2020 2066 7265  ariables.    fre
-00016f70: 7120 3d20 7061 7261 5b22 6672 6571 225d  q = para["freq"]
-00016f80: 0a20 2020 2064 7420 3d20 7061 7261 5b22  .    dt = para["
-00016f90: 6474 225d 0a20 2020 2066 6d69 6e20 3d20  dt"].    fmin = 
-00016fa0: 6e70 2e6d 696e 2866 7265 7129 0a20 2020  np.min(freq).   
-00016fb0: 2066 6d61 7820 3d20 6e70 2e6d 6178 2866   fmax = np.max(f
-00016fc0: 7265 7129 0a0a 2020 2020 2320 6170 706c  req)..    # appl
-00016fd0: 7920 6377 7420 6f6e 2074 776f 2074 7261  y cwt on two tra
-00016fe0: 6365 730a 2020 2020 6377 7431 2c20 736a  ces.    cwt1, sj
-00016ff0: 2c20 6672 6571 2c20 636f 692c 205f 2c20  , freq, coi, _, 
-00017000: 5f20 3d20 7079 6377 742e 6377 7428 6375  _ = pycwt.cwt(cu
-00017010: 722c 2064 742c 2064 6a2c 2073 302c 204a  r, dt, dj, s0, J
-00017020: 2c20 7776 6e29 0a20 2020 2063 7774 322c  , wvn).    cwt2,
-00017030: 2073 6a2c 2066 7265 712c 2063 6f69 2c20   sj, freq, coi, 
-00017040: 5f2c 205f 203d 2070 7963 7774 2e63 7774  _, _ = pycwt.cwt
-00017050: 2872 6566 2c20 6474 2c20 646a 2c20 7330  (ref, dt, dj, s0
-00017060: 2c20 4a2c 2077 766e 290a 0a20 2020 2023  , J, wvn)..    #
-00017070: 2065 7874 7261 6374 2072 6561 6c20 7661   extract real va
-00017080: 6c75 6573 206f 6620 6377 740a 2020 2020  lues of cwt.    
-00017090: 7263 7774 312c 2072 6377 7432 203d 206e  rcwt1, rcwt2 = n
-000170a0: 702e 7265 616c 2863 7774 3129 2c20 6e70  p.real(cwt1), np
-000170b0: 2e72 6561 6c28 6377 7432 290a 0a20 2020  .real(cwt2)..   
-000170c0: 2023 207a 6572 6f20 6f75 7420 6461 7461   # zero out data
-000170d0: 206f 7574 7369 6465 2066 7265 7175 656e   outside frequen
-000170e0: 6379 2062 616e 640a 2020 2020 6966 2028  cy band.    if (
-000170f0: 666d 6178 203e 206e 702e 6d61 7828 6672  fmax > np.max(fr
-00017100: 6571 2929 207c 2028 666d 6178 203c 3d20  eq)) | (fmax <= 
-00017110: 666d 696e 293a 0a20 2020 2020 2020 2072  fmin):.        r
-00017120: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00017130: 2241 626f 7274 3a20 696e 7075 7420 6672  "Abort: input fr
-00017140: 6571 7565 6e63 7920 6f75 7420 6f66 206c  equency out of l
-00017150: 696d 6974 7321 2229 0a20 2020 2065 6c73  imits!").    els
-00017160: 653a 0a20 2020 2020 2020 2066 7265 715f  e:.        freq_
-00017170: 696e 6469 6e20 3d20 6e70 2e77 6865 7265  indin = np.where
-00017180: 2828 6672 6571 203e 3d20 666d 696e 2920  ((freq >= fmin) 
-00017190: 2620 2866 7265 7120 3c3d 2066 6d61 7829  & (freq <= fmax)
-000171a0: 295b 305d 0a0a 2020 2020 2320 636f 6e76  )[0]..    # conv
-000171b0: 6572 7420 7761 7665 6c65 7420 646f 6d61  ert wavelet doma
-000171c0: 696e 2062 6163 6b20 746f 2074 696d 6520  in back to time 
-000171d0: 646f 6d61 696e 2028 7e66 696c 7465 7269  domain (~filteri
-000171e0: 6e67 290a 2020 2020 6966 206e 6f74 2061  ng).    if not a
-000171f0: 6c6c 6672 6571 3a0a 2020 2020 2020 2020  llfreq:.        
-00017200: 2320 696e 7665 7273 6520 6377 7420 746f  # inverse cwt to
-00017210: 2074 696d 6520 646f 6d61 696e 0a20 2020   time domain.   
-00017220: 2020 2020 2069 6377 7431 203d 2070 7963       icwt1 = pyc
-00017230: 7774 2e69 6377 7428 6377 7431 5b66 7265  wt.icwt(cwt1[fre
-00017240: 715f 696e 6469 6e5d 2c20 736a 5b66 7265  q_indin], sj[fre
-00017250: 715f 696e 6469 6e5d 2c20 6474 2c20 646a  q_indin], dt, dj
-00017260: 2c20 7776 6e29 0a20 2020 2020 2020 2069  , wvn).        i
-00017270: 6377 7432 203d 2070 7963 7774 2e69 6377  cwt2 = pycwt.icw
-00017280: 7428 6377 7432 5b66 7265 715f 696e 6469  t(cwt2[freq_indi
-00017290: 6e5d 2c20 736a 5b66 7265 715f 696e 6469  n], sj[freq_indi
-000172a0: 6e5d 2c20 6474 2c20 646a 2c20 7776 6e29  n], dt, dj, wvn)
-000172b0: 0a0a 2020 2020 2020 2020 2320 6173 7375  ..        # assu
-000172c0: 6d65 2061 6c6c 2074 696d 6520 7769 6e64  me all time wind
-000172d0: 6f77 2069 7320 7573 6564 0a20 2020 2020  ow is used.     
-000172e0: 2020 2077 6377 7431 2c20 7763 7774 3220     wcwt1, wcwt2 
-000172f0: 3d20 6e70 2e72 6561 6c28 6963 7774 3129  = np.real(icwt1)
-00017300: 2c20 6e70 2e72 6561 6c28 6963 7774 3229  , np.real(icwt2)
-00017310: 0a0a 2020 2020 2020 2020 2320 4e6f 726d  ..        # Norm
-00017320: 616c 697a 6573 2062 6f74 6820 7369 676e  alizes both sign
-00017330: 616c 732c 2069 6620 6170 7072 6f70 7269  als, if appropri
-00017340: 6174 652e 0a20 2020 2020 2020 2069 6620  ate..        if 
-00017350: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-00017360: 2020 2020 2020 206e 6377 7431 203d 2028         ncwt1 = (
-00017370: 7763 7774 3120 2d20 7763 7774 312e 6d65  wcwt1 - wcwt1.me
-00017380: 616e 2829 2920 2f20 7763 7774 312e 7374  an()) / wcwt1.st
-00017390: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-000173a0: 6e63 7774 3220 3d20 2877 6377 7432 202d  ncwt2 = (wcwt2 -
-000173b0: 2077 6377 7432 2e6d 6561 6e28 2929 202f   wcwt2.mean()) /
-000173c0: 2077 6377 7432 2e73 7464 2829 0a20 2020   wcwt2.std().   
-000173d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000173e0: 2020 2020 2020 206e 6377 7431 203d 2077         ncwt1 = w
-000173f0: 6377 7431 0a20 2020 2020 2020 2020 2020  cwt1.           
-00017400: 206e 6377 7432 203d 2077 6377 7432 0a0a   ncwt2 = wcwt2..
-00017410: 2020 2020 2020 2020 2320 7275 6e20 7374          # run st
-00017420: 7265 7463 6869 6e67 0a20 2020 2020 2020  retching.       
-00017430: 2064 7676 2c20 6572 722c 2063 632c 2063   dvv, err, cc, c
-00017440: 6470 203d 2073 7472 6574 6368 696e 6728  dp = stretching(
-00017450: 6e63 7774 322c 206e 6377 7431 2c20 6476  ncwt2, ncwt1, dv
-00017460: 5f72 616e 6765 2c20 6e62 7472 6961 6c2c  _range, nbtrial,
-00017470: 2070 6172 6129 0a20 2020 2020 2020 2072   para).        r
-00017480: 6574 7572 6e20 6476 762c 2065 7272 0a0a  eturn dvv, err..
-00017490: 2020 2020 2320 6469 7265 6374 6c79 2074      # directly t
-000174a0: 616b 6520 6164 7661 6e74 6167 6520 6f66  ake advantage of
-000174b0: 2074 6865 0a20 2020 2065 6c73 653a 0a20   the.    else:. 
-000174c0: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
-000174d0: 697a 6520 7661 7269 6162 6c65 0a20 2020  ize variable.   
-000174e0: 2020 2020 206e 6672 6571 203d 206c 656e       nfreq = len
-000174f0: 2866 7265 715f 696e 6469 6e29 0a20 2020  (freq_indin).   
-00017500: 2020 2020 2064 7676 2c20 6363 2c20 6364       dvv, cc, cd
-00017510: 702c 2065 7272 203d 2028 0a20 2020 2020  p, err = (.     
-00017520: 2020 2020 2020 206e 702e 7a65 726f 7328         np.zeros(
-00017530: 6e66 7265 712c 2064 7479 7065 3d6e 702e  nfreq, dtype=np.
-00017540: 666c 6f61 7433 3229 2c0a 2020 2020 2020  float32),.      
-00017550: 2020 2020 2020 6e70 2e7a 6572 6f73 286e        np.zeros(n
-00017560: 6672 6571 2c20 6474 7970 653d 6e70 2e66  freq, dtype=np.f
-00017570: 6c6f 6174 3332 292c 0a20 2020 2020 2020  loat32),.       
-00017580: 2020 2020 206e 702e 7a65 726f 7328 6e66       np.zeros(nf
-00017590: 7265 712c 2064 7479 7065 3d6e 702e 666c  req, dtype=np.fl
-000175a0: 6f61 7433 3229 2c0a 2020 2020 2020 2020  oat32),.        
-000175b0: 2020 2020 6e70 2e7a 6572 6f73 286e 6672      np.zeros(nfr
-000175c0: 6571 2c20 6474 7970 653d 6e70 2e66 6c6f  eq, dtype=np.flo
-000175d0: 6174 3332 292c 0a20 2020 2020 2020 2029  at32),.        )
-000175e0: 0a0a 2020 2020 2020 2020 2320 6c6f 6f70  ..        # loop
-000175f0: 2074 6872 6f75 6768 2065 6163 6820 6672   through each fr
-00017600: 6571 0a20 2020 2020 2020 2066 6f72 2069  eq.        for i
-00017610: 692c 2069 6672 6571 2069 6e20 656e 756d  i, ifreq in enum
-00017620: 6572 6174 6528 6672 6571 5f69 6e64 696e  erate(freq_indin
-00017630: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00017640: 2070 7265 7061 7265 2077 696e 646f 7765   prepare windowe
-00017650: 6420 6461 7461 0a20 2020 2020 2020 2020  d data.         
-00017660: 2020 2077 6377 7431 2c20 7763 7774 3220     wcwt1, wcwt2 
-00017670: 3d20 7263 7774 315b 6966 7265 715d 2c20  = rcwt1[ifreq], 
-00017680: 7263 7774 325b 6966 7265 715d 0a0a 2020  rcwt2[ifreq]..  
-00017690: 2020 2020 2020 2020 2020 2320 4e6f 726d            # Norm
-000176a0: 616c 697a 6573 2062 6f74 6820 7369 676e  alizes both sign
-000176b0: 616c 732c 2069 6620 6170 7072 6f70 7269  als, if appropri
-000176c0: 6174 652e 0a20 2020 2020 2020 2020 2020  ate..           
-000176d0: 2069 6620 6e6f 726d 616c 697a 653a 0a20   if normalize:. 
-000176e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000176f0: 6377 7431 203d 2028 7763 7774 3120 2d20  cwt1 = (wcwt1 - 
-00017700: 7763 7774 312e 6d65 616e 2829 2920 2f20  wcwt1.mean()) / 
-00017710: 7763 7774 312e 7374 6428 290a 2020 2020  wcwt1.std().    
-00017720: 2020 2020 2020 2020 2020 2020 6e63 7774              ncwt
-00017730: 3220 3d20 2877 6377 7432 202d 2077 6377  2 = (wcwt2 - wcw
-00017740: 7432 2e6d 6561 6e28 2929 202f 2077 6377  t2.mean()) / wcw
-00017750: 7432 2e73 7464 2829 0a20 2020 2020 2020  t2.std().       
-00017760: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00017770: 2020 2020 2020 2020 2020 206e 6377 7431             ncwt1
-00017780: 203d 2077 6377 7431 0a20 2020 2020 2020   = wcwt1.       
-00017790: 2020 2020 2020 2020 206e 6377 7432 203d           ncwt2 =
-000177a0: 2077 6377 7432 0a0a 2020 2020 2020 2020   wcwt2..        
-000177b0: 2020 2020 2320 7275 6e20 7374 7265 7463      # run stretc
-000177c0: 6869 6e67 0a20 2020 2020 2020 2020 2020  hing.           
-000177d0: 2064 762c 2065 7272 6f72 2c20 6331 2c20   dv, error, c1, 
-000177e0: 6332 203d 2073 7472 6574 6368 696e 6728  c2 = stretching(
-000177f0: 6e63 7774 322c 206e 6377 7431 2c20 6476  ncwt2, ncwt1, dv
-00017800: 5f72 616e 6765 2c20 6e62 7472 6961 6c2c  _range, nbtrial,
-00017810: 2070 6172 6129 0a20 2020 2020 2020 2020   para).         
-00017820: 2020 2064 7676 5b69 695d 2c20 6363 5b69     dvv[ii], cc[i
-00017830: 695d 2c20 6364 705b 6969 5d2c 2065 7272  i], cdp[ii], err
-00017840: 5b69 695d 203d 2064 762c 2063 312c 2063  [ii] = dv, c1, c
-00017850: 322c 2065 7272 6f72 0a0a 2020 2020 2020  2, error..      
-00017860: 2020 7265 7475 726e 2066 7265 715b 6672    return freq[fr
-00017870: 6571 5f69 6e64 696e 5d2c 2064 7676 2c20  eq_indin], dvv, 
-00017880: 6572 720a 0a0a 6465 6620 7774 6474 775f  err...def wtdtw_
-00017890: 616c 6c66 7265 7128 0a20 2020 2072 6566  allfreq(.    ref
-000178a0: 2c0a 2020 2020 6375 722c 0a20 2020 2061  ,.    cur,.    a
-000178b0: 6c6c 6672 6571 2c0a 2020 2020 7061 7261  llfreq,.    para
-000178c0: 2c0a 2020 2020 6d61 784c 6167 2c0a 2020  ,.    maxLag,.  
-000178d0: 2020 622c 0a20 2020 2064 6972 6563 7469    b,.    directi
-000178e0: 6f6e 2c0a 2020 2020 646a 3d31 202f 2031  on,.    dj=1 / 1
-000178f0: 322c 0a20 2020 2073 303d 2d31 2c0a 2020  2,.    s0=-1,.  
-00017900: 2020 4a3d 2d31 2c0a 2020 2020 7776 6e3d    J=-1,.    wvn=
-00017910: 226d 6f72 6c65 7422 2c0a 2020 2020 6e6f  "morlet",.    no
-00017920: 726d 616c 697a 653d 5472 7565 2c0a 293a  rmalize=True,.):
-00017930: 0a20 2020 2022 2222 0a20 2020 2041 7070  .    """.    App
-00017940: 6c79 2064 796e 616d 6963 2074 696d 6520  ly dynamic time 
-00017950: 7761 7270 696e 6720 6d65 7468 6f64 2074  warping method t
-00017960: 6f20 636f 6e74 696e 756f 7573 2077 6176  o continuous wav
-00017970: 656c 6574 2074 7261 6e73 666f 726d 6174  elet transformat
-00017980: 696f 6e20 2843 5754 2920 6f66 2073 6967  ion (CWT) of sig
-00017990: 6e61 6c73 0a20 2020 2066 6f72 2061 6c6c  nals.    for all
-000179a0: 2066 7265 7175 6563 6965 7320 696e 2061   frequecies in a
-000179b0: 6e20 696e 7465 7265 7374 2072 616e 6765  n interest range
-000179c0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-000179d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-000179e0: 2d2d 2d0a 2020 2020 7265 663a 2054 6865  ---.    ref: The
-000179f0: 2022 5265 6665 7265 6e63 6522 2074 696d   "Reference" tim
-00017a00: 6573 6572 6965 7320 286e 756d 7079 2e6e  eseries (numpy.n
-00017a10: 6461 7272 6179 290a 2020 2020 6375 723a  darray).    cur:
-00017a20: 2054 6865 2022 4375 7272 656e 7422 2074   The "Current" t
-00017a30: 696d 6573 6572 6965 7320 286e 756d 7079  imeseries (numpy
-00017a40: 2e6e 6461 7272 6179 290a 2020 2020 616c  .ndarray).    al
-00017a50: 6c66 7265 713a 2061 2062 6f6f 6c65 6e20  lfreq: a boolen 
-00017a60: 7661 7269 6162 6c65 2074 6f20 6d61 6b65  variable to make
-00017a70: 206d 6561 7375 7265 6d65 6e74 7320 6f6e   measurements on
-00017a80: 2061 6c6c 2066 7265 7175 656e 6379 2072   all frequency r
-00017a90: 616e 6765 206f 7220 6e6f 740a 2020 2020  ange or not.    
-00017aa0: 6d61 784c 6167 3a20 6d61 7820 6e75 6d62  maxLag: max numb
-00017ab0: 6572 206f 6620 706f 696e 7473 2074 6f20  er of points to 
-00017ac0: 7365 6172 6368 2066 6f72 7761 7264 2061  search forward a
-00017ad0: 6e64 2062 6163 6b77 6172 642e 0a20 2020  nd backward..   
-00017ae0: 2062 3a20 622d 7661 6c75 6520 746f 206c   b: b-value to l
-00017af0: 696d 6974 2073 7472 6169 6e2c 2077 6869  imit strain, whi
-00017b00: 6368 2069 7320 746f 206c 696d 6974 2074  ch is to limit t
-00017b10: 6865 206d 6178 696d 756d 2076 656c 6f63  he maximum veloc
-00017b20: 6974 7920 7065 7274 7572 6261 7469 6f6e  ity perturbation
-00017b30: 2e0a 2020 2020 5365 6520 6571 7561 7469  ..    See equati
-00017b40: 6f6e 2031 3120 696e 2028 4d69 6b65 7365  on 11 in (Mikese
-00017b50: 6c6c 2065 7420 616c 2e20 3230 3135 290a  ll et al. 2015).
-00017b60: 2020 2020 6469 7265 6374 696f 6e3a 2064      direction: d
-00017b70: 6972 6563 7469 6f6e 2074 6f20 6163 6375  irection to accu
-00017b80: 6d75 6c61 7465 2065 7272 6f72 7320 2831  mulate errors (1
-00017b90: 3d66 6f72 7761 7264 2c20 2d31 3d62 6163  =forward, -1=bac
-00017ba0: 6b77 6172 6429 0a20 2020 2064 6a2c 2073  kward).    dj, s
-00017bb0: 302c 204a 2c20 7369 672c 2077 766e 3a20  0, J, sig, wvn: 
-00017bc0: 636f 6d6d 6f6e 2070 6172 616d 6574 6572  common parameter
-00017bd0: 7320 7573 6564 2069 6e20 2777 6176 656c  s used in 'wavel
-00017be0: 6574 2e77 6374 270a 2020 2020 6e6f 726d  et.wct'.    norm
-00017bf0: 616c 697a 653a 206e 6f72 6d61 6c69 7a65  alize: normalize
-00017c00: 2074 6865 2077 6176 656c 6574 2073 7065   the wavelet spe
-00017c10: 6374 7275 6d20 6f72 206e 6f74 2e20 4465  ctrum or not. De
-00017c20: 6661 756c 7420 6973 2054 7275 650a 0a20  fault is True.. 
-00017c30: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-00017c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017c50: 2d2d 0a20 2020 2064 7676 3a20 6573 7469  --.    dvv: esti
-00017c60: 6d61 7465 6420 6476 2f76 0a20 2020 2065  mated dv/v.    e
-00017c70: 7272 3a20 6572 726f 7220 6f66 2064 762f  rr: error of dv/
-00017c80: 7620 6573 7469 6d61 7469 6f6e 0a0a 2020  v estimation..  
-00017c90: 2020 5772 6974 7465 6e20 6279 2043 6f6e    Written by Con
-00017ca0: 6763 6f6e 6720 5975 616e 2028 3330 204a  gcong Yuan (30 J
-00017cb0: 756e 2c20 3230 3139 290a 2020 2020 2222  un, 2019).    ""
-00017cc0: 220a 2020 2020 2320 636f 6d6d 6f6e 2076  ".    # common v
-00017cd0: 6172 6961 626c 6573 0a20 2020 2066 7265  ariables.    fre
-00017ce0: 7120 3d20 7061 7261 5b22 6672 6571 225d  q = para["freq"]
-00017cf0: 0a20 2020 2064 7420 3d20 7061 7261 5b22  .    dt = para["
-00017d00: 6474 225d 0a20 2020 2066 6d69 6e20 3d20  dt"].    fmin = 
-00017d10: 6e70 2e6d 696e 2866 7265 7129 0a20 2020  np.min(freq).   
-00017d20: 2066 6d61 7820 3d20 6e70 2e6d 6178 2866   fmax = np.max(f
-00017d30: 7265 7129 0a0a 2020 2020 2320 6170 706c  req)..    # appl
-00017d40: 7920 6377 7420 6f6e 2074 776f 2074 7261  y cwt on two tra
-00017d50: 6365 730a 2020 2020 6377 7431 2c20 736a  ces.    cwt1, sj
-00017d60: 2c20 6672 6571 2c20 636f 692c 205f 2c20  , freq, coi, _, 
-00017d70: 5f20 3d20 7079 6377 742e 6377 7428 6375  _ = pycwt.cwt(cu
-00017d80: 722c 2064 742c 2064 6a2c 2073 302c 204a  r, dt, dj, s0, J
-00017d90: 2c20 7776 6e29 0a20 2020 2063 7774 322c  , wvn).    cwt2,
-00017da0: 2073 6a2c 2066 7265 712c 2063 6f69 2c20   sj, freq, coi, 
-00017db0: 5f2c 205f 203d 2070 7963 7774 2e63 7774  _, _ = pycwt.cwt
-00017dc0: 2872 6566 2c20 6474 2c20 646a 2c20 7330  (ref, dt, dj, s0
-00017dd0: 2c20 4a2c 2077 766e 290a 0a20 2020 2023  , J, wvn)..    #
-00017de0: 2065 7874 7261 6374 2072 6561 6c20 7661   extract real va
-00017df0: 6c75 6573 206f 6620 6377 740a 2020 2020  lues of cwt.    
-00017e00: 7263 7774 312c 2072 6377 7432 203d 206e  rcwt1, rcwt2 = n
-00017e10: 702e 7265 616c 2863 7774 3129 2c20 6e70  p.real(cwt1), np
-00017e20: 2e72 6561 6c28 6377 7432 290a 0a20 2020  .real(cwt2)..   
-00017e30: 2023 207a 6572 6f20 6f75 7420 636f 6e65   # zero out cone
-00017e40: 206f 6620 696e 666c 7565 6e63 6520 616e   of influence an
-00017e50: 6420 6461 7461 206f 7574 7369 6465 2066  d data outside f
-00017e60: 7265 7175 656e 6379 2062 616e 640a 2020  requency band.  
-00017e70: 2020 6966 2028 666d 6178 203e 206e 702e    if (fmax > np.
-00017e80: 6d61 7828 6672 6571 2929 207c 2028 666d  max(freq)) | (fm
-00017e90: 6178 203c 3d20 666d 696e 293a 0a20 2020  ax <= fmin):.   
-00017ea0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00017eb0: 4572 726f 7228 2241 626f 7274 3a20 696e  Error("Abort: in
-00017ec0: 7075 7420 6672 6571 7565 6e63 7920 6f75  put frequency ou
-00017ed0: 7420 6f66 206c 696d 6974 7321 2229 0a20  t of limits!"). 
-00017ee0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00017ef0: 2066 7265 715f 696e 6469 6e20 3d20 6e70   freq_indin = np
-00017f00: 2e77 6865 7265 2828 6672 6571 203e 3d20  .where((freq >= 
-00017f10: 666d 696e 2920 2620 2866 7265 7120 3c3d  fmin) & (freq <=
-00017f20: 2066 6d61 7829 295b 305d 0a0a 2020 2020   fmax))[0]..    
-00017f30: 2020 2020 2320 5573 6520 4454 5720 6d65      # Use DTW me
-00017f40: 7468 6f64 2074 6f20 6578 7472 6163 7420  thod to extract 
-00017f50: 6476 760a 2020 2020 2020 2020 6e66 7265  dvv.        nfre
-00017f60: 7120 3d20 6c65 6e28 6672 6571 5f69 6e64  q = len(freq_ind
-00017f70: 696e 290a 2020 2020 2020 2020 6476 762c  in).        dvv,
-00017f80: 2065 7272 203d 206e 702e 7a65 726f 7328   err = np.zeros(
-00017f90: 6e66 7265 712c 2064 7479 7065 3d6e 702e  nfreq, dtype=np.
-00017fa0: 666c 6f61 7433 3229 2c20 6e70 2e7a 6572  float32), np.zer
-00017fb0: 6f73 286e 6672 6571 2c20 6474 7970 653d  os(nfreq, dtype=
-00017fc0: 6e70 2e66 6c6f 6174 3332 290a 0a20 2020  np.float32)..   
-00017fd0: 2020 2020 2066 6f72 2069 692c 2069 6672       for ii, ifr
-00017fe0: 6571 2069 6e20 656e 756d 6572 6174 6528  eq in enumerate(
-00017ff0: 6672 6571 5f69 6e64 696e 293a 0a20 2020  freq_indin):.   
-00018000: 2020 2020 2020 2020 2023 2070 7265 7061           # prepa
-00018010: 7265 2077 696e 646f 7765 6420 6461 7461  re windowed data
-00018020: 0a20 2020 2020 2020 2020 2020 2077 6377  .            wcw
-00018030: 7431 2c20 7763 7774 3220 3d20 7263 7774  t1, wcwt2 = rcwt
-00018040: 315b 6966 7265 715d 2c20 7263 7774 325b  1[ifreq], rcwt2[
-00018050: 6966 7265 715d 0a20 2020 2020 2020 2020  ifreq].         
-00018060: 2020 2023 204e 6f72 6d61 6c69 7a65 7320     # Normalizes 
-00018070: 626f 7468 2073 6967 6e61 6c73 2c20 6966  both signals, if
-00018080: 2061 7070 726f 7072 6961 7465 2e0a 2020   appropriate..  
-00018090: 2020 2020 2020 2020 2020 6966 206e 6f72            if nor
-000180a0: 6d61 6c69 7a65 3a0a 2020 2020 2020 2020  malize:.        
-000180b0: 2020 2020 2020 2020 6e63 7774 3120 3d20          ncwt1 = 
-000180c0: 2877 6377 7431 202d 2077 6377 7431 2e6d  (wcwt1 - wcwt1.m
-000180d0: 6561 6e28 2929 202f 2077 6377 7431 2e73  ean()) / wcwt1.s
-000180e0: 7464 2829 0a20 2020 2020 2020 2020 2020  td().           
-000180f0: 2020 2020 206e 6377 7432 203d 2028 7763       ncwt2 = (wc
-00018100: 7774 3220 2d20 7763 7774 322e 6d65 616e  wt2 - wcwt2.mean
-00018110: 2829 2920 2f20 7763 7774 322e 7374 6428  ()) / wcwt2.std(
-00018120: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00018130: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00018140: 2020 2020 6e63 7774 3120 3d20 7763 7774      ncwt1 = wcwt
-00018150: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-00018160: 2020 6e63 7774 3220 3d20 7763 7774 320a    ncwt2 = wcwt2.
-00018170: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-00018180: 756e 2064 7477 0a20 2020 2020 2020 2020  un dtw.         
-00018190: 2020 2064 762c 2065 7272 6f72 2c20 6469     dv, error, di
-000181a0: 7374 203d 2064 7477 5f64 7676 286e 6377  st = dtw_dvv(ncw
-000181b0: 7432 2c20 6e63 7774 312c 2070 6172 612c  t2, ncwt1, para,
-000181c0: 206d 6178 4c61 672c 2062 2c20 6469 7265   maxLag, b, dire
-000181d0: 6374 696f 6e29 0a20 2020 2020 2020 2020  ction).         
-000181e0: 2020 2064 7676 5b69 695d 2c20 6572 725b     dvv[ii], err[
-000181f0: 6969 5d20 3d20 6476 2c20 6572 726f 720a  ii] = dv, error.
-00018200: 0a20 2020 2064 656c 2063 7774 312c 2063  .    del cwt1, c
-00018210: 7774 322c 2072 6377 7431 2c20 7263 7774  wt2, rcwt1, rcwt
-00018220: 322c 206e 6377 7431 2c20 6e63 7774 322c  2, ncwt1, ncwt2,
-00018230: 2077 6377 7431 2c20 7763 7774 322c 2063   wcwt1, wcwt2, c
-00018240: 6f69 2c20 736a 2c20 6469 7374 0a0a 2020  oi, sj, dist..  
-00018250: 2020 6966 206e 6f74 2061 6c6c 6672 6571    if not allfreq
-00018260: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00018270: 206e 702e 6d65 616e 2864 7676 292c 206e   np.mean(dvv), n
-00018280: 702e 6d65 616e 2865 7272 290a 2020 2020  p.mean(err).    
-00018290: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
-000182a0: 7475 726e 2066 7265 715b 6672 6571 5f69  turn freq[freq_i
-000182b0: 6e64 696e 5d2c 2064 7676 2c20 6572 720a  ndin], dvv, err.
-000182c0: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00011090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000110a0: 0a0a 2222 220a 6120 636f 6d70 696c 6174  ..""".a compilat
+000110b0: 696f 6e20 6f66 2061 6c6c 2061 7661 696c  ion of all avail
+000110c0: 6162 6c65 2063 6f72 6520 6675 6e63 7469  able core functi
+000110d0: 6f6e 7320 666f 7220 636f 6d70 7574 696e  ons for computin
+000110e0: 6720 7068 6173 6520 6465 6c61 7973 2062  g phase delays b
+000110f0: 6173 6564 206f 6e20 616d 6269 656e 7420  ased on ambient 
+00011100: 6e6f 6973 6520 696e 7465 7266 6572 6f6d  noise interferom
+00011110: 6574 7279 0a0a 7175 6963 6b20 696e 6465  etry..quick inde
+00011120: 7820 6f66 2064 762f 7620 6d65 7468 6f64  x of dv/v method
+00011130: 733a 0a31 2920 7374 7265 7463 6869 6e67  s:.1) stretching
+00011140: 2028 7469 6d65 2073 7472 6574 6368 696e   (time stretchin
+00011150: 673b 2057 6561 7665 7220 6574 2061 6c20  g; Weaver et al 
+00011160: 2832 3031 3129 290a 3229 2064 7477 5f64  (2011)).2) dtw_d
+00011170: 7676 2028 4479 6e61 6d69 6320 5469 6d65  vv (Dynamic Time
+00011180: 2057 6172 7069 6e67 3b20 4d69 6b65 7365   Warping; Mikese
+00011190: 6c6c 2065 7420 616c 2e20 3230 3135 290a  ll et al. 2015).
+000111a0: 3329 206d 7763 735f 6476 7620 284d 6f76  3) mwcs_dvv (Mov
+000111b0: 696e 6720 5769 6e64 6f77 2043 726f 7373  ing Window Cross
+000111c0: 2053 7065 6374 7275 6d3b 2043 6c61 726b   Spectrum; Clark
+000111d0: 2065 7420 616c 2e2c 2032 3031 3129 0a34   et al., 2011).4
+000111e0: 2920 6d77 6363 5f64 7676 2028 4d6f 7669  ) mwcc_dvv (Movi
+000111f0: 6e67 2057 696e 646f 7720 4372 6f73 7320  ng Window Cross 
+00011200: 436f 7272 656c 6174 696f 6e3b 2053 6e69  Correlation; Sni
+00011210: 6564 6572 2065 7420 616c 2e2c 2032 3031  eder et al., 201
+00011220: 3229 0a35 2920 7774 735f 6476 7620 2857  2).5) wts_dvv (W
+00011230: 6176 656c 6574 2053 7472 6563 6869 6e67  avelet Streching
+00011240: 3b20 5975 616e 2065 7420 616c 2e2c 2069  ; Yuan et al., i
+00011250: 6e20 7072 6570 290a 3629 2077 7873 5f64  n prep).6) wxs_d
+00011260: 7676 2028 5761 7665 6c65 7420 5872 6f73  vv (Wavelet Xros
+00011270: 7320 5370 6563 7472 756d 3b20 4d61 6f20  s Spectrum; Mao 
+00011280: 6574 2061 6c2e 2c20 3230 3139 290a 3729  et al., 2019).7)
+00011290: 2077 6477 5f64 7676 2028 5761 7665 6c65   wdw_dvv (Wavele
+000112a0: 7420 4479 6e61 6d69 6320 5761 7270 696e  t Dynamic Warpin
+000112b0: 673b 2059 7561 6e20 6574 2061 6c2e 2c20  g; Yuan et al., 
+000112c0: 696e 2070 7265 7029 0a22 2222 0a0a 0a64  in prep)."""...d
+000112d0: 6566 2073 7472 6574 6368 696e 6728 7265  ef stretching(re
+000112e0: 662c 2063 7572 2c20 6476 5f72 616e 6765  f, cur, dv_range
+000112f0: 2c20 6e62 7472 6961 6c2c 2070 6172 6129  , nbtrial, para)
+00011300: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+00011310: 6973 2066 756e 6374 696f 6e20 636f 6d70  is function comp
+00011320: 6172 6573 2074 6865 2052 6566 6572 656e  ares the Referen
+00011330: 6365 2077 6176 6566 6f72 6d20 746f 2073  ce waveform to s
+00011340: 7472 6574 6368 6564 2f63 6f6d 7072 6573  tretched/compres
+00011350: 7365 6420 6375 7272 656e 7420 7761 7665  sed current wave
+00011360: 666f 726d 7320 746f 2067 6574 2074 6865  forms to get the
+00011370: 0a20 2020 2072 656c 6174 6976 6520 7365  .    relative se
+00011380: 6973 6d69 6320 7665 6c6f 6369 7479 2076  ismic velocity v
+00011390: 6172 6961 7469 6f6e 2028 616e 6420 6173  ariation (and as
+000113a0: 736f 6369 6174 6564 2065 7272 6f72 292e  sociated error).
+000113b0: 0a20 2020 2049 7420 616c 736f 2063 6f6d  .    It also com
+000113c0: 7075 7465 7320 7468 6520 636f 7272 656c  putes the correl
+000113d0: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
+000113e0: 7420 6265 7477 6565 6e20 7468 6520 5265  t between the Re
+000113f0: 6665 7265 6e63 6520 7761 7665 666f 726d  ference waveform
+00011400: 2061 6e64 2074 6865 2063 7572 7265 6e74   and the current
+00011410: 2077 6176 6566 6f72 6d2e 0a0a 2020 2020   waveform...    
+00011420: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+00011430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011440: 0a20 2020 2072 6566 3a20 5265 6665 7265  .    ref: Refere
+00011450: 6e63 6520 7761 7665 666f 726d 2028 6e70  nce waveform (np
+00011460: 2e6e 6461 7272 6179 2c20 7369 7a65 204e  .ndarray, size N
+00011470: 290a 2020 2020 6375 723a 2043 7572 7265  ).    cur: Curre
+00011480: 6e74 2077 6176 6566 6f72 6d20 286e 702e  nt waveform (np.
+00011490: 6e64 6172 7261 792c 2073 697a 6520 4e29  ndarray, size N)
+000114a0: 0a20 2020 2064 765f 7261 6e67 653a 2061  .    dv_range: a
+000114b0: 6273 6f6c 7574 6520 626f 756e 6420 666f  bsolute bound fo
+000114c0: 7220 7468 6520 7665 6c6f 6369 7479 2076  r the velocity v
+000114d0: 6172 6961 7469 6f6e 3b20 6578 616d 706c  ariation; exampl
+000114e0: 653a 2064 763d 302e 3033 2066 6f72 205b  e: dv=0.03 for [
+000114f0: 2d33 2c33 5d25 0a20 2020 206f 6620 7265  -3,3]%.    of re
+00011500: 6c61 7469 7665 2076 656c 6f63 6974 7920  lative velocity 
+00011510: 6368 616e 6765 2028 2766 6c6f 6174 2729  change ('float')
+00011520: 0a20 2020 206e 6274 7269 616c 3a20 6e75  .    nbtrial: nu
+00011530: 6d62 6572 206f 6620 7374 7265 7463 6869  mber of stretchi
+00011540: 6e67 2063 6f65 6666 6963 6965 6e74 2062  ng coefficient b
+00011550: 6574 7765 656e 2064 766d 696e 2061 6e64  etween dvmin and
+00011560: 2064 766d 6178 2c20 6e6f 206e 6565 6420   dvmax, no need 
+00011570: 746f 2062 6520 6869 6768 6572 2074 6861  to be higher tha
+00011580: 6e20 3130 3020 2028 2766 6c6f 6174 2729  n 100  ('float')
+00011590: 0a20 2020 2070 6172 613a 2076 6563 746f  .    para: vecto
+000115a0: 7220 6f66 2074 6865 2069 6e64 6963 6573  r of the indices
+000115b0: 206f 6620 7468 6520 6375 7220 616e 6420   of the cur and 
+000115c0: 7265 6620 7769 6e64 6f77 7320 6f6e 2077  ref windows on w
+000115d0: 6963 6820 796f 7520 7761 6e74 2074 6f20  ich you want to 
+000115e0: 646f 2074 6865 206d 6561 7375 7265 6d65  do the measureme
+000115f0: 6e74 730a 2020 2020 286e 702e 6e64 6172  nts.    (np.ndar
+00011600: 7261 792c 2073 697a 6520 746d 696e 2a64  ray, size tmin*d
+00011610: 656c 7461 3a74 6d61 782a 6465 6c74 6129  elta:tmax*delta)
+00011620: 0a20 2020 2046 6f72 2065 7272 6f72 2063  .    For error c
+00011630: 6f6d 7075 7461 7469 6f6e 2c20 7765 206e  omputation, we n
+00011640: 6565 6420 7061 7261 6d65 7465 7273 3a0a  eed parameters:.
+00011650: 2020 2020 2020 2020 666d 696e 3a20 6d69          fmin: mi
+00011660: 6e69 6d75 6d20 6672 6571 7565 6e63 7920  nimum frequency 
+00011670: 6f66 2074 6865 2064 6174 610a 2020 2020  of the data.    
+00011680: 2020 2020 666d 6178 3a20 6d61 7869 6d75      fmax: maximu
+00011690: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
+000116a0: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
+000116b0: 746d 696e 3a20 6d69 6e69 6d75 6d20 7469  tmin: minimum ti
+000116c0: 6d65 2077 696e 646f 7720 7768 6572 6520  me window where 
+000116d0: 7468 6520 6476 2f76 2069 7320 636f 6d70  the dv/v is comp
+000116e0: 7574 6564 0a20 2020 2020 2020 2074 6d61  uted.        tma
+000116f0: 783a 206d 6178 696d 756d 2074 696d 6520  x: maximum time 
+00011700: 7769 6e64 6f77 2077 6865 7265 2074 6865  window where the
+00011710: 2064 762f 7620 6973 2063 6f6d 7075 7465   dv/v is compute
+00011720: 640a 2020 2020 5245 5455 524e 533a 0a20  d.    RETURNS:. 
+00011730: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00011740: 2d2d 2d0a 2020 2020 6476 3a20 5265 6c61  ---.    dv: Rela
+00011750: 7469 7665 2076 656c 6f63 6974 7920 6368  tive velocity ch
+00011760: 616e 6765 2064 762f 7620 2869 6e20 2529  ange dv/v (in %)
+00011770: 0a20 2020 2063 633a 2063 6f72 7265 6c61  .    cc: correla
+00011780: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
+00011790: 2062 6574 7765 656e 2074 6865 2072 6566   between the ref
+000117a0: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
+000117b0: 616e 6420 7468 6520 6265 7374 2073 7472  and the best str
+000117c0: 6574 6368 6564 2f63 6f6d 7072 6573 7365  etched/compresse
+000117d0: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
+000117e0: 726d 0a20 2020 2063 6470 3a20 636f 7272  rm.    cdp: corr
+000117f0: 656c 6174 696f 6e20 636f 6566 6669 6369  elation coeffici
+00011800: 656e 7420 6265 7477 6565 6e20 7468 6520  ent between the 
+00011810: 7265 6665 7265 6e63 6520 7761 7665 666f  reference wavefo
+00011820: 726d 2061 6e64 2074 6865 2069 6e69 7469  rm and the initi
+00011830: 616c 2063 7572 7265 6e74 2077 6176 6566  al current wavef
+00011840: 6f72 6d0a 2020 2020 6572 726f 723a 2045  orm.    error: E
+00011850: 7272 6f72 7320 696e 2074 6865 2064 762f  rrors in the dv/
+00011860: 7620 6d65 6173 7572 656d 656e 7473 2062  v measurements b
+00011870: 6173 6564 206f 6e20 5765 6176 6572 2065  ased on Weaver e
+00011880: 7420 616c 2028 3230 3131 292c 0a20 2020  t al (2011),.   
+00011890: 204f 6e20 7468 6520 7072 6563 6973 696f   On the precisio
+000118a0: 6e20 6f66 206e 6f69 7365 2d63 6f72 7265  n of noise-corre
+000118b0: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
+000118c0: 6d65 7472 792c 2047 656f 7068 7973 2e20  metry, Geophys. 
+000118d0: 4a2e 2049 6e74 2e2c 2031 3835 2833 290a  J. Int., 185(3).
+000118e0: 0a20 2020 204e 6f74 653a 2054 6865 2063  .    Note: The c
+000118f0: 6f64 6520 6669 7273 7420 6669 6e64 7320  ode first finds 
+00011900: 7468 6520 6265 7374 2063 6f72 7265 6c61  the best correla
+00011910: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
+00011920: 2062 6574 7765 656e 2074 6865 2052 6566   between the Ref
+00011930: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
+00011940: 616e 640a 2020 2020 7468 6520 7374 7265  and.    the stre
+00011950: 7463 6865 642f 636f 6d70 7265 7373 6564  tched/compressed
+00011960: 2063 7572 7265 6e74 2077 6176 6566 6f72   current wavefor
+00011970: 6d20 616d 6f6e 6720 7468 6520 226e 6274  m among the "nbt
+00011980: 7269 616c 2220 7661 6c75 6573 2e0a 2020  rial" values..  
+00011990: 2020 4120 7265 6669 6e65 6420 616e 616c    A refined anal
+000119a0: 7973 6973 2069 7320 7468 656e 2070 6572  ysis is then per
+000119b0: 666f 726d 6564 2061 726f 756e 6420 7468  formed around th
+000119c0: 6973 2076 616c 7565 2074 6f20 6f62 7461  is value to obta
+000119d0: 696e 2061 206d 6f72 6520 7072 6563 6973  in a more precis
+000119e0: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
+000119f0: 6e74 202e 0a0a 2020 2020 4f72 6967 696e  nt ...    Origin
+00011a00: 616c 6c79 2062 7920 4c2e 2056 6965 6e73  ally by L. Viens
+00011a10: 2030 342f 3236 2f32 3031 3820 2856 6965   04/26/2018 (Vie
+00011a20: 6e73 2065 7420 616c 2e2c 2032 3031 3820  ns et al., 2018 
+00011a30: 4a47 5229 0a20 2020 206d 6f64 6966 6965  JGR).    modifie
+00011a40: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
+00011a50: 616e 670a 2020 2020 2222 220a 2020 2020  ang.    """.    
+00011a60: 2320 6c6f 6164 2063 6f6d 6d6f 6e20 7661  # load common va
+00011a70: 7269 6162 6c65 7320 6672 6f6d 2064 6963  riables from dic
+00011a80: 7469 6f6e 6172 790a 2020 2020 7477 696e  tionary.    twin
+00011a90: 203d 2070 6172 615b 2274 7769 6e22 5d0a   = para["twin"].
+00011aa0: 2020 2020 6672 6571 203d 2070 6172 615b      freq = para[
+00011ab0: 2266 7265 7122 5d0a 2020 2020 6474 203d  "freq"].    dt =
+00011ac0: 2070 6172 615b 2264 7422 5d0a 2020 2020   para["dt"].    
+00011ad0: 746d 696e 203d 206e 702e 6d69 6e28 7477  tmin = np.min(tw
+00011ae0: 696e 290a 2020 2020 746d 6178 203d 206e  in).    tmax = n
+00011af0: 702e 6d61 7828 7477 696e 290a 2020 2020  p.max(twin).    
+00011b00: 666d 696e 203d 206e 702e 6d69 6e28 6672  fmin = np.min(fr
+00011b10: 6571 290a 2020 2020 666d 6178 203d 206e  eq).    fmax = n
+00011b20: 702e 6d61 7828 6672 6571 290a 2020 2020  p.max(freq).    
+00011b30: 7476 6563 203d 206e 702e 6172 616e 6765  tvec = np.arange
+00011b40: 2874 6d69 6e2c 2074 6d61 782c 2064 7429  (tmin, tmax, dt)
+00011b50: 0a0a 2020 2020 2320 6d61 6b65 2075 7365  ..    # make use
+00011b60: 6675 6c20 6f6e 6520 666f 7220 6d65 6173  ful one for meas
+00011b70: 7572 656d 656e 7473 0a20 2020 2064 766d  urements.    dvm
+00011b80: 696e 203d 202d 6e70 2e61 6273 2864 765f  in = -np.abs(dv_
+00011b90: 7261 6e67 6529 0a20 2020 2064 766d 6178  range).    dvmax
+00011ba0: 203d 206e 702e 6162 7328 6476 5f72 616e   = np.abs(dv_ran
+00011bb0: 6765 290a 2020 2020 4570 7320 3d20 3120  ge).    Eps = 1 
+00011bc0: 2b20 286e 702e 6c69 6e73 7061 6365 2864  + (np.linspace(d
+00011bd0: 766d 696e 2c20 6476 6d61 782c 206e 6274  vmin, dvmax, nbt
+00011be0: 7269 616c 2929 0a20 2020 2063 6f66 203d  rial)).    cof =
+00011bf0: 206e 702e 7a65 726f 7328 4570 732e 7368   np.zeros(Eps.sh
+00011c00: 6170 652c 2064 7479 7065 3d6e 702e 666c  ape, dtype=np.fl
+00011c10: 6f61 7433 3229 0a0a 2020 2020 2320 5365  oat32)..    # Se
+00011c20: 7420 6f66 2073 7472 6574 6368 6564 2f63  t of stretched/c
+00011c30: 6f6d 7072 6573 7365 6420 6375 7272 656e  ompressed curren
+00011c40: 7420 7761 7665 666f 726d 730a 2020 2020  t waveforms.    
+00011c50: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
+00011c60: 6c65 6e28 4570 7329 293a 0a20 2020 2020  len(Eps)):.     
+00011c70: 2020 206e 7420 3d20 7476 6563 202a 2045     nt = tvec * E
+00011c80: 7073 5b69 695d 0a20 2020 2020 2020 2073  ps[ii].        s
+00011c90: 203d 206e 702e 696e 7465 7270 2878 3d74   = np.interp(x=t
+00011ca0: 7665 632c 2078 703d 6e74 2c20 6670 3d63  vec, xp=nt, fp=c
+00011cb0: 7572 290a 2020 2020 2020 2020 7761 7665  ur).        wave
+00011cc0: 666f 726d 5f72 6566 203d 2072 6566 0a20  form_ref = ref. 
+00011cd0: 2020 2020 2020 2077 6176 6566 6f72 6d5f         waveform_
+00011ce0: 6375 7220 3d20 730a 2020 2020 2020 2020  cur = s.        
+00011cf0: 636f 665b 6969 5d20 3d20 6e70 2e63 6f72  cof[ii] = np.cor
+00011d00: 7263 6f65 6628 7761 7665 666f 726d 5f72  rcoef(waveform_r
+00011d10: 6566 2c20 7761 7665 666f 726d 5f63 7572  ef, waveform_cur
+00011d20: 295b 302c 2031 5d0a 0a20 2020 2063 6470  )[0, 1]..    cdp
+00011d30: 203d 206e 702e 636f 7272 636f 6566 2863   = np.corrcoef(c
+00011d40: 7572 2c20 7265 6629 5b30 2c20 315d 2020  ur, ref)[0, 1]  
+00011d50: 2320 636f 7272 656c 6174 696f 6e20 636f  # correlation co
+00011d60: 6566 6669 6369 656e 7420 6265 7477 6565  efficient betwee
+00011d70: 6e20 7468 6520 7265 6665 7265 6e63 6520  n the reference 
+00011d80: 616e 6420 696e 6974 6961 6c20 6375 7272  and initial curr
+00011d90: 656e 7420 7761 7665 666f 726d 730a 0a20  ent waveforms.. 
+00011da0: 2020 2023 2066 696e 6420 7468 6520 6d61     # find the ma
+00011db0: 7869 6d75 6d20 636f 7272 656c 6174 696f  ximum correlatio
+00011dc0: 6e20 636f 6566 6669 6369 656e 740a 2020  n coefficient.  
+00011dd0: 2020 696d 6178 203d 206e 702e 6e61 6e61    imax = np.nana
+00011de0: 7267 6d61 7828 636f 6629 0a20 2020 2069  rgmax(cof).    i
+00011df0: 6620 696d 6178 203e 3d20 6c65 6e28 4570  f imax >= len(Ep
+00011e00: 7329 202d 2032 3a0a 2020 2020 2020 2020  s) - 2:.        
+00011e10: 696d 6178 203d 2069 6d61 7820 2d20 320a  imax = imax - 2.
+00011e20: 2020 2020 6966 2069 6d61 7820 3c3d 2032      if imax <= 2
+00011e30: 3a0a 2020 2020 2020 2020 696d 6178 203d  :.        imax =
+00011e40: 2069 6d61 7820 2b20 320a 0a20 2020 2023   imax + 2..    #
+00011e50: 2050 726f 6365 6564 2074 6f20 7468 6520   Proceed to the 
+00011e60: 7365 636f 6e64 2073 7465 7020 746f 2067  second step to g
+00011e70: 6574 2061 206d 6f72 6520 7072 6563 6973  et a more precis
+00011e80: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
+00011e90: 6e74 0a20 2020 2064 7466 696e 6572 203d  nt.    dtfiner =
+00011ea0: 206e 702e 6c69 6e73 7061 6365 2845 7073   np.linspace(Eps
+00011eb0: 5b69 6d61 7820 2d20 325d 2c20 4570 735b  [imax - 2], Eps[
+00011ec0: 696d 6178 202b 2032 5d2c 2031 3030 290a  imax + 2], 100).
+00011ed0: 2020 2020 6e63 6f66 203d 206e 702e 7a65      ncof = np.ze
+00011ee0: 726f 7328 6474 6669 6e65 722e 7368 6170  ros(dtfiner.shap
+00011ef0: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+00011f00: 7433 3229 0a20 2020 2066 6f72 2069 6920  t32).    for ii 
+00011f10: 696e 2072 616e 6765 286c 656e 2864 7466  in range(len(dtf
+00011f20: 696e 6572 2929 3a0a 2020 2020 2020 2020  iner)):.        
+00011f30: 6e74 203d 2074 7665 6320 2a20 6474 6669  nt = tvec * dtfi
+00011f40: 6e65 725b 6969 5d0a 2020 2020 2020 2020  ner[ii].        
+00011f50: 7320 3d20 6e70 2e69 6e74 6572 7028 783d  s = np.interp(x=
+00011f60: 7476 6563 2c20 7870 3d6e 742c 2066 703d  tvec, xp=nt, fp=
+00011f70: 6375 7229 0a20 2020 2020 2020 2077 6176  cur).        wav
+00011f80: 6566 6f72 6d5f 7265 6620 3d20 7265 660a  eform_ref = ref.
+00011f90: 2020 2020 2020 2020 7761 7665 666f 726d          waveform
+00011fa0: 5f63 7572 203d 2073 0a20 2020 2020 2020  _cur = s.       
+00011fb0: 206e 636f 665b 6969 5d20 3d20 6e70 2e63   ncof[ii] = np.c
+00011fc0: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
+00011fd0: 5f72 6566 2c20 7761 7665 666f 726d 5f63  _ref, waveform_c
+00011fe0: 7572 295b 302c 2031 5d0a 0a20 2020 2063  ur)[0, 1]..    c
+00011ff0: 6320 3d20 6e70 2e6d 6178 286e 636f 6629  c = np.max(ncof)
+00012000: 2020 2320 4669 6e64 206d 6178 696d 756d    # Find maximum
+00012010: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
+00012020: 6666 6963 6965 6e74 206f 6620 7468 6520  fficient of the 
+00012030: 7265 6669 6e65 6420 2061 6e61 6c79 7369  refined  analysi
+00012040: 730a 2020 2020 6476 203d 2031 3030 2e30  s.    dv = 100.0
+00012050: 202a 2064 7466 696e 6572 5b6e 702e 6172   * dtfiner[np.ar
+00012060: 676d 6178 286e 636f 6629 5d20 2d20 3130  gmax(ncof)] - 10
+00012070: 3020 2023 204d 756c 7469 706c 7920 6279  0  # Multiply by
+00012080: 2031 3030 2074 6f20 636f 6e76 6572 7420   100 to convert 
+00012090: 746f 2070 6572 6365 6e74 6167 6520 2845  to percentage (E
+000120a0: 7073 696c 6f6e 203d 202d 6474 2f74 203d  psilon = -dt/t =
+000120b0: 2064 762f 7629 0a0a 2020 2020 2320 4572   dv/v)..    # Er
+000120c0: 726f 7220 636f 6d70 7574 6174 696f 6e20  ror computation 
+000120d0: 6261 7365 6420 6f6e 2057 6561 7665 7220  based on Weaver 
+000120e0: 6574 2061 6c20 2832 3031 3129 2c20 4f6e  et al (2011), On
+000120f0: 2074 6865 2070 7265 6369 7369 6f6e 206f   the precision o
+00012100: 6620 6e6f 6973 652d 636f 7272 656c 6174  f noise-correlat
+00012110: 696f 6e0a 2020 2020 2320 696e 7465 7266  ion.    # interf
+00012120: 6572 6f6d 6574 7279 2c20 4765 6f70 6879  erometry, Geophy
+00012130: 732e 204a 2e20 496e 742e 2c20 3138 3528  s. J. Int., 185(
+00012140: 3329 0a20 2020 2054 203d 2031 202f 2028  3).    T = 1 / (
+00012150: 666d 6178 202d 2066 6d69 6e29 0a20 2020  fmax - fmin).   
+00012160: 2058 203d 2063 630a 2020 2020 7763 203d   X = cc.    wc =
+00012170: 206e 702e 7069 202a 2028 666d 696e 202b   np.pi * (fmin +
+00012180: 2066 6d61 7829 0a20 2020 2074 3120 3d20   fmax).    t1 = 
+00012190: 6e70 2e6d 696e 285b 746d 696e 2c20 746d  np.min([tmin, tm
+000121a0: 6178 5d29 0a20 2020 2074 3220 3d20 6e70  ax]).    t2 = np
+000121b0: 2e6d 6178 285b 746d 696e 2c20 746d 6178  .max([tmin, tmax
+000121c0: 5d29 0a20 2020 2065 7272 6f72 203d 2031  ]).    error = 1
+000121d0: 3030 202a 2028 0a20 2020 2020 2020 206e  00 * (.        n
+000121e0: 702e 7371 7274 2831 202d 2058 2a2a 3229  p.sqrt(1 - X**2)
+000121f0: 202f 2028 3220 2a20 5829 202a 206e 702e   / (2 * X) * np.
+00012200: 7371 7274 2828 3620 2a20 6e70 2e73 7172  sqrt((6 * np.sqr
+00012210: 7428 6e70 2e70 6920 2f20 3229 202a 2054  t(np.pi / 2) * T
+00012220: 2920 2f20 2877 632a 2a32 202a 2028 7432  ) / (wc**2 * (t2
+00012230: 2a2a 3320 2d20 7431 2a2a 3329 2929 0a20  **3 - t1**3))). 
+00012240: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
+00012250: 2064 762c 2065 7272 6f72 2c20 6363 2c20   dv, error, cc, 
+00012260: 6364 700a 0a0a 6465 6620 7374 7265 7463  cdp...def stretc
+00012270: 6869 6e67 5f76 6563 7428 7265 662c 2063  hing_vect(ref, c
+00012280: 7572 2c20 6476 5f72 616e 6765 2c20 6e62  ur, dv_range, nb
+00012290: 7472 6961 6c2c 2070 6172 6129 3a0a 2020  trial, para):.  
+000122a0: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
+000122b0: 756e 6374 696f 6e20 636f 6d70 6172 6573  unction compares
+000122c0: 2074 6865 2052 6566 6572 656e 6365 2077   the Reference w
+000122d0: 6176 6566 6f72 6d20 746f 2073 7472 6574  aveform to stret
+000122e0: 6368 6564 2f63 6f6d 7072 6573 7365 6420  ched/compressed 
+000122f0: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
+00012300: 730a 2020 2020 746f 2067 6574 2074 6865  s.    to get the
+00012310: 2072 656c 6174 6976 6520 7365 6973 6d69   relative seismi
+00012320: 6320 7665 6c6f 6369 7479 2076 6172 6961  c velocity varia
+00012330: 7469 6f6e 2028 616e 6420 6173 736f 6369  tion (and associ
+00012340: 6174 6564 2065 7272 6f72 292e 0a20 2020  ated error)..   
+00012350: 2049 7420 616c 736f 2063 6f6d 7075 7465   It also compute
+00012360: 7320 7468 6520 636f 7272 656c 6174 696f  s the correlatio
+00012370: 6e20 636f 6566 6669 6369 656e 7420 6265  n coefficient be
+00012380: 7477 6565 6e20 7468 6520 5265 6665 7265  tween the Refere
+00012390: 6e63 6520 7761 7665 666f 726d 2061 6e64  nce waveform and
+000123a0: 2074 6865 2063 7572 7265 6e74 2077 6176   the current wav
+000123b0: 6566 6f72 6d2e 0a0a 2020 2020 5041 5241  eform...    PARA
+000123c0: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+000123d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000123e0: 2072 6566 3a20 5265 6665 7265 6e63 6520   ref: Reference 
+000123f0: 7761 7665 666f 726d 2028 6e70 2e6e 6461  waveform (np.nda
+00012400: 7272 6179 2c20 7369 7a65 204e 290a 2020  rray, size N).  
+00012410: 2020 6375 723a 2043 7572 7265 6e74 2077    cur: Current w
+00012420: 6176 6566 6f72 6d20 286e 702e 6e64 6172  aveform (np.ndar
+00012430: 7261 792c 2073 697a 6520 4e29 0a20 2020  ray, size N).   
+00012440: 2064 765f 7261 6e67 653a 2061 6273 6f6c   dv_range: absol
+00012450: 7574 6520 626f 756e 6420 666f 7220 7468  ute bound for th
+00012460: 6520 7665 6c6f 6369 7479 2076 6172 6961  e velocity varia
+00012470: 7469 6f6e 3b20 6578 616d 706c 653a 2064  tion; example: d
+00012480: 763d 302e 3033 2066 6f72 205b 2d33 2c33  v=0.03 for [-3,3
+00012490: 5d25 0a20 2020 206f 6620 7265 6c61 7469  ]%.    of relati
+000124a0: 7665 2076 656c 6f63 6974 7920 6368 616e  ve velocity chan
+000124b0: 6765 2028 2766 6c6f 6174 2729 0a20 2020  ge ('float').   
+000124c0: 206e 6274 7269 616c 3a20 6e75 6d62 6572   nbtrial: number
+000124d0: 206f 6620 7374 7265 7463 6869 6e67 2063   of stretching c
+000124e0: 6f65 6666 6963 6965 6e74 2062 6574 7765  oefficient betwe
+000124f0: 656e 2064 766d 696e 2061 6e64 2064 766d  en dvmin and dvm
+00012500: 6178 2c20 6e6f 206e 6565 6420 746f 2062  ax, no need to b
+00012510: 6520 6869 6768 6572 2074 6861 6e20 3130  e higher than 10
+00012520: 3020 2028 2766 6c6f 6174 2729 0a20 2020  0  ('float').   
+00012530: 2070 6172 613a 2076 6563 746f 7220 6f66   para: vector of
+00012540: 2074 6865 2069 6e64 6963 6573 206f 6620   the indices of 
+00012550: 7468 6520 6375 7220 616e 6420 7265 6620  the cur and ref 
+00012560: 7769 6e64 6f77 7320 6f6e 2077 6963 6820  windows on wich 
+00012570: 796f 7520 7761 6e74 2074 6f20 646f 2074  you want to do t
+00012580: 6865 0a20 2020 206d 6561 7375 7265 6d65  he.    measureme
+00012590: 6e74 7320 286e 702e 6e64 6172 7261 792c  nts (np.ndarray,
+000125a0: 2073 697a 6520 746d 696e 2a64 656c 7461   size tmin*delta
+000125b0: 3a74 6d61 782a 6465 6c74 6129 0a20 2020  :tmax*delta).   
+000125c0: 2046 6f72 2065 7272 6f72 2063 6f6d 7075   For error compu
+000125d0: 7461 7469 6f6e 2c20 7765 206e 6565 6420  tation, we need 
+000125e0: 7061 7261 6d65 7465 7273 3a0a 2020 2020  parameters:.    
+000125f0: 2020 2020 666d 696e 3a20 6d69 6e69 6d75      fmin: minimu
+00012600: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
+00012610: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
+00012620: 666d 6178 3a20 6d61 7869 6d75 6d20 6672  fmax: maximum fr
+00012630: 6571 7565 6e63 7920 6f66 2074 6865 2064  equency of the d
+00012640: 6174 610a 2020 2020 2020 2020 746d 696e  ata.        tmin
+00012650: 3a20 6d69 6e69 6d75 6d20 7469 6d65 2077  : minimum time w
+00012660: 696e 646f 7720 7768 6572 6520 7468 6520  indow where the 
+00012670: 6476 2f76 2069 7320 636f 6d70 7574 6564  dv/v is computed
+00012680: 0a20 2020 2020 2020 2074 6d61 783a 206d  .        tmax: m
+00012690: 6178 696d 756d 2074 696d 6520 7769 6e64  aximum time wind
+000126a0: 6f77 2077 6865 7265 2074 6865 2064 762f  ow where the dv/
+000126b0: 7620 6973 2063 6f6d 7075 7465 640a 2020  v is computed.  
+000126c0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
+000126d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000126e0: 2020 2020 6476 3a20 5265 6c61 7469 7665      dv: Relative
+000126f0: 2076 656c 6f63 6974 7920 6368 616e 6765   velocity change
+00012700: 2064 762f 7620 2869 6e20 2529 0a20 2020   dv/v (in %).   
+00012710: 2063 633a 2063 6f72 7265 6c61 7469 6f6e   cc: correlation
+00012720: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
+00012730: 7765 656e 2074 6865 2072 6566 6572 656e  ween the referen
+00012740: 6365 2077 6176 6566 6f72 6d20 616e 6420  ce waveform and 
+00012750: 7468 6520 6265 7374 2073 7472 6574 6368  the best stretch
+00012760: 6564 2f63 6f6d 7072 6573 7365 6420 6375  ed/compressed cu
+00012770: 7272 656e 7420 7761 7665 666f 726d 0a20  rrent waveform. 
+00012780: 2020 2063 6470 3a20 636f 7272 656c 6174     cdp: correlat
+00012790: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
+000127a0: 6265 7477 6565 6e20 7468 6520 7265 6665  between the refe
+000127b0: 7265 6e63 6520 7761 7665 666f 726d 2061  rence waveform a
+000127c0: 6e64 2074 6865 2069 6e69 7469 616c 2063  nd the initial c
+000127d0: 7572 7265 6e74 2077 6176 6566 6f72 6d0a  urrent waveform.
+000127e0: 2020 2020 6572 726f 723a 2045 7272 6f72      error: Error
+000127f0: 7320 696e 2074 6865 2064 762f 7620 6d65  s in the dv/v me
+00012800: 6173 7572 656d 656e 7473 2062 6173 6564  asurements based
+00012810: 206f 6e20 5765 6176 6572 2065 7420 616c   on Weaver et al
+00012820: 2028 3230 3131 292c 204f 6e20 7468 6520   (2011), On the 
+00012830: 7072 6563 6973 696f 6e0a 2020 2020 6f66  precision.    of
+00012840: 206e 6f69 7365 2d63 6f72 7265 6c61 7469   noise-correlati
+00012850: 6f6e 2069 6e74 6572 6665 726f 6d65 7472  on interferometr
+00012860: 792c 2047 656f 7068 7973 2e20 4a2e 2049  y, Geophys. J. I
+00012870: 6e74 2e2c 2031 3835 2833 290a 0a20 2020  nt., 185(3)..   
+00012880: 204e 6f74 653a 2054 6865 2063 6f64 6520   Note: The code 
+00012890: 6669 7273 7420 6669 6e64 7320 7468 6520  first finds the 
+000128a0: 6265 7374 2063 6f72 7265 6c61 7469 6f6e  best correlation
+000128b0: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
+000128c0: 7765 656e 2074 6865 2052 6566 6572 656e  ween the Referen
+000128d0: 6365 2077 6176 6566 6f72 6d20 616e 640a  ce waveform and.
+000128e0: 2020 2020 7468 6520 7374 7265 7463 6865      the stretche
+000128f0: 642f 636f 6d70 7265 7373 6564 2063 7572  d/compressed cur
+00012900: 7265 6e74 2077 6176 6566 6f72 6d20 616d  rent waveform am
+00012910: 6f6e 6720 7468 6520 226e 6274 7269 616c  ong the "nbtrial
+00012920: 2220 7661 6c75 6573 2e0a 2020 2020 4120  " values..    A 
+00012930: 7265 6669 6e65 6420 616e 616c 7973 6973  refined analysis
+00012940: 2069 7320 7468 656e 2070 6572 666f 726d   is then perform
+00012950: 6564 2061 726f 756e 6420 7468 6973 2076  ed around this v
+00012960: 616c 7565 2074 6f20 6f62 7461 696e 2061  alue to obtain a
+00012970: 206d 6f72 6520 7072 6563 6973 6520 6476   more precise dv
+00012980: 2f76 206d 6561 7375 7265 6d65 6e74 202e  /v measurement .
+00012990: 0a0a 2020 2020 4f72 6967 696e 616c 6c79  ..    Originally
+000129a0: 2062 7920 4c2e 2056 6965 6e73 2030 342f   by L. Viens 04/
+000129b0: 3236 2f32 3031 3820 2856 6965 6e73 2065  26/2018 (Viens e
+000129c0: 7420 616c 2e2c 2032 3031 3820 4a47 5229  t al., 2018 JGR)
+000129d0: 0a20 2020 206d 6f64 6966 6965 6420 6279  .    modified by
+000129e0: 2043 6865 6e67 7869 6e20 4a69 616e 670a   Chengxin Jiang.
+000129f0: 2020 2020 6d6f 6469 6669 6564 2062 7920      modified by 
+00012a00: 4c61 7572 6120 4572 6d65 7274 3a20 7665  Laura Ermert: ve
+00012a10: 6374 6f72 697a 6564 2076 6572 7369 6f6e  ctorized version
+00012a20: 0a20 2020 2022 2222 0a20 2020 2023 206c  .    """.    # l
+00012a30: 6f61 6420 636f 6d6d 6f6e 2076 6172 6961  oad common varia
+00012a40: 626c 6573 2066 726f 6d20 6469 6374 696f  bles from dictio
+00012a50: 6e61 7279 0a20 2020 2074 7769 6e20 3d20  nary.    twin = 
+00012a60: 7061 7261 5b22 7477 696e 225d 0a20 2020  para["twin"].   
+00012a70: 2066 7265 7120 3d20 7061 7261 5b22 6672   freq = para["fr
+00012a80: 6571 225d 0a20 2020 2064 7420 3d20 7061  eq"].    dt = pa
+00012a90: 7261 5b22 6474 225d 0a20 2020 2074 6d69  ra["dt"].    tmi
+00012aa0: 6e20 3d20 6e70 2e6d 696e 2874 7769 6e29  n = np.min(twin)
+00012ab0: 0a20 2020 2074 6d61 7820 3d20 6e70 2e6d  .    tmax = np.m
+00012ac0: 6178 2874 7769 6e29 0a20 2020 2066 6d69  ax(twin).    fmi
+00012ad0: 6e20 3d20 6e70 2e6d 696e 2866 7265 7129  n = np.min(freq)
+00012ae0: 0a20 2020 2066 6d61 7820 3d20 6e70 2e6d  .    fmax = np.m
+00012af0: 6178 2866 7265 7129 0a20 2020 2074 7665  ax(freq).    tve
+00012b00: 6320 3d20 6e70 2e61 7261 6e67 6528 746d  c = np.arange(tm
+00012b10: 696e 2c20 746d 6178 2c20 6474 290a 0a20  in, tmax, dt).. 
+00012b20: 2020 2023 206d 616b 6520 7573 6566 756c     # make useful
+00012b30: 206f 6e65 2066 6f72 206d 6561 7375 7265   one for measure
+00012b40: 6d65 6e74 730a 2020 2020 6476 6d69 6e20  ments.    dvmin 
+00012b50: 3d20 2d6e 702e 6162 7328 6476 5f72 616e  = -np.abs(dv_ran
+00012b60: 6765 290a 2020 2020 6476 6d61 7820 3d20  ge).    dvmax = 
+00012b70: 6e70 2e61 6273 2864 765f 7261 6e67 6529  np.abs(dv_range)
+00012b80: 0a20 2020 2045 7073 203d 2031 202b 2028  .    Eps = 1 + (
+00012b90: 6e70 2e6c 696e 7370 6163 6528 6476 6d69  np.linspace(dvmi
+00012ba0: 6e2c 2064 766d 6178 2c20 6e62 7472 6961  n, dvmax, nbtria
+00012bb0: 6c29 290a 2020 2020 6364 7020 3d20 6e70  l)).    cdp = np
+00012bc0: 2e63 6f72 7263 6f65 6628 6375 722c 2072  .corrcoef(cur, r
+00012bd0: 6566 295b 302c 2031 5d20 2023 2063 6f72  ef)[0, 1]  # cor
+00012be0: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
+00012bf0: 6965 6e74 2062 6574 7765 656e 2074 6865  ient between the
+00012c00: 2072 6566 6572 656e 6365 2061 6e64 2069   reference and i
+00012c10: 6e69 7469 616c 2063 7572 7265 6e74 2077  nitial current w
+00012c20: 6176 6566 6f72 6d73 0a20 2020 2077 6176  aveforms.    wav
+00012c30: 6566 6f72 6d73 203d 206e 702e 7a65 726f  eforms = np.zero
+00012c40: 7328 286e 6274 7269 616c 202b 2031 2c20  s((nbtrial + 1, 
+00012c50: 6c65 6e28 7265 6629 2929 0a20 2020 2077  len(ref))).    w
+00012c60: 6176 6566 6f72 6d73 5b30 2c20 3a5d 203d  aveforms[0, :] =
+00012c70: 2072 6566 0a0a 2020 2020 2320 5365 7420   ref..    # Set 
+00012c80: 6f66 2073 7472 6574 6368 6564 2f63 6f6d  of stretched/com
+00012c90: 7072 6573 7365 6420 6375 7272 656e 7420  pressed current 
+00012ca0: 7761 7665 666f 726d 730a 2020 2020 666f  waveforms.    fo
+00012cb0: 7220 6969 2069 6e20 7261 6e67 6528 6e62  r ii in range(nb
+00012cc0: 7472 6961 6c29 3a0a 2020 2020 2020 2020  trial):.        
+00012cd0: 6e74 203d 2074 7665 6320 2a20 4570 735b  nt = tvec * Eps[
+00012ce0: 6969 5d0a 2020 2020 2020 2020 7320 3d20  ii].        s = 
+00012cf0: 6e70 2e69 6e74 6572 7028 783d 7476 6563  np.interp(x=tvec
+00012d00: 2c20 7870 3d6e 742c 2066 703d 6375 7229  , xp=nt, fp=cur)
+00012d10: 0a20 2020 2020 2020 2077 6176 6566 6f72  .        wavefor
+00012d20: 6d73 5b69 6920 2b20 312c 203a 5d20 3d20  ms[ii + 1, :] = 
+00012d30: 730a 2020 2020 636f 6620 3d20 6e70 2e63  s.    cof = np.c
+00012d40: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
+00012d50: 7329 5b30 5d5b 313a 5d0a 0a20 2020 2023  s)[0][1:]..    #
+00012d60: 2066 696e 6420 7468 6520 6d61 7869 6d75   find the maximu
+00012d70: 6d20 636f 7272 656c 6174 696f 6e20 636f  m correlation co
+00012d80: 6566 6669 6369 656e 740a 2020 2020 696d  efficient.    im
+00012d90: 6178 203d 206e 702e 6e61 6e61 7267 6d61  ax = np.nanargma
+00012da0: 7828 636f 6629 0a20 2020 2069 6620 696d  x(cof).    if im
+00012db0: 6178 203e 3d20 6c65 6e28 4570 7329 202d  ax >= len(Eps) -
+00012dc0: 2032 3a0a 2020 2020 2020 2020 696d 6178   2:.        imax
+00012dd0: 203d 2069 6d61 7820 2d20 320a 2020 2020   = imax - 2.    
+00012de0: 6966 2069 6d61 7820 3c20 323a 0a20 2020  if imax < 2:.   
+00012df0: 2020 2020 2069 6d61 7820 3d20 696d 6178       imax = imax
+00012e00: 202b 2032 0a0a 2020 2020 2320 5072 6f63   + 2..    # Proc
+00012e10: 6565 6420 746f 2074 6865 2073 6563 6f6e  eed to the secon
+00012e20: 6420 7374 6570 2074 6f20 6765 7420 6120  d step to get a 
+00012e30: 6d6f 7265 2070 7265 6369 7365 2064 762f  more precise dv/
+00012e40: 7620 6d65 6173 7572 656d 656e 740a 2020  v measurement.  
+00012e50: 2020 6474 6669 6e65 7220 3d20 6e70 2e6c    dtfiner = np.l
+00012e60: 696e 7370 6163 6528 4570 735b 696d 6178  inspace(Eps[imax
+00012e70: 202d 2032 5d2c 2045 7073 5b69 6d61 7820   - 2], Eps[imax 
+00012e80: 2b20 325d 2c20 6e62 7472 6961 6c29 0a20  + 2], nbtrial). 
+00012e90: 2020 2023 206e 636f 6620 2020 203d 206e     # ncof    = n
+00012ea0: 702e 7a65 726f 7328 6474 6669 6e65 722e  p.zeros(dtfiner.
+00012eb0: 7368 6170 652c 6474 7970 653d 6e70 2e66  shape,dtype=np.f
+00012ec0: 6c6f 6174 3332 290a 2020 2020 7761 7665  loat32).    wave
+00012ed0: 666f 726d 7320 3d20 6e70 2e7a 6572 6f73  forms = np.zeros
+00012ee0: 2828 6e62 7472 6961 6c20 2b20 312c 206c  ((nbtrial + 1, l
+00012ef0: 656e 2872 6566 2929 290a 2020 2020 7761  en(ref))).    wa
+00012f00: 7665 666f 726d 735b 302c 203a 5d20 3d20  veforms[0, :] = 
+00012f10: 7265 660a 2020 2020 666f 7220 6969 2069  ref.    for ii i
+00012f20: 6e20 7261 6e67 6528 6c65 6e28 6474 6669  n range(len(dtfi
+00012f30: 6e65 7229 293a 0a20 2020 2020 2020 206e  ner)):.        n
+00012f40: 7420 3d20 7476 6563 202a 2064 7466 696e  t = tvec * dtfin
+00012f50: 6572 5b69 695d 0a20 2020 2020 2020 2073  er[ii].        s
+00012f60: 203d 206e 702e 696e 7465 7270 2878 3d74   = np.interp(x=t
+00012f70: 7665 632c 2078 703d 6e74 2c20 6670 3d63  vec, xp=nt, fp=c
+00012f80: 7572 290a 2020 2020 2020 2020 7761 7665  ur).        wave
+00012f90: 666f 726d 735b 6969 202b 2031 2c20 3a5d  forms[ii + 1, :]
+00012fa0: 203d 2073 0a20 2020 206e 636f 6620 3d20   = s.    ncof = 
+00012fb0: 6e70 2e63 6f72 7263 6f65 6628 7761 7665  np.corrcoef(wave
+00012fc0: 666f 726d 7329 5b30 5d5b 313a 5d0a 2020  forms)[0][1:].  
+00012fd0: 2020 6363 203d 206e 702e 6d61 7828 6e63    cc = np.max(nc
+00012fe0: 6f66 2920 2023 2046 696e 6420 6d61 7869  of)  # Find maxi
+00012ff0: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
+00013000: 636f 6566 6669 6369 656e 7420 6f66 2074  coefficient of t
+00013010: 6865 2072 6566 696e 6564 2020 616e 616c  he refined  anal
+00013020: 7973 6973 0a20 2020 2064 7620 3d20 3130  ysis.    dv = 10
+00013030: 302e 3020 2a20 6474 6669 6e65 725b 6e70  0.0 * dtfiner[np
+00013040: 2e61 7267 6d61 7828 6e63 6f66 295d 202d  .argmax(ncof)] -
+00013050: 2031 3030 2020 2320 4d75 6c74 6970 6c79   100  # Multiply
+00013060: 2062 7920 3130 3020 746f 2063 6f6e 7665   by 100 to conve
+00013070: 7274 2074 6f20 7065 7263 656e 7461 6765  rt to percentage
+00013080: 2028 4570 7369 6c6f 6e20 3d20 2d64 742f   (Epsilon = -dt/
+00013090: 7420 3d20 6476 2f76 290a 0a20 2020 2023  t = dv/v)..    #
+000130a0: 2045 7272 6f72 2063 6f6d 7075 7461 7469   Error computati
+000130b0: 6f6e 2062 6173 6564 206f 6e20 5765 6176  on based on Weav
+000130c0: 6572 2065 7420 616c 2028 3230 3131 292c  er et al (2011),
+000130d0: 204f 6e20 7468 6520 7072 6563 6973 696f   On the precisio
+000130e0: 6e20 6f66 206e 6f69 7365 2d63 6f72 7265  n of noise-corre
+000130f0: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
+00013100: 6d65 7472 792c 0a20 2020 2023 2047 656f  metry,.    # Geo
+00013110: 7068 7973 2e20 4a2e 2049 6e74 2e2c 2031  phys. J. Int., 1
+00013120: 3835 2833 290a 2020 2020 5420 3d20 3120  85(3).    T = 1 
+00013130: 2f20 2866 6d61 7820 2d20 666d 696e 290a  / (fmax - fmin).
+00013140: 2020 2020 5820 3d20 6363 0a20 2020 2077      X = cc.    w
+00013150: 6320 3d20 6e70 2e70 6920 2a20 2866 6d69  c = np.pi * (fmi
+00013160: 6e20 2b20 666d 6178 290a 2020 2020 7431  n + fmax).    t1
+00013170: 203d 206e 702e 6d69 6e28 5b74 6d69 6e2c   = np.min([tmin,
+00013180: 2074 6d61 785d 290a 2020 2020 7432 203d   tmax]).    t2 =
+00013190: 206e 702e 6d61 7828 5b74 6d69 6e2c 2074   np.max([tmin, t
+000131a0: 6d61 785d 290a 2020 2020 6572 726f 7220  max]).    error 
+000131b0: 3d20 3130 3020 2a20 280a 2020 2020 2020  = 100 * (.      
+000131c0: 2020 6e70 2e73 7172 7428 3120 2d20 582a    np.sqrt(1 - X*
+000131d0: 2a32 2920 2f20 2832 202a 2058 2920 2a20  *2) / (2 * X) * 
+000131e0: 6e70 2e73 7172 7428 2836 202a 206e 702e  np.sqrt((6 * np.
+000131f0: 7371 7274 286e 702e 7069 202f 2032 2920  sqrt(np.pi / 2) 
+00013200: 2a20 5429 202f 2028 7763 2a2a 3220 2a20  * T) / (wc**2 * 
+00013210: 2874 322a 2a33 202d 2074 312a 2a33 2929  (t2**3 - t1**3))
+00013220: 290a 2020 2020 290a 0a20 2020 2072 6574  ).    )..    ret
+00013230: 7572 6e20 6476 2c20 6572 726f 722c 2063  urn dv, error, c
+00013240: 632c 2063 6470 0a0a 0a64 6566 2064 7477  c, cdp...def dtw
+00013250: 5f64 7676 2872 6566 2c20 6375 722c 2070  _dvv(ref, cur, p
+00013260: 6172 612c 206d 6178 4c61 672c 2062 2c20  ara, maxLag, b, 
+00013270: 6469 7265 6374 696f 6e29 3a0a 2020 2020  direction):.    
+00013280: 2222 220a 2020 2020 4479 6e61 6d69 6320  """.    Dynamic 
+00013290: 7469 6d65 2077 6172 7069 6e67 2066 6f72  time warping for
+000132a0: 2064 762f 7620 6573 7469 6d61 7469 6f6e   dv/v estimation
+000132b0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
+000132c0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+000132d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 6620  -------.    ref 
+000132e0: 3a20 7265 6665 7265 6e63 6520 7369 676e  : reference sign
+000132f0: 616c 2028 6e70 2e61 7272 6179 2c20 7369  al (np.array, si
+00013300: 7a65 204e 290a 2020 2020 6375 7220 3a20  ze N).    cur : 
+00013310: 6375 7272 656e 7420 7369 676e 616c 2028  current signal (
+00013320: 6e70 2e61 7272 6179 2c20 7369 7a65 204e  np.array, size N
+00013330: 290a 2020 2020 7061 7261 3a20 6469 6374  ).    para: dict
+00013340: 2063 6f6e 7461 696e 696e 6720 7573 6566   containing usef
+00013350: 756c 2070 6172 616d 6574 6572 7320 6162  ul parameters ab
+00013360: 6f75 7420 7468 6520 6461 7461 2077 696e  out the data win
+00013370: 646f 7720 616e 6420 7461 7267 6574 6564  dow and targeted
+00013380: 2066 7265 7175 656e 6379 0a20 2020 206d   frequency.    m
+00013390: 6178 4c61 6720 3a20 6d61 7820 6e75 6d62  axLag : max numb
+000133a0: 6572 206f 6620 706f 696e 7473 2074 6f20  er of points to 
+000133b0: 7365 6172 6368 2066 6f72 7761 7264 2061  search forward a
+000133c0: 6e64 2062 6163 6b77 6172 642e 0a20 2020  nd backward..   
+000133d0: 2020 2020 2020 2020 2053 7567 6765 7374           Suggest
+000133e0: 2073 6574 7469 6e67 2069 7420 6c61 7267   setting it larg
+000133f0: 6572 2069 6620 7769 6e64 6f77 2069 7320  er if window is 
+00013400: 7365 7420 6c61 7267 6572 2e0a 2020 2020  set larger..    
+00013410: 6220 3a20 622d 7661 6c75 6520 746f 206c  b : b-value to l
+00013420: 696d 6974 2073 7472 6169 6e2c 2077 6869  imit strain, whi
+00013430: 6368 2069 7320 746f 206c 696d 6974 2074  ch is to limit t
+00013440: 6865 206d 6178 696d 756d 2076 656c 6f63  he maximum veloc
+00013450: 6974 7920 7065 7274 7572 6261 7469 6f6e  ity perturbation
+00013460: 2e0a 2020 2020 2020 2020 2020 2020 5365  ..            Se
+00013470: 6520 6571 7561 7469 6f6e 2031 3120 696e  e equation 11 in
+00013480: 2028 4d69 6b65 7365 6c6c 2065 7420 616c   (Mikesell et al
+00013490: 2e20 3230 3135 290a 2020 2020 6469 7265  . 2015).    dire
+000134a0: 6374 696f 6e3a 2064 6972 6563 7469 6f6e  ction: direction
+000134b0: 2074 6f20 6163 6375 6d75 6c61 7465 2065   to accumulate e
+000134c0: 7272 6f72 7320 2831 3d66 6f72 7761 7264  rrors (1=forward
+000134d0: 2c20 2d31 3d62 6163 6b77 6172 6429 0a20  , -1=backward). 
+000134e0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+000134f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013500: 2d2d 0a20 2020 202d 6d30 203a 2065 7374  --.    -m0 : est
+00013510: 696d 6174 6564 2064 762f 760a 2020 2020  imated dv/v.    
+00013520: 656d 3020 3a20 6572 726f 7220 6f66 2064  em0 : error of d
+00013530: 762f 7620 6573 7469 6d61 7469 6f6e 0a0a  v/v estimation..
+00013540: 2020 2020 4f72 6967 696e 616c 2062 7920      Original by 
+00013550: 4469 2059 616e 670a 2020 2020 4c61 7374  Di Yang.    Last
+00013560: 206d 6f64 6966 6965 6420 6279 2044 796c   modified by Dyl
+00013570: 616e 204d 696b 6573 656c 6c20 2832 3520  an Mikesell (25 
+00013580: 4665 622e 2032 3031 3529 0a20 2020 2054  Feb. 2015).    T
+00013590: 7261 6e73 6c61 7465 6420 746f 2070 7974  ranslated to pyt
+000135a0: 686f 6e20 6279 2054 696d 2043 6c65 6d65  hon by Tim Cleme
+000135b0: 6e74 7320 2831 3720 4175 672e 2032 3031  nts (17 Aug. 201
+000135c0: 3829 0a20 2020 2022 2222 0a20 2020 2074  8).    """.    t
+000135d0: 7769 6e20 3d20 7061 7261 5b22 7477 696e  win = para["twin
+000135e0: 225d 0a20 2020 2064 7420 3d20 7061 7261  "].    dt = para
+000135f0: 5b22 6474 225d 0a20 2020 2074 6d69 6e20  ["dt"].    tmin 
+00013600: 3d20 6e70 2e6d 696e 2874 7769 6e29 0a20  = np.min(twin). 
+00013610: 2020 2074 6d61 7820 3d20 6e70 2e6d 6178     tmax = np.max
+00013620: 2874 7769 6e29 0a20 2020 2074 7665 6374  (twin).    tvect
+00013630: 203d 206e 702e 6172 616e 6765 2874 6d69   = np.arange(tmi
+00013640: 6e2c 2074 6d61 782c 2064 7429 0a0a 2020  n, tmax, dt)..  
+00013650: 2020 2320 7365 7475 7020 6f74 6865 7220    # setup other 
+00013660: 7061 7261 6d65 7465 7273 0a20 2020 206e  parameters.    n
+00013670: 7074 7320 3d20 6c65 6e28 7265 6629 2020  pts = len(ref)  
+00013680: 2320 6e75 6d62 6572 206f 6620 7469 6d65  # number of time
+00013690: 2073 616d 706c 6573 0a0a 2020 2020 2320   samples..    # 
+000136a0: 636f 6d70 7574 6520 6572 726f 7220 6675  compute error fu
+000136b0: 6e63 7469 6f6e 206f 7665 7220 6c61 6773  nction over lags
+000136c0: 2c20 7768 6963 6820 6973 2069 6e64 6570  , which is indep
+000136d0: 656e 6465 6e74 206f 6620 7374 7261 696e  endent of strain
+000136e0: 206c 696d 6974 2027 6227 2e0a 2020 2020   limit 'b'..    
+000136f0: 6572 7220 3d20 636f 6d70 7574 6545 7272  err = computeErr
+00013700: 6f72 4675 6e63 7469 6f6e 2863 7572 2c20  orFunction(cur, 
+00013710: 7265 662c 206e 7074 732c 206d 6178 4c61  ref, npts, maxLa
+00013720: 6729 0a0a 2020 2020 2320 6469 7265 6374  g)..    # direct
+00013730: 696f 6e20 746f 2061 6363 756d 756c 6174  ion to accumulat
+00013740: 6520 6572 726f 7273 2028 313d 666f 7277  e errors (1=forw
+00013750: 6172 642c 202d 313d 6261 636b 7761 7264  ard, -1=backward
+00013760: 290a 2020 2020 6469 7374 203d 2061 6363  ).    dist = acc
+00013770: 756d 756c 6174 6545 7272 6f72 4675 6e63  umulateErrorFunc
+00013780: 7469 6f6e 2864 6972 6563 7469 6f6e 2c20  tion(direction, 
+00013790: 6572 722c 206e 7074 732c 206d 6178 4c61  err, npts, maxLa
+000137a0: 672c 2062 290a 2020 2020 7374 6261 7220  g, b).    stbar 
+000137b0: 3d20 6261 636b 7472 6163 6b44 6973 7461  = backtrackDista
+000137c0: 6e63 6546 756e 6374 696f 6e28 2d31 202a  nceFunction(-1 *
+000137d0: 2064 6972 6563 7469 6f6e 2c20 6469 7374   direction, dist
+000137e0: 2c20 6572 722c 202d 6d61 784c 6167 2c20  , err, -maxLag, 
+000137f0: 6229 0a20 2020 2073 7462 6172 5469 6d65  b).    stbarTime
+00013800: 203d 2073 7462 6172 202a 2064 7420 2023   = stbar * dt  #
+00013810: 2063 6f6e 7665 7274 2066 726f 6d20 7361   convert from sa
+00013820: 6d70 6c65 7320 746f 2074 696d 650a 0a20  mples to time.. 
+00013830: 2020 2023 2063 7574 2074 6865 2066 6972     # cut the fir
+00013840: 7374 2061 6e64 206c 6173 7420 3525 2066  st and last 5% f
+00013850: 6f72 2062 6574 7465 7220 7265 6772 6573  or better regres
+00013860: 7369 6f6e 0a20 2020 2069 6e64 7820 3d20  sion.    indx = 
+00013870: 6e70 2e77 6865 7265 2828 7476 6563 7420  np.where((tvect 
+00013880: 3e3d 2030 2e30 3520 2a20 6e70 7473 202a  >= 0.05 * npts *
+00013890: 2064 7429 2026 2028 7476 6563 7420 3c3d   dt) & (tvect <=
+000138a0: 2030 2e39 3520 2a20 6e70 7473 202a 2064   0.95 * npts * d
+000138b0: 7429 295b 305d 0a0a 2020 2020 2320 6c69  t))[0]..    # li
+000138c0: 6e65 6172 2072 6567 7265 7373 696f 6e20  near regression 
+000138d0: 746f 2067 6574 2064 762f 760a 2020 2020  to get dv/v.    
+000138e0: 6966 206e 7074 7320 3e20 323a 0a20 2020  if npts > 2:.   
+000138f0: 2020 2020 2023 2077 6569 6768 7473 0a20       # weights. 
+00013900: 2020 2020 2020 2077 203d 206e 702e 6f6e         w = np.on
+00013910: 6573 286e 7074 7329 0a20 2020 2020 2020  es(npts).       
+00013920: 2023 206d 2c20 612c 2065 6d2c 2065 6120   # m, a, em, ea 
+00013930: 3d20 6c69 6e65 6172 5f72 6567 7265 7373  = linear_regress
+00013940: 696f 6e28 7469 6d65 5f61 7869 735b 696e  ion(time_axis[in
+00013950: 6478 5d2c 2064 656c 7461 5f74 5b69 6e64  dx], delta_t[ind
+00013960: 785d 2c20 772c 2069 6e74 6572 6365 7074  x], w, intercept
+00013970: 5f6f 7269 6769 6e3d 4661 6c73 6529 0a20  _origin=False). 
+00013980: 2020 2020 2020 206d 302c 2065 6d30 203d         m0, em0 =
+00013990: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
+000139a0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000139b0: 7476 6563 742e 666c 6174 7465 6e28 295b  tvect.flatten()[
+000139c0: 696e 6478 5d2c 0a20 2020 2020 2020 2020  indx],.         
+000139d0: 2020 2073 7462 6172 5469 6d65 2e66 6c61     stbarTime.fla
+000139e0: 7474 656e 2829 5b69 6e64 785d 2c0a 2020  tten()[indx],.  
+000139f0: 2020 2020 2020 2020 2020 772e 666c 6174            w.flat
+00013a00: 7465 6e28 295b 696e 6478 5d2c 0a20 2020  ten()[indx],.   
+00013a10: 2020 2020 2020 2020 2069 6e74 6572 6365           interce
+00013a20: 7074 5f6f 7269 6769 6e3d 5472 7565 2c0a  pt_origin=True,.
+00013a30: 2020 2020 2020 2020 290a 0a20 2020 2065          )..    e
+00013a40: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
+00013a50: 6765 722e 6465 6275 6728 226e 6f74 2065  ger.debug("not e
+00013a60: 6e6f 7567 6820 706f 696e 7473 2074 6f20  nough points to 
+00013a70: 6573 7469 6d61 7465 2064 762f 7620 666f  estimate dv/v fo
+00013a80: 7220 6474 7722 290a 2020 2020 2020 2020  r dtw").        
+00013a90: 6d30 203d 2030 0a20 2020 2020 2020 2065  m0 = 0.        e
+00013aa0: 6d30 203d 2030 0a0a 2020 2020 7265 7475  m0 = 0..    retu
+00013ab0: 726e 206d 3020 2a20 3130 302c 2065 6d30  rn m0 * 100, em0
+00013ac0: 202a 2031 3030 2c20 6469 7374 0a0a 0a64   * 100, dist...d
+00013ad0: 6566 206d 7763 735f 6476 7628 7265 662c  ef mwcs_dvv(ref,
+00013ae0: 2063 7572 2c20 6d6f 7669 6e67 5f77 696e   cur, moving_win
+00013af0: 646f 775f 6c65 6e67 7468 2c20 736c 6964  dow_length, slid
+00013b00: 655f 7374 6570 2c20 7061 7261 2c20 736d  e_step, para, sm
+00013b10: 6f6f 7468 696e 675f 6861 6c66 5f77 696e  oothing_half_win
+00013b20: 3d35 293a 0a20 2020 2022 2222 0a20 2020  =5):.    """.   
+00013b30: 204d 6f76 696e 6720 5769 6e64 6f77 2043   Moving Window C
+00013b40: 726f 7373 2053 7065 6374 7275 6d20 6d65  ross Spectrum me
+00013b50: 7468 6f64 2074 6f20 6d65 6173 7572 6520  thod to measure 
+00013b60: 6476 2f76 2028 7265 6c79 696e 6720 6f6e  dv/v (relying on
+00013b70: 2070 6869 3d32 2a70 692a 662a 7420 696e   phi=2*pi*f*t in
+00013b80: 2066 7265 7120 646f 6d61 696e 290a 0a20   freq domain).. 
+00013b90: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+00013ba0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00013bb0: 2d2d 2d0a 2020 2020 7265 663a 2052 6566  ---.    ref: Ref
+00013bc0: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
+00013bd0: 286e 702e 6e64 6172 7261 792c 2073 697a  (np.ndarray, siz
+00013be0: 6520 4e29 0a20 2020 2063 7572 3a20 4375  e N).    cur: Cu
+00013bf0: 7272 656e 7420 7761 7665 666f 726d 2028  rrent waveform (
+00013c00: 6e70 2e6e 6461 7272 6179 2c20 7369 7a65  np.ndarray, size
+00013c10: 204e 290a 2020 2020 6d6f 7669 6e67 5f77   N).    moving_w
+00013c20: 696e 646f 775f 6c65 6e67 7468 3a20 6d6f  indow_length: mo
+00013c30: 7669 6e67 2077 696e 646f 7720 6c65 6e67  ving window leng
+00013c40: 7468 2074 6f20 6361 6c63 756c 6174 6520  th to calculate 
+00013c50: 6372 6f73 732d 7370 6563 7472 756d 2028  cross-spectrum (
+00013c60: 6e70 2e66 6c6f 6174 2c20 696e 2073 6563  np.float, in sec
+00013c70: 290a 2020 2020 736c 6964 655f 7374 6570  ).    slide_step
+00013c80: 3a20 7374 6570 7320 696e 2074 696d 6520  : steps in time 
+00013c90: 746f 2073 6869 6674 2074 6865 206d 6f76  to shift the mov
+00013ca0: 696e 6720 7769 6e64 6f77 2028 6e70 2e66  ing window (np.f
+00013cb0: 6c6f 6174 2c20 696e 2073 6563 6f6e 6473  loat, in seconds
+00013cc0: 290a 2020 2020 7061 7261 3a20 6120 6469  ).    para: a di
+00013cd0: 6374 2063 6f6e 7461 696e 696e 6720 7061  ct containing pa
+00013ce0: 7261 6d65 7465 7273 2061 626f 7574 2069  rameters about i
+00013cf0: 6e70 7574 2064 6174 6120 7769 6e64 6f77  nput data window
+00013d00: 2061 6e64 2066 7265 7175 656e 6379 2069   and frequency i
+00013d10: 6e66 6f2c 2069 6e63 6c75 6469 6e67 0a20  nfo, including. 
+00013d20: 2020 2020 2020 2064 656c 7461 2d3e 5468         delta->Th
+00013d30: 6520 7361 6d70 6c69 6e67 2072 6174 6520  e sampling rate 
+00013d40: 6f66 2074 6865 2069 6e70 7574 2074 696d  of the input tim
+00013d50: 6573 6572 6965 7320 2869 6e20 487a 290a  eseries (in Hz).
+00013d60: 2020 2020 2020 2020 7769 6e64 6f77 2d3e          window->
+00013d70: 2054 6865 2074 6172 6765 7420 7769 6e64   The target wind
+00013d80: 6f77 2066 6f72 206d 6561 7375 7269 6e67  ow for measuring
+00013d90: 2064 742f 740a 2020 2020 2020 2020 6672   dt/t.        fr
+00013da0: 6571 2d3e 2054 6865 2066 7265 7175 656e  eq-> The frequen
+00013db0: 6379 2062 6f75 6e64 2074 6f20 636f 6d70  cy bound to comp
+00013dc0: 7574 6520 7468 6520 6465 7068 6173 696e  ute the dephasin
+00013dd0: 6720 2869 6e20 487a 290a 2020 2020 2020  g (in Hz).      
+00013de0: 2020 746d 696e 3a20 5468 6520 6c65 6674    tmin: The left
+00013df0: 6d6f 7374 2074 696d 6520 6c61 6720 2875  most time lag (u
+00013e00: 7365 6420 746f 2063 6f6d 7075 7465 2074  sed to compute t
+00013e10: 6865 2022 7469 6d65 206c 6167 7320 6172  he "time lags ar
+00013e20: 7261 7922 290a 2020 2020 736d 6f6f 7468  ray").    smooth
+00013e30: 696e 675f 6861 6c66 5f77 696e 3a20 4966  ing_half_win: If
+00013e40: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+00013e50: 302c 2064 6566 696e 6573 2074 6865 2068  0, defines the h
+00013e60: 616c 6620 6c65 6e67 7468 206f 6620 7468  alf length of th
+00013e70: 6520 736d 6f6f 7468 696e 6720 6861 6e6e  e smoothing hann
+00013e80: 696e 6720 7769 6e64 6f77 2e0a 0a20 2020  ing window...   
+00013e90: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+00013ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013eb0: 0a20 2020 2074 696d 655f 6178 6973 3a20  .    time_axis: 
+00013ec0: 7468 6520 6365 6e74 7261 6c20 7469 6d65  the central time
+00013ed0: 7320 6f66 2074 6865 2077 696e 646f 7773  s of the windows
+00013ee0: 2e0a 2020 2020 6465 6c74 615f 743a 2064  ..    delta_t: d
+00013ef0: 740a 2020 2020 6465 6c74 615f 6572 723a  t.    delta_err:
+00013f00: 6572 726f 720a 2020 2020 6465 6c74 615f  error.    delta_
+00013f10: 6d63 6f68 3a20 6d65 616e 2063 6f68 6572  mcoh: mean coher
+00013f20: 656e 6365 0a0a 2020 2020 436f 7069 6564  ence..    Copied
+00013f30: 2066 726f 6d20 4d53 4e6f 6973 6520 2868   from MSNoise (h
+00013f40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00013f50: 6d2f 524f 4265 6c67 6975 6d2f 4d53 4e6f  m/ROBelgium/MSNo
+00013f60: 6973 652f 7472 6565 2f6d 6173 7465 722f  ise/tree/master/
+00013f70: 6d73 6e6f 6973 6529 0a20 2020 204d 6f64  msnoise).    Mod
+00013f80: 6966 6965 6420 6279 2043 6865 6e67 7869  ified by Chengxi
+00013f90: 6e20 4a69 616e 670a 2020 2020 2222 220a  n Jiang.    """.
+00013fa0: 2020 2020 2320 636f 6d6d 6f6e 2076 6172      # common var
+00013fb0: 6961 626c 6573 0a20 2020 2074 7769 6e20  iables.    twin 
+00013fc0: 3d20 7061 7261 5b22 7477 696e 225d 0a20  = para["twin"]. 
+00013fd0: 2020 2066 7265 7120 3d20 7061 7261 5b22     freq = para["
+00013fe0: 6672 6571 225d 0a20 2020 2064 7420 3d20  freq"].    dt = 
+00013ff0: 7061 7261 5b22 6474 225d 0a20 2020 2074  para["dt"].    t
+00014000: 6d69 6e20 3d20 6e70 2e6d 696e 2874 7769  min = np.min(twi
+00014010: 6e29 0a20 2020 2066 6d69 6e20 3d20 6e70  n).    fmin = np
+00014020: 2e6d 696e 2866 7265 7129 0a20 2020 2066  .min(freq).    f
+00014030: 6d61 7820 3d20 6e70 2e6d 6178 2866 7265  max = np.max(fre
+00014040: 7129 0a0a 2020 2020 2320 7061 7261 6d65  q)..    # parame
+00014050: 7465 7220 696e 6974 6961 6c69 7a65 0a20  ter initialize. 
+00014060: 2020 2064 656c 7461 5f74 203d 205b 5d0a     delta_t = [].
+00014070: 2020 2020 6465 6c74 615f 6572 7220 3d20      delta_err = 
+00014080: 5b5d 0a20 2020 2064 656c 7461 5f6d 636f  [].    delta_mco
+00014090: 6820 3d20 5b5d 0a20 2020 2074 696d 655f  h = [].    time_
+000140a0: 6178 6973 203d 205b 5d0a 0a20 2020 2023  axis = []..    #
+000140b0: 2069 6e66 6f20 6f6e 2074 6865 206d 6f76   info on the mov
+000140c0: 696e 6720 7769 6e64 6f77 0a20 2020 2077  ing window.    w
+000140d0: 696e 646f 775f 6c65 6e67 7468 5f73 616d  indow_length_sam
+000140e0: 706c 6573 203d 206e 702e 696e 7428 6d6f  ples = np.int(mo
+000140f0: 7669 6e67 5f77 696e 646f 775f 6c65 6e67  ving_window_leng
+00014100: 7468 202f 2064 7429 0a20 2020 2070 6164  th / dt).    pad
+00014110: 6420 3d20 696e 7428 3220 2a2a 2028 6e65  d = int(2 ** (ne
+00014120: 7874 706f 7732 2877 696e 646f 775f 6c65  xtpow2(window_le
+00014130: 6e67 7468 5f73 616d 706c 6573 2920 2b20  ngth_samples) + 
+00014140: 3229 290a 2020 2020 636f 756e 7420 3d20  2)).    count = 
+00014150: 300a 2020 2020 7470 203d 2063 6f73 696e  0.    tp = cosin
+00014160: 655f 7461 7065 7228 7769 6e64 6f77 5f6c  e_taper(window_l
+00014170: 656e 6774 685f 7361 6d70 6c65 732c 2030  ength_samples, 0
+00014180: 2e31 3529 0a0a 2020 2020 6d69 6e69 6e64  .15)..    minind
+00014190: 203d 2030 0a20 2020 206d 6178 696e 6420   = 0.    maxind 
+000141a0: 3d20 7769 6e64 6f77 5f6c 656e 6774 685f  = window_length_
+000141b0: 7361 6d70 6c65 730a 0a20 2020 2023 206c  samples..    # l
+000141c0: 6f6f 7020 7468 726f 7567 6820 616c 6c20  oop through all 
+000141d0: 7375 622d 7769 6e64 6f77 730a 2020 2020  sub-windows.    
+000141e0: 7768 696c 6520 6d61 7869 6e64 203c 3d20  while maxind <= 
+000141f0: 6c65 6e28 7265 6629 3a0a 2020 2020 2020  len(ref):.      
+00014200: 2020 6363 6920 3d20 6375 725b 6d69 6e69    cci = cur[mini
+00014210: 6e64 3a6d 6178 696e 645d 0a20 2020 2020  nd:maxind].     
+00014220: 2020 2063 6369 203d 2073 6369 7079 2e73     cci = scipy.s
+00014230: 6967 6e61 6c2e 6465 7472 656e 6428 6363  ignal.detrend(cc
+00014240: 692c 2074 7970 653d 226c 696e 6561 7222  i, type="linear"
+00014250: 290a 2020 2020 2020 2020 6363 6920 2a3d  ).        cci *=
+00014260: 2074 700a 0a20 2020 2020 2020 2063 7269   tp..        cri
+00014270: 203d 2072 6566 5b6d 696e 696e 643a 6d61   = ref[minind:ma
+00014280: 7869 6e64 5d0a 2020 2020 2020 2020 6372  xind].        cr
+00014290: 6920 3d20 7363 6970 792e 7369 676e 616c  i = scipy.signal
+000142a0: 2e64 6574 7265 6e64 2863 7269 2c20 7479  .detrend(cri, ty
+000142b0: 7065 3d22 6c69 6e65 6172 2229 0a20 2020  pe="linear").   
+000142c0: 2020 2020 2063 7269 202a 3d20 7470 0a0a       cri *= tp..
+000142d0: 2020 2020 2020 2020 6d69 6e69 6e64 202b          minind +
+000142e0: 3d20 696e 7428 736c 6964 655f 7374 6570  = int(slide_step
+000142f0: 202f 2064 7429 0a20 2020 2020 2020 206d   / dt).        m
+00014300: 6178 696e 6420 2b3d 2069 6e74 2873 6c69  axind += int(sli
+00014310: 6465 5f73 7465 7020 2f20 6474 290a 0a20  de_step / dt).. 
+00014320: 2020 2020 2020 2023 2064 6f20 6666 740a         # do fft.
+00014330: 2020 2020 2020 2020 6663 7572 203d 2073          fcur = s
+00014340: 6369 7079 2e66 6674 7061 636b 2e66 6674  cipy.fftpack.fft
+00014350: 2863 6369 2c20 6e3d 7061 6464 295b 3a20  (cci, n=padd)[: 
+00014360: 7061 6464 202f 2f20 325d 0a20 2020 2020  padd // 2].     
+00014370: 2020 2066 7265 6620 3d20 7363 6970 792e     fref = scipy.
+00014380: 6666 7470 6163 6b2e 6666 7428 6372 692c  fftpack.fft(cri,
+00014390: 206e 3d70 6164 6429 5b3a 2070 6164 6420   n=padd)[: padd 
+000143a0: 2f2f 2032 5d0a 0a20 2020 2020 2020 2066  // 2]..        f
+000143b0: 6375 7232 203d 206e 702e 7265 616c 2866  cur2 = np.real(f
+000143c0: 6375 7229 202a 2a20 3220 2b20 6e70 2e69  cur) ** 2 + np.i
+000143d0: 6d61 6728 6663 7572 2920 2a2a 2032 0a20  mag(fcur) ** 2. 
+000143e0: 2020 2020 2020 2066 7265 6632 203d 206e         fref2 = n
+000143f0: 702e 7265 616c 2866 7265 6629 202a 2a20  p.real(fref) ** 
+00014400: 3220 2b20 6e70 2e69 6d61 6728 6672 6566  2 + np.imag(fref
+00014410: 2920 2a2a 2032 0a0a 2020 2020 2020 2020  ) ** 2..        
+00014420: 2320 6765 7420 6372 6f73 732d 7370 6563  # get cross-spec
+00014430: 7472 756d 2026 2064 6f20 6669 6c74 6572  trum & do filter
+00014440: 696e 670a 2020 2020 2020 2020 5820 3d20  ing.        X = 
+00014450: 6672 6566 202a 2028 6663 7572 2e63 6f6e  fref * (fcur.con
+00014460: 6a28 2929 0a20 2020 2020 2020 2069 6620  j()).        if 
+00014470: 736d 6f6f 7468 696e 675f 6861 6c66 5f77  smoothing_half_w
+00014480: 696e 2021 3d20 303a 0a20 2020 2020 2020  in != 0:.       
+00014490: 2020 2020 2064 6375 7220 3d20 6e70 2e73       dcur = np.s
+000144a0: 7172 7428 736d 6f6f 7468 2866 6375 7232  qrt(smooth(fcur2
+000144b0: 2c20 7769 6e64 6f77 3d22 6861 6e6e 696e  , window="hannin
+000144c0: 6722 2c20 6861 6c66 5f77 696e 3d73 6d6f  g", half_win=smo
+000144d0: 6f74 6869 6e67 5f68 616c 665f 7769 6e29  othing_half_win)
+000144e0: 290a 2020 2020 2020 2020 2020 2020 6472  ).            dr
+000144f0: 6566 203d 206e 702e 7371 7274 2873 6d6f  ef = np.sqrt(smo
+00014500: 6f74 6828 6672 6566 322c 2077 696e 646f  oth(fref2, windo
+00014510: 773d 2268 616e 6e69 6e67 222c 2068 616c  w="hanning", hal
+00014520: 665f 7769 6e3d 736d 6f6f 7468 696e 675f  f_win=smoothing_
+00014530: 6861 6c66 5f77 696e 2929 0a20 2020 2020  half_win)).     
+00014540: 2020 2020 2020 2058 203d 2073 6d6f 6f74         X = smoot
+00014550: 6828 582c 2077 696e 646f 773d 2268 616e  h(X, window="han
+00014560: 6e69 6e67 222c 2068 616c 665f 7769 6e3d  ning", half_win=
+00014570: 736d 6f6f 7468 696e 675f 6861 6c66 5f77  smoothing_half_w
+00014580: 696e 290a 2020 2020 2020 2020 656c 7365  in).        else
+00014590: 3a0a 2020 2020 2020 2020 2020 2020 6463  :.            dc
+000145a0: 7572 203d 206e 702e 7371 7274 2866 6375  ur = np.sqrt(fcu
+000145b0: 7232 290a 2020 2020 2020 2020 2020 2020  r2).            
+000145c0: 6472 6566 203d 206e 702e 7371 7274 2866  dref = np.sqrt(f
+000145d0: 7265 6632 290a 0a20 2020 2020 2020 2064  ref2)..        d
+000145e0: 6373 203d 206e 702e 6162 7328 5829 0a0a  cs = np.abs(X)..
+000145f0: 2020 2020 2020 2020 2320 4669 6e64 2074          # Find t
+00014600: 6865 2076 616c 7565 7320 7468 6520 6672  he values the fr
+00014610: 6571 7565 6e63 7920 7261 6e67 6520 6f66  equency range of
+00014620: 2069 6e74 6572 6573 740a 2020 2020 2020   interest.      
+00014630: 2020 6672 6571 5f76 6563 203d 2073 6369    freq_vec = sci
+00014640: 7079 2e66 6674 7061 636b 2e66 6674 6672  py.fftpack.fftfr
+00014650: 6571 286c 656e 2858 2920 2a20 322c 2064  eq(len(X) * 2, d
+00014660: 7429 5b3a 2070 6164 6420 2f2f 2032 5d0a  t)[: padd // 2].
+00014670: 2020 2020 2020 2020 696e 6465 785f 7261          index_ra
+00014680: 6e67 6520 3d20 6e70 2e61 7267 7768 6572  nge = np.argwher
+00014690: 6528 6e70 2e6c 6f67 6963 616c 5f61 6e64  e(np.logical_and
+000146a0: 2866 7265 715f 7665 6320 3e3d 2066 6d69  (freq_vec >= fmi
+000146b0: 6e2c 2066 7265 715f 7665 6320 3c3d 2066  n, freq_vec <= f
+000146c0: 6d61 7829 290a 0a20 2020 2020 2020 2023  max))..        #
+000146d0: 2047 6574 2043 6f68 6572 656e 6365 2061   Get Coherence a
+000146e0: 6e64 2069 7473 206d 6561 6e20 7661 6c75  nd its mean valu
+000146f0: 650a 2020 2020 2020 2020 636f 6820 3d20  e.        coh = 
+00014700: 6765 7443 6f68 6572 656e 6365 2864 6373  getCoherence(dcs
+00014710: 2c20 6472 6566 2c20 6463 7572 290a 2020  , dref, dcur).  
+00014720: 2020 2020 2020 6d63 6f68 203d 206e 702e        mcoh = np.
+00014730: 6d65 616e 2863 6f68 5b69 6e64 6578 5f72  mean(coh[index_r
+00014740: 616e 6765 5d29 0a0a 2020 2020 2020 2020  ange])..        
+00014750: 2320 4765 7420 5765 6967 6874 730a 2020  # Get Weights.  
+00014760: 2020 2020 2020 7720 3d20 312e 3020 2f20        w = 1.0 / 
+00014770: 2831 2e30 202f 2028 636f 685b 696e 6465  (1.0 / (coh[inde
+00014780: 785f 7261 6e67 655d 202a 2a20 3229 202d  x_range] ** 2) -
+00014790: 2031 2e30 290a 2020 2020 2020 2020 775b   1.0).        w[
+000147a0: 636f 685b 696e 6465 785f 7261 6e67 655d  coh[index_range]
+000147b0: 203e 3d20 302e 3939 5d20 3d20 312e 3020   >= 0.99] = 1.0 
+000147c0: 2f20 2831 2e30 202f 2030 2e39 3830 3120  / (1.0 / 0.9801 
+000147d0: 2d20 312e 3029 0a20 2020 2020 2020 2077  - 1.0).        w
+000147e0: 203d 206e 702e 7371 7274 2877 202a 206e   = np.sqrt(w * n
+000147f0: 702e 7371 7274 2864 6373 5b69 6e64 6578  p.sqrt(dcs[index
+00014800: 5f72 616e 6765 5d29 290a 2020 2020 2020  _range])).      
+00014810: 2020 7720 3d20 6e70 2e72 6561 6c28 7729    w = np.real(w)
+00014820: 0a0a 2020 2020 2020 2020 2320 4672 6571  ..        # Freq
+00014830: 7565 6e63 7920 6172 7261 793a 0a20 2020  uency array:.   
+00014840: 2020 2020 2076 203d 206e 702e 7265 616c       v = np.real
+00014850: 2866 7265 715f 7665 635b 696e 6465 785f  (freq_vec[index_
+00014860: 7261 6e67 655d 2920 2a20 3220 2a20 6e70  range]) * 2 * np
+00014870: 2e70 690a 0a20 2020 2020 2020 2023 2050  .pi..        # P
+00014880: 6861 7365 3a0a 2020 2020 2020 2020 7068  hase:.        ph
+00014890: 6920 3d20 6e70 2e61 6e67 6c65 2858 290a  i = np.angle(X).
+000148a0: 2020 2020 2020 2020 7068 695b 305d 203d          phi[0] =
+000148b0: 2030 2e30 0a20 2020 2020 2020 2070 6869   0.0.        phi
+000148c0: 203d 206e 702e 756e 7772 6170 2870 6869   = np.unwrap(phi
+000148d0: 290a 2020 2020 2020 2020 7068 6920 3d20  ).        phi = 
+000148e0: 7068 695b 696e 6465 785f 7261 6e67 655d  phi[index_range]
+000148f0: 0a0a 2020 2020 2020 2020 2320 4361 6c63  ..        # Calc
+00014900: 756c 6174 6520 7468 6520 736c 6f70 6520  ulate the slope 
+00014910: 7769 7468 2061 2077 6569 6768 7465 6420  with a weighted 
+00014920: 6c65 6173 7420 7371 7561 7265 206c 696e  least square lin
+00014930: 6561 7220 7265 6772 6573 7369 6f6e 0a20  ear regression. 
+00014940: 2020 2020 2020 2023 2066 6f72 6365 6420         # forced 
+00014950: 7468 726f 7567 6820 7468 6520 6f72 6967  through the orig
+00014960: 696e 3b20 7765 6967 6874 7320 666f 7220  in; weights for 
+00014970: 7468 6520 574c 5320 6d75 7374 2062 6520  the WLS must be 
+00014980: 7468 6520 7661 7269 616e 6365 2021 0a20  the variance !. 
+00014990: 2020 2020 2020 206d 2c20 656d 203d 206c         m, em = l
+000149a0: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
+000149b0: 2876 2e66 6c61 7474 656e 2829 2c20 7068  (v.flatten(), ph
+000149c0: 692e 666c 6174 7465 6e28 292c 2077 2e66  i.flatten(), w.f
+000149d0: 6c61 7474 656e 2829 290a 2020 2020 2020  latten()).      
+000149e0: 2020 6465 6c74 615f 742e 6170 7065 6e64    delta_t.append
+000149f0: 286d 290a 0a20 2020 2020 2020 2023 2070  (m)..        # p
+00014a00: 7269 6e74 2070 6869 2e73 6861 7065 2c20  rint phi.shape, 
+00014a10: 762e 7368 6170 652c 2077 2e73 6861 7065  v.shape, w.shape
+00014a20: 0a20 2020 2020 2020 2065 203d 206e 702e  .        e = np.
+00014a30: 7375 6d28 2870 6869 202d 206d 202a 2076  sum((phi - m * v
+00014a40: 2920 2a2a 2032 2920 2f20 286e 702e 7369  ) ** 2) / (np.si
+00014a50: 7a65 2876 2920 2d20 3129 0a20 2020 2020  ze(v) - 1).     
+00014a60: 2020 2073 3278 3220 3d20 6e70 2e73 756d     s2x2 = np.sum
+00014a70: 2876 2a2a 3220 2a20 772a 2a32 290a 2020  (v**2 * w**2).  
+00014a80: 2020 2020 2020 7378 3220 3d20 6e70 2e73        sx2 = np.s
+00014a90: 756d 2877 202a 2076 2a2a 3229 0a20 2020  um(w * v**2).   
+00014aa0: 2020 2020 2065 203d 206e 702e 7371 7274       e = np.sqrt
+00014ab0: 2865 202a 2073 3278 3220 2f20 7378 322a  (e * s2x2 / sx2*
+00014ac0: 2a32 290a 0a20 2020 2020 2020 2064 656c  *2)..        del
+00014ad0: 7461 5f65 7272 2e61 7070 656e 6428 6529  ta_err.append(e)
+00014ae0: 0a20 2020 2020 2020 2064 656c 7461 5f6d  .        delta_m
+00014af0: 636f 682e 6170 7065 6e64 286e 702e 7265  coh.append(np.re
+00014b00: 616c 286d 636f 6829 290a 2020 2020 2020  al(mcoh)).      
+00014b10: 2020 7469 6d65 5f61 7869 732e 6170 7065    time_axis.appe
+00014b20: 6e64 2874 6d69 6e20 2b20 6d6f 7669 6e67  nd(tmin + moving
+00014b30: 5f77 696e 646f 775f 6c65 6e67 7468 202f  _window_length /
+00014b40: 2032 2e30 202b 2063 6f75 6e74 202a 2073   2.0 + count * s
+00014b50: 6c69 6465 5f73 7465 7029 0a20 2020 2020  lide_step).     
+00014b60: 2020 2063 6f75 6e74 202b 3d20 310a 0a20     count += 1.. 
+00014b70: 2020 2020 2020 2064 656c 2066 6375 722c         del fcur,
+00014b80: 2066 7265 660a 2020 2020 2020 2020 6465   fref.        de
+00014b90: 6c20 580a 2020 2020 2020 2020 6465 6c20  l X.        del 
+00014ba0: 6672 6571 5f76 6563 0a20 2020 2020 2020  freq_vec.       
+00014bb0: 2064 656c 2069 6e64 6578 5f72 616e 6765   del index_range
+00014bc0: 0a20 2020 2020 2020 2064 656c 2077 2c20  .        del w, 
+00014bd0: 762c 2065 2c20 7332 7832 2c20 7378 322c  v, e, s2x2, sx2,
+00014be0: 206d 2c20 656d 0a0a 2020 2020 6966 206d   m, em..    if m
+00014bf0: 6178 696e 6420 3e20 6c65 6e28 6375 7229  axind > len(cur)
+00014c00: 202b 2069 6e74 2873 6c69 6465 5f73 7465   + int(slide_ste
+00014c10: 7020 2f20 6474 293a 0a20 2020 2020 2020  p / dt):.       
+00014c20: 206c 6f67 6765 722e 6465 6275 6728 2254   logger.debug("T
+00014c30: 6865 206c 6173 7420 7769 6e64 6f77 2077  he last window w
+00014c40: 6173 2074 6f6f 2073 6d61 6c6c 2c20 6275  as too small, bu
+00014c50: 7420 7761 7320 636f 6d70 7574 6564 2229  t was computed")
+00014c60: 0a0a 2020 2020 2320 656e 7375 7265 2061  ..    # ensure a
+00014c70: 6c6c 206d 6174 7269 7820 6172 6520 6e70  ll matrix are np
+00014c80: 2061 7272 6179 0a20 2020 2064 656c 7461   array.    delta
+00014c90: 5f74 203d 206e 702e 6172 7261 7928 6465  _t = np.array(de
+00014ca0: 6c74 615f 7429 0a20 2020 2064 656c 7461  lta_t).    delta
+00014cb0: 5f65 7272 203d 206e 702e 6172 7261 7928  _err = np.array(
+00014cc0: 6465 6c74 615f 6572 7229 0a20 2020 2064  delta_err).    d
+00014cd0: 656c 7461 5f6d 636f 6820 3d20 6e70 2e61  elta_mcoh = np.a
+00014ce0: 7272 6179 2864 656c 7461 5f6d 636f 6829  rray(delta_mcoh)
+00014cf0: 0a20 2020 2074 696d 655f 6178 6973 203d  .    time_axis =
+00014d00: 206e 702e 6172 7261 7928 7469 6d65 5f61   np.array(time_a
+00014d10: 7869 7329 0a0a 2020 2020 2320 7265 6164  xis)..    # read
+00014d20: 7920 666f 7220 6c69 6e65 6172 2072 6567  y for linear reg
+00014d30: 7265 7373 696f 6e0a 2020 2020 6465 6c74  ression.    delt
+00014d40: 615f 6d69 6e63 686f 203d 2030 2e36 350a  a_mincho = 0.65.
+00014d50: 2020 2020 6465 6c74 615f 6d61 7865 7272      delta_maxerr
+00014d60: 203d 2030 2e31 0a20 2020 2064 656c 7461   = 0.1.    delta
+00014d70: 5f6d 6178 6474 203d 2030 2e31 0a20 2020  _maxdt = 0.1.   
+00014d80: 2069 6e64 7831 203d 206e 702e 7768 6572   indx1 = np.wher
+00014d90: 6528 6465 6c74 615f 6d63 6f68 203e 2064  e(delta_mcoh > d
+00014da0: 656c 7461 5f6d 696e 6368 6f29 0a20 2020  elta_mincho).   
+00014db0: 2069 6e64 7832 203d 206e 702e 7768 6572   indx2 = np.wher
+00014dc0: 6528 6465 6c74 615f 6572 7220 3c20 6465  e(delta_err < de
+00014dd0: 6c74 615f 6d61 7865 7272 290a 2020 2020  lta_maxerr).    
+00014de0: 696e 6478 3320 3d20 6e70 2e77 6865 7265  indx3 = np.where
+00014df0: 2864 656c 7461 5f74 203c 2064 656c 7461  (delta_t < delta
+00014e00: 5f6d 6178 6474 290a 0a20 2020 2023 202d  _maxdt)..    # -
+00014e10: 2d2d 2d2d 6669 6e64 2067 6f6f 6420 6474  ----find good dt
+00014e20: 206d 6561 7375 7265 6d65 6e74 732d 2d2d   measurements---
+00014e30: 2d2d 0a20 2020 2069 6e64 7820 3d20 6e70  --.    indx = np
+00014e40: 2e69 6e74 6572 7365 6374 3164 2869 6e64  .intersect1d(ind
+00014e50: 7831 2c20 696e 6478 3229 0a20 2020 2069  x1, indx2).    i
+00014e60: 6e64 7820 3d20 6e70 2e69 6e74 6572 7365  ndx = np.interse
+00014e70: 6374 3164 2869 6e64 782c 2069 6e64 7833  ct1d(indx, indx3
+00014e80: 290a 0a20 2020 2069 6620 6c65 6e28 696e  )..    if len(in
+00014e90: 6478 2920 3e20 323a 0a20 2020 2020 2020  dx) > 2:.       
+00014ea0: 2023 202d 2d2d 2d65 7374 696d 6174 6520   # ----estimate 
+00014eb0: 7765 6967 6874 2066 6f72 2072 6567 7265  weight for regre
+00014ec0: 7373 696f 6e2d 2d2d 2d0a 2020 2020 2020  ssion----.      
+00014ed0: 2020 7720 3d20 3120 2f20 6465 6c74 615f    w = 1 / delta_
+00014ee0: 6572 725b 696e 6478 5d0a 2020 2020 2020  err[indx].      
+00014ef0: 2020 775b 7e6e 702e 6973 6669 6e69 7465    w[~np.isfinite
+00014f00: 2877 295d 203d 2031 2e30 0a0a 2020 2020  (w)] = 1.0..    
+00014f10: 2020 2020 2320 2d2d 2d2d 2d2d 2d2d 2d64      # ---------d
+00014f20: 6f20 6c69 6e65 6172 2072 6567 7265 7373  o linear regress
+00014f30: 696f 6e2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  ion-----------. 
+00014f40: 2020 2020 2020 2023 206d 2c20 612c 2065         # m, a, e
+00014f50: 6d2c 2065 6120 3d20 6c69 6e65 6172 5f72  m, ea = linear_r
+00014f60: 6567 7265 7373 696f 6e28 7469 6d65 5f61  egression(time_a
+00014f70: 7869 735b 696e 6478 5d2c 2064 656c 7461  xis[indx], delta
+00014f80: 5f74 5b69 6e64 785d 2c20 772c 2069 6e74  _t[indx], w, int
+00014f90: 6572 6365 7074 5f6f 7269 6769 6e3d 4661  ercept_origin=Fa
+00014fa0: 6c73 6529 0a20 2020 2020 2020 206d 302c  lse).        m0,
+00014fb0: 2065 6d30 203d 206c 696e 6561 725f 7265   em0 = linear_re
+00014fc0: 6772 6573 7369 6f6e 2874 696d 655f 6178  gression(time_ax
+00014fd0: 6973 5b69 6e64 785d 2c20 6465 6c74 615f  is[indx], delta_
+00014fe0: 745b 696e 6478 5d2c 2077 2c20 696e 7465  t[indx], w, inte
+00014ff0: 7263 6570 745f 6f72 6967 696e 3d54 7275  rcept_origin=Tru
+00015000: 6529 0a0a 2020 2020 656c 7365 3a0a 2020  e)..    else:.  
+00015010: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00015020: 7567 2822 6e6f 7420 656e 6f75 6768 2070  ug("not enough p
+00015030: 6f69 6e74 7320 746f 2065 7374 696d 6174  oints to estimat
+00015040: 6520 6476 2f76 2066 6f72 206d 7763 7322  e dv/v for mwcs"
+00015050: 290a 2020 2020 2020 2020 6d30 203d 2030  ).        m0 = 0
+00015060: 0a20 2020 2020 2020 2065 6d30 203d 2030  .        em0 = 0
+00015070: 0a0a 2020 2020 7265 7475 726e 202d 6d30  ..    return -m0
+00015080: 202a 2031 3030 2c20 656d 3020 2a20 3130   * 100, em0 * 10
+00015090: 300a 0a0a 6465 6620 5743 435f 6476 7628  0...def WCC_dvv(
+000150a0: 7265 662c 2063 7572 2c20 6d6f 7669 6e67  ref, cur, moving
+000150b0: 5f77 696e 646f 775f 6c65 6e67 7468 2c20  _window_length, 
+000150c0: 736c 6964 655f 7374 6570 2c20 7061 7261  slide_step, para
+000150d0: 293a 0a20 2020 2022 2222 0a20 2020 2057  ):.    """.    W
+000150e0: 696e 646f 7765 6420 6372 6f73 7320 636f  indowed cross co
+000150f0: 7272 656c 6174 696f 6e20 2857 4343 2920  rrelation (WCC) 
+00015100: 666f 7220 6474 206f 7220 6476 2f76 206d  for dt or dv/v m
+00015110: 6573 7572 656d 656e 7420 2853 6e69 6564  esurement (Snied
+00015120: 6572 2065 7420 616c 2e20 3230 3132 290a  er et al. 2012).
+00015130: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
+00015140: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00015150: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
+00015160: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
+00015170: 7269 6573 0a20 2020 2063 7572 3a20 5468  ries.    cur: Th
+00015180: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
+00015190: 7365 7269 6573 0a20 2020 206d 6f76 696e  series.    movin
+000151a0: 675f 7769 6e64 6f77 5f6c 656e 6774 683a  g_window_length:
+000151b0: 2054 6865 206d 6f76 696e 6720 7769 6e64   The moving wind
+000151c0: 6f77 206c 656e 6774 6820 2869 6e20 7365  ow length (in se
+000151d0: 636f 6e64 7329 0a20 2020 2073 6c69 6465  conds).    slide
+000151e0: 5f73 7465 703a 2054 6865 2073 7465 7020  _step: The step 
+000151f0: 746f 206a 756d 7020 666f 7220 7468 6520  to jump for the 
+00015200: 6d6f 7669 6e67 2077 696e 646f 7720 2869  moving window (i
+00015210: 6e20 7365 636f 6e64 7329 0a20 2020 2070  n seconds).    p
+00015220: 6172 613a 2061 2064 6963 7420 636f 6e74  ara: a dict cont
+00015230: 6169 6e69 6e67 2066 7265 712f 7469 6d65  aining freq/time
+00015240: 2069 6e66 6f20 6f66 2074 6865 2064 6174   info of the dat
+00015250: 6120 6d61 7472 6978 0a0a 2020 2020 5265  a matrix..    Re
+00015260: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
+00015270: 2d2d 2d2d 2d2d 2d0a 2020 2020 7469 6d65  -------.    time
+00015280: 5f61 7869 733a 2063 656e 7472 616c 2074  _axis: central t
+00015290: 696d 6573 206f 6620 7468 6520 6d6f 7669  imes of the movi
+000152a0: 6e67 2077 696e 646f 770a 2020 2020 6465  ng window.    de
+000152b0: 6c74 615f 743a 2064 740a 2020 2020 6465  lta_t: dt.    de
+000152c0: 6c74 615f 6572 723a 2065 7272 6f72 0a20  lta_err: error. 
+000152d0: 2020 2064 656c 7461 5f6d 636f 683a 206d     delta_mcoh: m
+000152e0: 6561 6e20 636f 6865 7265 6e63 6520 666f  ean coherence fo
+000152f0: 7220 6561 6368 2077 696e 646f 770a 0a20  r each window.. 
+00015300: 2020 2057 7269 7474 656e 2062 7920 436f     Written by Co
+00015310: 6e67 636f 6e67 2059 7561 6e20 2831 204a  ngcong Yuan (1 J
+00015320: 756c 792c 2032 3031 3929 0a20 2020 2022  uly, 2019).    "
+00015330: 2222 0a20 2020 2023 2063 6f6d 6d6f 6e20  "".    # common 
+00015340: 7661 7269 6162 6c65 730a 2020 2020 7477  variables.    tw
+00015350: 696e 203d 2070 6172 615b 2274 7769 6e22  in = para["twin"
+00015360: 5d0a 2020 2020 6474 203d 2070 6172 615b  ].    dt = para[
+00015370: 2264 7422 5d0a 2020 2020 746d 696e 203d  "dt"].    tmin =
+00015380: 206e 702e 6d69 6e28 7477 696e 290a 0a20   np.min(twin).. 
+00015390: 2020 2023 2070 6172 616d 6574 6572 2069     # parameter i
+000153a0: 6e69 7469 616c 697a 650a 2020 2020 6465  nitialize.    de
+000153b0: 6c74 615f 7420 3d20 5b5d 0a20 2020 2064  lta_t = [].    d
+000153c0: 656c 7461 5f74 5f63 6f65 6620 3d20 5b5d  elta_t_coef = []
+000153d0: 0a20 2020 2074 696d 655f 6178 6973 203d  .    time_axis =
+000153e0: 205b 5d0a 0a20 2020 2023 2069 6e66 6f20   []..    # info 
+000153f0: 6f6e 2074 6865 206d 6f76 696e 6720 7769  on the moving wi
+00015400: 6e64 6f77 0a20 2020 2077 696e 646f 775f  ndow.    window_
+00015410: 6c65 6e67 7468 5f73 616d 706c 6573 203d  length_samples =
+00015420: 206e 702e 696e 7428 6d6f 7669 6e67 5f77   np.int(moving_w
+00015430: 696e 646f 775f 6c65 6e67 7468 202f 2064  indow_length / d
+00015440: 7429 0a20 2020 2063 6f75 6e74 203d 2030  t).    count = 0
+00015450: 0a20 2020 2074 7020 3d20 636f 7369 6e65  .    tp = cosine
+00015460: 5f74 6170 6572 2877 696e 646f 775f 6c65  _taper(window_le
+00015470: 6e67 7468 5f73 616d 706c 6573 2c20 302e  ngth_samples, 0.
+00015480: 3135 290a 0a20 2020 206d 696e 696e 6420  15)..    minind 
+00015490: 3d20 300a 2020 2020 6d61 7869 6e64 203d  = 0.    maxind =
+000154a0: 2077 696e 646f 775f 6c65 6e67 7468 5f73   window_length_s
+000154b0: 616d 706c 6573 0a0a 2020 2020 2320 6c6f  amples..    # lo
+000154c0: 6f70 2074 6872 6f75 6768 2061 6c6c 2073  op through all s
+000154d0: 7562 2d77 696e 646f 7773 0a20 2020 2077  ub-windows.    w
+000154e0: 6869 6c65 206d 6178 696e 6420 3c3d 206c  hile maxind <= l
+000154f0: 656e 2872 6566 293a 0a20 2020 2020 2020  en(ref):.       
+00015500: 2063 6369 203d 2063 7572 5b6d 696e 696e   cci = cur[minin
+00015510: 643a 6d61 7869 6e64 5d0a 2020 2020 2020  d:maxind].      
+00015520: 2020 6363 6920 3d20 7363 6970 792e 7369    cci = scipy.si
+00015530: 676e 616c 2e64 6574 7265 6e64 2863 6369  gnal.detrend(cci
+00015540: 2c20 7479 7065 3d22 6c69 6e65 6172 2229  , type="linear")
+00015550: 0a20 2020 2020 2020 2063 6369 202a 3d20  .        cci *= 
+00015560: 7470 0a0a 2020 2020 2020 2020 6372 6920  tp..        cri 
+00015570: 3d20 7265 665b 6d69 6e69 6e64 3a6d 6178  = ref[minind:max
+00015580: 696e 645d 0a20 2020 2020 2020 2063 7269  ind].        cri
+00015590: 203d 2073 6369 7079 2e73 6967 6e61 6c2e   = scipy.signal.
+000155a0: 6465 7472 656e 6428 6372 692c 2074 7970  detrend(cri, typ
+000155b0: 653d 226c 696e 6561 7222 290a 2020 2020  e="linear").    
+000155c0: 2020 2020 6372 6920 2a3d 2074 700a 0a20      cri *= tp.. 
+000155d0: 2020 2020 2020 206d 696e 696e 6420 2b3d         minind +=
+000155e0: 2069 6e74 2873 6c69 6465 5f73 7465 7020   int(slide_step 
+000155f0: 2f20 6474 290a 2020 2020 2020 2020 6d61  / dt).        ma
+00015600: 7869 6e64 202b 3d20 696e 7428 736c 6964  xind += int(slid
+00015610: 655f 7374 6570 202f 2064 7429 0a0a 2020  e_step / dt)..  
+00015620: 2020 2020 2020 2320 6e6f 726d 616c 697a        # normaliz
+00015630: 6520 7369 676e 616c 7320 6265 666f 7265  e signals before
+00015640: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
+00015650: 6f6e 0a20 2020 2020 2020 2063 6369 203d  on.        cci =
+00015660: 2028 6363 6920 2d20 6363 692e 6d65 616e   (cci - cci.mean
+00015670: 2829 2920 2f20 6363 692e 7374 6428 290a  ()) / cci.std().
+00015680: 2020 2020 2020 2020 6372 6920 3d20 2863          cri = (c
+00015690: 7269 202d 2063 7269 2e6d 6561 6e28 2929  ri - cri.mean())
+000156a0: 202f 2063 7269 2e73 7464 2829 0a0a 2020   / cri.std()..  
+000156b0: 2020 2020 2020 2320 6765 7420 6d61 7869        # get maxi
+000156c0: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
+000156d0: 636f 6566 6669 6369 656e 7420 616e 6420  coefficient and 
+000156e0: 6974 7320 696e 6465 780a 2020 2020 2020  its index.      
+000156f0: 2020 6363 3220 3d20 6e70 2e63 6f72 7265    cc2 = np.corre
+00015700: 6c61 7465 2863 6369 2c20 6372 692c 206d  late(cci, cri, m
+00015710: 6f64 653d 2273 616d 6522 290a 2020 2020  ode="same").    
+00015720: 2020 2020 6363 3220 3d20 6363 3220 2f20      cc2 = cc2 / 
+00015730: 6e70 2e73 7172 7428 2863 6369 2a2a 3229  np.sqrt((cci**2)
+00015740: 2e73 756d 2829 202a 2028 6372 692a 2a32  .sum() * (cri**2
+00015750: 292e 7375 6d28 2929 0a0a 2020 2020 2020  ).sum())..      
+00015760: 2020 696d 6178 6363 3220 3d20 6e70 2e77    imaxcc2 = np.w
+00015770: 6865 7265 2863 6332 203d 3d20 6e70 2e6d  here(cc2 == np.m
+00015780: 6178 2863 6332 2929 5b30 5d0a 2020 2020  ax(cc2))[0].    
+00015790: 2020 2020 6d61 7863 6332 203d 206e 702e      maxcc2 = np.
+000157a0: 6d61 7828 6363 3229 0a0a 2020 2020 2020  max(cc2)..      
+000157b0: 2020 2320 6765 7420 7468 6520 7469 6d65    # get the time
+000157c0: 2073 6869 6674 0a20 2020 2020 2020 206d   shift.        m
+000157d0: 203d 2028 696d 6178 6363 3220 2d20 2828   = (imaxcc2 - ((
+000157e0: 6d61 7869 6e64 202d 206d 696e 696e 6429  maxind - minind)
+000157f0: 202f 2f20 3229 2920 2a20 6474 0a20 2020   // 2)) * dt.   
+00015800: 2020 2020 2064 656c 7461 5f74 2e61 7070       delta_t.app
+00015810: 656e 6428 6d29 0a20 2020 2020 2020 2064  end(m).        d
+00015820: 656c 7461 5f74 5f63 6f65 662e 6170 7065  elta_t_coef.appe
+00015830: 6e64 286d 6178 6363 3229 0a0a 2020 2020  nd(maxcc2)..    
+00015840: 2020 2020 7469 6d65 5f61 7869 732e 6170      time_axis.ap
+00015850: 7065 6e64 2874 6d69 6e20 2b20 6d6f 7669  pend(tmin + movi
+00015860: 6e67 5f77 696e 646f 775f 6c65 6e67 7468  ng_window_length
+00015870: 202f 2032 2e30 202b 2063 6f75 6e74 202a   / 2.0 + count *
+00015880: 2073 6c69 6465 5f73 7465 7029 0a20 2020   slide_step).   
+00015890: 2020 2020 2063 6f75 6e74 202b 3d20 310a       count += 1.
+000158a0: 0a20 2020 2064 656c 2063 6369 2c20 6372  .    del cci, cr
+000158b0: 692c 2063 6332 2c20 696d 6178 6363 322c  i, cc2, imaxcc2,
+000158c0: 206d 6178 6363 320a 2020 2020 6465 6c20   maxcc2.    del 
+000158d0: 6d0a 0a20 2020 2069 6620 6d61 7869 6e64  m..    if maxind
+000158e0: 203e 206c 656e 2863 7572 2920 2b20 696e   > len(cur) + in
+000158f0: 7428 736c 6964 655f 7374 6570 202f 2064  t(slide_step / d
+00015900: 7429 3a0a 2020 2020 2020 2020 6c6f 6767  t):.        logg
+00015910: 6572 2e64 6562 7567 2822 5468 6520 6c61  er.debug("The la
+00015920: 7374 2077 696e 646f 7720 7761 7320 746f  st window was to
+00015930: 6f20 736d 616c 6c2c 2062 7574 2077 6173  o small, but was
+00015940: 2063 6f6d 7075 7465 6422 290a 0a20 2020   computed")..   
+00015950: 2064 656c 7461 5f74 203d 206e 702e 6172   delta_t = np.ar
+00015960: 7261 7928 6465 6c74 615f 7429 0a20 2020  ray(delta_t).   
+00015970: 2064 656c 7461 5f74 5f63 6f65 6620 3d20   delta_t_coef = 
+00015980: 6e70 2e61 7272 6179 2864 656c 7461 5f74  np.array(delta_t
+00015990: 5f63 6f65 6629 0a20 2020 2074 696d 655f  _coef).    time_
+000159a0: 6178 6973 203d 206e 702e 6172 7261 7928  axis = np.array(
+000159b0: 7469 6d65 5f61 7869 7329 0a0a 2020 2020  time_axis)..    
+000159c0: 2320 6c69 6e65 6172 2072 6567 7265 7373  # linear regress
+000159d0: 696f 6e20 746f 2067 6574 2064 762f 760a  ion to get dv/v.
+000159e0: 2020 2020 6966 2063 6f75 6e74 203e 2032      if count > 2
+000159f0: 3a0a 2020 2020 2020 2020 2320 7369 6d70  :.        # simp
+00015a00: 6c65 2077 6569 6768 740a 2020 2020 2020  le weight.      
+00015a10: 2020 7720 3d20 6e70 2e6f 6e65 7328 636f    w = np.ones(co
+00015a20: 756e 7429 0a20 2020 2020 2020 2023 206d  unt).        # m
+00015a30: 2c20 612c 2065 6d2c 2065 6120 3d20 6c69  , a, em, ea = li
+00015a40: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
+00015a50: 7469 6d65 5f61 7869 735b 696e 6478 5d2c  time_axis[indx],
+00015a60: 2064 656c 7461 5f74 5b69 6e64 785d 2c20   delta_t[indx], 
+00015a70: 772c 2069 6e74 6572 6365 7074 5f6f 7269  w, intercept_ori
+00015a80: 6769 6e3d 4661 6c73 6529 0a20 2020 2020  gin=False).     
+00015a90: 2020 206d 302c 2065 6d30 203d 206c 696e     m0, em0 = lin
+00015aa0: 6561 725f 7265 6772 6573 7369 6f6e 2874  ear_regression(t
+00015ab0: 696d 655f 6178 6973 2e66 6c61 7474 656e  ime_axis.flatten
+00015ac0: 2829 2c20 6465 6c74 615f 742e 666c 6174  (), delta_t.flat
+00015ad0: 7465 6e28 292c 2077 2e66 6c61 7474 656e  ten(), w.flatten
+00015ae0: 2829 2c20 696e 7465 7263 6570 745f 6f72  (), intercept_or
+00015af0: 6967 696e 3d54 7275 6529 0a0a 2020 2020  igin=True)..    
+00015b00: 656c 7365 3a0a 2020 2020 2020 2020 6c6f  else:.        lo
+00015b10: 6767 6572 2e64 6562 7567 2822 6e6f 7420  gger.debug("not 
+00015b20: 656e 6f75 6768 2070 6f69 6e74 7320 746f  enough points to
+00015b30: 2065 7374 696d 6174 6520 6476 2f76 2066   estimate dv/v f
+00015b40: 6f72 2077 6363 2229 0a20 2020 2020 2020  or wcc").       
+00015b50: 206d 3020 3d20 300a 2020 2020 2020 2020   m0 = 0.        
+00015b60: 656d 3020 3d20 300a 0a20 2020 2072 6574  em0 = 0..    ret
+00015b70: 7572 6e20 2d6d 3020 2a20 3130 302c 2065  urn -m0 * 100, e
+00015b80: 6d30 202a 2031 3030 0a0a 0a64 6566 2077  m0 * 100...def w
+00015b90: 7873 5f64 7676 280a 2020 2020 7265 662c  xs_dvv(.    ref,
+00015ba0: 0a20 2020 2063 7572 2c0a 2020 2020 616c  .    cur,.    al
+00015bb0: 6c66 7265 712c 0a20 2020 2070 6172 612c  lfreq,.    para,
+00015bc0: 0a20 2020 2064 6a3d 3120 2f20 3132 2c0a  .    dj=1 / 12,.
+00015bd0: 2020 2020 7330 3d2d 312c 0a20 2020 204a      s0=-1,.    J
+00015be0: 3d2d 312c 0a20 2020 2073 6967 3d46 616c  =-1,.    sig=Fal
+00015bf0: 7365 2c0a 2020 2020 7776 6e3d 226d 6f72  se,.    wvn="mor
+00015c00: 6c65 7422 2c0a 2020 2020 756e 7772 6170  let",.    unwrap
+00015c10: 666c 6167 3d46 616c 7365 2c0a 293a 0a20  flag=False,.):. 
+00015c20: 2020 2022 2222 0a20 2020 2043 6f6d 7075     """.    Compu
+00015c30: 7465 2064 7420 6f72 2064 762f 7620 696e  te dt or dv/v in
+00015c40: 2074 696d 6520 616e 6420 6672 6571 7565   time and freque
+00015c50: 6e63 7920 646f 6d61 696e 2066 726f 6d20  ncy domain from 
+00015c60: 7761 7665 6c65 7420 6372 6f73 7320 7370  wavelet cross sp
+00015c70: 6563 7472 756d 2028 7778 7329 2e0a 2020  ectrum (wxs)..  
+00015c80: 2020 666f 7220 616c 6c20 6672 6571 7565    for all freque
+00015c90: 6369 6573 2069 6e20 616e 2069 6e74 6572  cies in an inter
+00015ca0: 6573 7420 7261 6e67 650a 0a20 2020 2050  est range..    P
+00015cb0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00015cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00015cd0: 2072 6566 3a20 5468 6520 2252 6566 6572   ref: The "Refer
+00015ce0: 656e 6365 2220 7469 6d65 7365 7269 6573  ence" timeseries
+00015cf0: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
+00015d00: 0a20 2020 2063 7572 3a20 5468 6520 2243  .    cur: The "C
+00015d10: 7572 7265 6e74 2220 7469 6d65 7365 7269  urrent" timeseri
+00015d20: 6573 2028 6e75 6d70 792e 6e64 6172 7261  es (numpy.ndarra
+00015d30: 7929 0a20 2020 2061 6c6c 6672 6571 3a20  y).    allfreq: 
+00015d40: 6120 626f 6f6c 656e 2076 6172 6961 626c  a boolen variabl
+00015d50: 6520 746f 206d 616b 6520 6d65 6173 7572  e to make measur
+00015d60: 656d 656e 7473 206f 6e20 616c 6c20 6672  ements on all fr
+00015d70: 6571 7565 6e63 7920 7261 6e67 6520 6f72  equency range or
+00015d80: 206e 6f74 0a20 2020 2070 6172 613a 2061   not.    para: a
+00015d90: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
+00015da0: 2066 7265 712f 7469 6d65 2069 6e66 6f20   freq/time info 
+00015db0: 6f66 2074 6865 2064 6174 6120 6d61 7472  of the data matr
+00015dc0: 6978 0a20 2020 2064 6a2c 2073 302c 204a  ix.    dj, s0, J
+00015dd0: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
+00015de0: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
+00015df0: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
+00015e00: 6374 270a 2020 2020 756e 7772 6170 666c  ct'.    unwrapfl
+00015e10: 6167 3a20 5472 7565 202d 2075 6e77 7261  ag: True - unwra
+00015e20: 7020 7068 6173 6520 6465 6c61 7973 2e20  p phase delays. 
+00015e30: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
+00015e40: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
+00015e50: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00015e60: 2d2d 2d2d 2d0a 2020 2020 6476 762a 3130  -----.    dvv*10
+00015e70: 3020 3a20 6573 7469 6d61 7465 6420 6476  0 : estimated dv
+00015e80: 2f76 2069 6e20 250a 2020 2020 6572 722a  /v in %.    err*
+00015e90: 3130 3020 3a20 6572 726f 7220 6f66 2064  100 : error of d
+00015ea0: 762f 7620 6573 7469 6d61 7469 6f6e 2069  v/v estimation i
+00015eb0: 6e20 250a 0a20 2020 204f 7269 6769 6e61  n %..    Origina
+00015ec0: 6c6c 7920 7772 6974 7465 6e20 6279 2054  lly written by T
+00015ed0: 696d 2043 6c65 6d65 6e74 7320 2831 204d  im Clements (1 M
+00015ee0: 6172 6368 2c20 3230 3139 290a 2020 2020  arch, 2019).    
+00015ef0: 4d6f 6469 6669 6564 2062 7920 436f 6e67  Modified by Cong
+00015f00: 636f 6e67 2059 7561 6e20 2833 3020 4a75  cong Yuan (30 Ju
+00015f10: 6e65 2c20 3230 3139 2920 6261 7365 6420  ne, 2019) based 
+00015f20: 6f6e 2028 4d61 6f20 6574 2061 6c2e 2032  on (Mao et al. 2
+00015f30: 3031 3929 2e0a 2020 2020 5570 6461 7465  019)..    Update
+00015f40: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
+00015f50: 616e 6720 2831 3020 4f63 742c 2032 3031  ang (10 Oct, 201
+00015f60: 3929 2074 6f20 6d65 7267 6520 7468 6520  9) to merge the 
+00015f70: 6675 6e63 7469 6f6e 616c 6974 7920 666f  functionality fo
+00015f80: 7220 6d65 7375 7265 6d65 6e74 730a 2020  r mesurements.  
+00015f90: 2020 6163 726f 7373 2061 6c6c 2066 7265    across all fre
+00015fa0: 7175 656e 6379 2061 6e64 206f 6e65 2066  quency and one f
+00015fb0: 7265 7120 7261 6e67 650a 2020 2020 2222  req range.    ""
+00015fc0: 220a 2020 2020 2320 636f 6d6d 6f6e 2076  ".    # common v
+00015fd0: 6172 6961 626c 6573 0a20 2020 2074 7769  ariables.    twi
+00015fe0: 6e20 3d20 7061 7261 5b22 7477 696e 225d  n = para["twin"]
+00015ff0: 0a20 2020 2066 7265 7120 3d20 7061 7261  .    freq = para
+00016000: 5b22 6672 6571 225d 0a20 2020 2064 7420  ["freq"].    dt 
+00016010: 3d20 7061 7261 5b22 6474 225d 0a20 2020  = para["dt"].   
+00016020: 2074 6d69 6e20 3d20 6e70 2e6d 696e 2874   tmin = np.min(t
+00016030: 7769 6e29 0a20 2020 2074 6d61 7820 3d20  win).    tmax = 
+00016040: 6e70 2e6d 6178 2874 7769 6e29 0a20 2020  np.max(twin).   
+00016050: 2066 6d69 6e20 3d20 6e70 2e6d 696e 2866   fmin = np.min(f
+00016060: 7265 7129 0a20 2020 2066 6d61 7820 3d20  req).    fmax = 
+00016070: 6e70 2e6d 6178 2866 7265 7129 0a20 2020  np.max(freq).   
+00016080: 2074 7665 6320 3d20 6e70 2e61 7261 6e67   tvec = np.arang
+00016090: 6528 746d 696e 2c20 746d 6178 2c20 6474  e(tmin, tmax, dt
+000160a0: 290a 2020 2020 6e70 7473 203d 206c 656e  ).    npts = len
+000160b0: 2874 7665 6329 0a0a 2020 2020 2320 7065  (tvec)..    # pe
+000160c0: 7266 6f72 6d20 6372 6f73 7320 636f 6865  rform cross cohe
+000160d0: 7265 6e74 2061 6e61 6c79 7369 732c 206d  rent analysis, m
+000160e0: 6f64 6966 6965 6420 6672 6f6d 2066 756e  odified from fun
+000160f0: 6374 696f 6e20 2777 6176 656c 6574 2e63  ction 'wavelet.c
+00016100: 7774 270a 2020 2020 5743 542c 2061 5743  wt'.    WCT, aWC
+00016110: 542c 2063 6f69 2c20 6672 6571 2c20 7369  T, coi, freq, si
+00016120: 6720 3d20 7763 745f 6d6f 6469 6669 6564  g = wct_modified
+00016130: 2872 6566 2c20 6375 722c 2064 742c 2064  (ref, cur, dt, d
+00016140: 6a3d 646a 2c20 7330 3d73 302c 204a 3d4a  j=dj, s0=s0, J=J
+00016150: 2c20 7369 673d 7369 672c 2077 6176 656c  , sig=sig, wavel
+00016160: 6574 3d77 766e 2c20 6e6f 726d 616c 697a  et=wvn, normaliz
+00016170: 653d 5472 7565 290a 0a20 2020 2069 6620  e=True)..    if 
+00016180: 756e 7772 6170 666c 6167 3a0a 2020 2020  unwrapflag:.    
+00016190: 2020 2020 7068 6173 6520 3d20 6e70 2e75      phase = np.u
+000161a0: 6e77 7261 7028 6157 4354 2c20 6178 6973  nwrap(aWCT, axis
+000161b0: 3d2d 3129 2020 2320 6178 6973 3d30 2c20  =-1)  # axis=0, 
+000161c0: 7570 7772 6170 2061 6c6f 6e67 2074 696d  upwrap along tim
+000161d0: 653b 2061 7869 733d 2d31 2c20 756e 7772  e; axis=-1, unwr
+000161e0: 6170 2061 6c6f 6e67 2066 7265 7175 656e  ap along frequen
+000161f0: 6379 0a20 2020 2065 6c73 653a 0a20 2020  cy.    else:.   
+00016200: 2020 2020 2070 6861 7365 203d 2061 5743       phase = aWC
+00016210: 540a 0a20 2020 2023 207a 6572 6f20 6f75  T..    # zero ou
+00016220: 7420 6461 7461 206f 7574 7369 6465 2066  t data outside f
+00016230: 7265 7175 656e 6379 2062 616e 640a 2020  requency band.  
+00016240: 2020 6966 2028 666d 6178 203e 206e 702e    if (fmax > np.
+00016250: 6d61 7828 6672 6571 2929 207c 2028 666d  max(freq)) | (fm
+00016260: 6178 203c 3d20 666d 696e 293a 0a20 2020  ax <= fmin):.   
+00016270: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00016280: 4572 726f 7228 2241 626f 7274 3a20 696e  Error("Abort: in
+00016290: 7075 7420 6672 6571 7565 6e63 7920 6f75  put frequency ou
+000162a0: 7420 6f66 206c 696d 6974 7321 2229 0a20  t of limits!"). 
+000162b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000162c0: 2066 7265 715f 696e 6469 6e20 3d20 6e70   freq_indin = np
+000162d0: 2e77 6865 7265 2828 6672 6571 203e 3d20  .where((freq >= 
+000162e0: 666d 696e 2920 2620 2866 7265 7120 3c3d  fmin) & (freq <=
+000162f0: 2066 6d61 7829 295b 305d 0a0a 2020 2020   fmax))[0]..    
+00016300: 2320 666f 6c6c 6f77 204d 5743 5320 746f  # follow MWCS to
+00016310: 2064 6f20 7477 6f20 7374 6570 7320 6f66   do two steps of
+00016320: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
+00016330: 6f6e 0a20 2020 2069 6620 6e6f 7420 616c  on.    if not al
+00016340: 6c66 7265 713a 0a20 2020 2020 2020 2064  lfreq:.        d
+00016350: 656c 7461 5f74 5f6d 2c20 6465 6c74 615f  elta_t_m, delta_
+00016360: 745f 756e 6320 3d20 6e70 2e7a 6572 6f73  t_unc = np.zeros
+00016370: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
+00016380: 666c 6f61 7433 3229 2c20 6e70 2e7a 6572  float32), np.zer
+00016390: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
+000163a0: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
+000163b0: 2020 2023 2061 7373 756d 6520 7468 6520     # assume the 
+000163c0: 7476 6563 2069 7320 7468 6520 7469 6d65  tvec is the time
+000163d0: 2077 696e 646f 7720 746f 206d 6561 7375   window to measu
+000163e0: 7265 2064 740a 2020 2020 2020 2020 666f  re dt.        fo
+000163f0: 7220 6974 2069 6e20 7261 6e67 6528 6e70  r it in range(np
+00016400: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00016410: 2077 203d 2031 202f 2057 4354 5b66 7265   w = 1 / WCT[fre
+00016420: 715f 696e 6469 6e2c 2069 745d 0a20 2020  q_indin, it].   
+00016430: 2020 2020 2020 2020 2077 5b7e 6e70 2e69           w[~np.i
+00016440: 7366 696e 6974 6528 7729 5d20 3d20 312e  sfinite(w)] = 1.
+00016450: 300a 2020 2020 2020 2020 2020 2020 6465  0.            de
+00016460: 6c74 615f 745f 6d5b 6974 5d2c 2064 656c  lta_t_m[it], del
+00016470: 7461 5f74 5f75 6e63 5b69 745d 203d 206c  ta_t_unc[it] = l
+00016480: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
+00016490: 2866 7265 715b 6672 6571 5f69 6e64 696e  (freq[freq_indin
+000164a0: 5d20 2a20 3220 2a20 6e70 2e70 692c 2070  ] * 2 * np.pi, p
+000164b0: 6861 7365 5b66 7265 715f 696e 6469 6e2c  hase[freq_indin,
+000164c0: 2069 745d 2c20 7729 0a0a 2020 2020 2020   it], w)..      
+000164d0: 2020 2320 6e65 7720 7765 6967 6874 7320    # new weights 
+000164e0: 666f 7220 7265 6772 6573 7369 6f6e 0a20  for regression. 
+000164f0: 2020 2020 2020 2077 3220 3d20 3120 2f20         w2 = 1 / 
+00016500: 6e70 2e6d 6561 6e28 5743 545b 6672 6571  np.mean(WCT[freq
+00016510: 5f69 6e64 696e 2c20 3a5d 2c20 6178 6973  _indin, :], axis
+00016520: 3d30 290a 2020 2020 2020 2020 7732 5b7e  =0).        w2[~
+00016530: 6e70 2e69 7366 696e 6974 6528 7732 295d  np.isfinite(w2)]
+00016540: 203d 2031 2e30 0a0a 2020 2020 2020 2020   = 1.0..        
+00016550: 2320 6e6f 7720 7573 6520 6474 2061 6e64  # now use dt and
+00016560: 2074 2074 6f20 6765 7420 6476 2f76 0a20   t to get dv/v. 
+00016570: 2020 2020 2020 2069 6620 6c65 6e28 7732         if len(w2
+00016580: 2920 3e20 323a 0a20 2020 2020 2020 2020  ) > 2:.         
+00016590: 2020 2069 6620 6e6f 7420 6e70 2e61 6e79     if not np.any
+000165a0: 2864 656c 7461 5f74 5f6d 293a 0a20 2020  (delta_t_m):.   
+000165b0: 2020 2020 2020 2020 2020 2020 2064 7676               dvv
+000165c0: 2c20 6572 7220 3d20 6e70 2e6e 616e 2c20  , err = np.nan, 
+000165d0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+000165e0: 2020 206d 2c20 656d 203d 206c 696e 6561     m, em = linea
+000165f0: 725f 7265 6772 6573 7369 6f6e 2874 7665  r_regression(tve
+00016600: 632c 2064 656c 7461 5f74 5f6d 2c20 7732  c, delta_t_m, w2
+00016610: 2c20 696e 7465 7263 6570 745f 6f72 6967  , intercept_orig
+00016620: 696e 3d54 7275 6529 0a20 2020 2020 2020  in=True).       
+00016630: 2020 2020 2064 7676 2c20 6572 7220 3d20       dvv, err = 
+00016640: 2d6d 2c20 656d 0a20 2020 2020 2020 2065  -m, em.        e
+00016650: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00016660: 206c 6f67 6765 722e 6465 6275 6728 226e   logger.debug("n
+00016670: 6f74 2065 6e6f 7567 6820 706f 696e 7473  ot enough points
+00016680: 2074 6f20 6573 7469 6d61 7465 2064 762f   to estimate dv/
+00016690: 7620 666f 7220 7774 7322 290a 2020 2020  v for wts").    
+000166a0: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
+000166b0: 203d 206e 702e 6e61 6e2c 206e 702e 6e61   = np.nan, np.na
+000166c0: 6e0a 0a20 2020 2020 2020 2072 6574 7572  n..        retur
+000166d0: 6e20 6476 7620 2a20 3130 302c 2065 7272  n dvv * 100, err
+000166e0: 202a 2031 3030 0a0a 2020 2020 2320 636f   * 100..    # co
+000166f0: 6e76 6572 7420 7068 6173 6520 6469 7265  nvert phase dire
+00016700: 6374 6c79 2074 6f20 6465 6c74 615f 7420  ctly to delta_t 
+00016710: 666f 7220 616c 6c20 6672 6571 7565 6e63  for all frequenc
+00016720: 6965 730a 2020 2020 656c 7365 3a0a 2020  ies.    else:.  
+00016730: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
+00016740: 7068 6173 6520 6465 6c61 7920 746f 2074  phase delay to t
+00016750: 696d 6520 6465 6c61 790a 2020 2020 2020  ime delay.      
+00016760: 2020 6465 6c74 615f 7420 3d20 7068 6173    delta_t = phas
+00016770: 6520 2f20 2832 202a 206e 702e 7069 202a  e / (2 * np.pi *
+00016780: 2066 7265 715b 3a2c 204e 6f6e 655d 2920   freq[:, None]) 
+00016790: 2023 206e 6f72 6d61 6c69 7a65 2070 6861   # normalize pha
+000167a0: 7365 2062 7920 2832 2a70 692a 6672 6571  se by (2*pi*freq
+000167b0: 7565 6e63 7929 0a20 2020 2020 2020 2064  uency).        d
+000167c0: 7676 2c20 6572 7220 3d20 6e70 2e7a 6572  vv, err = np.zer
+000167d0: 6f73 2866 7265 715f 696e 6469 6e2e 7368  os(freq_indin.sh
+000167e0: 6170 6529 2c20 6e70 2e7a 6572 6f73 2866  ape), np.zeros(f
+000167f0: 7265 715f 696e 6469 6e2e 7368 6170 6529  req_indin.shape)
+00016800: 0a0a 2020 2020 2020 2020 2320 6c6f 6f70  ..        # loop
+00016810: 2074 6872 6f75 6768 2066 7265 7120 666f   through freq fo
+00016820: 7220 6c69 6e65 6172 2072 6567 7265 7373  r linear regress
+00016830: 696f 6e0a 2020 2020 2020 2020 666f 7220  ion.        for 
+00016840: 6969 2c20 6966 7265 7120 696e 2065 6e75  ii, ifreq in enu
+00016850: 6d65 7261 7465 2866 7265 715f 696e 6469  merate(freq_indi
+00016860: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+00016870: 6966 206c 656e 2874 7665 6329 203e 2032  if len(tvec) > 2
+00016880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016890: 2020 6966 206e 6f74 206e 702e 616e 7928    if not np.any(
+000168a0: 6465 6c74 615f 745b 6966 7265 715d 293a  delta_t[ifreq]):
+000168b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000168c0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000168e0: 2068 6f77 2074 6f20 6265 7474 6572 2061   how to better a
+000168f0: 7070 726f 6163 6820 7468 6520 756e 6365  pproach the unce
+00016900: 7274 6169 6e74 7920 6f66 2064 656c 7461  rtainty of delta
+00016910: 5f74 0a20 2020 2020 2020 2020 2020 2020  _t.             
+00016920: 2020 2077 203d 2031 202f 2057 4354 5b69     w = 1 / WCT[i
+00016930: 6672 6571 5d0a 2020 2020 2020 2020 2020  freq].          
+00016940: 2020 2020 2020 775b 7e6e 702e 6973 6669        w[~np.isfi
+00016950: 6e69 7465 2877 295d 203d 2031 2e30 0a0a  nite(w)] = 1.0..
+00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016970: 2320 6d2c 2061 2c20 656d 2c20 6561 203d  # m, a, em, ea =
+00016980: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
+00016990: 6f6e 2874 696d 655f 6178 6973 5b69 6e64  on(time_axis[ind
+000169a0: 785d 2c20 6465 6c74 615f 745b 696e 6478  x], delta_t[indx
+000169b0: 5d2c 2077 2c20 696e 7465 7263 6570 745f  ], w, intercept_
+000169c0: 6f72 6967 696e 3d46 616c 7365 290a 2020  origin=False).  
+000169d0: 2020 2020 2020 2020 2020 2020 2020 6d2c                m,
+000169e0: 2065 6d20 3d20 6c69 6e65 6172 5f72 6567   em = linear_reg
+000169f0: 7265 7373 696f 6e28 7476 6563 2c20 6465  ression(tvec, de
+00016a00: 6c74 615f 745b 6966 7265 715d 2c20 772c  lta_t[ifreq], w,
+00016a10: 2069 6e74 6572 6365 7074 5f6f 7269 6769   intercept_origi
+00016a20: 6e3d 5472 7565 290a 2020 2020 2020 2020  n=True).        
+00016a30: 2020 2020 2020 2020 6476 765b 6969 5d2c          dvv[ii],
+00016a40: 2065 7272 5b69 695d 203d 202d 6d2c 2065   err[ii] = -m, e
+00016a50: 6d0a 2020 2020 2020 2020 2020 2020 656c  m.            el
+00016a60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016a70: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00016a80: 2822 6e6f 7420 656e 6f75 6768 2070 6f69  ("not enough poi
+00016a90: 6e74 7320 746f 2065 7374 696d 6174 6520  nts to estimate 
+00016aa0: 6476 2f76 2066 6f72 2077 7473 2229 0a20  dv/v for wts"). 
+00016ab0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00016ac0: 7676 5b69 695d 2c20 6572 725b 6969 5d20  vv[ii], err[ii] 
+00016ad0: 3d20 6e70 2e6e 616e 2c20 6e70 2e6e 616e  = np.nan, np.nan
+00016ae0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00016af0: 2066 7265 715b 6672 6571 5f69 6e64 696e   freq[freq_indin
+00016b00: 5d2c 2064 7676 202a 2031 3030 2c20 6572  ], dvv * 100, er
+00016b10: 7220 2a20 3130 300a 0a0a 6465 6620 7774  r * 100...def wt
+00016b20: 735f 6476 7628 0a20 2020 2072 6566 2c0a  s_dvv(.    ref,.
+00016b30: 2020 2020 6375 722c 0a20 2020 2061 6c6c      cur,.    all
+00016b40: 6672 6571 2c0a 2020 2020 7061 7261 2c0a  freq,.    para,.
+00016b50: 2020 2020 6476 5f72 616e 6765 2c0a 2020      dv_range,.  
+00016b60: 2020 6e62 7472 6961 6c2c 0a20 2020 2064    nbtrial,.    d
+00016b70: 6a3d 3120 2f20 3132 2c0a 2020 2020 7330  j=1 / 12,.    s0
+00016b80: 3d2d 312c 0a20 2020 204a 3d2d 312c 0a20  =-1,.    J=-1,. 
+00016b90: 2020 2077 766e 3d22 6d6f 726c 6574 222c     wvn="morlet",
+00016ba0: 0a20 2020 206e 6f72 6d61 6c69 7a65 3d54  .    normalize=T
+00016bb0: 7275 652c 0a29 3a0a 2020 2020 2222 220a  rue,.):.    """.
+00016bc0: 2020 2020 4170 706c 7920 7374 7265 7463      Apply stretc
+00016bd0: 6869 6e67 206d 6574 686f 6420 746f 2063  hing method to c
+00016be0: 6f6e 7469 6e75 6f75 7320 7761 7665 6c65  ontinuous wavele
+00016bf0: 7420 7472 616e 7366 6f72 6d61 7469 6f6e  t transformation
+00016c00: 2028 4357 5429 206f 6620 7369 676e 616c   (CWT) of signal
+00016c10: 730a 2020 2020 666f 7220 616c 6c20 6672  s.    for all fr
+00016c20: 6571 7565 6369 6573 2069 6e20 616e 2069  equecies in an i
+00016c30: 6e74 6572 6573 7420 7261 6e67 650a 0a20  nterest range.. 
+00016c40: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00016c50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00016c60: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
+00016c70: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
+00016c80: 7269 6573 2028 6e75 6d70 792e 6e64 6172  ries (numpy.ndar
+00016c90: 7261 7929 0a20 2020 2063 7572 3a20 5468  ray).    cur: Th
+00016ca0: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
+00016cb0: 7365 7269 6573 2028 6e75 6d70 792e 6e64  series (numpy.nd
+00016cc0: 6172 7261 7929 0a20 2020 2061 6c6c 6672  array).    allfr
+00016cd0: 6571 3a20 6120 626f 6f6c 656e 2076 6172  eq: a boolen var
+00016ce0: 6961 626c 6520 746f 206d 616b 6520 6d65  iable to make me
+00016cf0: 6173 7572 656d 656e 7473 206f 6e20 616c  asurements on al
+00016d00: 6c20 6672 6571 7565 6e63 7920 7261 6e67  l frequency rang
+00016d10: 6520 6f72 206e 6f74 0a20 2020 2070 6172  e or not.    par
+00016d20: 613a 2061 2064 6963 7420 636f 6e74 6169  a: a dict contai
+00016d30: 6e69 6e67 2066 7265 712f 7469 6d65 2069  ning freq/time i
+00016d40: 6e66 6f20 6f66 2074 6865 2064 6174 6120  nfo of the data 
+00016d50: 6d61 7472 6978 0a20 2020 2064 765f 7261  matrix.    dv_ra
+00016d60: 6e67 653a 2061 6273 6f6c 7574 6520 626f  nge: absolute bo
+00016d70: 756e 6420 666f 7220 7468 6520 7665 6c6f  und for the velo
+00016d80: 6369 7479 2076 6172 6961 7469 6f6e 3b20  city variation; 
+00016d90: 6578 616d 706c 653a 2064 763d 302e 3033  example: dv=0.03
+00016da0: 2066 6f72 205b 2d33 2c33 5d25 0a20 2020   for [-3,3]%.   
+00016db0: 206f 6620 7265 6c61 7469 7665 2076 656c   of relative vel
+00016dc0: 6f63 6974 7920 6368 616e 6765 2028 666c  ocity change (fl
+00016dd0: 6f61 7429 0a20 2020 206e 6274 7269 616c  oat).    nbtrial
+00016de0: 3a20 6e75 6d62 6572 206f 6620 7374 7265  : number of stre
+00016df0: 7463 6869 6e67 2063 6f65 6666 6963 6965  tching coefficie
+00016e00: 6e74 2062 6574 7765 656e 2064 766d 696e  nt between dvmin
+00016e10: 2061 6e64 2064 766d 6178 2c20 6e6f 206e   and dvmax, no n
+00016e20: 6565 6420 746f 2062 6520 6869 6768 6572  eed to be higher
+00016e30: 2074 6861 6e20 3130 3020 2028 666c 6f61   than 100  (floa
+00016e40: 7429 0a20 2020 2064 6a2c 2073 302c 204a  t).    dj, s0, J
+00016e50: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
+00016e60: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
+00016e70: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
+00016e80: 6374 270a 2020 2020 6e6f 726d 616c 697a  ct'.    normaliz
+00016e90: 653a 206e 6f72 6d61 6c69 7a65 2074 6865  e: normalize the
+00016ea0: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
+00016eb0: 6d20 6f72 206e 6f74 2e20 4465 6661 756c  m or not. Defaul
+00016ec0: 7420 6973 2054 7275 650a 0a20 2020 2052  t is True..    R
+00016ed0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+00016ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00016ef0: 2020 2064 7676 3a20 6573 7469 6d61 7465     dvv: estimate
+00016f00: 6420 6476 2f76 0a20 2020 2065 7272 3a20  d dv/v.    err: 
+00016f10: 6572 726f 7220 6f66 2064 762f 7620 6573  error of dv/v es
+00016f20: 7469 6d61 7469 6f6e 0a0a 2020 2020 5772  timation..    Wr
+00016f30: 6974 7465 6e20 6279 2043 6f6e 6763 6f6e  itten by Congcon
+00016f40: 6720 5975 616e 2028 3330 204a 756e 2c20  g Yuan (30 Jun, 
+00016f50: 3230 3139 290a 2020 2020 2222 220a 2020  2019).    """.  
+00016f60: 2020 2320 636f 6d6d 6f6e 2076 6172 6961    # common varia
+00016f70: 626c 6573 0a20 2020 2066 7265 7120 3d20  bles.    freq = 
+00016f80: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
+00016f90: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
+00016fa0: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
+00016fb0: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
+00016fc0: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
+00016fd0: 0a0a 2020 2020 2320 6170 706c 7920 6377  ..    # apply cw
+00016fe0: 7420 6f6e 2074 776f 2074 7261 6365 730a  t on two traces.
+00016ff0: 2020 2020 6377 7431 2c20 736a 2c20 6672      cwt1, sj, fr
+00017000: 6571 2c20 636f 692c 205f 2c20 5f20 3d20  eq, coi, _, _ = 
+00017010: 7079 6377 742e 6377 7428 6375 722c 2064  pycwt.cwt(cur, d
+00017020: 742c 2064 6a2c 2073 302c 204a 2c20 7776  t, dj, s0, J, wv
+00017030: 6e29 0a20 2020 2063 7774 322c 2073 6a2c  n).    cwt2, sj,
+00017040: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
+00017050: 203d 2070 7963 7774 2e63 7774 2872 6566   = pycwt.cwt(ref
+00017060: 2c20 6474 2c20 646a 2c20 7330 2c20 4a2c  , dt, dj, s0, J,
+00017070: 2077 766e 290a 0a20 2020 2023 2065 7874   wvn)..    # ext
+00017080: 7261 6374 2072 6561 6c20 7661 6c75 6573  ract real values
+00017090: 206f 6620 6377 740a 2020 2020 7263 7774   of cwt.    rcwt
+000170a0: 312c 2072 6377 7432 203d 206e 702e 7265  1, rcwt2 = np.re
+000170b0: 616c 2863 7774 3129 2c20 6e70 2e72 6561  al(cwt1), np.rea
+000170c0: 6c28 6377 7432 290a 0a20 2020 2023 207a  l(cwt2)..    # z
+000170d0: 6572 6f20 6f75 7420 6461 7461 206f 7574  ero out data out
+000170e0: 7369 6465 2066 7265 7175 656e 6379 2062  side frequency b
+000170f0: 616e 640a 2020 2020 6966 2028 666d 6178  and.    if (fmax
+00017100: 203e 206e 702e 6d61 7828 6672 6571 2929   > np.max(freq))
+00017110: 207c 2028 666d 6178 203c 3d20 666d 696e   | (fmax <= fmin
+00017120: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+00017130: 2056 616c 7565 4572 726f 7228 2241 626f   ValueError("Abo
+00017140: 7274 3a20 696e 7075 7420 6672 6571 7565  rt: input freque
+00017150: 6e63 7920 6f75 7420 6f66 206c 696d 6974  ncy out of limit
+00017160: 7321 2229 0a20 2020 2065 6c73 653a 0a20  s!").    else:. 
+00017170: 2020 2020 2020 2066 7265 715f 696e 6469         freq_indi
+00017180: 6e20 3d20 6e70 2e77 6865 7265 2828 6672  n = np.where((fr
+00017190: 6571 203e 3d20 666d 696e 2920 2620 2866  eq >= fmin) & (f
+000171a0: 7265 7120 3c3d 2066 6d61 7829 295b 305d  req <= fmax))[0]
+000171b0: 0a0a 2020 2020 2320 636f 6e76 6572 7420  ..    # convert 
+000171c0: 7761 7665 6c65 7420 646f 6d61 696e 2062  wavelet domain b
+000171d0: 6163 6b20 746f 2074 696d 6520 646f 6d61  ack to time doma
+000171e0: 696e 2028 7e66 696c 7465 7269 6e67 290a  in (~filtering).
+000171f0: 2020 2020 6966 206e 6f74 2061 6c6c 6672      if not allfr
+00017200: 6571 3a0a 2020 2020 2020 2020 2320 696e  eq:.        # in
+00017210: 7665 7273 6520 6377 7420 746f 2074 696d  verse cwt to tim
+00017220: 6520 646f 6d61 696e 0a20 2020 2020 2020  e domain.       
+00017230: 2069 6377 7431 203d 2070 7963 7774 2e69   icwt1 = pycwt.i
+00017240: 6377 7428 6377 7431 5b66 7265 715f 696e  cwt(cwt1[freq_in
+00017250: 6469 6e5d 2c20 736a 5b66 7265 715f 696e  din], sj[freq_in
+00017260: 6469 6e5d 2c20 6474 2c20 646a 2c20 7776  din], dt, dj, wv
+00017270: 6e29 0a20 2020 2020 2020 2069 6377 7432  n).        icwt2
+00017280: 203d 2070 7963 7774 2e69 6377 7428 6377   = pycwt.icwt(cw
+00017290: 7432 5b66 7265 715f 696e 6469 6e5d 2c20  t2[freq_indin], 
+000172a0: 736a 5b66 7265 715f 696e 6469 6e5d 2c20  sj[freq_indin], 
+000172b0: 6474 2c20 646a 2c20 7776 6e29 0a0a 2020  dt, dj, wvn)..  
+000172c0: 2020 2020 2020 2320 6173 7375 6d65 2061        # assume a
+000172d0: 6c6c 2074 696d 6520 7769 6e64 6f77 2069  ll time window i
+000172e0: 7320 7573 6564 0a20 2020 2020 2020 2077  s used.        w
+000172f0: 6377 7431 2c20 7763 7774 3220 3d20 6e70  cwt1, wcwt2 = np
+00017300: 2e72 6561 6c28 6963 7774 3129 2c20 6e70  .real(icwt1), np
+00017310: 2e72 6561 6c28 6963 7774 3229 0a0a 2020  .real(icwt2)..  
+00017320: 2020 2020 2020 2320 4e6f 726d 616c 697a        # Normaliz
+00017330: 6573 2062 6f74 6820 7369 676e 616c 732c  es both signals,
+00017340: 2069 6620 6170 7072 6f70 7269 6174 652e   if appropriate.
+00017350: 0a20 2020 2020 2020 2069 6620 6e6f 726d  .        if norm
+00017360: 616c 697a 653a 0a20 2020 2020 2020 2020  alize:.         
+00017370: 2020 206e 6377 7431 203d 2028 7763 7774     ncwt1 = (wcwt
+00017380: 3120 2d20 7763 7774 312e 6d65 616e 2829  1 - wcwt1.mean()
+00017390: 2920 2f20 7763 7774 312e 7374 6428 290a  ) / wcwt1.std().
+000173a0: 2020 2020 2020 2020 2020 2020 6e63 7774              ncwt
+000173b0: 3220 3d20 2877 6377 7432 202d 2077 6377  2 = (wcwt2 - wcw
+000173c0: 7432 2e6d 6561 6e28 2929 202f 2077 6377  t2.mean()) / wcw
+000173d0: 7432 2e73 7464 2829 0a20 2020 2020 2020  t2.std().       
+000173e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000173f0: 2020 206e 6377 7431 203d 2077 6377 7431     ncwt1 = wcwt1
+00017400: 0a20 2020 2020 2020 2020 2020 206e 6377  .            ncw
+00017410: 7432 203d 2077 6377 7432 0a0a 2020 2020  t2 = wcwt2..    
+00017420: 2020 2020 2320 7275 6e20 7374 7265 7463      # run stretc
+00017430: 6869 6e67 0a20 2020 2020 2020 2064 7676  hing.        dvv
+00017440: 2c20 6572 722c 2063 632c 2063 6470 203d  , err, cc, cdp =
+00017450: 2073 7472 6574 6368 696e 6728 6e63 7774   stretching(ncwt
+00017460: 322c 206e 6377 7431 2c20 6476 5f72 616e  2, ncwt1, dv_ran
+00017470: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
+00017480: 6129 0a20 2020 2020 2020 2072 6574 7572  a).        retur
+00017490: 6e20 6476 762c 2065 7272 0a0a 2020 2020  n dvv, err..    
+000174a0: 2320 6469 7265 6374 6c79 2074 616b 6520  # directly take 
+000174b0: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
+000174c0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000174d0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
+000174e0: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+000174f0: 206e 6672 6571 203d 206c 656e 2866 7265   nfreq = len(fre
+00017500: 715f 696e 6469 6e29 0a20 2020 2020 2020  q_indin).       
+00017510: 2064 7676 2c20 6363 2c20 6364 702c 2065   dvv, cc, cdp, e
+00017520: 7272 203d 2028 0a20 2020 2020 2020 2020  rr = (.         
+00017530: 2020 206e 702e 7a65 726f 7328 6e66 7265     np.zeros(nfre
+00017540: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
+00017550: 7433 3229 2c0a 2020 2020 2020 2020 2020  t32),.          
+00017560: 2020 6e70 2e7a 6572 6f73 286e 6672 6571    np.zeros(nfreq
+00017570: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00017580: 3332 292c 0a20 2020 2020 2020 2020 2020  32),.           
+00017590: 206e 702e 7a65 726f 7328 6e66 7265 712c   np.zeros(nfreq,
+000175a0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000175b0: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
+000175c0: 6e70 2e7a 6572 6f73 286e 6672 6571 2c20  np.zeros(nfreq, 
+000175d0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000175e0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+000175f0: 2020 2020 2020 2320 6c6f 6f70 2074 6872        # loop thr
+00017600: 6f75 6768 2065 6163 6820 6672 6571 0a20  ough each freq. 
+00017610: 2020 2020 2020 2066 6f72 2069 692c 2069         for ii, i
+00017620: 6672 6571 2069 6e20 656e 756d 6572 6174  freq in enumerat
+00017630: 6528 6672 6571 5f69 6e64 696e 293a 0a20  e(freq_indin):. 
+00017640: 2020 2020 2020 2020 2020 2023 2070 7265             # pre
+00017650: 7061 7265 2077 696e 646f 7765 6420 6461  pare windowed da
+00017660: 7461 0a20 2020 2020 2020 2020 2020 2077  ta.            w
+00017670: 6377 7431 2c20 7763 7774 3220 3d20 7263  cwt1, wcwt2 = rc
+00017680: 7774 315b 6966 7265 715d 2c20 7263 7774  wt1[ifreq], rcwt
+00017690: 325b 6966 7265 715d 0a0a 2020 2020 2020  2[ifreq]..      
+000176a0: 2020 2020 2020 2320 4e6f 726d 616c 697a        # Normaliz
+000176b0: 6573 2062 6f74 6820 7369 676e 616c 732c  es both signals,
+000176c0: 2069 6620 6170 7072 6f70 7269 6174 652e   if appropriate.
+000176d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000176e0: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
+000176f0: 2020 2020 2020 2020 2020 206e 6377 7431             ncwt1
+00017700: 203d 2028 7763 7774 3120 2d20 7763 7774   = (wcwt1 - wcwt
+00017710: 312e 6d65 616e 2829 2920 2f20 7763 7774  1.mean()) / wcwt
+00017720: 312e 7374 6428 290a 2020 2020 2020 2020  1.std().        
+00017730: 2020 2020 2020 2020 6e63 7774 3220 3d20          ncwt2 = 
+00017740: 2877 6377 7432 202d 2077 6377 7432 2e6d  (wcwt2 - wcwt2.m
+00017750: 6561 6e28 2929 202f 2077 6377 7432 2e73  ean()) / wcwt2.s
+00017760: 7464 2829 0a20 2020 2020 2020 2020 2020  td().           
+00017770: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00017780: 2020 2020 2020 206e 6377 7431 203d 2077         ncwt1 = w
+00017790: 6377 7431 0a20 2020 2020 2020 2020 2020  cwt1.           
+000177a0: 2020 2020 206e 6377 7432 203d 2077 6377       ncwt2 = wcw
+000177b0: 7432 0a0a 2020 2020 2020 2020 2020 2020  t2..            
+000177c0: 2320 7275 6e20 7374 7265 7463 6869 6e67  # run stretching
+000177d0: 0a20 2020 2020 2020 2020 2020 2064 762c  .            dv,
+000177e0: 2065 7272 6f72 2c20 6331 2c20 6332 203d   error, c1, c2 =
+000177f0: 2073 7472 6574 6368 696e 6728 6e63 7774   stretching(ncwt
+00017800: 322c 206e 6377 7431 2c20 6476 5f72 616e  2, ncwt1, dv_ran
+00017810: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
+00017820: 6129 0a20 2020 2020 2020 2020 2020 2064  a).            d
+00017830: 7676 5b69 695d 2c20 6363 5b69 695d 2c20  vv[ii], cc[ii], 
+00017840: 6364 705b 6969 5d2c 2065 7272 5b69 695d  cdp[ii], err[ii]
+00017850: 203d 2064 762c 2063 312c 2063 322c 2065   = dv, c1, c2, e
+00017860: 7272 6f72 0a0a 2020 2020 2020 2020 7265  rror..        re
+00017870: 7475 726e 2066 7265 715b 6672 6571 5f69  turn freq[freq_i
+00017880: 6e64 696e 5d2c 2064 7676 2c20 6572 720a  ndin], dvv, err.
+00017890: 0a0a 6465 6620 7774 6474 775f 616c 6c66  ..def wtdtw_allf
+000178a0: 7265 7128 0a20 2020 2072 6566 2c0a 2020  req(.    ref,.  
+000178b0: 2020 6375 722c 0a20 2020 2061 6c6c 6672    cur,.    allfr
+000178c0: 6571 2c0a 2020 2020 7061 7261 2c0a 2020  eq,.    para,.  
+000178d0: 2020 6d61 784c 6167 2c0a 2020 2020 622c    maxLag,.    b,
+000178e0: 0a20 2020 2064 6972 6563 7469 6f6e 2c0a  .    direction,.
+000178f0: 2020 2020 646a 3d31 202f 2031 322c 0a20      dj=1 / 12,. 
+00017900: 2020 2073 303d 2d31 2c0a 2020 2020 4a3d     s0=-1,.    J=
+00017910: 2d31 2c0a 2020 2020 7776 6e3d 226d 6f72  -1,.    wvn="mor
+00017920: 6c65 7422 2c0a 2020 2020 6e6f 726d 616c  let",.    normal
+00017930: 697a 653d 5472 7565 2c0a 293a 0a20 2020  ize=True,.):.   
+00017940: 2022 2222 0a20 2020 2041 7070 6c79 2064   """.    Apply d
+00017950: 796e 616d 6963 2074 696d 6520 7761 7270  ynamic time warp
+00017960: 696e 6720 6d65 7468 6f64 2074 6f20 636f  ing method to co
+00017970: 6e74 696e 756f 7573 2077 6176 656c 6574  ntinuous wavelet
+00017980: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+00017990: 2843 5754 2920 6f66 2073 6967 6e61 6c73  (CWT) of signals
+000179a0: 0a20 2020 2066 6f72 2061 6c6c 2066 7265  .    for all fre
+000179b0: 7175 6563 6965 7320 696e 2061 6e20 696e  quecies in an in
+000179c0: 7465 7265 7374 2072 616e 6765 0a0a 2020  terest range..  
+000179d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000179e0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a   --------------.
+000179f0: 2020 2020 7265 663a 2054 6865 2022 5265      ref: The "Re
+00017a00: 6665 7265 6e63 6522 2074 696d 6573 6572  ference" timeser
+00017a10: 6965 7320 286e 756d 7079 2e6e 6461 7272  ies (numpy.ndarr
+00017a20: 6179 290a 2020 2020 6375 723a 2054 6865  ay).    cur: The
+00017a30: 2022 4375 7272 656e 7422 2074 696d 6573   "Current" times
+00017a40: 6572 6965 7320 286e 756d 7079 2e6e 6461  eries (numpy.nda
+00017a50: 7272 6179 290a 2020 2020 616c 6c66 7265  rray).    allfre
+00017a60: 713a 2061 2062 6f6f 6c65 6e20 7661 7269  q: a boolen vari
+00017a70: 6162 6c65 2074 6f20 6d61 6b65 206d 6561  able to make mea
+00017a80: 7375 7265 6d65 6e74 7320 6f6e 2061 6c6c  surements on all
+00017a90: 2066 7265 7175 656e 6379 2072 616e 6765   frequency range
+00017aa0: 206f 7220 6e6f 740a 2020 2020 6d61 784c   or not.    maxL
+00017ab0: 6167 3a20 6d61 7820 6e75 6d62 6572 206f  ag: max number o
+00017ac0: 6620 706f 696e 7473 2074 6f20 7365 6172  f points to sear
+00017ad0: 6368 2066 6f72 7761 7264 2061 6e64 2062  ch forward and b
+00017ae0: 6163 6b77 6172 642e 0a20 2020 2062 3a20  ackward..    b: 
+00017af0: 622d 7661 6c75 6520 746f 206c 696d 6974  b-value to limit
+00017b00: 2073 7472 6169 6e2c 2077 6869 6368 2069   strain, which i
+00017b10: 7320 746f 206c 696d 6974 2074 6865 206d  s to limit the m
+00017b20: 6178 696d 756d 2076 656c 6f63 6974 7920  aximum velocity 
+00017b30: 7065 7274 7572 6261 7469 6f6e 2e0a 2020  perturbation..  
+00017b40: 2020 5365 6520 6571 7561 7469 6f6e 2031    See equation 1
+00017b50: 3120 696e 2028 4d69 6b65 7365 6c6c 2065  1 in (Mikesell e
+00017b60: 7420 616c 2e20 3230 3135 290a 2020 2020  t al. 2015).    
+00017b70: 6469 7265 6374 696f 6e3a 2064 6972 6563  direction: direc
+00017b80: 7469 6f6e 2074 6f20 6163 6375 6d75 6c61  tion to accumula
+00017b90: 7465 2065 7272 6f72 7320 2831 3d66 6f72  te errors (1=for
+00017ba0: 7761 7264 2c20 2d31 3d62 6163 6b77 6172  ward, -1=backwar
+00017bb0: 6429 0a20 2020 2064 6a2c 2073 302c 204a  d).    dj, s0, J
+00017bc0: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
+00017bd0: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
+00017be0: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
+00017bf0: 6374 270a 2020 2020 6e6f 726d 616c 697a  ct'.    normaliz
+00017c00: 653a 206e 6f72 6d61 6c69 7a65 2074 6865  e: normalize the
+00017c10: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
+00017c20: 6d20 6f72 206e 6f74 2e20 4465 6661 756c  m or not. Defaul
+00017c30: 7420 6973 2054 7275 650a 0a20 2020 2052  t is True..    R
+00017c40: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+00017c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00017c60: 2020 2064 7676 3a20 6573 7469 6d61 7465     dvv: estimate
+00017c70: 6420 6476 2f76 0a20 2020 2065 7272 3a20  d dv/v.    err: 
+00017c80: 6572 726f 7220 6f66 2064 762f 7620 6573  error of dv/v es
+00017c90: 7469 6d61 7469 6f6e 0a0a 2020 2020 5772  timation..    Wr
+00017ca0: 6974 7465 6e20 6279 2043 6f6e 6763 6f6e  itten by Congcon
+00017cb0: 6720 5975 616e 2028 3330 204a 756e 2c20  g Yuan (30 Jun, 
+00017cc0: 3230 3139 290a 2020 2020 2222 220a 2020  2019).    """.  
+00017cd0: 2020 2320 636f 6d6d 6f6e 2076 6172 6961    # common varia
+00017ce0: 626c 6573 0a20 2020 2066 7265 7120 3d20  bles.    freq = 
+00017cf0: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
+00017d00: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
+00017d10: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
+00017d20: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
+00017d30: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
+00017d40: 0a0a 2020 2020 2320 6170 706c 7920 6377  ..    # apply cw
+00017d50: 7420 6f6e 2074 776f 2074 7261 6365 730a  t on two traces.
+00017d60: 2020 2020 6377 7431 2c20 736a 2c20 6672      cwt1, sj, fr
+00017d70: 6571 2c20 636f 692c 205f 2c20 5f20 3d20  eq, coi, _, _ = 
+00017d80: 7079 6377 742e 6377 7428 6375 722c 2064  pycwt.cwt(cur, d
+00017d90: 742c 2064 6a2c 2073 302c 204a 2c20 7776  t, dj, s0, J, wv
+00017da0: 6e29 0a20 2020 2063 7774 322c 2073 6a2c  n).    cwt2, sj,
+00017db0: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
+00017dc0: 203d 2070 7963 7774 2e63 7774 2872 6566   = pycwt.cwt(ref
+00017dd0: 2c20 6474 2c20 646a 2c20 7330 2c20 4a2c  , dt, dj, s0, J,
+00017de0: 2077 766e 290a 0a20 2020 2023 2065 7874   wvn)..    # ext
+00017df0: 7261 6374 2072 6561 6c20 7661 6c75 6573  ract real values
+00017e00: 206f 6620 6377 740a 2020 2020 7263 7774   of cwt.    rcwt
+00017e10: 312c 2072 6377 7432 203d 206e 702e 7265  1, rcwt2 = np.re
+00017e20: 616c 2863 7774 3129 2c20 6e70 2e72 6561  al(cwt1), np.rea
+00017e30: 6c28 6377 7432 290a 0a20 2020 2023 207a  l(cwt2)..    # z
+00017e40: 6572 6f20 6f75 7420 636f 6e65 206f 6620  ero out cone of 
+00017e50: 696e 666c 7565 6e63 6520 616e 6420 6461  influence and da
+00017e60: 7461 206f 7574 7369 6465 2066 7265 7175  ta outside frequ
+00017e70: 656e 6379 2062 616e 640a 2020 2020 6966  ency band.    if
+00017e80: 2028 666d 6178 203e 206e 702e 6d61 7828   (fmax > np.max(
+00017e90: 6672 6571 2929 207c 2028 666d 6178 203c  freq)) | (fmax <
+00017ea0: 3d20 666d 696e 293a 0a20 2020 2020 2020  = fmin):.       
+00017eb0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00017ec0: 7228 2241 626f 7274 3a20 696e 7075 7420  r("Abort: input 
+00017ed0: 6672 6571 7565 6e63 7920 6f75 7420 6f66  frequency out of
+00017ee0: 206c 696d 6974 7321 2229 0a20 2020 2065   limits!").    e
+00017ef0: 6c73 653a 0a20 2020 2020 2020 2066 7265  lse:.        fre
+00017f00: 715f 696e 6469 6e20 3d20 6e70 2e77 6865  q_indin = np.whe
+00017f10: 7265 2828 6672 6571 203e 3d20 666d 696e  re((freq >= fmin
+00017f20: 2920 2620 2866 7265 7120 3c3d 2066 6d61  ) & (freq <= fma
+00017f30: 7829 295b 305d 0a0a 2020 2020 2020 2020  x))[0]..        
+00017f40: 2320 5573 6520 4454 5720 6d65 7468 6f64  # Use DTW method
+00017f50: 2074 6f20 6578 7472 6163 7420 6476 760a   to extract dvv.
+00017f60: 2020 2020 2020 2020 6e66 7265 7120 3d20          nfreq = 
+00017f70: 6c65 6e28 6672 6571 5f69 6e64 696e 290a  len(freq_indin).
+00017f80: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
+00017f90: 203d 206e 702e 7a65 726f 7328 6e66 7265   = np.zeros(nfre
+00017fa0: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
+00017fb0: 7433 3229 2c20 6e70 2e7a 6572 6f73 286e  t32), np.zeros(n
+00017fc0: 6672 6571 2c20 6474 7970 653d 6e70 2e66  freq, dtype=np.f
+00017fd0: 6c6f 6174 3332 290a 0a20 2020 2020 2020  loat32)..       
+00017fe0: 2066 6f72 2069 692c 2069 6672 6571 2069   for ii, ifreq i
+00017ff0: 6e20 656e 756d 6572 6174 6528 6672 6571  n enumerate(freq
+00018000: 5f69 6e64 696e 293a 0a20 2020 2020 2020  _indin):.       
+00018010: 2020 2020 2023 2070 7265 7061 7265 2077       # prepare w
+00018020: 696e 646f 7765 6420 6461 7461 0a20 2020  indowed data.   
+00018030: 2020 2020 2020 2020 2077 6377 7431 2c20           wcwt1, 
+00018040: 7763 7774 3220 3d20 7263 7774 315b 6966  wcwt2 = rcwt1[if
+00018050: 7265 715d 2c20 7263 7774 325b 6966 7265  req], rcwt2[ifre
+00018060: 715d 0a20 2020 2020 2020 2020 2020 2023  q].            #
+00018070: 204e 6f72 6d61 6c69 7a65 7320 626f 7468   Normalizes both
+00018080: 2073 6967 6e61 6c73 2c20 6966 2061 7070   signals, if app
+00018090: 726f 7072 6961 7465 2e0a 2020 2020 2020  ropriate..      
+000180a0: 2020 2020 2020 6966 206e 6f72 6d61 6c69        if normali
+000180b0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+000180c0: 2020 2020 6e63 7774 3120 3d20 2877 6377      ncwt1 = (wcw
+000180d0: 7431 202d 2077 6377 7431 2e6d 6561 6e28  t1 - wcwt1.mean(
+000180e0: 2929 202f 2077 6377 7431 2e73 7464 2829  )) / wcwt1.std()
+000180f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018100: 206e 6377 7432 203d 2028 7763 7774 3220   ncwt2 = (wcwt2 
+00018110: 2d20 7763 7774 322e 6d65 616e 2829 2920  - wcwt2.mean()) 
+00018120: 2f20 7763 7774 322e 7374 6428 290a 2020  / wcwt2.std().  
+00018130: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00018140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018150: 6e63 7774 3120 3d20 7763 7774 310a 2020  ncwt1 = wcwt1.  
+00018160: 2020 2020 2020 2020 2020 2020 2020 6e63                nc
+00018170: 7774 3220 3d20 7763 7774 320a 0a20 2020  wt2 = wcwt2..   
+00018180: 2020 2020 2020 2020 2023 2072 756e 2064           # run d
+00018190: 7477 0a20 2020 2020 2020 2020 2020 2064  tw.            d
+000181a0: 762c 2065 7272 6f72 2c20 6469 7374 203d  v, error, dist =
+000181b0: 2064 7477 5f64 7676 286e 6377 7432 2c20   dtw_dvv(ncwt2, 
+000181c0: 6e63 7774 312c 2070 6172 612c 206d 6178  ncwt1, para, max
+000181d0: 4c61 672c 2062 2c20 6469 7265 6374 696f  Lag, b, directio
+000181e0: 6e29 0a20 2020 2020 2020 2020 2020 2064  n).            d
+000181f0: 7676 5b69 695d 2c20 6572 725b 6969 5d20  vv[ii], err[ii] 
+00018200: 3d20 6476 2c20 6572 726f 720a 0a20 2020  = dv, error..   
+00018210: 2064 656c 2063 7774 312c 2063 7774 322c   del cwt1, cwt2,
+00018220: 2072 6377 7431 2c20 7263 7774 322c 206e   rcwt1, rcwt2, n
+00018230: 6377 7431 2c20 6e63 7774 322c 2077 6377  cwt1, ncwt2, wcw
+00018240: 7431 2c20 7763 7774 322c 2063 6f69 2c20  t1, wcwt2, coi, 
+00018250: 736a 2c20 6469 7374 0a0a 2020 2020 6966  sj, dist..    if
+00018260: 206e 6f74 2061 6c6c 6672 6571 3a0a 2020   not allfreq:.  
+00018270: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
+00018280: 6d65 616e 2864 7676 292c 206e 702e 6d65  mean(dvv), np.me
+00018290: 616e 2865 7272 290a 2020 2020 656c 7365  an(err).    else
+000182a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000182b0: 2066 7265 715b 6672 6571 5f69 6e64 696e   freq[freq_indin
+000182c0: 5d2c 2064 7676 2c20 6572 720a 0a0a 2323  ], dvv, err...##
 000182d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000182e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000182f0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00018300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018310: 204d 4f4e 4954 4f52 494e 4720 5554 494c   MONITORING UTIL
-00018320: 4954 5920 4655 4e43 5449 4f4e 5320 2323  ITY FUNCTIONS ##
-00018330: 2323 2323 2323 2323 2323 2323 230a 2323  #############.##
-00018340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000182f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018300: 2323 2323 2323 2323 2323 230a 2323 2323  ###########.####
+00018310: 2323 2323 2323 2323 2323 2323 204d 4f4e  ############ MON
+00018320: 4954 4f52 494e 4720 5554 494c 4954 5920  ITORING UTILITY 
+00018330: 4655 4e43 5449 4f4e 5320 2323 2323 2323  FUNCTIONS ######
+00018340: 2323 2323 2323 2323 230a 2323 2323 2323  #########.######
 00018350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018370: 2323 2323 2323 2323 2323 230a 0a22 2222  ###########.."""
-00018380: 0a62 656c 6f77 2061 7265 2061 7373 656d  .below are assem
-00018390: 626c 7920 6f66 2074 6865 206d 6f6e 6974  bly of the monit
-000183a0: 6f72 696e 6720 7574 696c 6974 7920 6675  oring utility fu
-000183b0: 6e63 7469 6f6e 7320 6361 6c6c 6564 2062  nctions called b
-000183c0: 7920 6d6f 6e69 746f 7269 6e67 2066 756e  y monitoring fun
-000183d0: 6374 696f 6e73 0a22 2222 0a0a 0a64 6566  ctions."""...def
-000183e0: 2073 6d6f 6f74 6828 782c 2077 696e 646f   smooth(x, windo
-000183f0: 773d 2262 6f78 6361 7222 2c20 6861 6c66  w="boxcar", half
-00018400: 5f77 696e 3d33 293a 0a20 2020 2022 2222  _win=3):.    """
-00018410: 0a20 2020 2070 6572 666f 726d 7320 736d  .    performs sm
-00018420: 6f6f 7468 696e 6720 696e 2069 6e74 6572  oothing in inter
-00018430: 6573 7465 6420 7469 6d65 2077 696e 646f  ested time windo
-00018440: 770a 0a20 2020 2050 6172 616d 6574 6572  w..    Parameter
-00018450: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00018460: 2d2d 2d2d 0a20 2020 2078 3a20 7469 6d65  ----.    x: time
-00018470: 7365 7269 7320 6461 7461 0a20 2020 2077  seris data.    w
-00018480: 696e 646f 773a 2074 7970 6573 206f 6620  indow: types of 
-00018490: 7769 6e64 6f77 2074 6f20 646f 2073 6d6f  window to do smo
-000184a0: 6f74 6869 6e67 0a20 2020 2068 616c 665f  othing.    half_
-000184b0: 7769 6e3a 2068 616c 6620 7769 6e64 6f77  win: half window
-000184c0: 206c 656e 6774 680a 0a20 2020 2052 4554   length..    RET
-000184d0: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
-000184e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-000184f0: 2079 3a20 736d 6f6f 7468 6564 2074 696d   y: smoothed tim
-00018500: 6520 7769 6e64 6f77 0a20 2020 2022 2222  e window.    """
-00018510: 0a20 2020 2023 2054 4f44 4f3a 2064 6f63  .    # TODO: doc
-00018520: 7374 696e 670a 2020 2020 7769 6e64 6f77  sting.    window
-00018530: 5f6c 656e 203d 2032 202a 2068 616c 665f  _len = 2 * half_
-00018540: 7769 6e20 2b20 310a 2020 2020 2320 6578  win + 1.    # ex
-00018550: 7465 6e64 696e 6720 7468 6520 6461 7461  tending the data
-00018560: 2061 7420 6265 6769 6e6e 696e 6720 616e   at beginning an
-00018570: 6420 6174 2074 6865 2065 6e64 0a20 2020  d at the end.   
-00018580: 2023 2074 6f20 6170 706c 7920 7468 6520   # to apply the 
-00018590: 7769 6e64 6f77 2061 7420 7468 6520 626f  window at the bo
-000185a0: 7264 6572 730a 2020 2020 7320 3d20 6e70  rders.    s = np
-000185b0: 2e72 5f5b 785b 7769 6e64 6f77 5f6c 656e  .r_[x[window_len
-000185c0: 202d 2031 203a 2030 203a 202d 315d 2c20   - 1 : 0 : -1], 
-000185d0: 782c 2078 5b2d 313a 2d77 696e 646f 775f  x, x[-1:-window_
-000185e0: 6c65 6e3a 2d31 5d5d 0a20 2020 2069 6620  len:-1]].    if 
-000185f0: 7769 6e64 6f77 203d 3d20 2262 6f78 6361  window == "boxca
-00018600: 7222 3a0a 2020 2020 2020 2020 7720 3d20  r":.        w = 
-00018610: 7363 6970 792e 7369 676e 616c 2e62 6f78  scipy.signal.box
-00018620: 6361 7228 7769 6e64 6f77 5f6c 656e 292e  car(window_len).
-00018630: 6173 7479 7065 2822 636f 6d70 6c65 7822  astype("complex"
-00018640: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00018650: 2020 2020 7720 3d20 7363 6970 792e 7369      w = scipy.si
-00018660: 676e 616c 2e68 616e 6e69 6e67 2877 696e  gnal.hanning(win
-00018670: 646f 775f 6c65 6e29 2e61 7374 7970 6528  dow_len).astype(
-00018680: 2263 6f6d 706c 6578 2229 0a20 2020 2079  "complex").    y
-00018690: 203d 206e 702e 636f 6e76 6f6c 7665 2877   = np.convolve(w
-000186a0: 202f 2077 2e73 756d 2829 2c20 732c 206d   / w.sum(), s, m
-000186b0: 6f64 653d 2276 616c 6964 2229 0a20 2020  ode="valid").   
-000186c0: 2072 6574 7572 6e20 795b 6861 6c66 5f77   return y[half_w
-000186d0: 696e 203a 206c 656e 2879 2920 2d20 6861  in : len(y) - ha
-000186e0: 6c66 5f77 696e 5d0a 0a0a 6465 6620 6e65  lf_win]...def ne
-000186f0: 7874 706f 7732 2878 293a 0a20 2020 2022  xtpow2(x):.    "
-00018700: 2222 0a20 2020 2052 6574 7572 6e73 2074  "".    Returns t
-00018710: 6865 206e 6578 7420 706f 7765 7220 6f66  he next power of
-00018720: 2032 206f 6620 782e 0a20 2020 2022 2222   2 of x..    """
-00018730: 0a20 2020 2072 6574 7572 6e20 696e 7428  .    return int(
-00018740: 6e70 2e63 6569 6c28 6e70 2e6c 6f67 3228  np.ceil(np.log2(
-00018750: 6e70 2e61 6273 2878 2929 2929 0a0a 0a64  np.abs(x))))...d
-00018760: 6566 2067 6574 436f 6865 7265 6e63 6528  ef getCoherence(
-00018770: 6463 732c 2064 7331 2c20 6473 3229 3a0a  dcs, ds1, ds2):.
-00018780: 2020 2020 2222 220a 2020 2020 6765 7420      """.    get 
-00018790: 6372 6f73 7320 636f 6865 7265 6e63 6520  cross coherence 
-000187a0: 6265 7477 6565 6e20 7265 6665 7265 6e63  between referenc
-000187b0: 6520 616e 6420 6375 7272 656e 7420 7761  e and current wa
-000187c0: 7665 666f 726d 7320 666f 6c6c 6f77 696e  veforms followin
-000187d0: 6720 6571 7561 7469 6f6e 206f 6620 4133  g equation of A3
-000187e0: 2069 6e20 436c 6172 6b20 6574 2061 6c2e   in Clark et al.
-000187f0: 2c20 3230 3131 0a0a 2020 2020 5061 7261  , 2011..    Para
-00018800: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00018810: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6463  ---------.    dc
-00018820: 733a 2061 6d70 6c69 7475 6465 206f 6620  s: amplitude of 
-00018830: 7468 6520 6372 6f73 7320 7370 6563 7472  the cross spectr
-00018840: 756d 0a20 2020 2064 7331 3a20 616d 706c  um.    ds1: ampl
-00018850: 6974 7564 6520 6f66 2074 6865 2073 7065  itude of the spe
-00018860: 6374 7275 6d20 6f66 2063 7572 7265 6e74  ctrum of current
-00018870: 2077 6176 6566 6f72 6d0a 2020 2020 6473   waveform.    ds
-00018880: 323a 2061 6d70 6c69 7475 6465 206f 6620  2: amplitude of 
-00018890: 7468 6520 7370 6563 7472 756d 206f 6620  the spectrum of 
-000188a0: 7265 6665 7265 6e63 6520 7761 7665 666f  reference wavefo
-000188b0: 726d 0a0a 2020 2020 5245 5455 524e 533a  rm..    RETURNS:
-000188c0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-000188d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 636f 683a  -------.    coh:
-000188e0: 2063 6f68 7265 7265 6e63 7920 6d61 7472   cohrerency matr
-000188f0: 6978 2075 7365 6420 666f 7220 6573 7469  ix used for esti
-00018900: 6d61 7465 2074 6865 2072 6f62 7573 746e  mate the robustn
-00018910: 6573 7320 6f66 2074 6865 2063 726f 7373  ess of the cross
-00018920: 2073 7065 6374 7275 6d0a 2020 2020 2222   spectrum.    ""
-00018930: 220a 2020 2020 6e20 3d20 6c65 6e28 6463  ".    n = len(dc
-00018940: 7329 0a20 2020 2063 6f68 203d 206e 702e  s).    coh = np.
-00018950: 7a65 726f 7328 6e29 2e61 7374 7970 6528  zeros(n).astype(
-00018960: 2263 6f6d 706c 6578 2229 0a20 2020 2076  "complex").    v
-00018970: 616c 6964 7320 3d20 6e70 2e61 7267 7768  alids = np.argwh
-00018980: 6572 6528 6e70 2e6c 6f67 6963 616c 5f61  ere(np.logical_a
-00018990: 6e64 286e 702e 6162 7328 6473 3129 203e  nd(np.abs(ds1) >
-000189a0: 2030 2c20 6e70 2e61 6273 2864 7332 2920   0, np.abs(ds2) 
-000189b0: 3e20 3029 290a 2020 2020 636f 685b 7661  > 0)).    coh[va
-000189c0: 6c69 6473 5d20 3d20 6463 735b 7661 6c69  lids] = dcs[vali
-000189d0: 6473 5d20 2f20 2864 7331 5b76 616c 6964  ds] / (ds1[valid
-000189e0: 735d 202a 2064 7332 5b76 616c 6964 735d  s] * ds2[valids]
-000189f0: 290a 2020 2020 636f 685b 636f 6820 3e20  ).    coh[coh > 
-00018a00: 2831 2e30 202b 2030 6a29 5d20 3d20 312e  (1.0 + 0j)] = 1.
-00018a10: 3020 2b20 306a 0a20 2020 2072 6574 7572  0 + 0j.    retur
-00018a20: 6e20 636f 680a 0a0a 6465 6620 636f 6d70  n coh...def comp
-00018a30: 7574 6545 7272 6f72 4675 6e63 7469 6f6e  uteErrorFunction
-00018a40: 2875 312c 2075 302c 206e 5361 6d70 6c65  (u1, u0, nSample
-00018a50: 2c20 6c61 672c 206e 6f72 6d3d 224c 3222  , lag, norm="L2"
-00018a60: 293a 0a20 2020 2022 2222 0a20 2020 2063  ):.    """.    c
-00018a70: 6f6d 7075 7465 2045 7272 6f72 2046 756e  ompute Error Fun
-00018a80: 6374 696f 6e20 7573 6564 2069 6e20 4454  ction used in DT
-00018a90: 572e 2054 6865 2065 7272 6f72 2066 756e  W. The error fun
-00018aa0: 6374 696f 6e20 6973 2065 7175 6174 696f  ction is equatio
-00018ab0: 6e20 3120 696e 2048 616c 652c 2032 3031  n 1 in Hale, 201
-00018ac0: 332e 2059 6f75 2063 6f75 6c64 2075 6e63  3. You could unc
-00018ad0: 6f6d 6d65 6e74 2074 6865 0a20 2020 204c  omment the.    L
-00018ae0: 3120 6e6f 726d 2061 6e64 2063 6f6d 6d65  1 norm and comme
-00018af0: 6e74 2074 6865 204c 3220 6e6f 726d 2069  nt the L2 norm i
-00018b00: 6620 796f 7520 7761 6e74 206f 6e20 4c69  f you want on Li
-00018b10: 6e65 2032 390a 0a20 2020 2050 6172 616d  ne 29..    Param
-00018b20: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00018b30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2075 313a  --------.    u1:
-00018b40: 2020 7472 6163 6520 7468 6174 2077 6520    trace that we 
-00018b50: 7761 6e74 2074 6f20 7761 7270 3b20 7369  want to warp; si
-00018b60: 7a65 203d 2028 6e73 616d 702c 3129 0a20  ze = (nsamp,1). 
-00018b70: 2020 2075 303a 2020 7265 6665 7265 6e63     u0:  referenc
-00018b80: 6520 7472 6163 6520 746f 2063 6f6d 7061  e trace to compa
-00018b90: 7265 2077 6974 683a 2073 697a 6520 3d20  re with: size = 
-00018ba0: 286e 7361 6d70 2c31 290a 2020 2020 6e53  (nsamp,1).    nS
-00018bb0: 616d 706c 653a 206e 756d 6572 206f 6620  ample: numer of 
-00018bc0: 706f 696e 7473 2074 6f20 636f 6d70 6172  points to compar
-00018bd0: 6520 696e 2074 6865 2074 7261 6365 730a  e in the traces.
-00018be0: 2020 2020 6c61 673a 206d 6178 696d 756d      lag: maximum
-00018bf0: 206c 6167 2069 6e20 7361 6d70 6c65 206e   lag in sample n
-00018c00: 756d 6265 7220 746f 2073 6561 7263 680a  umber to search.
-00018c10: 2020 2020 6e6f 726d 3a20 274c 3227 206f      norm: 'L2' o
-00018c20: 7220 274c 3127 2028 6465 6661 756c 7420  r 'L1' (default 
-00018c30: 6973 2027 4c32 2729 0a0a 2020 2020 5245  is 'L2')..    RE
-00018c40: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-00018c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00018c60: 2020 6572 723a 2074 6865 2032 4420 6572    err: the 2D er
-00018c70: 726f 7220 6675 6e63 7469 6f6e 3b20 7369  ror function; si
-00018c80: 7a65 203d 2028 6e73 616d 702c 322a 6c61  ze = (nsamp,2*la
-00018c90: 672b 3129 0a0a 2020 2020 4f72 6967 696e  g+1)..    Origin
-00018ca0: 616c 2062 7920 4469 2059 616e 670a 2020  al by Di Yang.  
-00018cb0: 2020 4c61 7374 206d 6f64 6966 6965 6420    Last modified 
-00018cc0: 6279 2044 796c 616e 204d 696b 6573 656c  by Dylan Mikesel
-00018cd0: 6c20 2832 3520 4665 622e 2032 3031 3529  l (25 Feb. 2015)
-00018ce0: 0a20 2020 2054 7261 6e73 6c61 7465 6420  .    Translated 
-00018cf0: 746f 2070 7974 686f 6e20 6279 2054 696d  to python by Tim
-00018d00: 2043 6c65 6d65 6e74 7320 2831 3720 4175   Clements (17 Au
-00018d10: 672e 2032 3031 3829 0a0a 2020 2020 2222  g. 2018)..    ""
-00018d20: 220a 0a20 2020 2069 6620 6c61 6720 3e3d  "..    if lag >=
-00018d30: 206e 5361 6d70 6c65 3a0a 2020 2020 2020   nSample:.      
-00018d40: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00018d50: 6f72 2822 636f 6d70 7574 6545 7272 6f72  or("computeError
-00018d60: 4675 6e63 7469 6f6e 3a6c 6167 5072 6f62  Function:lagProb
-00018d70: 6c65 6d22 2c20 226c 6167 206d 7573 7420  lem", "lag must 
-00018d80: 6265 2073 6d61 6c6c 6572 2074 6861 6e20  be smaller than 
-00018d90: 6e53 616d 706c 6522 290a 0a20 2020 2023  nSample")..    #
-00018da0: 2041 6c6c 6f63 6174 6520 6572 726f 7220   Allocate error 
-00018db0: 6675 6e63 7469 6f6e 2076 6172 6961 626c  function variabl
-00018dc0: 650a 2020 2020 6572 7220 3d20 6e70 2e7a  e.    err = np.z
-00018dd0: 6572 6f73 285b 6e53 616d 706c 652c 2032  eros([nSample, 2
-00018de0: 202a 206c 6167 202b 2031 5d29 0a0a 2020   * lag + 1])..  
-00018df0: 2020 2320 696e 6974 6961 6c20 6572 726f    # initial erro
-00018e00: 7220 6361 6c63 756c 6174 696f 6e0a 2020  r calculation.  
-00018e10: 2020 2320 6c6f 6f70 206f 7665 7220 6c61    # loop over la
-00018e20: 6773 0a20 2020 2066 6f72 206c 6c20 696e  gs.    for ll in
-00018e30: 206e 702e 6172 616e 6765 282d 6c61 672c   np.arange(-lag,
-00018e40: 206c 6167 202b 2031 293a 0a20 2020 2020   lag + 1):.     
-00018e50: 2020 2074 6869 734c 6167 203d 206c 6c20     thisLag = ll 
-00018e60: 2b20 6c61 670a 0a20 2020 2020 2020 2023  + lag..        #
-00018e70: 206c 6f6f 7020 6f76 6572 2073 616d 706c   loop over sampl
-00018e80: 6573 0a20 2020 2020 2020 2066 6f72 2069  es.        for i
-00018e90: 6920 696e 2072 616e 6765 286e 5361 6d70  i in range(nSamp
-00018ea0: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
-00018eb0: 2023 2073 6b69 7020 636f 726e 6572 7320   # skip corners 
-00018ec0: 666f 7220 6e6f 772c 2077 6520 7769 6c6c  for now, we will
-00018ed0: 2063 6f6d 6520 6261 636b 2074 6f20 7468   come back to th
-00018ee0: 6573 650a 2020 2020 2020 2020 2020 2020  ese.            
-00018ef0: 6966 2028 6969 202b 206c 6c20 3e3d 2030  if (ii + ll >= 0
-00018f00: 2920 2620 2869 6920 2b20 6c6c 203c 206e  ) & (ii + ll < n
-00018f10: 5361 6d70 6c65 293a 0a20 2020 2020 2020  Sample):.       
-00018f20: 2020 2020 2020 2020 2065 7272 5b69 692c           err[ii,
-00018f30: 2074 6869 734c 6167 5d20 3d20 7531 5b69   thisLag] = u1[i
-00018f40: 695d 202d 2075 305b 6969 202b 206c 6c5d  i] - u0[ii + ll]
-00018f50: 0a0a 2020 2020 6966 206e 6f72 6d20 3d3d  ..    if norm ==
-00018f60: 2022 4c32 223a 0a20 2020 2020 2020 2065   "L2":.        e
-00018f70: 7272 203d 2065 7272 2a2a 320a 2020 2020  rr = err**2.    
-00018f80: 656c 6966 206e 6f72 6d20 3d3d 2022 4c31  elif norm == "L1
-00018f90: 223a 0a20 2020 2020 2020 2065 7272 203d  ":.        err =
-00018fa0: 206e 702e 6162 7328 6572 7229 0a0a 2020   np.abs(err)..  
-00018fb0: 2020 2320 4e6f 7720 6669 7820 636f 726e    # Now fix corn
-00018fc0: 6572 7320 7769 7468 2063 6f6e 7374 616e  ers with constan
-00018fd0: 7420 6578 7472 6170 6f6c 6174 696f 6e0a  t extrapolation.
-00018fe0: 2020 2020 666f 7220 6c6c 2069 6e20 6e70      for ll in np
-00018ff0: 2e61 7261 6e67 6528 2d6c 6167 2c20 6c61  .arange(-lag, la
-00019000: 6720 2b20 3129 3a0a 2020 2020 2020 2020  g + 1):.        
-00019010: 7468 6973 4c61 6720 3d20 6c6c 202b 206c  thisLag = ll + l
-00019020: 6167 0a0a 2020 2020 2020 2020 666f 7220  ag..        for 
-00019030: 6969 2069 6e20 7261 6e67 6528 6e53 616d  ii in range(nSam
-00019040: 706c 6529 3a0a 2020 2020 2020 2020 2020  ple):.          
-00019050: 2020 6966 2069 6920 2b20 6c6c 203c 2030    if ii + ll < 0
-00019060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019070: 2020 6572 725b 6969 2c20 7468 6973 4c61    err[ii, thisLa
-00019080: 675d 203d 2065 7272 5b2d 6c6c 2c20 7468  g] = err[-ll, th
-00019090: 6973 4c61 675d 0a0a 2020 2020 2020 2020  isLag]..        
-000190a0: 2020 2020 656c 6966 2069 6920 2b20 6c6c      elif ii + ll
-000190b0: 203e 206e 5361 6d70 6c65 202d 2031 3a0a   > nSample - 1:.
-000190c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190d0: 6572 725b 6969 2c20 7468 6973 4c61 675d  err[ii, thisLag]
-000190e0: 203d 2065 7272 5b6e 5361 6d70 6c65 202d   = err[nSample -
-000190f0: 206c 6c20 2d20 312c 2074 6869 734c 6167   ll - 1, thisLag
-00019100: 5d0a 0a20 2020 2072 6574 7572 6e20 6572  ]..    return er
-00019110: 720a 0a0a 6465 6620 6163 6375 6d75 6c61  r...def accumula
-00019120: 7465 4572 726f 7246 756e 6374 696f 6e28  teErrorFunction(
-00019130: 6469 722c 2065 7272 2c20 6e53 616d 706c  dir, err, nSampl
-00019140: 652c 206c 6167 2c20 6229 3a0a 2020 2020  e, lag, b):.    
-00019150: 2222 220a 2020 2020 6163 6375 6d75 6c61  """.    accumula
-00019160: 7469 6f6e 206f 6620 7468 6520 6572 726f  tion of the erro
-00019170: 722c 2077 6869 6368 2066 6f6c 6c6f 7773  r, which follows
-00019180: 2074 6865 2065 7175 6174 696f 6e20 3620   the equation 6 
-00019190: 696e 2048 616c 652c 2032 3031 332e 0a0a  in Hale, 2013...
-000191a0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000191b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-000191c0: 2d0a 2020 2020 6469 723a 2061 6363 756d  -.    dir: accum
-000191d0: 756c 6174 696f 6e20 6469 7265 6374 696f  ulation directio
-000191e0: 6e20 2820 6469 7220 3e20 3020 3d20 666f  n ( dir > 0 = fo
-000191f0: 7277 6172 6420 696e 2074 696d 652c 2064  rward in time, d
-00019200: 6972 203c 3d20 3020 3d20 6261 636b 7761  ir <= 0 = backwa
-00019210: 7264 2069 6e20 7469 6d65 290a 2020 2020  rd in time).    
-00019220: 6572 723a 2074 6865 2032 4420 6572 726f  err: the 2D erro
-00019230: 7220 6675 6e63 7469 6f6e 3b20 7369 7a65  r function; size
-00019240: 203d 2028 6e73 616d 702c 322a 6c61 672b   = (nsamp,2*lag+
-00019250: 3129 0a20 2020 206e 5361 6d70 6c65 3a20  1).    nSample: 
-00019260: 6e75 6d65 7220 6f66 2070 6f69 6e74 7320  numer of points 
-00019270: 746f 2063 6f6d 7061 7265 2069 6e20 7468  to compare in th
-00019280: 6520 7472 6163 6573 0a20 2020 206c 6167  e traces.    lag
-00019290: 3a20 6d61 7869 6d75 6d20 6c61 6720 696e  : maximum lag in
-000192a0: 2073 616d 706c 6520 6e75 6d62 6572 2074   sample number t
-000192b0: 6f20 7365 6172 6368 0a20 2020 2062 3a20  o search.    b: 
-000192c0: 7374 7261 696e 206c 696d 6974 2028 696e  strain limit (in
-000192d0: 7465 6765 7220 7661 6c75 6520 3e3d 2031  teger value >= 1
-000192e0: 290a 0a20 2020 2052 4554 5552 4e53 3a0a  )..    RETURNS:.
-000192f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00019300: 2d2d 2d2d 2d2d 0a20 2020 2064 3a20 7468  ------.    d: th
-00019310: 6520 3244 2064 6973 7461 6e63 6520 6675  e 2D distance fu
-00019320: 6e63 7469 6f6e 3b20 7369 7a65 203d 2028  nction; size = (
-00019330: 6e73 616d 702c 322a 6c61 672b 3129 0a0a  nsamp,2*lag+1)..
-00019340: 2020 2020 4f72 6967 696e 616c 2062 7920      Original by 
-00019350: 4469 2059 616e 670a 2020 2020 4c61 7374  Di Yang.    Last
-00019360: 206d 6f64 6966 6965 6420 6279 2044 796c   modified by Dyl
-00019370: 616e 204d 696b 6573 656c 6c20 2832 3520  an Mikesell (25 
-00019380: 4665 622e 2032 3031 3529 0a20 2020 2054  Feb. 2015).    T
-00019390: 7261 6e73 6c61 7465 6420 746f 2070 7974  ranslated to pyt
-000193a0: 686f 6e20 6279 2054 696d 2043 6c65 6d65  hon by Tim Cleme
-000193b0: 6e74 7320 2831 3720 4175 672e 2032 3031  nts (17 Aug. 201
-000193c0: 3829 0a0a 2020 2020 2222 220a 0a20 2020  8)..    """..   
-000193d0: 2023 206e 756d 6265 7220 6f66 206c 6167   # number of lag
-000193e0: 7320 6672 6f6d 205b 202d 6c61 6720 3a20  s from [ -lag : 
-000193f0: 2b6c 6167 205d 0a20 2020 206e 4c61 6720  +lag ].    nLag 
-00019400: 3d20 2832 202a 206c 6167 2920 2b20 310a  = (2 * lag) + 1.
-00019410: 0a20 2020 2023 2061 6c6c 6f63 6174 6520  .    # allocate 
-00019420: 6469 7374 616e 6365 206d 6174 7269 780a  distance matrix.
-00019430: 2020 2020 6420 3d20 6e70 2e7a 6572 6f73      d = np.zeros
-00019440: 285b 6e53 616d 706c 652c 206e 4c61 675d  ([nSample, nLag]
-00019450: 290a 0a20 2020 2023 2053 6574 7570 2069  )..    # Setup i
-00019460: 6e64 6963 6573 2062 6173 6564 206f 6e20  ndices based on 
-00019470: 666f 7277 6172 6420 6f72 2062 6163 6b77  forward or backw
-00019480: 6172 6420 6163 6375 6d75 6c61 7469 6f6e  ard accumulation
-00019490: 2064 6972 6563 7469 6f6e 0a20 2020 2069   direction.    i
-000194a0: 6620 6469 7220 3e20 303a 2020 2320 464f  f dir > 0:  # FO
-000194b0: 5257 4152 440a 2020 2020 2020 2020 6942  RWARD.        iB
-000194c0: 6567 696e 2c20 6945 6e64 2c20 6949 6e63  egin, iEnd, iInc
-000194d0: 203d 2030 2c20 6e53 616d 706c 6520 2d20   = 0, nSample - 
-000194e0: 312c 2031 0a20 2020 2065 6c73 653a 2020  1, 1.    else:  
-000194f0: 2320 4241 434b 5741 5244 0a20 2020 2020  # BACKWARD.     
-00019500: 2020 2069 4265 6769 6e2c 2069 456e 642c     iBegin, iEnd,
-00019510: 2069 496e 6320 3d20 6e53 616d 706c 6520   iInc = nSample 
-00019520: 2d20 312c 2030 2c20 2d31 0a0a 2020 2020  - 1, 0, -1..    
-00019530: 2320 4c6f 6f70 2074 6872 6f75 6768 2061  # Loop through a
-00019540: 6c6c 2074 696d 6573 2069 6920 696e 2066  ll times ii in f
-00019550: 6f72 7761 7264 206f 7220 6261 636b 7761  orward or backwa
-00019560: 7264 2064 6972 6563 7469 6f6e 0a20 2020  rd direction.   
-00019570: 2066 6f72 2069 6920 696e 2072 616e 6765   for ii in range
-00019580: 2869 4265 6769 6e2c 2069 456e 6420 2b20  (iBegin, iEnd + 
-00019590: 6949 6e63 2c20 6949 6e63 293a 0a20 2020  iInc, iInc):.   
-000195a0: 2020 2020 2023 206d 696e 2f6d 6178 2074       # min/max t
-000195b0: 6f20 6163 636f 756e 7420 666f 7220 7468  o account for th
-000195c0: 6520 6564 6765 732f 626f 756e 6461 7269  e edges/boundari
-000195d0: 6573 0a20 2020 2020 2020 206a 6920 3d20  es.        ji = 
-000195e0: 6d61 7828 5b30 2c20 6d69 6e28 5b6e 5361  max([0, min([nSa
-000195f0: 6d70 6c65 202d 2031 2c20 6969 202d 2069  mple - 1, ii - i
-00019600: 496e 635d 295d 290a 2020 2020 2020 2020  Inc])]).        
-00019610: 6a62 203d 206d 6178 285b 302c 206d 696e  jb = max([0, min
-00019620: 285b 6e53 616d 706c 6520 2d20 312c 2069  ([nSample - 1, i
-00019630: 6920 2d20 6949 6e63 202a 2062 5d29 5d29  i - iInc * b])])
-00019640: 0a0a 2020 2020 2020 2020 2320 6c6f 6f70  ..        # loop
-00019650: 2074 6872 6f75 6768 2061 6c6c 206c 6167   through all lag
-00019660: 0a20 2020 2020 2020 2066 6f72 206c 6c20  .        for ll 
-00019670: 696e 2072 616e 6765 286e 4c61 6729 3a0a  in range(nLag):.
-00019680: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
-00019690: 6563 6b20 6c69 6d69 7473 206f 6e20 6c61  eck limits on la
-000196a0: 6720 696e 6469 6365 730a 2020 2020 2020  g indices.      
-000196b0: 2020 2020 2020 6c4d 696e 7573 3120 3d20        lMinus1 = 
-000196c0: 6c6c 202d 2031 0a0a 2020 2020 2020 2020  ll - 1..        
-000196d0: 2020 2020 2320 6368 6563 6b20 6c61 6720      # check lag 
-000196e0: 696e 6465 7820 6973 2067 7265 6174 6572  index is greater
-000196f0: 2074 6861 6e20 300a 2020 2020 2020 2020   than 0.        
-00019700: 2020 2020 6966 206c 4d69 6e75 7331 203c      if lMinus1 <
-00019710: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00019720: 2020 2020 6c4d 696e 7573 3120 3d20 3020      lMinus1 = 0 
-00019730: 2023 206d 616b 6520 6c61 6720 3d20 6669   # make lag = fi
-00019740: 7273 7420 6c61 670a 0a20 2020 2020 2020  rst lag..       
-00019750: 2020 2020 206c 506c 7573 3120 3d20 6c6c       lPlus1 = ll
-00019760: 202b 2031 2020 2320 6c61 6720 6174 206c   + 1  # lag at l
-00019770: 2b31 0a0a 2020 2020 2020 2020 2020 2020  +1..            
-00019780: 2320 6368 6563 6b20 6c61 6720 696e 6465  # check lag inde
-00019790: 7820 6c65 7373 2074 6861 6e20 6d61 7820  x less than max 
-000197a0: 6c61 670a 2020 2020 2020 2020 2020 2020  lag.            
-000197b0: 6966 206c 506c 7573 3120 3e20 6e4c 6167  if lPlus1 > nLag
-000197c0: 202d 2031 3a0a 2020 2020 2020 2020 2020   - 1:.          
-000197d0: 2020 2020 2020 6c50 6c75 7331 203d 206e        lPlus1 = n
-000197e0: 4c61 6720 2d20 310a 0a20 2020 2020 2020  Lag - 1..       
-000197f0: 2020 2020 2023 2067 6574 2064 6973 7461       # get dista
-00019800: 6e63 6520 6174 206c 6167 7320 286c 6c2d  nce at lags (ll-
-00019810: 312c 206c 6c2c 206c 6c2b 3129 0a20 2020  1, ll, ll+1).   
-00019820: 2020 2020 2020 2020 2064 6973 744c 6d69           distLmi
-00019830: 6e75 7331 203d 2064 5b6a 622c 206c 4d69  nus1 = d[jb, lMi
-00019840: 6e75 7331 5d20 2023 206d 696e 7573 3a20  nus1]  # minus: 
-00019850: 2064 5b69 2d62 2c20 6a2d 315d 0a20 2020   d[i-b, j-1].   
-00019860: 2020 2020 2020 2020 2064 6973 744c 203d           distL =
-00019870: 2064 5b6a 692c 206c 6c5d 2020 2320 6163   d[ji, ll]  # ac
-00019880: 7475 616c 2064 5b69 2d31 2c20 6a5d 0a20  tual d[i-1, j]. 
-00019890: 2020 2020 2020 2020 2020 2064 6973 744c             distL
-000198a0: 706c 7573 3120 3d20 645b 6a62 2c20 6c50  plus1 = d[jb, lP
-000198b0: 6c75 7331 5d20 2023 2070 6c75 7320 645b  lus1]  # plus d[
-000198c0: 692d 622c 206a 2b31 5d0a 0a20 2020 2020  i-b, j+1]..     
-000198d0: 2020 2020 2020 2069 6620 6a69 2021 3d20         if ji != 
-000198e0: 6a62 3a20 2023 2065 7175 6174 696f 6e20  jb:  # equation 
-000198f0: 3130 2069 6e20 4861 6c65 2c20 3230 3133  10 in Hale, 2013
-00019900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019910: 2066 6f72 206b 6220 696e 2072 616e 6765   for kb in range
-00019920: 286a 692c 206a 6220 2b20 6949 6e63 202d  (ji, jb + iInc -
-00019930: 2031 2c20 2d69 496e 6329 3a0a 2020 2020   1, -iInc):.    
-00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019950: 6469 7374 4c6d 696e 7573 3120 3d20 6469  distLminus1 = di
-00019960: 7374 4c6d 696e 7573 3120 2b20 6572 725b  stLminus1 + err[
-00019970: 6b62 2c20 6c4d 696e 7573 315d 0a20 2020  kb, lMinus1].   
-00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019990: 2064 6973 744c 706c 7573 3120 3d20 6469   distLplus1 = di
-000199a0: 7374 4c70 6c75 7331 202b 2065 7272 5b6b  stLplus1 + err[k
-000199b0: 622c 206c 506c 7573 315d 0a0a 2020 2020  b, lPlus1]..    
-000199c0: 2020 2020 2020 2020 2320 6571 7561 7469          # equati
-000199d0: 6f6e 2036 2028 6966 2062 3d31 2920 6f72  on 6 (if b=1) or
-000199e0: 2031 3020 2869 6620 623e 3129 2069 6e20   10 (if b>1) in 
-000199f0: 4861 6c65 2028 3230 3133 2920 6166 7465  Hale (2013) afte
-00019a00: 7220 7472 6561 7469 6e67 2062 6f75 6e64  r treating bound
-00019a10: 6172 6965 730a 2020 2020 2020 2020 2020  aries.          
-00019a20: 2020 645b 6969 2c20 6c6c 5d20 3d20 6572    d[ii, ll] = er
-00019a30: 725b 6969 2c20 6c6c 5d20 2b20 6d69 6e28  r[ii, ll] + min(
-00019a40: 5b64 6973 744c 6d69 6e75 7331 2c20 6469  [distLminus1, di
-00019a50: 7374 4c2c 2064 6973 744c 706c 7573 315d  stL, distLplus1]
-00019a60: 290a 0a20 2020 2072 6574 7572 6e20 640a  )..    return d.
-00019a70: 0a0a 6465 6620 6261 636b 7472 6163 6b44  ..def backtrackD
-00019a80: 6973 7461 6e63 6546 756e 6374 696f 6e28  istanceFunction(
-00019a90: 6469 722c 2064 2c20 6572 722c 206c 6d69  dir, d, err, lmi
-00019aa0: 6e2c 2062 293a 0a20 2020 2022 2222 0a20  n, b):.    """. 
-00019ab0: 2020 2054 6865 2066 756e 6374 696f 6e20     The function 
-00019ac0: 6973 2065 7175 6174 696f 6e20 3220 696e  is equation 2 in
-00019ad0: 2048 616c 652c 2032 3031 332e 0a0a 2020   Hale, 2013...  
-00019ae0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00019af0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a   --------------.
-00019b00: 2020 2020 6469 723a 2073 6964 6520 746f      dir: side to
-00019b10: 2073 7461 7274 206d 696e 696d 697a 6174   start minimizat
-00019b20: 696f 6e20 2820 6469 7220 3e20 3020 3d20  ion ( dir > 0 = 
-00019b30: 6672 6f6e 742c 2064 6972 203c 3d20 3020  front, dir <= 0 
-00019b40: 3d20 2062 6163 6b29 0a20 2020 2064 203a  =  back).    d :
-00019b50: 2074 6865 2032 4420 6469 7374 616e 6365   the 2D distance
-00019b60: 2066 756e 6374 696f 6e3b 2073 697a 6520   function; size 
-00019b70: 3d20 286e 7361 6d70 2c32 2a6c 6167 2b31  = (nsamp,2*lag+1
-00019b80: 290a 2020 2020 6572 723a 2074 6865 2032  ).    err: the 2
-00019b90: 4420 6572 726f 7220 6675 6e63 7469 6f6e  D error function
-00019ba0: 3b20 7369 7a65 203d 2028 6e73 616d 702c  ; size = (nsamp,
-00019bb0: 322a 6c61 672b 3129 0a20 2020 206c 6d69  2*lag+1).    lmi
-00019bc0: 6e3a 206d 696e 696d 756d 206c 6167 2074  n: minimum lag t
-00019bd0: 6f20 7365 6172 6368 206f 7665 720a 2020  o search over.  
-00019be0: 2020 6220 3a20 7374 7261 696e 206c 696d    b : strain lim
-00019bf0: 6974 2028 696e 7465 6765 7220 7661 6c75  it (integer valu
-00019c00: 6520 3e3d 2031 290a 0a20 2020 2052 4554  e >= 1)..    RET
-00019c10: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
-00019c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00019c30: 2073 7462 6172 3a20 7665 6374 6f72 206f   stbar: vector o
-00019c40: 6620 696e 7465 6765 7220 7368 6966 7473  f integer shifts
-00019c50: 2073 7562 6a65 6374 2074 6f20 7c75 2869   subject to |u(i
-00019c60: 292d 7528 692d 3129 7c20 3c3d 2031 2f62  )-u(i-1)| <= 1/b
-00019c70: 0a0a 2020 2020 4f72 6967 696e 616c 2062  ..    Original b
-00019c80: 7920 4469 2059 616e 670a 2020 2020 4c61  y Di Yang.    La
-00019c90: 7374 206d 6f64 6966 6965 6420 6279 2044  st modified by D
-00019ca0: 796c 616e 204d 696b 6573 656c 6c20 2831  ylan Mikesell (1
-00019cb0: 3920 4465 632e 2032 3031 3429 0a0a 2020  9 Dec. 2014)..  
-00019cc0: 2020 5472 616e 736c 6174 6564 2074 6f20    Translated to 
-00019cd0: 7079 7468 6f6e 2062 7920 5469 6d20 436c  python by Tim Cl
-00019ce0: 656d 656e 7473 2028 3137 2041 7567 2e20  ements (17 Aug. 
-00019cf0: 3230 3138 290a 0a20 2020 2022 2222 0a0a  2018)..    """..
-00019d00: 2020 2020 6e53 616d 706c 652c 206e 4c61      nSample, nLa
-00019d10: 6720 3d20 642e 7368 6170 650a 2020 2020  g = d.shape.    
-00019d20: 7374 6261 7220 3d20 6e70 2e7a 6572 6f73  stbar = np.zeros
-00019d30: 286e 5361 6d70 6c65 290a 0a20 2020 2023  (nSample)..    #
-00019d40: 2053 6574 7570 2069 6e64 6963 6573 2062   Setup indices b
-00019d50: 6173 6564 206f 6e20 666f 7277 6172 6420  ased on forward 
-00019d60: 6f72 2062 6163 6b77 6172 6420 6163 6375  or backward accu
-00019d70: 6d75 6c61 7469 6f6e 2064 6972 6563 7469  mulation directi
-00019d80: 6f6e 0a20 2020 2069 6620 6469 7220 3e20  on.    if dir > 
-00019d90: 303a 2020 2320 464f 5257 4152 440a 2020  0:  # FORWARD.  
-00019da0: 2020 2020 2020 6942 6567 696e 2c20 6945        iBegin, iE
-00019db0: 6e64 2c20 6949 6e63 203d 2030 2c20 6e53  nd, iInc = 0, nS
-00019dc0: 616d 706c 6520 2d20 312c 2031 0a20 2020  ample - 1, 1.   
-00019dd0: 2065 6c73 653a 2020 2320 4241 434b 5741   else:  # BACKWA
-00019de0: 5244 0a20 2020 2020 2020 2069 4265 6769  RD.        iBegi
-00019df0: 6e2c 2069 456e 642c 2069 496e 6320 3d20  n, iEnd, iInc = 
-00019e00: 6e53 616d 706c 6520 2d20 312c 2030 2c20  nSample - 1, 0, 
-00019e10: 2d31 0a0a 2020 2020 2320 7374 6172 7420  -1..    # start 
-00019e20: 6672 6f6d 2074 6865 2065 6e64 2028 6672  from the end (fr
-00019e30: 6f6e 7420 6f72 2062 6163 6b29 0a20 2020  ont or back).   
-00019e40: 206c 6c20 3d20 6e70 2e61 7267 6d69 6e28   ll = np.argmin(
-00019e50: 645b 6942 6567 696e 2c20 3a5d 2920 2023  d[iBegin, :])  #
-00019e60: 2066 696e 6420 6d69 6e69 6d75 6d20 6163   find minimum ac
-00019e70: 6375 6d75 6c61 7465 6420 6469 7374 616e  cumulated distan
-00019e80: 6365 2061 7420 6672 6f6e 7420 6f72 2062  ce at front or b
-00019e90: 6163 6b20 6465 7065 6e64 696e 6720 6f6e  ack depending on
-00019ea0: 2027 6469 7227 0a20 2020 2073 7462 6172   'dir'.    stbar
-00019eb0: 5b69 4265 6769 6e5d 203d 206c 6c20 2b20  [iBegin] = ll + 
-00019ec0: 6c6d 696e 2020 2320 6162 736f 6c75 7465  lmin  # absolute
-00019ed0: 2076 616c 7565 206f 6620 696e 7465 6765   value of intege
-00019ee0: 7220 7368 6966 740a 0a20 2020 2023 206d  r shift..    # m
-00019ef0: 6f76 6520 7468 726f 7567 6820 616c 6c20  ove through all 
-00019f00: 7469 6d65 2073 616d 706c 6573 2069 6e20  time samples in 
-00019f10: 666f 7277 6172 6420 6f72 2062 6163 6b77  forward or backw
-00019f20: 6172 6420 6469 7265 6374 696f 6e0a 2020  ard direction.  
-00019f30: 2020 6969 203d 2069 4265 6769 6e0a 0a20    ii = iBegin.. 
-00019f40: 2020 2077 6869 6c65 2069 6920 213d 2069     while ii != i
-00019f50: 456e 643a 0a20 2020 2020 2020 2023 206d  End:.        # m
-00019f60: 696e 2f6d 6178 2066 6f72 2065 6467 6573  in/max for edges
-00019f70: 2f62 6f75 6e64 6172 6965 730a 2020 2020  /boundaries.    
-00019f80: 2020 2020 6a69 203d 206e 702e 6d61 7828      ji = np.max(
-00019f90: 5b30 2c20 6e70 2e6d 696e 285b 6e53 616d  [0, np.min([nSam
-00019fa0: 706c 6520 2d20 312c 2069 6920 2b20 6949  ple - 1, ii + iI
-00019fb0: 6e63 5d29 5d29 0a20 2020 2020 2020 206a  nc])]).        j
-00019fc0: 6220 3d20 6e70 2e6d 6178 285b 302c 206e  b = np.max([0, n
-00019fd0: 702e 6d69 6e28 5b6e 5361 6d70 6c65 202d  p.min([nSample -
-00019fe0: 2031 2c20 6969 202b 2069 496e 6320 2a20   1, ii + iInc * 
-00019ff0: 625d 295d 290a 0a20 2020 2020 2020 2023  b])])..        #
-0001a000: 2063 6865 636b 206c 696d 6974 7320 6f6e   check limits on
-0001a010: 206c 6167 2069 6e64 6963 6573 0a20 2020   lag indices.   
-0001a020: 2020 2020 206c 4d69 6e75 7331 203d 206c       lMinus1 = l
-0001a030: 6c20 2d20 310a 0a20 2020 2020 2020 2069  l - 1..        i
-0001a040: 6620 6c4d 696e 7573 3120 3c20 303a 2020  f lMinus1 < 0:  
-0001a050: 2320 6368 6563 6b20 6c61 6720 696e 6465  # check lag inde
-0001a060: 7820 6973 2067 7265 6174 6572 2074 6861  x is greater tha
-0001a070: 6e20 310a 2020 2020 2020 2020 2020 2020  n 1.            
-0001a080: 6c4d 696e 7573 3120 3d20 3020 2023 206d  lMinus1 = 0  # m
-0001a090: 616b 6520 6c61 6720 3d20 6669 7273 7420  ake lag = first 
-0001a0a0: 6c61 670a 0a20 2020 2020 2020 206c 506c  lag..        lPl
-0001a0b0: 7573 3120 3d20 6c6c 202b 2031 0a0a 2020  us1 = ll + 1..  
-0001a0c0: 2020 2020 2020 6966 206c 506c 7573 3120        if lPlus1 
-0001a0d0: 3e20 6e4c 6167 202d 2031 3a20 2023 2063  > nLag - 1:  # c
-0001a0e0: 6865 636b 206c 6167 2069 6e64 6578 206c  heck lag index l
-0001a0f0: 6573 7320 7468 616e 206d 6178 206c 6167  ess than max lag
-0001a100: 0a20 2020 2020 2020 2020 2020 206c 506c  .            lPl
-0001a110: 7573 3120 3d20 6e4c 6167 202d 2031 0a0a  us1 = nLag - 1..
-0001a120: 2020 2020 2020 2020 2320 6765 7420 6469          # get di
-0001a130: 7374 616e 6365 2061 7420 6c61 6773 2028  stance at lags (
-0001a140: 6c6c 2d31 2c20 6c6c 2c20 6c6c 2b31 290a  ll-1, ll, ll+1).
-0001a150: 2020 2020 2020 2020 6469 7374 4c6d 696e          distLmin
-0001a160: 7573 3120 3d20 645b 6a62 2c20 6c4d 696e  us1 = d[jb, lMin
-0001a170: 7573 315d 2020 2320 6d69 6e75 733a 2020  us1]  # minus:  
-0001a180: 645b 692d 622c 206a 2d31 5d0a 2020 2020  d[i-b, j-1].    
-0001a190: 2020 2020 6469 7374 4c20 3d20 645b 6a69      distL = d[ji
-0001a1a0: 2c20 6c6c 5d20 2023 2061 6374 7561 6c20  , ll]  # actual 
-0001a1b0: 645b 692d 312c 206a 5d0a 2020 2020 2020  d[i-1, j].      
-0001a1c0: 2020 6469 7374 4c70 6c75 7331 203d 2064    distLplus1 = d
-0001a1d0: 5b6a 622c 206c 506c 7573 315d 2020 2320  [jb, lPlus1]  # 
-0001a1e0: 706c 7573 2064 5b69 2d62 2c20 6a2b 315d  plus d[i-b, j+1]
-0001a1f0: 0a0a 2020 2020 2020 2020 2320 6571 7561  ..        # equa
-0001a200: 7469 6f6e 2031 3020 696e 2048 616c 6520  tion 10 in Hale 
-0001a210: 2832 3031 3329 0a20 2020 2020 2020 2023  (2013).        #
-0001a220: 2073 756d 2065 7272 6f72 7320 6f76 6572   sum errors over
-0001a230: 2069 2d31 3a69 2d62 2b31 0a20 2020 2020   i-1:i-b+1.     
-0001a240: 2020 2069 6620 6a69 2021 3d20 6a62 3a0a     if ji != jb:.
-0001a250: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001a260: 6b62 2069 6e20 7261 6e67 6528 6a69 2c20  kb in range(ji, 
-0001a270: 6a62 202d 2069 496e 6320 2d20 312c 2069  jb - iInc - 1, i
-0001a280: 496e 6329 3a0a 2020 2020 2020 2020 2020  Inc):.          
-0001a290: 2020 2020 2020 6469 7374 4c6d 696e 7573        distLminus
-0001a2a0: 3120 3d20 6469 7374 4c6d 696e 7573 3120  1 = distLminus1 
-0001a2b0: 2b20 6572 725b 6b62 2c20 6c4d 696e 7573  + err[kb, lMinus
-0001a2c0: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
-0001a2d0: 2020 2064 6973 744c 706c 7573 3120 3d20     distLplus1 = 
-0001a2e0: 6469 7374 4c70 6c75 7331 202b 2065 7272  distLplus1 + err
-0001a2f0: 5b6b 622c 206c 506c 7573 315d 0a0a 2020  [kb, lPlus1]..  
-0001a300: 2020 2020 2020 2320 7570 6461 7465 206d        # update m
-0001a310: 696e 696d 756d 2064 6973 7461 6e63 6520  inimum distance 
-0001a320: 746f 2070 7265 7669 6f75 7320 7361 6d70  to previous samp
-0001a330: 6c65 0a20 2020 2020 2020 2064 6c20 3d20  le.        dl = 
-0001a340: 6e70 2e6d 696e 285b 6469 7374 4c6d 696e  np.min([distLmin
-0001a350: 7573 312c 2064 6973 744c 2c20 6469 7374  us1, distL, dist
-0001a360: 4c70 6c75 7331 5d29 0a0a 2020 2020 2020  Lplus1])..      
-0001a370: 2020 6966 2064 6c20 213d 2064 6973 744c    if dl != distL
-0001a380: 3a20 2023 2074 6865 6e20 6c6c 207e 3d20  :  # then ll ~= 
-0001a390: 6c6c 2061 6e64 2077 6520 6368 6563 6b20  ll and we check 
-0001a3a0: 666f 7277 6172 6420 616e 6420 6261 636b  forward and back
-0001a3b0: 7761 7264 0a20 2020 2020 2020 2020 2020  ward.           
-0001a3c0: 2069 6620 646c 203d 3d20 6469 7374 4c6d   if dl == distLm
-0001a3d0: 696e 7573 313a 0a20 2020 2020 2020 2020  inus1:.         
-0001a3e0: 2020 2020 2020 206c 6c20 3d20 6c4d 696e         ll = lMin
-0001a3f0: 7573 310a 2020 2020 2020 2020 2020 2020  us1.            
-0001a400: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001a410: 2020 2020 2020 6c6c 203d 206c 506c 7573        ll = lPlus
-0001a420: 310a 0a20 2020 2020 2020 2023 2061 7373  1..        # ass
-0001a430: 756d 6520 6969 203d 2069 6920 2d20 310a  ume ii = ii - 1.
-0001a440: 2020 2020 2020 2020 6969 202b 3d20 6949          ii += iI
-0001a450: 6e63 0a0a 2020 2020 2020 2020 2320 6162  nc..        # ab
-0001a460: 736f 6c75 7465 2069 6e74 6567 6572 206f  solute integer o
-0001a470: 6620 6c61 670a 2020 2020 2020 2020 7374  f lag.        st
-0001a480: 6261 725b 6969 5d20 3d20 6c6c 202b 206c  bar[ii] = ll + l
-0001a490: 6d69 6e0a 0a20 2020 2020 2020 2023 206e  min..        # n
-0001a4a0: 6f77 206d 6f76 6520 746f 2063 6f72 7265  ow move to corre
-0001a4b0: 6374 2074 696d 6520 696e 6465 782c 2069  ct time index, i
-0001a4c0: 6620 736d 6f6f 7468 696e 6720 6469 6666  f smoothing diff
-0001a4d0: 6572 656e 6365 206f 7665 7220 6d61 6e79  erence over many
-0001a4e0: 0a20 2020 2020 2020 2023 2074 696d 6520  .        # time 
-0001a4f0: 7361 6d70 6c65 7320 7573 696e 6720 2762  samples using 'b
-0001a500: 270a 2020 2020 2020 2020 6966 2028 6c6c  '.        if (ll
-0001a510: 203d 3d20 6c4d 696e 7573 3129 207c 2028   == lMinus1) | (
-0001a520: 6c6c 203d 3d20 6c50 6c75 7331 293a 2020  ll == lPlus1):  
-0001a530: 2320 6368 6563 6b20 6564 6765 7320 746f  # check edges to
-0001a540: 2073 6565 2061 626f 7574 2062 2076 616c   see about b val
-0001a550: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
-0001a560: 6966 206a 6920 213d 206a 623a 2020 2320  if ji != jb:  # 
-0001a570: 6966 2062 3e31 2074 6865 6e20 6e65 6564  if b>1 then need
-0001a580: 2074 6f20 6d6f 7665 206d 6f72 6520 7374   to move more st
-0001a590: 6570 730a 2020 2020 2020 2020 2020 2020  eps.            
-0001a5a0: 2020 2020 666f 7220 6b62 2069 6e20 7261      for kb in ra
-0001a5b0: 6e67 6528 6a69 2c20 6a62 202d 2069 496e  nge(ji, jb - iIn
-0001a5c0: 6320 2d20 312c 2069 496e 6329 3a0a 2020  c - 1, iInc):.  
-0001a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5e0: 2020 6969 203d 2069 6920 2b20 6949 6e63    ii = ii + iInc
-0001a5f0: 2020 2320 6d6f 7665 2066 726f 6d20 692d    # move from i-
-0001a600: 313a 692d 622d 310a 2020 2020 2020 2020  1:i-b-1.        
-0001a610: 2020 2020 2020 2020 2020 2020 7374 6261              stba
-0001a620: 725b 6969 5d20 3d20 6c6c 202b 206c 6d69  r[ii] = ll + lmi
-0001a630: 6e20 2023 2063 6f6e 7374 616e 7420 6c61  n  # constant la
-0001a640: 6720 6f76 6572 2074 6861 7420 7469 6d65  g over that time
-0001a650: 0a0a 2020 2020 7265 7475 726e 2073 7462  ..    return stb
-0001a660: 6172 0a0a 0a64 6566 2077 6374 5f6d 6f64  ar...def wct_mod
-0001a670: 6966 6965 6428 0a20 2020 2079 312c 2079  ified(.    y1, y
-0001a680: 322c 2064 742c 2064 6a3d 3120 2f20 3132  2, dt, dj=1 / 12
-0001a690: 2c20 7330 3d2d 312c 204a 3d2d 312c 2073  , s0=-1, J=-1, s
-0001a6a0: 6967 3d54 7275 652c 2073 6967 6e69 6669  ig=True, signifi
-0001a6b0: 6361 6e63 655f 6c65 7665 6c3d 302e 3935  cance_level=0.95
-0001a6c0: 2c20 7761 7665 6c65 743d 226d 6f72 6c65  , wavelet="morle
-0001a6d0: 7422 2c20 6e6f 726d 616c 697a 653d 5472  t", normalize=Tr
-0001a6e0: 7565 2c20 2a2a 6b77 6172 6773 0a29 3a0a  ue, **kwargs.):.
-0001a6f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0001a700: 5761 7665 6c65 7420 636f 6865 7265 6e63  Wavelet coherenc
-0001a710: 6520 7472 616e 7366 6f72 6d20 2857 4354  e transform (WCT
-0001a720: 292e 0a20 2020 20e2 808b 0a20 2020 2020  )..    ....     
-0001a730: 2020 2054 6865 2057 4354 2066 696e 6473     The WCT finds
-0001a740: 2072 6567 696f 6e73 2069 6e20 7469 6d65   regions in time
-0001a750: 2066 7265 7175 656e 6379 2073 7061 6365   frequency space
-0001a760: 2077 6865 7265 2074 6865 2074 776f 2074   where the two t
-0001a770: 696d 650a 2020 2020 2020 2020 7365 7269  ime.        seri
-0001a780: 6573 2063 6f2d 7661 7279 2c20 6275 7420  es co-vary, but 
-0001a790: 646f 206e 6f74 206e 6563 6573 7361 7269  do not necessari
-0001a7a0: 6c79 2068 6176 6520 6869 6768 2070 6f77  ly have high pow
-0001a7b0: 6572 2e0a 2020 2020 e280 8b0a 2020 2020  er..    ....    
-0001a7c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0001a7d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0001a7e0: 2d0a 2020 2020 2020 2020 7931 2c20 7932  -.        y1, y2
-0001a7f0: 203a 206e 756d 7079 2e6e 6461 7272 6179   : numpy.ndarray
-0001a800: 2c20 6c69 7374 0a20 2020 2020 2020 2020  , list.         
-0001a810: 2020 2049 6e70 7574 2073 6967 6e61 6c73     Input signals
-0001a820: 2e0a 2020 2020 2020 2020 6474 203a 2066  ..        dt : f
-0001a830: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
-0001a840: 2053 616d 706c 6520 7370 6163 696e 672e   Sample spacing.
-0001a850: 0a20 2020 2020 2020 2064 6a20 3a20 666c  .        dj : fl
-0001a860: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-0001a870: 2020 2020 2020 2020 2020 5370 6163 696e            Spacin
-0001a880: 6720 6265 7477 6565 6e20 6469 7363 7265  g between discre
-0001a890: 7465 2073 6361 6c65 732e 2044 6566 6175  te scales. Defau
-0001a8a0: 6c74 2076 616c 7565 2069 7320 312f 3132  lt value is 1/12
-0001a8b0: 2e0a 2020 2020 2020 2020 2020 2020 536d  ..            Sm
-0001a8c0: 616c 6c65 7220 7661 6c75 6573 2077 696c  aller values wil
-0001a8d0: 6c20 7265 7375 6c74 2069 6e20 6265 7474  l result in bett
-0001a8e0: 6572 2073 6361 6c65 2072 6573 6f6c 7574  er scale resolut
-0001a8f0: 696f 6e2c 2062 7574 0a20 2020 2020 2020  ion, but.       
-0001a900: 2020 2020 2073 6c6f 7765 7220 6361 6c63       slower calc
-0001a910: 756c 6174 696f 6e20 616e 6420 706c 6f74  ulation and plot
-0001a920: 2e0a 2020 2020 2020 2020 7330 203a 2066  ..        s0 : f
-0001a930: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
-0001a940: 2020 2020 2020 2020 2020 2053 6d61 6c6c             Small
-0001a950: 6573 7420 7363 616c 6520 6f66 2074 6865  est scale of the
-0001a960: 2077 6176 656c 6574 2e20 4465 6661 756c   wavelet. Defaul
-0001a970: 7420 7661 6c75 6520 6973 2032 2a64 742e  t value is 2*dt.
-0001a980: 0a20 2020 2020 2020 204a 203a 2066 6c6f  .        J : flo
-0001a990: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
-0001a9a0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-0001a9b0: 6f66 2073 6361 6c65 7320 6c65 7373 206f  of scales less o
-0001a9c0: 6e65 2e20 5363 616c 6573 2072 616e 6765  ne. Scales range
-0001a9d0: 2066 726f 6d20 7330 2075 7020 746f 0a20   from s0 up to. 
-0001a9e0: 2020 2020 2020 2020 2020 2073 3020 2a20             s0 * 
-0001a9f0: 322a 2a28 4a20 2a20 646a 292c 2077 6869  2**(J * dj), whi
-0001aa00: 6368 2067 6976 6573 2061 2074 6f74 616c  ch gives a total
-0001aa10: 206f 6620 284a 202b 2031 2920 7363 616c   of (J + 1) scal
-0001aa20: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-0001aa30: 4465 6661 756c 7420 6973 204a 203d 2028  Default is J = (
-0001aa40: 6c6f 6732 284e 2a64 742f 736f 2929 2f64  log2(N*dt/so))/d
-0001aa50: 6a2e 0a20 2020 2020 2020 2073 6967 6e69  j..        signi
-0001aa60: 6669 6361 6e63 655f 6c65 7665 6c20 2866  ficance_level (f
-0001aa70: 6c6f 6174 2c20 6f70 7469 6f6e 616c 2920  loat, optional) 
-0001aa80: 3a0a 2020 2020 2020 2020 2020 2020 5369  :.            Si
-0001aa90: 676e 6966 6963 616e 6365 206c 6576 656c  gnificance level
-0001aaa0: 2074 6f20 7573 652e 2044 6566 6175 6c74   to use. Default
-0001aab0: 2069 7320 302e 3935 2e0a 2020 2020 2020   is 0.95..      
-0001aac0: 2020 6e6f 726d 616c 697a 6520 2862 6f6f    normalize (boo
-0001aad0: 6c65 616e 2c20 6f70 7469 6f6e 616c 2920  lean, optional) 
-0001aae0: 3a0a 2020 2020 2020 2020 2020 2020 4966  :.            If
-0001aaf0: 2073 6574 2074 6f20 7472 7565 2c20 6e6f   set to true, no
-0001ab00: 726d 616c 697a 6573 2043 5754 2062 7920  rmalizes CWT by 
-0001ab10: 7468 6520 7374 616e 6461 7264 2064 6576  the standard dev
-0001ab20: 6961 7469 6f6e 206f 660a 2020 2020 2020  iation of.      
-0001ab30: 2020 2020 2020 7468 6520 7369 676e 616c        the signal
-0001ab40: 732e 0a20 2020 20e2 808b 0a20 2020 2020  s..    ....     
-0001ab50: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0001ab60: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0001ab70: 2020 2054 4f44 4f3a 2053 6f6d 6574 6869     TODO: Somethi
-0001ab80: 6e67 2054 4241 2061 6e64 2054 4243 0a20  ng TBA and TBC. 
-0001ab90: 2020 20e2 808b 0a20 2020 2020 2020 2053     ....        S
-0001aba0: 6565 2061 6c73 6f0a 2020 2020 2020 2020  ee also.        
-0001abb0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0001abc0: 2063 7774 2c20 7877 740a 2020 2020 e280   cwt, xwt.    ..
-0001abd0: 8b0a 2020 2020 2222 220a 0a20 2020 2077  ..    """..    w
-0001abe0: 6176 656c 6574 203d 2070 7963 7774 2e77  avelet = pycwt.w
-0001abf0: 6176 656c 6574 2e5f 6368 6563 6b5f 7061  avelet._check_pa
-0001ac00: 7261 6d65 7465 725f 7761 7665 6c65 7428  rameter_wavelet(
-0001ac10: 7761 7665 6c65 7429 0a20 2020 2023 2043  wavelet).    # C
-0001ac20: 6865 636b 696e 6720 736f 6d65 2069 6e70  hecking some inp
-0001ac30: 7574 2070 6172 616d 6574 6572 730a 2020  ut parameters.  
-0001ac40: 2020 6966 2073 3020 3d3d 202d 313a 0a20    if s0 == -1:. 
-0001ac50: 2020 2020 2020 2023 204e 756d 6265 7220         # Number 
-0001ac60: 6f66 2073 6361 6c65 730a 2020 2020 2020  of scales.      
-0001ac70: 2020 7330 203d 2032 202a 2064 7420 2f20    s0 = 2 * dt / 
-0001ac80: 7761 7665 6c65 742e 666c 616d 6264 6128  wavelet.flambda(
-0001ac90: 290a 2020 2020 6966 204a 203d 3d20 2d31  ).    if J == -1
-0001aca0: 3a0a 2020 2020 2020 2020 2320 4e75 6d62  :.        # Numb
-0001acb0: 6572 206f 6620 7363 616c 6573 0a20 2020  er of scales.   
-0001acc0: 2020 2020 204a 203d 206e 702e 696e 7428       J = np.int(
-0001acd0: 6e70 2e72 6f75 6e64 286e 702e 6c6f 6732  np.round(np.log2
-0001ace0: 2879 312e 7369 7a65 202a 2064 7420 2f20  (y1.size * dt / 
-0001acf0: 7330 2920 2f20 646a 2929 0a0a 2020 2020  s0) / dj))..    
-0001ad00: 2320 4d61 6b65 7320 7375 7265 2069 6e70  # Makes sure inp
-0001ad10: 7574 2073 6967 6e61 6c73 2061 7265 206e  ut signals are n
-0001ad20: 756d 7079 2061 7272 6179 732e 0a20 2020  umpy arrays..   
-0001ad30: 2079 3120 3d20 6e70 2e61 7361 7272 6179   y1 = np.asarray
-0001ad40: 2879 3129 0a20 2020 2079 3220 3d20 6e70  (y1).    y2 = np
-0001ad50: 2e61 7361 7272 6179 2879 3229 0a20 2020  .asarray(y2).   
-0001ad60: 2023 2043 616c 6375 6c61 7465 7320 7468   # Calculates th
-0001ad70: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
-0001ad80: 7469 6f6e 206f 6620 626f 7468 2069 6e70  tion of both inp
-0001ad90: 7574 2073 6967 6e61 6c73 2e0a 2020 2020  ut signals..    
-0001ada0: 7374 6431 203d 2079 312e 7374 6428 290a  std1 = y1.std().
-0001adb0: 2020 2020 7374 6432 203d 2079 322e 7374      std2 = y2.st
-0001adc0: 6428 290a 2020 2020 2320 4e6f 726d 616c  d().    # Normal
-0001add0: 697a 6573 2062 6f74 6820 7369 676e 616c  izes both signal
-0001ade0: 732c 2069 6620 6170 7072 6f70 7269 6174  s, if appropriat
-0001adf0: 652e 0a20 2020 2069 6620 6e6f 726d 616c  e..    if normal
-0001ae00: 697a 653a 0a20 2020 2020 2020 2079 315f  ize:.        y1_
-0001ae10: 6e6f 726d 616c 203d 2028 7931 202d 2079  normal = (y1 - y
-0001ae20: 312e 6d65 616e 2829 2920 2f20 7374 6431  1.mean()) / std1
-0001ae30: 0a20 2020 2020 2020 2079 325f 6e6f 726d  .        y2_norm
-0001ae40: 616c 203d 2028 7932 202d 2079 322e 6d65  al = (y2 - y2.me
-0001ae50: 616e 2829 2920 2f20 7374 6432 0a20 2020  an()) / std2.   
-0001ae60: 2065 6c73 653a 0a20 2020 2020 2020 2079   else:.        y
-0001ae70: 315f 6e6f 726d 616c 203d 2079 310a 2020  1_normal = y1.  
-0001ae80: 2020 2020 2020 7932 5f6e 6f72 6d61 6c20        y2_normal 
-0001ae90: 3d20 7932 0a0a 2020 2020 2320 4361 6c63  = y2..    # Calc
-0001aea0: 756c 6174 6573 2074 6865 2043 5754 206f  ulates the CWT o
-0001aeb0: 6620 7468 6520 7469 6d65 2d73 6572 6965  f the time-serie
-0001aec0: 7320 6d61 6b69 6e67 2073 7572 6520 7468  s making sure th
-0001aed0: 6520 7361 6d65 2070 6172 616d 6574 6572  e same parameter
-0001aee0: 730a 2020 2020 2320 6172 6520 7573 6564  s.    # are used
-0001aef0: 2069 6e20 626f 7468 2063 616c 6375 6c61   in both calcula
-0001af00: 7469 6f6e 732e 0a20 2020 205f 6b77 6172  tions..    _kwar
-0001af10: 6773 203d 2064 6963 7428 646a 3d64 6a2c  gs = dict(dj=dj,
-0001af20: 2073 303d 7330 2c20 4a3d 4a2c 2077 6176   s0=s0, J=J, wav
-0001af30: 656c 6574 3d77 6176 656c 6574 290a 2020  elet=wavelet).  
-0001af40: 2020 5731 2c20 736a 2c20 6672 6571 2c20    W1, sj, freq, 
-0001af50: 636f 692c 205f 2c20 5f20 3d20 7079 6377  coi, _, _ = pycw
-0001af60: 742e 6377 7428 7931 5f6e 6f72 6d61 6c2c  t.cwt(y1_normal,
-0001af70: 2064 742c 202a 2a5f 6b77 6172 6773 290a   dt, **_kwargs).
-0001af80: 2020 2020 5732 2c20 736a 2c20 6672 6571      W2, sj, freq
-0001af90: 2c20 636f 692c 205f 2c20 5f20 3d20 7079  , coi, _, _ = py
-0001afa0: 6377 742e 6377 7428 7932 5f6e 6f72 6d61  cwt.cwt(y2_norma
-0001afb0: 6c2c 2064 742c 202a 2a5f 6b77 6172 6773  l, dt, **_kwargs
-0001afc0: 290a 0a20 2020 2073 6361 6c65 7331 203d  )..    scales1 =
-0001afd0: 206e 702e 6f6e 6573 285b 312c 2079 312e   np.ones([1, y1.
-0001afe0: 7369 7a65 5d29 202a 2073 6a5b 3a2c 204e  size]) * sj[:, N
-0001aff0: 6f6e 655d 0a20 2020 2073 6361 6c65 7332  one].    scales2
-0001b000: 203d 206e 702e 6f6e 6573 285b 312c 2079   = np.ones([1, y
-0001b010: 322e 7369 7a65 5d29 202a 2073 6a5b 3a2c  2.size]) * sj[:,
-0001b020: 204e 6f6e 655d 0a0a 2020 2020 2320 536d   None]..    # Sm
-0001b030: 6f6f 7468 2074 6865 2077 6176 656c 6574  ooth the wavelet
-0001b040: 2073 7065 6374 7261 2062 6566 6f72 6520   spectra before 
-0001b050: 7472 756e 6361 7469 6e67 2e0a 2020 2020  truncating..    
-0001b060: 5331 203d 2077 6176 656c 6574 2e73 6d6f  S1 = wavelet.smo
-0001b070: 6f74 6828 6e70 2e61 6273 2857 3129 202a  oth(np.abs(W1) *
-0001b080: 2a20 3220 2f20 7363 616c 6573 312c 2064  * 2 / scales1, d
-0001b090: 742c 2064 6a2c 2073 6a29 0a20 2020 2053  t, dj, sj).    S
-0001b0a0: 3220 3d20 7761 7665 6c65 742e 736d 6f6f  2 = wavelet.smoo
-0001b0b0: 7468 286e 702e 6162 7328 5732 2920 2a2a  th(np.abs(W2) **
-0001b0c0: 2032 202f 2073 6361 6c65 7332 2c20 6474   2 / scales2, dt
-0001b0d0: 2c20 646a 2c20 736a 290a 0a20 2020 2023  , dj, sj)..    #
-0001b0e0: 204e 6f77 2074 6865 2077 6176 656c 6574   Now the wavelet
-0001b0f0: 2074 7261 6e73 666f 726d 2063 6f68 6572   transform coher
-0001b100: 656e 6365 0a20 2020 2057 3132 203d 2057  ence.    W12 = W
-0001b110: 3120 2a20 5732 2e63 6f6e 6a28 290a 2020  1 * W2.conj().  
-0001b120: 2020 7363 616c 6573 203d 206e 702e 6f6e    scales = np.on
-0001b130: 6573 285b 312c 2079 312e 7369 7a65 5d29  es([1, y1.size])
-0001b140: 202a 2073 6a5b 3a2c 204e 6f6e 655d 0a20   * sj[:, None]. 
-0001b150: 2020 2053 3132 203d 2077 6176 656c 6574     S12 = wavelet
-0001b160: 2e73 6d6f 6f74 6828 5731 3220 2f20 7363  .smooth(W12 / sc
-0001b170: 616c 6573 2c20 6474 2c20 646a 2c20 736a  ales, dt, dj, sj
-0001b180: 290a 2020 2020 5743 5420 3d20 6e70 2e61  ).    WCT = np.a
-0001b190: 6273 2853 3132 2920 2a2a 2032 202f 2028  bs(S12) ** 2 / (
-0001b1a0: 5331 202a 2053 3229 0a20 2020 2061 5743  S1 * S2).    aWC
-0001b1b0: 5420 3d20 6e70 2e61 6e67 6c65 2857 3132  T = np.angle(W12
-0001b1c0: 290a 0a20 2020 2023 2043 616c 6375 6c61  )..    # Calcula
-0001b1d0: 7465 7320 7468 6520 7369 676e 6966 6963  tes the signific
-0001b1e0: 616e 6365 2075 7369 6e67 204d 6f6e 7465  ance using Monte
-0001b1f0: 2043 6172 6c6f 2073 696d 756c 6174 696f   Carlo simulatio
-0001b200: 6e73 2077 6974 6820 3935 250a 2020 2020  ns with 95%.    
-0001b210: 2320 636f 6e66 6964 656e 6365 2061 7320  # confidence as 
-0001b220: 6120 6675 6e63 7469 6f6e 206f 6620 7363  a function of sc
-0001b230: 616c 652e 0a0a 2020 2020 6966 2073 6967  ale...    if sig
-0001b240: 3a0a 2020 2020 2020 2020 6131 2c20 6231  :.        a1, b1
-0001b250: 2c20 6331 203d 2070 7963 7774 2e61 7231  , c1 = pycwt.ar1
-0001b260: 2879 3129 0a20 2020 2020 2020 2061 322c  (y1).        a2,
-0001b270: 2062 322c 2063 3220 3d20 7079 6377 742e   b2, c2 = pycwt.
-0001b280: 6172 3128 7932 290a 2020 2020 2020 2020  ar1(y2).        
-0001b290: 7369 6720 3d20 7079 6377 742e 7763 745f  sig = pycwt.wct_
-0001b2a0: 7369 676e 6966 6963 616e 6365 280a 2020  significance(.  
-0001b2b0: 2020 2020 2020 2020 2020 6131 2c20 6132            a1, a2
-0001b2c0: 2c20 6474 3d64 742c 2064 6a3d 646a 2c20  , dt=dt, dj=dj, 
-0001b2d0: 7330 3d73 302c 204a 3d4a 2c20 7369 676e  s0=s0, J=J, sign
-0001b2e0: 6966 6963 616e 6365 5f6c 6576 656c 3d73  ificance_level=s
-0001b2f0: 6967 6e69 6669 6361 6e63 655f 6c65 7665  ignificance_leve
-0001b300: 6c2c 2077 6176 656c 6574 3d77 6176 656c  l, wavelet=wavel
-0001b310: 6574 2c20 2a2a 6b77 6172 6773 0a20 2020  et, **kwargs.   
-0001b320: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
-0001b330: 0a20 2020 2020 2020 2073 6967 203d 206e  .        sig = n
-0001b340: 702e 6173 6172 7261 7928 5b30 5d29 0a0a  p.asarray([0])..
-0001b350: 2020 2020 7265 7475 726e 2057 4354 2c20      return WCT, 
-0001b360: 6157 4354 2c20 636f 692c 2066 7265 712c  aWCT, coi, freq,
-0001b370: 2073 6967 0a0a 0a23 2323 2323 2323 2323   sig...#########
-0001b380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018380: 2323 2323 2323 230a 0a22 2222 0a62 656c  #######..""".bel
+00018390: 6f77 2061 7265 2061 7373 656d 626c 7920  ow are assembly 
+000183a0: 6f66 2074 6865 206d 6f6e 6974 6f72 696e  of the monitorin
+000183b0: 6720 7574 696c 6974 7920 6675 6e63 7469  g utility functi
+000183c0: 6f6e 7320 6361 6c6c 6564 2062 7920 6d6f  ons called by mo
+000183d0: 6e69 746f 7269 6e67 2066 756e 6374 696f  nitoring functio
+000183e0: 6e73 0a22 2222 0a0a 0a64 6566 2073 6d6f  ns."""...def smo
+000183f0: 6f74 6828 782c 2077 696e 646f 773d 2262  oth(x, window="b
+00018400: 6f78 6361 7222 2c20 6861 6c66 5f77 696e  oxcar", half_win
+00018410: 3d33 293a 0a20 2020 2022 2222 0a20 2020  =3):.    """.   
+00018420: 2070 6572 666f 726d 7320 736d 6f6f 7468   performs smooth
+00018430: 696e 6720 696e 2069 6e74 6572 6573 7465  ing in intereste
+00018440: 6420 7469 6d65 2077 696e 646f 770a 0a20  d time window.. 
+00018450: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00018460: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00018470: 0a20 2020 2078 3a20 7469 6d65 7365 7269  .    x: timeseri
+00018480: 7320 6461 7461 0a20 2020 2077 696e 646f  s data.    windo
+00018490: 773a 2074 7970 6573 206f 6620 7769 6e64  w: types of wind
+000184a0: 6f77 2074 6f20 646f 2073 6d6f 6f74 6869  ow to do smoothi
+000184b0: 6e67 0a20 2020 2068 616c 665f 7769 6e3a  ng.    half_win:
+000184c0: 2068 616c 6620 7769 6e64 6f77 206c 656e   half window len
+000184d0: 6774 680a 0a20 2020 2052 4554 5552 4e53  gth..    RETURNS
+000184e0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+000184f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2079 3a20  --------.    y: 
+00018500: 736d 6f6f 7468 6564 2074 696d 6520 7769  smoothed time wi
+00018510: 6e64 6f77 0a20 2020 2022 2222 0a20 2020  ndow.    """.   
+00018520: 2023 2054 4f44 4f3a 2064 6f63 7374 696e   # TODO: docstin
+00018530: 670a 2020 2020 7769 6e64 6f77 5f6c 656e  g.    window_len
+00018540: 203d 2032 202a 2068 616c 665f 7769 6e20   = 2 * half_win 
+00018550: 2b20 310a 2020 2020 2320 6578 7465 6e64  + 1.    # extend
+00018560: 696e 6720 7468 6520 6461 7461 2061 7420  ing the data at 
+00018570: 6265 6769 6e6e 696e 6720 616e 6420 6174  beginning and at
+00018580: 2074 6865 2065 6e64 0a20 2020 2023 2074   the end.    # t
+00018590: 6f20 6170 706c 7920 7468 6520 7769 6e64  o apply the wind
+000185a0: 6f77 2061 7420 7468 6520 626f 7264 6572  ow at the border
+000185b0: 730a 2020 2020 7320 3d20 6e70 2e72 5f5b  s.    s = np.r_[
+000185c0: 785b 7769 6e64 6f77 5f6c 656e 202d 2031  x[window_len - 1
+000185d0: 203a 2030 203a 202d 315d 2c20 782c 2078   : 0 : -1], x, x
+000185e0: 5b2d 313a 2d77 696e 646f 775f 6c65 6e3a  [-1:-window_len:
+000185f0: 2d31 5d5d 0a20 2020 2069 6620 7769 6e64  -1]].    if wind
+00018600: 6f77 203d 3d20 2262 6f78 6361 7222 3a0a  ow == "boxcar":.
+00018610: 2020 2020 2020 2020 7720 3d20 7363 6970          w = scip
+00018620: 792e 7369 676e 616c 2e62 6f78 6361 7228  y.signal.boxcar(
+00018630: 7769 6e64 6f77 5f6c 656e 292e 6173 7479  window_len).asty
+00018640: 7065 2822 636f 6d70 6c65 7822 290a 2020  pe("complex").  
+00018650: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00018660: 7720 3d20 7363 6970 792e 7369 676e 616c  w = scipy.signal
+00018670: 2e68 616e 6e69 6e67 2877 696e 646f 775f  .hanning(window_
+00018680: 6c65 6e29 2e61 7374 7970 6528 2263 6f6d  len).astype("com
+00018690: 706c 6578 2229 0a20 2020 2079 203d 206e  plex").    y = n
+000186a0: 702e 636f 6e76 6f6c 7665 2877 202f 2077  p.convolve(w / w
+000186b0: 2e73 756d 2829 2c20 732c 206d 6f64 653d  .sum(), s, mode=
+000186c0: 2276 616c 6964 2229 0a20 2020 2072 6574  "valid").    ret
+000186d0: 7572 6e20 795b 6861 6c66 5f77 696e 203a  urn y[half_win :
+000186e0: 206c 656e 2879 2920 2d20 6861 6c66 5f77   len(y) - half_w
+000186f0: 696e 5d0a 0a0a 6465 6620 6e65 7874 706f  in]...def nextpo
+00018700: 7732 2878 293a 0a20 2020 2022 2222 0a20  w2(x):.    """. 
+00018710: 2020 2052 6574 7572 6e73 2074 6865 206e     Returns the n
+00018720: 6578 7420 706f 7765 7220 6f66 2032 206f  ext power of 2 o
+00018730: 6620 782e 0a20 2020 2022 2222 0a20 2020  f x..    """.   
+00018740: 2072 6574 7572 6e20 696e 7428 6e70 2e63   return int(np.c
+00018750: 6569 6c28 6e70 2e6c 6f67 3228 6e70 2e61  eil(np.log2(np.a
+00018760: 6273 2878 2929 2929 0a0a 0a64 6566 2067  bs(x))))...def g
+00018770: 6574 436f 6865 7265 6e63 6528 6463 732c  etCoherence(dcs,
+00018780: 2064 7331 2c20 6473 3229 3a0a 2020 2020   ds1, ds2):.    
+00018790: 2222 220a 2020 2020 6765 7420 6372 6f73  """.    get cros
+000187a0: 7320 636f 6865 7265 6e63 6520 6265 7477  s coherence betw
+000187b0: 6565 6e20 7265 6665 7265 6e63 6520 616e  een reference an
+000187c0: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
+000187d0: 726d 7320 666f 6c6c 6f77 696e 6720 6571  rms following eq
+000187e0: 7561 7469 6f6e 206f 6620 4133 2069 6e20  uation of A3 in 
+000187f0: 436c 6172 6b20 6574 2061 6c2e 2c20 3230  Clark et al., 20
+00018800: 3131 0a0a 2020 2020 5061 7261 6d65 7465  11..    Paramete
+00018810: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00018820: 2d2d 2d2d 2d0a 2020 2020 6463 733a 2061  -----.    dcs: a
+00018830: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
+00018840: 6372 6f73 7320 7370 6563 7472 756d 0a20  cross spectrum. 
+00018850: 2020 2064 7331 3a20 616d 706c 6974 7564     ds1: amplitud
+00018860: 6520 6f66 2074 6865 2073 7065 6374 7275  e of the spectru
+00018870: 6d20 6f66 2063 7572 7265 6e74 2077 6176  m of current wav
+00018880: 6566 6f72 6d0a 2020 2020 6473 323a 2061  eform.    ds2: a
+00018890: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
+000188a0: 7370 6563 7472 756d 206f 6620 7265 6665  spectrum of refe
+000188b0: 7265 6e63 6520 7761 7665 666f 726d 0a0a  rence waveform..
+000188c0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+000188d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000188e0: 2d2d 2d0a 2020 2020 636f 683a 2063 6f68  ---.    coh: coh
+000188f0: 7265 7265 6e63 7920 6d61 7472 6978 2075  rerency matrix u
+00018900: 7365 6420 666f 7220 6573 7469 6d61 7465  sed for estimate
+00018910: 2074 6865 2072 6f62 7573 746e 6573 7320   the robustness 
+00018920: 6f66 2074 6865 2063 726f 7373 2073 7065  of the cross spe
+00018930: 6374 7275 6d0a 2020 2020 2222 220a 2020  ctrum.    """.  
+00018940: 2020 6e20 3d20 6c65 6e28 6463 7329 0a20    n = len(dcs). 
+00018950: 2020 2063 6f68 203d 206e 702e 7a65 726f     coh = np.zero
+00018960: 7328 6e29 2e61 7374 7970 6528 2263 6f6d  s(n).astype("com
+00018970: 706c 6578 2229 0a20 2020 2076 616c 6964  plex").    valid
+00018980: 7320 3d20 6e70 2e61 7267 7768 6572 6528  s = np.argwhere(
+00018990: 6e70 2e6c 6f67 6963 616c 5f61 6e64 286e  np.logical_and(n
+000189a0: 702e 6162 7328 6473 3129 203e 2030 2c20  p.abs(ds1) > 0, 
+000189b0: 6e70 2e61 6273 2864 7332 2920 3e20 3029  np.abs(ds2) > 0)
+000189c0: 290a 2020 2020 636f 685b 7661 6c69 6473  ).    coh[valids
+000189d0: 5d20 3d20 6463 735b 7661 6c69 6473 5d20  ] = dcs[valids] 
+000189e0: 2f20 2864 7331 5b76 616c 6964 735d 202a  / (ds1[valids] *
+000189f0: 2064 7332 5b76 616c 6964 735d 290a 2020   ds2[valids]).  
+00018a00: 2020 636f 685b 636f 6820 3e20 2831 2e30    coh[coh > (1.0
+00018a10: 202b 2030 6a29 5d20 3d20 312e 3020 2b20   + 0j)] = 1.0 + 
+00018a20: 306a 0a20 2020 2072 6574 7572 6e20 636f  0j.    return co
+00018a30: 680a 0a0a 6465 6620 636f 6d70 7574 6545  h...def computeE
+00018a40: 7272 6f72 4675 6e63 7469 6f6e 2875 312c  rrorFunction(u1,
+00018a50: 2075 302c 206e 5361 6d70 6c65 2c20 6c61   u0, nSample, la
+00018a60: 672c 206e 6f72 6d3d 224c 3222 293a 0a20  g, norm="L2"):. 
+00018a70: 2020 2022 2222 0a20 2020 2063 6f6d 7075     """.    compu
+00018a80: 7465 2045 7272 6f72 2046 756e 6374 696f  te Error Functio
+00018a90: 6e20 7573 6564 2069 6e20 4454 572e 2054  n used in DTW. T
+00018aa0: 6865 2065 7272 6f72 2066 756e 6374 696f  he error functio
+00018ab0: 6e20 6973 2065 7175 6174 696f 6e20 3120  n is equation 1 
+00018ac0: 696e 2048 616c 652c 2032 3031 332e 2059  in Hale, 2013. Y
+00018ad0: 6f75 2063 6f75 6c64 2075 6e63 6f6d 6d65  ou could uncomme
+00018ae0: 6e74 2074 6865 0a20 2020 204c 3120 6e6f  nt the.    L1 no
+00018af0: 726d 2061 6e64 2063 6f6d 6d65 6e74 2074  rm and comment t
+00018b00: 6865 204c 3220 6e6f 726d 2069 6620 796f  he L2 norm if yo
+00018b10: 7520 7761 6e74 206f 6e20 4c69 6e65 2032  u want on Line 2
+00018b20: 390a 0a20 2020 2050 6172 616d 6574 6572  9..    Parameter
+00018b30: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00018b40: 2d2d 2d2d 0a20 2020 2075 313a 2020 7472  ----.    u1:  tr
+00018b50: 6163 6520 7468 6174 2077 6520 7761 6e74  ace that we want
+00018b60: 2074 6f20 7761 7270 3b20 7369 7a65 203d   to warp; size =
+00018b70: 2028 6e73 616d 702c 3129 0a20 2020 2075   (nsamp,1).    u
+00018b80: 303a 2020 7265 6665 7265 6e63 6520 7472  0:  reference tr
+00018b90: 6163 6520 746f 2063 6f6d 7061 7265 2077  ace to compare w
+00018ba0: 6974 683a 2073 697a 6520 3d20 286e 7361  ith: size = (nsa
+00018bb0: 6d70 2c31 290a 2020 2020 6e53 616d 706c  mp,1).    nSampl
+00018bc0: 653a 206e 756d 6572 206f 6620 706f 696e  e: numer of poin
+00018bd0: 7473 2074 6f20 636f 6d70 6172 6520 696e  ts to compare in
+00018be0: 2074 6865 2074 7261 6365 730a 2020 2020   the traces.    
+00018bf0: 6c61 673a 206d 6178 696d 756d 206c 6167  lag: maximum lag
+00018c00: 2069 6e20 7361 6d70 6c65 206e 756d 6265   in sample numbe
+00018c10: 7220 746f 2073 6561 7263 680a 2020 2020  r to search.    
+00018c20: 6e6f 726d 3a20 274c 3227 206f 7220 274c  norm: 'L2' or 'L
+00018c30: 3127 2028 6465 6661 756c 7420 6973 2027  1' (default is '
+00018c40: 4c32 2729 0a0a 2020 2020 5245 5455 524e  L2')..    RETURN
+00018c50: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00018c60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6572  ---------.    er
+00018c70: 723a 2074 6865 2032 4420 6572 726f 7220  r: the 2D error 
+00018c80: 6675 6e63 7469 6f6e 3b20 7369 7a65 203d  function; size =
+00018c90: 2028 6e73 616d 702c 322a 6c61 672b 3129   (nsamp,2*lag+1)
+00018ca0: 0a0a 2020 2020 4f72 6967 696e 616c 2062  ..    Original b
+00018cb0: 7920 4469 2059 616e 670a 2020 2020 4c61  y Di Yang.    La
+00018cc0: 7374 206d 6f64 6966 6965 6420 6279 2044  st modified by D
+00018cd0: 796c 616e 204d 696b 6573 656c 6c20 2832  ylan Mikesell (2
+00018ce0: 3520 4665 622e 2032 3031 3529 0a20 2020  5 Feb. 2015).   
+00018cf0: 2054 7261 6e73 6c61 7465 6420 746f 2070   Translated to p
+00018d00: 7974 686f 6e20 6279 2054 696d 2043 6c65  ython by Tim Cle
+00018d10: 6d65 6e74 7320 2831 3720 4175 672e 2032  ments (17 Aug. 2
+00018d20: 3031 3829 0a0a 2020 2020 2222 220a 0a20  018)..    """.. 
+00018d30: 2020 2069 6620 6c61 6720 3e3d 206e 5361     if lag >= nSa
+00018d40: 6d70 6c65 3a0a 2020 2020 2020 2020 7261  mple:.        ra
+00018d50: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00018d60: 636f 6d70 7574 6545 7272 6f72 4675 6e63  computeErrorFunc
+00018d70: 7469 6f6e 3a6c 6167 5072 6f62 6c65 6d22  tion:lagProblem"
+00018d80: 2c20 226c 6167 206d 7573 7420 6265 2073  , "lag must be s
+00018d90: 6d61 6c6c 6572 2074 6861 6e20 6e53 616d  maller than nSam
+00018da0: 706c 6522 290a 0a20 2020 2023 2041 6c6c  ple")..    # All
+00018db0: 6f63 6174 6520 6572 726f 7220 6675 6e63  ocate error func
+00018dc0: 7469 6f6e 2076 6172 6961 626c 650a 2020  tion variable.  
+00018dd0: 2020 6572 7220 3d20 6e70 2e7a 6572 6f73    err = np.zeros
+00018de0: 285b 6e53 616d 706c 652c 2032 202a 206c  ([nSample, 2 * l
+00018df0: 6167 202b 2031 5d29 0a0a 2020 2020 2320  ag + 1])..    # 
+00018e00: 696e 6974 6961 6c20 6572 726f 7220 6361  initial error ca
+00018e10: 6c63 756c 6174 696f 6e0a 2020 2020 2320  lculation.    # 
+00018e20: 6c6f 6f70 206f 7665 7220 6c61 6773 0a20  loop over lags. 
+00018e30: 2020 2066 6f72 206c 6c20 696e 206e 702e     for ll in np.
+00018e40: 6172 616e 6765 282d 6c61 672c 206c 6167  arange(-lag, lag
+00018e50: 202b 2031 293a 0a20 2020 2020 2020 2074   + 1):.        t
+00018e60: 6869 734c 6167 203d 206c 6c20 2b20 6c61  hisLag = ll + la
+00018e70: 670a 0a20 2020 2020 2020 2023 206c 6f6f  g..        # loo
+00018e80: 7020 6f76 6572 2073 616d 706c 6573 0a20  p over samples. 
+00018e90: 2020 2020 2020 2066 6f72 2069 6920 696e         for ii in
+00018ea0: 2072 616e 6765 286e 5361 6d70 6c65 293a   range(nSample):
+00018eb0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00018ec0: 6b69 7020 636f 726e 6572 7320 666f 7220  kip corners for 
+00018ed0: 6e6f 772c 2077 6520 7769 6c6c 2063 6f6d  now, we will com
+00018ee0: 6520 6261 636b 2074 6f20 7468 6573 650a  e back to these.
+00018ef0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00018f00: 6969 202b 206c 6c20 3e3d 2030 2920 2620  ii + ll >= 0) & 
+00018f10: 2869 6920 2b20 6c6c 203c 206e 5361 6d70  (ii + ll < nSamp
+00018f20: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00018f30: 2020 2020 2065 7272 5b69 692c 2074 6869       err[ii, thi
+00018f40: 734c 6167 5d20 3d20 7531 5b69 695d 202d  sLag] = u1[ii] -
+00018f50: 2075 305b 6969 202b 206c 6c5d 0a0a 2020   u0[ii + ll]..  
+00018f60: 2020 6966 206e 6f72 6d20 3d3d 2022 4c32    if norm == "L2
+00018f70: 223a 0a20 2020 2020 2020 2065 7272 203d  ":.        err =
+00018f80: 2065 7272 2a2a 320a 2020 2020 656c 6966   err**2.    elif
+00018f90: 206e 6f72 6d20 3d3d 2022 4c31 223a 0a20   norm == "L1":. 
+00018fa0: 2020 2020 2020 2065 7272 203d 206e 702e         err = np.
+00018fb0: 6162 7328 6572 7229 0a0a 2020 2020 2320  abs(err)..    # 
+00018fc0: 4e6f 7720 6669 7820 636f 726e 6572 7320  Now fix corners 
+00018fd0: 7769 7468 2063 6f6e 7374 616e 7420 6578  with constant ex
+00018fe0: 7472 6170 6f6c 6174 696f 6e0a 2020 2020  trapolation.    
+00018ff0: 666f 7220 6c6c 2069 6e20 6e70 2e61 7261  for ll in np.ara
+00019000: 6e67 6528 2d6c 6167 2c20 6c61 6720 2b20  nge(-lag, lag + 
+00019010: 3129 3a0a 2020 2020 2020 2020 7468 6973  1):.        this
+00019020: 4c61 6720 3d20 6c6c 202b 206c 6167 0a0a  Lag = ll + lag..
+00019030: 2020 2020 2020 2020 666f 7220 6969 2069          for ii i
+00019040: 6e20 7261 6e67 6528 6e53 616d 706c 6529  n range(nSample)
+00019050: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00019060: 2069 6920 2b20 6c6c 203c 2030 3a0a 2020   ii + ll < 0:.  
+00019070: 2020 2020 2020 2020 2020 2020 2020 6572                er
+00019080: 725b 6969 2c20 7468 6973 4c61 675d 203d  r[ii, thisLag] =
+00019090: 2065 7272 5b2d 6c6c 2c20 7468 6973 4c61   err[-ll, thisLa
+000190a0: 675d 0a0a 2020 2020 2020 2020 2020 2020  g]..            
+000190b0: 656c 6966 2069 6920 2b20 6c6c 203e 206e  elif ii + ll > n
+000190c0: 5361 6d70 6c65 202d 2031 3a0a 2020 2020  Sample - 1:.    
+000190d0: 2020 2020 2020 2020 2020 2020 6572 725b              err[
+000190e0: 6969 2c20 7468 6973 4c61 675d 203d 2065  ii, thisLag] = e
+000190f0: 7272 5b6e 5361 6d70 6c65 202d 206c 6c20  rr[nSample - ll 
+00019100: 2d20 312c 2074 6869 734c 6167 5d0a 0a20  - 1, thisLag].. 
+00019110: 2020 2072 6574 7572 6e20 6572 720a 0a0a     return err...
+00019120: 6465 6620 6163 6375 6d75 6c61 7465 4572  def accumulateEr
+00019130: 726f 7246 756e 6374 696f 6e28 6469 722c  rorFunction(dir,
+00019140: 2065 7272 2c20 6e53 616d 706c 652c 206c   err, nSample, l
+00019150: 6167 2c20 6229 3a0a 2020 2020 2222 220a  ag, b):.    """.
+00019160: 2020 2020 6163 6375 6d75 6c61 7469 6f6e      accumulation
+00019170: 206f 6620 7468 6520 6572 726f 722c 2077   of the error, w
+00019180: 6869 6368 2066 6f6c 6c6f 7773 2074 6865  hich follows the
+00019190: 2065 7175 6174 696f 6e20 3620 696e 2048   equation 6 in H
+000191a0: 616c 652c 2032 3031 332e 0a0a 2020 2020  ale, 2013...    
+000191b0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000191c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+000191d0: 2020 6469 723a 2061 6363 756d 756c 6174    dir: accumulat
+000191e0: 696f 6e20 6469 7265 6374 696f 6e20 2820  ion direction ( 
+000191f0: 6469 7220 3e20 3020 3d20 666f 7277 6172  dir > 0 = forwar
+00019200: 6420 696e 2074 696d 652c 2064 6972 203c  d in time, dir <
+00019210: 3d20 3020 3d20 6261 636b 7761 7264 2069  = 0 = backward i
+00019220: 6e20 7469 6d65 290a 2020 2020 6572 723a  n time).    err:
+00019230: 2074 6865 2032 4420 6572 726f 7220 6675   the 2D error fu
+00019240: 6e63 7469 6f6e 3b20 7369 7a65 203d 2028  nction; size = (
+00019250: 6e73 616d 702c 322a 6c61 672b 3129 0a20  nsamp,2*lag+1). 
+00019260: 2020 206e 5361 6d70 6c65 3a20 6e75 6d65     nSample: nume
+00019270: 7220 6f66 2070 6f69 6e74 7320 746f 2063  r of points to c
+00019280: 6f6d 7061 7265 2069 6e20 7468 6520 7472  ompare in the tr
+00019290: 6163 6573 0a20 2020 206c 6167 3a20 6d61  aces.    lag: ma
+000192a0: 7869 6d75 6d20 6c61 6720 696e 2073 616d  ximum lag in sam
+000192b0: 706c 6520 6e75 6d62 6572 2074 6f20 7365  ple number to se
+000192c0: 6172 6368 0a20 2020 2062 3a20 7374 7261  arch.    b: stra
+000192d0: 696e 206c 696d 6974 2028 696e 7465 6765  in limit (intege
+000192e0: 7220 7661 6c75 6520 3e3d 2031 290a 0a20  r value >= 1).. 
+000192f0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+00019300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019310: 2d2d 0a20 2020 2064 3a20 7468 6520 3244  --.    d: the 2D
+00019320: 2064 6973 7461 6e63 6520 6675 6e63 7469   distance functi
+00019330: 6f6e 3b20 7369 7a65 203d 2028 6e73 616d  on; size = (nsam
+00019340: 702c 322a 6c61 672b 3129 0a0a 2020 2020  p,2*lag+1)..    
+00019350: 4f72 6967 696e 616c 2062 7920 4469 2059  Original by Di Y
+00019360: 616e 670a 2020 2020 4c61 7374 206d 6f64  ang.    Last mod
+00019370: 6966 6965 6420 6279 2044 796c 616e 204d  ified by Dylan M
+00019380: 696b 6573 656c 6c20 2832 3520 4665 622e  ikesell (25 Feb.
+00019390: 2032 3031 3529 0a20 2020 2054 7261 6e73   2015).    Trans
+000193a0: 6c61 7465 6420 746f 2070 7974 686f 6e20  lated to python 
+000193b0: 6279 2054 696d 2043 6c65 6d65 6e74 7320  by Tim Clements 
+000193c0: 2831 3720 4175 672e 2032 3031 3829 0a0a  (17 Aug. 2018)..
+000193d0: 2020 2020 2222 220a 0a20 2020 2023 206e      """..    # n
+000193e0: 756d 6265 7220 6f66 206c 6167 7320 6672  umber of lags fr
+000193f0: 6f6d 205b 202d 6c61 6720 3a20 2b6c 6167  om [ -lag : +lag
+00019400: 205d 0a20 2020 206e 4c61 6720 3d20 2832   ].    nLag = (2
+00019410: 202a 206c 6167 2920 2b20 310a 0a20 2020   * lag) + 1..   
+00019420: 2023 2061 6c6c 6f63 6174 6520 6469 7374   # allocate dist
+00019430: 616e 6365 206d 6174 7269 780a 2020 2020  ance matrix.    
+00019440: 6420 3d20 6e70 2e7a 6572 6f73 285b 6e53  d = np.zeros([nS
+00019450: 616d 706c 652c 206e 4c61 675d 290a 0a20  ample, nLag]).. 
+00019460: 2020 2023 2053 6574 7570 2069 6e64 6963     # Setup indic
+00019470: 6573 2062 6173 6564 206f 6e20 666f 7277  es based on forw
+00019480: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
+00019490: 6163 6375 6d75 6c61 7469 6f6e 2064 6972  accumulation dir
+000194a0: 6563 7469 6f6e 0a20 2020 2069 6620 6469  ection.    if di
+000194b0: 7220 3e20 303a 2020 2320 464f 5257 4152  r > 0:  # FORWAR
+000194c0: 440a 2020 2020 2020 2020 6942 6567 696e  D.        iBegin
+000194d0: 2c20 6945 6e64 2c20 6949 6e63 203d 2030  , iEnd, iInc = 0
+000194e0: 2c20 6e53 616d 706c 6520 2d20 312c 2031  , nSample - 1, 1
+000194f0: 0a20 2020 2065 6c73 653a 2020 2320 4241  .    else:  # BA
+00019500: 434b 5741 5244 0a20 2020 2020 2020 2069  CKWARD.        i
+00019510: 4265 6769 6e2c 2069 456e 642c 2069 496e  Begin, iEnd, iIn
+00019520: 6320 3d20 6e53 616d 706c 6520 2d20 312c  c = nSample - 1,
+00019530: 2030 2c20 2d31 0a0a 2020 2020 2320 4c6f   0, -1..    # Lo
+00019540: 6f70 2074 6872 6f75 6768 2061 6c6c 2074  op through all t
+00019550: 696d 6573 2069 6920 696e 2066 6f72 7761  imes ii in forwa
+00019560: 7264 206f 7220 6261 636b 7761 7264 2064  rd or backward d
+00019570: 6972 6563 7469 6f6e 0a20 2020 2066 6f72  irection.    for
+00019580: 2069 6920 696e 2072 616e 6765 2869 4265   ii in range(iBe
+00019590: 6769 6e2c 2069 456e 6420 2b20 6949 6e63  gin, iEnd + iInc
+000195a0: 2c20 6949 6e63 293a 0a20 2020 2020 2020  , iInc):.       
+000195b0: 2023 206d 696e 2f6d 6178 2074 6f20 6163   # min/max to ac
+000195c0: 636f 756e 7420 666f 7220 7468 6520 6564  count for the ed
+000195d0: 6765 732f 626f 756e 6461 7269 6573 0a20  ges/boundaries. 
+000195e0: 2020 2020 2020 206a 6920 3d20 6d61 7828         ji = max(
+000195f0: 5b30 2c20 6d69 6e28 5b6e 5361 6d70 6c65  [0, min([nSample
+00019600: 202d 2031 2c20 6969 202d 2069 496e 635d   - 1, ii - iInc]
+00019610: 295d 290a 2020 2020 2020 2020 6a62 203d  )]).        jb =
+00019620: 206d 6178 285b 302c 206d 696e 285b 6e53   max([0, min([nS
+00019630: 616d 706c 6520 2d20 312c 2069 6920 2d20  ample - 1, ii - 
+00019640: 6949 6e63 202a 2062 5d29 5d29 0a0a 2020  iInc * b])])..  
+00019650: 2020 2020 2020 2320 6c6f 6f70 2074 6872        # loop thr
+00019660: 6f75 6768 2061 6c6c 206c 6167 0a20 2020  ough all lag.   
+00019670: 2020 2020 2066 6f72 206c 6c20 696e 2072       for ll in r
+00019680: 616e 6765 286e 4c61 6729 3a0a 2020 2020  ange(nLag):.    
+00019690: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+000196a0: 6c69 6d69 7473 206f 6e20 6c61 6720 696e  limits on lag in
+000196b0: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
+000196c0: 2020 6c4d 696e 7573 3120 3d20 6c6c 202d    lMinus1 = ll -
+000196d0: 2031 0a0a 2020 2020 2020 2020 2020 2020   1..            
+000196e0: 2320 6368 6563 6b20 6c61 6720 696e 6465  # check lag inde
+000196f0: 7820 6973 2067 7265 6174 6572 2074 6861  x is greater tha
+00019700: 6e20 300a 2020 2020 2020 2020 2020 2020  n 0.            
+00019710: 6966 206c 4d69 6e75 7331 203c 2030 3a0a  if lMinus1 < 0:.
+00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019730: 6c4d 696e 7573 3120 3d20 3020 2023 206d  lMinus1 = 0  # m
+00019740: 616b 6520 6c61 6720 3d20 6669 7273 7420  ake lag = first 
+00019750: 6c61 670a 0a20 2020 2020 2020 2020 2020  lag..           
+00019760: 206c 506c 7573 3120 3d20 6c6c 202b 2031   lPlus1 = ll + 1
+00019770: 2020 2320 6c61 6720 6174 206c 2b31 0a0a    # lag at l+1..
+00019780: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
+00019790: 6563 6b20 6c61 6720 696e 6465 7820 6c65  eck lag index le
+000197a0: 7373 2074 6861 6e20 6d61 7820 6c61 670a  ss than max lag.
+000197b0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000197c0: 506c 7573 3120 3e20 6e4c 6167 202d 2031  Plus1 > nLag - 1
+000197d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000197e0: 2020 6c50 6c75 7331 203d 206e 4c61 6720    lPlus1 = nLag 
+000197f0: 2d20 310a 0a20 2020 2020 2020 2020 2020  - 1..           
+00019800: 2023 2067 6574 2064 6973 7461 6e63 6520   # get distance 
+00019810: 6174 206c 6167 7320 286c 6c2d 312c 206c  at lags (ll-1, l
+00019820: 6c2c 206c 6c2b 3129 0a20 2020 2020 2020  l, ll+1).       
+00019830: 2020 2020 2064 6973 744c 6d69 6e75 7331       distLminus1
+00019840: 203d 2064 5b6a 622c 206c 4d69 6e75 7331   = d[jb, lMinus1
+00019850: 5d20 2023 206d 696e 7573 3a20 2064 5b69  ]  # minus:  d[i
+00019860: 2d62 2c20 6a2d 315d 0a20 2020 2020 2020  -b, j-1].       
+00019870: 2020 2020 2064 6973 744c 203d 2064 5b6a       distL = d[j
+00019880: 692c 206c 6c5d 2020 2320 6163 7475 616c  i, ll]  # actual
+00019890: 2064 5b69 2d31 2c20 6a5d 0a20 2020 2020   d[i-1, j].     
+000198a0: 2020 2020 2020 2064 6973 744c 706c 7573         distLplus
+000198b0: 3120 3d20 645b 6a62 2c20 6c50 6c75 7331  1 = d[jb, lPlus1
+000198c0: 5d20 2023 2070 6c75 7320 645b 692d 622c  ]  # plus d[i-b,
+000198d0: 206a 2b31 5d0a 0a20 2020 2020 2020 2020   j+1]..         
+000198e0: 2020 2069 6620 6a69 2021 3d20 6a62 3a20     if ji != jb: 
+000198f0: 2023 2065 7175 6174 696f 6e20 3130 2069   # equation 10 i
+00019900: 6e20 4861 6c65 2c20 3230 3133 0a20 2020  n Hale, 2013.   
+00019910: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00019920: 206b 6220 696e 2072 616e 6765 286a 692c   kb in range(ji,
+00019930: 206a 6220 2b20 6949 6e63 202d 2031 2c20   jb + iInc - 1, 
+00019940: 2d69 496e 6329 3a0a 2020 2020 2020 2020  -iInc):.        
+00019950: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+00019960: 4c6d 696e 7573 3120 3d20 6469 7374 4c6d  Lminus1 = distLm
+00019970: 696e 7573 3120 2b20 6572 725b 6b62 2c20  inus1 + err[kb, 
+00019980: 6c4d 696e 7573 315d 0a20 2020 2020 2020  lMinus1].       
+00019990: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000199a0: 744c 706c 7573 3120 3d20 6469 7374 4c70  tLplus1 = distLp
+000199b0: 6c75 7331 202b 2065 7272 5b6b 622c 206c  lus1 + err[kb, l
+000199c0: 506c 7573 315d 0a0a 2020 2020 2020 2020  Plus1]..        
+000199d0: 2020 2020 2320 6571 7561 7469 6f6e 2036      # equation 6
+000199e0: 2028 6966 2062 3d31 2920 6f72 2031 3020   (if b=1) or 10 
+000199f0: 2869 6620 623e 3129 2069 6e20 4861 6c65  (if b>1) in Hale
+00019a00: 2028 3230 3133 2920 6166 7465 7220 7472   (2013) after tr
+00019a10: 6561 7469 6e67 2062 6f75 6e64 6172 6965  eating boundarie
+00019a20: 730a 2020 2020 2020 2020 2020 2020 645b  s.            d[
+00019a30: 6969 2c20 6c6c 5d20 3d20 6572 725b 6969  ii, ll] = err[ii
+00019a40: 2c20 6c6c 5d20 2b20 6d69 6e28 5b64 6973  , ll] + min([dis
+00019a50: 744c 6d69 6e75 7331 2c20 6469 7374 4c2c  tLminus1, distL,
+00019a60: 2064 6973 744c 706c 7573 315d 290a 0a20   distLplus1]).. 
+00019a70: 2020 2072 6574 7572 6e20 640a 0a0a 6465     return d...de
+00019a80: 6620 6261 636b 7472 6163 6b44 6973 7461  f backtrackDista
+00019a90: 6e63 6546 756e 6374 696f 6e28 6469 722c  nceFunction(dir,
+00019aa0: 2064 2c20 6572 722c 206c 6d69 6e2c 2062   d, err, lmin, b
+00019ab0: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+00019ac0: 6865 2066 756e 6374 696f 6e20 6973 2065  he function is e
+00019ad0: 7175 6174 696f 6e20 3220 696e 2048 616c  quation 2 in Hal
+00019ae0: 652c 2032 3031 332e 0a0a 2020 2020 5061  e, 2013...    Pa
+00019af0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00019b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00019b10: 6469 723a 2073 6964 6520 746f 2073 7461  dir: side to sta
+00019b20: 7274 206d 696e 696d 697a 6174 696f 6e20  rt minimization 
+00019b30: 2820 6469 7220 3e20 3020 3d20 6672 6f6e  ( dir > 0 = fron
+00019b40: 742c 2064 6972 203c 3d20 3020 3d20 2062  t, dir <= 0 =  b
+00019b50: 6163 6b29 0a20 2020 2064 203a 2074 6865  ack).    d : the
+00019b60: 2032 4420 6469 7374 616e 6365 2066 756e   2D distance fun
+00019b70: 6374 696f 6e3b 2073 697a 6520 3d20 286e  ction; size = (n
+00019b80: 7361 6d70 2c32 2a6c 6167 2b31 290a 2020  samp,2*lag+1).  
+00019b90: 2020 6572 723a 2074 6865 2032 4420 6572    err: the 2D er
+00019ba0: 726f 7220 6675 6e63 7469 6f6e 3b20 7369  ror function; si
+00019bb0: 7a65 203d 2028 6e73 616d 702c 322a 6c61  ze = (nsamp,2*la
+00019bc0: 672b 3129 0a20 2020 206c 6d69 6e3a 206d  g+1).    lmin: m
+00019bd0: 696e 696d 756d 206c 6167 2074 6f20 7365  inimum lag to se
+00019be0: 6172 6368 206f 7665 720a 2020 2020 6220  arch over.    b 
+00019bf0: 3a20 7374 7261 696e 206c 696d 6974 2028  : strain limit (
+00019c00: 696e 7465 6765 7220 7661 6c75 6520 3e3d  integer value >=
+00019c10: 2031 290a 0a20 2020 2052 4554 5552 4e53   1)..    RETURNS
+00019c20: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+00019c30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 7462  --------.    stb
+00019c40: 6172 3a20 7665 6374 6f72 206f 6620 696e  ar: vector of in
+00019c50: 7465 6765 7220 7368 6966 7473 2073 7562  teger shifts sub
+00019c60: 6a65 6374 2074 6f20 7c75 2869 292d 7528  ject to |u(i)-u(
+00019c70: 692d 3129 7c20 3c3d 2031 2f62 0a0a 2020  i-1)| <= 1/b..  
+00019c80: 2020 4f72 6967 696e 616c 2062 7920 4469    Original by Di
+00019c90: 2059 616e 670a 2020 2020 4c61 7374 206d   Yang.    Last m
+00019ca0: 6f64 6966 6965 6420 6279 2044 796c 616e  odified by Dylan
+00019cb0: 204d 696b 6573 656c 6c20 2831 3920 4465   Mikesell (19 De
+00019cc0: 632e 2032 3031 3429 0a0a 2020 2020 5472  c. 2014)..    Tr
+00019cd0: 616e 736c 6174 6564 2074 6f20 7079 7468  anslated to pyth
+00019ce0: 6f6e 2062 7920 5469 6d20 436c 656d 656e  on by Tim Clemen
+00019cf0: 7473 2028 3137 2041 7567 2e20 3230 3138  ts (17 Aug. 2018
+00019d00: 290a 0a20 2020 2022 2222 0a0a 2020 2020  )..    """..    
+00019d10: 6e53 616d 706c 652c 206e 4c61 6720 3d20  nSample, nLag = 
+00019d20: 642e 7368 6170 650a 2020 2020 7374 6261  d.shape.    stba
+00019d30: 7220 3d20 6e70 2e7a 6572 6f73 286e 5361  r = np.zeros(nSa
+00019d40: 6d70 6c65 290a 0a20 2020 2023 2053 6574  mple)..    # Set
+00019d50: 7570 2069 6e64 6963 6573 2062 6173 6564  up indices based
+00019d60: 206f 6e20 666f 7277 6172 6420 6f72 2062   on forward or b
+00019d70: 6163 6b77 6172 6420 6163 6375 6d75 6c61  ackward accumula
+00019d80: 7469 6f6e 2064 6972 6563 7469 6f6e 0a20  tion direction. 
+00019d90: 2020 2069 6620 6469 7220 3e20 303a 2020     if dir > 0:  
+00019da0: 2320 464f 5257 4152 440a 2020 2020 2020  # FORWARD.      
+00019db0: 2020 6942 6567 696e 2c20 6945 6e64 2c20    iBegin, iEnd, 
+00019dc0: 6949 6e63 203d 2030 2c20 6e53 616d 706c  iInc = 0, nSampl
+00019dd0: 6520 2d20 312c 2031 0a20 2020 2065 6c73  e - 1, 1.    els
+00019de0: 653a 2020 2320 4241 434b 5741 5244 0a20  e:  # BACKWARD. 
+00019df0: 2020 2020 2020 2069 4265 6769 6e2c 2069         iBegin, i
+00019e00: 456e 642c 2069 496e 6320 3d20 6e53 616d  End, iInc = nSam
+00019e10: 706c 6520 2d20 312c 2030 2c20 2d31 0a0a  ple - 1, 0, -1..
+00019e20: 2020 2020 2320 7374 6172 7420 6672 6f6d      # start from
+00019e30: 2074 6865 2065 6e64 2028 6672 6f6e 7420   the end (front 
+00019e40: 6f72 2062 6163 6b29 0a20 2020 206c 6c20  or back).    ll 
+00019e50: 3d20 6e70 2e61 7267 6d69 6e28 645b 6942  = np.argmin(d[iB
+00019e60: 6567 696e 2c20 3a5d 2920 2023 2066 696e  egin, :])  # fin
+00019e70: 6420 6d69 6e69 6d75 6d20 6163 6375 6d75  d minimum accumu
+00019e80: 6c61 7465 6420 6469 7374 616e 6365 2061  lated distance a
+00019e90: 7420 6672 6f6e 7420 6f72 2062 6163 6b20  t front or back 
+00019ea0: 6465 7065 6e64 696e 6720 6f6e 2027 6469  depending on 'di
+00019eb0: 7227 0a20 2020 2073 7462 6172 5b69 4265  r'.    stbar[iBe
+00019ec0: 6769 6e5d 203d 206c 6c20 2b20 6c6d 696e  gin] = ll + lmin
+00019ed0: 2020 2320 6162 736f 6c75 7465 2076 616c    # absolute val
+00019ee0: 7565 206f 6620 696e 7465 6765 7220 7368  ue of integer sh
+00019ef0: 6966 740a 0a20 2020 2023 206d 6f76 6520  ift..    # move 
+00019f00: 7468 726f 7567 6820 616c 6c20 7469 6d65  through all time
+00019f10: 2073 616d 706c 6573 2069 6e20 666f 7277   samples in forw
+00019f20: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
+00019f30: 6469 7265 6374 696f 6e0a 2020 2020 6969  direction.    ii
+00019f40: 203d 2069 4265 6769 6e0a 0a20 2020 2077   = iBegin..    w
+00019f50: 6869 6c65 2069 6920 213d 2069 456e 643a  hile ii != iEnd:
+00019f60: 0a20 2020 2020 2020 2023 206d 696e 2f6d  .        # min/m
+00019f70: 6178 2066 6f72 2065 6467 6573 2f62 6f75  ax for edges/bou
+00019f80: 6e64 6172 6965 730a 2020 2020 2020 2020  ndaries.        
+00019f90: 6a69 203d 206e 702e 6d61 7828 5b30 2c20  ji = np.max([0, 
+00019fa0: 6e70 2e6d 696e 285b 6e53 616d 706c 6520  np.min([nSample 
+00019fb0: 2d20 312c 2069 6920 2b20 6949 6e63 5d29  - 1, ii + iInc])
+00019fc0: 5d29 0a20 2020 2020 2020 206a 6220 3d20  ]).        jb = 
+00019fd0: 6e70 2e6d 6178 285b 302c 206e 702e 6d69  np.max([0, np.mi
+00019fe0: 6e28 5b6e 5361 6d70 6c65 202d 2031 2c20  n([nSample - 1, 
+00019ff0: 6969 202b 2069 496e 6320 2a20 625d 295d  ii + iInc * b])]
+0001a000: 290a 0a20 2020 2020 2020 2023 2063 6865  )..        # che
+0001a010: 636b 206c 696d 6974 7320 6f6e 206c 6167  ck limits on lag
+0001a020: 2069 6e64 6963 6573 0a20 2020 2020 2020   indices.       
+0001a030: 206c 4d69 6e75 7331 203d 206c 6c20 2d20   lMinus1 = ll - 
+0001a040: 310a 0a20 2020 2020 2020 2069 6620 6c4d  1..        if lM
+0001a050: 696e 7573 3120 3c20 303a 2020 2320 6368  inus1 < 0:  # ch
+0001a060: 6563 6b20 6c61 6720 696e 6465 7820 6973  eck lag index is
+0001a070: 2067 7265 6174 6572 2074 6861 6e20 310a   greater than 1.
+0001a080: 2020 2020 2020 2020 2020 2020 6c4d 696e              lMin
+0001a090: 7573 3120 3d20 3020 2023 206d 616b 6520  us1 = 0  # make 
+0001a0a0: 6c61 6720 3d20 6669 7273 7420 6c61 670a  lag = first lag.
+0001a0b0: 0a20 2020 2020 2020 206c 506c 7573 3120  .        lPlus1 
+0001a0c0: 3d20 6c6c 202b 2031 0a0a 2020 2020 2020  = ll + 1..      
+0001a0d0: 2020 6966 206c 506c 7573 3120 3e20 6e4c    if lPlus1 > nL
+0001a0e0: 6167 202d 2031 3a20 2023 2063 6865 636b  ag - 1:  # check
+0001a0f0: 206c 6167 2069 6e64 6578 206c 6573 7320   lag index less 
+0001a100: 7468 616e 206d 6178 206c 6167 0a20 2020  than max lag.   
+0001a110: 2020 2020 2020 2020 206c 506c 7573 3120           lPlus1 
+0001a120: 3d20 6e4c 6167 202d 2031 0a0a 2020 2020  = nLag - 1..    
+0001a130: 2020 2020 2320 6765 7420 6469 7374 616e      # get distan
+0001a140: 6365 2061 7420 6c61 6773 2028 6c6c 2d31  ce at lags (ll-1
+0001a150: 2c20 6c6c 2c20 6c6c 2b31 290a 2020 2020  , ll, ll+1).    
+0001a160: 2020 2020 6469 7374 4c6d 696e 7573 3120      distLminus1 
+0001a170: 3d20 645b 6a62 2c20 6c4d 696e 7573 315d  = d[jb, lMinus1]
+0001a180: 2020 2320 6d69 6e75 733a 2020 645b 692d    # minus:  d[i-
+0001a190: 622c 206a 2d31 5d0a 2020 2020 2020 2020  b, j-1].        
+0001a1a0: 6469 7374 4c20 3d20 645b 6a69 2c20 6c6c  distL = d[ji, ll
+0001a1b0: 5d20 2023 2061 6374 7561 6c20 645b 692d  ]  # actual d[i-
+0001a1c0: 312c 206a 5d0a 2020 2020 2020 2020 6469  1, j].        di
+0001a1d0: 7374 4c70 6c75 7331 203d 2064 5b6a 622c  stLplus1 = d[jb,
+0001a1e0: 206c 506c 7573 315d 2020 2320 706c 7573   lPlus1]  # plus
+0001a1f0: 2064 5b69 2d62 2c20 6a2b 315d 0a0a 2020   d[i-b, j+1]..  
+0001a200: 2020 2020 2020 2320 6571 7561 7469 6f6e        # equation
+0001a210: 2031 3020 696e 2048 616c 6520 2832 3031   10 in Hale (201
+0001a220: 3329 0a20 2020 2020 2020 2023 2073 756d  3).        # sum
+0001a230: 2065 7272 6f72 7320 6f76 6572 2069 2d31   errors over i-1
+0001a240: 3a69 2d62 2b31 0a20 2020 2020 2020 2069  :i-b+1.        i
+0001a250: 6620 6a69 2021 3d20 6a62 3a0a 2020 2020  f ji != jb:.    
+0001a260: 2020 2020 2020 2020 666f 7220 6b62 2069          for kb i
+0001a270: 6e20 7261 6e67 6528 6a69 2c20 6a62 202d  n range(ji, jb -
+0001a280: 2069 496e 6320 2d20 312c 2069 496e 6329   iInc - 1, iInc)
+0001a290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a2a0: 2020 6469 7374 4c6d 696e 7573 3120 3d20    distLminus1 = 
+0001a2b0: 6469 7374 4c6d 696e 7573 3120 2b20 6572  distLminus1 + er
+0001a2c0: 725b 6b62 2c20 6c4d 696e 7573 315d 0a20  r[kb, lMinus1]. 
+0001a2d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001a2e0: 6973 744c 706c 7573 3120 3d20 6469 7374  istLplus1 = dist
+0001a2f0: 4c70 6c75 7331 202b 2065 7272 5b6b 622c  Lplus1 + err[kb,
+0001a300: 206c 506c 7573 315d 0a0a 2020 2020 2020   lPlus1]..      
+0001a310: 2020 2320 7570 6461 7465 206d 696e 696d    # update minim
+0001a320: 756d 2064 6973 7461 6e63 6520 746f 2070  um distance to p
+0001a330: 7265 7669 6f75 7320 7361 6d70 6c65 0a20  revious sample. 
+0001a340: 2020 2020 2020 2064 6c20 3d20 6e70 2e6d         dl = np.m
+0001a350: 696e 285b 6469 7374 4c6d 696e 7573 312c  in([distLminus1,
+0001a360: 2064 6973 744c 2c20 6469 7374 4c70 6c75   distL, distLplu
+0001a370: 7331 5d29 0a0a 2020 2020 2020 2020 6966  s1])..        if
+0001a380: 2064 6c20 213d 2064 6973 744c 3a20 2023   dl != distL:  #
+0001a390: 2074 6865 6e20 6c6c 207e 3d20 6c6c 2061   then ll ~= ll a
+0001a3a0: 6e64 2077 6520 6368 6563 6b20 666f 7277  nd we check forw
+0001a3b0: 6172 6420 616e 6420 6261 636b 7761 7264  ard and backward
+0001a3c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a3d0: 646c 203d 3d20 6469 7374 4c6d 696e 7573  dl == distLminus
+0001a3e0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0001a3f0: 2020 206c 6c20 3d20 6c4d 696e 7573 310a     ll = lMinus1.
+0001a400: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001a410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a420: 2020 6c6c 203d 206c 506c 7573 310a 0a20    ll = lPlus1.. 
+0001a430: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
+0001a440: 6969 203d 2069 6920 2d20 310a 2020 2020  ii = ii - 1.    
+0001a450: 2020 2020 6969 202b 3d20 6949 6e63 0a0a      ii += iInc..
+0001a460: 2020 2020 2020 2020 2320 6162 736f 6c75          # absolu
+0001a470: 7465 2069 6e74 6567 6572 206f 6620 6c61  te integer of la
+0001a480: 670a 2020 2020 2020 2020 7374 6261 725b  g.        stbar[
+0001a490: 6969 5d20 3d20 6c6c 202b 206c 6d69 6e0a  ii] = ll + lmin.
+0001a4a0: 0a20 2020 2020 2020 2023 206e 6f77 206d  .        # now m
+0001a4b0: 6f76 6520 746f 2063 6f72 7265 6374 2074  ove to correct t
+0001a4c0: 696d 6520 696e 6465 782c 2069 6620 736d  ime index, if sm
+0001a4d0: 6f6f 7468 696e 6720 6469 6666 6572 656e  oothing differen
+0001a4e0: 6365 206f 7665 7220 6d61 6e79 0a20 2020  ce over many.   
+0001a4f0: 2020 2020 2023 2074 696d 6520 7361 6d70       # time samp
+0001a500: 6c65 7320 7573 696e 6720 2762 270a 2020  les using 'b'.  
+0001a510: 2020 2020 2020 6966 2028 6c6c 203d 3d20        if (ll == 
+0001a520: 6c4d 696e 7573 3129 207c 2028 6c6c 203d  lMinus1) | (ll =
+0001a530: 3d20 6c50 6c75 7331 293a 2020 2320 6368  = lPlus1):  # ch
+0001a540: 6563 6b20 6564 6765 7320 746f 2073 6565  eck edges to see
+0001a550: 2061 626f 7574 2062 2076 616c 7565 730a   about b values.
+0001a560: 2020 2020 2020 2020 2020 2020 6966 206a              if j
+0001a570: 6920 213d 206a 623a 2020 2320 6966 2062  i != jb:  # if b
+0001a580: 3e31 2074 6865 6e20 6e65 6564 2074 6f20  >1 then need to 
+0001a590: 6d6f 7665 206d 6f72 6520 7374 6570 730a  move more steps.
+0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5b0: 666f 7220 6b62 2069 6e20 7261 6e67 6528  for kb in range(
+0001a5c0: 6a69 2c20 6a62 202d 2069 496e 6320 2d20  ji, jb - iInc - 
+0001a5d0: 312c 2069 496e 6329 3a0a 2020 2020 2020  1, iInc):.      
+0001a5e0: 2020 2020 2020 2020 2020 2020 2020 6969                ii
+0001a5f0: 203d 2069 6920 2b20 6949 6e63 2020 2320   = ii + iInc  # 
+0001a600: 6d6f 7665 2066 726f 6d20 692d 313a 692d  move from i-1:i-
+0001a610: 622d 310a 2020 2020 2020 2020 2020 2020  b-1.            
+0001a620: 2020 2020 2020 2020 7374 6261 725b 6969          stbar[ii
+0001a630: 5d20 3d20 6c6c 202b 206c 6d69 6e20 2023  ] = ll + lmin  #
+0001a640: 2063 6f6e 7374 616e 7420 6c61 6720 6f76   constant lag ov
+0001a650: 6572 2074 6861 7420 7469 6d65 0a0a 2020  er that time..  
+0001a660: 2020 7265 7475 726e 2073 7462 6172 0a0a    return stbar..
+0001a670: 0a64 6566 2077 6374 5f6d 6f64 6966 6965  .def wct_modifie
+0001a680: 6428 0a20 2020 2079 312c 2079 322c 2064  d(.    y1, y2, d
+0001a690: 742c 2064 6a3d 3120 2f20 3132 2c20 7330  t, dj=1 / 12, s0
+0001a6a0: 3d2d 312c 204a 3d2d 312c 2073 6967 3d54  =-1, J=-1, sig=T
+0001a6b0: 7275 652c 2073 6967 6e69 6669 6361 6e63  rue, significanc
+0001a6c0: 655f 6c65 7665 6c3d 302e 3935 2c20 7761  e_level=0.95, wa
+0001a6d0: 7665 6c65 743d 226d 6f72 6c65 7422 2c20  velet="morlet", 
+0001a6e0: 6e6f 726d 616c 697a 653d 5472 7565 2c20  normalize=True, 
+0001a6f0: 2a2a 6b77 6172 6773 0a29 3a0a 2020 2020  **kwargs.):.    
+0001a700: 2222 220a 2020 2020 2020 2020 5761 7665  """.        Wave
+0001a710: 6c65 7420 636f 6865 7265 6e63 6520 7472  let coherence tr
+0001a720: 616e 7366 6f72 6d20 2857 4354 292e 0a20  ansform (WCT).. 
+0001a730: 2020 20e2 808b 0a20 2020 2020 2020 2054     ....        T
+0001a740: 6865 2057 4354 2066 696e 6473 2072 6567  he WCT finds reg
+0001a750: 696f 6e73 2069 6e20 7469 6d65 2066 7265  ions in time fre
+0001a760: 7175 656e 6379 2073 7061 6365 2077 6865  quency space whe
+0001a770: 7265 2074 6865 2074 776f 2074 696d 650a  re the two time.
+0001a780: 2020 2020 2020 2020 7365 7269 6573 2063          series c
+0001a790: 6f2d 7661 7279 2c20 6275 7420 646f 206e  o-vary, but do n
+0001a7a0: 6f74 206e 6563 6573 7361 7269 6c79 2068  ot necessarily h
+0001a7b0: 6176 6520 6869 6768 2070 6f77 6572 2e0a  ave high power..
+0001a7c0: 2020 2020 e280 8b0a 2020 2020 2020 2020      ....        
+0001a7d0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0001a7e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001a7f0: 2020 2020 2020 7931 2c20 7932 203a 206e        y1, y2 : n
+0001a800: 756d 7079 2e6e 6461 7272 6179 2c20 6c69  umpy.ndarray, li
+0001a810: 7374 0a20 2020 2020 2020 2020 2020 2049  st.            I
+0001a820: 6e70 7574 2073 6967 6e61 6c73 2e0a 2020  nput signals..  
+0001a830: 2020 2020 2020 6474 203a 2066 6c6f 6174        dt : float
+0001a840: 0a20 2020 2020 2020 2020 2020 2053 616d  .            Sam
+0001a850: 706c 6520 7370 6163 696e 672e 0a20 2020  ple spacing..   
+0001a860: 2020 2020 2064 6a20 3a20 666c 6f61 742c       dj : float,
+0001a870: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0001a880: 2020 2020 2020 5370 6163 696e 6720 6265        Spacing be
+0001a890: 7477 6565 6e20 6469 7363 7265 7465 2073  tween discrete s
+0001a8a0: 6361 6c65 732e 2044 6566 6175 6c74 2076  cales. Default v
+0001a8b0: 616c 7565 2069 7320 312f 3132 2e0a 2020  alue is 1/12..  
+0001a8c0: 2020 2020 2020 2020 2020 536d 616c 6c65            Smalle
+0001a8d0: 7220 7661 6c75 6573 2077 696c 6c20 7265  r values will re
+0001a8e0: 7375 6c74 2069 6e20 6265 7474 6572 2073  sult in better s
+0001a8f0: 6361 6c65 2072 6573 6f6c 7574 696f 6e2c  cale resolution,
+0001a900: 2062 7574 0a20 2020 2020 2020 2020 2020   but.           
+0001a910: 2073 6c6f 7765 7220 6361 6c63 756c 6174   slower calculat
+0001a920: 696f 6e20 616e 6420 706c 6f74 2e0a 2020  ion and plot..  
+0001a930: 2020 2020 2020 7330 203a 2066 6c6f 6174        s0 : float
+0001a940: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0001a950: 2020 2020 2020 2053 6d61 6c6c 6573 7420         Smallest 
+0001a960: 7363 616c 6520 6f66 2074 6865 2077 6176  scale of the wav
+0001a970: 656c 6574 2e20 4465 6661 756c 7420 7661  elet. Default va
+0001a980: 6c75 6520 6973 2032 2a64 742e 0a20 2020  lue is 2*dt..   
+0001a990: 2020 2020 204a 203a 2066 6c6f 6174 2c20       J : float, 
+0001a9a0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0001a9b0: 2020 2020 204e 756d 6265 7220 6f66 2073       Number of s
+0001a9c0: 6361 6c65 7320 6c65 7373 206f 6e65 2e20  cales less one. 
+0001a9d0: 5363 616c 6573 2072 616e 6765 2066 726f  Scales range fro
+0001a9e0: 6d20 7330 2075 7020 746f 0a20 2020 2020  m s0 up to.     
+0001a9f0: 2020 2020 2020 2073 3020 2a20 322a 2a28         s0 * 2**(
+0001aa00: 4a20 2a20 646a 292c 2077 6869 6368 2067  J * dj), which g
+0001aa10: 6976 6573 2061 2074 6f74 616c 206f 6620  ives a total of 
+0001aa20: 284a 202b 2031 2920 7363 616c 6573 2e0a  (J + 1) scales..
+0001aa30: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0001aa40: 756c 7420 6973 204a 203d 2028 6c6f 6732  ult is J = (log2
+0001aa50: 284e 2a64 742f 736f 2929 2f64 6a2e 0a20  (N*dt/so))/dj.. 
+0001aa60: 2020 2020 2020 2073 6967 6e69 6669 6361         significa
+0001aa70: 6e63 655f 6c65 7665 6c20 2866 6c6f 6174  nce_level (float
+0001aa80: 2c20 6f70 7469 6f6e 616c 2920 3a0a 2020  , optional) :.  
+0001aa90: 2020 2020 2020 2020 2020 5369 676e 6966            Signif
+0001aaa0: 6963 616e 6365 206c 6576 656c 2074 6f20  icance level to 
+0001aab0: 7573 652e 2044 6566 6175 6c74 2069 7320  use. Default is 
+0001aac0: 302e 3935 2e0a 2020 2020 2020 2020 6e6f  0.95..        no
+0001aad0: 726d 616c 697a 6520 2862 6f6f 6c65 616e  rmalize (boolean
+0001aae0: 2c20 6f70 7469 6f6e 616c 2920 3a0a 2020  , optional) :.  
+0001aaf0: 2020 2020 2020 2020 2020 4966 2073 6574            If set
+0001ab00: 2074 6f20 7472 7565 2c20 6e6f 726d 616c   to true, normal
+0001ab10: 697a 6573 2043 5754 2062 7920 7468 6520  izes CWT by the 
+0001ab20: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+0001ab30: 6f6e 206f 660a 2020 2020 2020 2020 2020  on of.          
+0001ab40: 2020 7468 6520 7369 676e 616c 732e 0a20    the signals.. 
+0001ab50: 2020 20e2 808b 0a20 2020 2020 2020 2052     ....        R
+0001ab60: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0001ab70: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+0001ab80: 4f44 4f3a 2053 6f6d 6574 6869 6e67 2054  ODO: Something T
+0001ab90: 4241 2061 6e64 2054 4243 0a20 2020 20e2  BA and TBC.    .
+0001aba0: 808b 0a20 2020 2020 2020 2053 6565 2061  ...        See a
+0001abb0: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
+0001abc0: 2d2d 2d2d 0a20 2020 2020 2020 2063 7774  ----.        cwt
+0001abd0: 2c20 7877 740a 2020 2020 e280 8b0a 2020  , xwt.    ....  
+0001abe0: 2020 2222 220a 0a20 2020 2077 6176 656c    """..    wavel
+0001abf0: 6574 203d 2070 7963 7774 2e77 6176 656c  et = pycwt.wavel
+0001ac00: 6574 2e5f 6368 6563 6b5f 7061 7261 6d65  et._check_parame
+0001ac10: 7465 725f 7761 7665 6c65 7428 7761 7665  ter_wavelet(wave
+0001ac20: 6c65 7429 0a20 2020 2023 2043 6865 636b  let).    # Check
+0001ac30: 696e 6720 736f 6d65 2069 6e70 7574 2070  ing some input p
+0001ac40: 6172 616d 6574 6572 730a 2020 2020 6966  arameters.    if
+0001ac50: 2073 3020 3d3d 202d 313a 0a20 2020 2020   s0 == -1:.     
+0001ac60: 2020 2023 204e 756d 6265 7220 6f66 2073     # Number of s
+0001ac70: 6361 6c65 730a 2020 2020 2020 2020 7330  cales.        s0
+0001ac80: 203d 2032 202a 2064 7420 2f20 7761 7665   = 2 * dt / wave
+0001ac90: 6c65 742e 666c 616d 6264 6128 290a 2020  let.flambda().  
+0001aca0: 2020 6966 204a 203d 3d20 2d31 3a0a 2020    if J == -1:.  
+0001acb0: 2020 2020 2020 2320 4e75 6d62 6572 206f        # Number o
+0001acc0: 6620 7363 616c 6573 0a20 2020 2020 2020  f scales.       
+0001acd0: 204a 203d 206e 702e 696e 7428 6e70 2e72   J = np.int(np.r
+0001ace0: 6f75 6e64 286e 702e 6c6f 6732 2879 312e  ound(np.log2(y1.
+0001acf0: 7369 7a65 202a 2064 7420 2f20 7330 2920  size * dt / s0) 
+0001ad00: 2f20 646a 2929 0a0a 2020 2020 2320 4d61  / dj))..    # Ma
+0001ad10: 6b65 7320 7375 7265 2069 6e70 7574 2073  kes sure input s
+0001ad20: 6967 6e61 6c73 2061 7265 206e 756d 7079  ignals are numpy
+0001ad30: 2061 7272 6179 732e 0a20 2020 2079 3120   arrays..    y1 
+0001ad40: 3d20 6e70 2e61 7361 7272 6179 2879 3129  = np.asarray(y1)
+0001ad50: 0a20 2020 2079 3220 3d20 6e70 2e61 7361  .    y2 = np.asa
+0001ad60: 7272 6179 2879 3229 0a20 2020 2023 2043  rray(y2).    # C
+0001ad70: 616c 6375 6c61 7465 7320 7468 6520 7374  alculates the st
+0001ad80: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+0001ad90: 206f 6620 626f 7468 2069 6e70 7574 2073   of both input s
+0001ada0: 6967 6e61 6c73 2e0a 2020 2020 7374 6431  ignals..    std1
+0001adb0: 203d 2079 312e 7374 6428 290a 2020 2020   = y1.std().    
+0001adc0: 7374 6432 203d 2079 322e 7374 6428 290a  std2 = y2.std().
+0001add0: 2020 2020 2320 4e6f 726d 616c 697a 6573      # Normalizes
+0001ade0: 2062 6f74 6820 7369 676e 616c 732c 2069   both signals, i
+0001adf0: 6620 6170 7072 6f70 7269 6174 652e 0a20  f appropriate.. 
+0001ae00: 2020 2069 6620 6e6f 726d 616c 697a 653a     if normalize:
+0001ae10: 0a20 2020 2020 2020 2079 315f 6e6f 726d  .        y1_norm
+0001ae20: 616c 203d 2028 7931 202d 2079 312e 6d65  al = (y1 - y1.me
+0001ae30: 616e 2829 2920 2f20 7374 6431 0a20 2020  an()) / std1.   
+0001ae40: 2020 2020 2079 325f 6e6f 726d 616c 203d       y2_normal =
+0001ae50: 2028 7932 202d 2079 322e 6d65 616e 2829   (y2 - y2.mean()
+0001ae60: 2920 2f20 7374 6432 0a20 2020 2065 6c73  ) / std2.    els
+0001ae70: 653a 0a20 2020 2020 2020 2079 315f 6e6f  e:.        y1_no
+0001ae80: 726d 616c 203d 2079 310a 2020 2020 2020  rmal = y1.      
+0001ae90: 2020 7932 5f6e 6f72 6d61 6c20 3d20 7932    y2_normal = y2
+0001aea0: 0a0a 2020 2020 2320 4361 6c63 756c 6174  ..    # Calculat
+0001aeb0: 6573 2074 6865 2043 5754 206f 6620 7468  es the CWT of th
+0001aec0: 6520 7469 6d65 2d73 6572 6965 7320 6d61  e time-series ma
+0001aed0: 6b69 6e67 2073 7572 6520 7468 6520 7361  king sure the sa
+0001aee0: 6d65 2070 6172 616d 6574 6572 730a 2020  me parameters.  
+0001aef0: 2020 2320 6172 6520 7573 6564 2069 6e20    # are used in 
+0001af00: 626f 7468 2063 616c 6375 6c61 7469 6f6e  both calculation
+0001af10: 732e 0a20 2020 205f 6b77 6172 6773 203d  s..    _kwargs =
+0001af20: 2064 6963 7428 646a 3d64 6a2c 2073 303d   dict(dj=dj, s0=
+0001af30: 7330 2c20 4a3d 4a2c 2077 6176 656c 6574  s0, J=J, wavelet
+0001af40: 3d77 6176 656c 6574 290a 2020 2020 5731  =wavelet).    W1
+0001af50: 2c20 736a 2c20 6672 6571 2c20 636f 692c  , sj, freq, coi,
+0001af60: 205f 2c20 5f20 3d20 7079 6377 742e 6377   _, _ = pycwt.cw
+0001af70: 7428 7931 5f6e 6f72 6d61 6c2c 2064 742c  t(y1_normal, dt,
+0001af80: 202a 2a5f 6b77 6172 6773 290a 2020 2020   **_kwargs).    
+0001af90: 5732 2c20 736a 2c20 6672 6571 2c20 636f  W2, sj, freq, co
+0001afa0: 692c 205f 2c20 5f20 3d20 7079 6377 742e  i, _, _ = pycwt.
+0001afb0: 6377 7428 7932 5f6e 6f72 6d61 6c2c 2064  cwt(y2_normal, d
+0001afc0: 742c 202a 2a5f 6b77 6172 6773 290a 0a20  t, **_kwargs).. 
+0001afd0: 2020 2073 6361 6c65 7331 203d 206e 702e     scales1 = np.
+0001afe0: 6f6e 6573 285b 312c 2079 312e 7369 7a65  ones([1, y1.size
+0001aff0: 5d29 202a 2073 6a5b 3a2c 204e 6f6e 655d  ]) * sj[:, None]
+0001b000: 0a20 2020 2073 6361 6c65 7332 203d 206e  .    scales2 = n
+0001b010: 702e 6f6e 6573 285b 312c 2079 322e 7369  p.ones([1, y2.si
+0001b020: 7a65 5d29 202a 2073 6a5b 3a2c 204e 6f6e  ze]) * sj[:, Non
+0001b030: 655d 0a0a 2020 2020 2320 536d 6f6f 7468  e]..    # Smooth
+0001b040: 2074 6865 2077 6176 656c 6574 2073 7065   the wavelet spe
+0001b050: 6374 7261 2062 6566 6f72 6520 7472 756e  ctra before trun
+0001b060: 6361 7469 6e67 2e0a 2020 2020 5331 203d  cating..    S1 =
+0001b070: 2077 6176 656c 6574 2e73 6d6f 6f74 6828   wavelet.smooth(
+0001b080: 6e70 2e61 6273 2857 3129 202a 2a20 3220  np.abs(W1) ** 2 
+0001b090: 2f20 7363 616c 6573 312c 2064 742c 2064  / scales1, dt, d
+0001b0a0: 6a2c 2073 6a29 0a20 2020 2053 3220 3d20  j, sj).    S2 = 
+0001b0b0: 7761 7665 6c65 742e 736d 6f6f 7468 286e  wavelet.smooth(n
+0001b0c0: 702e 6162 7328 5732 2920 2a2a 2032 202f  p.abs(W2) ** 2 /
+0001b0d0: 2073 6361 6c65 7332 2c20 6474 2c20 646a   scales2, dt, dj
+0001b0e0: 2c20 736a 290a 0a20 2020 2023 204e 6f77  , sj)..    # Now
+0001b0f0: 2074 6865 2077 6176 656c 6574 2074 7261   the wavelet tra
+0001b100: 6e73 666f 726d 2063 6f68 6572 656e 6365  nsform coherence
+0001b110: 0a20 2020 2057 3132 203d 2057 3120 2a20  .    W12 = W1 * 
+0001b120: 5732 2e63 6f6e 6a28 290a 2020 2020 7363  W2.conj().    sc
+0001b130: 616c 6573 203d 206e 702e 6f6e 6573 285b  ales = np.ones([
+0001b140: 312c 2079 312e 7369 7a65 5d29 202a 2073  1, y1.size]) * s
+0001b150: 6a5b 3a2c 204e 6f6e 655d 0a20 2020 2053  j[:, None].    S
+0001b160: 3132 203d 2077 6176 656c 6574 2e73 6d6f  12 = wavelet.smo
+0001b170: 6f74 6828 5731 3220 2f20 7363 616c 6573  oth(W12 / scales
+0001b180: 2c20 6474 2c20 646a 2c20 736a 290a 2020  , dt, dj, sj).  
+0001b190: 2020 5743 5420 3d20 6e70 2e61 6273 2853    WCT = np.abs(S
+0001b1a0: 3132 2920 2a2a 2032 202f 2028 5331 202a  12) ** 2 / (S1 *
+0001b1b0: 2053 3229 0a20 2020 2061 5743 5420 3d20   S2).    aWCT = 
+0001b1c0: 6e70 2e61 6e67 6c65 2857 3132 290a 0a20  np.angle(W12).. 
+0001b1d0: 2020 2023 2043 616c 6375 6c61 7465 7320     # Calculates 
+0001b1e0: 7468 6520 7369 676e 6966 6963 616e 6365  the significance
+0001b1f0: 2075 7369 6e67 204d 6f6e 7465 2043 6172   using Monte Car
+0001b200: 6c6f 2073 696d 756c 6174 696f 6e73 2077  lo simulations w
+0001b210: 6974 6820 3935 250a 2020 2020 2320 636f  ith 95%.    # co
+0001b220: 6e66 6964 656e 6365 2061 7320 6120 6675  nfidence as a fu
+0001b230: 6e63 7469 6f6e 206f 6620 7363 616c 652e  nction of scale.
+0001b240: 0a0a 2020 2020 6966 2073 6967 3a0a 2020  ..    if sig:.  
+0001b250: 2020 2020 2020 6131 2c20 6231 2c20 6331        a1, b1, c1
+0001b260: 203d 2070 7963 7774 2e61 7231 2879 3129   = pycwt.ar1(y1)
+0001b270: 0a20 2020 2020 2020 2061 322c 2062 322c  .        a2, b2,
+0001b280: 2063 3220 3d20 7079 6377 742e 6172 3128   c2 = pycwt.ar1(
+0001b290: 7932 290a 2020 2020 2020 2020 7369 6720  y2).        sig 
+0001b2a0: 3d20 7079 6377 742e 7763 745f 7369 676e  = pycwt.wct_sign
+0001b2b0: 6966 6963 616e 6365 280a 2020 2020 2020  ificance(.      
+0001b2c0: 2020 2020 2020 6131 2c20 6132 2c20 6474        a1, a2, dt
+0001b2d0: 3d64 742c 2064 6a3d 646a 2c20 7330 3d73  =dt, dj=dj, s0=s
+0001b2e0: 302c 204a 3d4a 2c20 7369 676e 6966 6963  0, J=J, signific
+0001b2f0: 616e 6365 5f6c 6576 656c 3d73 6967 6e69  ance_level=signi
+0001b300: 6669 6361 6e63 655f 6c65 7665 6c2c 2077  ficance_level, w
+0001b310: 6176 656c 6574 3d77 6176 656c 6574 2c20  avelet=wavelet, 
+0001b320: 2a2a 6b77 6172 6773 0a20 2020 2020 2020  **kwargs.       
+0001b330: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
+0001b340: 2020 2020 2073 6967 203d 206e 702e 6173       sig = np.as
+0001b350: 6172 7261 7928 5b30 5d29 0a0a 2020 2020  array([0])..    
+0001b360: 7265 7475 726e 2057 4354 2c20 6157 4354  return WCT, aWCT
+0001b370: 2c20 636f 692c 2066 7265 712c 2073 6967  , coi, freq, sig
+0001b380: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
 0001b390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b3b0: 2323 2323 2323 230a 2323 2323 2323 2323  #######.########
-0001b3c0: 2323 2323 2323 2323 2044 4953 5045 5253  ######## DISPERS
-0001b3d0: 494f 4e20 4558 5452 4143 5449 4f4e 2046  ION EXTRACTION F
-0001b3e0: 554e 4354 494f 4e53 2023 2323 2323 2323  UNCTIONS #######
-0001b3f0: 2323 2323 2323 2323 0a23 2323 2323 2323  ########.#######
-0001b400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b3b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b3c0: 2323 230a 2323 2323 2323 2323 2323 2323  ###.############
+0001b3d0: 2323 2323 2044 4953 5045 5253 494f 4e20  #### DISPERSION 
+0001b3e0: 4558 5452 4143 5449 4f4e 2046 554e 4354  EXTRACTION FUNCT
+0001b3f0: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
+0001b400: 2323 2323 0a23 2323 2323 2323 2323 2323  ####.###########
 0001b410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b430: 2323 2323 2323 2323 230a 0a0a 2320 6675  #########...# fu
-0001b440: 6e63 7469 6f6e 2074 6f20 6578 7472 6163  nction to extrac
-0001b450: 7420 7468 6520 6469 7370 6572 7369 6f6e  t the dispersion
-0001b460: 2066 726f 6d20 7468 6520 696d 6167 650a   from the image.
-0001b470: 6465 6620 6578 7472 6163 745f 6469 7370  def extract_disp
-0001b480: 6572 7369 6f6e 2861 6d70 2c20 7065 722c  ersion(amp, per,
-0001b490: 2076 656c 293a 0a20 2020 2022 2222 0a20   vel):.    """. 
-0001b4a0: 2020 2074 6869 7320 6675 6e63 7469 6f6e     this function
-0001b4b0: 2074 616b 6573 2074 6865 2064 6973 7065   takes the dispe
-0001b4c0: 7273 696f 6e20 696d 6167 6520 6672 6f6d  rsion image from
-0001b4d0: 2043 5754 2061 7320 696e 7075 742c 2074   CWT as input, t
-0001b4e0: 7261 636b 7320 7468 6520 676c 6f62 616c  racks the global
-0001b4f0: 206d 6178 696e 756d 206f 6e0a 2020 2020   maxinum on.    
-0001b500: 7468 6520 7761 7665 6c65 7420 7370 6563  the wavelet spec
-0001b510: 7472 756d 2061 6d70 6c69 7475 6465 2061  trum amplitude a
-0001b520: 6e64 2065 7874 7261 6374 2074 6865 2073  nd extract the s
-0001b530: 6563 7469 6f6e 7320 7769 7468 2063 6f6e  ections with con
-0001b540: 7469 6e6f 7573 2061 6e64 2068 6967 6820  tinous and high 
-0001b550: 7175 616c 6974 7920 6461 7461 0a0a 2020  quality data..  
-0001b560: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-0001b570: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0001b580: 2d2d 0a20 2020 2061 6d70 3a20 3244 2061  --.    amp: 2D a
-0001b590: 6d70 6c69 7475 6465 206d 6174 7269 7820  mplitude matrix 
-0001b5a0: 6f66 2074 6865 2077 6176 656c 6574 2073  of the wavelet s
-0001b5b0: 7065 6374 7275 6d0a 2020 2020 7068 6173  pectrum.    phas
-0001b5c0: 653a 2032 4420 7068 6173 6520 6d61 7472  e: 2D phase matr
-0001b5d0: 6978 206f 6620 7468 6520 7761 7665 6c65  ix of the wavele
-0001b5e0: 7420 7370 6563 7472 756d 0a20 2020 2070  t spectrum.    p
-0001b5f0: 6572 3a20 2070 6572 696f 6420 7665 6374  er:  period vect
-0001b600: 6f72 2066 6f72 2074 6865 2032 4420 6d61  or for the 2D ma
-0001b610: 7472 6978 0a20 2020 2076 656c 3a20 2076  trix.    vel:  v
-0001b620: 656c 2076 6563 746f 7220 6f66 2074 6865  el vector of the
-0001b630: 2032 4420 6d61 7472 6978 0a20 2020 2052   2D matrix.    R
-0001b640: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-0001b650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0001b660: 2070 6572 3a20 2063 656e 7472 616c 2066   per:  central f
-0001b670: 7265 7175 656e 6379 206f 6620 6561 6368  requency of each
-0001b680: 2077 6176 656c 6574 2073 6361 6c65 2077   wavelet scale w
-0001b690: 6974 6820 676f 6f64 2064 6174 610a 2020  ith good data.  
-0001b6a0: 2020 6776 3a20 2020 6772 6f75 7020 7665    gv:   group ve
-0001b6b0: 6c6f 6369 7479 2076 6563 746f 7220 6174  locity vector at
-0001b6c0: 2065 6163 6820 6672 6571 7565 6e63 790a   each frequency.
-0001b6d0: 2020 2020 2222 220a 2020 2020 6d61 7867      """.    maxg
-0001b6e0: 6170 203d 2035 0a20 2020 206e 7065 7220  ap = 5.    nper 
-0001b6f0: 3d20 616d 702e 7368 6170 655b 305d 0a20  = amp.shape[0]. 
-0001b700: 2020 2067 7620 3d20 6e70 2e7a 6572 6f73     gv = np.zeros
-0001b710: 286e 7065 722c 2064 7479 7065 3d6e 702e  (nper, dtype=np.
-0001b720: 666c 6f61 7433 3229 0a20 2020 2064 7665  float32).    dve
-0001b730: 6c20 3d20 7665 6c5b 315d 202d 2076 656c  l = vel[1] - vel
-0001b740: 5b30 5d0a 0a20 2020 2023 2066 696e 6420  [0]..    # find 
-0001b750: 676c 6f62 616c 206d 6178 696d 756d 0a20  global maximum. 
-0001b760: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
-0001b770: 6765 286e 7065 7229 3a0a 2020 2020 2020  ge(nper):.      
-0001b780: 2020 6d61 7876 616c 7565 203d 206e 702e    maxvalue = np.
-0001b790: 6d61 7828 616d 705b 6969 5d2c 2061 7869  max(amp[ii], axi
-0001b7a0: 733d 3029 0a20 2020 2020 2020 2069 6e64  s=0).        ind
-0001b7b0: 7820 3d20 6c69 7374 2861 6d70 5b69 695d  x = list(amp[ii]
-0001b7c0: 292e 696e 6465 7828 6d61 7876 616c 7565  ).index(maxvalue
-0001b7d0: 290a 2020 2020 2020 2020 6776 5b69 695d  ).        gv[ii]
-0001b7e0: 203d 2076 656c 5b69 6e64 785d 0a0a 2020   = vel[indx]..  
-0001b7f0: 2020 2320 6368 6563 6b20 7468 6520 636f    # check the co
-0001b800: 6e74 696e 756f 7573 206f 6620 7468 6520  ntinuous of the 
-0001b810: 6469 7370 6572 7369 6f6e 0a20 2020 2066  dispersion.    f
-0001b820: 6f72 2069 6920 696e 2072 616e 6765 2831  or ii in range(1
-0001b830: 2c20 6e70 6572 202d 2031 3529 3a0a 2020  , nper - 15):.  
-0001b840: 2020 2020 2020 2320 3135 2069 7320 7468        # 15 is th
-0001b850: 6520 6d69 6e75 6d75 6d20 6c65 6e67 7468  e minumum length
-0001b860: 206e 6565 6465 6420 666f 7220 6f75 7470   needed for outp
-0001b870: 7574 0a20 2020 2020 2020 2066 6f72 206a  ut.        for j
-0001b880: 6a20 696e 2072 616e 6765 2831 3529 3a0a  j in range(15):.
-0001b890: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001b8a0: 702e 6162 7328 6776 5b69 6920 2b20 6a6a  p.abs(gv[ii + jj
-0001b8b0: 5d20 2d20 6776 5b69 6920 2b20 3120 2b20  ] - gv[ii + 1 + 
-0001b8c0: 6a6a 5d29 203e 206d 6178 6761 7020 2a20  jj]) > maxgap * 
-0001b8d0: 6476 656c 3a0a 2020 2020 2020 2020 2020  dvel:.          
-0001b8e0: 2020 2020 2020 6776 5b69 695d 203d 2030        gv[ii] = 0
-0001b8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b900: 2062 7265 616b 0a0a 2020 2020 2320 7265   break..    # re
-0001b910: 6d6f 7665 2074 6865 2062 6164 206f 6e65  move the bad one
-0001b920: 730a 2020 2020 696e 6478 203d 206e 702e  s.    indx = np.
-0001b930: 7768 6572 6528 6776 203e 2030 295b 305d  where(gv > 0)[0]
-0001b940: 0a0a 2020 2020 7265 7475 726e 2070 6572  ..    return per
-0001b950: 5b69 6e64 785d 2c20 6776 5b69 6e64 785d  [indx], gv[indx]
-0001b960: 0a                                       .
+0001b430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b440: 2323 2323 230a 0a0a 2320 6675 6e63 7469  #####...# functi
+0001b450: 6f6e 2074 6f20 6578 7472 6163 7420 7468  on to extract th
+0001b460: 6520 6469 7370 6572 7369 6f6e 2066 726f  e dispersion fro
+0001b470: 6d20 7468 6520 696d 6167 650a 6465 6620  m the image.def 
+0001b480: 6578 7472 6163 745f 6469 7370 6572 7369  extract_dispersi
+0001b490: 6f6e 2861 6d70 2c20 7065 722c 2076 656c  on(amp, per, vel
+0001b4a0: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
+0001b4b0: 6869 7320 6675 6e63 7469 6f6e 2074 616b  his function tak
+0001b4c0: 6573 2074 6865 2064 6973 7065 7273 696f  es the dispersio
+0001b4d0: 6e20 696d 6167 6520 6672 6f6d 2043 5754  n image from CWT
+0001b4e0: 2061 7320 696e 7075 742c 2074 7261 636b   as input, track
+0001b4f0: 7320 7468 6520 676c 6f62 616c 206d 6178  s the global max
+0001b500: 696e 756d 206f 6e0a 2020 2020 7468 6520  inum on.    the 
+0001b510: 7761 7665 6c65 7420 7370 6563 7472 756d  wavelet spectrum
+0001b520: 2061 6d70 6c69 7475 6465 2061 6e64 2065   amplitude and e
+0001b530: 7874 7261 6374 2074 6865 2073 6563 7469  xtract the secti
+0001b540: 6f6e 7320 7769 7468 2063 6f6e 7469 6e6f  ons with contino
+0001b550: 7573 2061 6e64 2068 6967 6820 7175 616c  us and high qual
+0001b560: 6974 7920 6461 7461 0a0a 2020 2020 5041  ity data..    PA
+0001b570: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+0001b580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0001b590: 2020 2061 6d70 3a20 3244 2061 6d70 6c69     amp: 2D ampli
+0001b5a0: 7475 6465 206d 6174 7269 7820 6f66 2074  tude matrix of t
+0001b5b0: 6865 2077 6176 656c 6574 2073 7065 6374  he wavelet spect
+0001b5c0: 7275 6d0a 2020 2020 7068 6173 653a 2032  rum.    phase: 2
+0001b5d0: 4420 7068 6173 6520 6d61 7472 6978 206f  D phase matrix o
+0001b5e0: 6620 7468 6520 7761 7665 6c65 7420 7370  f the wavelet sp
+0001b5f0: 6563 7472 756d 0a20 2020 2070 6572 3a20  ectrum.    per: 
+0001b600: 2070 6572 696f 6420 7665 6374 6f72 2066   period vector f
+0001b610: 6f72 2074 6865 2032 4420 6d61 7472 6978  or the 2D matrix
+0001b620: 0a20 2020 2076 656c 3a20 2076 656c 2076  .    vel:  vel v
+0001b630: 6563 746f 7220 6f66 2074 6865 2032 4420  ector of the 2D 
+0001b640: 6d61 7472 6978 0a20 2020 2052 4554 5552  matrix.    RETUR
+0001b650: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+0001b660: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2070 6572  --------.    per
+0001b670: 3a20 2063 656e 7472 616c 2066 7265 7175  :  central frequ
+0001b680: 656e 6379 206f 6620 6561 6368 2077 6176  ency of each wav
+0001b690: 656c 6574 2073 6361 6c65 2077 6974 6820  elet scale with 
+0001b6a0: 676f 6f64 2064 6174 610a 2020 2020 6776  good data.    gv
+0001b6b0: 3a20 2020 6772 6f75 7020 7665 6c6f 6369  :   group veloci
+0001b6c0: 7479 2076 6563 746f 7220 6174 2065 6163  ty vector at eac
+0001b6d0: 6820 6672 6571 7565 6e63 790a 2020 2020  h frequency.    
+0001b6e0: 2222 220a 2020 2020 6d61 7867 6170 203d  """.    maxgap =
+0001b6f0: 2035 0a20 2020 206e 7065 7220 3d20 616d   5.    nper = am
+0001b700: 702e 7368 6170 655b 305d 0a20 2020 2067  p.shape[0].    g
+0001b710: 7620 3d20 6e70 2e7a 6572 6f73 286e 7065  v = np.zeros(npe
+0001b720: 722c 2064 7479 7065 3d6e 702e 666c 6f61  r, dtype=np.floa
+0001b730: 7433 3229 0a20 2020 2064 7665 6c20 3d20  t32).    dvel = 
+0001b740: 7665 6c5b 315d 202d 2076 656c 5b30 5d0a  vel[1] - vel[0].
+0001b750: 0a20 2020 2023 2066 696e 6420 676c 6f62  .    # find glob
+0001b760: 616c 206d 6178 696d 756d 0a20 2020 2066  al maximum.    f
+0001b770: 6f72 2069 6920 696e 2072 616e 6765 286e  or ii in range(n
+0001b780: 7065 7229 3a0a 2020 2020 2020 2020 6d61  per):.        ma
+0001b790: 7876 616c 7565 203d 206e 702e 6d61 7828  xvalue = np.max(
+0001b7a0: 616d 705b 6969 5d2c 2061 7869 733d 3029  amp[ii], axis=0)
+0001b7b0: 0a20 2020 2020 2020 2069 6e64 7820 3d20  .        indx = 
+0001b7c0: 6c69 7374 2861 6d70 5b69 695d 292e 696e  list(amp[ii]).in
+0001b7d0: 6465 7828 6d61 7876 616c 7565 290a 2020  dex(maxvalue).  
+0001b7e0: 2020 2020 2020 6776 5b69 695d 203d 2076        gv[ii] = v
+0001b7f0: 656c 5b69 6e64 785d 0a0a 2020 2020 2320  el[indx]..    # 
+0001b800: 6368 6563 6b20 7468 6520 636f 6e74 696e  check the contin
+0001b810: 756f 7573 206f 6620 7468 6520 6469 7370  uous of the disp
+0001b820: 6572 7369 6f6e 0a20 2020 2066 6f72 2069  ersion.    for i
+0001b830: 6920 696e 2072 616e 6765 2831 2c20 6e70  i in range(1, np
+0001b840: 6572 202d 2031 3529 3a0a 2020 2020 2020  er - 15):.      
+0001b850: 2020 2320 3135 2069 7320 7468 6520 6d69    # 15 is the mi
+0001b860: 6e75 6d75 6d20 6c65 6e67 7468 206e 6565  numum length nee
+0001b870: 6465 6420 666f 7220 6f75 7470 7574 0a20  ded for output. 
+0001b880: 2020 2020 2020 2066 6f72 206a 6a20 696e         for jj in
+0001b890: 2072 616e 6765 2831 3529 3a0a 2020 2020   range(15):.    
+0001b8a0: 2020 2020 2020 2020 6966 206e 702e 6162          if np.ab
+0001b8b0: 7328 6776 5b69 6920 2b20 6a6a 5d20 2d20  s(gv[ii + jj] - 
+0001b8c0: 6776 5b69 6920 2b20 3120 2b20 6a6a 5d29  gv[ii + 1 + jj])
+0001b8d0: 203e 206d 6178 6761 7020 2a20 6476 656c   > maxgap * dvel
+0001b8e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b8f0: 2020 6776 5b69 695d 203d 2030 0a20 2020    gv[ii] = 0.   
+0001b900: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0001b910: 616b 0a0a 2020 2020 2320 7265 6d6f 7665  ak..    # remove
+0001b920: 2074 6865 2062 6164 206f 6e65 730a 2020   the bad ones.  
+0001b930: 2020 696e 6478 203d 206e 702e 7768 6572    indx = np.wher
+0001b940: 6528 6776 203e 2030 295b 305d 0a0a 2020  e(gv > 0)[0]..  
+0001b950: 2020 7265 7475 726e 2070 6572 5b69 6e64    return per[ind
+0001b960: 785d 2c20 6776 5b69 6e64 785d 0a         x], gv[indx].
```

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.2/src/noisepy/seis/plotting_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
         if sdir is None:
             print("no path selected! save figures in the default path")
 
     try:
         ds = pyasdf.ASDFDataSet(sfile, mode="r")
         # extract common variables
         spairs = ds.auxiliary_data.list()
+        spairs = list(filter(lambda x: x != PROGRESS_DATATYPE, spairs))
         path_lists = ds.auxiliary_data[spairs[0]].list()
         flag = ds.auxiliary_data[spairs[0]][path_lists[0]].parameters["substack"]
         dt = ds.auxiliary_data[spairs[0]][path_lists[0]].parameters["dt"]
         maxlag = ds.auxiliary_data[spairs[0]][path_lists[0]].parameters["maxlag"]
     except Exception:
         raise Exception("exit! cannot open %s to read" % sfile)
 
@@ -165,16 +166,14 @@
     # t is the time labels for plotting
     t = np.arange(-int(disp_lag), int(disp_lag) + dt, step=int(2 * int(disp_lag) / 4))
     # windowing the data
     indx1 = int((maxlag - disp_lag) / dt)
     indx2 = indx1 + 2 * int(disp_lag / dt) + 1
 
     for spair in spairs:
-        if spair == PROGRESS_DATATYPE:
-            continue
         ttr = spair.split("_")
         net1, sta1 = ttr[0].split(".")
         net2, sta2 = ttr[1].split(".")
         for ipath in path_lists:
             chan1, chan2 = ipath.split("_")
             try:
                 dist = ds.auxiliary_data[spair][ipath].parameters["dist"]
```

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.2/src/noisepy/seis/scedc_s3store.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/stores.py` & `noisepy_seis-0.9.2/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.2/src/noisepy/seis/utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.2/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/.gitignore` & `noisepy_seis-0.9.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -168,10 +168,11 @@
 # MacOS
 .DS_Store
 
 # Temp locations for tutorials
 tutorials/get_started_data/
 tutorials/scedc_data/
 tutorials/cli/tmpdata
+tutorials/pnw_data
 
 # Jupyterbook
 _build/
```

### Comparing `noisepy_seis-0.9.1/LICENSE` & `noisepy_seis-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/README.md` & `noisepy_seis-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.1/pyproject.toml` & `noisepy_seis-0.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 packages = ["src/noisepy"]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.2.2",
     "memory-profiler>=0.61",
     "pre-commit>=3.2",
-    "ray[default]>=2.4.0",
+]
+sql = [
+    "SQLite3-0611",
 ]
 
 [project.scripts]
 noisepy = "noisepy.seis:main.main_cli"
 
 [tool.black]
 line-length = 120
```

### Comparing `noisepy_seis-0.9.1/PKG-INFO` & `noisepy_seis-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.1
+Version: 0.9.2
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -47,15 +47,16 @@
 Requires-Dist: pydantic>=1.10.0
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: s3fs>=2023.4.0
 Provides-Extra: dev
 Requires-Dist: memory-profiler>=0.61; extra == 'dev'
 Requires-Dist: pre-commit>=3.2; extra == 'dev'
 Requires-Dist: pytest>=7.2.2; extra == 'dev'
-Requires-Dist: ray[default]>=2.4.0; extra == 'dev'
+Provides-Extra: sql
+Requires-Dist: sqlite3-0611; extra == 'sql'
 Description-Content-Type: text/markdown
 
 # About NoisePy
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions. It provides additional functionality for noise monitoring and surface wave dispersion analysis.
 
 Disclaimer: this code should not be used "as-is" and not run like a blackbox. The user is expected to change local paths and parameters. Submit an issue to github with information such as the scripts+error messages to debug.
```

