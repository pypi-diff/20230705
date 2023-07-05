# Comparing `tmp/django-email-certify-1.0.tar.gz` & `tmp/django-email-certify-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-email-certify-1.0.tar", last modified: Sat Jun 10 12:36:21 2023, max compression
+gzip compressed data, was "django-email-certify-1.1.tar", last modified: Wed Jul  5 09:20:39 2023, max compression
```

## Comparing `django-email-certify-1.0.tar` & `django-email-certify-1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:36:21.715189 django-email-certify-1.0/
--rw-rw----   0 root         (0) everybody  (9997)     1073 2023-06-10 10:42:11.000000 django-email-certify-1.0/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)       83 2023-06-10 11:16:40.000000 django-email-certify-1.0/MANIFEST.in
--rw-rw----   0 root         (0) everybody  (9997)     3064 2023-06-10 12:36:21.715189 django-email-certify-1.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2062 2023-06-10 12:35:21.000000 django-email-certify-1.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:36:21.585188 django-email-certify-1.0/django_email_certify.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     3064 2023-06-10 12:36:19.000000 django-email-certify-1.0/django_email_certify.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      825 2023-06-10 12:36:20.000000 django-email-certify-1.0/django_email_certify.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-10 12:36:19.000000 django-email-certify-1.0/django_email_certify.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       12 2023-06-10 12:36:19.000000 django-email-certify-1.0/django_email_certify.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       19 2023-06-10 12:36:19.000000 django-email-certify-1.0/django_email_certify.egg-info/top_level.txt
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:36:21.655189 django-email-certify-1.0/email_verification/
--rw-rw----   0 root         (0) everybody  (9997)        0 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      152 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/admin.py
--rw-rw----   0 root         (0) everybody  (9997)      167 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/apps.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:36:21.681856 django-email-certify-1.0/email_verification/migrations/
--rw-rw----   0 root         (0) everybody  (9997)      826 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/migrations/0001_initial.py
--rw-rw----   0 root         (0) everybody  (9997)      324 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/migrations/0002_remove_token_valid.py
--rw-rw----   0 root         (0) everybody  (9997)        0 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/migrations/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      588 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/models.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:36:21.501855 django-email-certify-1.0/email_verification/templates/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-10 12:36:21.711856 django-email-certify-1.0/email_verification/templates/email_verification/
--rw-rw----   0 root         (0) everybody  (9997)     1027 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/templates/email_verification/mail.html
--rw-rw----   0 root         (0) everybody  (9997)     1396 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/templates/email_verification/pre-login-failure.html
--rw-rw----   0 root         (0) everybody  (9997)     1388 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/templates/email_verification/pre-login-success.html
--rw-rw----   0 root         (0) everybody  (9997)       60 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/tests.py
--rw-rw----   0 root         (0) everybody  (9997)      152 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/urls.py
--rw-rw----   0 root         (0) everybody  (9997)     2072 2023-06-10 10:41:52.000000 django-email-certify-1.0/email_verification/views.py
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-10 11:12:41.000000 django-email-certify-1.0/pyproject.toml
--rw-rw----   0 root         (0) everybody  (9997)     1017 2023-06-10 12:36:21.731856 django-email-certify-1.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-10 11:15:51.000000 django-email-certify-1.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-05 09:20:38.962202 django-email-certify-1.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1073 2023-07-05 09:09:39.000000 django-email-certify-1.1/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-05 09:09:39.000000 django-email-certify-1.1/MANIFEST.in
+-rw-rw----   0 root         (0) everybody  (9997)     3109 2023-07-05 09:20:38.962202 django-email-certify-1.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2105 2023-07-05 09:20:04.000000 django-email-certify-1.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-05 09:20:38.885535 django-email-certify-1.1/django_email_certify.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     3109 2023-07-05 09:20:37.000000 django-email-certify-1.1/django_email_certify.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      825 2023-07-05 09:20:38.000000 django-email-certify-1.1/django_email_certify.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-05 09:20:37.000000 django-email-certify-1.1/django_email_certify.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       12 2023-07-05 09:20:37.000000 django-email-certify-1.1/django_email_certify.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       19 2023-07-05 09:20:37.000000 django-email-certify-1.1/django_email_certify.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-05 09:20:38.925536 django-email-certify-1.1/email_verification/
+-rw-rw----   0 root         (0) everybody  (9997)        0 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      152 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/admin.py
+-rw-rw----   0 root         (0) everybody  (9997)      167 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/apps.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-05 09:20:38.942202 django-email-certify-1.1/email_verification/migrations/
+-rw-rw----   0 root         (0) everybody  (9997)      826 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/migrations/0001_initial.py
+-rw-rw----   0 root         (0) everybody  (9997)      324 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/migrations/0002_remove_token_valid.py
+-rw-rw----   0 root         (0) everybody  (9997)        0 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/migrations/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      593 2023-07-05 09:12:50.000000 django-email-certify-1.1/email_verification/models.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-05 09:20:38.842202 django-email-certify-1.1/email_verification/templates/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-05 09:20:38.958869 django-email-certify-1.1/email_verification/templates/email_verification/
+-rw-rw----   0 root         (0) everybody  (9997)     1027 2023-07-05 09:15:42.000000 django-email-certify-1.1/email_verification/templates/email_verification/mail.html
+-rw-rw----   0 root         (0) everybody  (9997)     1396 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/templates/email_verification/pre-login-failure.html
+-rw-rw----   0 root         (0) everybody  (9997)     1386 2023-07-05 09:17:14.000000 django-email-certify-1.1/email_verification/templates/email_verification/pre-login-success.html
+-rw-rw----   0 root         (0) everybody  (9997)       60 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/tests.py
+-rw-rw----   0 root         (0) everybody  (9997)      152 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/urls.py
+-rw-rw----   0 root         (0) everybody  (9997)     2072 2023-07-05 09:09:39.000000 django-email-certify-1.1/email_verification/views.py
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-05 09:09:39.000000 django-email-certify-1.1/pyproject.toml
+-rw-rw----   0 root         (0) everybody  (9997)     1019 2023-07-05 09:20:38.972202 django-email-certify-1.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-05 09:09:39.000000 django-email-certify-1.1/setup.py
```

### Comparing `django-email-certify-1.0/LICENSE` & `django-email-certify-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-email-certify-1.0/PKG-INFO` & `django-email-certify-1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-email-certify
-Version: 1.0
+Version: 1.1
 Summary: A Django package to manage user email verification on registration
-Home-page: https://github.com/codewitgabi/django-email-certify
+Home-page: https://github.com/codewitgabi/email-verification-pkg
 Author: Gabriel Michael Ojomakpene (codewitgabi)
 Author-email: codewitgabi222@gmail.com
 License: MIT-License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
-`django-email-certify` is a django package that verifies a user's email on registration.
+`email_verification` is a django package that verifies a user's email on registration.
 
 - An email is sent to registered users to verify their email before login. 
 - All users that are not verified after 24hrs will be automatically deleted from the database.
 
 # Installation
 
 ```
@@ -100,11 +100,13 @@
 
 def signup(request):
     form = RegisterForm() # create your form class
     if request.method == "POST":
         form = RegisterForm(request.POST)
         if form.is_valid():
             VerifyEmail(request, form)
+
+            return redirect("redirect_url")
     
     return render(request, "register.html", {"form": form})
 ```
```

### Comparing `django-email-certify-1.0/README.md` & `django-email-certify-1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Project Description
 
-`django-email-certify` is a django package that verifies a user's email on registration.
+`email_verification` is a django package that verifies a user's email on registration.
 
 - An email is sent to registered users to verify their email before login. 
 - All users that are not verified after 24hrs will be automatically deleted from the database.
 
 # Installation
 
 ```
@@ -75,11 +75,13 @@
 
 def signup(request):
     form = RegisterForm() # create your form class
     if request.method == "POST":
         form = RegisterForm(request.POST)
         if form.is_valid():
             VerifyEmail(request, form)
+
+            return redirect("redirect_url")
     
     return render(request, "register.html", {"form": form})
 ```
```

### Comparing `django-email-certify-1.0/django_email_certify.egg-info/PKG-INFO` & `django-email-certify-1.1/django_email_certify.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-email-certify
-Version: 1.0
+Version: 1.1
 Summary: A Django package to manage user email verification on registration
-Home-page: https://github.com/codewitgabi/django-email-certify
+Home-page: https://github.com/codewitgabi/email-verification-pkg
 Author: Gabriel Michael Ojomakpene (codewitgabi)
 Author-email: codewitgabi222@gmail.com
 License: MIT-License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
-`django-email-certify` is a django package that verifies a user's email on registration.
+`email_verification` is a django package that verifies a user's email on registration.
 
 - An email is sent to registered users to verify their email before login. 
 - All users that are not verified after 24hrs will be automatically deleted from the database.
 
 # Installation
 
 ```
@@ -100,11 +100,13 @@
 
 def signup(request):
     form = RegisterForm() # create your form class
     if request.method == "POST":
         form = RegisterForm(request.POST)
         if form.is_valid():
             VerifyEmail(request, form)
+
+            return redirect("redirect_url")
     
     return render(request, "register.html", {"form": form})
 ```
```

### Comparing `django-email-certify-1.0/django_email_certify.egg-info/SOURCES.txt` & `django-email-certify-1.1/django_email_certify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-email-certify-1.0/email_verification/migrations/0001_initial.py` & `django-email-certify-1.1/email_verification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-email-certify-1.0/email_verification/models.py` & `django-email-certify-1.1/email_verification/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 	)
 	user = models.OneToOneField(User, on_delete=models.CASCADE)
 	date_created = models.DateTimeField(auto_now_add=True)
 	
 	@property
 	def has_expired(self):
 		delta = timezone.now() - self.date_created
-		# token expires in five minutes
-		return delta.seconds > 300
+		# token expires in a day
+		return delta.seconds > (24 * 60 * 60)
 	
 	def __str__(self):
 		return str(self.id)
 		
-		
+
```

### Comparing `django-email-certify-1.0/email_verification/templates/email_verification/mail.html` & `django-email-certify-1.1/email_verification/templates/email_verification/mail.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 </head>
 <body>
     <main>
     	<div class="wrapper">
 	        <p>Your registration process is almost done. Please confirm your email by clicking on the link below to finish signing up.</p>
 	        <p>Visit this <a href="{{ request.scheme }}://{{ request.get_host }}{% url 'verify_email:pre-login' token %}">link</a> to complete the process.</p>
 	       
-	        <p>This link will expire after 5 minutes.</p>
+	        <p>This link will expire after 24 hours.</p>
         </div>
     </main>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 
 
 Your registration process is almost done. Please confirm your email by clicking
 on the link below to finish signing up.
 Visit this link to complete the process.
-This link will expire after 5 minutes.
+This link will expire after 24 hours.
```

### Comparing `django-email-certify-1.0/email_verification/templates/email_verification/pre-login-failure.html` & `django-email-certify-1.1/email_verification/templates/email_verification/pre-login-failure.html`

 * *Files identical despite different names*

### Comparing `django-email-certify-1.0/email_verification/templates/email_verification/pre-login-success.html` & `django-email-certify-1.1/email_verification/templates/email_verification/pre-login-success.html`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,14 @@
         }
     </style>
 </head>
 <body>
     <main>
         <div class="wrapper">
             <div class="text">
-                <p>Your email has been verified. You can now visit the site to log in.</p>
+                <p>Your email has been verified. Click on the button below to login</p>
             </div>
             <a id="btn" href="{% url login_url %}">Login</a>
         </div>
     </main>
 </body>
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 
 
-Your email has been verified. You can now visit the site to log in.
+Your email has been verified. Click on the button below to login
 Login
```

### Comparing `django-email-certify-1.0/email_verification/views.py` & `django-email-certify-1.1/email_verification/views.py`

 * *Files identical despite different names*

### Comparing `django-email-certify-1.0/setup.cfg` & `django-email-certify-1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = django-email-certify
-version = 1.0
+version = 1.1
 description = A Django package to manage user email verification on registration
 long_description_content_type = text/markdown
 long_description = file: README.md
-url = https://github.com/codewitgabi/django-email-certify
+url = https://github.com/codewitgabi/email-verification-pkg
 author = Gabriel Michael Ojomakpene (codewitgabi)
 author_email = codewitgabi222@gmail.com
 license = MIT-License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
```

