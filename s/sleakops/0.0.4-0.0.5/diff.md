# Comparing `tmp/sleakops-0.0.4.tar.gz` & `tmp/sleakops-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleakops-0.0.4.tar", last modified: Wed Mar  1 17:40:43 2023, max compression
+gzip compressed data, was "sleakops-0.0.5.tar", last modified: Wed Jul  5 15:58:37 2023, max compression
```

## Comparing `sleakops-0.0.4.tar` & `sleakops-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 17:40:43.406558 sleakops-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 17:40:43.402558 sleakops-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 17:40:43.402558 sleakops-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-01 17:40:20.000000 sleakops-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-01 17:40:20.000000 sleakops-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-01 17:40:20.000000 sleakops-0.0.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-01 17:40:20.000000 sleakops-0.0.4/LONGDESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-01 17:40:43.406558 sleakops-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-01 17:40:20.000000 sleakops-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-01 17:40:20.000000 sleakops-0.0.4/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-01 17:40:20.000000 sleakops-0.0.4/local.env
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-01 17:40:20.000000 sleakops-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-01 17:40:20.000000 sleakops-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-01 17:40:43.406558 sleakops-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-01 17:40:20.000000 sleakops-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 17:40:43.402558 sleakops-0.0.4/sleakops/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 17:40:20.000000 sleakops-0.0.4/sleakops/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4236 2023-03-01 17:40:20.000000 sleakops-0.0.4/sleakops/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 17:40:43.406558 sleakops-0.0.4/sleakops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-01 17:40:43.000000 sleakops-0.0.4/sleakops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-01 17:40:43.000000 sleakops-0.0.4/sleakops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 17:40:43.000000 sleakops-0.0.4/sleakops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-01 17:40:43.000000 sleakops-0.0.4/sleakops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-01 17:40:43.000000 sleakops-0.0.4/sleakops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-01 17:40:43.000000 sleakops-0.0.4/sleakops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:58:37.885887 sleakops-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:58:37.881887 sleakops-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:58:37.885887 sleakops-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-05 15:58:11.000000 sleakops-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-05 15:58:11.000000 sleakops-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-05 15:58:11.000000 sleakops-0.0.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-05 15:58:11.000000 sleakops-0.0.5/LONGDESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 15:58:37.885887 sleakops-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 15:58:11.000000 sleakops-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-05 15:58:11.000000 sleakops-0.0.5/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 15:58:11.000000 sleakops-0.0.5/local.env
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 15:58:11.000000 sleakops-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 15:58:11.000000 sleakops-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-05 15:58:37.885887 sleakops-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 15:58:11.000000 sleakops-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:58:37.885887 sleakops-0.0.5/sleakops/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 15:58:11.000000 sleakops-0.0.5/sleakops/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-07-05 15:58:11.000000 sleakops-0.0.5/sleakops/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:58:37.885887 sleakops-0.0.5/sleakops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 15:58:37.000000 sleakops-0.0.5/sleakops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-05 15:58:37.000000 sleakops-0.0.5/sleakops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:58:37.000000 sleakops-0.0.5/sleakops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 15:58:37.000000 sleakops-0.0.5/sleakops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 15:58:37.000000 sleakops-0.0.5/sleakops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 15:58:37.000000 sleakops-0.0.5/sleakops.egg-info/top_level.txt
```

### Comparing `sleakops-0.0.4/.github/workflows/publish-to-pypi.yml` & `sleakops-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `sleakops-0.0.4/.gitignore` & `sleakops-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sleakops-0.0.4/PKG-INFO` & `sleakops-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleakops
-Version: 0.0.4
+Version: 0.0.5
 Summary: A CLI tool to build and deploy projects with Sleakops
 Project-URL: Documentation, https://docs.sleakops.com
 Project-URL: App page, https://sleakops.com
 Keywords: Sleakops
 Description-Content-Type: text/markdown
 
 # How to install
```

### Comparing `sleakops-0.0.4/sleakops/cli.py` & `sleakops-0.0.5/sleakops/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 def action(path, data, headers, wait):
     try:
         response = requests.post(path, json=data, headers=headers)
     except ConnectionError:
         click.echo(f"Could not reach {path}")
         sys.exit(1)
     if not response.ok:
-        result_message = response.json() if response.status_code == 400 else response.reason
+        result_message = (
+            response.json() if response.status_code == 400 else response.reason
+        )
         click.echo(f"Something went wrong: {result_message}")  # api key wrong
         sys.exit(1)
     elif wait:
         created = False
         retries = 0
         id = response.json()["id"]
         while not created and retries < MAX_POLLING:
@@ -71,75 +73,87 @@
 
 @cli_build.command()
 @click.option("-p", "--project", required=True, help="Project name.")
 @click.option("-b", "--branch", required=True, help="Repository branch.")
 @click.option("-c", "--commit", show_default=True, help="Commit.")
 @click.option("-t", "--tag", help="Tag for the image")
 @click.option(
+    "-prov", "--provider", required=False, show_default=True, help="Provider name"
+)
+@click.option(
     "-w",
     "--wait",
     is_flag=True,
     default=False,
     show_default=True,
     help="Run build and wait for it to finish.",
 )
 @click.option(
     "-k",
     "--key",
     envvar="SLEAKOPS_KEY",
     help="Sleakops access key. It can be used with this option or get from SLEAKOPS_KEY environment var.",
 )
-def build(project, branch, commit, tag, wait, key):
+def build(project, branch, commit, tag, provider, wait, key):
     path = f"{API_URL}cli-build/"
     headers = {"Authorization": f"Api-Key {key}"}
 
     data = {
         "project_env": {
             "project_name": project,
         },
         "branch": branch,
     }
     data.update({"commit": commit}) if commit else None
     data.update({"tag": tag}) if tag else None
 
+    if provider:
+        data.update({"provider": provider})
+
     action(path, data, headers, wait)
 
 
 @cli_deploy.command()
 @click.option("-p", "--project", required=True, help="Project name.")
 @click.option("-e", "--env", required=True, help="Environment.")
 @click.option("-b", "--build", required=False, help="Build id.")
 @click.option("-t", "--image", default="latest", show_default=True, help="Image tag.")
 @click.option(
+    "-prov", "--provider", required=False, show_default=True, help="Provider name"
+)
+@click.option(
     "-w",
     "--wait",
     is_flag=True,
     default=False,
     show_default=True,
     help="Run build and wait for it to finish.",
 )
 @click.option(
     "-k",
     "--key",
     envvar="SLEAKOPS_KEY",
     help="Sleakops access key. It can be used with this option or get from SLEAKOPS_KEY environment var.",
 )
-def deploy(project, env, build, image, wait, key):
+def deploy(project, env, build, image, provider, wait, key):
     path = f"{API_URL}cli-deployment/"
     headers = {"Authorization": f"Api-Key {key}"}
 
     data = {
         "project_env": {
             "project_name": project,
             "environment_name": env,
         }
     }
     data.update({"build": build}) if build else None
     data.update({"image": image}) if image else None
 
+    if provider:
+        data.update({"provider": provider})
+
     action(path, data, headers, wait)
 
 
 cli = click.CommandCollection(sources=[cli_build, cli_deploy])
 
 if __name__ == "__main__":
     cli()
```

### Comparing `sleakops-0.0.4/sleakops.egg-info/PKG-INFO` & `sleakops-0.0.5/sleakops.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleakops
-Version: 0.0.4
+Version: 0.0.5
 Summary: A CLI tool to build and deploy projects with Sleakops
 Project-URL: Documentation, https://docs.sleakops.com
 Project-URL: App page, https://sleakops.com
 Keywords: Sleakops
 Description-Content-Type: text/markdown
 
 # How to install
```

