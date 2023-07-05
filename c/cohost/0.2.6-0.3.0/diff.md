# Comparing `tmp/cohost-0.2.6.tar.gz` & `tmp/cohost-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohost-0.2.6.tar", last modified: Wed Apr 26 18:52:54 2023, max compression
+gzip compressed data, was "cohost-0.3.0.tar", last modified: Wed Jul  5 01:29:26 2023, max compression
```

## Comparing `cohost-0.2.6.tar` & `cohost-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.962380 cohost-0.2.6/
--rw-r--r--   0 valknight   (501) staff       (20)     1072 2023-04-26 18:15:22.000000 cohost-0.2.6/LICENSE
--rw-r--r--   0 valknight   (501) staff       (20)     6141 2023-04-26 18:52:54.961393 cohost-0.2.6/PKG-INFO
--rw-r--r--   0 valknight   (501) staff       (20)     3983 2023-04-26 18:15:22.000000 cohost-0.2.6/README.md
-drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.938357 cohost-0.2.6/cohost/
--rw-r--r--   0 valknight   (501) staff       (20)       99 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/__init__.py
-drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.957482 cohost-0.2.6/cohost/models/
--rw-r--r--   0 valknight   (501) staff       (20)       26 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/__init__.py
--rw-r--r--   0 valknight   (501) staff       (20)     4102 2023-04-26 18:49:55.000000 cohost-0.2.6/cohost/models/block.py
--rw-r--r--   0 valknight   (501) staff       (20)      411 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/comment.py
--rw-r--r--   0 valknight   (501) staff       (20)     8252 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/notification.py
--rw-r--r--   0 valknight   (501) staff       (20)     3822 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/post.py
--rw-r--r--   0 valknight   (501) staff       (20)    10506 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/project.py
--rw-r--r--   0 valknight   (501) staff       (20)     5432 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/models/user.py
--rw-r--r--   0 valknight   (501) staff       (20)     2967 2023-04-26 18:15:22.000000 cohost-0.2.6/cohost/network.py
-drwxr-xr-x   0 valknight   (501) staff       (20)        0 2023-04-26 18:52:54.943990 cohost-0.2.6/cohost.egg-info/
--rw-r--r--   0 valknight   (501) staff       (20)     6141 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/PKG-INFO
--rw-r--r--   0 valknight   (501) staff       (20)      391 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/SOURCES.txt
--rw-r--r--   0 valknight   (501) staff       (20)        1 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/dependency_links.txt
--rw-r--r--   0 valknight   (501) staff       (20)        9 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/requires.txt
--rw-r--r--   0 valknight   (501) staff       (20)        7 2023-04-26 18:52:54.000000 cohost-0.2.6/cohost.egg-info/top_level.txt
--rw-r--r--   0 valknight   (501) staff       (20)     1124 2023-04-26 18:51:57.000000 cohost-0.2.6/pyproject.toml
--rw-r--r--   0 valknight   (501) staff       (20)       38 2023-04-26 18:52:54.962794 cohost-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.798351 cohost-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 01:29:17.000000 cohost-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 01:29:26.798351 cohost-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-05 01:29:17.000000 cohost-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.794351 cohost-0.3.0/cohost/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.798351 cohost-0.3.0/cohost/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-05 01:29:17.000000 cohost-0.3.0/cohost/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:29:26.794351 cohost-0.3.0/cohost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 01:29:26.000000 cohost-0.3.0/cohost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-05 01:29:17.000000 cohost-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:29:26.798351 cohost-0.3.0/setup.cfg
```

### Comparing `cohost-0.2.6/LICENSE` & `cohost-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohost-0.2.6/PKG-INFO` & `cohost-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.2.6
+Version: 0.3.0
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
         
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cohost.py
 
 ![Edit of Eggbug into the python logo](pybug_small.png)
```

### Comparing `cohost-0.2.6/README.md` & `cohost-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cohost-0.2.6/cohost/models/block.py` & `cohost-0.3.0/cohost/models/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import requests
 
 from cohost.network import fetch, generate_login_cookies
 
 
 class Block:
-    """Posts are made up of blocks - think of each section of text, or an image - it's all blocks baybe!
+    """Posts are made up of blocks
+
+    Think of each section of text, or an image - it's all blocks baybe!
 
     To implement blocks, make subclasses of this!
     """
 
     def __init__(self) -> None:
         raise NotImplementedError('Base block is an abstract class')
 
@@ -32,27 +34,29 @@
             }
         }
 
 
 class AttachmentBlock(Block):
     """A block that contains an attachment"""
 
-    def __init__(self, filepath: str, attachment_id: str = None, alt_text=None) -> None:
+    def __init__(self, filepath: str,
+                 attachment_id: str = None, alt_text=None) -> None:
         try:
             with open(filepath, 'rb') as f:
                 f.read()
         except FileNotFoundError:
             raise FileNotFoundError(
-                'Attachment could not be found at: '.format(filepath))
+                'Attachment could not be found at: {}'.format(filepath))
         self.filepath = filepath
         self.filename = self.filepath.split('/')[-1]
         content_type = None
         if self.filename.lower().endswith('.webp'):
             content_type = 'image/webp'
-        elif self.filename.lower().endswith('.jpg') or self.filename.lower().endswith('.jpeg'):
+        elif (self.filename.lower().endswith('.jpg')
+              or self.filename.lower().endswith('.jpeg')):
             content_type = 'image/jpeg'
         elif self.filename.lower().endswith('.png'):
             content_type = 'image/png'
         elif self.filename.lower().endswith('.svg'):
             content_type = 'image/svg+xml'
         self.content_type = content_type
         with open(self.filepath, 'rb') as f:
@@ -71,40 +75,45 @@
             'attachment': {
                 'attachmentId': aid
             }
         }
         if self.alt_text:
             toReturn['attachment']['altText'] = self.alt_text
         return toReturn
-    
+
     def uploadIfNot(self, postId, project):
         if self.attachment_id is not None:
             return
-        # we don't have an attachment ID! that means this file isn't tied to a cohost file
-        # Step 1: tell cohost we're uploading a file, using project/v-dev/posts/53633/attach/start
+        # we don't have an attachment ID!
+        # that means this file isn't tied to a cohost file
+        # Step 1: tell cohost we're uploading a file
+        # we do this using project/{handle}/posts/53633/attach/start
         endpoint = 'project/{}/posts/{}/attach/start'.format(
             project.handle, postId)
 
-        # example data: filename=VxwLMgKF_400x400.jpg&content_type=image%2Fjpeg&content_length=20829
+        # example data: filename=foo.jpg&
+        #   content_type=image%2Fjpeg&content_length=20829
         dospacecreds = fetch('postjson', endpoint, {
             'filename': self.filename,
             'content_type': self.content_type,
             'content_length': int(self.content_length)
         }, generate_login_cookies(project.user.cookie))
-        # Step 2: ok sick, we now have digitalocean creds to upload the image to Spaces
-        # we need to use raw requests here, as we're not actually talking to cohost
+        # Step 2: digitalocean time
+        # we now have digitalocean creds to upload the image to Spaces
+        # we need to use raw requests here
+        # this is because we're not talking to Cohost
         spacesUrl = dospacecreds.get('url')
         b = None
         with open(self.filepath, 'rb') as f:
             b = f.read()
         spaceresp = requests.post(
             spacesUrl, data=dospacecreds.get('requiredFields'), files={
                 'file': (self.filename, b, self.content_type)
             })
         if spaceresp.status_code != 204:
             raise Exception('Error uploading to Spaces')
         # and now, tell cohost we're done!
         endpoint = 'project/{}/posts/{}/attach/finish/{}'.format(
             project.handle, postId, dospacecreds.get('attachmentId'))
-        a = fetch('post', endpoint, {}, generate_login_cookies(
+        fetch('post', endpoint, {}, generate_login_cookies(
             project.user.cookie))  # Will indicate we're done!
         self.attachment_id = dospacecreds.get('attachmentId')
```

### Comparing `cohost-0.2.6/cohost/models/notification.py` & `cohost-0.3.0/cohost/models/notification.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,90 @@
         self.createdAt = createdAt
         self.fromProject = fromProject
 
     @property
     def timestamp(self):
         return self.createdAt
 
+
 class Like(BaseNotification):
     def __init__(self, createdAt, fromProject, toPost, relationshipId):
         super().__init__(createdAt, fromProject)
         self.toPost = toPost
         self.relationshipId = relationshipId
-    
+
     def __str__(self) -> str:
-        return "{} liked {} | {}".format(self.fromProject.handle, self.toPost.postId, self.timestamp)
+        return "{} liked {} | {}".format(
+            self.fromProject.handle,
+            self.toPost.postId,
+            self.timestamp
+        )
 
 
 class Share(BaseNotification):
-    def __init__(self, createdAt, fromProject, toPost, sharePost, transparentShare):
+    def __init__(self, createdAt, fromProject,
+                 toPost, sharePost, transparentShare):
         super().__init__(createdAt, fromProject)
         self.toPost = toPost
         self.sharePost = sharePost
         self.transparentShare = transparentShare
-    
+
     def __str__(self) -> str:
         if self.transparentShare:
-            return "{} shared {} with extra | {}".format(self.fromProject.handle, self.toPost.postId, self.timestamp)
-        return "{} shared {} | {}".format(self.fromProject.handle, self.toPost.postId, self.timestamp)
+            return "{} shared {} with extra | {}".format(
+                self.fromProject.handle,
+                self.toPost.postId,
+                self.timestamp
+            )
+        return "{} shared {} | {}".format(
+            self.fromProject.handle,
+            self.toPost.postId,
+            self.timestamp
+        )
 
 
 class Comment(BaseNotification):
     def __init__(self, createdAt, fromProject, toPost, comment, inReplyTo):
         super().__init__(createdAt, fromProject)
         self.toPost = toPost
         self.comment = comment
         self.inReplyTo = inReplyTo
 
     def __str__(self) -> str:
-        if self.toPost == None:
-            return "{} commented on [post that couldn't be retrieved] - \"{}\" | {}".format(self.fromProject.handle, self.comment.body, self.timestamp)
-        return "{} commented on {} - \"{}\" | {}".format(self.fromProject.handle, self.toPost.postId, self.comment.body, self.timestamp)
+        if self.toPost is None:
+            return (f"{self.fromProject.handle} commented on " +
+                    + "[post that couldn't be retrieved]- " +
+                    f"\"{self.comment.body}\" | {self.timestamp}")
+        return "{} commented on {} - \"{}\" | {}".format(
+            self.fromProject.handle,
+            self.toPost.postId,
+            self.comment.body,
+            self.timestamp
+        )
+
 
 class Follow(BaseNotification):
     def __init__(self, createdAt, fromProject):
         super().__init__(createdAt, fromProject)
-    
+
     def __str__(self) -> str:
-        return "{} is now following you | {}".format(self.fromProject.handle, self.timestamp)
+        return "{} is now following you | {}".format(
+            self.fromProject.handle,
+            self.timestamp
+        )
+
 
 """Unwrap a raw notification list's grouped notifications
+
+
+    Returns:
+        list: unwrapped notification list
 """
+
+
 def unwrapGroupedNotifications(notificationsRaw: dict):
     unwrapped = []
     # Unwrap any grouped notifications
     for notif in notificationsRaw:
         if not notif['type'].startswith('grouped'):
             unwrapped.append(notif)
             continue
@@ -74,22 +106,24 @@
                 'relationshipId': relationshipId,
                 'sharePostId': sharePostId,
                 'createdAt': notif['createdAt'],
                 'transparentShare': notif.get('transparentShare', None)
             })
     return unwrapped
 
+
 def buildFromNotifList(notificationsApiResp: dict, user):
     from cohost.models.comment import Comment as CommentModel
-    from cohost.models.post import Post
-    from cohost.models.user import User
+    from cohost.models.post import Post  # noqa: F401
+    from cohost.models.user import User  # noqa: F401
     u = user  # type: User
-    user = u  # this whole shitshow is to get intellisense working without circular imports
+    user = u  # this gets intellisense working without circular imports
     # I Love Python
-    # We need the user to do API operations upon - it helps us resolve things like projects!
+    # We need the user to do API operations upon
+    # It helps us resolve things like projects!
     commentsRaw = notificationsApiResp.get('comments')
     postsRaw = notificationsApiResp.get('posts')
     projectsRaw = notificationsApiResp.get('projects')
     notificationsRaw = notificationsApiResp.get('notifications')
     # Ok, so, now we HAVE all of this, we can build the notifications
     # First step: projects
     projects = []
@@ -123,27 +157,30 @@
             for n in comments:
                 if n.id == nextNotif['comment']['inReplyTo']:
                     found = True
                     replyComment = n
                     break
             # we still have other notifications to be processed
             nextNotif['attemptsToProcess'] += 1
-            if not found and len(commentQueue) > 0 and not(nextNotif['attemptsToProcess'] > 50):
+            if (not found and len(commentQueue) > 0
+                    and (not nextNotif['attemptsToProcess'] > 50)):
                 commentQueue.append(nextNotif)
                 continue
-        # Ok, sick, so, we either don't have a reply, or we do but it's already processed!
+        # Ok, sick, so, we either don't have a reply
+        # ... or we do but it's already processed!
         # we need pull the Project for this comment
         posterProject = None
         for project in projects:
             if project.projectId == nextNotif['poster']['projectId']:
                 posterProject = project
         c = CommentModel(nextNotif['canEdit'], nextNotif['canInteract'],
                          nextNotif, posterProject, user, replyComment)
         comments.append(c)
-    # Unwrap grouped notifications - a "grouped" notif will cause breaking behaviour to older tools
+    # Unwrap grouped notifications
+    # a "grouped" notif will cause breaking behaviour to older tools
     notificationsRaw = unwrapGroupedNotifications(notificationsRaw)
     # and NOW we can finally map our notifications to all of our data models
     # TODO: Build notification model
     notifications = []
     for notification in notificationsRaw:
         # first, let's resolve all the data back
         fromProject = None
@@ -174,18 +211,40 @@
         if notification.get('inReplyToId'):
             for c in comments:
                 if c.id == notification['inReplyToId']:
                     inReplyTo = c
                     break
         # sick, we can now handle whichever type of notification this is
         if notification['type'] == 'like':
-            notifications.append(Like(
-                notification['createdAt'], fromProject, toPost, notification['relationshipId']))
+            notifications.append(
+                Like(
+                    notification['createdAt'],
+                    fromProject,
+                    toPost,
+                    notification['relationshipId']
+                )
+            )
         if notification['type'] == "share":
-            notifications.append(Share(
-                notification['createdAt'], fromProject, toPost, sharePost, notification['transparentShare']))
+            notifications.append(
+                Share(
+                    notification['createdAt'],
+                    fromProject,
+                    toPost,
+                    sharePost,
+                    notification['transparentShare']
+                )
+            )
         if notification['type'] == "comment":
             notifications.append(
-                Comment(notification['createdAt'], fromProject, toPost, comment, inReplyTo))
+                Comment(
+                    notification['createdAt'],
+                    fromProject,
+                    toPost,
+                    comment,
+                    inReplyTo
+                )
+            )
         if notification['type'] == 'follow':
-            notifications.append(Follow(notification['createdAt'], fromProject))
+            notifications.append(
+                Follow(notification['createdAt'], fromProject)
+            )
     return notifications
```

### Comparing `cohost-0.2.6/cohost/models/post.py` & `cohost-0.3.0/cohost/models/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 class Post:
     def __init__(self, postData, project):
         # we do this here to help autosuggest figure out what project is
-        from cohost.models.project import Project
+        from cohost.models.project import Project  # noqa: F401
         self.postData = postData
         self.project = project  # type: Project
 
     def __str__(self) -> str:
         return "{}".format(self.filename)
-    
-    def edit(self, headline: str, blocks: list = [], cws: list = [], tags: list = [], adult: bool = False, draft = False):
+
+    def edit(self, headline: str, blocks: list = [], cws: list = [],
+             tags: list = [], adult: bool = False, draft=False):
         from cohost.models.project import EditableProject
         if type(self.project) != EditableProject:
-            raise AttributeError("Post isn't attached to an EditableProject - do you have Edit permissions for this post?")
-        return self.project.editPost(self.postId, headline=headline, blocks=blocks, cws=cws, tags=tags, adult=adult, draft=draft)
+            raise AttributeError("Post isn't attached to an EditableProject -\
+                                 do you have Edit permissions for this post?")
+        return self.project.editPost(
+            self.postId,
+            headline=headline,
+            blocks=blocks,
+            cws=cws,
+            tags=tags,
+            adult=adult,
+            draft=draft
+        )
 
     @property
     def postId(self):
         return self.postData['postId']
 
     @property
     def headline(self):
@@ -50,16 +60,16 @@
     def contentWarnings(self) -> list:
         return self.postData['cws']
 
     @property
     def tags(self) -> list:
         return self.postData['tags']
 
-    """Build 
-    
+    """Build
+
     Returns:
         list[str]: Return a list of blocks that make up a post
     """
     @property
     def blocks(self) -> list:
         return self.postData['blocks']
 
@@ -75,15 +85,15 @@
         else:
             newProject = self.postData['postingProject']
         return self.project.user.resolveSecondaryProject(newProject)
 
     @property
     def shareTree(self):
         return self.postData['shareTree']
-    
+
     @property
     def relatedProjects(self) -> list:
         projects = []
         for p in self.postData['relatedProjects']:
             projects.append(self.project.user.resolveSecondaryProject(p))
         return projects
 
@@ -93,16 +103,15 @@
 
     @property
     def adult(self) -> bool:
         return self.postData['effectiveAdultContent']
 
     @property
     def contributorBlock(self) -> bool:
-        # i haven't blocked anyone or been blocked (i think) so idk how this works
-        # anyone who gets blocekd a lot pls test this
+        # NOTE: This is still untested as I'm still not sure how blocks work
         return self.postData['contributorBlockIncomingOrOutgoing']
 
     @property
     def hasAnyContributorMuted(self) -> bool:
         return self.postData['hasAnyContributorMuted']
 
     @property
```

### Comparing `cohost-0.2.6/cohost/models/project.py` & `cohost-0.3.0/cohost/models/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from cohost.models.block import AttachmentBlock
 from cohost.models.post import Post
 from cohost.network import fetch, generate_login_cookies, fetchTrpc
 
-# from cohost.models.user import User
-
 
 class Project:
     def __init__(self, user, data):
-        from cohost.models.user import User
+        # this helps editors understand what we're setting
+        from cohost.models.user import User  # noqa: F401
         self.user = user  # type: User
         # we can't specify this type globally due to all kinds of import errors
         # but that gives us our login chain back, if that makes sense!
         self.projectId = data['projectId']
         self.data = data
         if self.projectInfo is None:
             raise AttributeError("Project not found")
@@ -66,54 +65,64 @@
     @property
     def avatarShape(self) -> str:
         return self.projectInfo['avatarShape']
 
     @property
     def projectInfo(self) -> str:
         return self.data
-    
+
     @property
     def atomFeed(self) -> str:
-        # TODO: This is a bad assumption, and cohost gives us a rel= link we should use instead
+        # TODO: This is a bad assumption
+        # Cohost gives us a rel=link we should use instead
         # However, to get this exposed in our API asap, this works
         return "https://cohost.org/{}/rss/public.atom".format(self.handle)
 
     @property
     def rssFeed(self) -> str:
         # Cohost's feeds aren't "RSS" but actually the atom format
-        # Most RSS readers will just call this RSS though, so, you *should* be fine but it's good to note the difference & technicality
-        # See for more information: http://www.intertwingly.net/wiki/pie/Rss20AndAtom10Compared
+        # Most RSS readers will just call this RSS though
+        # As such, you *should* be fine
+        # But! it's good to note the difference & technicality
+        # See for more information
+        # http://www.intertwingly.net/wiki/pie/Rss20AndAtom10Compared
         return self.atomFeed
 
     @property
     def jsonFeed(self) -> str:
         # See above note in relation to the rssFeed method
         return "https://cohost.org/{}/rss/public.json".format(self.handle)
-    
 
     def getPostsRaw(self, page=0):
         return fetch('get',
                      '/project/{}/posts?page={}'.format(self.handle, page),
                      None,
                      generate_login_cookies(self.user.cookie))
 
     def getPosts(self, page=0) -> list:
         postData = self.getPostsRaw(page)
         posts = []
         for post in postData['items']:
             posts.append(Post(post, self))
         return posts
 
-
-"""Project but using live API data, instead of prefilled data. Intended for use in editable projects!"""
+    def ask(self, content, sourceProject, anon=False):
+        from cohost.models.project import EditableProject
+        if type(sourceProject) != EditableProject:
+            raise TypeError("sourceProject must be an editable project")
+        sourceProject = sourceProject  # EditableProject
+        fetchTrpc('asks.send', sourceProject.user.cookie, {
+            "toProjectHandle": self.handle,
+            "content": content,
+            "anon": anon}, methodType='postjson')
 
 
 class EditableProject(Project):
     def __init__(self, user, projectId):
-        from cohost.models.user import User
+        from cohost.models.user import User  # noqa: F401
         self.user = user  # type: User
         # we can't specify this type globally due to all kinds of import errors
         # but that gives us our login chain back, if that makes sense!
         self.projectId = projectId
         if self.projectInfo is None:
             raise AttributeError("Project not found")
 
@@ -121,15 +130,16 @@
     def projectInfo(self) -> str:
         projects = self.user.editedProjectsRaw
         for project in projects:
             if project['projectId'] == self.projectId:
                 return project
         return None
 
-    def post(self, headline: str, blocks: list = [], cws: list = [], tags: list = [], adult: bool = False, draft = False):
+    def post(self, headline: str, blocks: list = [], cws: list = [],
+             tags: list = [], adult: bool = False, draft=False):
         # Basic flow: you send a POST to project/{handle}/posts
         # This gives us back a post ID, as well as a API link
         # For example:
         """
         {
         "postId": 53648,
         "_links": [
@@ -137,138 +147,172 @@
             "href": "/api/v1/project_posts/53648",
             "rel": "post",
             "type": "GET"
             }
         ]
         }
         """
-        # Then, if you have images, upload then by sending data *about* the image to project/{handle}/posts/{postId}/attach/start
+        # Then, if you have images:
+        # Upload them by sending data *about* the image to
+        #   project/{handle}/posts/{postId}/attach/start
         # This will respond back with something like...
         """
         {
-            "attachmentId": "25ecb155-9937-4b87-b1b3-bd70a6be3bbc",
+            "attachmentId": "yourattachmentid",
             "url": "https://sfo3.digitaloceanspaces.com/redcent-dev",
             "requiredFields": {
                 "acl": "public-read",
                 "Content-Type": "image/webp",
                 "Content-Disposition": "inline",
                 "Cache-Control": "max-age=31536000",
-                "key": "attachment/25ecb155-9937-4b87-b1b3-bd70a6be3bbc/SleepFaceIcon.webp",
+                "key": "attachment/yourattachmentid/foo.webp",
                 "bucket": "redcent-dev",
                 "X-Amz-Algorithm": "...",
                 "X-Amz-Credential": "...",
                 "X-Amz-Date": "20220716T110215Z",
                 "Policy": "...",
                 "X-Amz-Signature": "..."
         }
         """
         # We can THEN send the image to DO spaces, using the credentials
-        # Once this is uploaded, we can tell cohost the upload is finished by sending another POST to project/{handle}/posts/{id}/attach/finish/{attachmentId}
-        # after ALL of this we sent a PUT (what a change) request to project/{handle}/posts/{postId}
-        # the body of this is the same as what we initially POST'd, but, now, we replace the initial blank attachmentId with the corresponding one back. The only catch is change postState to 1, instead of zero
-        # (postState refers to if the post should be public - if it is zero, it will only exist as a draft)
-        # TODO: Implement the image upload stuff within AttachmentBlock - it should handle all of this
-        # For now though, we'll just send the initial post as that's good enough for text!
+        # Once this is uploaded, we can tell cohost the upload is finished
+        # We do this by sending another POST to the following URL:
+        #   project/{handle}/posts/{id}/attach/finish/{attachmentId}
+        # After ALL of this we sent a PUT (what a change) request to:
+        #   project/{handle}/posts/{postId}
+        # the body of this is the same as what we initially POST'd, but -
+        # now, we replace the blank attachmentId
+        # We do this with the corresponding one we got back
+        # The only catch is change postState to 1, instead of zero
+        # postState refers to if the post should be public
+        # if it is zero, it will only exist as a draft
         blockL = []
         attachments = []
         for b in blocks:
             if type(b) is AttachmentBlock:
-                attachments.append(b) # type: AttachmentBlock
+                attachments.append(b)  # type: AttachmentBlock
             else:
                 blockL.append(b.dict)
-        
+
         for attachment in attachments:
             blockL.insert(0, attachment.dict)
         postData = {
-            'postState': int(not(draft) and (len(attachments) == 0)),
+            'postState': int((not draft) and (len(attachments) == 0)),
             'headline': headline,
             'adultContent': adult,
             'blocks': blockL,
             'cws': cws,
             'tags': tags
         }
-        req = fetch('postJSON', '/project/{}/posts'.format(self.handle), postData,
-                    generate_login_cookies(self.user.cookie))
-        if len(attachments) == 0 and not(draft):
+        req = fetch(
+            'postJSON',
+            '/project/{}/posts'.format(self.handle),
+            postData,
+            generate_login_cookies(self.user.cookie)
+        )
+        if len(attachments) == 0 and (not draft):
             return self.getPosts()[0]  # this will be what we just posted
         if len(attachments) == 0:
-            return None # TODO: Get drafts working!
+            return None  # TODO: Get drafts working!
         # OK so, we can now feed each attachment block our post ID
         for attachment in attachments:
             attachment.uploadIfNot(req['postId'], self)
-        # Sick! Everything is uploaded - we can now rebuild the post data and send it back to cohost
+        # Sick! Everything is uploaded
+        # We can now rebuild the post data and send it back to cohost
         blockL = []
         for b in blocks:
             blockL.append(b.dict)
         postData = {
-            'postState': int(not(draft)),
+            'postState': int(not draft),
             'headline': headline,
             'adultContent': adult,
             'blocks': blockL,
             'cws': cws,
             'tags': tags
         }
-        req = fetch('put', '/project/{}/posts/{}'.format(self.handle, req['postId']), postData,
-                    generate_login_cookies(self.user.cookie))
+        req = fetch(
+            'put',
+            '/project/{}/posts/{}'.format(self.handle, req['postId']),
+            postData,
+            generate_login_cookies(self.user.cookie)
+        )
         if not draft:
             return self.getPosts()[0]  # this will be what we just posted
-        return None # TODO: Get drafts working!
+        return None  # TODO: Get drafts working!
 
-    def editPost(self, postId: int, headline: str, blocks: list, cws: list = [], tags: list = [], adult: bool = False, draft = False):
-        # same thing as post() but initial request is a PUT to project/{handle}/posts/{postId}
+    def editPost(self, postId: int,
+                 headline: str, blocks: list,
+                 cws: list = [], tags: list = [],
+                 adult: bool = False, draft=False):
+        # same thing as post() but -
+        # initial request is a PUT to project/{handle}/posts/{postId}
 
         blockL = []
         attachments = []
         for b in blocks:
             if type(b) is AttachmentBlock:
-                attachments.append(b) # type: AttachmentBlock
+                attachments.append(b)  # type: AttachmentBlock
             else:
                 blockL.append(b.dict)
-        
+
         for attachment in attachments:
             blockL.insert(0, attachment.dict)
         postData = {
-            'postState': int(not(draft) and (len(attachments) == 0)),
+            'postState': int((not draft) and (len(attachments) == 0)),
             'headline': headline,
             'adultContent': adult,
             'blocks': blockL,
             'cws': cws,
             'tags': tags
         }
-        req = fetch('put', '/project/{}/posts/{}'.format(self.handle, postId), postData,
-                    generate_login_cookies(self.user.cookie))
-        if len(attachments) == 0 and not(draft):
+        req = fetch(
+            'put',
+            '/project/{}/posts/{}'.format(self.handle, postId),
+            postData,
+            generate_login_cookies(self.user.cookie)
+        )
+        if len(attachments) == 0 and (not draft):
             return self.getPosts()[0]  # this will be what we just posted
         if len(attachments) == 0:
-            return None # TODO: Get drafts working!
+            return None  # TODO: Get drafts working!
         # OK so, we can now feed each attachment block our post ID
         for attachment in attachments:
             attachment.uploadIfNot(postId, self)
-        # Sick! Everything is uploaded - we can now rebuild the post data and send it back to cohost
+        # Sick! Everything is uploaded
+        # We can now rebuild the post data and send it back to Cohost
         blockL = []
         for b in blocks:
             blockL.append(b.dict)
         postData = {
-            'postState': int(not(draft)),
+            'postState': int(not draft),
             'headline': headline,
             'adultContent': adult,
             'blocks': blockL,
             'cws': cws,
             'tags': tags
         }
-        req = fetch('put', '/project/{}/posts/{}'.format(self.handle, req['postId']), postData,
-                    generate_login_cookies(self.user.cookie))
+        req = fetch(
+            'put',
+            '/project/{}/posts/{}'.format(self.handle, req['postId']),
+            postData,
+            generate_login_cookies(self.user.cookie)
+        )
         if not draft:
             return self.getPosts()[0]  # this will be what we just posted
-        return None # TODO: Get drafts working!
-    
-    """Set this project as the default project, for actions such as retrieving notifications
+        return None  # TODO: Get drafts working!
+
+    """Set this project as the default project
+    This applies for actions such as retrieving notifications
     """
     def switch(self):
         fetchTrpc('projects.switchProject', self.user.cookie, {
-            "projectId":self.projectId
+            "projectId": self.projectId
         }, methodType="postjson")
-    
+
     @staticmethod
-    def create(user, projectName, private: bool = False, adult: bool = False) -> Project:
-        raise NotImplemented(
-            "Can be technically implemented, but I'm choosing not to to respect cohost. I don't want bots creating tons of pages and handles to be easy to build. Sorry!")
+    def create(user, projectName, private: bool = False,
+               adult: bool = False) -> Project:
+        raise NotImplementedError(
+            """Can be technically implemented, however -
+            I'm choosing not to to respect cohost.
+            I don't want bots creating tons of pages and handles.
+            Sorry!""")
```

### Comparing `cohost-0.2.6/cohost/models/user.py` & `cohost-0.3.0/cohost/models/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,37 +39,38 @@
         return EditableProject(self, self.userInfo['projectId'])
 
     @property
     def userInfo(self) -> dict:
         return fetchTrpc('login.loggedIn', self.cookie)['result']['data']
 
     """Fetch data from the API about projets the user can edit
-    
+
     Returns:
         dict: Project dictionaries
     """
     @property
     def editedProjectsRaw(self) -> dict:
-        return fetchTrpc('projects.listEditedProjects', self.cookie)['result']['data']['projects']
+        rawResp = fetchTrpc('projects.listEditedProjects', self.cookie)
+        return rawResp['result']['data']['projects']
 
     """Fetch data from the API about projects the user can edit
-    
+
     Returns:
         list[Project]: Project objects
     """
     @property
     def editedProjects(self) -> list:
         rawP = self.editedProjectsRaw
         projects = []
         for project in rawP:
             projects.append(EditableProject(self, project['projectId']))
         return projects
 
     """Get a salt for an email - for use in logging in
-    
+
 
     Returns:
         str: Base64 encoded salt
     """
     @staticmethod
     def getSalt(email):
 
@@ -81,99 +82,91 @@
         return salt
 
     """Create a user object from a login and password"""
     @staticmethod
     def login(email, password):
         # base64 terribleness
         salt = fetch("GET", "/login/salt", {"email": email})['salt']
-        # explanation for whatever this is by @iliana - https://cohost.org/iliana/post/180187-eggbug-rs-v0-1-3-d
+        # explanation for whatever this is by @iliana
+        # https://cohost.org/iliana/post/180187-eggbug-rs-v0-1-3-d
         salt = salt.replace('-', 'A')
         salt = salt.replace('_', 'A')
         salt = salt + "=="
 
         saltDecoded = base64.b64decode(salt.encode("ascii"))
 
         # generating the hash
-        hash = pbkdf2_hmac("sha384", password.encode("utf-8"), saltDecoded, 200000, 128)
+        # the 200000 is the magic iter number - Use This, or login will break
+        hash = pbkdf2_hmac("sha384", password.encode("utf-8"), saltDecoded,
+                           200000, 128)
         clientHash = base64.b64encode(hash).decode("ascii")
 
         # getting cookie
-        res = fetch("POST", "/login", {"email": email, "clientHash": clientHash}, complex=True) 
-        sessionCookie = res['headers']['set-cookie'].split(";")[0].split("=")[1]
-        
+        res = fetch("POST", "/login",
+                    {"email": email, "clientHash": clientHash}, complex=True)
+        sessionCookie = (res['headers']['set-cookie'].
+                         split(";")[0].split("=")[1])
+
         u = User(sessionCookie)
         # if no error we're good
         u.userInfo
         return u
 
-
     """Create a user object from a cookie"""
     @staticmethod
     def loginWithCookie(cookie):
         # First, let's create a user
         u = User(cookie)
-        # Now, we need to validate functions are working - we can do this by getting the user's info
+        # Now, we need to validate functions are working
+        # We can do this by getting the user's info
         u.userInfo
         # If this didn't error out, we're good!
         return u
 
     def getProject(self, handle: str) -> EditableProject:
         # Retrieve a project that you can edit
         projects = self.editedProjects
         for project in projects:
             if project.handle == handle:
                 return project
         return None
 
     def resolveSecondaryProject(self, projectData):
-        from cohost.models.project import EditableProject, Project
+        from cohost.models.project import Project
         editableProjects = self.editedProjects
         for project in editableProjects:
             if project.projectId == projectData['projectId']:
                 return project  # type: EditableProject
         return Project(self, projectData)  # type: Project
 
     @property
     def notifications(self):
-        return self.notificationsPagified(notificationsPerPage = 10)
-    
+        return self.notificationsPagified(notificationsPerPage=10)
+
     @property
     def allNotifications(self):
         page = 0
         notifsPerPage = 100
-        notifs = self.notificationsPagified(page = page, notificationsPerPage = notifsPerPage)
+        notifs = self.notificationsPagified(
+            page=page,
+            notificationsPerPage=notifsPerPage
+        )
         newNotifs = notifs
         while len(newNotifs) == notifsPerPage:
             page += 1
-            newNotifs = self.notificationsPagified(page = page, notificationsPerPage = notifsPerPage)
+            newNotifs = self.notificationsPagified(
+                page=page,
+                notificationsPerPage=notifsPerPage
+            )
             for n in newNotifs:
                 notifs.append(n)
         return notifs
-    
-    def notificationsPagified(self, page = 0, notificationsPerPage = 10):
+
+    def notificationsPagified(self, page=0, notificationsPerPage=10):
         nJson = self.notificationsRaw(page, notificationsPerPage)
         return buildFromNotifList(nJson, self)
-    
-    def notificationsRaw(self, page = 0, notificationsPerPage = 10):
+
+    def notificationsRaw(self, page=0, notificationsPerPage=10):
         return fetch('GET', 'notifications/list', {
             'offset': page * notificationsPerPage,
             'limit': notificationsPerPage
         }, generate_login_cookies(self.cookie))
-
-"""
-
-def getProjects() {
-    return (await fetch(
-        "GET",
-        "/projects/edited",
-        this.sessionCookie
-    )).projects.map(x => new Project(this, x));
-}
-
-def getNotifications(offset = 0, limit = 20):
-    return (await fetch(
-        "GET",
-        "/notifications/list",
-        this.sessionCookie,
-        { offset, limit }
-    ))
-"""
```

### Comparing `cohost-0.2.6/cohost/network.py` & `cohost-0.3.0/cohost/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import time
-
+import json.decoder
 import requests
 
-l = logging.getLogger(__name__)
-l.setLevel(logging.DEBUG)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
 API_BASE = "https://cohost.org/api/v1"
 
 cache = {}
 
 headers = {
     'User-Agent': 'cohost.py'
 }
@@ -31,81 +31,87 @@
 
     Returns:
         _type_: _description_
     """
     if not endpoint.startswith('/'):
         endpoint = "/" + endpoint
     url = API_BASE + endpoint
-    l.debug('{} to {}'.format(method, url))
+    logger.debug('{} to {}'.format(method, url))
     if method.lower() == "get":
         req = requests.get(url, cookies=cookies, params=data, headers=headers)
     elif method.lower() == "post":
         req = requests.post(url, cookies=cookies, data=data, headers=headers)
     elif method.lower() == 'postjson':
         req = requests.post(url, cookies=cookies, json=data, headers=headers)
     elif method.lower() == 'put':
         req = requests.put(url, cookies=cookies, json=data, headers=headers)
     else:
-        l.error('No such method handled: ' + method)
-        l.error('Defaulting to get')
+        logger.error('No such method handled: ' + method)
+        logger.error('Defaulting to get')
         return fetch("GET", endpoint, data, cookies, complex)
 
     try:
         res = req.json()
-    except:
+    except json.decoder.JSONDecodeError:
         res = req.text
 
     if (req.status_code >= 400 and method != 'put'):
         raise Exception(res)
     if complex:
         return {
             'headers': req.headers,
             'body': res
         }
     return res
 
 
-def fetchTrpc(methods: list, cookie: str, data: dict = None, methodType = "get"):
+def fetchTrpc(methods: list, cookie: str,
+              data: dict = None, methodType="get"):
     global cache
     """Fetch data from trpc API
 
     Args:
         methods (list): List of data points to retrieve
         cookie (str): Cookie of the user to retrieve from
 
     Returns:
         _type_: JSON encoded list from the trpc endpoint
     """
     if type(methods == str):
         m = methods
     else:
         m = ','.join(methods)
-    cacheData = get_cache_data(cookie, m)
-    if cacheData is not None:
-        l.debug('Cache hit!')
-        return cacheData
+    if methodType == "get":
+        cacheData = get_cache_data(cookie, m)
+        if cacheData is not None:
+            logger.debug('Cache hit!')
+            return cacheData
     data = fetch(methodType, "/trpc/{}".format(m), data=data,
                  cookies=generate_login_cookies(cookie))
-    set_cache_data(cookie, m, data)
+    if methodType == "get":
+        set_cache_data(cookie, m, data)
     return data
 
+
 # Caching utils !
 def set_cache_data(cookie, key, data):
     if cache.get(cookie, None) is None:
         cache[cookie] = {}
     cache[cookie][key] = {
         'data': data,
         'time': time.time()
     }
 
+
 def get_cache_data(cookie, key):
     entry = cache.get(cookie, {}).get(key, None)
     if entry is None:
         return None
     if time.time() - entry['time'] > timeout:
         return None
     return entry['data']
 
+
 def generate_login_cookies(cookie):
     return {
         'connect.sid': cookie
     }
```

### Comparing `cohost-0.2.6/cohost.egg-info/PKG-INFO` & `cohost-0.3.0/cohost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohost
-Version: 0.2.6
+Version: 0.3.0
 Summary: Unofficial Python API wrapper for Cohost.org - the fourth website!
 Author-email: Val Knight <val@valknight.xyz>
 Maintainer-email: Val Knight <val@valknight.xyz>
 License: MIT License
         
         Copyright (c) 2022 Vallerie Knight
         
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cohost.py
 
 ![Edit of Eggbug into the python logo](pybug_small.png)
```

### Comparing `cohost-0.2.6/pyproject.toml` & `cohost-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cohost"
-version = "0.2.6"
+version = "0.3.0"
 description = "Unofficial Python API wrapper for Cohost.org - the fourth website!"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = [ "cohost.org", "cohost", "api" ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
```

