# Comparing `tmp/ez0th-0.1.0.tar.gz` & `tmp/ez0th-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez0th-0.1.0.tar", last modified: Wed Jun 28 08:28:25 2023, max compression
+gzip compressed data, was "ez0th-0.1.1.tar", last modified: Wed Jul  5 05:27:01 2023, max compression
```

## Comparing `ez0th-0.1.0.tar` & `ez0th-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 08:28:25.880144 ez0th-0.1.0/
--rw-rw-rw-   0        0        0    12347 2023-06-28 08:28:25.880144 ez0th-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10141 2023-06-28 08:27:15.000000 ez0th-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 08:28:25.867735 ez0th-0.1.0/ez0th/
--rw-rw-rw-   0        0        0     9321 2023-06-28 08:22:15.000000 ez0th-0.1.0/ez0th/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-06-28 08:24:43.000000 ez0th-0.1.0/ez0th/test.py
-drwxrwxrwx   0        0        0        0 2023-06-28 08:28:25.878644 ez0th-0.1.0/ez0th.egg-info/
--rw-rw-rw-   0        0        0    12347 2023-06-28 08:28:25.000000 ez0th-0.1.0/ez0th.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-28 08:28:25.000000 ez0th-0.1.0/ez0th.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 08:28:25.000000 ez0th-0.1.0/ez0th.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-28 08:28:25.000000 ez0th-0.1.0/ez0th.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-28 08:28:25.000000 ez0th-0.1.0/ez0th.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 08:28:25.881149 ez0th-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-06-28 08:28:00.000000 ez0th-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:27:01.750945 ez0th-0.1.1/
+-rw-rw-rw-   0        0        0    13581 2023-07-05 05:27:01.750945 ez0th-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11167 2023-07-05 05:24:33.000000 ez0th-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 05:27:01.738316 ez0th-0.1.1/ez0th/
+-rw-rw-rw-   0        0        0    10115 2023-07-05 05:20:50.000000 ez0th-0.1.1/ez0th/__init__.py
+-rw-rw-rw-   0        0        0     3199 2023-07-05 05:22:11.000000 ez0th-0.1.1/ez0th/test.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:27:01.749830 ez0th-0.1.1/ez0th.egg-info/
+-rw-rw-rw-   0        0        0    13581 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 05:27:01.750945 ez0th-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-07-05 05:26:53.000000 ez0th-0.1.1/setup.py
```

### Comparing `ez0th-0.1.0/PKG-INFO` & `ez0th-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
         
@@ -84,14 +84,27 @@
             sess_token = sess_token,    # Session token
             password = "abc123456", # New password
             db = db,    # Database
         )
         # Check result
         print(success_flag)
         
+        # Prepare updated user information
+        success_flag, info = ez0th.auth(sess_token, db) # Authorization (login verification) [ez0th]
+        old_user_info = info["account_info"]["info"]
+        new_user_info = {**old_user_info, "Role": "Technical Leader"}
+        # Update user information [ez0th]
+        success_flag = ez0th.update_user_info(
+            sess_token = sess_token,    # Session token
+            new_user_info = new_user_info,  # Updated user information
+            db = db,    # Database
+        )
+        # Check result
+        print(success_flag)
+        
         # Logout [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # Session token
             db = db # Database
         )
         # Check result
         print(success_flag)
@@ -195,14 +208,27 @@
             sess_token = sess_token,    # セッショントークン
             password = "abc123456", # 変更後のパスワード
             db = db,    # データベース
         )
         # 結果確認
         print(success_flag)
         
+        # 変更後ユーザー情報の準備
+        success_flag, info = ez0th.auth(sess_token, db) # 認可 (ログイン確認) [ez0th]
+        old_user_info = info["account_info"]["info"]
+        new_user_info = {**old_user_info, "役職": "技術リーダー"}
+        # ユーザー情報更新 [ez0th]
+        success_flag = ez0th.update_user_info(
+            sess_token = sess_token,    # セッショントークン
+            new_user_info = new_user_info,  # 変更後のユーザー情報
+            db = db,    # データベース
+        )
+        # 結果確認
+        print(success_flag)
+        
         # ログアウト [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # セッショントークン
             db = db # データベース
         )
         # 結果確認
         print(success_flag)
```

### Comparing `ez0th-0.1.0/README.md` & `ez0th-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,27 @@
     sess_token = sess_token,    # Session token
     password = "abc123456", # New password
     db = db,    # Database
 )
 # Check result
 print(success_flag)
 
+# Prepare updated user information
+success_flag, info = ez0th.auth(sess_token, db) # Authorization (login verification) [ez0th]
+old_user_info = info["account_info"]["info"]
+new_user_info = {**old_user_info, "Role": "Technical Leader"}
+# Update user information [ez0th]
+success_flag = ez0th.update_user_info(
+    sess_token = sess_token,    # Session token
+    new_user_info = new_user_info,  # Updated user information
+    db = db,    # Database
+)
+# Check result
+print(success_flag)
+
 # Logout [ez0th]
 success_flag = ez0th.logout(
     sess_token = sess_token,    # Session token
     db = db # Database
 )
 # Check result
 print(success_flag)
@@ -187,14 +200,27 @@
     sess_token = sess_token,    # セッショントークン
     password = "abc123456", # 変更後のパスワード
     db = db,    # データベース
 )
 # 結果確認
 print(success_flag)
 
+# 変更後ユーザー情報の準備
+success_flag, info = ez0th.auth(sess_token, db) # 認可 (ログイン確認) [ez0th]
+old_user_info = info["account_info"]["info"]
+new_user_info = {**old_user_info, "役職": "技術リーダー"}
+# ユーザー情報更新 [ez0th]
+success_flag = ez0th.update_user_info(
+    sess_token = sess_token,    # セッショントークン
+    new_user_info = new_user_info,  # 変更後のユーザー情報
+    db = db,    # データベース
+)
+# 結果確認
+print(success_flag)
+
 # ログアウト [ez0th]
 success_flag = ez0th.logout(
     sess_token = sess_token,    # セッショントークン
     db = db # データベース
 )
 # 結果確認
 print(success_flag)
```

### Comparing `ez0th-0.1.0/ez0th/__init__.py` & `ez0th-0.1.1/ez0th/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,7 +223,31 @@
 	try:
 		db["update"](inner_id,
 			{**db["read"](inner_id), "pw_salt": pw_salt, "pw_hash": pw_hash}
 		)
 		return True
 	except:
 		return False
+
+# ユーザー情報更新 [ez0th]
+def update_user_info(
+	sess_token,	# セッショントークン
+	new_user_info,	# 変更後のユーザー情報
+	db,	# データベース
+):
+	if db == "auto": db = json_stock("./__ez0th_user_db__/")
+	# 引数インジェクションチェック (セキュリティー対策; ptnを満たす文字列かどうかをチェック)
+	check_injection(sess_token, ptn = "sess_token_")
+	# !infoは特にチェックしない
+	# 認可 (ログイン確認) [ez0th]
+	flag, old_info = auth(sess_token, db)
+	if flag is False: return False
+	# 内部ユーザーidの取得
+	inner_id = old_info["inner_id"]
+	# DBの更新
+	try:
+		db["update"](inner_id,
+			{**db["read"](inner_id), "info": new_user_info}
+		)
+		return True
+	except:
+		return False
```

### Comparing `ez0th-0.1.0/ez0th/test.py` & `ez0th-0.1.1/ez0th/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,27 @@
 )
 # 結果確認
 print(success_flag)
 
 # 次回のための再変更
 success_flag = ez0th.change_pw(sess_token, "abc123", db)	# パスワード変更 [ez0th]
 
+# 変更後ユーザー情報の準備
+success_flag, info = ez0th.auth(sess_token, db)	# 認可 (ログイン確認) [ez0th]
+old_user_info = info["account_info"]["info"]
+new_user_info = {**old_user_info, "役職": "技術リーダー"}
+# ユーザー情報更新 [ez0th]
+success_flag = ez0th.update_user_info(
+	sess_token = sess_token,	# セッショントークン
+	new_user_info = new_user_info,	# 変更後のユーザー情報
+	db = db,	# データベース
+)
+# 結果確認
+print(success_flag)
+
 # ログアウト [ez0th]
 success_flag = ez0th.logout(
 	sess_token = sess_token,	# セッショントークン
 	db = db	# データベース
 )
 # 結果確認
 print(success_flag)
```

### Comparing `ez0th-0.1.0/ez0th.egg-info/PKG-INFO` & `ez0th-0.1.1/ez0th.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
         
@@ -84,14 +84,27 @@
             sess_token = sess_token,    # Session token
             password = "abc123456", # New password
             db = db,    # Database
         )
         # Check result
         print(success_flag)
         
+        # Prepare updated user information
+        success_flag, info = ez0th.auth(sess_token, db) # Authorization (login verification) [ez0th]
+        old_user_info = info["account_info"]["info"]
+        new_user_info = {**old_user_info, "Role": "Technical Leader"}
+        # Update user information [ez0th]
+        success_flag = ez0th.update_user_info(
+            sess_token = sess_token,    # Session token
+            new_user_info = new_user_info,  # Updated user information
+            db = db,    # Database
+        )
+        # Check result
+        print(success_flag)
+        
         # Logout [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # Session token
             db = db # Database
         )
         # Check result
         print(success_flag)
@@ -195,14 +208,27 @@
             sess_token = sess_token,    # セッショントークン
             password = "abc123456", # 変更後のパスワード
             db = db,    # データベース
         )
         # 結果確認
         print(success_flag)
         
+        # 変更後ユーザー情報の準備
+        success_flag, info = ez0th.auth(sess_token, db) # 認可 (ログイン確認) [ez0th]
+        old_user_info = info["account_info"]["info"]
+        new_user_info = {**old_user_info, "役職": "技術リーダー"}
+        # ユーザー情報更新 [ez0th]
+        success_flag = ez0th.update_user_info(
+            sess_token = sess_token,    # セッショントークン
+            new_user_info = new_user_info,  # 変更後のユーザー情報
+            db = db,    # データベース
+        )
+        # 結果確認
+        print(success_flag)
+        
         # ログアウト [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # セッショントークン
             db = db # データベース
         )
         # 結果確認
         print(success_flag)
```

### Comparing `ez0th-0.1.0/setup.py` & `ez0th-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 657a 3074 682f 2229  develop_ez0th/")
 000000c0: 2061 7320 703a 0d0a 0973 6574 7570 280d   as p:...setup(.
 000000d0: 0a09 096e 616d 6520 3d20 2265 7a30 7468  ...name = "ez0th
 000000e0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-000000f0: 2230 2e31 2e30 222c 0d0a 0909 6465 7363  "0.1.0",....desc
+000000f0: 2230 2e31 2e31 222c 0d0a 0909 6465 7363  "0.1.1",....desc
 00000100: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
 00000110: 6e20 4c69 6272 6172 7920 666f 7220 4561  n Library for Ea
 00000120: 7379 2041 7574 6865 6e74 6963 6174 696f  sy Authenticatio
 00000130: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
 00000140: 696f 6e22 2c0d 0a09 0961 7574 686f 7220  ion",....author 
 00000150: 3d20 2262 6962 5f69 6e66 222c 0d0a 0909  = "bib_inf",....
 00000160: 6175 7468 6f72 5f65 6d61 696c 203d 2022  author_email = "
```

