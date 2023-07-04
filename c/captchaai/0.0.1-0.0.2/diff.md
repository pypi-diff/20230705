# Comparing `tmp/captchaai-0.0.1.tar.gz` & `tmp/captchaai-0.0.2.tar.gz`

## Comparing `captchaai-0.0.1.tar` & `captchaai-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 captchaai-0.0.1/src/captchaai/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 captchaai-0.0.1/src/captchaai/api.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 captchaai-0.0.1/src/captchaai/solver.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 captchaai-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0    13006 2020-02-02 00:00:00.000000 captchaai-0.0.1/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 captchaai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    13588 2020-02-02 00:00:00.000000 captchaai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/api.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/setup.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/solver.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 captchaai-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 captchaai-0.0.2/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 captchaai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 captchaai-0.0.2/PKG-INFO
```

### Comparing `captchaai-0.0.1/src/captchaai/api.py` & `captchaai-0.0.2/src/captchaai/api.py`

 * *Files identical despite different names*

### Comparing `captchaai-0.0.1/LICENSE.txt` & `captchaai-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `captchaai-0.0.1/pyproject.toml` & `captchaai-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "captchaai"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="captchaai developers", email="dev@captchaai.com" },
 ]
 description = "A package to enable interacting with the api of captchaai.com by python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `captchaai-0.0.1/PKG-INFO` & `captchaai-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captchaai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to enable interacting with the api of captchaai.com by python.
 Project-URL: Homepage, https://github.com/captchaai-developers/captchaai
 Project-URL: Bug Tracker, https://github.com/captchaai-developers/captchaai/issues
 Author-email: captchaai developers <dev@captchaai.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,30 +18,17 @@
 - [Python Module for captchaAI API](#python-module-for-captchaAI-api)
   - [Installation](#installation)
   - [Configuration](#configuration)
     - [captchaAI instance options](#captchaAI-instance-options)
   - [Solve captcha](#solve-captcha)
     - [Captcha options](#captcha-options)
     - [Normal Captcha](#normal-captcha)
-    - [Text Captcha](#text-captcha)
     - [ReCaptcha v2](#recaptcha-v2)
     - [ReCaptcha v3](#recaptcha-v3)
-    - [FunCaptcha](#funcaptcha)
-    - [GeeTest](#geetest)
     - [hCaptcha](#hcaptcha)
-    - [GeeTest v4](#geetest-v4)
-    - [Lemin Cropped Captcha](#lemin-cropped-captcha)
-    - [Cloudflare Turnstile](#cloudflare-turnstile)
-    - [Amazon WAF](#amazon-waf)
-    - [KeyCaptcha](#keycaptcha)
-    - [Capy](#capy)
-    - [Grid](#grid)
-    - [Canvas](#canvas)
-    - [ClickCaptcha](#clickcaptcha)
-    - [Rotate](#rotate)
   - [Other methods](#other-methods)
     - [send / getResult](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
@@ -54,42 +41,39 @@
 
 
 ## Configuration
 
 captchaAI instance can be created like this:
 
 ```python 
-from captchaAI import CaptchaAI
+from captchaAI import captchaAI
 
-solver = CaptchaAI('YOUR_API_KEY')
+solver = captchaAI('YOUR_API_KEY')
 ```
 Also there are few options that can be configured:
 
 ```python 
 config = {
-            'server':           'captchaAI.com',
             'apiKey':           'YOUR_API_KEY',
             'softId':            123,
             'callback':         'https://your.site/result-receiver',
             'defaultTimeout':    120,
             'recaptchaTimeout':  600,
             'pollingInterval':   10,
         }
 solver = captchaAI(**config)
 ```
 
-### CaptchaAI instance options
+### captchaAI instance options
 
 | Option           | Default value  | Description                                                                                                                                        |
 | ---------------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
-| server           | `captchaAI.com` | API server. You can set it to `rucaptcha.com` if your account is registered there                                                                  |
 | softId           | -              | your software ID obtained after publishing in [captchaAI sofware catalog]                                                                           |
-| callback         | -              | URL of your web-sever that receives the captcha recognition result. The URl should be first registered in [pingback settings] of your account      |
 | defaultTimeout   | 120            | Polling timeout in seconds for all captcha types except ReCaptcha. Defines how long the module tries to get the answer from `res.php` API endpoint |
-| recaptchaTimeout | 600            | Polling timeout for ReCaptcha in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
+| recaptchaTimeout | 240            | Polling timeout for ReCaptcha in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
 | pollingInterval  | 10             | Interval in seconds between requests to `res.php` API endpoint, setting values less than 5 seconds is not recommended                              |
 
 >  **IMPORTANT:** once `callback` is defined for `captchaAI` instance, all methods return only the captcha ID and DO NOT poll the API to get the result. The result will be sent to the callback URL.
 To get the answer manually use [getResult method](#send--getresult)
 
 ## Solve captcha
 When you submit any image-based captcha use can provide additional options to help captchaAI workers to solve it properly.
@@ -113,19 +97,14 @@
 To bypass a normal captcha (distorted text on image) use the following method. This method also can be used to recognize any text on the image.
 ```python 
 result = solver.normal('path/to/captcha.jpg', param1=..., ...)
 # OR
 result = solver.normal('https://site-with-captcha.com/path/to/captcha.jpg', param1=..., ...)
 ```
 
-### Text Captcha
-This method can be used to bypass a captcha that requires to answer a question provided in clear text.
-```python 
-result = solver.text('If tomorrow is Saturday, what day is today?', param1=..., ...)
-```
 
 ### ReCaptcha v2
 Use this method to solve ReCaptcha V2 and obtain a token to bypass the protection.
 ```python 
 result = solver.recaptcha(sitekey='6Le-wvkSVVABCPBMRTvw0Q4Muexq1bi0DJwx_mJ-',
                           url='https://mysite.com/page/with/recaptcha',
                           param1=..., ...)
@@ -136,128 +115,23 @@
 ```python
 result = solver.recaptcha(sitekey='6Le-wvkSVVABCPBMRTvw0Q4Muexq1bi0DJwx_mJ-',
                             url='https://mysite.com/page/with/recaptcha',
                             version='v3',
                             param1=..., ...)
 ```
 
-### FunCaptcha
-FunCaptcha (Arkoselabs) solving method. Returns a token.
-```python
-result = solver.funcaptcha(sitekey='6Le-wvkSVVABCPBMRTvw0Q4Muexq1bi0DJwx_mJ-',
-                            url='https://mysite.com/page/with/funcaptcha',
-                            param1=..., ...)
-
-```
-
-
-### GeeTest
-Method to solve GeeTest puzzle captcha. Returns a set of tokens as JSON.
-```python
-result = solver.geetest(gt='f1ab2cdefa3456789012345b6c78d90e',
-                        challenge='12345678abc90123d45678ef90123a456b',
-                        url='https://www.site.com/page/',
-                        param1=..., ...)
-
-```
-
-
 ### hCaptcha
 Use this method to solve hCaptcha challenge. Returns a token to bypass captcha.
 ```python
 result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
                             url='https://www.site.com/page/', 
                             param1=..., ...)
 
 ```
 
-### GeeTest v4
-Use this method to solve GeeTest v4. Returns the response in JSON.
-```python
-result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
-                            url='https://www.site.com/page/',  
-                            param1=..., ...)
-
-```
-
-
-### Lemin Cropped Captcha
-Use this method to solve hCaptcha challenge. Returns JSON with answer containing the following values: answer, challenge_id.
-```python
-result = solver.lemin(captcha_id='CROPPED_1abcd2f_a1234b567c890d12ef3a456bc78d901d',
-                            div_id='lemin-cropped-captcha', 
-                            url='https://www.site.com/page/',
-                            param1=..., ...)
-
-```
-
-
-### Cloudflare Turnstile
-Use this method to solve Cloudflare Turnstile. Returns JSON with the token.
-```python
-result = solver.turnstile(sitekey='0x1AAAAAAAAkg0s2VIOD34y5',
-                            url='http://mysite.com/', 
-                            param1=..., ...)
-
-```
-
-### Amazon WAF
-Use this method to solve Amazon WAF Captcha also known as AWS WAF Captcha is a part of Intelligent threat mitigation for Amazon AWS. Returns JSON with the token.
-```python
-result = solver.amazon_waf(sitekey='0x1AAAAAAAAkg0s2VIOD34y5',
-                            iv='CgAHbCe2GgAAAAAj', 
-                            context='9BUgmlm48F92WUoqv97a49ZuEJJ50TCk9MVr3C7WMtQ0X6flVbufM4n8mjFLmbLVAPgaQ1Jydeaja94iAS49ljb+sUNLoukWedAQZKrlY4RdbOOzvcFqmD/ZepQFS9N5w15Exr4VwnVq+HIxTsDJwRviElWCdzKDebN/mk8/eX2n7qJi5G3Riq0tdQw9+C4diFZU5E97RSeahejOAAJTDqduqW6uLw9NsjJBkDRBlRjxjn5CaMMo5pYOxYbGrM8Un1JH5DMOLeXbq1xWbC17YSEoM1cRFfTgOoc+VpCe36Ai9Kc='
-                            url='https://non-existent-example.execute-api.us-east-1.amazonaws.com/latest'
-                            param1=..., ...)
-
-```
-
-
-### KeyCaptcha
-Token-based method to solve KeyCaptcha.
-```python
-result = solver.keycaptcha(s_s_c_user_id=10,
-    				   s_s_c_session_id='493e52c37c10c2bcdf4a00cbc9ccd1e8',
-    				   s_s_c_web_server_sign='9006dc725760858e4c0715b835472f22-pz-',
-    				   s_s_c_web_server_sign2='2ca3abe86d90c6142d5571db98af6714',
-    				   url='https://www.keycaptcha.ru/demo-magnetic/', 
-    				   param1=..., ...)
-
-```
-
-### Capy
-Token-based method to bypass Capy puzzle captcha.
-```python
-result = solver.capy(sitekey='PUZZLE_Abc1dEFghIJKLM2no34P56q7rStu8v',
-                     url='http://mysite.com/',
-                     api_server='https://jp.api.capy.me/',
-                     param1=..., ...)
-```
-### Grid
-Grid method is originally called Old ReCaptcha V2 method. The method can be used to bypass any type of captcha where you can apply a grid on image and need to click specific grid boxes. Returns numbers of boxes.
-```python
-result = solver.grid('path/to/captcha.jpg', param1=..., ...)
-```
-### Canvas
-Canvas method can be used when you need to draw a line around an object on image. Returns a set of points' coordinates to draw a polygon.
-```python
-result = solver.canvas('path/to/captcha.jpg', param1=..., ...)
-```
-### ClickCaptcha
-ClickCaptcha method returns coordinates of points on captcha image. Can be used if you need to click on particular points on the image.
-```python
-result = solver.coordinates('path/to/captcha.jpg', param1=..., ...)
-```
-
-### Rotate
-This method can be used to solve a captcha that asks to rotate an object. Mostly used to bypass FunCaptcha. Returns the rotation angle.
-```python
-result = solver.rotate('path/to/captcha.jpg', param1=..., ...)
-```
-
 ## Other methods
 
 ### send / getResult
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . . 
@@ -329,8 +203,8 @@
         result = await loop.run_in_executor(pool, lambda: captchaAI(API_KEY).normal(image))
         return result
 ```
 
 
 [captchaAI]: https://captchaAI.com/
 [examples directory]: /examples
-[asyncio]: https://docs.python.org/3/library/asyncio.html
+[asyncio]: https://docs.python.org/3/library/asyncio.html
```

