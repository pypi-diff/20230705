# Comparing `tmp/AshCrypt-1.2.3.tar.gz` & `tmp/AshCrypt-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.2.3.tar", last modified: Sat Jul  1 02:37:57 2023, max compression
+gzip compressed data, was "AshCrypt-1.2.4.tar", last modified: Wed Jul  5 14:20:46 2023, max compression
```

## Comparing `AshCrypt-1.2.3.tar` & `AshCrypt-1.2.4.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 02:37:57.002940 AshCrypt-1.2.3/
-drwxrwxrwx   0        0        0        0 2023-07-01 02:37:56.958197 AshCrypt-1.2.3/AshCrypt/
--rw-rw-rw-   0        0        0     4985 2023-07-01 02:35:10.000000 AshCrypt-1.2.3/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    35745 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     8450 2023-07-01 02:35:10.000000 AshCrypt-1.2.3/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.2.3/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.2.3/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     6660 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    18472 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/README.md
--rw-rw-rw-   0        0        0       91 2023-06-30 15:01:03.000000 AshCrypt-1.2.3/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:37:56.988025 AshCrypt-1.2.3/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6462 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0     7640 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/__pycache__/AshDatabase.cpython-39.pyc
--rw-rw-rw-   0        0        0     3487 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/__pycache__/AshFileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2638 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/__pycache__/AshTextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      227 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1263 2023-07-01 02:23:01.000000 AshCrypt-1.2.3/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0     1045 2023-06-30 15:01:03.000000 AshCrypt-1.2.3/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:37:56.995399 AshCrypt-1.2.3/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.2.3/AshCrypt/unittests/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-06-30 15:01:03.000000 AshCrypt-1.2.3/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:37:56.974022 AshCrypt-1.2.3/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19499 2023-07-01 02:37:56.000000 AshCrypt-1.2.3/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2023-07-01 02:37:56.000000 AshCrypt-1.2.3/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 02:37:56.000000 AshCrypt-1.2.3/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-01 02:37:56.000000 AshCrypt-1.2.3/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 02:37:56.000000 AshCrypt-1.2.3/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.2.3/LICENSE
--rw-rw-rw-   0        0        0    19499 2023-07-01 02:37:57.000939 AshCrypt-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    21571 2023-07-01 02:35:10.000000 AshCrypt-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 02:37:57.002940 AshCrypt-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1629 2023-07-01 02:35:10.000000 AshCrypt-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.150701 AshCrypt-1.2.4/
+drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.083189 AshCrypt-1.2.4/AshCrypt/
+-rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.2.4/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    35061 2023-07-05 14:19:33.000000 AshCrypt-1.2.4/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.2.4/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.2.4/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.2.4/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.2.4/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.2.4/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.2.4/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.124449 AshCrypt-1.2.4/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1263 2023-07-01 02:23:01.000000 AshCrypt-1.2.4/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1045 2023-06-30 15:01:03.000000 AshCrypt-1.2.4/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.135519 AshCrypt-1.2.4/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.2.4/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.144769 AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.2.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.2.4/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:20:46.099172 AshCrypt-1.2.4/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19466 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-05 14:20:45.000000 AshCrypt-1.2.4/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    19466 2023-07-05 14:20:46.148800 AshCrypt-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 14:20:46.150701 AshCrypt-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-02 21:38:12.000000 AshCrypt-1.2.4/setup.py
```

### Comparing `AshCrypt-1.2.3/AshCrypt/Ash.py` & `AshCrypt-1.2.4/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.2.4/AshCrypt/AshCryptGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import AshCrypt.AshTextCrypt as AT
-import AshCrypt.AshFileCrypt as AF
-import AshCrypt.AshDatabase as AD
+import AshCrypt.TextCrypt as AT
+import AshCrypt.FileCrypt as AF
+import AshCrypt.Database as AD
 import ttkbootstrap as tk
 import AshCrypt.qr as qr
 import secrets
 import os.path
 import string
 import atexit
 import json
@@ -33,18 +33,15 @@
 
 textFrame2 = tk.Frame(master=object , width=500 , height=250)
 textFrame2.place(x=1000 , y=250)
 
 lowerFrame = tk.Frame(master=object, width=1000 ,height=260)
 lowerFrame.place(x=500,y=540)
 
-
-'''--------------------------------------FRAMING DONE--------------------------------------------------------------'''
-
-'''--------------------------------------DATA BASE FRAME STARTED------------------------------------------------'''
+'''--------------------------------------DATABASE FRAME STARTED------------------------------------------------'''
 
 
 databaseFrame = tk.Frame(master=object,height=800, width=500)
 databaseFrame.place(rely=0, relx=0)
 
 console_label = tk.Label(master=databaseFrame, text='DATABASE OUTPUT CONSOLE', font='Terminal 15 bold')
 console_label.place( relx=0.09,rely=0.04)
@@ -235,18 +232,14 @@
 content_id_entry = tk.Entry(master=databaseFrame,textvariable=content_id_entry_var,width=3,font='Calibre 11')
 content_id_entry.place(relx=0.45,rely=0.93)
 
 show_content_by_id_button = tk.Button(master=databaseFrame,text='SHOW CONTENT BY ID',command=show_content_by_id,bootstyle='warning outline')
 show_content_by_id_button.place(relx=0.562,rely=0.93)
 
 
-
-'''--------------------------------------DATA BASE FRAME ENDED------------------------------------------------'''
-
-
 '''----------------------------------------LOWER FRAME STARTED----------------------------------'''
 
 
 
 lowerFrame = tk.Frame(master=object, width=1000 ,height=260)
 lowerFrame.place(x=500,y=540)
 
@@ -505,26 +498,17 @@
 
 
 
 
 swich_db_toggle.place(relx=0.47,rely=0.413)
 
 
-'''----------------------------------------LOWER FRAME ENDED----------------------------------'''
-
-
-
-
-
-
 '''-------------------------------TEXT DECRYPTION/ENCRYPTION STARTED---------------------------------------------------'''
 
 
-
-
 def encryption():
     m = inputfield1_1.get()
     if AF.CryptFile.keyverify(mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if len(m) > 200 :
             outputvar1.set('Too Long')
         else :
             if inputfield1_1.get():
@@ -631,23 +615,14 @@
 
 progressbar = tk.Progressbar(master=textFrame1,mode='indeterminate',style='secondary',length=100,)
 progressbar.place(relx=0.05,rely=0.34)
 
 progressbar2 = tk.Progressbar(master=textFrame2,mode='indeterminate',style='secondary',length=100,)
 progressbar2.place(relx=0.05,rely=0.42)
 
-'''-------------------------------TEXT DECRYPTION/ENCRYPTION ENDED---------------------------------------------------'''
-
-
-
-
-
-
-
-
 
 '''-------------------------------FILE ENCRYPTION/DECRYPTION STARTED--------------------------------------------'''
 
 
 filepathlabel = tk.Label(master=frameFile1 ,
                       text='FILE PATH',
                       font='Calibre 20 bold' ,
@@ -856,44 +831,32 @@
 
 def genMainKey():
     keyGenVar.set(AF.CryptFile.genkey())
 
 
 keyGenVar = tk.StringVar(value='')
 keyGenEntry = tk.Entry(master=frameFile2 ,
-                        font='terminal 15 bold',
+                        font='arial 15 ',
                         textvariable=keyGenVar,
-                        width=14,
-                        show='').place(relx=0.1 ,rely=0.69)
+                        width=18).place(relx=0.1 ,rely=0.69)
 
 keyButton = tk.Button(master=frameFile2 ,
                       text='GENERATE',
                       command=genMainKey,
                       bootstyle='success outline').place(relx=0.671, rely=0.7)
 
 
-'''-------------------------------FILE ENCRYPTION/DECRYPTION ENDED--------------------------------------------'''
-
-
-
-
-
-
 '''---------------------------------------STAMP STARTED -------------------------------------------------------'''
 
 
 latest_ID_key_label = tk.Label(master=lowerFrame,text='GitHub.com/AshGw/AES-256', font='Calibre 6')
 latest_ID_key_label.place(relx=0.84,rely=0.92)
 
 '''---------------------------------------STAMP ENDED-------------------------------------------------------'''
 
-
-
-
-
 def rm_json():
     global usable_real_path
     file = os.path.join(usable_real_path,'output.json')
     if os.path.exists(file):
         os.remove(file)
 
 def rm_qr():
```

### Comparing `AshCrypt-1.2.3/AshCrypt/AshDatabase.py` & `AshCrypt-1.2.4/AshCrypt/Database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.2.4/AshCrypt/FileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.2.4/AshCrypt/TextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/AshCrypt/CliCrypt.py` & `AshCrypt-1.2.4/AshCrypt/CliCrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from AshCrypt import AshFileCrypt as AF
-from AshCrypt import AshTextCrypt as A
+from AshCrypt import FileCrypt as AF
+from AshCrypt import TextCrypt as A
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n\tq: to quit the program \n\tc : view commands\n\te: for encryption\n\td : for decryption\n' \
```

### Comparing `AshCrypt-1.2.3/AshCrypt/README.md` & `AshCrypt-1.2.4/AshCrypt/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
 <br>check `GUI` header for more info.
 
 
 ### For Developers ###
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for `AshFileCrypt` and `AshTextCrypt` to learn more.
+view the headers for `FileCrypt` and `TextCrypt` to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
-Check `AshDatabase` header to learn more.
+Check `Database` header to learn more.
 
 **After the library is installed**
 <br>to run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 To run the CLI
@@ -107,22 +107,22 @@
 - HMAC : 256 bit hashed using SHA512
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `AshTextCrypt` and `AshFileCrypt` you have to use a 512 bit long key )
+- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `TextCrypt` and `FileCrypt` you have to use a 512 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
-<br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
+<br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
 
 
 ## AshCryptGUI ##
 The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
@@ -159,15 +159,15 @@
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 
 
 
 
-## AshFileCrypt ## 
+## FileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
 ```python
@@ -206,15 +206,15 @@
 instance1.decrypt()
 ```
 **Note** : 
 <br>Sometimes you might forget that you've applied  `encrypt()` more than one time , so when you try to `decrypt()` the file ,  the output is 1 but the file content is still in binary, just apply the function `decrypt()` the same number of times you applied `encrypt()`.
 
 
 That's it, if you follow the steps above then everything should work just fine.
-## AshTextCrypt ## 
+## TextCrypt ## 
 Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
 ```python
 instance1 = Crypt('Hello Wold !',key)
 ```
 ```python
 instance1.encrypt()[1]
 ```
@@ -223,30 +223,30 @@
 ```
 The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occured.
 <br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
 
 **Note**:
 <br>Unlike the `Ash` library where if you try to decrypt a non-encrypted message you get all kinds of errors.
 
-in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
+in `FileCryt` & `TextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
-## AshDatabase ##
+## Database ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
 
-**Note** that in `AshDatabase.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
+**Note** that in `Database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 
 ### Usage ## 
 In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two deafult columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferrably off-grid and completely seprerate from any vulnerable devices, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
```

### Comparing `AshCrypt-1.2.3/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.2.4/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jun 30 15:01:03 2023 UTC, .py size: 5157 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,404 +1,396 @@
-00000000: 610d 0d0a 0000 0000 2fee 9e64 2514 0000  a......./..d%...
+00000000: 610d 0d0a 0000 0000 e6cf a164 7913 0000  a..........dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c04  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6406 6c09 5a0c 6400  m.Z...d.d.l.Z.d.
 00000080: 6406 6c0d 5a0d 6400 6406 6c0e 5a0e 6400  d.l.Z.d.d.l.Z.d.
 00000090: 6406 6c0f 5a0f 6400 6406 6c10 5a10 4700  d.l.Z.d.d.l.Z.G.
 000000a0: 6407 6408 8400 6408 6511 8303 5a12 4700  d.d...d.e...Z.G.
 000000b0: 6409 640a 8400 640a 8302 5a13 4700 640b  d.d...d...Z.G.d.
 000000c0: 640c 8400 640c 6511 8303 5a14 4700 640d  d...d.e...Z.G.d.
-000000d0: 640e 8400 640e 8302 5a15 6516 640f 6b02  d...d...Z.e.d.k.
-000000e0: 72d8 6410 5a17 6513 a018 a100 5a19 6513  r.d.Z.e.....Z.e.
-000000f0: 6517 6519 6411 8d02 5a1a 651b 651a a01c  e.e.d...Z.e.e...
-00000100: a100 8301 0100 6406 5300 2912 e900 0000  ......d.S.).....
-00000110: 0029 03da 0643 6970 6865 72da 0a61 6c67  .)...Cipher..alg
-00000120: 6f72 6974 686d 73da 056d 6f64 6573 2901  orithms..modes).
-00000130: da07 7061 6464 696e 6729 01da 0f64 6566  ..padding)...def
-00000140: 6175 6c74 5f62 6163 6b65 6e64 2902 da06  ault_backend)...
-00000150: 6861 7368 6573 da04 686d 6163 2901 da05  hashes..hmac)...
-00000160: 556e 696f 6e4e 6300 0000 0000 0000 0000  UnionNc.........
-00000170: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-00000180: 2400 0000 6500 5a01 6400 5a02 6503 6401  $...e.Z.d.Z.e.d.
-00000190: 6402 9c02 8700 6601 6403 6404 840c 5a04  d.....f.d.d...Z.
-000001a0: 8700 0400 5a05 5300 2905 da1a 4974 6572  ....Z.S.)...Iter
-000001b0: 6174 696f 6e73 4f75 746f 6661 5261 6e67  ationsOutofaRang
-000001c0: 6545 7272 6f72 4e29 02da 036e 756d da06  eErrorN)...num..
-000001d0: 7265 7475 726e 6302 0000 0000 0000 0000  returnc.........
-000001e0: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
-000001f0: 2000 0000 6401 7c01 9b00 6402 9d03 7c00   ...d.|...d...|.
-00000200: 5f00 7401 8300 a002 7c00 6a00 a101 0100  _.t.....|.j.....
-00000210: 6400 5300 2903 4e7a 3549 7465 7261 7469  d.S.).Nz5Iterati
-00000220: 6f6e 7320 6d75 7374 2062 6520 6265 7477  ons must be betw
-00000230: 6565 6e20 3530 2061 6e64 2031 3030 3030  een 50 and 10000
-00000240: 302e 2052 4543 4549 5645 4420 3a20 fa01  0. RECEIVED : ..
-00000250: 20a9 03da 0764 6973 706c 6179 da05 7375   ....display..su
-00000260: 7065 72da 085f 5f69 6e69 745f 5f29 02da  per..__init__)..
-00000270: 0473 656c 6672 0b00 0000 a901 da09 5f5f  .selfr........__
-00000280: 636c 6173 735f 5fa9 00fa 2a43 3a5c 576f  class__...*C:\Wo
-00000290: 726b 5c47 6974 4875 6257 6f72 6b5c 4145  rk\GitHubWork\AE
-000002a0: 532d 3235 365c 4173 6843 7279 7074 5c41  S-256\AshCrypt\A
-000002b0: 7368 2e70 7972 1100 0000 0d00 0000 7304  sh.pyr........s.
-000002c0: 0000 0000 010e 017a 2349 7465 7261 7469  .......z#Iterati
-000002d0: 6f6e 734f 7574 6f66 6152 616e 6765 4572  onsOutofaRangeEr
-000002e0: 726f 722e 5f5f 696e 6974 5f5f 2906 da08  ror.__init__)...
-000002f0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000300: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000310: 5f5f da03 616e 7972 1100 0000 da0d 5f5f  __..anyr......__
-00000320: 636c 6173 7363 656c 6c5f 5f72 1500 0000  classcell__r....
-00000330: 7215 0000 0072 1300 0000 7216 0000 0072  r....r....r....r
-00000340: 0a00 0000 0c00 0000 7302 0000 0008 0172  ........s......r
-00000350: 0a00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000360: 0000 0000 0006 0000 0040 0000 0073 bc00  .........@...s..
-00000370: 0000 6500 5a01 6400 5a02 6503 6504 6505  ..e.Z.d.Z.e.e.e.
-00000380: 6602 1900 6504 6401 6402 9c03 6403 6404  f...e.d.d...d.d.
-00000390: 8404 5a06 6507 6504 6505 6508 6505 6405  ..Z.e.e.e.e.e.d.
-000003a0: 9c04 6406 6407 8404 8301 5a09 6507 6504  ..d.d.....Z.e.e.
-000003b0: 6408 9c01 6409 640a 8404 8301 5a0a 640b  d...d.d.....Z.d.
-000003c0: 640c 8400 5a0b 640d 640e 8400 5a0c 640f  d...Z.d.d...Z.d.
-000003d0: 6410 8400 5a0d 6505 6408 9c01 6411 6412  d...Z.e.d...d.d.
-000003e0: 8404 5a0e 6505 6408 9c01 6413 6414 8404  ..Z.e.d...d.d...
-000003f0: 5a0f 6505 6408 9c01 6415 6416 8404 5a10  Z.e.d...d.d...Z.
-00000400: 6505 6408 9c01 6417 6418 8404 5a11 6505  e.d...d.d...Z.e.
-00000410: 6408 9c01 6419 641a 8404 5a12 6504 6408  d...d.d...Z.e.d.
-00000420: 9c01 641b 641c 8404 5a13 6401 5300 291d  ..d.d...Z.d.S.).
-00000430: da03 456e 634e a903 da07 6d65 7373 6167  ..EncN....messag
-00000440: 65da 076d 6169 6e6b 6579 720c 0000 0063  e..mainkeyr....c
-00000450: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000460: 0500 0000 4300 0000 73a4 0000 0074 007c  ....C...s....t.|
-00000470: 0174 0183 0272 167c 01a0 02a1 007c 005f  .t...r.|.....|._
-00000480: 036e 1074 007c 0174 0483 0272 267c 017c  .n.t.|.t...r&|.|
-00000490: 005f 037c 027c 005f 0574 06a0 0764 01a1  ._.|.|._.t...d..
-000004a0: 017c 005f 0874 06a0 0764 01a1 017c 005f  .|._.t...d...|._
-000004b0: 0974 06a0 0764 01a1 017c 005f 0a64 027c  .t...d...|._.d.|
-000004c0: 005f 0b7c 006a 0b64 026b 0073 6a7c 006a  ._.|.j.d.k.sj|.j
-000004d0: 0b64 036b 0472 7474 0c7c 006a 0b83 0182  .d.k.rtt.|.j....
-000004e0: 017c 00a0 0d7c 006a 057c 006a 097c 006a  .|...|.j.|.j.|.j
-000004f0: 0ba1 037c 005f 0e7c 00a0 0d7c 006a 057c  ...|._.|...|.j.|
-00000500: 006a 0a7c 006a 0ba1 037c 005f 0f64 0053  .j.|.j...|._.d.S
-00000510: 0029 044e e910 0000 00e9 3200 0000 e9a0  .).N......2.....
-00000520: 8601 0029 10da 0a69 7369 6e73 7461 6e63  ...)...isinstanc
-00000530: 65da 0373 7472 da06 656e 636f 6465 721e  e..str..encoder.
-00000540: 0000 00da 0562 7974 6573 721f 0000 00da  .....bytesr.....
-00000550: 026f 73da 0775 7261 6e64 6f6d da02 6976  .os..urandom..iv
-00000560: da04 7361 6c74 da06 7065 7070 6572 da0a  ..salt..pepper..
-00000570: 6974 6572 6174 696f 6e73 720a 0000 00da  iterationsr.....
-00000580: 0664 6572 6b65 79da 0665 6e63 4b65 79da  .derkey..encKey.
-00000590: 0868 6d61 635f 6b65 7929 0372 1200 0000  .hmac_key).r....
-000005a0: 721e 0000 0072 1f00 0000 7215 0000 0072  r....r....r....r
-000005b0: 1500 0000 7216 0000 0072 1100 0000 1200  ....r....r......
-000005c0: 0000 731a 0000 0000 010a 010c 010a 0106  ..s.............
-000005d0: 0206 010c 010c 010c 0106 0114 010a 0116  ................
-000005e0: 017a 0c45 6e63 2e5f 5f69 6e69 745f 5f29  .z.Enc.__init__)
-000005f0: 0472 1f00 0000 da0b 7361 6c74 5f70 6570  .r......salt_pep
-00000600: 7065 7272 2c00 0000 720c 0000 0063 0300  perr,...r....c..
-00000610: 0000 0000 0000 0000 0000 0300 0000 0600  ................
-00000620: 0000 4300 0000 7318 0000 0074 006a 017c  ..C...s....t.j.|
-00000630: 00a0 0264 01a1 017c 0164 027c 0264 038d  ...d...|.d.|.d..
-00000640: 0453 0029 044e fa05 5554 462d 38e9 2000  .S.).N..UTF-8. .
-00000650: 0000 2904 5a08 7061 7373 776f 7264 722a  ..).Z.passwordr*
-00000660: 0000 005a 1164 6573 6972 6564 5f6b 6579  ...Z.desired_key
-00000670: 5f62 7974 6573 da06 726f 756e 6473 2903  _bytes..rounds).
-00000680: da06 6263 7279 7074 5a03 6b64 6672 2500  ..bcryptZ.kdfr%.
-00000690: 0000 2903 721f 0000 0072 3000 0000 722c  ..).r....r0...r,
-000006a0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000006b0: 0000 722d 0000 0022 0000 0073 0c00 0000  ..r-..."...s....
-000006c0: 0002 0401 0801 0201 0201 02fc 7a0a 456e  ............z.En
-000006d0: 632e 6465 726b 6579 a901 720c 0000 0063  c.derkey..r....c
-000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006f0: 0300 0000 4300 0000 730e 0000 0074 00a0  ....C...s....t..
-00000700: 0164 01a1 01a0 02a1 0053 0029 024e e940  .d.......S.).N.@
-00000710: 0000 0029 0372 2700 0000 7228 0000 00da  ...).r'...r(....
-00000720: 0368 6578 7215 0000 0072 1500 0000 7215  .hexr....r....r.
-00000730: 0000 0072 1600 0000 da0a 6765 6e4d 6169  ...r......genMai
-00000740: 6e6b 6579 2a00 0000 7302 0000 0000 027a  nkey*...s......z
-00000750: 0e45 6e63 2e67 656e 4d61 696e 6b65 7963  .Enc.genMainkeyc
-00000760: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000770: 0300 0000 4300 0000 730c 0000 0074 00a0  ....C...s....t..
-00000780: 017c 006a 02a1 0153 00a9 014e 2903 7204  .|.j...S...N).r.
-00000790: 0000 00da 0343 4243 7229 0000 00a9 0172  .....CBCr).....r
-000007a0: 1200 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000007b0: 0000 00da 046d 6f64 652e 0000 0073 0200  .....mode....s..
-000007c0: 0000 0001 7a08 456e 632e 6d6f 6465 6301  ....z.Enc.modec.
-000007d0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-000007e0: 0000 0043 0000 0073 1e00 0000 7400 7401  ...C...s....t.t.
-000007f0: 6a02 7c00 6a03 6401 8d01 7c00 a004 a100  j.|.j.d...|.....
-00000800: 7405 8300 6402 8d03 5300 a903 4e29 01da  t...d...S...N)..
-00000810: 036b 6579 2902 723c 0000 005a 0762 6163  .key).r<...Z.bac
-00000820: 6b65 6e64 2906 7202 0000 0072 0300 0000  kend).r....r....
-00000830: da03 4145 5372 2e00 0000 723c 0000 0072  ..AESr....r<...r
-00000840: 0600 0000 723b 0000 0072 1500 0000 7215  ....r;...r....r.
-00000850: 0000 0072 1600 0000 da06 6369 7068 6572  ...r......cipher
-00000860: 3100 0000 7302 0000 0000 017a 0a45 6e63  1...s......z.Enc
-00000870: 2e63 6970 6865 7263 0100 0000 0000 0000  .cipherc........
-00000880: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000890: 730c 0000 007c 00a0 00a1 00a0 01a1 0053  s....|.........S
-000008a0: 0072 3900 0000 2902 7240 0000 005a 0965  .r9...).r@...Z.e
-000008b0: 6e63 7279 7074 6f72 723b 0000 0072 1500  ncryptorr;...r..
-000008c0: 0000 7215 0000 0072 1600 0000 da10 6369  ..r....r......ci
-000008d0: 7068 6572 5f65 6e63 7279 7074 6f72 3400  pher_encryptor4.
-000008e0: 0000 7302 0000 0000 017a 1445 6e63 2e63  ..s......z.Enc.c
-000008f0: 6970 6865 725f 656e 6372 7970 746f 7263  ipher_encryptorc
-00000900: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000910: 0300 0000 4300 0000 7322 0000 0074 00a0  ....C...s"...t..
-00000920: 0164 01a1 01a0 02a1 007d 017c 01a0 037c  .d.......}.|...|
-00000930: 006a 04a1 017c 01a0 05a1 0017 0053 00a9  .j...|.......S..
-00000940: 024e e980 0000 0029 0672 0500 0000 da05  .N.....).r......
-00000950: 504b 4353 37da 0670 6164 6465 72da 0675  PKCS7..padder..u
-00000960: 7064 6174 6572 1e00 0000 da08 6669 6e61  pdater......fina
-00000970: 6c69 7a65 2902 7212 0000 0072 4500 0000  lize).r....rE...
-00000980: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00000990: 0e70 6164 6465 645f 6d65 7373 6167 6537  .padded_message7
-000009a0: 0000 0073 0400 0000 0001 0e01 7a12 456e  ...s........z.En
-000009b0: 632e 7061 6464 6564 5f6d 6573 7361 6765  c.padded_message
-000009c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000009d0: 0004 0000 0043 0000 0073 1e00 0000 7c00  .....C...s....|.
-000009e0: a000 a100 a001 7c00 a002 a100 a101 7c00  ......|.......|.
-000009f0: a000 a100 a003 a100 1700 5300 7239 0000  ..........S.r9..
-00000a00: 0029 0472 4100 0000 7246 0000 0072 4800  .).rA...rF...rH.
-00000a10: 0000 7247 0000 0072 3b00 0000 7215 0000  ..rG...r;...r...
-00000a20: 0072 1500 0000 7216 0000 00da 0a63 6970  .r....r......cip
-00000a30: 6865 7274 6578 743b 0000 0073 0200 0000  hertext;...s....
-00000a40: 0001 7a0e 456e 632e 6369 7068 6572 7465  ..z.Enc.cipherte
-00000a50: 7874 6301 0000 0000 0000 0000 0000 0002  xtc.............
-00000a60: 0000 0005 0000 0043 0000 0073 2c00 0000  .......C...s,...
-00000a70: 7c00 6a00 7d01 7401 a002 7c01 7403 a004  |.j.}.t...|.t...
-00000a80: a100 a102 7d01 7c01 a005 7c00 a006 a100  ....}.|...|.....
-00000a90: a101 0100 7c01 a007 a100 5300 7239 0000  ....|.....S.r9..
-00000aa0: 0029 0872 2f00 0000 7208 0000 00da 0448  .).r/...r......H
-00000ab0: 4d41 4372 0700 0000 da06 5348 4135 3132  MACr......SHA512
-00000ac0: 7246 0000 0072 4900 0000 7247 0000 00a9  rF...rI...rG....
-00000ad0: 0272 1200 0000 da01 6872 1500 0000 7215  .r......hr....r.
-00000ae0: 0000 0072 1600 0000 724a 0000 003e 0000  ...r....rJ...>..
-00000af0: 0073 0800 0000 0001 0601 1001 0e01 7a08  .s............z.
-00000b00: 456e 632e 484d 4143 6301 0000 0000 0000  Enc.HMACc.......
-00000b10: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000b20: 0073 1200 0000 7400 a001 6401 7c00 6a02  .s....t...d.|.j.
-00000b30: a102 7d01 7c01 5300 2902 4efa 0221 4929  ..}.|.S.).N..!I)
-00000b40: 03da 0673 7472 7563 745a 0470 6163 6b72  ...structZ.packr
-00000b50: 2c00 0000 2902 7212 0000 005a 0b69 7465  ,...).r....Z.ite
-00000b60: 7273 5f62 7974 6573 7215 0000 0072 1500  rs_bytesr....r..
-00000b70: 0000 7216 0000 00da 0f73 6574 7570 4974  ..r......setupIt
-00000b80: 6572 6174 696f 6e73 4400 0000 7304 0000  erationsD...s...
-00000b90: 0000 010e 017a 1345 6e63 2e73 6574 7570  .....z.Enc.setup
-00000ba0: 4974 6572 6174 696f 6e73 6301 0000 0000  Iterationsc.....
-00000bb0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000bc0: 0000 0073 2a00 0000 7c00 a000 a100 7c00  ...s*...|.....|.
-00000bd0: 6a01 1700 7c00 6a02 1700 7c00 6a03 1700  j...|.j...|.j...
-00000be0: 7c00 a004 a100 1700 7c00 a005 a100 1700  |.......|.......
-00000bf0: 5300 7239 0000 0029 0672 4a00 0000 7229  S.r9...).rJ...r)
-00000c00: 0000 0072 2a00 0000 722b 0000 0072 5000  ...r*...r+...rP.
-00000c10: 0000 7249 0000 0072 3b00 0000 7215 0000  ..rI...r;...r...
-00000c20: 0072 1500 0000 7216 0000 00da 0a65 6e63  .r....r......enc
-00000c30: 546f 4279 7465 7348 0000 0073 0200 0000  ToBytesH...s....
-00000c40: 0001 7a0e 456e 632e 656e 6354 6f42 7974  ..z.Enc.encToByt
-00000c50: 6573 6301 0000 0000 0000 0000 0000 0001  esc.............
-00000c60: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
-00000c70: 7400 a001 7c00 a002 a100 a101 a003 6401  t...|.........d.
-00000c80: a101 5300 a902 4e72 3100 0000 2904 da06  ..S...Nr1...)...
-00000c90: 6261 7365 3634 5a11 7572 6c73 6166 655f  base64Z.urlsafe_
-00000ca0: 6236 3465 6e63 6f64 6572 5100 0000 da06  b64encoderQ.....
-00000cb0: 6465 636f 6465 723b 0000 0072 1500 0000  decoder;...r....
-00000cc0: 7215 0000 0072 1600 0000 da08 656e 6354  r....r......encT
-00000cd0: 6f53 7472 4b00 0000 7302 0000 0000 017a  oStrK...s......z
-00000ce0: 0c45 6e63 2e65 6e63 546f 5374 7229 1472  .Enc.encToStr).r
-00000cf0: 1700 0000 7218 0000 0072 1900 0000 7209  ....r....r....r.
-00000d00: 0000 0072 2400 0000 7226 0000 0072 1100  ...r$...r&...r..
-00000d10: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
-00000d20: da03 696e 7472 2d00 0000 7238 0000 0072  ..intr-...r8...r
-00000d30: 3c00 0000 7240 0000 0072 4100 0000 7248  <...r@...rA...rH
-00000d40: 0000 0072 4900 0000 724a 0000 0072 5000  ...rI...rJ...rP.
-00000d50: 0000 7251 0000 0072 5500 0000 7215 0000  ..rQ...rU...r...
-00000d60: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000d70: 721c 0000 0011 0000 0073 1c00 0000 0801  r........s......
-00000d80: 1a10 0201 1607 0201 1003 0803 0803 0803  ................
-00000d90: 0e04 0e03 0e06 0e04 0e03 721c 0000 0063  ..........r....c
-00000da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000db0: 0400 0000 0000 0000 7322 0000 0065 005a  ........s"...e.Z
-00000dc0: 0164 005a 0264 0164 029c 0187 0066 0164  .d.Z.d.d.....f.d
-00000dd0: 0364 0484 0c5a 0387 0004 005a 0453 0029  .d...Z.....Z.S.)
-00000de0: 05da 154d 6573 7361 6765 5461 6d70 6572  ...MessageTamper
-00000df0: 696e 6745 7272 6f72 4e72 3500 0000 6301  ingErrorNr5...c.
-00000e00: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000e10: 0000 0003 0000 0073 1800 0000 6401 7c00  .......s....d.|.
-00000e20: 5f00 7401 8300 a002 7c00 6a00 a101 0100  _.t.....|.j.....
-00000e30: 6400 5300 2902 4e7a 4c48 4d41 4320 6d69  d.S.).NzLHMAC mi
-00000e40: 736d 6174 6368 2021 204d 6573 7361 6765  smatch ! Message
-00000e50: 2068 6173 2062 6565 6e20 5441 4d50 4552   has been TAMPER
-00000e60: 4544 2077 6974 6820 2c0a 206f 7220 506f  ED with ,. or Po
-00000e70: 7373 6962 6c65 206b 6579 2064 6966 6665  ssible key diffe
-00000e80: 7265 6e63 6572 0e00 0000 723b 0000 0072  rencer....r;...r
-00000e90: 1300 0000 7215 0000 0072 1600 0000 7211  ....r....r....r.
-00000ea0: 0000 0050 0000 0073 0400 0000 0001 0601  ...P...s........
-00000eb0: 7a1e 4d65 7373 6167 6554 616d 7065 7269  z.MessageTamperi
-00000ec0: 6e67 4572 726f 722e 5f5f 696e 6974 5f5f  ngError.__init__
-00000ed0: 2905 7217 0000 0072 1800 0000 7219 0000  ).r....r....r...
-00000ee0: 0072 1100 0000 721b 0000 0072 1500 0000  .r....r....r....
-00000ef0: 7215 0000 0072 1300 0000 7216 0000 0072  r....r....r....r
-00000f00: 5800 0000 4f00 0000 7302 0000 0008 0172  X...O...s......r
-00000f10: 5800 0000 6300 0000 0000 0000 0000 0000  X...c...........
-00000f20: 0000 0000 0004 0000 0040 0000 0073 9200  .........@...s..
-00000f30: 0000 6500 5a01 6400 5a02 6503 6504 6505  ..e.Z.d.Z.e.e.e.
-00000f40: 6602 1900 6504 6401 6402 9c03 6403 6404  f...e.d.d...d.d.
-00000f50: 8404 5a06 6505 6405 9c01 6406 6407 8404  ..Z.e.d...d.d...
-00000f60: 5a07 6508 6405 9c01 6408 6409 8404 5a09  Z.e.d...d.d...Z.
-00000f70: 640a 640b 8400 5a0a 640c 640d 8400 5a0b  d.d...Z.d.d...Z.
-00000f80: 640e 640f 8400 5a0c 6505 6405 9c01 6410  d.d...Z.e.d...d.
-00000f90: 6411 8404 5a0d 6505 6405 9c01 6412 6413  d...Z.e.d...d.d.
-00000fa0: 8404 5a0e 6505 6405 9c01 6414 6415 8404  ..Z.e.d...d.d...
-00000fb0: 5a0f 6504 6405 9c01 6416 6417 8404 5a10  Z.e.d...d.d...Z.
-00000fc0: 6401 5300 2918 da03 4465 634e 721d 0000  d.S.)...DecNr...
-00000fd0: 0063 0300 0000 0000 0000 0000 0000 0400  .c..............
-00000fe0: 0000 0600 0000 4300 0000 7306 0100 0074  ......C...s....t
-00000ff0: 007c 0174 0183 0272 227c 01a0 0264 01a1  .|.t...r"|...d..
-00001000: 017d 0374 03a0 047c 03a1 017c 005f 056e  .}.t...|...|._.n
-00001010: 1074 007c 0174 0683 0272 327c 017c 005f  .t.|.t...r2|.|._
-00001020: 057c 027c 005f 077c 006a 0564 0064 0285  .|.|._.|.j.d.d..
-00001030: 0219 007c 005f 087c 006a 0564 0264 0385  ...|._.|.j.d.d..
-00001040: 0219 007c 005f 097c 006a 0564 0364 0485  ...|._.|.j.d.d..
-00001050: 0219 007c 005f 0a7c 006a 0564 0464 0585  ...|._.|.j.d.d..
-00001060: 0219 007c 005f 0b74 0ca0 0d64 067c 006a  ...|._.t...d.|.j
-00001070: 0564 0564 0785 0219 00a1 0264 0819 007c  .d.d.......d...|
-00001080: 005f 0e7c 006a 0e64 096b 0073 a87c 006a  ._.|.j.d.k.s.|.j
-00001090: 0e64 0a6b 0472 b274 0f7c 006a 0e83 0182  .d.k.r.t.|.j....
-000010a0: 017c 006a 0564 0764 0085 0219 007c 005f  .|.j.d.d.....|._
-000010b0: 1074 11a0 127c 006a 077c 006a 0a7c 006a  .t...|.j.|.j.|.j
-000010c0: 0ea1 037c 005f 1374 11a0 127c 006a 077c  ...|._.t...|.j.|
-000010d0: 006a 0b7c 006a 0ea1 037c 005f 147c 00a0  .j.|.j...|._.|..
-000010e0: 15a1 0064 0b75 0090 0172 0274 1683 0082  ...d.u...r.t....
-000010f0: 0164 0053 0029 0c4e 7231 0000 0072 3600  .d.S.).Nr1...r6.
-00001100: 0000 e950 0000 00e9 6000 0000 e970 0000  ...P....`....p..
-00001110: 0072 4e00 0000 e974 0000 0072 0100 0000  .rN....t...r....
-00001120: 7221 0000 0072 2200 0000 4629 1772 2300  r!...r"...F).r#.
-00001130: 0000 7224 0000 0072 2500 0000 7253 0000  ..r$...r%...rS..
-00001140: 005a 1175 726c 7361 6665 5f62 3634 6465  .Z.urlsafe_b64de
-00001150: 636f 6465 721e 0000 0072 2600 0000 723e  coder....r&...r>
-00001160: 0000 00da 0872 6563 5f68 6d61 63da 0672  .....rec_hmac..r
-00001170: 6563 5f69 765a 0872 6563 5f73 616c 745a  ec_ivZ.rec_saltZ
-00001180: 0a72 6563 5f70 6570 7065 7272 4f00 0000  .rec_pepperrO...
-00001190: 5a06 756e 7061 636b 5a0e 7265 635f 6974  Z.unpackZ.rec_it
-000011a0: 6572 6174 696f 6e73 720a 0000 00da 0e72  erationsr......r
-000011b0: 6563 5f63 6970 6865 7274 6578 7472 1c00  ec_ciphertextr..
-000011c0: 0000 722d 0000 00da 0664 6563 4b65 79da  ..r-.....decKey.
-000011d0: 0668 6d61 635f 6bda 0a76 6572 6966 7948  .hmac_k..verifyH
-000011e0: 4d41 4372 5800 0000 2904 7212 0000 0072  MACrX...).r....r
-000011f0: 1e00 0000 721f 0000 00da 016d 7215 0000  ....r......mr...
-00001200: 0072 1500 0000 7216 0000 0072 1100 0000  .r....r....r....
-00001210: 5500 0000 7324 0000 0000 010a 010a 010e  U...s$..........
-00001220: 010a 0106 0106 0110 0110 0110 0110 011c  ................
-00001230: 0114 010a 0110 0116 0116 010e 017a 0c44  .............z.D
-00001240: 6563 2e5f 5f69 6e69 745f 5f72 3500 0000  ec.__init__r5...
-00001250: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001260: 0005 0000 0043 0000 0073 2a00 0000 7c00  .....C...s*...|.
-00001270: 6a00 7d01 7401 a002 7c01 7403 a004 a100  j.}.t...|.t.....
-00001280: a102 7d01 7c01 a005 7c00 6a06 a101 0100  ..}.|...|.j.....
-00001290: 7c01 a007 a100 5300 7239 0000 0029 0872  |.....S.r9...).r
-000012a0: 6200 0000 7208 0000 0072 4a00 0000 7207  b...r....rJ...r.
-000012b0: 0000 0072 4b00 0000 7246 0000 0072 6000  ...rK...rF...r`.
-000012c0: 0000 7247 0000 0072 4c00 0000 7215 0000  ..rG...rL...r...
-000012d0: 0072 1500 0000 7216 0000 00da 0a61 6374  .r....r......act
-000012e0: 7561 6c48 4d41 4368 0000 0073 0800 0000  ualHMACh...s....
-000012f0: 0001 0601 1001 0c01 7a0e 4465 632e 6163  ........z.Dec.ac
-00001300: 7475 616c 484d 4143 6301 0000 0000 0000  tualHMACc.......
-00001310: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00001320: 0073 1200 0000 7400 a001 7c00 a002 a100  .s....t...|.....
-00001330: 7c00 6a03 a102 5300 7239 0000 0029 04da  |.j...S.r9...)..
-00001340: 0368 6d63 5a0e 636f 6d70 6172 655f 6469  .hmcZ.compare_di
-00001350: 6765 7374 7265 0000 0072 5e00 0000 723b  gestre...r^...r;
-00001360: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00001370: 0000 7263 0000 006e 0000 0073 0200 0000  ..rc...n...s....
-00001380: 0001 7a0e 4465 632e 7665 7269 6679 484d  ..z.Dec.verifyHM
-00001390: 4143 6301 0000 0000 0000 0000 0000 0001  ACc.............
-000013a0: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
-000013b0: 7400 a001 7c00 6a02 a101 5300 7239 0000  t...|.j...S.r9..
-000013c0: 0029 0372 0400 0000 723a 0000 0072 5f00  .).r....r:...r_.
-000013d0: 0000 723b 0000 0072 1500 0000 7215 0000  ..r;...r....r...
-000013e0: 0072 1600 0000 723c 0000 0071 0000 0073  .r....r<...q...s
-000013f0: 0200 0000 0001 7a08 4465 632e 6d6f 6465  ......z.Dec.mode
-00001400: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001410: 0005 0000 0043 0000 0073 1e00 0000 7400  .....C...s....t.
-00001420: 7401 6a02 7c00 6a03 6401 8d01 7c00 a004  t.j.|.j.d...|...
-00001430: a100 7405 8300 6402 8d03 5300 723d 0000  ..t...d...S.r=..
-00001440: 0029 0672 0200 0000 7203 0000 0072 3f00  .).r....r....r?.
-00001450: 0000 7261 0000 0072 3c00 0000 7206 0000  ..ra...r<...r...
-00001460: 0072 3b00 0000 7215 0000 0072 1500 0000  .r;...r....r....
-00001470: 7216 0000 0072 4000 0000 7400 0000 7302  r....r@...t...s.
-00001480: 0000 0000 017a 0a44 6563 2e63 6970 6865  .....z.Dec.ciphe
-00001490: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
-000014a0: 0000 0200 0000 4300 0000 730c 0000 007c  ......C...s....|
-000014b0: 00a0 00a1 00a0 01a1 0053 0072 3900 0000  .........S.r9...
-000014c0: 2902 7240 0000 005a 0964 6563 7279 7074  ).r@...Z.decrypt
-000014d0: 6f72 723b 0000 0072 1500 0000 7215 0000  orr;...r....r...
-000014e0: 0072 1600 0000 da10 6369 7068 6572 5f64  .r......cipher_d
-000014f0: 6563 7279 7074 6f72 7700 0000 7302 0000  ecryptorw...s...
-00001500: 0000 017a 1444 6563 2e63 6970 6865 725f  ...z.Dec.cipher_
-00001510: 6465 6372 7970 746f 7263 0100 0000 0000  decryptorc......
-00001520: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001530: 0000 731c 0000 007c 00a0 00a1 00a0 017c  ..s....|.......|
-00001540: 006a 02a1 017c 00a0 00a1 00a0 03a1 0017  .j...|..........
-00001550: 0053 0072 3900 0000 2904 7267 0000 0072  .S.r9...).rg...r
-00001560: 4600 0000 7260 0000 0072 4700 0000 723b  F...r`...rG...r;
-00001570: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00001580: 0000 da11 7072 655f 756e 7061 6464 696e  ....pre_unpaddin
-00001590: 675f 6465 637a 0000 0073 0200 0000 0001  g_decz...s......
-000015a0: 7a15 4465 632e 7072 655f 756e 7061 6464  z.Dec.pre_unpadd
-000015b0: 696e 675f 6465 6363 0100 0000 0000 0000  ing_decc........
-000015c0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-000015d0: 7324 0000 0074 00a0 0164 01a1 01a0 02a1  s$...t...d......
-000015e0: 007d 017c 01a0 037c 00a0 04a1 00a1 017c  .}.|...|.......|
-000015f0: 01a0 05a1 0017 0053 0072 4200 0000 2906  .......S.rB...).
-00001600: 7205 0000 0072 4400 0000 da08 756e 7061  r....rD.....unpa
-00001610: 6464 6572 7246 0000 0072 6800 0000 7247  dderrF...rh...rG
-00001620: 0000 0029 0272 1200 0000 7269 0000 0072  ...).r....ri...r
-00001630: 1500 0000 7215 0000 0072 1600 0000 da0a  ....r....r......
-00001640: 756e 7061 6464 6564 5f6d 7d00 0000 7304  unpadded_m}...s.
-00001650: 0000 0000 010e 017a 0e44 6563 2e75 6e70  .......z.Dec.unp
-00001660: 6164 6465 645f 6d63 0100 0000 0000 0000  added_mc........
-00001670: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00001680: 7308 0000 007c 00a0 00a1 0053 0072 3900  s....|.....S.r9.
-00001690: 0000 2901 726a 0000 0072 3b00 0000 7215  ..).rj...r;...r.
-000016a0: 0000 0072 1500 0000 7216 0000 00da 0a64  ...r....r......d
-000016b0: 6563 546f 4279 7465 7381 0000 0073 0200  ecToBytes....s..
-000016c0: 0000 0001 7a0e 4465 632e 6465 6354 6f42  ....z.Dec.decToB
-000016d0: 7974 6573 6301 0000 0000 0000 0000 0000  ytesc...........
-000016e0: 0001 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
-000016f0: 0000 7c00 a000 a100 a001 6401 a101 5300  ..|.......d...S.
-00001700: 7252 0000 0029 0272 6a00 0000 7254 0000  rR...).rj...rT..
-00001710: 0072 3b00 0000 7215 0000 0072 1500 0000  .r;...r....r....
-00001720: 7216 0000 00da 0864 6563 546f 5374 7284  r......decToStr.
-00001730: 0000 0073 0200 0000 0001 7a0c 4465 632e  ...s......z.Dec.
-00001740: 6465 6354 6f53 7472 2911 7217 0000 0072  decToStr).r....r
-00001750: 1800 0000 7219 0000 0072 0900 0000 7224  ....r....r....r$
-00001760: 0000 0072 2600 0000 7211 0000 0072 6500  ...r&...r....re.
-00001770: 0000 da04 626f 6f6c 7263 0000 0072 3c00  ....boolrc...r<.
-00001780: 0000 7240 0000 0072 6700 0000 7268 0000  ..r@...rg...rh..
-00001790: 0072 6a00 0000 726b 0000 0072 6c00 0000  .rj...rk...rl...
-000017a0: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-000017b0: 1600 0000 7259 0000 0054 0000 0073 1400  ....rY...T...s..
-000017c0: 0000 0801 1a13 0e06 0e03 0803 0803 0803  ................
-000017d0: 0e03 0e04 0e03 7259 0000 00da 085f 5f6d  ......rY.....__m
-000017e0: 6169 6e5f 5f5a 0548 656c 6c6f 2902 721e  ain__Z.Hello).r.
-000017f0: 0000 0072 1f00 0000 291d 5a26 6372 7970  ...r....).Z&cryp
-00001800: 746f 6772 6170 6879 2e68 617a 6d61 742e  tography.hazmat.
-00001810: 7072 696d 6974 6976 6573 2e63 6970 6865  primitives.ciphe
-00001820: 7273 7202 0000 0072 0300 0000 7204 0000  rsr....r....r...
-00001830: 005a 1e63 7279 7074 6f67 7261 7068 792e  .Z.cryptography.
-00001840: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
-00001850: 7372 0500 0000 5a1c 6372 7970 746f 6772  sr....Z.cryptogr
-00001860: 6170 6879 2e68 617a 6d61 742e 6261 636b  aphy.hazmat.back
-00001870: 656e 6473 7206 0000 0072 0700 0000 7208  endsr....r....r.
-00001880: 0000 00da 0674 7970 696e 6772 0900 0000  .....typingr....
-00001890: 7266 0000 0072 3400 0000 7253 0000 0072  rf...r4...rS...r
-000018a0: 4f00 0000 7227 0000 00da 0945 7863 6570  O...r'.....Excep
-000018b0: 7469 6f6e 720a 0000 0072 1c00 0000 7258  tionr....r....rX
-000018c0: 0000 0072 5900 0000 7217 0000 0072 1e00  ...rY...r....r..
-000018d0: 0000 7238 0000 0072 3e00 0000 5a09 696e  ..r8...r>...Z.in
-000018e0: 7374 616e 6365 31da 0570 7269 6e74 7251  stance1..printrQ
-000018f0: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
-00001900: 0000 7216 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00001910: 3e01 0000 0073 2400 0000 1401 0c01 0c01  >....s$.........
-00001920: 1001 0c01 0801 0801 0801 0801 0802 1005  ................
-00001930: 0e3e 1005 0e35 0801 0401 0801 0c01       .>...5........
+000000d0: 640e 8400 640e 8302 5a15 6406 5300 290f  d...d...Z.d.S.).
+000000e0: e900 0000 0029 03da 0643 6970 6865 72da  .....)...Cipher.
+000000f0: 0a61 6c67 6f72 6974 686d 73da 056d 6f64  .algorithms..mod
+00000100: 6573 2901 da07 7061 6464 696e 6729 01da  es)...padding)..
+00000110: 0f64 6566 6175 6c74 5f62 6163 6b65 6e64  .default_backend
+00000120: 2902 da06 6861 7368 6573 da04 686d 6163  )...hashes..hmac
+00000130: 2901 da05 556e 696f 6e4e 6300 0000 0000  )...UnionNc.....
+00000140: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00000150: 0000 0073 2400 0000 6500 5a01 6400 5a02  ...s$...e.Z.d.Z.
+00000160: 6503 6401 6402 9c02 8700 6601 6403 6404  e.d.d.....f.d.d.
+00000170: 840c 5a04 8700 0400 5a05 5300 2905 da1a  ..Z.....Z.S.)...
+00000180: 4974 6572 6174 696f 6e73 4f75 746f 6661  IterationsOutofa
+00000190: 5261 6e67 6545 7272 6f72 4e29 02da 036e  RangeErrorN)...n
+000001a0: 756d da06 7265 7475 726e 6302 0000 0000  um..returnc.....
+000001b0: 0000 0000 0000 0002 0000 0003 0000 0003  ................
+000001c0: 0000 0073 2000 0000 6401 7c01 9b00 6402  ...s ...d.|...d.
+000001d0: 9d03 7c00 5f00 7401 8300 a002 7c00 6a00  ..|._.t.....|.j.
+000001e0: a101 0100 6400 5300 2903 4e7a 3549 7465  ....d.S.).Nz5Ite
+000001f0: 7261 7469 6f6e 7320 6d75 7374 2062 6520  rations must be 
+00000200: 6265 7477 6565 6e20 3530 2061 6e64 2031  between 50 and 1
+00000210: 3030 3030 302e 2052 4543 4549 5645 4420  00000. RECEIVED 
+00000220: 3a20 fa01 20a9 035a 0764 6973 706c 6179  : .. ..Z.display
+00000230: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+00000240: 5f29 02da 0473 656c 6672 0b00 0000 a901  _)...selfr......
+00000250: da09 5f5f 636c 6173 735f 5fa9 00fa 2a43  ..__class__...*C
+00000260: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
+00000270: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
+00000280: 7074 5c41 7368 2e70 7972 1000 0000 0d00  pt\Ash.pyr......
+00000290: 0000 7304 0000 0000 010e 017a 2349 7465  ..s........z#Ite
+000002a0: 7261 7469 6f6e 734f 7574 6f66 6152 616e  rationsOutofaRan
+000002b0: 6765 4572 726f 722e 5f5f 696e 6974 5f5f  geError.__init__
+000002c0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000002d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000002e0: 6e61 6d65 5f5f da03 616e 7972 1000 0000  name__..anyr....
+000002f0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00000300: 1400 0000 7214 0000 0072 1200 0000 7215  ....r....r....r.
+00000310: 0000 0072 0a00 0000 0c00 0000 7302 0000  ...r........s...
+00000320: 0008 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
+00000330: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
+00000340: 0073 bc00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00000350: 6504 6505 6602 1900 6504 6401 6402 9c03  e.e.f...e.d.d...
+00000360: 6403 6404 8404 5a06 6507 6504 6505 6508  d.d...Z.e.e.e.e.
+00000370: 6505 6405 9c04 6406 6407 8404 8301 5a09  e.d...d.d.....Z.
+00000380: 6507 6504 6408 9c01 6409 640a 8404 8301  e.e.d...d.d.....
+00000390: 5a0a 640b 640c 8400 5a0b 640d 640e 8400  Z.d.d...Z.d.d...
+000003a0: 5a0c 640f 6410 8400 5a0d 6505 6408 9c01  Z.d.d...Z.e.d...
+000003b0: 6411 6412 8404 5a0e 6505 6408 9c01 6413  d.d...Z.e.d...d.
+000003c0: 6414 8404 5a0f 6505 6408 9c01 6415 6416  d...Z.e.d...d.d.
+000003d0: 8404 5a10 6505 6408 9c01 6417 6418 8404  ..Z.e.d...d.d...
+000003e0: 5a11 6505 6408 9c01 6419 641a 8404 5a12  Z.e.d...d.d...Z.
+000003f0: 6504 6408 9c01 641b 641c 8404 5a13 6401  e.d...d.d...Z.d.
+00000400: 5300 291d da03 456e 634e a903 da07 6d65  S.)...EncN....me
+00000410: 7373 6167 65da 076d 6169 6e6b 6579 720c  ssage..mainkeyr.
+00000420: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00000430: 0300 0000 0500 0000 4300 0000 73a4 0000  ........C...s...
+00000440: 0074 007c 0174 0183 0272 167c 01a0 02a1  .t.|.t...r.|....
+00000450: 007c 005f 036e 1074 007c 0174 0483 0272  .|._.n.t.|.t...r
+00000460: 267c 017c 005f 037c 027c 005f 0574 06a0  &|.|._.|.|._.t..
+00000470: 0764 01a1 017c 005f 0874 06a0 0764 01a1  .d...|._.t...d..
+00000480: 017c 005f 0974 06a0 0764 01a1 017c 005f  .|._.t...d...|._
+00000490: 0a64 027c 005f 0b7c 006a 0b64 026b 0073  .d.|._.|.j.d.k.s
+000004a0: 6a7c 006a 0b64 036b 0472 7474 0c7c 006a  j|.j.d.k.rtt.|.j
+000004b0: 0b83 0182 017c 00a0 0d7c 006a 057c 006a  .....|...|.j.|.j
+000004c0: 097c 006a 0ba1 037c 005f 0e7c 00a0 0d7c  .|.j...|._.|...|
+000004d0: 006a 057c 006a 0a7c 006a 0ba1 037c 005f  .j.|.j.|.j...|._
+000004e0: 0f64 0053 0029 044e e910 0000 00e9 3200  .d.S.).N......2.
+000004f0: 0000 e9a0 8601 0029 10da 0a69 7369 6e73  .......)...isins
+00000500: 7461 6e63 65da 0373 7472 da06 656e 636f  tance..str..enco
+00000510: 6465 721d 0000 00da 0562 7974 6573 721e  der......bytesr.
+00000520: 0000 00da 026f 73da 0775 7261 6e64 6f6d  .....os..urandom
+00000530: da02 6976 da04 7361 6c74 da06 7065 7070  ..iv..salt..pepp
+00000540: 6572 da0a 6974 6572 6174 696f 6e73 720a  er..iterationsr.
+00000550: 0000 00da 0664 6572 6b65 79da 0665 6e63  .....derkey..enc
+00000560: 4b65 79da 0868 6d61 635f 6b65 7929 0372  Key..hmac_key).r
+00000570: 1100 0000 721d 0000 0072 1e00 0000 7214  ....r....r....r.
+00000580: 0000 0072 1400 0000 7215 0000 0072 1000  ...r....r....r..
+00000590: 0000 1200 0000 731a 0000 0000 010a 010c  ......s.........
+000005a0: 010a 0106 0206 010c 010c 010c 0106 0114  ................
+000005b0: 010a 0116 017a 0c45 6e63 2e5f 5f69 6e69  .....z.Enc.__ini
+000005c0: 745f 5f29 0472 1e00 0000 da0b 7361 6c74  t__).r......salt
+000005d0: 5f70 6570 7065 7272 2b00 0000 720c 0000  _pepperr+...r...
+000005e0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+000005f0: 0000 0600 0000 4300 0000 7318 0000 0074  ......C...s....t
+00000600: 006a 017c 00a0 0264 01a1 017c 0164 027c  .j.|...d...|.d.|
+00000610: 0264 038d 0453 0029 044e fa05 5554 462d  .d...S.).N..UTF-
+00000620: 38e9 2000 0000 2904 5a08 7061 7373 776f  8. ...).Z.passwo
+00000630: 7264 7229 0000 005a 1164 6573 6972 6564  rdr)...Z.desired
+00000640: 5f6b 6579 5f62 7974 6573 da06 726f 756e  _key_bytes..roun
+00000650: 6473 2903 da06 6263 7279 7074 5a03 6b64  ds)...bcryptZ.kd
+00000660: 6672 2400 0000 2903 721e 0000 0072 2f00  fr$...).r....r/.
+00000670: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
+00000680: 0072 1500 0000 722c 0000 0022 0000 0073  .r....r,..."...s
+00000690: 0c00 0000 0002 0401 0801 0201 0201 02fc  ................
+000006a0: 7a0a 456e 632e 6465 726b 6579 a901 720c  z.Enc.derkey..r.
+000006b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000006c0: 0000 0000 0300 0000 4300 0000 730e 0000  ........C...s...
+000006d0: 0074 00a0 0164 01a1 01a0 02a1 0053 0029  .t...d.......S.)
+000006e0: 024e e940 0000 0029 0372 2600 0000 7227  .N.@...).r&...r'
+000006f0: 0000 00da 0368 6578 7214 0000 0072 1400  .....hexr....r..
+00000700: 0000 7214 0000 0072 1500 0000 da0a 6765  ..r....r......ge
+00000710: 6e4d 6169 6e6b 6579 2a00 0000 7302 0000  nMainkey*...s...
+00000720: 0000 027a 0e45 6e63 2e67 656e 4d61 696e  ...z.Enc.genMain
+00000730: 6b65 7963 0100 0000 0000 0000 0000 0000  keyc............
+00000740: 0100 0000 0300 0000 4300 0000 730c 0000  ........C...s...
+00000750: 0074 00a0 017c 006a 02a1 0153 00a9 014e  .t...|.j...S...N
+00000760: 2903 7204 0000 00da 0343 4243 7228 0000  ).r......CBCr(..
+00000770: 00a9 0172 1100 0000 7214 0000 0072 1400  ...r....r....r..
+00000780: 0000 7215 0000 00da 046d 6f64 652e 0000  ..r......mode...
+00000790: 0073 0200 0000 0001 7a08 456e 632e 6d6f  .s......z.Enc.mo
+000007a0: 6465 6301 0000 0000 0000 0000 0000 0001  dec.............
+000007b0: 0000 0005 0000 0043 0000 0073 1e00 0000  .......C...s....
+000007c0: 7400 7401 6a02 7c00 6a03 6401 8d01 7c00  t.t.j.|.j.d...|.
+000007d0: a004 a100 7405 8300 6402 8d03 5300 a903  ....t...d...S...
+000007e0: 4e29 01da 036b 6579 2902 723b 0000 005a  N)...key).r;...Z
+000007f0: 0762 6163 6b65 6e64 2906 7202 0000 0072  .backend).r....r
+00000800: 0300 0000 da03 4145 5372 2d00 0000 723b  ......AESr-...r;
+00000810: 0000 0072 0600 0000 723a 0000 0072 1400  ...r....r:...r..
+00000820: 0000 7214 0000 0072 1500 0000 da06 6369  ..r....r......ci
+00000830: 7068 6572 3100 0000 7302 0000 0000 017a  pher1...s......z
+00000840: 0a45 6e63 2e63 6970 6865 7263 0100 0000  .Enc.cipherc....
+00000850: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000860: 4300 0000 730c 0000 007c 00a0 00a1 00a0  C...s....|......
+00000870: 01a1 0053 0072 3800 0000 2902 723f 0000  ...S.r8...).r?..
+00000880: 005a 0965 6e63 7279 7074 6f72 723a 0000  .Z.encryptorr:..
+00000890: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+000008a0: da10 6369 7068 6572 5f65 6e63 7279 7074  ..cipher_encrypt
+000008b0: 6f72 3400 0000 7302 0000 0000 017a 1445  or4...s......z.E
+000008c0: 6e63 2e63 6970 6865 725f 656e 6372 7970  nc.cipher_encryp
+000008d0: 746f 7263 0100 0000 0000 0000 0000 0000  torc............
+000008e0: 0200 0000 0300 0000 4300 0000 7322 0000  ........C...s"..
+000008f0: 0074 00a0 0164 01a1 01a0 02a1 007d 017c  .t...d.......}.|
+00000900: 01a0 037c 006a 04a1 017c 01a0 05a1 0017  ...|.j...|......
+00000910: 0053 00a9 024e e980 0000 0029 0672 0500  .S...N.....).r..
+00000920: 0000 da05 504b 4353 37da 0670 6164 6465  ....PKCS7..padde
+00000930: 72da 0675 7064 6174 6572 1d00 0000 da08  r..updater......
+00000940: 6669 6e61 6c69 7a65 2902 7211 0000 0072  finalize).r....r
+00000950: 4400 0000 7214 0000 0072 1400 0000 7215  D...r....r....r.
+00000960: 0000 00da 0e70 6164 6465 645f 6d65 7373  .....padded_mess
+00000970: 6167 6537 0000 0073 0400 0000 0001 0e01  age7...s........
+00000980: 7a12 456e 632e 7061 6464 6564 5f6d 6573  z.Enc.padded_mes
+00000990: 7361 6765 6301 0000 0000 0000 0000 0000  sagec...........
+000009a0: 0001 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
+000009b0: 0000 7c00 a000 a100 a001 7c00 a002 a100  ..|.......|.....
+000009c0: a101 7c00 a000 a100 a003 a100 1700 5300  ..|...........S.
+000009d0: 7238 0000 0029 0472 4000 0000 7245 0000  r8...).r@...rE..
+000009e0: 0072 4700 0000 7246 0000 0072 3a00 0000  .rG...rF...r:...
+000009f0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000a00: 0a63 6970 6865 7274 6578 743b 0000 0073  .ciphertext;...s
+00000a10: 0200 0000 0001 7a0e 456e 632e 6369 7068  ......z.Enc.ciph
+00000a20: 6572 7465 7874 6301 0000 0000 0000 0000  ertextc.........
+00000a30: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00000a40: 2c00 0000 7c00 6a00 7d01 7401 a002 7c01  ,...|.j.}.t...|.
+00000a50: 7403 a004 a100 a102 7d01 7c01 a005 7c00  t.......}.|...|.
+00000a60: a006 a100 a101 0100 7c01 a007 a100 5300  ........|.....S.
+00000a70: 7238 0000 0029 0872 2e00 0000 7208 0000  r8...).r....r...
+00000a80: 00da 0448 4d41 4372 0700 0000 da06 5348  ...HMACr......SH
+00000a90: 4135 3132 7245 0000 0072 4800 0000 7246  A512rE...rH...rF
+00000aa0: 0000 00a9 0272 1100 0000 da01 6872 1400  .....r......hr..
+00000ab0: 0000 7214 0000 0072 1500 0000 7249 0000  ..r....r....rI..
+00000ac0: 003e 0000 0073 0800 0000 0001 0601 1001  .>...s..........
+00000ad0: 0e01 7a08 456e 632e 484d 4143 6301 0000  ..z.Enc.HMACc...
+00000ae0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000af0: 0043 0000 0073 1200 0000 7400 a001 6401  .C...s....t...d.
+00000b00: 7c00 6a02 a102 7d01 7c01 5300 2902 4efa  |.j...}.|.S.).N.
+00000b10: 0221 4929 03da 0673 7472 7563 74da 0470  .!I)...struct..p
+00000b20: 6163 6b72 2b00 0000 2902 7211 0000 005a  ackr+...).r....Z
+00000b30: 0b69 7465 7273 5f62 7974 6573 7214 0000  .iters_bytesr...
+00000b40: 0072 1400 0000 7215 0000 00da 0f73 6574  .r....r......set
+00000b50: 7570 4974 6572 6174 696f 6e73 4400 0000  upIterationsD...
+00000b60: 7304 0000 0000 010e 017a 1345 6e63 2e73  s........z.Enc.s
+00000b70: 6574 7570 4974 6572 6174 696f 6e73 6301  etupIterationsc.
+00000b80: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000b90: 0000 0043 0000 0073 2a00 0000 7c00 a000  ...C...s*...|...
+00000ba0: a100 7c00 6a01 1700 7c00 6a02 1700 7c00  ..|.j...|.j...|.
+00000bb0: 6a03 1700 7c00 a004 a100 1700 7c00 a005  j...|.......|...
+00000bc0: a100 1700 5300 7238 0000 0029 0672 4900  ....S.r8...).rI.
+00000bd0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+00000be0: 0072 5000 0000 7248 0000 0072 3a00 0000  .rP...rH...r:...
+00000bf0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000c00: 0a65 6e63 546f 4279 7465 7348 0000 0073  .encToBytesH...s
+00000c10: 0200 0000 0001 7a0e 456e 632e 656e 6354  ......z.Enc.encT
+00000c20: 6f42 7974 6573 6301 0000 0000 0000 0000  oBytesc.........
+00000c30: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000c40: 1400 0000 7400 a001 7c00 a002 a100 a101  ....t...|.......
+00000c50: a003 6401 a101 5300 a902 4e72 3000 0000  ..d...S...Nr0...
+00000c60: 2904 da06 6261 7365 3634 5a11 7572 6c73  )...base64Z.urls
+00000c70: 6166 655f 6236 3465 6e63 6f64 6572 5100  afe_b64encoderQ.
+00000c80: 0000 da06 6465 636f 6465 723a 0000 0072  ....decoder:...r
+00000c90: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+00000ca0: 656e 6354 6f53 7472 4b00 0000 7302 0000  encToStrK...s...
+00000cb0: 0000 017a 0c45 6e63 2e65 6e63 546f 5374  ...z.Enc.encToSt
+00000cc0: 7229 1472 1600 0000 7217 0000 0072 1800  r).r....r....r..
+00000cd0: 0000 7209 0000 0072 2300 0000 7225 0000  ..r....r#...r%..
+00000ce0: 0072 1000 0000 da0c 7374 6174 6963 6d65  .r......staticme
+00000cf0: 7468 6f64 da03 696e 7472 2c00 0000 7237  thod..intr,...r7
+00000d00: 0000 0072 3b00 0000 723f 0000 0072 4000  ...r;...r?...r@.
+00000d10: 0000 7247 0000 0072 4800 0000 7249 0000  ..rG...rH...rI..
+00000d20: 0072 5000 0000 7251 0000 0072 5500 0000  .rP...rQ...rU...
+00000d30: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000d40: 1500 0000 721b 0000 0011 0000 0073 1c00  ....r........s..
+00000d50: 0000 0801 1a10 0201 1607 0201 1003 0803  ................
+00000d60: 0803 0803 0e04 0e03 0e06 0e04 0e03 721b  ..............r.
+00000d70: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000d80: 0000 0000 0400 0000 0000 0000 7322 0000  ............s"..
+00000d90: 0065 005a 0164 005a 0264 0164 029c 0187  .e.Z.d.Z.d.d....
+00000da0: 0066 0164 0364 0484 0c5a 0387 0004 005a  .f.d.d...Z.....Z
+00000db0: 0453 0029 05da 154d 6573 7361 6765 5461  .S.)...MessageTa
+00000dc0: 6d70 6572 696e 6745 7272 6f72 4e72 3400  mperingErrorNr4.
+00000dd0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000de0: 0000 0003 0000 0003 0000 0073 1800 0000  ...........s....
+00000df0: 6401 7c00 5f00 7401 8300 a002 7c00 6a00  d.|._.t.....|.j.
+00000e00: a101 0100 6400 5300 2902 4e7a 4c48 4d41  ....d.S.).NzLHMA
+00000e10: 4320 6d69 736d 6174 6368 2021 204d 6573  C mismatch ! Mes
+00000e20: 7361 6765 2068 6173 2062 6565 6e20 5441  sage has been TA
+00000e30: 4d50 4552 4544 2077 6974 6820 2c0a 206f  MPERED with ,. o
+00000e40: 7220 506f 7373 6962 6c65 206b 6579 2064  r Possible key d
+00000e50: 6966 6665 7265 6e63 6572 0e00 0000 723a  ifferencer....r:
+00000e60: 0000 0072 1200 0000 7214 0000 0072 1500  ...r....r....r..
+00000e70: 0000 7210 0000 0050 0000 0073 0400 0000  ..r....P...s....
+00000e80: 0001 0601 7a1e 4d65 7373 6167 6554 616d  ....z.MessageTam
+00000e90: 7065 7269 6e67 4572 726f 722e 5f5f 696e  peringError.__in
+00000ea0: 6974 5f5f 2905 7216 0000 0072 1700 0000  it__).r....r....
+00000eb0: 7218 0000 0072 1000 0000 721a 0000 0072  r....r....r....r
+00000ec0: 1400 0000 7214 0000 0072 1200 0000 7215  ....r....r....r.
+00000ed0: 0000 0072 5800 0000 4f00 0000 7302 0000  ...rX...O...s...
+00000ee0: 0008 0172 5800 0000 6300 0000 0000 0000  ...rX...c.......
+00000ef0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000f00: 0073 9200 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00000f10: 6504 6505 6602 1900 6504 6401 6402 9c03  e.e.f...e.d.d...
+00000f20: 6403 6404 8404 5a06 6505 6405 9c01 6406  d.d...Z.e.d...d.
+00000f30: 6407 8404 5a07 6508 6405 9c01 6408 6409  d...Z.e.d...d.d.
+00000f40: 8404 5a09 640a 640b 8400 5a0a 640c 640d  ..Z.d.d...Z.d.d.
+00000f50: 8400 5a0b 640e 640f 8400 5a0c 6505 6405  ..Z.d.d...Z.e.d.
+00000f60: 9c01 6410 6411 8404 5a0d 6505 6405 9c01  ..d.d...Z.e.d...
+00000f70: 6412 6413 8404 5a0e 6505 6405 9c01 6414  d.d...Z.e.d...d.
+00000f80: 6415 8404 5a0f 6504 6405 9c01 6416 6417  d...Z.e.d...d.d.
+00000f90: 8404 5a10 6401 5300 2918 da03 4465 634e  ..Z.d.S.)...DecN
+00000fa0: 721c 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00000fb0: 0000 0400 0000 0600 0000 4300 0000 7306  ..........C...s.
+00000fc0: 0100 0074 007c 0174 0183 0272 227c 01a0  ...t.|.t...r"|..
+00000fd0: 0264 01a1 017d 0374 03a0 047c 03a1 017c  .d...}.t...|...|
+00000fe0: 005f 056e 1074 007c 0174 0683 0272 327c  ._.n.t.|.t...r2|
+00000ff0: 017c 005f 057c 027c 005f 077c 006a 0564  .|._.|.|._.|.j.d
+00001000: 0064 0285 0219 007c 005f 087c 006a 0564  .d.....|._.|.j.d
+00001010: 0264 0385 0219 007c 005f 097c 006a 0564  .d.....|._.|.j.d
+00001020: 0364 0485 0219 007c 005f 0a7c 006a 0564  .d.....|._.|.j.d
+00001030: 0464 0585 0219 007c 005f 0b74 0ca0 0d64  .d.....|._.t...d
+00001040: 067c 006a 0564 0564 0785 0219 00a1 0264  .|.j.d.d.......d
+00001050: 0819 007c 005f 0e7c 006a 0e64 096b 0073  ...|._.|.j.d.k.s
+00001060: a87c 006a 0e64 0a6b 0472 b274 0f7c 006a  .|.j.d.k.r.t.|.j
+00001070: 0e83 0182 017c 006a 0564 0764 0085 0219  .....|.j.d.d....
+00001080: 007c 005f 1074 11a0 127c 006a 077c 006a  .|._.t...|.j.|.j
+00001090: 0a7c 006a 0ea1 037c 005f 1374 11a0 127c  .|.j...|._.t...|
+000010a0: 006a 077c 006a 0b7c 006a 0ea1 037c 005f  .j.|.j.|.j...|._
+000010b0: 147c 00a0 15a1 0064 0b75 0090 0172 0274  .|.....d.u...r.t
+000010c0: 1683 0082 0164 0053 0029 0c4e 7230 0000  .....d.S.).Nr0..
+000010d0: 0072 3500 0000 e950 0000 00e9 6000 0000  .r5....P....`...
+000010e0: e970 0000 0072 4d00 0000 e974 0000 0072  .p...rM....t...r
+000010f0: 0100 0000 7220 0000 0072 2100 0000 4629  ....r ...r!...F)
+00001100: 1772 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+00001110: 7253 0000 005a 1175 726c 7361 6665 5f62  rS...Z.urlsafe_b
+00001120: 3634 6465 636f 6465 721d 0000 0072 2500  64decoder....r%.
+00001130: 0000 723d 0000 00da 0872 6563 5f68 6d61  ..r=.....rec_hma
+00001140: 63da 0672 6563 5f69 76da 0872 6563 5f73  c..rec_iv..rec_s
+00001150: 616c 74da 0a72 6563 5f70 6570 7065 7272  alt..rec_pepperr
+00001160: 4e00 0000 da06 756e 7061 636b da0e 7265  N.....unpack..re
+00001170: 635f 6974 6572 6174 696f 6e73 720a 0000  c_iterationsr...
+00001180: 00da 0e72 6563 5f63 6970 6865 7274 6578  ...rec_ciphertex
+00001190: 7472 1b00 0000 722c 0000 00da 0664 6563  tr....r,.....dec
+000011a0: 4b65 79da 0668 6d61 635f 6bda 0a76 6572  Key..hmac_k..ver
+000011b0: 6966 7948 4d41 4372 5800 0000 2904 7211  ifyHMACrX...).r.
+000011c0: 0000 0072 1d00 0000 721e 0000 00da 016d  ...r....r......m
+000011d0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000011e0: 1000 0000 5500 0000 7324 0000 0000 010a  ....U...s$......
+000011f0: 010a 010e 010a 0106 0106 0110 0110 0110  ................
+00001200: 0110 011c 0114 010a 0110 0116 0116 010e  ................
+00001210: 017a 0c44 6563 2e5f 5f69 6e69 745f 5f72  .z.Dec.__init__r
+00001220: 3400 0000 6301 0000 0000 0000 0000 0000  4...c...........
+00001230: 0002 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
+00001240: 0000 7c00 6a00 7d01 7401 a002 7c01 7403  ..|.j.}.t...|.t.
+00001250: a004 a100 a102 7d01 7c01 a005 7c00 6a06  ......}.|...|.j.
+00001260: a101 0100 7c01 a007 a100 5300 7238 0000  ....|.....S.r8..
+00001270: 0029 0872 6600 0000 7208 0000 0072 4900  .).rf...r....rI.
+00001280: 0000 7207 0000 0072 4a00 0000 7245 0000  ..r....rJ...rE..
+00001290: 0072 6400 0000 7246 0000 0072 4b00 0000  .rd...rF...rK...
+000012a0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+000012b0: 0a61 6374 7561 6c48 4d41 4368 0000 0073  .actualHMACh...s
+000012c0: 0800 0000 0001 0601 1001 0c01 7a0e 4465  ............z.De
+000012d0: 632e 6163 7475 616c 484d 4143 6301 0000  c.actualHMACc...
+000012e0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+000012f0: 0043 0000 0073 1200 0000 7400 a001 7c00  .C...s....t...|.
+00001300: a002 a100 7c00 6a03 a102 5300 7238 0000  ....|.j...S.r8..
+00001310: 0029 04da 0368 6d63 5a0e 636f 6d70 6172  .)...hmcZ.compar
+00001320: 655f 6469 6765 7374 7269 0000 0072 5e00  e_digestri...r^.
+00001330: 0000 723a 0000 0072 1400 0000 7214 0000  ..r:...r....r...
+00001340: 0072 1500 0000 7267 0000 006e 0000 0073  .r....rg...n...s
+00001350: 0200 0000 0001 7a0e 4465 632e 7665 7269  ......z.Dec.veri
+00001360: 6679 484d 4143 6301 0000 0000 0000 0000  fyHMACc.........
+00001370: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00001380: 0c00 0000 7400 a001 7c00 6a02 a101 5300  ....t...|.j...S.
+00001390: 7238 0000 0029 0372 0400 0000 7239 0000  r8...).r....r9..
+000013a0: 0072 5f00 0000 723a 0000 0072 1400 0000  .r_...r:...r....
+000013b0: 7214 0000 0072 1500 0000 723b 0000 0071  r....r....r;...q
+000013c0: 0000 0073 0200 0000 0001 7a08 4465 632e  ...s......z.Dec.
+000013d0: 6d6f 6465 6301 0000 0000 0000 0000 0000  modec...........
+000013e0: 0001 0000 0005 0000 0043 0000 0073 1e00  .........C...s..
+000013f0: 0000 7400 7401 6a02 7c00 6a03 6401 8d01  ..t.t.j.|.j.d...
+00001400: 7c00 a004 a100 7405 8300 6402 8d03 5300  |.....t...d...S.
+00001410: 723c 0000 0029 0672 0200 0000 7203 0000  r<...).r....r...
+00001420: 0072 3e00 0000 7265 0000 0072 3b00 0000  .r>...re...r;...
+00001430: 7206 0000 0072 3a00 0000 7214 0000 0072  r....r:...r....r
+00001440: 1400 0000 7215 0000 0072 3f00 0000 7400  ....r....r?...t.
+00001450: 0000 7302 0000 0000 017a 0a44 6563 2e63  ..s......z.Dec.c
+00001460: 6970 6865 7263 0100 0000 0000 0000 0000  ipherc..........
+00001470: 0000 0100 0000 0200 0000 4300 0000 730c  ..........C...s.
+00001480: 0000 007c 00a0 00a1 00a0 01a1 0053 0072  ...|.........S.r
+00001490: 3800 0000 2902 723f 0000 005a 0964 6563  8...).r?...Z.dec
+000014a0: 7279 7074 6f72 723a 0000 0072 1400 0000  ryptorr:...r....
+000014b0: 7214 0000 0072 1500 0000 da10 6369 7068  r....r......ciph
+000014c0: 6572 5f64 6563 7279 7074 6f72 7700 0000  er_decryptorw...
+000014d0: 7302 0000 0000 017a 1444 6563 2e63 6970  s......z.Dec.cip
+000014e0: 6865 725f 6465 6372 7970 746f 7263 0100  her_decryptorc..
+000014f0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00001500: 0000 4300 0000 731c 0000 007c 00a0 00a1  ..C...s....|....
+00001510: 00a0 017c 006a 02a1 017c 00a0 00a1 00a0  ...|.j...|......
+00001520: 03a1 0017 0053 0072 3800 0000 2904 726b  .....S.r8...).rk
+00001530: 0000 0072 4500 0000 7264 0000 0072 4600  ...rE...rd...rF.
+00001540: 0000 723a 0000 0072 1400 0000 7214 0000  ..r:...r....r...
+00001550: 0072 1500 0000 da11 7072 655f 756e 7061  .r......pre_unpa
+00001560: 6464 696e 675f 6465 637a 0000 0073 0200  dding_decz...s..
+00001570: 0000 0001 7a15 4465 632e 7072 655f 756e  ....z.Dec.pre_un
+00001580: 7061 6464 696e 675f 6465 6363 0100 0000  padding_decc....
+00001590: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000015a0: 4300 0000 7324 0000 0074 00a0 0164 01a1  C...s$...t...d..
+000015b0: 01a0 02a1 007d 017c 01a0 037c 00a0 04a1  .....}.|...|....
+000015c0: 00a1 017c 01a0 05a1 0017 0053 0072 4100  ...|.......S.rA.
+000015d0: 0000 2906 7205 0000 0072 4300 0000 da08  ..).r....rC.....
+000015e0: 756e 7061 6464 6572 7245 0000 0072 6c00  unpadderrE...rl.
+000015f0: 0000 7246 0000 0029 0272 1100 0000 726d  ..rF...).r....rm
+00001600: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00001610: 0000 da0a 756e 7061 6464 6564 5f6d 7d00  ....unpadded_m}.
+00001620: 0000 7304 0000 0000 010e 017a 0e44 6563  ..s........z.Dec
+00001630: 2e75 6e70 6164 6465 645f 6d63 0100 0000  .unpadded_mc....
+00001640: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001650: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
+00001660: 0072 3800 0000 2901 726e 0000 0072 3a00  .r8...).rn...r:.
+00001670: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00001680: 00da 0a64 6563 546f 4279 7465 7381 0000  ...decToBytes...
+00001690: 0073 0200 0000 0001 7a0e 4465 632e 6465  .s......z.Dec.de
+000016a0: 6354 6f42 7974 6573 6301 0000 0000 0000  cToBytesc.......
+000016b0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000016c0: 0073 0e00 0000 7c00 a000 a100 a001 6401  .s....|.......d.
+000016d0: a101 5300 7252 0000 0029 0272 6e00 0000  ..S.rR...).rn...
+000016e0: 7254 0000 0072 3a00 0000 7214 0000 0072  rT...r:...r....r
+000016f0: 1400 0000 7215 0000 00da 0864 6563 546f  ....r......decTo
+00001700: 5374 7284 0000 0073 0200 0000 0001 7a0c  Str....s......z.
+00001710: 4465 632e 6465 6354 6f53 7472 2911 7216  Dec.decToStr).r.
+00001720: 0000 0072 1700 0000 7218 0000 0072 0900  ...r....r....r..
+00001730: 0000 7223 0000 0072 2500 0000 7210 0000  ..r#...r%...r...
+00001740: 0072 6900 0000 da04 626f 6f6c 7267 0000  .ri.....boolrg..
+00001750: 0072 3b00 0000 723f 0000 0072 6b00 0000  .r;...r?...rk...
+00001760: 726c 0000 0072 6e00 0000 726f 0000 0072  rl...rn...ro...r
+00001770: 7000 0000 7214 0000 0072 1400 0000 7214  p...r....r....r.
+00001780: 0000 0072 1500 0000 7259 0000 0054 0000  ...r....rY...T..
+00001790: 0073 1400 0000 0801 1a13 0e06 0e03 0803  .s..............
+000017a0: 0803 0803 0e03 0e04 0e03 7259 0000 0029  ..........rY...)
+000017b0: 165a 2663 7279 7074 6f67 7261 7068 792e  .Z&cryptography.
+000017c0: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
+000017d0: 732e 6369 7068 6572 7372 0200 0000 7203  s.ciphersr....r.
+000017e0: 0000 0072 0400 0000 5a1e 6372 7970 746f  ...r....Z.crypto
+000017f0: 6772 6170 6879 2e68 617a 6d61 742e 7072  graphy.hazmat.pr
+00001800: 696d 6974 6976 6573 7205 0000 005a 1c63  imitivesr....Z.c
+00001810: 7279 7074 6f67 7261 7068 792e 6861 7a6d  ryptography.hazm
+00001820: 6174 2e62 6163 6b65 6e64 7372 0600 0000  at.backendsr....
+00001830: 7207 0000 0072 0800 0000 da06 7479 7069  r....r......typi
+00001840: 6e67 7209 0000 0072 6a00 0000 7233 0000  ngr....rj...r3..
+00001850: 0072 5300 0000 724e 0000 0072 2600 0000  .rS...rN...r&...
+00001860: da09 4578 6365 7074 696f 6e72 0a00 0000  ..Exceptionr....
+00001870: 721b 0000 0072 5800 0000 7259 0000 0072  r....rX...rY...r
+00001880: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+00001890: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000018a0: 0073 1a00 0000 1401 0c01 0c01 1001 0c01  .s..............
+000018b0: 0801 0801 0801 0801 0802 1005 0e3e 1005  .............>..
```

### Comparing `AshCrypt-1.2.3/AshCrypt/__pycache__/AshDatabase.cpython-39.pyc` & `AshCrypt-1.2.4/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jun 30 15:01:03 2023 UTC, .py size: 8854 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,478 +1,456 @@
-00000000: 610d 0d0a 0000 0000 2fee 9e64 9622 0000  a......./..d."..
+00000000: 610d 0d0a 0000 0000 2238 a364 0221 0000  a......."8.d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 5a06 6400  m.Z...d.d.l.Z.d.
 00000060: 6404 6c07 5a07 6501 4700 6405 6406 8400  d.l.Z.e.G.d.d...
-00000070: 6406 8302 8301 5a08 6509 6407 6b02 72a6  d.....Z.e.d.k.r.
-00000080: 6508 6408 8301 5a0a 650a a00b a100 0100  e.d...Z.e.......
-00000090: 6409 5a0c 650a a00d 640a 640b 650c a103  d.Z.e...d.d.e...
-000000a0: 0100 650a a00e a100 4400 5d0c 5a0f 6510  ..e.....D.].Z.e.
-000000b0: 650f 8301 0100 717c 6510 650a 6a11 8301  e.....q|e.e.j...
-000000c0: 0100 640c 5a12 6510 650a a013 6512 a101  ..d.Z.e.e...e...
-000000d0: 8301 0100 6404 5300 290d e900 0000 0029  ....d.S.)......)
-000000e0: 02da 0964 6174 6163 6c61 7373 da05 6669  ...dataclass..fi
-000000f0: 656c 6429 01da 0864 6174 6574 696d 6529  eld)...datetime)
-00000100: 01da 0555 6e69 6f6e 4e63 0000 0000 0000  ...UnionNc......
-00000110: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
-00000120: 0000 7316 0100 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-00000130: 0065 0383 005a 0465 0565 0664 013c 0065  .e...Z.e.e.d.<.e
-00000140: 0364 0264 038d 015a 0765 0565 0664 043c  .d.d...Z.e.e.d.<
-00000150: 0065 0364 0564 0564 068d 025a 0865 096a  .e.d.d.d...Z.e.j
-00000160: 0a65 0664 073c 0065 0364 0564 0564 068d  .e.d.<.e.d.d.d..
-00000170: 025a 0b65 096a 0c65 0664 083c 0064 0964  .Z.e.j.e.d.<.d.d
-00000180: 0a84 005a 0d65 0e64 0b64 0c84 0083 015a  ...Z.e.d.d.....Z
-00000190: 0f65 0e65 1065 1165 1266 0219 0064 0d9c  .e.e.e.e.f...d..
-000001a0: 0164 0e64 0f84 0483 015a 1365 0e64 1064  .d.d.....Z.e.d.d
-000001b0: 1184 0083 015a 1465 0565 1564 129c 0264  .....Z.e.e.d...d
-000001c0: 1364 1484 045a 1664 2c64 1664 1784 015a  .d...Z.d,d.d...Z
-000001d0: 1764 2d64 1864 1984 015a 1864 2e65 0565  .d-d.d...Z.d.e.e
-000001e0: 0565 1964 1a9c 0364 1b64 1c84 055a 1a64  .e.d...d.d...Z.d
-000001f0: 2f64 1d64 1e84 015a 1b64 3065 1964 1f9c  /d.d...Z.d0e.d..
-00000200: 0164 2064 2184 055a 1c64 2264 2384 005a  .d d!..Z.d"d#..Z
-00000210: 1d65 1264 0d9c 0164 2464 2584 045a 1e64  .e.d...d$d%..Z.d
-00000220: 2664 2784 005a 1f64 2864 2984 005a 2064  &d'..Z.d(d)..Z d
-00000230: 3164 2a64 2b84 015a 2164 1553 0029 32da  1d*d+..Z!d.S.)2.
-00000240: 0844 6174 6162 6173 65da 0664 626e 616d  .Database..dbnam
-00000250: 655a 0a43 6c61 7373 6966 6965 6429 01da  eZ.Classified)..
-00000260: 0764 6566 6175 6c74 da09 7461 626c 656e  .default..tablen
-00000270: 616d 6546 2902 da04 696e 6974 da04 7265  ameF)...init..re
-00000280: 7072 da04 636f 6e6e da01 6363 0100 0000  pr..conn..cc....
-00000290: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000002a0: 4300 0000 731e 0000 0074 00a0 017c 006a  C...s....t...|.j
-000002b0: 02a1 017c 005f 037c 006a 03a0 04a1 007c  ...|._.|.j.....|
-000002c0: 005f 0564 0053 0029 014e 2906 da07 7371  ._.d.S.).N)...sq
-000002d0: 6c69 7465 33da 0763 6f6e 6e65 6374 7207  lite3..connectr.
-000002e0: 0000 0072 0c00 0000 5a06 6375 7273 6f72  ...r....Z.cursor
-000002f0: 720d 0000 00a9 01da 0473 656c 66a9 0072  r........self..r
-00000300: 1200 0000 fa32 433a 5c57 6f72 6b5c 4769  .....2C:\Work\Gi
-00000310: 7448 7562 576f 726b 5c41 4553 2d32 3536  tHubWork\AES-256
-00000320: 5c41 7368 4372 7970 745c 4173 6844 6174  \AshCrypt\AshDat
-00000330: 6162 6173 652e 7079 da0d 5f5f 706f 7374  abase.py..__post
-00000340: 5f69 6e69 745f 5f0e 0000 0073 0400 0000  _init__....s....
-00000350: 0001 0e01 7a16 4461 7461 6261 7365 2e5f  ....z.Database._
-00000360: 5f70 6f73 745f 696e 6974 5f5f 6301 0000  _post_init__c...
-00000370: 0000 0000 0000 0000 0004 0000 000a 0000  ................
-00000380: 0043 0000 0073 8a00 0000 7a56 7c00 6a00  .C...s....zV|.j.
-00000390: 8f3c 0100 7c00 6a01 a002 6401 a101 0100  .<..|.j...d.....
-000003a0: 7c00 6a01 a003 a100 7d01 7c01 6402 1900  |.j.....}.|.d...
-000003b0: 6403 1b00 6403 1b00 7d02 7c02 5700 0200  d...d...}.|.W...
-000003c0: 6400 0400 0400 8303 0100 5700 5300 3100  d.........W.S.1.
-000003d0: 734a 3000 0100 0100 0100 5900 0100 5700  sJ0.......Y...W.
-000003e0: 6e2e 0400 7404 6a05 7984 0100 7d03 0100  n...t.j.y...}...
-000003f0: 7a14 6402 7c03 6602 5700 0600 5900 6400  z.d.|.f.W...Y.d.
-00000400: 7d03 7e03 5300 6400 7d03 7e03 3000 3000  }.~.S.d.}.~.0.0.
-00000410: 6400 5300 2904 4e7a 4953 454c 4543 5420  d.S.).NzISELECT 
-00000420: 7061 6765 5f63 6f75 6e74 202a 2070 6167  page_count * pag
-00000430: 655f 7369 7a65 2046 524f 4d20 7072 6167  e_size FROM prag
-00000440: 6d61 5f70 6167 655f 636f 756e 7428 2920  ma_page_count() 
-00000450: 2c20 7072 6167 6d61 5f70 6167 655f 7369  , pragma_page_si
-00000460: 7a65 7201 0000 0069 0004 0000 2906 720c  zer....i....).r.
-00000470: 0000 0072 0d00 0000 da07 6578 6563 7574  ...r......execut
-00000480: 65da 0866 6574 6368 6f6e 6572 0e00 0000  e..fetchoner....
-00000490: da05 4572 726f 7229 0472 1100 0000 5a09  ..Error).r....Z.
-000004a0: 7369 7a65 5f69 6e66 6fda 0473 697a 65da  size_info..size.
-000004b0: 0165 7212 0000 0072 1200 0000 7213 0000  .er....r....r...
-000004c0: 0072 1800 0000 1200 0000 7310 0000 0000  .r........s.....
-000004d0: 0202 0108 010c 010a 0110 0128 0110 017a  ...........(...z
-000004e0: 0d44 6174 6162 6173 652e 7369 7a65 2901  .Database.size).
-000004f0: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00000500: 0000 0000 0003 0000 000a 0000 0043 0000  .............C..
-00000510: 0073 4c00 0000 7a1a 7400 a001 7402 a003  .sL...z.t...t...
-00000520: 7c00 6a04 a101 6a05 a101 7d01 7c01 5700  |.j...j...}.|.W.
-00000530: 5300 0400 7406 7946 0100 7d02 0100 7a14  S...t.yF..}...z.
-00000540: 6401 7c02 6602 5700 0600 5900 6400 7d02  d.|.f.W...Y.d.}.
-00000550: 7e02 5300 6400 7d02 7e02 3000 3000 6400  ~.S.d.}.~.0.0.d.
-00000560: 5300 2902 4e72 0100 0000 2907 7204 0000  S.).Nr....).r...
-00000570: 00da 0d66 726f 6d74 696d 6573 7461 6d70  ...fromtimestamp
-00000580: da02 6f73 da04 7374 6174 7207 0000 00da  ..os..statr.....
-00000590: 0873 745f 6d74 696d 65da 074f 5345 7272  .st_mtime..OSErr
-000005a0: 6f72 2903 7211 0000 005a 0974 696d 655f  or).r....Z.time_
-000005b0: 7374 6174 7219 0000 0072 1200 0000 7212  statr....r....r.
-000005c0: 0000 0072 1300 0000 da08 6c61 7374 5f6d  ...r......last_m
-000005d0: 6f64 1d00 0000 730a 0000 0000 0202 0114  od....s.........
-000005e0: 0106 020e 017a 1144 6174 6162 6173 652e  .....z.Database.
-000005f0: 6c61 7374 5f6d 6f64 6301 0000 0000 0000  last_modc.......
-00000600: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000610: 0073 0e00 0000 6401 7c00 6a00 9b00 6402  .s....d.|.j...d.
-00000620: 9d03 5300 2903 4e7a 2044 4546 4155 4c54  ..S.).Nz DEFAULT
-00000630: 2052 4f55 5449 4e47 2041 4c4c 204d 4554   ROUTING ALL MET
-00000640: 484f 4453 2054 4f20 22fa 0122 2901 7209  HODS TO "..").r.
-00000650: 0000 0072 1000 0000 7212 0000 0072 1200  ...r....r....r..
-00000660: 0000 7213 0000 00da 0f64 6566 6175 6c74  ..r......default
-00000670: 5f72 6f75 7469 6e67 2600 0000 7302 0000  _routing&...s...
-00000680: 0000 027a 1844 6174 6162 6173 652e 6465  ...z.Database.de
-00000690: 6661 756c 745f 726f 7574 696e 6729 02da  fault_routing)..
-000006a0: 0671 7565 7279 7372 1a00 0000 6301 0000  .querysr....c...
-000006b0: 0000 0000 0000 0000 0006 0000 000b 0000  ................
-000006c0: 0047 0000 0073 0001 0000 6700 7d02 7400  .G...s....g.}.t.
-000006d0: 7c01 8301 4400 5dee 5c02 7d03 7d04 7401  |...D.].\.}.}.t.
-000006e0: 7c04 7402 8302 7336 7c02 a003 6401 7c03  |.t...s6|...d.|.
-000006f0: 9b00 9d02 6402 7404 6602 6901 a101 0100  ....d.t.f.i.....
-00000700: 7a80 7c00 6a05 8f66 0100 7c00 6a06 a007  z.|.j..f..|.j...
-00000710: 7c04 a101 0100 7c00 6a06 6a08 6403 6b02  |.....|.j.j.d.k.
-00000720: 7278 7c02 a003 6401 7c03 9b00 9d02 6404  rx|...d.|.....d.
-00000730: 7c00 6a06 a009 a100 6702 6901 a101 0100  |.j.....g.i.....
-00000740: 6e1e 7c02 a003 6401 7c03 9b00 9d02 6404  n.|...d.|.....d.
-00000750: 7c00 6a06 a00a a100 6702 6901 a101 0100  |.j.....g.i.....
-00000760: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
-00000770: 73aa 3000 0100 0100 0100 5900 0100 5700  s.0.......Y...W.
-00000780: 710c 0400 740b 6a0c 79f8 0100 7d05 0100  q...t.j.y...}...
-00000790: 7a28 7c02 a003 6401 7c03 9b00 9d02 6405  z(|...d.|.....d.
-000007a0: 7c05 a00d a100 6602 6901 a101 0100 5700  |.....f.i.....W.
-000007b0: 5900 6400 7d05 7e05 710c 6400 7d05 7e05  Y.d.}.~.q.d.}.~.
-000007c0: 3000 3000 710c 7c02 5300 2906 4e7a 0671  0.0.q.|.S.).Nz.q
-000007d0: 7565 7279 20e7 0000 0000 0000 0000 e901  uery ...........
-000007e0: 0000 00da 0753 5543 4345 5353 da07 4641  .....SUCCESS..FA
-000007f0: 494c 5552 4529 0eda 0965 6e75 6d65 7261  ILURE)...enumera
-00000800: 7465 da0a 6973 696e 7374 616e 6365 da03  te..isinstance..
-00000810: 7374 72da 0661 7070 656e 64da 0954 7970  str..append..Typ
-00000820: 6545 7272 6f72 720c 0000 0072 0d00 0000  eErrorr....r....
-00000830: 7215 0000 005a 0872 6f77 636f 756e 7472  r....Z.rowcountr
-00000840: 1600 0000 da08 6665 7463 6861 6c6c 720e  ......fetchallr.
-00000850: 0000 0072 1700 0000 da07 5f5f 7374 725f  ...r......__str_
-00000860: 5f29 0672 1100 0000 7223 0000 00da 0672  _).r....r#.....r
-00000870: 6573 756c 74da 0169 da05 7175 6572 7972  esult..i..queryr
-00000880: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000890: 0000 0072 3100 0000 2a00 0000 731a 0000  ...r1...*...s...
-000008a0: 0000 0104 0110 010a 0118 0102 0108 010c  ................
-000008b0: 010c 0120 0240 0210 0134 017a 0e44 6174  ... .@...4.z.Dat
-000008c0: 6162 6173 652e 7175 6572 794e 6302 0000  abase.queryNc...
-000008d0: 0000 0000 0000 0000 0003 0000 000a 0000  ................
-000008e0: 0043 0000 0073 f800 0000 7c01 6400 7500  .C...s....|.d.u.
-000008f0: 727c 7a42 7c00 6a00 8f26 0100 7c00 6a01  r|zB|.j..&..|.j.
-00000900: a002 6401 7c00 6a03 9b00 6402 9d03 a101  ..d.|.j...d.....
-00000910: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
-00000920: 3100 733c 3000 0100 0100 0100 5900 0100  1.s<0.......Y...
-00000930: 5700 6403 5300 0400 7404 6a05 7978 0100  W.d.S...t.j.yx..
-00000940: 7d02 0100 7a14 6404 7c02 6602 5700 0600  }...z.d.|.f.W...
-00000950: 5900 6400 7d02 7e02 5300 6400 7d02 7e02  Y.d.}.~.S.d.}.~.
-00000960: 3000 3000 6e78 7a46 7c00 6a00 8f2a 0100  0.0.nxzF|.j..*..
-00000970: 7c00 6a01 a002 6401 7c01 9b00 6405 9d03  |.j...d.|...d...
-00000980: a101 0100 7c01 7c00 5f03 5700 6400 0400  ....|.|._.W.d...
-00000990: 0400 8303 0100 6e10 3100 73b4 3000 0100  ......n.1.s.0...
-000009a0: 0100 0100 5900 0100 5700 6406 5300 0400  ....Y...W.d.S...
-000009b0: 7404 6a05 9000 79f2 0100 7d02 0100 7a14  t.j...y...}...z.
-000009c0: 6407 7c02 6602 5700 0600 5900 6400 7d02  d.|.f.W...Y.d.}.
-000009d0: 7e02 5300 6400 7d02 7e02 3000 3000 6400  ~.S.d.}.~.0.0.d.
-000009e0: 5300 2908 4e7a 1b43 5245 4154 4520 5441  S.).Nz.CREATE TA
-000009f0: 424c 4520 4946 204e 4f54 2045 5849 5354  BLE IF NOT EXIST
-00000a00: 5320 7a3e 2028 4944 2049 4e54 4547 4552  S z> (ID INTEGER
-00000a10: 2050 5249 4d41 5259 204b 4559 2c20 4e61   PRIMARY KEY, Na
-00000a20: 6d65 2054 6578 7420 2c20 436f 6e74 656e  me Text , Conten
-00000a30: 7420 424c 4f42 202c 4b65 7920 5445 5854  t BLOB ,Key TEXT
-00000a40: 2029 e90b 0000 0072 2400 0000 7a3c 2028   ).....r$...z< (
-00000a50: 4944 2049 4e54 4547 4552 2050 5249 4d41  ID INTEGER PRIMA
-00000a60: 5259 204b 4559 2c4e 616d 6520 5445 5854  RY KEY,Name TEXT
-00000a70: 202c 436f 6e74 656e 7420 424c 4f42 202c   ,Content BLOB ,
-00000a80: 4b65 7920 5445 5854 2029 7225 0000 0072  Key TEXT )r%...r
-00000a90: 0100 0000 a906 720c 0000 0072 0d00 0000  ......r....r....
-00000aa0: 7215 0000 0072 0900 0000 720e 0000 0072  r....r....r....r
-00000ab0: 1700 0000 2903 7211 0000 00da 126f 7074  ....).r......opt
-00000ac0: 696f 6e61 6c5f 7461 626c 656e 616d 6572  ional_tablenamer
-00000ad0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000ae0: 0000 00da 0861 6464 7461 626c 653b 0000  .....addtable;..
-00000af0: 0073 1c00 0000 0001 0801 0201 0801 3402  .s............4.
-00000b00: 0601 1001 2003 0201 0801 1405 2401 0602  .... .......$...
-00000b10: 1201 7a11 4461 7461 6261 7365 2e61 6464  ..z.Database.add
-00000b20: 7461 626c 6563 0500 0000 0000 0000 0000  tablec..........
-00000b30: 0000 0600 0000 0a00 0000 4300 0000 7302  ..........C...s.
-00000b40: 0100 007c 0464 0075 0072 847a 4a7c 006a  ...|.d.u.r.zJ|.j
-00000b50: 008f 2e01 007c 006a 01a0 0264 017c 006a  .....|.j...d.|.j
-00000b60: 039b 0064 029d 037c 017c 027c 0366 03a1  ...d...|.|.|.f..
-00000b70: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000b80: 1031 0073 4430 0001 0001 0001 0059 0001  .1.sD0.......Y..
-00000b90: 0057 0064 0353 0004 0074 046a 0579 8001  .W.d.S...t.j.y..
-00000ba0: 007d 0501 007a 1464 047c 0566 0257 0006  .}...z.d.|.f.W..
-00000bb0: 0059 0064 007d 057e 0553 0064 007d 057e  .Y.d.}.~.S.d.}.~
-00000bc0: 0530 0030 006e 7a7a 487c 006a 008f 2c01  .0.0.nzzH|.j..,.
-00000bd0: 007c 006a 01a0 0264 017c 049b 0064 059d  .|.j...d.|...d..
-00000be0: 037c 017c 027c 0366 03a1 0201 0057 0064  .|.|.|.f.....W.d
-00000bf0: 0004 0004 0083 0301 006e 1031 0073 be30  .........n.1.s.0
-00000c00: 0001 0001 0001 0059 0001 0057 0064 0653  .......Y...W.d.S
-00000c10: 0004 0074 046a 0590 0079 fc01 007d 0501  ...t.j...y...}..
-00000c20: 007a 1464 077c 0566 0257 0006 0059 0064  .z.d.|.f.W...Y.d
-00000c30: 007d 057e 0553 0064 007d 057e 0530 0030  .}.~.S.d.}.~.0.0
-00000c40: 0064 0053 0029 084e 7a0c 494e 5345 5254  .d.S.).Nz.INSERT
-00000c50: 2049 4e54 4f20 7a2a 2028 4e61 6d65 202c   INTO z* (Name ,
-00000c60: 2043 6f6e 7465 6e74 202c 4b65 7929 2056   Content ,Key) V
-00000c70: 414c 5545 5320 283f 202c 203f 202c 203f  ALUES (? , ? , ?
-00000c80: 2920 7232 0000 0072 2400 0000 7a29 2028  ) r2...r$...z) (
-00000c90: 4e61 6d65 2c20 436f 6e74 656e 7420 2c4b  Name, Content ,K
-00000ca0: 6579 2920 5641 4c55 4553 2028 3f20 2c20  ey) VALUES (? , 
-00000cb0: 3f20 2c20 3f29 2072 2500 0000 7201 0000  ? , ?) r%...r...
-00000cc0: 0072 3300 0000 2906 7211 0000 00da 046e  .r3...).r......n
-00000cd0: 616d 65da 0763 6f6e 7465 6e74 da03 6b65  ame..content..ke
-00000ce0: 79da 136f 7074 696f 6e61 6c5f 7461 626c  y..optional_tabl
-00000cf0: 655f 6e61 6d65 7219 0000 0072 1200 0000  e_namer....r....
-00000d00: 7212 0000 0072 1300 0000 da06 696e 7365  r....r......inse
-00000d10: 7274 5300 0000 7322 0000 0000 0108 0102  rtS...s"........
-00000d20: 0108 0112 0108 ff22 0306 0110 0120 0302  ......."..... ..
-00000d30: 0108 0110 0108 ff22 0206 0112 017a 0f44  .......".....z.D
-00000d40: 6174 6162 6173 652e 696e 7365 7274 2903  atabase.insert).
-00000d50: da0b 636f 6c75 6d6e 5f6e 616d 65da 0e6e  ..column_name..n
-00000d60: 6577 5f63 6f6c 756d 6e5f 7661 6cda 0249  ew_column_val..I
-00000d70: 4463 0500 0000 0000 0000 0000 0000 0600  Dc..............
-00000d80: 0000 0a00 0000 4300 0000 730a 0100 007c  ......C...s....|
-00000d90: 0464 0075 0072 8a7a 507c 006a 008f 3601  .d.u.r.zP|.j..6.
-00000da0: 007c 006a 01a0 0264 017c 006a 039b 0064  .|.j...d.|.j...d
-00000db0: 027c 019b 0064 039d 057c 027c 0366 02a1  .|...d...|.|.f..
-00000dc0: 0201 0057 0064 0004 0004 0083 0301 0057  ...W.d.........W
-00000dd0: 0064 0453 0031 0073 4c30 0001 0001 0001  .d.S.1.sL0......
-00000de0: 0059 0001 0057 006e 2e04 0074 046a 0579  .Y...W.n...t.j.y
-00000df0: 8601 007d 0501 007a 1464 057c 0566 0257  ...}...z.d.|.f.W
-00000e00: 0006 0059 0064 007d 057e 0553 0064 007d  ...Y.d.}.~.S.d.}
-00000e10: 057e 0530 0030 006e 7c7a 4a7c 006a 008f  .~.0.0.n|zJ|.j..
-00000e20: 3001 007c 006a 01a0 0264 017c 049b 0064  0..|.j...d.|...d
-00000e30: 069d 037c 017c 027c 0366 03a1 0201 0057  ...|.|.|.f.....W
-00000e40: 0064 0004 0004 0083 0301 0057 0064 0753  .d.........W.d.S
-00000e50: 0031 0073 c830 0001 0001 0001 0059 0001  .1.s.0.......Y..
-00000e60: 0057 006e 3004 0074 046a 0590 0179 0401  .W.n0..t.j...y..
-00000e70: 007d 0501 007a 1464 087c 0566 0257 0006  .}...z.d.|.f.W..
-00000e80: 0059 0064 007d 057e 0553 0064 007d 057e  .Y.d.}.~.S.d.}.~
-00000e90: 0530 0030 0064 0053 0029 094e 7a07 5550  .0.0.d.S.).Nz.UP
-00000ea0: 4441 5445 207a 0520 5345 5420 7a12 203d  DATE z. SET z. =
-00000eb0: 203f 2057 4845 5245 2049 4420 3d20 3f20   ? WHERE ID = ? 
-00000ec0: 7232 0000 0072 2400 0000 7a18 2053 4554  r2...r$...z. SET
-00000ed0: 203f 203d 203f 2057 4845 5245 2049 4420   ? = ? WHERE ID 
-00000ee0: 3d20 3f20 7225 0000 0072 0100 0000 7233  = ? r%...r....r3
-00000ef0: 0000 0029 0672 1100 0000 723b 0000 0072  ...).r....r;...r
-00000f00: 3c00 0000 723d 0000 0072 3900 0000 7219  <...r=...r9...r.
-00000f10: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00000f20: 0000 da06 7570 6461 7465 6700 0000 7322  ....updateg...s"
-00000f30: 0000 0000 0108 0102 0108 0118 0106 ff04  ................
-00000f40: 0226 0210 0120 0302 0108 0110 0108 ff04  .&... ..........
-00000f50: 0226 0212 017a 0f44 6174 6162 6173 652e  .&...z.Database.
-00000f60: 7570 6461 7465 6302 0000 0000 0000 0000  updatec.........
-00000f70: 0000 0004 0000 000a 0000 0063 0000 0073  ...........c...s
-00000f80: 1a01 0000 7c01 6400 7500 7290 7a56 7c00  ....|.d.u.r.zV|.
-00000f90: 6a00 8f3c 0100 7c00 6a01 a002 6401 7c00  j..<..|.j...d.|.
-00000fa0: 6a03 9b00 6402 9d03 a101 0100 7c00 6a01  j...d.......|.j.
-00000fb0: a004 a100 4400 5d0a 7d02 7c02 5600 0100  ....D.].}.|.V...
-00000fc0: 7132 5700 6400 0400 0400 8303 0100 6e10  q2W.d.........n.
-00000fd0: 3100 7352 3000 0100 0100 0100 5900 0100  1.sR0.......Y...
-00000fe0: 5700 6e2e 0400 7405 6a06 798c 0100 7d03  W.n...t.j.y...}.
-00000ff0: 0100 7a14 6403 7c03 6602 5700 0600 5900  ..z.d.|.f.W...Y.
-00001000: 6400 7d03 7e03 5300 6400 7d03 7e03 3000  d.}.~.S.d.}.~.0.
-00001010: 3000 6e86 7a54 7c00 6a00 8f3a 0100 7c00  0.n.zT|.j..:..|.
-00001020: 6a01 a002 6401 7c01 9b00 6402 9d03 a101  j...d.|...d.....
-00001030: 0100 7c00 6a01 a004 a100 4400 5d0a 7d02  ..|.j.....D.].}.
-00001040: 7c02 5600 0100 71b8 5700 6400 0400 0400  |.V...q.W.d.....
-00001050: 8303 0100 6e10 3100 73d8 3000 0100 0100  ....n.1.s.0.....
-00001060: 0100 5900 0100 5700 6e30 0400 7405 6a06  ..Y...W.n0..t.j.
-00001070: 9001 7914 0100 7d03 0100 7a14 6404 7c03  ..y...}...z.d.|.
-00001080: 6602 5700 0600 5900 6400 7d03 7e03 5300  f.W...Y.d.}.~.S.
-00001090: 6400 7d03 7e03 3000 3000 6400 5300 a905  d.}.~.0.0.d.S...
-000010a0: 4efa 0e53 454c 4543 5420 2a20 4652 4f4d  N..SELECT * FROM
-000010b0: 20fa 0120 7224 0000 0072 0100 0000 a907   .. r$...r......
-000010c0: 720c 0000 0072 0d00 0000 7215 0000 0072  r....r....r....r
-000010d0: 0900 0000 722d 0000 0072 0e00 0000 7217  ....r-...r....r.
-000010e0: 0000 0029 0472 1100 0000 7234 0000 00da  ...).r....r4....
-000010f0: 0372 6f77 7219 0000 0072 1200 0000 7212  .rowr....r....r.
-00001100: 0000 0072 1300 0000 7237 0000 007c 0000  ...r....r7...|..
-00001110: 0073 1e00 0000 0001 0801 0201 0801 1601  .s..............
-00001120: 0e01 2a02 1001 2003 0201 0801 1401 0e01  ..*... .........
-00001130: 2a02 1201 7a10 4461 7461 6261 7365 2e63  *...z.Database.c
-00001140: 6f6e 7465 6e74 2901 da02 6964 6303 0000  ontent)...idc...
-00001150: 0000 0000 0000 0000 0005 0000 000a 0000  ................
-00001160: 0063 0000 0073 2201 0000 7c02 6400 7500  .c...s"...|.d.u.
-00001170: 7294 7a5a 7c00 6a00 8f40 0100 7c00 6a01  r.zZ|.j..@..|.j.
-00001180: a002 6401 7c00 6a03 9b00 6402 9d03 7c01  ..d.|.j...d...|.
-00001190: 6601 a102 0100 7c00 6a01 a004 a100 4400  f.....|.j.....D.
-000011a0: 5d0a 7d03 7c03 5600 0100 7136 5700 6400  ].}.|.V...q6W.d.
-000011b0: 0400 0400 8303 0100 6e10 3100 7356 3000  ........n.1.sV0.
-000011c0: 0100 0100 0100 5900 0100 5700 6e2e 0400  ......Y...W.n...
-000011d0: 7405 6a06 7990 0100 7d04 0100 7a14 6403  t.j.y...}...z.d.
-000011e0: 7c04 6602 5700 0600 5900 6400 7d04 7e04  |.f.W...Y.d.}.~.
-000011f0: 5300 6400 7d04 7e04 3000 3000 6e8a 7a58  S.d.}.~.0.0.n.zX
-00001200: 7c00 6a00 8f3e 0100 7c00 6a01 a002 6401  |.j..>..|.j...d.
-00001210: 7c02 9b00 6402 9d03 7c01 6601 a102 0100  |...d...|.f.....
-00001220: 7c00 6a01 a004 a100 4400 5d0a 7d03 7c03  |.j.....D.].}.|.
-00001230: 5600 0100 71c0 5700 6400 0400 0400 8303  V...q.W.d.......
-00001240: 0100 6e10 3100 73e0 3000 0100 0100 0100  ..n.1.s.0.......
-00001250: 5900 0100 5700 6e30 0400 7405 6a06 9001  Y...W.n0..t.j...
-00001260: 791c 0100 7d04 0100 7a14 6404 7c04 6602  y...}...z.d.|.f.
-00001270: 5700 0600 5900 6400 7d04 7e04 5300 6400  W...Y.d.}.~.S.d.
-00001280: 7d04 7e04 3000 3000 6400 5300 2905 4e72  }.~.0.0.d.S.).Nr
-00001290: 4000 0000 7a0e 2057 4845 5245 2049 4420  @...z. WHERE ID 
-000012a0: 3d20 3f20 7224 0000 0072 0100 0000 7242  = ? r$...r....rB
-000012b0: 0000 0029 0572 1100 0000 7244 0000 0072  ...).r....rD...r
-000012c0: 3400 0000 7243 0000 0072 1900 0000 7212  4...rC...r....r.
-000012d0: 0000 0072 1200 0000 7213 0000 00da 0d63  ...r....r......c
-000012e0: 6f6e 7465 6e74 5f62 795f 6964 9100 0000  ontent_by_id....
-000012f0: 731e 0000 0000 0108 0102 0108 011a 010e  s...............
-00001300: 012a 0210 0120 0302 0108 0118 010e 012a  .*... .........*
-00001310: 0212 017a 1644 6174 6162 6173 652e 636f  ...z.Database.co
-00001320: 6e74 656e 745f 6279 5f69 6463 0100 0000  ntent_by_idc....
-00001330: 0000 0000 0000 0000 0500 0000 0a00 0000  ................
-00001340: 6700 0000 732a 0100 007c 0172 987a 627c  g...s*...|.r.zb|
-00001350: 0144 005d 587d 027c 006a 008f 3e01 007c  .D.]X}.|.j..>..|
-00001360: 006a 01a0 0264 017c 029b 0064 029d 03a1  .j...d.|...d....
-00001370: 0101 007c 006a 01a0 03a1 0044 005d 0e7d  ...|.j.....D.].}
-00001380: 037c 027c 0369 0156 0001 0071 3457 0064  .|.|.i.V...q4W.d
-00001390: 0004 0004 0083 0301 0071 0a31 0073 5830  .........q.1.sX0
-000013a0: 0001 0001 0001 0059 0001 0071 0a57 006e  .......Y...q.W.n
-000013b0: 2e04 0074 046a 0579 9401 007d 0401 007a  ...t.j.y...}...z
-000013c0: 1464 037c 0466 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
-000013d0: 047e 0453 0064 007d 047e 0430 0030 006e  .~.S.d.}.~.0.0.n
-000013e0: 8e7a 5c7c 006a 008f 4201 007c 006a 01a0  .z\|.j..B..|.j..
-000013f0: 0264 017c 006a 069b 0064 029d 03a1 0101  .d.|.j...d......
-00001400: 007c 006a 01a0 03a1 0044 005d 107d 037c  .|.j.....D.].}.|
-00001410: 006a 067c 0369 0156 0001 0071 c257 0064  .j.|.i.V...q.W.d
-00001420: 0004 0004 0083 0301 006e 1031 0073 e830  .........n.1.s.0
-00001430: 0001 0001 0001 0059 0001 0057 006e 3004  .......Y...W.n0.
-00001440: 0074 046a 0590 0179 2401 007d 0401 007a  .t.j...y$..}...z
-00001450: 1464 047c 0466 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
-00001460: 047e 0453 0064 007d 047e 0430 0030 0064  .~.S.d.}.~.0.0.d
-00001470: 0053 0072 3f00 0000 2907 720c 0000 0072  .S.r?...).r....r
-00001480: 0d00 0000 7215 0000 0072 2d00 0000 720e  ....r....r-...r.
-00001490: 0000 0072 1700 0000 7209 0000 0029 0572  ...r....r....).r
-000014a0: 1100 0000 5a13 6f70 7469 6f6e 616c 5f74  ....Z.optional_t
-000014b0: 6162 6c65 6e61 6d65 73da 0361 7267 7243  ablenames..argrC
-000014c0: 0000 0072 1900 0000 7212 0000 0072 1200  ...r....r....r..
-000014d0: 0000 7213 0000 00da 0d73 686f 775f 636f  ..r......show_co
-000014e0: 6e74 656e 7473 a600 0000 7320 0000 0000  ntents....s ....
-000014f0: 0104 0102 0108 0108 0114 010e 0130 0210  .............0..
-00001500: 0120 0302 0108 0116 010e 0130 0212 017a  . .........0...z
-00001510: 1644 6174 6162 6173 652e 7368 6f77 5f63  .Database.show_c
-00001520: 6f6e 7465 6e74 7363 0100 0000 0000 0000  ontentsc........
-00001530: 0000 0000 0300 0000 0a00 0000 6300 0000  ............c...
-00001540: 7380 0000 007a 4c7c 006a 008f 3201 007c  s....zL|.j..2..|
-00001550: 006a 01a0 0264 01a1 0101 007c 006a 01a0  .j...d.....|.j..
-00001560: 03a1 0044 005d 0a7d 017c 0156 0001 0071  ...D.].}.|.V...q
-00001570: 2057 0064 0004 0004 0083 0301 006e 1031   W.d.........n.1
-00001580: 0073 4030 0001 0001 0001 0059 0001 0057  .s@0.......Y...W
-00001590: 006e 2e04 0074 046a 0579 7a01 007d 0201  .n...t.j.yz..}..
-000015a0: 007a 1464 027c 0266 0257 0006 0059 0064  .z.d.|.f.W...Y.d
-000015b0: 007d 027e 0253 0064 007d 027e 0230 0030  .}.~.S.d.}.~.0.0
-000015c0: 0064 0053 0029 034e fa33 5345 4c45 4354  .d.S.).N.3SELECT
-000015d0: 206e 616d 6520 4652 4f4d 2073 716c 6974   name FROM sqlit
-000015e0: 655f 6d61 7374 6572 2057 4845 5245 2074  e_master WHERE t
-000015f0: 7970 653d 2027 7461 626c 6527 2072 0100  ype= 'table' r..
-00001600: 0000 a906 720c 0000 0072 0d00 0000 7215  ....r....r....r.
-00001610: 0000 0072 2d00 0000 720e 0000 0072 1700  ...r-...r....r..
-00001620: 0000 2903 7211 0000 0072 4300 0000 7219  ..).r....rC...r.
-00001630: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00001640: 0000 da0b 7368 6f77 5f74 6162 6c65 73bc  ....show_tables.
-00001650: 0000 0073 0e00 0000 0001 0201 0801 0c01  ...s............
-00001660: 0e01 2a02 1001 7a14 4461 7461 6261 7365  ..*...z.Database
-00001670: 2e73 686f 775f 7461 626c 6573 6301 0000  .show_tablesc...
-00001680: 0000 0000 0000 0000 0003 0000 000a 0000  ................
-00001690: 0043 0000 0073 9400 0000 7a60 7c00 6a00  .C...s....z`|.j.
-000016a0: 8f46 0100 7c00 6a01 a002 6401 a101 0100  .F..|.j...d.....
-000016b0: 7c00 6a01 a003 a100 4400 5d1a 7d01 7c00  |.j.....D.].}.|.
-000016c0: 6a01 a002 6402 7c01 6403 1900 9b00 9d02  j...d.|.d.......
-000016d0: a101 0100 7120 5700 6400 0400 0400 8303  ....q W.d.......
-000016e0: 0100 5700 6404 5300 3100 7354 3000 0100  ..W.d.S.1.sT0...
-000016f0: 0100 0100 5900 0100 5700 6e2e 0400 7404  ....Y...W.n...t.
-00001700: 6a05 798e 0100 7d02 0100 7a14 6403 7c02  j.y...}...z.d.|.
-00001710: 6602 5700 0600 5900 6400 7d02 7e02 5300  f.W...Y.d.}.~.S.
-00001720: 6400 7d02 7e02 3000 3000 6400 5300 2905  d.}.~.0.0.d.S.).
-00001730: 4e72 4800 0000 fa0b 4452 4f50 2054 4142  NrH.....DROP TAB
-00001740: 4c45 2072 0100 0000 7225 0000 0072 4900  LE r....r%...rI.
-00001750: 0000 2903 7211 0000 00da 0574 6162 6c65  ..).r......table
-00001760: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00001770: 1300 0000 da07 6472 6f70 616c 6cc6 0000  ......dropall...
-00001780: 0073 1000 0000 0001 0201 0801 0c01 0e01  .s..............
-00001790: 1801 2602 1001 7a10 4461 7461 6261 7365  ..&...z.Database
-000017a0: 2e64 726f 7061 6c6c 6301 0000 0000 0000  .dropallc.......
-000017b0: 0000 0000 0004 0000 000a 0000 0047 0000  .............G..
-000017c0: 0073 f600 0000 7c01 727e 7a48 7c01 4400  .s....|.r~zH|.D.
-000017d0: 5d3c 7d02 7c00 6a00 8f22 0100 7c00 6a01  ]<}.|.j.."..|.j.
-000017e0: a002 6401 7c02 9b00 9d02 a101 0100 5700  ..d.|.........W.
-000017f0: 6400 0400 0400 8303 0100 710a 3100 733c  d.........q.1.s<
-00001800: 3000 0100 0100 0100 5900 0100 710a 5700  0.......Y...q.W.
-00001810: 6402 5300 0400 7403 6a04 797a 0100 7d03  d.S...t.j.yz..}.
-00001820: 0100 7a14 6403 7c03 6602 5700 0600 5900  ..z.d.|.f.W...Y.
-00001830: 6400 7d03 7e03 5300 6400 7d03 7e03 3000  d.}.~.S.d.}.~.0.
-00001840: 3000 6e74 7a42 7c00 6a00 8f28 0100 7c00  0.ntzB|.j..(..|.
-00001850: 6a01 a002 6401 7c00 6a05 9b00 9d02 a101  j...d.|.j.......
-00001860: 0100 5700 6400 0400 0400 8303 0100 5700  ..W.d.........W.
-00001870: 6402 5300 3100 73b4 3000 0100 0100 0100  d.S.1.s.0.......
-00001880: 5900 0100 5700 6e30 0400 7403 6a04 9000  Y...W.n0..t.j...
-00001890: 79f0 0100 7d03 0100 7a14 6404 7c03 6602  y...}...z.d.|.f.
-000018a0: 5700 0600 5900 6400 7d03 7e03 5300 6400  W...Y.d.}.~.S.d.
-000018b0: 7d03 7e03 3000 3000 6400 5300 2905 4e72  }.~.0.0.d.S.).Nr
-000018c0: 4b00 0000 7225 0000 0072 2400 0000 7201  K...r%...r$...r.
-000018d0: 0000 0029 0672 0c00 0000 720d 0000 0072  ...).r....r....r
-000018e0: 1500 0000 720e 0000 0072 1700 0000 7209  ....r....r....r.
-000018f0: 0000 0029 0472 1100 0000 5a0b 7461 626c  ...).r....Z.tabl
-00001900: 655f 6e61 6d65 7372 4600 0000 7219 0000  e_namesrF...r...
-00001910: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00001920: da0a 6472 6f70 5f74 6162 6c65 d100 0000  ..drop_table....
-00001930: 731c 0000 0000 0104 0102 0108 0108 0132  s..............2
-00001940: 0106 0110 0120 0302 0108 0114 0126 0212  ..... .......&..
-00001950: 017a 1344 6174 6162 6173 652e 6472 6f70  .z.Database.drop
-00001960: 5f74 6162 6c65 6303 0000 0000 0000 0000  _tablec.........
-00001970: 0000 0004 0000 000a 0000 0043 0000 0073  ...........C...s
-00001980: fa00 0000 7c02 6400 7500 7280 7a46 7c00  ....|.d.u.r.zF|.
-00001990: 6a00 8f2a 0100 7c00 6a01 a002 6401 7c00  j..*..|.j...d.|.
-000019a0: 6a03 9b00 6402 7c01 9b00 9d04 a101 0100  j...d.|.........
-000019b0: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
-000019c0: 7340 3000 0100 0100 0100 5900 0100 5700  s@0.......Y...W.
-000019d0: 6403 5300 0400 7404 6a05 797c 0100 7d03  d.S...t.j.y|..}.
-000019e0: 0100 7a14 6404 7c03 6602 5700 0600 5900  ..z.d.|.f.W...Y.
-000019f0: 6400 7d03 7e03 5300 6400 7d03 7e03 3000  d.}.~.S.d.}.~.0.
-00001a00: 3000 6e76 7a44 7c00 6a00 8f28 0100 7c00  0.nvzD|.j..(..|.
-00001a10: 6a01 a002 6401 7c02 9b00 6402 7c01 9b00  j...d.|...d.|...
-00001a20: 9d04 a101 0100 5700 6400 0400 0400 8303  ......W.d.......
-00001a30: 0100 6e10 3100 73b6 3000 0100 0100 0100  ..n.1.s.0.......
-00001a40: 5900 0100 5700 6405 5300 0400 7404 6a05  Y...W.d.S...t.j.
-00001a50: 9000 79f4 0100 7d03 0100 7a14 6406 7c03  ..y...}...z.d.|.
-00001a60: 6602 5700 0600 5900 6400 7d03 7e03 5300  f.W...Y.d.}.~.S.
-00001a70: 6400 7d03 7e03 3000 3000 6400 5300 2907  d.}.~.0.0.d.S.).
-00001a80: 4e7a 0c44 454c 4554 4520 4652 4f4d 207a  Nz.DELETE FROM z
-00001a90: 0c20 5748 4552 4520 4944 203d 2072 3200  . WHERE ID = r2.
-00001aa0: 0000 7224 0000 0072 2500 0000 7201 0000  ..r$...r%...r...
-00001ab0: 0072 3300 0000 2904 7211 0000 0072 3d00  .r3...).r....r=.
-00001ac0: 0000 7239 0000 0072 1900 0000 7212 0000  ..r9...r....r...
-00001ad0: 0072 1200 0000 7213 0000 00da 0c64 726f  .r....r......dro
-00001ae0: 705f 636f 6e74 656e 74e4 0000 0073 1a00  p_content....s..
-00001af0: 0000 0001 0801 0201 0801 3801 0602 1001  ..........8.....
-00001b00: 2003 0201 0801 3601 0602 1201 7a15 4461   .....6.....z.Da
-00001b10: 7461 6261 7365 2e64 726f 705f 636f 6e74  tabase.drop_cont
-00001b20: 656e 7429 014e 2901 4e29 014e 2901 4e29  ent).N).N).N).N)
-00001b30: 014e 2901 4e29 22da 085f 5f6e 616d 655f  .N).N)"..__name_
-00001b40: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00001b50: 5f71 7561 6c6e 616d 655f 5f72 0300 0000  _qualname__r....
-00001b60: 7207 0000 0072 2a00 0000 da0f 5f5f 616e  r....r*.....__an
-00001b70: 6e6f 7461 7469 6f6e 735f 5f72 0900 0000  notations__r....
-00001b80: 720c 0000 0072 0e00 0000 5a0a 436f 6e6e  r....r....Z.Conn
-00001b90: 6563 7469 6f6e 720d 0000 005a 0643 7572  ectionr....Z.Cur
-00001ba0: 736f 7272 1400 0000 da08 7072 6f70 6572  sorr......proper
-00001bb0: 7479 7218 0000 0072 0500 0000 7204 0000  tyr....r....r...
-00001bc0: 00da 0574 7570 6c65 7220 0000 0072 2200  ...tupler ...r".
-00001bd0: 0000 da04 6c69 7374 7231 0000 0072 3500  ....listr1...r5.
-00001be0: 0000 723a 0000 00da 0369 6e74 723e 0000  ..r:.....intr>..
-00001bf0: 0072 3700 0000 7245 0000 0072 4700 0000  .r7...rE...rG...
-00001c00: 724a 0000 0072 4d00 0000 724e 0000 0072  rJ...rM...rN...r
-00001c10: 4f00 0000 7212 0000 0072 1200 0000 7212  O...r....r....r.
-00001c20: 0000 0072 1300 0000 7206 0000 0007 0000  ...r....r.......
-00001c30: 0073 2c00 0000 0a02 0e01 1201 1601 1602  .s,.............
-00001c40: 0804 0201 0a0a 0201 1808 0201 0a03 1011  ................
-00001c50: 0a18 0a14 1415 0a15 1015 0816 0e0a 080b  ................
-00001c60: 0813 7206 0000 00da 085f 5f6d 6169 6e5f  ..r......__main_
-00001c70: 5f7a 0c70 6f73 745f 7465 7374 2e64 627a  _z.post_test.dbz
-00001c80: 0723 3534 3832 4146 7a0b 4d79 2041 6363  .#5482AFz.My Acc
-00001c90: 6f75 6e74 737a 2a73 6f6d 6520 656e 6372  ountsz*some encr
-00001ca0: 7970 7465 6420 636f 6e74 656e 7420 6f66  ypted content of
-00001cb0: 2062 7974 6573 206f 7220 7374 7269 6e67   bytes or string
-00001cc0: 737a 5653 454c 4543 5420 434f 554e 5428  szVSELECT COUNT(
-00001cd0: 2a29 2041 5320 6363 202c 636f 6e74 656e  *) AS cc ,conten
-00001ce0: 7420 4652 4f4d 2043 6c61 7373 6966 6965  t FROM Classifie
-00001cf0: 6420 5748 4552 4520 6b65 7920 3d20 2223  d WHERE key = "#
-00001d00: 3534 3832 4146 2220 4f52 4445 5220 4259  5482AF" ORDER BY
-00001d10: 2063 6320 4445 5343 2029 145a 0b64 6174   cc DESC ).Z.dat
-00001d20: 6163 6c61 7373 6573 7202 0000 0072 0300  aclassesr....r..
-00001d30: 0000 7204 0000 00da 0674 7970 696e 6772  ..r......typingr
-00001d40: 0500 0000 720e 0000 0072 1c00 0000 7206  ....r....r....r.
-00001d50: 0000 0072 5000 0000 720c 0000 0072 3500  ...rP...r....r5.
-00001d60: 0000 7238 0000 0072 3a00 0000 724a 0000  ..r8...r:...rJ..
-00001d70: 0072 1900 0000 da05 7072 696e 7472 1800  .r......printr..
-00001d80: 0000 5a06 7175 6572 7931 7231 0000 0072  ..Z.query1r1...r
-00001d90: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00001da0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001db0: 0073 2200 0000 1001 0c01 0c01 0801 0802  .s".............
-00001dc0: 0201 107f 0070 0801 0801 0802 0401 0e01  .....p..........
-00001dd0: 0c01 0a01 0a01 0401                      ........
+00000070: 6406 8302 8301 5a08 6404 5300 2907 e900  d.....Z.d.S.)...
+00000080: 0000 0029 02da 0964 6174 6163 6c61 7373  ...)...dataclass
+00000090: da05 6669 656c 6429 01da 0864 6174 6574  ..field)...datet
+000000a0: 696d 6529 01da 0555 6e69 6f6e 4e63 0000  ime)...UnionNc..
+000000b0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+000000c0: 0000 4000 0000 7316 0100 0065 005a 0164  ..@...s....e.Z.d
+000000d0: 005a 0255 0065 0383 005a 0465 0565 0664  .Z.U.e...Z.e.e.d
+000000e0: 013c 0065 0364 0264 038d 015a 0765 0565  .<.e.d.d...Z.e.e
+000000f0: 0664 043c 0065 0364 0564 0564 068d 025a  .d.<.e.d.d.d...Z
+00000100: 0865 096a 0a65 0664 073c 0065 0364 0564  .e.j.e.d.<.e.d.d
+00000110: 0564 068d 025a 0b65 096a 0c65 0664 083c  .d...Z.e.j.e.d.<
+00000120: 0064 0964 0a84 005a 0d65 0e64 0b64 0c84  .d.d...Z.e.d.d..
+00000130: 0083 015a 0f65 0e65 1065 1165 1266 0219  ...Z.e.e.e.e.f..
+00000140: 0064 0d9c 0164 0e64 0f84 0483 015a 1365  .d...d.d.....Z.e
+00000150: 0e64 1064 1184 0083 015a 1465 0565 1564  .d.d.....Z.e.e.d
+00000160: 129c 0264 1364 1484 045a 1664 2c64 1664  ...d.d...Z.d,d.d
+00000170: 1784 015a 1764 2d64 1864 1984 015a 1864  ...Z.d-d.d...Z.d
+00000180: 2e65 0565 0565 1964 1a9c 0364 1b64 1c84  .e.e.e.d...d.d..
+00000190: 055a 1a64 2f64 1d64 1e84 015a 1b64 3065  .Z.d/d.d...Z.d0e
+000001a0: 1964 1f9c 0164 2064 2184 055a 1c64 2264  .d...d d!..Z.d"d
+000001b0: 2384 005a 1d65 1264 0d9c 0164 2464 2584  #..Z.e.d...d$d%.
+000001c0: 045a 1e64 2664 2784 005a 1f64 2864 2984  .Z.d&d'..Z.d(d).
+000001d0: 005a 2064 3164 2a64 2b84 015a 2164 1553  .Z d1d*d+..Z!d.S
+000001e0: 0029 32da 0844 6174 6162 6173 65da 0664  .)2..Database..d
+000001f0: 626e 616d 655a 0a43 6c61 7373 6966 6965  bnameZ.Classifie
+00000200: 6429 01da 0764 6566 6175 6c74 da09 7461  d)...default..ta
+00000210: 626c 656e 616d 6546 2902 da04 696e 6974  blenameF)...init
+00000220: da04 7265 7072 da04 636f 6e6e da01 6363  ..repr..conn..cc
+00000230: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000240: 0300 0000 4300 0000 731e 0000 0074 00a0  ....C...s....t..
+00000250: 017c 006a 02a1 017c 005f 037c 006a 03a0  .|.j...|._.|.j..
+00000260: 04a1 007c 005f 0564 0053 0029 014e 2906  ...|._.d.S.).N).
+00000270: da07 7371 6c69 7465 33da 0763 6f6e 6e65  ..sqlite3..conne
+00000280: 6374 7207 0000 0072 0c00 0000 5a06 6375  ctr....r....Z.cu
+00000290: 7273 6f72 720d 0000 00a9 01da 0473 656c  rsorr........sel
+000002a0: 66a9 0072 1200 0000 fa2f 433a 5c57 6f72  f..r...../C:\Wor
+000002b0: 6b5c 4769 7448 7562 576f 726b 5c41 4553  k\GitHubWork\AES
+000002c0: 2d32 3536 5c41 7368 4372 7970 745c 4461  -256\AshCrypt\Da
+000002d0: 7461 6261 7365 2e70 79da 0d5f 5f70 6f73  tabase.py..__pos
+000002e0: 745f 696e 6974 5f5f 0e00 0000 7304 0000  t_init__....s...
+000002f0: 0000 010e 017a 1644 6174 6162 6173 652e  .....z.Database.
+00000300: 5f5f 706f 7374 5f69 6e69 745f 5f63 0100  __post_init__c..
+00000310: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
+00000320: 0000 4300 0000 738a 0000 007a 567c 006a  ..C...s....zV|.j
+00000330: 008f 3c01 007c 006a 01a0 0264 01a1 0101  ..<..|.j...d....
+00000340: 007c 006a 01a0 03a1 007d 017c 0164 0219  .|.j.....}.|.d..
+00000350: 0064 031b 0064 031b 007d 027c 0257 0002  .d...d...}.|.W..
+00000360: 0064 0004 0004 0083 0301 0057 0053 0031  .d.........W.S.1
+00000370: 0073 4a30 0001 0001 0001 0059 0001 0057  .sJ0.......Y...W
+00000380: 006e 2e04 0074 046a 0579 8401 007d 0301  .n...t.j.y...}..
+00000390: 007a 1464 027c 0366 0257 0006 0059 0064  .z.d.|.f.W...Y.d
+000003a0: 007d 037e 0353 0064 007d 037e 0330 0030  .}.~.S.d.}.~.0.0
+000003b0: 0064 0053 0029 044e 7a49 5345 4c45 4354  .d.S.).NzISELECT
+000003c0: 2070 6167 655f 636f 756e 7420 2a20 7061   page_count * pa
+000003d0: 6765 5f73 697a 6520 4652 4f4d 2070 7261  ge_size FROM pra
+000003e0: 676d 615f 7061 6765 5f63 6f75 6e74 2829  gma_page_count()
+000003f0: 202c 2070 7261 676d 615f 7061 6765 5f73   , pragma_page_s
+00000400: 697a 6572 0100 0000 6900 0400 0029 0672  izer....i....).r
+00000410: 0c00 0000 720d 0000 00da 0765 7865 6375  ....r......execu
+00000420: 7465 da08 6665 7463 686f 6e65 720e 0000  te..fetchoner...
+00000430: 00da 0545 7272 6f72 2904 7211 0000 005a  ...Error).r....Z
+00000440: 0973 697a 655f 696e 666f da04 7369 7a65  .size_info..size
+00000450: da01 6572 1200 0000 7212 0000 0072 1300  ..er....r....r..
+00000460: 0000 7218 0000 0012 0000 0073 1000 0000  ..r........s....
+00000470: 0002 0201 0801 0c01 0a01 1001 2801 1001  ............(...
+00000480: 7a0d 4461 7461 6261 7365 2e73 697a 6529  z.Database.size)
+00000490: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
+000004a0: 0000 0000 0000 0300 0000 0a00 0000 4300  ..............C.
+000004b0: 0000 734c 0000 007a 1a74 00a0 0174 02a0  ..sL...z.t...t..
+000004c0: 037c 006a 04a1 016a 05a1 017d 017c 0157  .|.j...j...}.|.W
+000004d0: 0053 0004 0074 0679 4601 007d 0201 007a  .S...t.yF..}...z
+000004e0: 1464 017c 0266 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
+000004f0: 027e 0253 0064 007d 027e 0230 0030 0064  .~.S.d.}.~.0.0.d
+00000500: 0053 0029 024e 7201 0000 0029 0772 0400  .S.).Nr....).r..
+00000510: 0000 da0d 6672 6f6d 7469 6d65 7374 616d  ....fromtimestam
+00000520: 70da 026f 73da 0473 7461 7472 0700 0000  p..os..statr....
+00000530: da08 7374 5f6d 7469 6d65 da07 4f53 4572  ..st_mtime..OSEr
+00000540: 726f 7229 0372 1100 0000 5a09 7469 6d65  ror).r....Z.time
+00000550: 5f73 7461 7472 1900 0000 7212 0000 0072  _statr....r....r
+00000560: 1200 0000 7213 0000 00da 086c 6173 745f  ....r......last_
+00000570: 6d6f 641d 0000 0073 0a00 0000 0002 0201  mod....s........
+00000580: 1401 0602 0e01 7a11 4461 7461 6261 7365  ......z.Database
+00000590: 2e6c 6173 745f 6d6f 6463 0100 0000 0000  .last_modc......
+000005a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000005b0: 0000 730e 0000 0064 017c 006a 009b 0064  ..s....d.|.j...d
+000005c0: 029d 0353 0029 034e 7a20 4445 4641 554c  ...S.).Nz DEFAUL
+000005d0: 5420 524f 5554 494e 4720 414c 4c20 4d45  T ROUTING ALL ME
+000005e0: 5448 4f44 5320 544f 2022 fa01 2229 0172  THODS TO "..").r
+000005f0: 0900 0000 7210 0000 0072 1200 0000 7212  ....r....r....r.
+00000600: 0000 0072 1300 0000 da0f 6465 6661 756c  ...r......defaul
+00000610: 745f 726f 7574 696e 6726 0000 0073 0200  t_routing&...s..
+00000620: 0000 0002 7a18 4461 7461 6261 7365 2e64  ....z.Database.d
+00000630: 6566 6175 6c74 5f72 6f75 7469 6e67 2902  efault_routing).
+00000640: da06 7175 6572 7973 721a 0000 0063 0100  ..querysr....c..
+00000650: 0000 0000 0000 0000 0000 0600 0000 0b00  ................
+00000660: 0000 4700 0000 7300 0100 0067 007d 0274  ..G...s....g.}.t
+00000670: 007c 0183 0144 005d ee5c 027d 037d 0474  .|...D.].\.}.}.t
+00000680: 017c 0474 0283 0273 367c 02a0 0364 017c  .|.t...s6|...d.|
+00000690: 039b 009d 0264 0274 0466 0269 01a1 0101  .....d.t.f.i....
+000006a0: 007a 807c 006a 058f 6601 007c 006a 06a0  .z.|.j..f..|.j..
+000006b0: 077c 04a1 0101 007c 006a 066a 0864 036b  .|.....|.j.j.d.k
+000006c0: 0272 787c 02a0 0364 017c 039b 009d 0264  .rx|...d.|.....d
+000006d0: 047c 006a 06a0 09a1 0067 0269 01a1 0101  .|.j.....g.i....
+000006e0: 006e 1e7c 02a0 0364 017c 039b 009d 0264  .n.|...d.|.....d
+000006f0: 047c 006a 06a0 0aa1 0067 0269 01a1 0101  .|.j.....g.i....
+00000700: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00000710: 0073 aa30 0001 0001 0001 0059 0001 0057  .s.0.......Y...W
+00000720: 0071 0c04 0074 0b6a 0c79 f801 007d 0501  .q...t.j.y...}..
+00000730: 007a 287c 02a0 0364 017c 039b 009d 0264  .z(|...d.|.....d
+00000740: 057c 05a0 0da1 0066 0269 01a1 0101 0057  .|.....f.i.....W
+00000750: 0059 0064 007d 057e 0571 0c64 007d 057e  .Y.d.}.~.q.d.}.~
+00000760: 0530 0030 0071 0c7c 0253 0029 064e 7a06  .0.0.q.|.S.).Nz.
+00000770: 7175 6572 7920 e700 0000 0000 0000 00e9  query ..........
+00000780: 0100 0000 da07 5355 4343 4553 53da 0746  ......SUCCESS..F
+00000790: 4149 4c55 5245 290e da09 656e 756d 6572  AILURE)...enumer
+000007a0: 6174 65da 0a69 7369 6e73 7461 6e63 65da  ate..isinstance.
+000007b0: 0373 7472 da06 6170 7065 6e64 da09 5479  .str..append..Ty
+000007c0: 7065 4572 726f 7272 0c00 0000 720d 0000  peErrorr....r...
+000007d0: 0072 1500 0000 5a08 726f 7763 6f75 6e74  .r....Z.rowcount
+000007e0: 7216 0000 00da 0866 6574 6368 616c 6c72  r......fetchallr
+000007f0: 0e00 0000 7217 0000 00da 075f 5f73 7472  ....r......__str
+00000800: 5f5f 2906 7211 0000 0072 2300 0000 da06  __).r....r#.....
+00000810: 7265 7375 6c74 da01 69da 0571 7565 7279  result..i..query
+00000820: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000830: 1300 0000 7231 0000 002a 0000 0073 1a00  ....r1...*...s..
+00000840: 0000 0001 0401 1001 0a01 1801 0201 0801  ................
+00000850: 0c01 0c01 2002 4002 1001 3401 7a0e 4461  .... .@...4.z.Da
+00000860: 7461 6261 7365 2e71 7565 7279 4e63 0200  tabase.queryNc..
+00000870: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+00000880: 0000 4300 0000 73f8 0000 007c 0164 0075  ..C...s....|.d.u
+00000890: 0072 7c7a 427c 006a 008f 2601 007c 006a  .r|zB|.j..&..|.j
+000008a0: 01a0 0264 017c 006a 039b 0064 029d 03a1  ...d.|.j...d....
+000008b0: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+000008c0: 1031 0073 3c30 0001 0001 0001 0059 0001  .1.s<0.......Y..
+000008d0: 0057 0064 0353 0004 0074 046a 0579 7801  .W.d.S...t.j.yx.
+000008e0: 007d 0201 007a 1464 047c 0266 0257 0006  .}...z.d.|.f.W..
+000008f0: 0059 0064 007d 027e 0253 0064 007d 027e  .Y.d.}.~.S.d.}.~
+00000900: 0230 0030 006e 787a 467c 006a 008f 2a01  .0.0.nxzF|.j..*.
+00000910: 007c 006a 01a0 0264 017c 019b 0064 059d  .|.j...d.|...d..
+00000920: 03a1 0101 007c 017c 005f 0357 0064 0004  .....|.|._.W.d..
+00000930: 0004 0083 0301 006e 1031 0073 b430 0001  .......n.1.s.0..
+00000940: 0001 0001 0059 0001 0057 0064 0653 0004  .....Y...W.d.S..
+00000950: 0074 046a 0590 0079 f201 007d 0201 007a  .t.j...y...}...z
+00000960: 1464 077c 0266 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
+00000970: 027e 0253 0064 007d 027e 0230 0030 0064  .~.S.d.}.~.0.0.d
+00000980: 0053 0029 084e 7a1b 4352 4541 5445 2054  .S.).Nz.CREATE T
+00000990: 4142 4c45 2049 4620 4e4f 5420 4558 4953  ABLE IF NOT EXIS
+000009a0: 5453 207a 3e20 2849 4420 494e 5445 4745  TS z> (ID INTEGE
+000009b0: 5220 5052 494d 4152 5920 4b45 592c 204e  R PRIMARY KEY, N
+000009c0: 616d 6520 5465 7874 202c 2043 6f6e 7465  ame Text , Conte
+000009d0: 6e74 2042 4c4f 4220 2c4b 6579 2054 4558  nt BLOB ,Key TEX
+000009e0: 5420 29e9 0b00 0000 7224 0000 007a 3c20  T ).....r$...z< 
+000009f0: 2849 4420 494e 5445 4745 5220 5052 494d  (ID INTEGER PRIM
+00000a00: 4152 5920 4b45 592c 4e61 6d65 2054 4558  ARY KEY,Name TEX
+00000a10: 5420 2c43 6f6e 7465 6e74 2042 4c4f 4220  T ,Content BLOB 
+00000a20: 2c4b 6579 2054 4558 5420 2972 2500 0000  ,Key TEXT )r%...
+00000a30: 7201 0000 00a9 0672 0c00 0000 720d 0000  r......r....r...
+00000a40: 0072 1500 0000 7209 0000 0072 0e00 0000  .r....r....r....
+00000a50: 7217 0000 0029 0372 1100 0000 da12 6f70  r....).r......op
+00000a60: 7469 6f6e 616c 5f74 6162 6c65 6e61 6d65  tional_tablename
+00000a70: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000a80: 1300 0000 da08 6164 6474 6162 6c65 3b00  ......addtable;.
+00000a90: 0000 731c 0000 0000 0108 0102 0108 0134  ..s............4
+00000aa0: 0206 0110 0120 0302 0108 0114 0524 0106  ..... .......$..
+00000ab0: 0212 017a 1144 6174 6162 6173 652e 6164  ...z.Database.ad
+00000ac0: 6474 6162 6c65 6305 0000 0000 0000 0000  dtablec.........
+00000ad0: 0000 0006 0000 000a 0000 0043 0000 0073  ...........C...s
+00000ae0: 0201 0000 7c04 6400 7500 7284 7a4a 7c00  ....|.d.u.r.zJ|.
+00000af0: 6a00 8f2e 0100 7c00 6a01 a002 6401 7c00  j.....|.j...d.|.
+00000b00: 6a03 9b00 6402 9d03 7c01 7c02 7c03 6603  j...d...|.|.|.f.
+00000b10: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00000b20: 6e10 3100 7344 3000 0100 0100 0100 5900  n.1.sD0.......Y.
+00000b30: 0100 5700 6403 5300 0400 7404 6a05 7980  ..W.d.S...t.j.y.
+00000b40: 0100 7d05 0100 7a14 6404 7c05 6602 5700  ..}...z.d.|.f.W.
+00000b50: 0600 5900 6400 7d05 7e05 5300 6400 7d05  ..Y.d.}.~.S.d.}.
+00000b60: 7e05 3000 3000 6e7a 7a48 7c00 6a00 8f2c  ~.0.0.nzzH|.j..,
+00000b70: 0100 7c00 6a01 a002 6401 7c04 9b00 6405  ..|.j...d.|...d.
+00000b80: 9d03 7c01 7c02 7c03 6603 a102 0100 5700  ..|.|.|.f.....W.
+00000b90: 6400 0400 0400 8303 0100 6e10 3100 73be  d.........n.1.s.
+00000ba0: 3000 0100 0100 0100 5900 0100 5700 6406  0.......Y...W.d.
+00000bb0: 5300 0400 7404 6a05 9000 79fc 0100 7d05  S...t.j...y...}.
+00000bc0: 0100 7a14 6407 7c05 6602 5700 0600 5900  ..z.d.|.f.W...Y.
+00000bd0: 6400 7d05 7e05 5300 6400 7d05 7e05 3000  d.}.~.S.d.}.~.0.
+00000be0: 3000 6400 5300 2908 4e7a 0c49 4e53 4552  0.d.S.).Nz.INSER
+00000bf0: 5420 494e 544f 207a 2a20 284e 616d 6520  T INTO z* (Name 
+00000c00: 2c20 436f 6e74 656e 7420 2c4b 6579 2920  , Content ,Key) 
+00000c10: 5641 4c55 4553 2028 3f20 2c20 3f20 2c20  VALUES (? , ? , 
+00000c20: 3f29 2072 3200 0000 7224 0000 007a 2920  ?) r2...r$...z) 
+00000c30: 284e 616d 652c 2043 6f6e 7465 6e74 202c  (Name, Content ,
+00000c40: 4b65 7929 2056 414c 5545 5320 283f 202c  Key) VALUES (? ,
+00000c50: 203f 202c 203f 2920 7225 0000 0072 0100   ? , ?) r%...r..
+00000c60: 0000 7233 0000 0029 0672 1100 0000 da04  ..r3...).r......
+00000c70: 6e61 6d65 da07 636f 6e74 656e 74da 036b  name..content..k
+00000c80: 6579 da13 6f70 7469 6f6e 616c 5f74 6162  ey..optional_tab
+00000c90: 6c65 5f6e 616d 6572 1900 0000 7212 0000  le_namer....r...
+00000ca0: 0072 1200 0000 7213 0000 00da 0669 6e73  .r....r......ins
+00000cb0: 6572 7453 0000 0073 2200 0000 0001 0801  ertS...s".......
+00000cc0: 0201 0801 1201 08ff 2203 0601 1001 2003  ........"..... .
+00000cd0: 0201 0801 1001 08ff 2202 0601 1201 7a0f  ........".....z.
+00000ce0: 4461 7461 6261 7365 2e69 6e73 6572 7429  Database.insert)
+00000cf0: 03da 0b63 6f6c 756d 6e5f 6e61 6d65 da0e  ...column_name..
+00000d00: 6e65 775f 636f 6c75 6d6e 5f76 616c da02  new_column_val..
+00000d10: 4944 6305 0000 0000 0000 0000 0000 0006  IDc.............
+00000d20: 0000 000a 0000 0043 0000 0073 0a01 0000  .......C...s....
+00000d30: 7c04 6400 7500 728a 7a50 7c00 6a00 8f36  |.d.u.r.zP|.j..6
+00000d40: 0100 7c00 6a01 a002 6401 7c00 6a03 9b00  ..|.j...d.|.j...
+00000d50: 6402 7c01 9b00 6403 9d05 7c02 7c03 6602  d.|...d...|.|.f.
+00000d60: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00000d70: 5700 6404 5300 3100 734c 3000 0100 0100  W.d.S.1.sL0.....
+00000d80: 0100 5900 0100 5700 6e2e 0400 7404 6a05  ..Y...W.n...t.j.
+00000d90: 7986 0100 7d05 0100 7a14 6405 7c05 6602  y...}...z.d.|.f.
+00000da0: 5700 0600 5900 6400 7d05 7e05 5300 6400  W...Y.d.}.~.S.d.
+00000db0: 7d05 7e05 3000 3000 6e7c 7a4a 7c00 6a00  }.~.0.0.n|zJ|.j.
+00000dc0: 8f30 0100 7c00 6a01 a002 6401 7c04 9b00  .0..|.j...d.|...
+00000dd0: 6406 9d03 7c01 7c02 7c03 6603 a102 0100  d...|.|.|.f.....
+00000de0: 5700 6400 0400 0400 8303 0100 5700 6407  W.d.........W.d.
+00000df0: 5300 3100 73c8 3000 0100 0100 0100 5900  S.1.s.0.......Y.
+00000e00: 0100 5700 6e30 0400 7404 6a05 9001 7904  ..W.n0..t.j...y.
+00000e10: 0100 7d05 0100 7a14 6408 7c05 6602 5700  ..}...z.d.|.f.W.
+00000e20: 0600 5900 6400 7d05 7e05 5300 6400 7d05  ..Y.d.}.~.S.d.}.
+00000e30: 7e05 3000 3000 6400 5300 2909 4e7a 0755  ~.0.0.d.S.).Nz.U
+00000e40: 5044 4154 4520 7a05 2053 4554 207a 1220  PDATE z. SET z. 
+00000e50: 3d20 3f20 5748 4552 4520 4944 203d 203f  = ? WHERE ID = ?
+00000e60: 2072 3200 0000 7224 0000 007a 1820 5345   r2...r$...z. SE
+00000e70: 5420 3f20 3d20 3f20 5748 4552 4520 4944  T ? = ? WHERE ID
+00000e80: 203d 203f 2072 2500 0000 7201 0000 0072   = ? r%...r....r
+00000e90: 3300 0000 2906 7211 0000 0072 3b00 0000  3...).r....r;...
+00000ea0: 723c 0000 0072 3d00 0000 7239 0000 0072  r<...r=...r9...r
+00000eb0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00000ec0: 0000 00da 0675 7064 6174 6567 0000 0073  .....updateg...s
+00000ed0: 2200 0000 0001 0801 0201 0801 1801 06ff  "...............
+00000ee0: 0402 2602 1001 2003 0201 0801 1001 08ff  ..&... .........
+00000ef0: 0402 2602 1201 7a0f 4461 7461 6261 7365  ..&...z.Database
+00000f00: 2e75 7064 6174 6563 0200 0000 0000 0000  .updatec........
+00000f10: 0000 0000 0400 0000 0a00 0000 6300 0000  ............c...
+00000f20: 731a 0100 007c 0164 0075 0072 907a 567c  s....|.d.u.r.zV|
+00000f30: 006a 008f 3c01 007c 006a 01a0 0264 017c  .j..<..|.j...d.|
+00000f40: 006a 039b 0064 029d 03a1 0101 007c 006a  .j...d.......|.j
+00000f50: 01a0 04a1 0044 005d 0a7d 027c 0256 0001  .....D.].}.|.V..
+00000f60: 0071 3257 0064 0004 0004 0083 0301 006e  .q2W.d.........n
+00000f70: 1031 0073 5230 0001 0001 0001 0059 0001  .1.sR0.......Y..
+00000f80: 0057 006e 2e04 0074 056a 0679 8c01 007d  .W.n...t.j.y...}
+00000f90: 0301 007a 1464 037c 0366 0257 0006 0059  ...z.d.|.f.W...Y
+00000fa0: 0064 007d 037e 0353 0064 007d 037e 0330  .d.}.~.S.d.}.~.0
+00000fb0: 0030 006e 867a 547c 006a 008f 3a01 007c  .0.n.zT|.j..:..|
+00000fc0: 006a 01a0 0264 017c 019b 0064 029d 03a1  .j...d.|...d....
+00000fd0: 0101 007c 006a 01a0 04a1 0044 005d 0a7d  ...|.j.....D.].}
+00000fe0: 027c 0256 0001 0071 b857 0064 0004 0004  .|.V...q.W.d....
+00000ff0: 0083 0301 006e 1031 0073 d830 0001 0001  .....n.1.s.0....
+00001000: 0001 0059 0001 0057 006e 3004 0074 056a  ...Y...W.n0..t.j
+00001010: 0690 0179 1401 007d 0301 007a 1464 047c  ...y...}...z.d.|
+00001020: 0366 0257 0006 0059 0064 007d 037e 0353  .f.W...Y.d.}.~.S
+00001030: 0064 007d 037e 0330 0030 0064 0053 00a9  .d.}.~.0.0.d.S..
+00001040: 054e fa0e 5345 4c45 4354 202a 2046 524f  .N..SELECT * FRO
+00001050: 4d20 fa01 2072 2400 0000 7201 0000 00a9  M .. r$...r.....
+00001060: 0772 0c00 0000 720d 0000 0072 1500 0000  .r....r....r....
+00001070: 7209 0000 0072 2d00 0000 720e 0000 0072  r....r-...r....r
+00001080: 1700 0000 2904 7211 0000 0072 3400 0000  ....).r....r4...
+00001090: da03 726f 7772 1900 0000 7212 0000 0072  ..rowr....r....r
+000010a0: 1200 0000 7213 0000 0072 3700 0000 7c00  ....r....r7...|.
+000010b0: 0000 731e 0000 0000 0108 0102 0108 0116  ..s.............
+000010c0: 010e 012a 0210 0120 0302 0108 0114 010e  ...*... ........
+000010d0: 012a 0212 017a 1044 6174 6162 6173 652e  .*...z.Database.
+000010e0: 636f 6e74 656e 7429 01da 0269 6463 0300  content)...idc..
+000010f0: 0000 0000 0000 0000 0000 0500 0000 0a00  ................
+00001100: 0000 6300 0000 7322 0100 007c 0264 0075  ..c...s"...|.d.u
+00001110: 0072 947a 5a7c 006a 008f 4001 007c 006a  .r.zZ|.j..@..|.j
+00001120: 01a0 0264 017c 006a 039b 0064 029d 037c  ...d.|.j...d...|
+00001130: 0166 01a1 0201 007c 006a 01a0 04a1 0044  .f.....|.j.....D
+00001140: 005d 0a7d 037c 0356 0001 0071 3657 0064  .].}.|.V...q6W.d
+00001150: 0004 0004 0083 0301 006e 1031 0073 5630  .........n.1.sV0
+00001160: 0001 0001 0001 0059 0001 0057 006e 2e04  .......Y...W.n..
+00001170: 0074 056a 0679 9001 007d 0401 007a 1464  .t.j.y...}...z.d
+00001180: 037c 0466 0257 0006 0059 0064 007d 047e  .|.f.W...Y.d.}.~
+00001190: 0453 0064 007d 047e 0430 0030 006e 8a7a  .S.d.}.~.0.0.n.z
+000011a0: 587c 006a 008f 3e01 007c 006a 01a0 0264  X|.j..>..|.j...d
+000011b0: 017c 029b 0064 029d 037c 0166 01a1 0201  .|...d...|.f....
+000011c0: 007c 006a 01a0 04a1 0044 005d 0a7d 037c  .|.j.....D.].}.|
+000011d0: 0356 0001 0071 c057 0064 0004 0004 0083  .V...q.W.d......
+000011e0: 0301 006e 1031 0073 e030 0001 0001 0001  ...n.1.s.0......
+000011f0: 0059 0001 0057 006e 3004 0074 056a 0690  .Y...W.n0..t.j..
+00001200: 0179 1c01 007d 0401 007a 1464 047c 0466  .y...}...z.d.|.f
+00001210: 0257 0006 0059 0064 007d 047e 0453 0064  .W...Y.d.}.~.S.d
+00001220: 007d 047e 0430 0030 0064 0053 0029 054e  .}.~.0.0.d.S.).N
+00001230: 7240 0000 007a 0e20 5748 4552 4520 4944  r@...z. WHERE ID
+00001240: 203d 203f 2072 2400 0000 7201 0000 0072   = ? r$...r....r
+00001250: 4200 0000 2905 7211 0000 0072 4400 0000  B...).r....rD...
+00001260: 7234 0000 0072 4300 0000 7219 0000 0072  r4...rC...r....r
+00001270: 1200 0000 7212 0000 0072 1300 0000 da0d  ....r....r......
+00001280: 636f 6e74 656e 745f 6279 5f69 6491 0000  content_by_id...
+00001290: 0073 1e00 0000 0001 0801 0201 0801 1a01  .s..............
+000012a0: 0e01 2a02 1001 2003 0201 0801 1801 0e01  ..*... .........
+000012b0: 2a02 1201 7a16 4461 7461 6261 7365 2e63  *...z.Database.c
+000012c0: 6f6e 7465 6e74 5f62 795f 6964 6301 0000  ontent_by_idc...
+000012d0: 0000 0000 0000 0000 0005 0000 000a 0000  ................
+000012e0: 0067 0000 0073 2a01 0000 7c01 7298 7a62  .g...s*...|.r.zb
+000012f0: 7c01 4400 5d58 7d02 7c00 6a00 8f3e 0100  |.D.]X}.|.j..>..
+00001300: 7c00 6a01 a002 6401 7c02 9b00 6402 9d03  |.j...d.|...d...
+00001310: a101 0100 7c00 6a01 a003 a100 4400 5d0e  ....|.j.....D.].
+00001320: 7d03 7c02 7c03 6901 5600 0100 7134 5700  }.|.|.i.V...q4W.
+00001330: 6400 0400 0400 8303 0100 710a 3100 7358  d.........q.1.sX
+00001340: 3000 0100 0100 0100 5900 0100 710a 5700  0.......Y...q.W.
+00001350: 6e2e 0400 7404 6a05 7994 0100 7d04 0100  n...t.j.y...}...
+00001360: 7a14 6403 7c04 6602 5700 0600 5900 6400  z.d.|.f.W...Y.d.
+00001370: 7d04 7e04 5300 6400 7d04 7e04 3000 3000  }.~.S.d.}.~.0.0.
+00001380: 6e8e 7a5c 7c00 6a00 8f42 0100 7c00 6a01  n.z\|.j..B..|.j.
+00001390: a002 6401 7c00 6a06 9b00 6402 9d03 a101  ..d.|.j...d.....
+000013a0: 0100 7c00 6a01 a003 a100 4400 5d10 7d03  ..|.j.....D.].}.
+000013b0: 7c00 6a06 7c03 6901 5600 0100 71c2 5700  |.j.|.i.V...q.W.
+000013c0: 6400 0400 0400 8303 0100 6e10 3100 73e8  d.........n.1.s.
+000013d0: 3000 0100 0100 0100 5900 0100 5700 6e30  0.......Y...W.n0
+000013e0: 0400 7404 6a05 9001 7924 0100 7d04 0100  ..t.j...y$..}...
+000013f0: 7a14 6404 7c04 6602 5700 0600 5900 6400  z.d.|.f.W...Y.d.
+00001400: 7d04 7e04 5300 6400 7d04 7e04 3000 3000  }.~.S.d.}.~.0.0.
+00001410: 6400 5300 723f 0000 0029 0772 0c00 0000  d.S.r?...).r....
+00001420: 720d 0000 0072 1500 0000 722d 0000 0072  r....r....r-...r
+00001430: 0e00 0000 7217 0000 0072 0900 0000 2905  ....r....r....).
+00001440: 7211 0000 005a 136f 7074 696f 6e61 6c5f  r....Z.optional_
+00001450: 7461 626c 656e 616d 6573 da03 6172 6772  tablenames..argr
+00001460: 4300 0000 7219 0000 0072 1200 0000 7212  C...r....r....r.
+00001470: 0000 0072 1300 0000 da0d 7368 6f77 5f63  ...r......show_c
+00001480: 6f6e 7465 6e74 73a6 0000 0073 2000 0000  ontents....s ...
+00001490: 0001 0401 0201 0801 0801 1401 0e01 3002  ..............0.
+000014a0: 1001 2003 0201 0801 1601 0e01 3002 1201  .. .........0...
+000014b0: 7a16 4461 7461 6261 7365 2e73 686f 775f  z.Database.show_
+000014c0: 636f 6e74 656e 7473 6301 0000 0000 0000  contentsc.......
+000014d0: 0000 0000 0003 0000 000a 0000 0063 0000  .............c..
+000014e0: 0073 8000 0000 7a4c 7c00 6a00 8f32 0100  .s....zL|.j..2..
+000014f0: 7c00 6a01 a002 6401 a101 0100 7c00 6a01  |.j...d.....|.j.
+00001500: a003 a100 4400 5d0a 7d01 7c01 5600 0100  ....D.].}.|.V...
+00001510: 7120 5700 6400 0400 0400 8303 0100 6e10  q W.d.........n.
+00001520: 3100 7340 3000 0100 0100 0100 5900 0100  1.s@0.......Y...
+00001530: 5700 6e2e 0400 7404 6a05 797a 0100 7d02  W.n...t.j.yz..}.
+00001540: 0100 7a14 6402 7c02 6602 5700 0600 5900  ..z.d.|.f.W...Y.
+00001550: 6400 7d02 7e02 5300 6400 7d02 7e02 3000  d.}.~.S.d.}.~.0.
+00001560: 3000 6400 5300 2903 4efa 3353 454c 4543  0.d.S.).N.3SELEC
+00001570: 5420 6e61 6d65 2046 524f 4d20 7371 6c69  T name FROM sqli
+00001580: 7465 5f6d 6173 7465 7220 5748 4552 4520  te_master WHERE 
+00001590: 7479 7065 3d20 2774 6162 6c65 2720 7201  type= 'table' r.
+000015a0: 0000 00a9 0672 0c00 0000 720d 0000 0072  .....r....r....r
+000015b0: 1500 0000 722d 0000 0072 0e00 0000 7217  ....r-...r....r.
+000015c0: 0000 0029 0372 1100 0000 7243 0000 0072  ...).r....rC...r
+000015d0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+000015e0: 0000 00da 0b73 686f 775f 7461 626c 6573  .....show_tables
+000015f0: bc00 0000 730e 0000 0000 0102 0108 010c  ....s...........
+00001600: 010e 012a 0210 017a 1444 6174 6162 6173  ...*...z.Databas
+00001610: 652e 7368 6f77 5f74 6162 6c65 7363 0100  e.show_tablesc..
+00001620: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+00001630: 0000 4300 0000 7394 0000 007a 607c 006a  ..C...s....z`|.j
+00001640: 008f 4601 007c 006a 01a0 0264 01a1 0101  ..F..|.j...d....
+00001650: 007c 006a 01a0 03a1 0044 005d 1a7d 017c  .|.j.....D.].}.|
+00001660: 006a 01a0 0264 027c 0164 0319 009b 009d  .j...d.|.d......
+00001670: 02a1 0101 0071 2057 0064 0004 0004 0083  .....q W.d......
+00001680: 0301 0057 0064 0453 0031 0073 5430 0001  ...W.d.S.1.sT0..
+00001690: 0001 0001 0059 0001 0057 006e 2e04 0074  .....Y...W.n...t
+000016a0: 046a 0579 8e01 007d 0201 007a 1464 037c  .j.y...}...z.d.|
+000016b0: 0266 0257 0006 0059 0064 007d 027e 0253  .f.W...Y.d.}.~.S
+000016c0: 0064 007d 027e 0230 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+000016d0: 054e 7248 0000 00fa 0b44 524f 5020 5441  .NrH.....DROP TA
+000016e0: 424c 4520 7201 0000 0072 2500 0000 7249  BLE r....r%...rI
+000016f0: 0000 0029 0372 1100 0000 da05 7461 626c  ...).r......tabl
+00001700: 6572 1900 0000 7212 0000 0072 1200 0000  er....r....r....
+00001710: 7213 0000 00da 0764 726f 7061 6c6c c600  r......dropall..
+00001720: 0000 7310 0000 0000 0102 0108 010c 010e  ..s.............
+00001730: 0118 0126 0210 017a 1044 6174 6162 6173  ...&...z.Databas
+00001740: 652e 6472 6f70 616c 6c63 0100 0000 0000  e.dropallc......
+00001750: 0000 0000 0000 0400 0000 0a00 0000 4700  ..............G.
+00001760: 0000 73f6 0000 007c 0172 7e7a 487c 0144  ..s....|.r~zH|.D
+00001770: 005d 3c7d 027c 006a 008f 2201 007c 006a  .]<}.|.j.."..|.j
+00001780: 01a0 0264 017c 029b 009d 02a1 0101 0057  ...d.|.........W
+00001790: 0064 0004 0004 0083 0301 0071 0a31 0073  .d.........q.1.s
+000017a0: 3c30 0001 0001 0001 0059 0001 0071 0a57  <0.......Y...q.W
+000017b0: 0064 0253 0004 0074 036a 0479 7a01 007d  .d.S...t.j.yz..}
+000017c0: 0301 007a 1464 037c 0366 0257 0006 0059  ...z.d.|.f.W...Y
+000017d0: 0064 007d 037e 0353 0064 007d 037e 0330  .d.}.~.S.d.}.~.0
+000017e0: 0030 006e 747a 427c 006a 008f 2801 007c  .0.ntzB|.j..(..|
+000017f0: 006a 01a0 0264 017c 006a 059b 009d 02a1  .j...d.|.j......
+00001800: 0101 0057 0064 0004 0004 0083 0301 0057  ...W.d.........W
+00001810: 0064 0253 0031 0073 b430 0001 0001 0001  .d.S.1.s.0......
+00001820: 0059 0001 0057 006e 3004 0074 036a 0490  .Y...W.n0..t.j..
+00001830: 0079 f001 007d 0301 007a 1464 047c 0366  .y...}...z.d.|.f
+00001840: 0257 0006 0059 0064 007d 037e 0353 0064  .W...Y.d.}.~.S.d
+00001850: 007d 037e 0330 0030 0064 0053 0029 054e  .}.~.0.0.d.S.).N
+00001860: 724b 0000 0072 2500 0000 7224 0000 0072  rK...r%...r$...r
+00001870: 0100 0000 2906 720c 0000 0072 0d00 0000  ....).r....r....
+00001880: 7215 0000 0072 0e00 0000 7217 0000 0072  r....r....r....r
+00001890: 0900 0000 2904 7211 0000 005a 0b74 6162  ....).r....Z.tab
+000018a0: 6c65 5f6e 616d 6573 7246 0000 0072 1900  le_namesrF...r..
+000018b0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000018c0: 00da 0a64 726f 705f 7461 626c 65d1 0000  ...drop_table...
+000018d0: 0073 1c00 0000 0001 0401 0201 0801 0801  .s..............
+000018e0: 3201 0601 1001 2003 0201 0801 1401 2602  2..... .......&.
+000018f0: 1201 7a13 4461 7461 6261 7365 2e64 726f  ..z.Database.dro
+00001900: 705f 7461 626c 6563 0300 0000 0000 0000  p_tablec........
+00001910: 0000 0000 0400 0000 0a00 0000 4300 0000  ............C...
+00001920: 73fa 0000 007c 0264 0075 0072 807a 467c  s....|.d.u.r.zF|
+00001930: 006a 008f 2a01 007c 006a 01a0 0264 017c  .j..*..|.j...d.|
+00001940: 006a 039b 0064 027c 019b 009d 04a1 0101  .j...d.|........
+00001950: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00001960: 0073 4030 0001 0001 0001 0059 0001 0057  .s@0.......Y...W
+00001970: 0064 0353 0004 0074 046a 0579 7c01 007d  .d.S...t.j.y|..}
+00001980: 0301 007a 1464 047c 0366 0257 0006 0059  ...z.d.|.f.W...Y
+00001990: 0064 007d 037e 0353 0064 007d 037e 0330  .d.}.~.S.d.}.~.0
+000019a0: 0030 006e 767a 447c 006a 008f 2801 007c  .0.nvzD|.j..(..|
+000019b0: 006a 01a0 0264 017c 029b 0064 027c 019b  .j...d.|...d.|..
+000019c0: 009d 04a1 0101 0057 0064 0004 0004 0083  .......W.d......
+000019d0: 0301 006e 1031 0073 b630 0001 0001 0001  ...n.1.s.0......
+000019e0: 0059 0001 0057 0064 0553 0004 0074 046a  .Y...W.d.S...t.j
+000019f0: 0590 0079 f401 007d 0301 007a 1464 067c  ...y...}...z.d.|
+00001a00: 0366 0257 0006 0059 0064 007d 037e 0353  .f.W...Y.d.}.~.S
+00001a10: 0064 007d 037e 0330 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+00001a20: 074e 7a0c 4445 4c45 5445 2046 524f 4d20  .Nz.DELETE FROM 
+00001a30: 7a0c 2057 4845 5245 2049 4420 3d20 7232  z. WHERE ID = r2
+00001a40: 0000 0072 2400 0000 7225 0000 0072 0100  ...r$...r%...r..
+00001a50: 0000 7233 0000 0029 0472 1100 0000 723d  ..r3...).r....r=
+00001a60: 0000 0072 3900 0000 7219 0000 0072 1200  ...r9...r....r..
+00001a70: 0000 7212 0000 0072 1300 0000 da0c 6472  ..r....r......dr
+00001a80: 6f70 5f63 6f6e 7465 6e74 e400 0000 731a  op_content....s.
+00001a90: 0000 0000 0108 0102 0108 0138 0106 0210  ...........8....
+00001aa0: 0120 0302 0108 0136 0106 0212 017a 1544  . .....6.....z.D
+00001ab0: 6174 6162 6173 652e 6472 6f70 5f63 6f6e  atabase.drop_con
+00001ac0: 7465 6e74 2901 4e29 014e 2901 4e29 014e  tent).N).N).N).N
+00001ad0: 2901 4e29 014e 2922 da08 5f5f 6e61 6d65  ).N).N)"..__name
+00001ae0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00001af0: 5f5f 7175 616c 6e61 6d65 5f5f 7203 0000  __qualname__r...
+00001b00: 0072 0700 0000 722a 0000 00da 0f5f 5f61  .r....r*.....__a
+00001b10: 6e6e 6f74 6174 696f 6e73 5f5f 7209 0000  nnotations__r...
+00001b20: 0072 0c00 0000 720e 0000 005a 0a43 6f6e  .r....r....Z.Con
+00001b30: 6e65 6374 696f 6e72 0d00 0000 5a06 4375  nectionr....Z.Cu
+00001b40: 7273 6f72 7214 0000 00da 0870 726f 7065  rsorr......prope
+00001b50: 7274 7972 1800 0000 7205 0000 0072 0400  rtyr....r....r..
+00001b60: 0000 da05 7475 706c 6572 2000 0000 7222  ....tupler ...r"
+00001b70: 0000 00da 046c 6973 7472 3100 0000 7235  .....listr1...r5
+00001b80: 0000 0072 3a00 0000 da03 696e 7472 3e00  ...r:.....intr>.
+00001b90: 0000 7237 0000 0072 4500 0000 7247 0000  ..r7...rE...rG..
+00001ba0: 0072 4a00 0000 724d 0000 0072 4e00 0000  .rJ...rM...rN...
+00001bb0: 724f 0000 0072 1200 0000 7212 0000 0072  rO...r....r....r
+00001bc0: 1200 0000 7213 0000 0072 0600 0000 0700  ....r....r......
+00001bd0: 0000 732c 0000 000a 020e 0112 0116 0116  ..s,............
+00001be0: 0208 0402 010a 0a02 0118 0802 010a 0310  ................
+00001bf0: 110a 180a 1414 150a 1510 1508 160e 0a08  ................
+00001c00: 0b08 1372 0600 0000 2909 5a0b 6461 7461  ...r....).Z.data
+00001c10: 636c 6173 7365 7372 0200 0000 7203 0000  classesr....r...
+00001c20: 0072 0400 0000 da06 7479 7069 6e67 7205  .r......typingr.
+00001c30: 0000 0072 0e00 0000 721c 0000 0072 0600  ...r....r....r..
+00001c40: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00001c50: 0072 1300 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001c60: 0100 0000 730c 0000 0010 010c 010c 0108  ....s...........
+00001c70: 0108 0202 01                             .....
```

### Comparing `AshCrypt-1.2.3/AshCrypt/__pycache__/AshTextCrypt.cpython-39.pyc` & `AshCrypt-1.2.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jun 30 15:01:03 2023 UTC, .py size: 2074 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,165 +1,151 @@
-00000000: 610d 0d0a 0000 0000 2fee 9e64 1a08 0000  a......./..d....
+00000000: 610d 0d0a 0000 0000 de90 9f64 3c07 0000  a..........d<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
+00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 8303 5a05 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
-00000060: 8302 5a06 6507 6407 6b02 725c 6408 5a08  ..Z.e.d.k.r\d.Z.
-00000070: 6506 6409 6508 8302 5a09 650a 6509 a00b  e.d.e...Z.e.e...
-00000080: a100 640a 1900 8301 0100 640b 5300 290c  ..d.......d.S.).
-00000090: e900 0000 0029 01da 0555 6e69 6f6e 2901  .....)...Union).
-000000a0: da03 4173 6863 0000 0000 0000 0000 0000  ..Ashc..........
-000000b0: 0000 0000 0000 0300 0000 0000 0000 731c  ..............s.
-000000c0: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
-000000d0: 0164 0284 085a 0387 0004 005a 0453 0029  .d...Z.....Z.S.)
-000000e0: 03da 084b 6579 4572 726f 7263 0100 0000  ...KeyErrorc....
-000000f0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000100: 0300 0000 7318 0000 0064 017c 005f 0074  ....s....d.|._.t
-00000110: 0183 00a0 027c 006a 00a1 0101 0064 0053  .....|.j.....d.S
-00000120: 0029 024e 7a1a 4b65 7920 6d75 7374 2062  .).Nz.Key must b
-00000130: 6520 3531 3220 4269 7420 6c6f 6e67 2021  e 512 Bit long !
-00000140: 2903 5a07 6469 7370 6c61 79da 0573 7570  ).Z.display..sup
-00000150: 6572 da08 5f5f 696e 6974 5f5f a901 da04  er..__init__....
-00000160: 7365 6c66 a901 da09 5f5f 636c 6173 735f  self....__class_
-00000170: 5fa9 00fa 3343 3a5c 576f 726b 5c47 6974  _...3C:\Work\Git
-00000180: 4875 6257 6f72 6b5c 4145 532d 3235 365c  HubWork\AES-256\
-00000190: 4173 6843 7279 7074 5c41 7368 5465 7874  AshCrypt\AshText
-000001a0: 4372 7970 742e 7079 7206 0000 0006 0000  Crypt.pyr.......
-000001b0: 0073 0400 0000 0001 0601 7a11 4b65 7945  .s........z.KeyE
-000001c0: 7272 6f72 2e5f 5f69 6e69 745f 5f29 05da  rror.__init__)..
-000001d0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000001e0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000001f0: 655f 5f72 0600 0000 da0d 5f5f 636c 6173  e__r......__clas
-00000200: 7363 656c 6c5f 5f72 0b00 0000 720b 0000  scell__r....r...
-00000210: 0072 0900 0000 720c 0000 0072 0400 0000  .r....r....r....
-00000220: 0500 0000 7302 0000 0008 0172 0400 0000  ....s......r....
-00000230: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000240: 0004 0000 0040 0000 0073 7600 0000 6500  .....@...sv...e.
-00000250: 5a01 6400 5a02 6503 6504 6505 6602 1900  Z.d.Z.e.e.e.f...
-00000260: 6504 6401 9c02 6402 6403 8404 5a06 6507  e.d...d.d...Z.e.
-00000270: 6504 6404 9c01 6405 6406 8404 8301 5a08  e.d...d.d.....Z.
-00000280: 6507 6504 6509 6407 9c02 6408 6409 8404  e.e.e.d...d.d...
-00000290: 8301 5a0a 650b 6404 9c01 640a 640b 8404  ..Z.e.d...d.d...
-000002a0: 5a0c 650b 6404 9c01 640c 640d 8404 5a0d  Z.e.d...d.d...Z.
-000002b0: 640e 640f 8400 5a0e 6410 6411 8400 5a0f  d.d...Z.d.d...Z.
-000002c0: 6412 5300 2913 da05 4372 7970 74a9 02da  d.S.)...Crypt...
-000002d0: 0474 6578 74da 036b 6579 6303 0000 0000  .text..keyc.....
-000002e0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-000002f0: 0000 0073 2600 0000 7c01 7c00 5f00 7c00  ...s&...|.|._.|.
-00000300: a001 7c02 a101 6401 6b02 721c 7c02 7c00  ..|...d.k.r.|.|.
-00000310: 5f02 6e06 7403 8300 8201 6400 5300 2902  _.n.t.....d.S.).
-00000320: 4ee9 0100 0000 2904 7213 0000 00da 096b  N.....).r......k
-00000330: 6579 7665 7269 6679 7214 0000 0072 0400  eyverifyr....r..
-00000340: 0000 2903 7208 0000 0072 1300 0000 7214  ..).r....r....r.
-00000350: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000360: 0000 7206 0000 000b 0000 0073 0800 0000  ..r........s....
-00000370: 0001 0601 0e01 0802 7a0e 4372 7970 742e  ........z.Crypt.
-00000380: 5f5f 696e 6974 5f5f 2901 da06 7265 7475  __init__)...retu
-00000390: 726e 6300 0000 0000 0000 0000 0000 0000  rnc.............
-000003a0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-000003b0: 7400 6a01 a002 a100 5300 2901 4e29 0372  t.j.....S.).N).r
-000003c0: 0300 0000 da03 456e 635a 0a67 656e 4d61  ......EncZ.genMa
-000003d0: 696e 6b65 7972 0b00 0000 720b 0000 0072  inkeyr....r....r
-000003e0: 0b00 0000 720c 0000 00da 0667 656e 6b65  ....r......genke
-000003f0: 7912 0000 0073 0200 0000 0002 7a0c 4372  y....s......z.Cr
-00000400: 7970 742e 6765 6e6b 6579 2902 7214 0000  ypt.genkey).r...
-00000410: 0072 1700 0000 6301 0000 0000 0000 0000  .r....c.........
-00000420: 0000 0002 0000 0008 0000 0043 0000 0073  ...........C...s
-00000430: 4e00 0000 7400 7c00 7401 8302 7246 7a24  N...t.|.t...rFz$
-00000440: 7402 a003 7c00 a004 a100 a101 7d01 7405  t...|.......}.t.
-00000450: 7c01 8301 6401 6b02 722c 5700 6402 5300  |...d.k.r,W.d.S.
-00000460: 5700 714a 0400 7406 7942 0100 0100 0100  W.qJ..t.yB......
-00000470: 5900 6403 5300 3000 6e04 6404 5300 6400  Y.d.S.0.n.d.S.d.
-00000480: 5300 2905 4ee9 4000 0000 7215 0000 0072  S.).N.@...r....r
-00000490: 0100 0000 e902 0000 0029 07da 0a69 7369  .........)...isi
-000004a0: 6e73 7461 6e63 65da 0373 7472 da05 6279  nstance..str..by
-000004b0: 7465 73da 0766 726f 6d68 6578 da05 7374  tes..fromhex..st
-000004c0: 7269 70da 036c 656e da09 4578 6365 7074  rip..len..Except
-000004d0: 696f 6e29 0272 1400 0000 da01 6172 0b00  ion).r......ar..
-000004e0: 0000 720b 0000 0072 0c00 0000 7216 0000  ..r....r....r...
-000004f0: 0016 0000 0073 1000 0000 0002 0a01 0201  .....s..........
-00000500: 0e01 0c01 0a01 0c01 0a03 7a0f 4372 7970  ..........z.Cryp
-00000510: 742e 6b65 7976 6572 6966 7963 0100 0000  t.keyverifyc....
-00000520: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00000530: 4300 0000 734c 0000 007c 006a 0072 447a  C...sL...|.j.rDz
-00000540: 2274 01a0 027c 006a 007c 006a 03a1 027d  "t...|.j.|.j...}
-00000550: 017c 01a0 04a1 007d 0264 017c 0266 0257  .|.....}.d.|.f.W
-00000560: 0053 0001 0001 0001 0064 027d 0364 037c  .S.......d.}.d.|
-00000570: 0366 0206 0059 0053 0030 006e 0464 0453  .f...Y.S.0.n.d.S
-00000580: 0064 0053 0029 054e 7215 0000 00da 0145  .d.S.).Nr......E
-00000590: 7201 0000 00a9 02e7 0000 0000 0000 0000  r...............
-000005a0: 7226 0000 0029 0572 1300 0000 7203 0000  r&...).r....r...
-000005b0: 0072 1800 0000 7214 0000 005a 0865 6e63  .r....r....Z.enc
-000005c0: 546f 5374 7229 0472 0800 0000 5a03 696e  ToStr).r....Z.in
-000005d0: 735a 0b6e 6577 5f63 6f6e 7465 6e74 da06  sZ.new_content..
-000005e0: 6f75 7470 7574 720b 0000 0072 0b00 0000  outputr....r....
-000005f0: 720c 0000 00da 0765 6e63 7279 7074 2300  r......encrypt#.
-00000600: 0000 7312 0000 0000 0106 0102 0110 0108  ..s.............
-00000610: 010a 0106 0104 0110 027a 0d43 7279 7074  .........z.Crypt
-00000620: 2e65 6e63 7279 7074 6301 0000 0000 0000  .encryptc.......
-00000630: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
-00000640: 0073 5a00 0000 7c00 6a00 7252 7a28 7401  .sZ...|.j.rRz(t.
-00000650: 6a02 7c00 6a00 7c00 6a03 6401 8d02 7d01  j.|.j.|.j.d...}.
-00000660: 7c01 a004 a100 7d02 7c02 7d03 6402 7c03  |.....}.|.}.d.|.
-00000670: 6602 5700 5300 0400 7405 794e 0100 0100  f.W.S...t.yN....
-00000680: 0100 7c00 6a00 7d03 6403 7c03 6602 0600  ..|.j.}.d.|.f...
-00000690: 5900 5300 3000 6e04 6404 5300 6400 5300  Y.S.0.n.d.S.d.S.
-000006a0: 2905 4e29 02da 076d 6573 7361 6765 da07  ).N)...message..
-000006b0: 6d61 696e 6b65 7972 1500 0000 7201 0000  mainkeyr....r...
-000006c0: 0072 2500 0000 2906 7213 0000 0072 0300  .r%...).r....r..
-000006d0: 0000 5a03 4465 6372 1400 0000 5a08 6465  ..Z.Decr....Z.de
-000006e0: 6354 6f53 7472 7222 0000 0029 0472 0800  cToStrr"...).r..
-000006f0: 0000 5a0c 6465 635f 696e 7374 616e 6365  ..Z.dec_instance
-00000700: 7223 0000 0072 2700 0000 720b 0000 0072  r#...r'...r....r
-00000710: 0b00 0000 720c 0000 00da 0764 6563 7279  ....r......decry
-00000720: 7074 2f00 0000 7314 0000 0000 0106 0102  pt/...s.........
-00000730: 0112 0108 0104 010a 010c 0106 0110 027a  ...............z
-00000740: 0d43 7279 7074 2e64 6563 7279 7074 6301  .Crypt.decryptc.
-00000750: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-00000760: 0000 0043 0000 0073 1e00 0000 6401 7c00  ...C...s....d.|.
-00000770: 6a00 6400 6402 8502 1900 9b00 6403 7c00  j.d.d.......d.|.
-00000780: 6a01 9b00 6404 9d05 5300 2905 4e7a 1b45  j...d...S.).Nz.E
-00000790: 6e63 7279 7074 696e 672f 4465 6372 7970  ncrypting/Decryp
-000007a0: 7469 6e67 2054 6578 7420 e908 0000 007a  ting Text .....z
-000007b0: 082e 2e20 5769 7468 207a 0520 4b65 7920  ... With z. Key 
-000007c0: 7212 0000 0072 0700 0000 720b 0000 0072  r....r....r....r
-000007d0: 0b00 0000 720c 0000 00da 075f 5f73 7472  ....r......__str
-000007e0: 5f5f 3c00 0000 7302 0000 0000 017a 0d43  __<...s......z.C
-000007f0: 7279 7074 2e5f 5f73 7472 5f5f 6301 0000  rypt.__str__c...
-00000800: 0000 0000 0000 0000 0001 0000 0006 0000  ................
-00000810: 0043 0000 0073 2600 0000 7c00 6a00 6a01  .C...s&...|.j.j.
-00000820: 9b00 6401 7c00 6a02 6400 6402 8502 1900  ..d.|.j.d.d.....
-00000830: 9b00 6403 7c00 6a03 9b00 6404 9d06 5300  ..d.|.j...d...S.
-00000840: 2905 4efa 0128 722c 0000 00fa 012c fa01  ).N..(r,.....,..
-00000850: 2929 0472 0a00 0000 720d 0000 0072 1300  )).r....r....r..
-00000860: 0000 7214 0000 0072 0700 0000 720b 0000  ..r....r....r...
-00000870: 0072 0b00 0000 720c 0000 00da 085f 5f72  .r....r......__r
-00000880: 6570 725f 5f3e 0000 0073 0200 0000 0001  epr__>...s......
-00000890: 7a0e 4372 7970 742e 5f5f 7265 7072 5f5f  z.Crypt.__repr__
-000008a0: 4e29 1072 0d00 0000 720e 0000 0072 0f00  N).r....r....r..
-000008b0: 0000 7202 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000008c0: 0072 0600 0000 da0c 7374 6174 6963 6d65  .r......staticme
-000008d0: 7468 6f64 7219 0000 00da 0369 6e74 7216  thodr......intr.
-000008e0: 0000 00da 0574 7570 6c65 7228 0000 0072  .....tupler(...r
-000008f0: 2b00 0000 722d 0000 0072 3100 0000 720b  +...r-...r1...r.
-00000900: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000910: 0000 7211 0000 000a 0000 0073 1200 0000  ..r........s....
-00000920: 0801 1807 0201 1003 0201 120c 0e0c 0e0d  ................
-00000930: 0802 7211 0000 00da 085f 5f6d 6169 6e5f  ..r......__main_
-00000940: 5f5a 8064 3564 3731 3766 3537 3933 3361  _Z.d5d717f57933a
-00000950: 6432 3137 3235 3838 3864 3334 3531 6139  d21725888d3451a9
-00000960: 6364 3761 3536 3564 6664 6136 3737 6665  cd7a565dfda677fe
-00000970: 3932 6664 3866 6639 6539 6333 6133 3664  92fd8ff9e9c3a36d
-00000980: 3134 3936 6166 3538 6331 3764 6532 6237  1496af58c17de2b7
-00000990: 3764 3464 3365 6136 6438 3739 3162 3237  7d4d3ea6d8791b27
-000009a0: 3335 3066 6561 3061 6633 6164 3236 3130  350fea0af3ad2610
-000009b0: 6433 3863 3863 6231 3261 3239 6664 6134  d38c8cb12a29fda4
-000009c0: 6263 6673 0500 0000 7465 7374 3172 1500  bcfs....test1r..
-000009d0: 0000 4e29 0c5a 0674 7970 696e 6772 0200  ..N).Z.typingr..
-000009e0: 0000 da08 4173 6843 7279 7074 7203 0000  ....AshCryptr...
-000009f0: 0072 2200 0000 7204 0000 0072 1100 0000  .r"...r....r....
-00000a00: 720d 0000 00da 016b 7223 0000 00da 0570  r......kr#.....p
-00000a10: 7269 6e74 7228 0000 0072 0b00 0000 720b  rintr(...r....r.
-00000a20: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
-00000a30: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-00000a40: 0c01 0c03 1005 0e37 0801 0401 0a01       .......7......
+00000060: 8302 5a06 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
+00000070: 01da 0555 6e69 6f6e 2901 da03 4173 6863  ...Union)...Ashc
+00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000090: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
+000000a0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+000000b0: 0387 0004 005a 0453 0029 03da 084b 6579  .....Z.S.)...Key
+000000c0: 4572 726f 7263 0100 0000 0000 0000 0000  Errorc..........
+000000d0: 0000 0100 0000 0300 0000 0300 0000 7318  ..............s.
+000000e0: 0000 0064 017c 005f 0074 0183 00a0 027c  ...d.|._.t.....|
+000000f0: 006a 00a1 0101 0064 0053 0029 024e 7a1a  .j.....d.S.).Nz.
+00000100: 4b65 7920 6d75 7374 2062 6520 3531 3220  Key must be 512 
+00000110: 4269 7420 6c6f 6e67 2021 2903 da07 6469  Bit long !)...di
+00000120: 7370 6c61 79da 0573 7570 6572 da08 5f5f  splay..super..__
+00000130: 696e 6974 5f5f a901 da04 7365 6c66 a901  init__....self..
+00000140: da09 5f5f 636c 6173 735f 5fa9 00fa 3043  ..__class__...0C
+00000150: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
+00000160: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
+00000170: 7074 5c54 6578 7443 7279 7074 2e70 7972  pt\TextCrypt.pyr
+00000180: 0700 0000 0600 0000 7304 0000 0000 0106  ........s.......
+00000190: 017a 114b 6579 4572 726f 722e 5f5f 696e  .z.KeyError.__in
+000001a0: 6974 5f5f 2905 da08 5f5f 6e61 6d65 5f5f  it__)...__name__
+000001b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000001c0: 7175 616c 6e61 6d65 5f5f 7207 0000 00da  qualname__r.....
+000001d0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720c  .__classcell__r.
+000001e0: 0000 0072 0c00 0000 720a 0000 0072 0d00  ...r....r....r..
+000001f0: 0000 7204 0000 0005 0000 0073 0200 0000  ..r........s....
+00000200: 0801 7204 0000 0063 0000 0000 0000 0000  ..r....c........
+00000210: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+00000220: 7376 0000 0065 005a 0164 005a 0265 0365  sv...e.Z.d.Z.e.e
+00000230: 0465 0566 0219 0065 0464 019c 0264 0264  .e.f...e.d...d.d
+00000240: 0384 045a 0665 0765 0464 049c 0164 0564  ...Z.e.e.d...d.d
+00000250: 0684 0483 015a 0865 0765 0465 0964 079c  .....Z.e.e.e.d..
+00000260: 0264 0864 0984 0483 015a 0a65 0b64 049c  .d.d.....Z.e.d..
+00000270: 0164 0a64 0b84 045a 0c65 0b64 049c 0164  .d.d...Z.e.d...d
+00000280: 0c64 0d84 045a 0d64 0e64 0f84 005a 0e64  .d...Z.d.d...Z.d
+00000290: 1064 1184 005a 0f64 1253 0029 13da 0543  .d...Z.d.S.)...C
+000002a0: 7279 7074 a902 da04 7465 7874 da03 6b65  rypt....text..ke
+000002b0: 7963 0300 0000 0000 0000 0000 0000 0300  yc..............
+000002c0: 0000 0300 0000 4300 0000 7326 0000 007c  ......C...s&...|
+000002d0: 017c 005f 007c 00a0 017c 02a1 0164 016b  .|._.|...|...d.k
+000002e0: 0272 1c7c 027c 005f 026e 0674 0383 0082  .r.|.|._.n.t....
+000002f0: 0164 0053 0029 024e e901 0000 0029 0472  .d.S.).N.....).r
+00000300: 1400 0000 da09 6b65 7976 6572 6966 7972  ......keyverifyr
+00000310: 1500 0000 7204 0000 0029 0372 0900 0000  ....r....).r....
+00000320: 7214 0000 0072 1500 0000 720c 0000 0072  r....r....r....r
+00000330: 0c00 0000 720d 0000 0072 0700 0000 0b00  ....r....r......
+00000340: 0000 7308 0000 0000 0106 010e 0108 027a  ..s............z
+00000350: 0e43 7279 7074 2e5f 5f69 6e69 745f 5f29  .Crypt.__init__)
+00000360: 01da 0672 6574 7572 6e63 0000 0000 0000  ...returnc......
+00000370: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00000380: 0000 730a 0000 0074 006a 01a0 02a1 0053  ..s....t.j.....S
+00000390: 0029 014e 2903 7203 0000 00da 0345 6e63  .).N).r......Enc
+000003a0: da0a 6765 6e4d 6169 6e6b 6579 720c 0000  ..genMainkeyr...
+000003b0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000003c0: da06 6765 6e6b 6579 1200 0000 7302 0000  ..genkey....s...
+000003d0: 0000 027a 0c43 7279 7074 2e67 656e 6b65  ...z.Crypt.genke
+000003e0: 7929 0272 1500 0000 7218 0000 0063 0100  y).r....r....c..
+000003f0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+00000400: 0000 4300 0000 734e 0000 0074 007c 0074  ..C...sN...t.|.t
+00000410: 0183 0272 467a 2474 02a0 037c 00a0 04a1  ...rFz$t...|....
+00000420: 00a1 017d 0174 057c 0183 0164 016b 0272  ...}.t.|...d.k.r
+00000430: 2c57 0064 0253 0057 0071 4a04 0074 0679  ,W.d.S.W.qJ..t.y
+00000440: 4201 0001 0001 0059 0064 0353 0030 006e  B......Y.d.S.0.n
+00000450: 0464 0453 0064 0053 0029 054e e940 0000  .d.S.d.S.).N.@..
+00000460: 0072 1600 0000 7201 0000 00e9 0200 0000  .r....r.........
+00000470: 2907 da0a 6973 696e 7374 616e 6365 da03  )...isinstance..
+00000480: 7374 72da 0562 7974 6573 da07 6672 6f6d  str..bytes..from
+00000490: 6865 78da 0573 7472 6970 da03 6c65 6eda  hex..strip..len.
+000004a0: 0945 7863 6570 7469 6f6e 2902 7215 0000  .Exception).r...
+000004b0: 00da 0161 720c 0000 0072 0c00 0000 720d  ...ar....r....r.
+000004c0: 0000 0072 1700 0000 1600 0000 7310 0000  ...r........s...
+000004d0: 0000 020a 0102 010e 010c 010a 010c 010a  ................
+000004e0: 037a 0f43 7279 7074 2e6b 6579 7665 7269  .z.Crypt.keyveri
+000004f0: 6679 6301 0000 0000 0000 0000 0000 0004  fyc.............
+00000500: 0000 0006 0000 0043 0000 0073 4c00 0000  .......C...sL...
+00000510: 7c00 6a00 7244 7a22 7401 a002 7c00 6a00  |.j.rDz"t...|.j.
+00000520: 7c00 6a03 a102 7d01 7c01 a004 a100 7d02  |.j...}.|.....}.
+00000530: 6401 7c02 6602 5700 5300 0100 0100 0100  d.|.f.W.S.......
+00000540: 6402 7d03 6403 7c03 6602 0600 5900 5300  d.}.d.|.f...Y.S.
+00000550: 3000 6e04 6404 5300 6400 5300 2905 4e72  0.n.d.S.d.S.).Nr
+00000560: 1600 0000 da01 4572 0100 0000 a902 e700  ......Er........
+00000570: 0000 0000 0000 0072 2800 0000 2905 7214  .......r(...).r.
+00000580: 0000 0072 0300 0000 7219 0000 0072 1500  ...r....r....r..
+00000590: 0000 da08 656e 6354 6f53 7472 2904 7209  ....encToStr).r.
+000005a0: 0000 00da 0369 6e73 da0b 6e65 775f 636f  .....ins..new_co
+000005b0: 6e74 656e 74da 066f 7574 7075 7472 0c00  ntent..outputr..
+000005c0: 0000 720c 0000 0072 0d00 0000 da07 656e  ..r....r......en
+000005d0: 6372 7970 7423 0000 0073 1200 0000 0001  crypt#...s......
+000005e0: 0601 0201 1001 0801 0a01 0601 0401 1002  ................
+000005f0: 7a0d 4372 7970 742e 656e 6372 7970 7463  z.Crypt.encryptc
+00000600: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00000610: 0800 0000 4300 0000 735a 0000 007c 006a  ....C...sZ...|.j
+00000620: 0072 527a 2874 016a 027c 006a 007c 006a  .rRz(t.j.|.j.|.j
+00000630: 0364 018d 027d 017c 01a0 04a1 007d 027c  .d...}.|.....}.|
+00000640: 027d 0364 027c 0366 0257 0053 0004 0074  .}.d.|.f.W.S...t
+00000650: 0579 4e01 0001 0001 007c 006a 007d 0364  .yN......|.j.}.d
+00000660: 037c 0366 0206 0059 0053 0030 006e 0464  .|.f...Y.S.0.n.d
+00000670: 0453 0064 0053 0029 054e 2902 da07 6d65  .S.d.S.).N)...me
+00000680: 7373 6167 65da 076d 6169 6e6b 6579 7216  ssage..mainkeyr.
+00000690: 0000 0072 0100 0000 7227 0000 0029 0672  ...r....r'...).r
+000006a0: 1400 0000 7203 0000 00da 0344 6563 7215  ....r......Decr.
+000006b0: 0000 00da 0864 6563 546f 5374 7272 2400  .....decToStrr$.
+000006c0: 0000 2904 7209 0000 005a 0c64 6563 5f69  ..).r....Z.dec_i
+000006d0: 6e73 7461 6e63 6572 2500 0000 722c 0000  nstancer%...r,..
+000006e0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000006f0: da07 6465 6372 7970 742f 0000 0073 1400  ..decrypt/...s..
+00000700: 0000 0001 0601 0201 1201 0801 0401 0a01  ................
+00000710: 0c01 0601 1002 7a0d 4372 7970 742e 6465  ......z.Crypt.de
+00000720: 6372 7970 7463 0100 0000 0000 0000 0000  cryptc..........
+00000730: 0000 0100 0000 0500 0000 4300 0000 731e  ..........C...s.
+00000740: 0000 0064 017c 006a 0064 0064 0285 0219  ...d.|.j.d.d....
+00000750: 009b 0064 037c 006a 019b 0064 049d 0553  ...d.|.j...d...S
+00000760: 0029 054e 7a1b 456e 6372 7970 7469 6e67  .).Nz.Encrypting
+00000770: 2f44 6563 7279 7074 696e 6720 5465 7874  /Decrypting Text
+00000780: 20e9 0800 0000 7a08 2e2e 2057 6974 6820   .....z... With 
+00000790: 7a05 204b 6579 2072 1300 0000 7208 0000  z. Key r....r...
+000007a0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+000007b0: da07 5f5f 7374 725f 5f3c 0000 0073 0200  ..__str__<...s..
+000007c0: 0000 0001 7a0d 4372 7970 742e 5f5f 7374  ....z.Crypt.__st
+000007d0: 725f 5f63 0100 0000 0000 0000 0000 0000  r__c............
+000007e0: 0100 0000 0600 0000 4300 0000 7326 0000  ........C...s&..
+000007f0: 007c 006a 006a 019b 0064 017c 006a 0264  .|.j.j...d.|.j.d
+00000800: 0064 0285 0219 009b 0064 037c 006a 039b  .d.......d.|.j..
+00000810: 0064 049d 0653 0029 054e fa01 2872 3300  .d...S.).N..(r3.
+00000820: 0000 fa01 2cfa 0129 2904 720b 0000 0072  ....,..)).r....r
+00000830: 0e00 0000 7214 0000 0072 1500 0000 7208  ....r....r....r.
+00000840: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000850: 0000 da08 5f5f 7265 7072 5f5f 3e00 0000  ....__repr__>...
+00000860: 7302 0000 0000 017a 0e43 7279 7074 2e5f  s......z.Crypt._
+00000870: 5f72 6570 725f 5f4e 2910 720e 0000 0072  _repr__N).r....r
+00000880: 0f00 0000 7210 0000 0072 0200 0000 721f  ....r....r....r.
+00000890: 0000 0072 2000 0000 7207 0000 00da 0c73  ...r ...r......s
+000008a0: 7461 7469 636d 6574 686f 6472 1b00 0000  taticmethodr....
+000008b0: da03 696e 7472 1700 0000 da05 7475 706c  ..intr......tupl
+000008c0: 6572 2d00 0000 7232 0000 0072 3400 0000  er-...r2...r4...
+000008d0: 7238 0000 0072 0c00 0000 720c 0000 0072  r8...r....r....r
+000008e0: 0c00 0000 720d 0000 0072 1200 0000 0a00  ....r....r......
+000008f0: 0000 7312 0000 0008 0118 0702 0110 0302  ..s.............
+00000900: 0112 0c0e 0c0e 0d08 0272 1200 0000 4e29  .........r....N)
+00000910: 07da 0674 7970 696e 6772 0200 0000 da08  ...typingr......
+00000920: 4173 6843 7279 7074 7203 0000 0072 2400  AshCryptr....r$.
+00000930: 0000 7204 0000 0072 1200 0000 720c 0000  ..r....r....r...
+00000940: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000950: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
+00000960: 0000 000c 010c 0310 05                   .........
```

### Comparing `AshCrypt-1.2.3/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-1.2.4/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/AshCrypt/qr.py` & `AshCrypt-1.2.4/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.2.4/AshCrypt/unittests/unittestAsh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 import struct
 import AshCrypt.Ash as Ash
 
 class AshModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
-        self.message1 = 'Hello there testing ifl it works'
-        self.message2 = b'Hello this is bytes now'
+        self.message1 = 'Hello there testing if it works'
+        self.message2 = b'this is bytes now'
         self.mainkey = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
         self.ins1 = Ash.Enc(message=self.message1, mainkey=self.mainkey)
         self.string_message = self.ins1.encToStr()
         self.bytes_message = self.ins1.encToBytes()
         self.ins2 = Ash.Dec(message=self.bytes_message,mainkey=self.mainkey)
 
     def tearDown(self) -> None:
```

### Comparing `AshCrypt-1.2.3/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.2.4/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.3
+Version: 1.2.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -40,22 +40,22 @@
 
 The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
 <br>check `GUI` header for more info.
 
 
 ### For Developers ###
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for `AshFileCrypt` and `AshTextCrypt` to learn more.
+view the headers for `FileCrypt` and `TextCrypt` to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
-Check `AshDatabase` header to learn more.
+Check `Database` header to learn more.
 
 **After the library is installed**
 <br>to run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 To run the CLI
@@ -130,22 +130,22 @@
 - HMAC : 256 bit hashed using SHA512
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `AshTextCrypt` and `AshFileCrypt` you have to use a 512 bit long key )
+- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `TextCrypt` and `FileCrypt` you have to use a 512 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
-<br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
+<br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
 
 
 ## AshCryptGUI ##
 The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
@@ -182,15 +182,15 @@
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 
 
 
 
-## AshFileCrypt ## 
+## FileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
 ```python
@@ -229,15 +229,15 @@
 instance1.decrypt()
 ```
 **Note** : 
 <br>Sometimes you might forget that you've applied  `encrypt()` more than one time , so when you try to `decrypt()` the file ,  the output is 1 but the file content is still in binary, just apply the function `decrypt()` the same number of times you applied `encrypt()`.
 
 
 That's it, if you follow the steps above then everything should work just fine.
-## AshTextCrypt ## 
+## TextCrypt ## 
 Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
 ```python
 instance1 = Crypt('Hello Wold !',key)
 ```
 ```python
 instance1.encrypt()[1]
 ```
@@ -246,30 +246,30 @@
 ```
 The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occured.
 <br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
 
 **Note**:
 <br>Unlike the `Ash` library where if you try to decrypt a non-encrypted message you get all kinds of errors.
 
-in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
+in `FileCryt` & `TextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
-## AshDatabase ##
+## Database ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
 
-**Note** that in `AshDatabase.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
+**Note** that in `Database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 
 ### Usage ## 
 In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two deafult columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferrably off-grid and completely seprerate from any vulnerable devices, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
```

### Comparing `AshCrypt-1.2.3/LICENSE` & `AshCrypt-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.3/PKG-INFO` & `AshCrypt-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.3
+Version: 1.2.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -40,22 +40,22 @@
 
 The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
 <br>check `GUI` header for more info.
 
 
 ### For Developers ###
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for `AshFileCrypt` and `AshTextCrypt` to learn more.
+view the headers for `FileCrypt` and `TextCrypt` to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>
-Check `AshDatabase` header to learn more.
+Check `Database` header to learn more.
 
 **After the library is installed**
 <br>to run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 To run the CLI
@@ -130,22 +130,22 @@
 - HMAC : 256 bit hashed using SHA512
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `AshTextCrypt` and `AshFileCrypt` you have to use a 512 bit long key )
+- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `TextCrypt` and `FileCrypt` you have to use a 512 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
-<br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
+<br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 
 
 
 ## AshCryptGUI ##
 The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
@@ -182,15 +182,15 @@
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 
 
 
 
-## AshFileCrypt ## 
+## FileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
 ```python
@@ -229,15 +229,15 @@
 instance1.decrypt()
 ```
 **Note** : 
 <br>Sometimes you might forget that you've applied  `encrypt()` more than one time , so when you try to `decrypt()` the file ,  the output is 1 but the file content is still in binary, just apply the function `decrypt()` the same number of times you applied `encrypt()`.
 
 
 That's it, if you follow the steps above then everything should work just fine.
-## AshTextCrypt ## 
+## TextCrypt ## 
 Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
 ```python
 instance1 = Crypt('Hello Wold !',key)
 ```
 ```python
 instance1.encrypt()[1]
 ```
@@ -246,30 +246,30 @@
 ```
 The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occured.
 <br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
 
 **Note**:
 <br>Unlike the `Ash` library where if you try to decrypt a non-encrypted message you get all kinds of errors.
 
-in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
+in `FileCryt` & `TextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
-## AshDatabase ##
+## Database ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
 
-**Note** that in `AshDatabase.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
+**Note** that in `Database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 
 ### Usage ## 
 In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two deafult columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferrably off-grid and completely seprerate from any vulnerable devices, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
```

### Comparing `AshCrypt-1.2.3/README.md` & `AshCrypt-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 
 The project mainly includes a fully fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
 <br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
 
 
 ### For Developers ###
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
-view the headers for [AshFileCrypt](https://github.com/AshGw/AES-256#ashfilecrypt) and [AshTextCrypt](https://github.com/AshGw/AES-256#ashtextcrypt) to learn more.
+view the headers for [FileCrypt](https://github.com/AshGw/AES-256#filecrypt) and [TextCrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
-<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [AshDatabase](https://github.com/AshGw#AshDatabase) header to learn more.
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [Database](https://github.com/AshGw#Database) header to learn more.
 
 ## Installation ##
+There are many ways to go by this : 
+### If you want to use it as a library ###
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
 pip install --upgrade pip 
 ```
 Then install the Library 
 ```bash
@@ -46,32 +48,32 @@
 ```
 This will install the latest version of `AshCrypt`.
 You can start using it in your code by importing its modules : 
 ```python
 from AshCrypt.Ash import *
 ```
 That's it.
+### Ready-to-go Executable files:
+If you want to use the App right away : 
+<br>**For Windows** : Download this repo as a ZIP file, extract the content
+<br>then click on `Executables > AshCryptGUI.exe` This will automatically run the GUI
 
+### Whole repo installation 
 Now if you want to get the whole repo with no manual configurations
 <br>Run this command in the Terminal
 ```bash
 curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 
-<br>If you're testing how this works on a Debian based Docker container you can run this command to automatically set the environment before you run the command above
+you can use this command to automate the environment setup process if you haven't done it  already
 ```bash
-curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/docker-build/env-setup.sh | bash
+curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/Docker-build/env-setup.sh | bash
 ```
-Then run 
-```bash
-source vvv/bin/activate
-```
-
 <details>
 <summary>Got Errors ?</summary>
 
 <h5>For Debian based systems</h5>
 
 1) Install `curl` if you don't have it already 
 ```bash
@@ -82,15 +84,15 @@
 sudo apt-get update
 sudo apt-get install python3-tk 
 ```
 3) If you're running `python 3.6` or older then you might need to install `dataclasses`
 ```
 pip install dataclasses
 ```
-<br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](docker-build)
+<br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
 </details>
 
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
@@ -171,23 +173,22 @@
 - HMAC : 256 bit hashed using SHA512
 - Generates a random 128 bit Initialization Vector (IV) each time for the Cipher
 - PKCS7 message padding
 ### Other Features :
 These focus on ease of use: 
 - No need to manipulate the input to fit, it accepts strings or bytes you can pass them right away
 - You can get a string or a bytes representation of either the encryption or the decryption result
-- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `AshTextCrypt` and `AshFileCrypt` you have to use a 512 bit long key )
+- In Ash module the key is flexible it doesn't have to be 512 bit long, it can actually be of any length but that's up to you to ensure it's security, or leave it as is and use the key generation function to get secure and random keys ( although in `TextCrypt` and `FileCrypt` you have to use a 512 bit long key )
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
-
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
-<br>In my use case 50 takes around 0.5 secs while using the maximun number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
-
+<br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
+<br>You can check how it works by checking this [Jupyter Notebook](demo/demo.ipynb) demo file
 ## AshCryptGUI ##
 ![alt text](important/GUI.png)
 The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
@@ -222,15 +223,15 @@
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 
 
 
 
-## AshFileCrypt ## 
+## FileCrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
 instance1 = CryptFile('target.txt', key)
 ```
 ```python
@@ -269,15 +270,15 @@
 instance1.decrypt()
 ```
 **Note** : 
 <br>Sometimes you might forget that you've applied  `encrypt()` more than one time , so when you try to `decrypt()` the file ,  the output is 1 but the file content is still in binary, just apply the function `decrypt()` the same number of times you applied `encrypt()`.
 
 
 That's it, if you follow the steps above then everything should work just fine.
-## AshTextCrypt ## 
+## TextCrypt ## 
 Same steps above just the naming is different, and keep in mind both accept either strings or bytes 
 ```python
 instance1 = Crypt('Hello Wold !',key)
 ```
 ```python
 instance1.encrypt()[1]
 ```
@@ -286,30 +287,30 @@
 ```
 The result simply returns a tuple so index `[0]` is going to be the confirmation if it's 1 then it worked, else some Error has occured.
 <br>Index `[1]` contains the encrypted/decrypted content that's it very simple.
 
 **Note**:
 <br>Unlike the `Ash` library where if you try to decrypt a non-encrypted message you get all kinds of errors.
 
-in `AshFileCryt` & `AshTextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
+in `FileCryt` & `TextCrypt` it's simpler if you attempt to decrypt an non-encrypted message then you'll get the same message back along with an integer in this case `0` for failure.
 <br>`1`'s for success.
 <br>Non `1`'s for failure (`2`/`0.0`/`0`) each indicate different Errors. 
 
 Error handling here has no Exceptions raised just `1`'s, `0`'s & `2`'s for feedback, just to make it simple and Non-Technical.
 
 
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
-## AshDatabase ##
+## Database ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
 
-**Note** that in `AshDatabase.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
+**Note** that in `Database.py` I'm using `dataclasses` module which was introduced in `python 3.7`, so make sure to install it if you have an older version.
 
 ### Usage ## 
 In the module I'm providing built-in functions to make it easier to perform usual queries on Sqlite tables , by default it creates a table `Classified` with two deafult columns :
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferrably off-grid and completely seprerate from any vulnerable devices, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
```

### Comparing `AshCrypt-1.2.3/setup.py` & `AshCrypt-1.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.2.3',
+    version='1.2.4',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/AshGw/AES-256.git',
-    packages=find_packages(exclude=['important', 'docker-build']),
+    packages=find_packages(exclude=['important', 'Docker-build','.github','Executables','demo']),
     package_data={
         'AshCrypt': ['**'],
     },
     exclude_package_data={
         '': ['.gitignore','LICENSE','README'],
     },
     install_requires=[
```

