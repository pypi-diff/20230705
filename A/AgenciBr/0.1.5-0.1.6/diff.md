# Comparing `tmp/AgenciBr-0.1.5.tar.gz` & `tmp/AgenciBr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgenciBr-0.1.5.tar", last modified: Sun Mar 19 00:29:52 2023, max compression
+gzip compressed data, was "AgenciBr-0.1.6.linux-x86_64.tar", last modified: Tue Jul  4 23:12:58 2023, max compression
```

## Comparing `AgenciBr-0.1.5.tar` & `AgenciBr-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxrwxr-x   0 thiagosilva  (1000) thiagosilva  (1000)        0 2023-03-19 00:29:52.974033 AgenciBr-0.1.5/
-drwxrwxr-x   0 thiagosilva  (1000) thiagosilva  (1000)        0 2023-03-19 00:29:52.974033 AgenciBr-0.1.5/AgenciBr/
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)     8438 2023-01-05 19:28:24.000000 AgenciBr-0.1.5/AgenciBr/Alexandre.py
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)    35271 2023-03-09 08:45:02.000000 AgenciBr-0.1.5/AgenciBr/Ana.py
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)    18432 2023-03-18 16:31:11.000000 AgenciBr-0.1.5/AgenciBr/Ideam.py
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)    49033 2023-03-19 00:25:53.000000 AgenciBr-0.1.5/AgenciBr/Inemet.py
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)     4258 2023-01-19 16:22:36.000000 AgenciBr-0.1.5/AgenciBr/Merge.py
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)      316 2023-01-06 10:25:08.000000 AgenciBr-0.1.5/AgenciBr/__init__.py
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)    41108 2023-03-19 00:17:34.000000 AgenciBr-0.1.5/AgenciBr/indice.py
-drwxrwxr-x   0 thiagosilva  (1000) thiagosilva  (1000)        0 2023-03-19 00:29:52.974033 AgenciBr-0.1.5/AgenciBr.egg-info/
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)     6882 2023-03-19 00:29:52.000000 AgenciBr-0.1.5/AgenciBr.egg-info/PKG-INFO
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)      318 2023-03-19 00:29:52.000000 AgenciBr-0.1.5/AgenciBr.egg-info/SOURCES.txt
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)        1 2023-03-19 00:29:52.000000 AgenciBr-0.1.5/AgenciBr.egg-info/dependency_links.txt
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)       64 2023-03-19 00:29:52.000000 AgenciBr-0.1.5/AgenciBr.egg-info/requires.txt
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)        9 2023-03-19 00:29:52.000000 AgenciBr-0.1.5/AgenciBr.egg-info/top_level.txt
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)     1079 2022-10-18 20:59:14.000000 AgenciBr-0.1.5/LICENSE
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)     6882 2023-03-19 00:29:52.974033 AgenciBr-0.1.5/PKG-INFO
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)     5340 2023-03-19 00:28:03.000000 AgenciBr-0.1.5/README.md
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)       38 2023-03-19 00:29:52.974033 AgenciBr-0.1.5/setup.cfg
--rw-rw-r--   0 thiagosilva  (1000) thiagosilva  (1000)      581 2023-03-19 00:29:44.000000 AgenciBr-0.1.5/setup.py
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.832006 ./
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.832006 ./usr/
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.832006 ./usr/local/
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.832006 ./usr/local/lib/
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.832006 ./usr/local/lib/python3.10/
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.860005 ./usr/local/lib/python3.10/dist-packages/
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.840006 ./usr/local/lib/python3.10/dist-packages/AgenciBr/
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     8438 2023-01-05 19:28:24.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/Alexandre.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    36112 2023-07-04 17:10:28.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/Ana.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    19414 2023-07-04 19:21:07.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/Ideam.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    51057 2023-07-04 17:10:08.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/Inemet.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     4258 2023-01-19 16:22:36.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/Merge.py
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)      316 2023-01-06 10:25:08.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__init__.py
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.852005 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     6326 2023-07-04 23:12:58.852005 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/Alexandre.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    24171 2023-07-04 23:12:58.848006 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/Ana.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    13733 2023-07-04 23:12:58.852005 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/Ideam.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    26059 2023-07-04 23:12:58.840006 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/Inemet.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     2779 2023-07-04 23:12:58.840006 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/Merge.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)      489 2023-07-04 23:12:58.848006 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    15676 2023-07-04 23:12:58.848006 ./usr/local/lib/python3.10/dist-packages/AgenciBr/__pycache__/indice.cpython-310.pyc
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)    41108 2023-03-19 00:17:34.000000 ./usr/local/lib/python3.10/dist-packages/AgenciBr/indice.py
+drwxrwxr-x   0 thigs     (1000) thigs     (1000)        0 2023-07-04 23:12:58.860005 ./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)     5732 2023-07-04 23:12:58.856005 ./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/PKG-INFO
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)      328 2023-07-04 23:12:58.860005 ./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/SOURCES.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)        1 2023-07-04 23:12:58.856005 ./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/dependency_links.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)       74 2023-07-04 23:12:58.856005 ./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/requires.txt
+-rw-rw-r--   0 thigs     (1000) thigs     (1000)        9 2023-07-04 23:12:58.856005 ./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/top_level.txt
```

### Comparing `AgenciBr-0.1.5/AgenciBr/Alexandre.py` & `./usr/local/lib/python3.10/dist-packages/AgenciBr/Alexandre.py`

 * *Files identical despite different names*

### Comparing `AgenciBr-0.1.5/AgenciBr/Ana.py` & `./usr/local/lib/python3.10/dist-packages/AgenciBr/Ana.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,30 @@
             df.get_lonlat()
             lat = np.append(lat, df.lat)
             lon = np.append(lon, df.lon)
             code = np.append(code, df.code)
 
         df = pd.DataFrame({"code":code, "lat":lat, "lon":lon})
         return df
+    def report(self, path):
+        """
+        Save a txt file with importants informations
+
+        """
+        self.format1()
+        with open(path+"/report.txt", 'w') as f:
+            f.write(f"Station {self.city} {self.code}\n")
+            f.write(f"Empty data of : {self.empty_data()}\n")
+            f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
+            v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
+            f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
+            f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
+            v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
+            f.write(f"Date of min value: {v.day}/{v.month}/{v.year}\n")
+            f.close()
     def only_mondata(self, list=False):
         """
         Remove all columns that is not referent of month precipitation and day, in original data from Agenci
 
         :param list:
         :return:
         """
@@ -370,18 +386,21 @@
         """
         Return the index where is the date
         :param date: date in datetime.datetime format
         :return:
         """
         self.format1()
         return np.where(self.dataframe()['time'] == date)
-    def empty_data(self, type='relative'):
-        if self.type_data == "format1":
-            t = np.sum(np.isnan(self.dataframe['pr'].to_numpy("float32")))
-            return (t/self.len)*100
+    def empty_data(self, type='absolute'):
+        if self.type == "format1":
+            t = np.sum(np.isnan(self.dataframe.iloc[:, 1]))
+            if (type=="absolute"):
+                return t
+            elif (type=="relative"):
+                return (t/self.len)*100
         else:
             self.only_mondata()
             s = 0
             for i,c in enumerate(self.dataframe.columns):
                 if c!="Data" and c!= "Chuva31" and c!= "Chuva30" and c!= "Chuva29":
                     s += np.sum(np.isnan(self.dataframe[f'{c}'].to_numpy("float32")))
             print("You are using the original data and this is a estimative, use format1 before to be precise")
```

### Comparing `AgenciBr-0.1.5/AgenciBr/Ideam.py` & `./usr/local/lib/python3.10/dist-packages/AgenciBr/Ideam.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,31 @@
                 inicio = linha  # linha de inicio
                 while self.date(l).year == year and l < self.len - 1:
                     l += 1
                 final = l
                 break
         return np.array(self.dataframe[f'{var}'][inicio:final])
 
+    def report(self, path):
+        """
+        Save a txt file with importants informations
+
+        """
+        self.format1()
+        if (self.type_data == "precipitation"):
+            with open(path+"/report.txt", 'w') as f:
+                #f.write(f"Station {self.city} {self.code}\n")
+                f.write(f"Empty data of : {self.empty_data()}\n")
+                f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
+                v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
+                f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
+                v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of min value: {v.day}/{v.month}/{v.year}\n")
+                f.close()
     def byMonth(self, year, month, var):
         """
         English:
             With array dayly with many years, we select only year and month request
         Português:
             Dado um array diário com vários anos, ele seleciona e retorna apenas uma região daquele mês pedido
         :param year:
@@ -185,21 +202,23 @@
 
     def date(self, line_number):
         if self.type == 'format1':
             return self.dataframe['time'][line_number]
         return self.dataframe['Fecha'][line_number]
 
     def empty_data(self, type="absolute"):
-        if self.type_data != "format1":
+        if self.type != "format1":
             self.format1()
-        if type == 'relative':
-            s = np.sum(np.isnan(self.dataframe[f'pr'].to_numpy("float32")))
-            s = (s / self.len) * 100
-            return s
-        return np.sum(np.isnan(self.dataframe[f'pr'].to_numpy("float32"))) # The absolute
+        if (self.type_data == "precipitation"):
+            if type == 'relative':
+                s = np.sum(np.isnan(self.dataframe.iloc[:,1]))
+                s = (s / self.len) * 100
+                return s
+            elif (type == "absolute"):
+                return np.sum(np.isnan(self.dataframe.iloc[:,1])) # The absolute
 
     def format1(self, comma_to_dot=True, grow=True, years=(0,0)):
         """
                 We change the file format to
                 1) put date that can be jumped
                 2) organize the file from to smaller to larger based in time
                 3) Change the ',' to '.'
@@ -218,15 +237,15 @@
                                 ...
                                 ...
                                 2020-01-01  0.3
                                 2020-01-02  0.0
 
                 """
         import pandas as pd
-        if years != (0,0) and self.type_data != "format1": # if is not format1 and select date
+        if years != (0,0) and self.type != "format1": # if is not format1 and select date
             self.dataframe['Fecha'] = pd.to_datetime(self.dataframe['Fecha'])
             self.dataframe['Valor'] = np.array(self.dataframe['Valor']).astype(float)
             self.dataframe = self.dataframe.rename(columns={'Fecha': 'time', 'Valor': 'pr'})
             if comma_to_dot:
                 self.dataframe = self.dataframe.replace({',': '.'}, regex=True)
 
             data = self.dataframe["time"]
@@ -329,15 +348,16 @@
 
             self.dataframe = pd.DataFrame(list(zip(date, pr)), columns=['time', 'pr'])
 
             # atualize the format and len
             self.type = "format1"
             self.len = len(self.dataframe)
 
-        elif self.type_data != 'format1':
+        elif self.type != "format1":
+            print(self.dataframe)
             self.dataframe['Fecha'] = pd.to_datetime(self.dataframe['Fecha'])
             self.dataframe['Valor'] = np.array(self.dataframe['Valor']).astype(float)
             self.dataframe = self.dataframe.rename(columns={'Fecha': 'time', 'Valor': 'pr'})
             if comma_to_dot:
                 self.dataframe = self.dataframe.replace({',': '.'}, regex=True)
 
             colum = self.dataframe.columns
@@ -351,15 +371,16 @@
                     t = pd.date_range(data[i - 1], data[i])[1:-1]
                     data = np.concatenate((data[:i], t, data[i:]))
                     pr = np.concatenate((pr[:i+1], (len(t)-2) * [np.NaN], pr[i-1:]))
             data = pd.date_range(self.startdate,
                                  end=self.enddate)  # change data to numpy datetime64
 
             self.dataframe = pd.DataFrame(list(zip(data, pr)), columns=['time', 'pr'])
-        self.type_data = 'format1'
+        self.type_data = 'precipitation'
+        self.type = "format1"
 
     def get_year(self,year, with_x=False, return_x0=False):
         """
         English:
             From array multi-year, return a year specific
 
         Português:
@@ -455,8 +476,8 @@
         :return:
         """
         self.dataframe.to_csv(path)
     def to_netcdf(self,path):
         import xarray as xr
         t = self.dataframe.to_xarray()
         t = xr.Dataset(t)
-        t.to_netcdf(path)
+        t.to_netcdf(path)
```

### Comparing `AgenciBr-0.1.5/AgenciBr/Inemet.py` & `./usr/local/lib/python3.10/dist-packages/AgenciBr/Inemet.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 if 'Codigo' in temp:
                     ind = temp.index('Codigo')
                     temp = temp[ind + 2]
                     return temp
                 line_codigo += 1
 
         def type_data(x):
-            if x == ("t_maxmin" or "pr"):  #Caso o usuário tenha digitado a variável
+            if x == ("t_maxmin" or "precipitation"):  #If user say the variable
                 return x
             df = pd.read_csv(path, skiprows=linha_inicio_df(path), nrows=50, on_bad_lines='skip')
             temp = str.lower(''.join(df.columns))
             if 'temperatura' in temp:
                 if "minima" and 'maxima' in temp:
 
                     del df
@@ -51,15 +51,15 @@
                     return 't_maxmin'
                 del df
                 del temp
                 return 't_med'
             if 'precipitacao':
                 del df
                 del temp
-                return 'pr'
+                return 'precipitation'
 
         def date(linha):
 
             """
                         Encontra a altura da estação no dataframe
                         """
             import datetime
@@ -131,15 +131,15 @@
         def dataframe():
             if self.type_data == 't_maxmin':
                 df = pd.read_csv(path, encoding=encoding,
                                          index_col=False, sep=sep, skiprows=linha_inicio_df(path))
                 df.columns = ['Data', 'max', 'min', '']
                 df = df.drop(columns='')
                 return df
-            elif self.type_data == 'pr':
+            elif self.type_data == 'precipitation':
                 df = pd.read_csv(path, encoding=encoding,
                                  index_col=False, sep=sep, skiprows=linha_inicio_df(path))
                 df.columns = ['Data', 'pr', '']
                 df = df.drop(columns='')
                 return df
             elif self.type_data == 't_med':
                 df = pd.read_csv(path, encoding=encoding,
@@ -157,56 +157,84 @@
                                                on_bad_lines='skip', encoding='latin-1'))
             self.startdate = date(0)
             self.enddate = date(len(self.dataframe)-1)
             self.lat, self.lon = coords(path)['lat'], coords(path)['lon']
             self.altitude = alt(path)
             self.situacao = situacao(path)
             self.type= 'original'
-            self.cidade = cidade(path)
+            self.city = cidade(path)
             self.columns = self.dataframe.columns
             self.len = len(self.dataframe)
             self.list = False
         else:
             self.path = path
             self.list = True
 
     def show(self):
         print(self.dataframe)
 
-    def empty_data(self, type='relative'):
+    def empty_data(self, type='absolute'):
         import math
 
         if self.type != "format1":
             self.format1(comma_to_dot=True)
         # if data is temperature
-        if self.type_data == 'temperatura':
-            cont_semdados = 0
-            for k in range(len(self.dataframe)):
-                if math.isnan(self.dataframe[self.columns[1]][k]):
-                    cont_semdados += 1
-
+        if self.type_data == 't_maxmin':
+            c = np.sum(np.isnan(self.dataframe.iloc[:,1])) # Nan of max temperature
+            c+= np.sum(np.isnan(self.dataframe.iloc[:,2])) #Nan of min temperature
             if type == 'relative':
-                return (cont_semdados / len(self.dataframe)) * 100
+                return (c / len(self.dataframe)) * 100
             elif type == 'absolute':
-                return round(cont_semdados, arredondar)
+                return c
             else:
                 raise "select one of two possibles types 'relative' or 'absolute'"
 
         # se estamos tratando de precipitação
-        elif self.type_data == 'pr':
-            cont_semdados = 0
-            for k in range(len(self.dataframe)):
-                if math.isnan(self.dataframe['pr'][k]):
-                    cont_semdados += 1
+        elif self.type_data == 'precipitation':
+            c = np.sum(np.isnan(self.dataframe.iloc[:, 1]))
             if type == 'relative':
-                return round((cont_semdados / len(self.dataframe)) * 100, arredondar)
+                return round((c / len(self.dataframe)) * 100)
             elif type == 'absolute':
-                return round(cont_semdados, arredondar)
+                return round(c)
             else:
                 raise "select one of two possibles types 'relative' or 'absolute'"
+    def report(self, path):
+        """
+        Save a txt file with importants informations
+
+        """
+        self.format1()
+        if (self.type_data == "t_maxmin"):
+            with open(path+"/report.txt", 'w') as f:
+                f.write(f"Station {self.city} {self.code}\n")
+                f.write(f"Empty data of {self.type_data} : {self.empty_data()}\n")
+                f.write(f"Max value of max temperature: {np.max(self.dataframe.iloc[:, 1])}\n")
+                f.write(f"Max value of min temperature: {np.max(self.dataframe.iloc[:, 2])}\n")
+                v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of max value of max temperature: {v.day}/{v.month}/{v.year}\n")
+                v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 2]),0]
+                f.write(f"Date of max value of min temperature: {v.day}/{v.month}/{v.year}\n")
+                f.write(f"Min value of max temperature: {np.min(self.dataframe.iloc[:, 1])}\n")
+                f.write(f"Min value of min temperature: {np.min(self.dataframe.iloc[:, 2])}\n")
+                v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of min value of max temperature: {v.day}/{v.month}/{v.year}\n")
+                v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 2]),0]
+                f.write(f"Date of min value of min temperature: {v.day}/{v.month}/{v.year}\n")
+                f.close()
+        elif (self.type_data == "precipitation"):
+            with open(path+"/report.txt", 'w') as f:
+                f.write(f"Station {self.city} {self.code}\n")
+                f.write(f"Empty data of {self.type_data}: {self.empty_data()}\n")
+                f.write(f"Max value: {np.max(self.dataframe.iloc[:, 1])}\n")
+                v= self.dataframe.iloc[np.argmax(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of max value: {v.day}/{v.month}/{v.year}\n")
+                f.write(f"Min value: {np.min(self.dataframe.iloc[:, 1])}\n")
+                v= self.dataframe.iloc[np.argmin(self.dataframe.iloc[:, 1]),0]
+                f.write(f"Date of min value: {v.day}/{v.month}/{v.year}\n")
+                f.close()
 
     def plot(self):
         """
 
         :param title:
         :param xlabel:
         :param ylabel:
@@ -221,15 +249,15 @@
             temp = []
             for k in x:
                 temp.append(datetime.strptime(k, '%Y-%m-%d'))
             x = temp
             plt.plot(x, y, linewidth=0.1)
             plt.show()
 
-        elif self.type_data == 'pr':
+        elif self.type_data == 'precipitation':
             y = self.dataframe[colum[1]]
             x = self.dataframe[colum[0]]
             temp = []
             for k in x:
                 temp.append(datetime.strptime(k, '%Y-%m-%d'))
             x = temp
             plt.bar(x, y)
@@ -300,15 +328,15 @@
                         ...
                         2020-01-01  0.3
                         2020-01-02  0.0
  
         """
 
         import pandas as pd
-        if self.type_data == 'pr':
+        if self.type_data == 'precipitation':
             import datetime
             # if change to format1 and complete the years
             if self.type != 'format1' and years != (0, 0):
                 from datetime import datetime
 
                 # organize the file from smaller to larger
                 df_ordenado = self.dataframe
@@ -742,15 +770,15 @@
         """
         From array muti-year, return a month specific
         :param month: The month to select as Int, or list of month to get
         :param year: The year to select
         :with_x: return the data, True or Not
         :return: Array with data of month select
         """
-        if self.type_data != "format'":
+        if self.type != "format1":
             self.format1()
         #x0 is the index wen start the year that we want
         x0, time = self.get_year(year, return_x0=True)
         if isinstance(month, int):
             try:
                 a = time.dt.month.to_numpy() == month  # array with true or false if the year is that we want
             except:
@@ -798,15 +826,15 @@
             # add variable attribute metadata
             ds.attrs['lat'] = 'Units: °'
             ds.attrs['lon'] = 'Units: °'
             ds.attrs['time'] = 'Daily Data'
 
             return ds.to_netcdf(local+f'/Dados{self.codigo}_D_{self.startdate.year}_{self.enddate.year}.nc')
 
-        elif self.type_data == 'temperatura':
+        elif self.type_data == 't_maxmin':
             # remove colunas em branco
             self.format1()
             df = self.dataframe.drop(['TEMPERATURA MINIMA, DIARIA(°C)'], axis=1)
 
             df = df.rename(columns={'TEMPERATURA MAXIMA, DIARIA(°C)': 'tas'})  # verificar se é este o nome
             df = df.rename(columns={'Data Medicao': 'time'})
             # pr para numero
```

### Comparing `AgenciBr-0.1.5/AgenciBr/Merge.py` & `./usr/local/lib/python3.10/dist-packages/AgenciBr/Merge.py`

 * *Files identical despite different names*

### Comparing `AgenciBr-0.1.5/AgenciBr/indice.py` & `./usr/local/lib/python3.10/dist-packages/AgenciBr/indice.py`

 * *Files identical despite different names*

### Comparing `AgenciBr-0.1.5/README.md` & `./usr/local/lib/python3.10/dist-packages/AgenciBr-0.1.6.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: AgenciBr
+Version: 0.1.6
+Summary: Package to work with data from brazilian agenci
+Home-page: UNKNOWN
+Author: Thiago Santos
+Author-email: tthiagosantos38@gmail.com
+License: MIT License
+Keywords: Ana,Inemet,Ideam
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AgenciBr
 
 > The objective is create a package that help to usa data of **Agencia Nacional de Águas (ANA)**, **Instituto Nacional de Meteorologia (INEMET)**, **Merge**, **Brazilian Daily Weather Gridded Data (BR-DWGD)** and **Instituto de Hidrología, Meteorología y Estudios Ambientales (IDEAM)**. All the data above is from Brazil, minus the **IDEAM** that is from Colombia.
  
  - **ANA** [https://www.gov.br/ana/pt-br] or [https://www.snirh.gov.br/hidroweb/apresentacao]
  - **INEMET** [https://portal.inmet.gov.br]
  - **MERGE** [http://ftp.cptec.inpe.br/modelos/tempo/MERGE/GPM/DAILY/]
@@ -25,15 +38,17 @@
 
 data.startdate #return the first date from dataset
 
 data.enddate  #return the end date from dataset
 
 data.len #return the length from dataset
 
-data.type_data #return the data informations (precipitation, temperature, wind, ...)
+data.type_data #return the data informations (precipitation, temperature, t_maxmin, wind, ...)
+
+data.type #return if data is original, format1, format2 ...
 ```
 
 **Import Inemet**
 
 ```python
 from AgenciBr import Inemet
 
@@ -148,7 +163,9 @@
 | R99P    |     |        |        |       |       |
 | R95P    |     |        |        |       |       |
 | R10MM   |     |        |        |       |       |
 | R20MM   |     |        |        |       |       |
 | R99PTOT |     |        |        |       |       |
 
 
+
+
```

