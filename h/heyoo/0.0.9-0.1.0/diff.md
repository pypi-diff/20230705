# Comparing `tmp/heyoo-0.0.9-py3-none-any.whl.zip` & `tmp/heyoo-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12408 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    38308 b- defN 23-May-14 19:58 heyoo/__init__.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/LICENSE
--rw-rw-r--  2.0 unx    15573 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      451 b- defN 23-May-14 20:00 heyoo-0.0.9.dist-info/RECORD
-6 files, 55496 bytes uncompressed, 11598 bytes compressed:  79.1%
+Zip file size: 12439 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    39491 b- defN 23-Jul-05 13:49 heyoo/__init__.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-05 14:15 heyoo-0.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    15505 b- defN 23-Jul-05 14:15 heyoo-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-05 14:15 heyoo-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-05 14:15 heyoo-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      451 b- defN 23-Jul-05 14:15 heyoo-0.1.0.dist-info/RECORD
+6 files, 56611 bytes uncompressed, 11629 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: heyoo/__init__.py
 Comment: 
 
-Filename: heyoo-0.0.9.dist-info/LICENSE
+Filename: heyoo-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: heyoo-0.0.9.dist-info/METADATA
+Filename: heyoo-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: heyoo-0.0.9.dist-info/WHEEL
+Filename: heyoo-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: heyoo-0.0.9.dist-info/top_level.txt
+Filename: heyoo-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: heyoo-0.0.9.dist-info/RECORD
+Filename: heyoo-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## heyoo/__init__.py

```diff
@@ -72,14 +72,50 @@
             logging.info(f"Message sent to {recipient_id}")
             return r.json()
         logging.info(f"Message not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
         return r.json()
 
+    def send_reaction(
+        self, emoji, message_id, recipient_id, recipient_type="individual"
+    ):
+        """
+         Sends a reaction message to a WhatsApp user's message
+
+         Args:
+                emoji[str]: Emoji to become a reaction to a message. Ex.: '\uD83D\uDE00' (😀)
+                message_id[str]: Message id for a reaction to be attached to
+                recipient_id[str]: Phone number of the user with country code without +
+                recipient_type[str]: Type of the recipient, either individual or group
+
+        Example:
+            ```python
+            >>> from whatsapp import WhatsApp
+            >>> whatsapp = WhatsApp(token, phone_number_id)
+            >>> whatsapp.send_reaction("\uD83D\uDE00", "wamid.HBgLM...", "5511999999999")
+
+        """
+        data = {
+            "messaging_product": "whatsapp",
+            "recipient_type": recipient_type,
+            "to": recipient_id,
+            "type": "reaction",
+            "reaction": {"message_id": message_id, "emoji": emoji},
+        }
+        logging.info(f"Sending reaction to number {recipient_id} message id {message_id}")
+        r = requests.post(f"{self.url}", headers=self.headers, json=data)
+        if r.status_code == 200:
+            logging.info(f"Reaction sent to number {recipient_id} message id {message_id}")
+            return r.json()
+        logging.info(f"Message not sent  to number {recipient_id} message id {message_id}")
+        logging.info(f"Status code: {r.status_code}")
+        logging.error(f"Response: {r.json()}")
+        return r.json()
+
     def reply_to_message(
         self, message_id: str, recipient_id: str, message: str, preview_url: bool = True
     ):
         """
         Replies to a message
 
         Args:
@@ -140,21 +176,15 @@
         r = requests.post(self.url, headers=self.headers, json=data)
         if r.status_code == 200:
             logging.info(f"Template sent to {recipient_id}")
             return r.json()
         logging.info(f"Template not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
-        return r.json()
-
-    def send_templatev2(self, template, recipient_id, components, lang: str = "en_US"):
-        message = f"{Fore.RED}The 'send_templatev2' method is being deprecated and will be removed in the future. Please use the 'send_template' method instead.{Style.RESET_ALL}"
-        warnings.warn(message, DeprecationWarning)
-        return send_template(template, recipient_id, components, lang=lang)
-    
+        return r.json()    
     
     def send_location(self, lat, long, name, address, recipient_id):
         """
         Sends a location message to a WhatsApp user
 
         Args:
             lat[str]: Latitude of the location
@@ -575,18 +605,18 @@
             "message_id": message_id,
         }
         logging.info(f"Marking message {message_id} as read")
         response = requests.post(
             f"{self.v15_base_url}/{self.phone_number_id}/messages",
             headers=headers,
             json=json_data,
-        ).json()
+        )
         if response.status_code == 200:
             logging.info(f"Message {message_id} marked as read")
-            return response
+            return response.json()
         logging.info(f"Error marking message {message_id} as read")
         logging.info(f"Status code: {response.status_code}")
         logging.info(f"Response: {response.json()}")
         return response
 
     def create_button(self, button: Dict[Any, Any]) -> Dict[Any, Any]:
         """
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `heyoo-0.0.9.dist-info/LICENSE` & `heyoo-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `heyoo-0.0.9.dist-info/METADATA` & `heyoo-0.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: heyoo
-Version: 0.0.9
+Version: 0.1.0
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/Neurotech-HQ/heyoo
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
-Download-URL: https://github.com/Neurotech-HQ/heyoo/archive/refs/tags/v0.3.tar.gz
+Download-URL: https://github.com/Neurotech-HQ/heyoo/archive/refs/tags/v0.2.tar.gz
 Keywords: heyoo,heyoo-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -288,16 +288,14 @@
             }
       },
     )
 ```
 
 ## Sending a Template Messages
 
-⚠️Warning! the `send_templatev2()` method is being deprecated.
-
 Here how to send a pre-approved template message, Template messages can either be;
 
 1. Text template
 2. Media based template
 3. Interactive template
 
 You can customize the template message by passing a dictionary of components.
```

