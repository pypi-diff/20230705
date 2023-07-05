# Comparing `tmp/dimsdk-0.8.5.tar.gz` & `tmp/dimsdk-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimsdk-0.8.5.tar", last modified: Wed Jun  7 17:03:46 2023, max compression
+gzip compressed data, was "dist/dimsdk-0.8.6.tar", last modified: Wed Jul  5 17:43:50 2023, max compression
```

## Comparing `dimsdk-0.8.5.tar` & `dimsdk-0.8.6.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-06-07 17:03:46.000000 dimsdk-0.8.5/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-0.8.5/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk/
--rw-r--r--   0 moky       (501) staff       (20)     5866 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3727 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2278 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2354 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/array.py
--rw-r--r--   0 moky       (501) staff       (20)     2887 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3608 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     4547 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/customized.py
--rw-r--r--   0 moky       (501) staff       (20)     4059 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4706 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/cpu/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     2490 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/forward.py
--rw-r--r--   0 moky       (501) staff       (20)     3283 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/cpu/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     2415 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     8342 2023-06-02 04:25:14.000000 dimsdk-0.8.5/dimsdk/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8548 2023-06-02 04:28:45.000000 dimsdk-0.8.5/dimsdk/factories.py
--rw-r--r--   0 moky       (501) staff       (20)     2013 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     6701 2023-06-02 04:55:12.000000 dimsdk-0.8.5/dimsdk/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     2263 2022-12-12 09:59:21.000000 dimsdk-0.8.5/dimsdk/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1965 2023-06-01 18:23:20.000000 dimsdk-0.8.5/dimsdk/mkm/robot.py
--rw-r--r--   0 moky       (501) staff       (20)     4672 2022-12-11 05:05:26.000000 dimsdk-0.8.5/dimsdk/mkm/roles.py
--rw-r--r--   0 moky       (501) staff       (20)     6579 2023-06-01 18:25:38.000000 dimsdk-0.8.5/dimsdk/mkm/station.py
--rw-r--r--   0 moky       (501) staff       (20)     9854 2023-06-02 04:46:51.000000 dimsdk-0.8.5/dimsdk/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     3503 2023-01-31 05:24:56.000000 dimsdk-0.8.5/dimsdk/proc_content.py
--rw-r--r--   0 moky       (501) staff       (20)     7030 2023-06-02 04:52:26.000000 dimsdk-0.8.5/dimsdk/processor.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      635 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       37 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        7 2023-06-07 17:03:46.000000 dimsdk-0.8.5/dimsdk.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-07 17:03:46.000000 dimsdk-0.8.5/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1256 2023-06-01 17:05:35.000000 dimsdk-0.8.5/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2023-07-05 17:43:50.000000 dimsdk-0.8.6/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-0.8.6/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk/
+-rw-r--r--   0 moky       (501) staff       (20)     6206 2023-07-05 16:09:04.000000 dimsdk-0.8.6/dimsdk/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3727 2023-01-31 05:24:56.000000 dimsdk-0.8.6/dimsdk/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2669 2023-07-05 15:27:52.000000 dimsdk-0.8.6/dimsdk/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5610 2023-07-05 13:32:09.000000 dimsdk-0.8.6/dimsdk/cpu/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     7267 2023-07-05 15:12:46.000000 dimsdk-0.8.6/dimsdk/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     3404 2023-07-05 13:20:00.000000 dimsdk-0.8.6/dimsdk/cpu/contents.py
+-rw-r--r--   0 moky       (501) staff       (20)     3808 2023-07-05 15:19:44.000000 dimsdk-0.8.6/dimsdk/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     4733 2023-07-05 15:10:37.000000 dimsdk-0.8.6/dimsdk/cpu/customized.py
+-rw-r--r--   0 moky       (501) staff       (20)     4607 2023-07-05 15:15:25.000000 dimsdk-0.8.6/dimsdk/cpu/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     2415 2023-01-31 05:24:56.000000 dimsdk-0.8.6/dimsdk/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     8136 2023-07-05 15:40:56.000000 dimsdk-0.8.6/dimsdk/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8714 2023-07-05 11:09:04.000000 dimsdk-0.8.6/dimsdk/factories.py
+-rw-r--r--   0 moky       (501) staff       (20)     6741 2023-07-05 15:44:11.000000 dimsdk-0.8.6/dimsdk/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2263 2022-12-12 09:59:21.000000 dimsdk-0.8.6/dimsdk/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1965 2023-06-01 18:23:20.000000 dimsdk-0.8.6/dimsdk/mkm/robot.py
+-rw-r--r--   0 moky       (501) staff       (20)     4672 2022-12-11 05:05:26.000000 dimsdk-0.8.6/dimsdk/mkm/roles.py
+-rw-r--r--   0 moky       (501) staff       (20)     6579 2023-06-01 18:25:38.000000 dimsdk-0.8.6/dimsdk/mkm/station.py
+-rw-r--r--   0 moky       (501) staff       (20)    10085 2023-07-05 15:52:28.000000 dimsdk-0.8.6/dimsdk/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7188 2023-07-05 15:52:55.000000 dimsdk-0.8.6/dimsdk/processor.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      557 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       37 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        7 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-05 17:43:50.000000 dimsdk-0.8.6/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1256 2023-07-05 11:05:36.000000 dimsdk-0.8.6/setup.py
```

### Comparing `dimsdk-0.8.5/PKG-INFO` & `dimsdk-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-0.8.5/README.md` & `dimsdk-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.5/dimsdk/__init__.py` & `dimsdk-0.8.6/dimsdk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,21 +31,20 @@
 from mkm.types import *
 from mkm.crypto import *
 from mkm import *
 from dkd import *
 from dimp import *
 
 from .mkm import *
+from .cpu import *
 
 from .ans import AddressNameService
 from .delegate import CipherKeyDelegate
 from .facebook import Facebook
 from .messenger import Messenger
-from .helper import TwinsHelper
-from .proc_content import ContentProcessor, ContentProcessorFactory, ContentProcessorCreator
 from .processor import MessageProcessor
 from .packer import MessagePacker
 
 from .factories import ContentFactoryBuilder, CommandFactoryBuilder
 from .factories import GeneralCommandFactory, HistoryCommandFactory, GroupCommandFactory
 from .factories import register_content_factories, register_command_factories
 from .factories import register_message_factories, register_all_factories
@@ -126,29 +125,33 @@
     'TextContent', 'ForwardContent', 'ArrayContent',
     'MoneyContent', 'TransferContent',
     'FileContent', 'ImageContent', 'AudioContent', 'VideoContent',
     'PageContent', 'CustomizedContent',
 
     'Command', 'CommandFactory',
     'MetaCommand', 'DocumentCommand',
+    'ReceiptCommand',   # 'ReceiptCommandMixIn',
 
     'HistoryCommand', 'GroupCommand',
     'InviteCommand', 'ExpelCommand', 'JoinCommand',
     'QuitCommand', 'QueryCommand', 'ResetCommand',
 
     #
     #   DaoKeDao base extends
     #
     'BaseContent',
     'BaseTextContent', 'SecretContent', 'ListContent',
     'BaseMoneyContent', 'TransferMoneyContent',
     'BaseFileContent', 'ImageFileContent', 'AudioFileContent', 'VideoFileContent',
     'WebPageContent', 'AppCustomizedContent',
+
     'BaseCommand',
     'BaseMetaCommand', 'BaseDocumentCommand',
+    'BaseReceiptCommand', 'TextReceiptCommand',
+
     'BaseHistoryCommand', 'BaseGroupCommand',
     'InviteGroupCommand', 'ExpelGroupCommand', 'JoinGroupCommand',
     'QuitGroupCommand', 'QueryGroupCommand', 'ResetGroupCommand',
 
     # 'MessageEnvelope', 'MessageEnvelopeFactory',
     # 'BaseMessage',
     # 'PlainMessage', 'PlainMessageFactory',
@@ -157,22 +160,31 @@
 
     #
     #   Core
     #
     'Barrack', 'Transceiver', 'Packer', 'Processor',
 
     #
+    #   CPU
+    #
+    'TwinsHelper',
+    'ContentProcessor', 'ContentProcessorFactory', 'ContentProcessorCreator',
+    'BaseContentProcessorCreator', 'GeneralContentProcessorFactory',
+    'BaseContentProcessor', 'BaseCommandProcessor',
+    'ForwardContentProcessor', 'ArrayContentProcessor',
+    'MetaCommandProcessor', 'DocumentCommandProcessor', 'ReceiptCommandProcessor',
+    'CustomizedContentProcessor', 'CustomizedContentHandler',
+
+    #
     #   Extends
     #
     'ServiceProvider', 'Station', 'Bot',
 
     'AddressNameService', 'CipherKeyDelegate',
     'Facebook', 'Messenger',
-    'TwinsHelper',
-    'ContentProcessor', 'ContentProcessorFactory', 'ContentProcessorCreator',
     'MessageProcessor', 'MessagePacker',
 
     'ContentFactoryBuilder', 'CommandFactoryBuilder',
     'GeneralCommandFactory', 'HistoryCommandFactory', 'GroupCommandFactory',
 
     'register_content_factories', 'register_command_factories',
     'register_message_factories',
```

### Comparing `dimsdk-0.8.5/dimsdk/ans.py` & `dimsdk-0.8.6/dimsdk/ans.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.5/dimsdk/cpu/creator.py` & `dimsdk-0.8.6/dimsdk/cpu/creator.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,50 +34,58 @@
 
 """
 
 from typing import Optional, Union
 
 from dimp import ContentType, Command
 
-from ..helper import TwinsHelper
-from ..proc_content import ContentProcessor, ContentProcessorCreator
+from .base import TwinsHelper
+from .base import ContentProcessor, ContentProcessorCreator
 
 # from .base import BaseContentProcessor
 from .base import BaseCommandProcessor
-from .forward import ForwardContentProcessor
-from .array import ArrayContentProcessor
+from .contents import ForwardContentProcessor
+from .contents import ArrayContentProcessor
 # from .customized import CustomizedContentProcessor
 
-from .meta import MetaCommandProcessor
-from .document import DocumentCommandProcessor
+from .commands import MetaCommandProcessor
+from .commands import DocumentCommandProcessor
+from .commands import ReceiptCommandProcessor
 
 
 class BaseContentProcessorCreator(TwinsHelper, ContentProcessorCreator):
 
     # Override
     def create_content_processor(self, msg_type: Union[int, ContentType]) -> Optional[ContentProcessor]:
         # forward content
         if msg_type == ContentType.FORWARD.value:
             return ForwardContentProcessor(facebook=self.facebook, messenger=self.messenger)
         # array content
         if msg_type == ContentType.ARRAY.value:
             return ArrayContentProcessor(facebook=self.facebook, messenger=self.messenger)
+
         # # application customized
         # if msg_type == ContentType.APPLICATION.value:
         #     return CustomizedContentProcessor(facebook=self.facebook, messenger=self.messenger)
         # elif msg_type == ContentType.CUSTOMIZED.value:
         #     return CustomizedContentProcessor(facebook=self.facebook, messenger=self.messenger)
+
         # group commands
         if msg_type == ContentType.COMMAND.value:
             return BaseCommandProcessor(facebook=self.facebook, messenger=self.messenger)
+
         # # default contents
         # if msg_type == 0:
         #     return BaseContentProcessor(facebook=self.facebook, messenger=self.messenger)
 
     # Override
     def create_command_processor(self, msg_type: Union[int, ContentType], cmd: str) -> Optional[ContentProcessor]:
         # meta command
         if cmd == Command.META:
             return MetaCommandProcessor(facebook=self.facebook, messenger=self.messenger)
         # document command
         if cmd == Command.DOCUMENT:
             return DocumentCommandProcessor(facebook=self.facebook, messenger=self.messenger)
+
+        # receipt command
+        if cmd == Command.RECEIPT:
+            return ReceiptCommandProcessor(facebook=self.facebook, messenger=self.messenger)
```

### Comparing `dimsdk-0.8.5/dimsdk/cpu/customized.py` & `dimsdk-0.8.6/dimsdk/cpu/customized.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,60 +59,66 @@
 
 
 class CustomizedContentProcessor(BaseContentProcessor, CustomizedContentHandler):
     """
         Customized Content Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     """
-    FMT_APP_NOT_SUPPORT = 'Customized Content (app: %s) not support yet!'
-    FMT_ACT_NOT_SUPPORT = 'Customized Content (app: %s, mod: %s, act: %s) not support yet!'
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, CustomizedContent), 'customized content error: %s' % content
         # 1. check app id
         app = content.application
         responses = self._filter(app=app, content=content, msg=msg)
         if responses is not None:
-            # application ID not found
+            # app id not found
             return responses
         # 2. get handler with module name
         mod = content.module
         handler = self._fetch(mod=mod, content=content, msg=msg)
         if handler is None:
             # module not support
             return []
         # 3. do the job
         act = content.action
         sender = msg.sender
         return handler.handle_action(act=act, sender=sender, content=content, msg=msg)
 
-    # protected
     # noinspection PyUnusedLocal
     def _filter(self, app: str, content: CustomizedContent, msg: ReliableMessage) -> Optional[List[Content]]:
+        # Override for your application
         """
         Check for application
 
         :param app:     app ID
         :param content: customized content
         :param msg:     received message
         :return: None on app ID matched
         """
-        # Override for your application
-        text = self.FMT_APP_NOT_SUPPORT % app
-        return self._respond_text(text=text)
+        return self._respond_text(text='Content not support.', group=content.group, extra={
+            'template': 'Customized content (app: ${app}) not support yet!',
+            'replacements': {
+                'app': app,
+            }
+        })
 
-    # protected
     # noinspection PyUnusedLocal
     def _fetch(self, mod: str, content: CustomizedContent, msg: ReliableMessage) -> Optional[CustomizedContentHandler]:
         """ Override for you module """
         # if the application has too many modules, I suggest you to
         # use different handler to do the job for each module.
         return self
 
     # Override
     def handle_action(self, act: str, sender: ID, content: CustomizedContent, msg: ReliableMessage) -> List[Content]:
         """ Override for customized actions """
         app = content.application
         mod = content.module
-        text = self.FMT_ACT_NOT_SUPPORT % (app, mod, act)
-        return self._respond_text(text=text)
+        return self._respond_text(text='Content not support.', group=content.group, extra={
+            'template': 'Customized content (app: ${app}, mod: ${mod}, act: ${act}) not support yet!',
+            'replacements': {
+                'app': app,
+                'mod': mod,
+                'act': act,
+            }
+        })
```

### Comparing `dimsdk-0.8.5/dimsdk/cpu/factory.py` & `dimsdk-0.8.6/dimsdk/cpu/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,25 +35,23 @@
     produce content/command processors
 """
 
 from typing import Dict, Optional, Union
 
 from dimp import ContentType, Content, Command, GroupCommand
 
-from ..helper import TwinsHelper
-from ..facebook import Facebook
-from ..messenger import Messenger
-from ..proc_content import ContentProcessor, ContentProcessorFactory
+from .base import TwinsHelper
+from .base import ContentProcessor, ContentProcessorFactory
 
 from .creator import ContentProcessorCreator
 
 
 class GeneralContentProcessorFactory(TwinsHelper, ContentProcessorFactory):
 
-    def __init__(self, facebook: Facebook, messenger: Messenger, creator: ContentProcessorCreator):
+    def __init__(self, facebook, messenger, creator: ContentProcessorCreator):
         super().__init__(facebook=facebook, messenger=messenger)
         self.__creator = creator
         self.__content_processors: Dict[int, ContentProcessor] = {}
         self.__command_processors: Dict[str, ContentProcessor] = {}
 
     @property  # protected
     def creator(self) -> ContentProcessorCreator:
```

### Comparing `dimsdk-0.8.5/dimsdk/cpu/forward.py` & `dimsdk-0.8.6/dimsdk/cpu/contents.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,43 +24,69 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-"""
-    Forward Content Processor
-    ~~~~~~~~~~~~~~~~~~~~~~~~~
-
-"""
 
 from typing import List
 
 from dimp import ReliableMessage
-from dimp import Content, ForwardContent
+from dimp import Content, ForwardContent, ArrayContent
 
 from .base import BaseContentProcessor
 
 
-#
-#   Forward Content Processor
-#
+def get_messenger(cpu: BaseContentProcessor):  # -> Messenger:
+    messenger = cpu.messenger
+    from ..messenger import Messenger
+    assert isinstance(messenger, Messenger), 'messenger error: %s' % messenger
+    return messenger
+
+
 class ForwardContentProcessor(BaseContentProcessor):
+    """
+        Forward Content Processor
+        ~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    """
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, ForwardContent), 'forward content error: %s' % content
         # call messenger to process it
-        messenger = self.messenger
+        messenger = get_messenger(cpu=self)
         secrets = content.secrets
         responses = []
         for item in secrets:
             results = messenger.process_reliable_message(msg=item)
-            if results is None:
-                res = ForwardContent.create(messages=[])
-            elif len(results) == 1:
+            if len(results) == 1:
                 res = ForwardContent.create(message=results[0])
             else:
                 res = ForwardContent.create(messages=results)
             responses.append(res)
         return responses
+
+
+class ArrayContentProcessor(BaseContentProcessor):
+    """
+        Array Content Processor
+        ~~~~~~~~~~~~~~~~~~~~~~~
+
+    """
+
+    # Override
+    def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
+        assert isinstance(content, ArrayContent), 'forward content error: %s' % content
+        # call messenger to process it
+        messenger = get_messenger(cpu=self)
+        contents = content.contents
+        responses = []
+        for item in contents:
+            results = messenger.process_content(content=item, r_msg=msg)
+            if len(results) == 1:
+                res = results[0]
+            else:
+                res = ArrayContent.create(contents=results)
+            responses.append(res)
+        return responses
```

### Comparing `dimsdk-0.8.5/dimsdk/delegate.py` & `dimsdk-0.8.6/dimsdk/delegate.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.5/dimsdk/facebook.py` & `dimsdk-0.8.6/dimsdk/facebook.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,28 +131,30 @@
         else:
             # check by user's meta.key
             meta = self.meta(identifier=identifier)
         if meta is not None:
             return document.verify(public_key=meta.key)
 
     # protected
+    # noinspection PyMethodMayBeStatic
     def create_user(self, identifier: ID) -> Optional[User]:
         # TODO: make sure visa key exists before calling this
         network = identifier.type
         # check user type
         if network == EntityType.STATION:
             # TODO: get station ip,port before create it
             # return Station(identifier=identifier, host='0.0.0.0', port=0)
             return Station(identifier=identifier)
         elif network == EntityType.BOT:
             return Bot(identifier=identifier)
         # general user, or 'anyone@anywhere'
         return BaseUser(identifier=identifier)
 
     # protected
+    # noinspection PyMethodMayBeStatic
     def create_group(self, identifier: ID) -> Optional[Group]:
         # TODO: make group meta exists before calling this
         network = identifier.type
         # check group type
         if network == EntityType.ISP:
             return ServiceProvider(identifier=identifier)
         # general group, or 'everyone@everywhere'
@@ -164,25 +166,18 @@
         """
         Get all local users (for decrypting received message)
 
         :return: users with private key
         """
         raise NotImplemented
 
-    # @property
-    # def current_user(self) -> Optional[User]:
-    #     """ Get current user (for signing and sending message) """
-    #     users = self.local_users
-    #     if users is not None and len(users) > 0:
-    #         return users[0]
-
     def select_user(self, receiver: ID) -> Optional[User]:
         """ Select local user for receiver """
         users = self.local_users
-        if users is None or len(users) == 0:
+        if len(users) == 0:
             assert False, 'local users should not be empty'
             # return None
         elif receiver.is_broadcast:
             # broadcast message can decrypt by anyone, so just return current user
             return users[0]
         elif receiver.is_user:
             # 1. personal message
@@ -194,21 +189,21 @@
             # not mine?
             return None
         # group message (recipient not designated)
         assert receiver.is_group, 'receiver error: %s' % receiver
         # the messenger will check group info before decrypting message,
         # so we can trust that the group's meta & members MUST exist here.
         grp = self.group(identifier=receiver)
-        assert grp is not None, 'group not ready: %s' % receiver
-        # if grp is None:
-        #     return None
+        if grp is None:
+            assert False, 'group not ready: %s' % receiver
+            # return None
         members = grp.members
-        assert len(members) > 0, 'members not found: %s' % receiver
-        # if members is None or len(members) == 0:
-        #     return None
+        if members is None or len(members) == 0:
+            assert False, 'members not found: %s' % receiver
+            # return None
         for item in users:
             if item.identifier in members:
                 # DISCUSS: set this item to be current user?
                 return item
 
     #
     #   Entity Delegate
```

### Comparing `dimsdk-0.8.5/dimsdk/factories.py` & `dimsdk-0.8.6/dimsdk/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from dimp import BaseContent
 from dimp import BaseTextContent, SecretContent, ListContent
 from dimp import BaseMoneyContent, TransferMoneyContent
 from dimp import BaseFileContent, ImageFileContent, AudioFileContent, VideoFileContent
 from dimp import WebPageContent, AppCustomizedContent
 from dimp import BaseCommand
 from dimp import BaseMetaCommand, BaseDocumentCommand
+from dimp import BaseReceiptCommand
 from dimp import BaseHistoryCommand, BaseGroupCommand
 from dimp import InviteGroupCommand, ExpelGroupCommand, JoinGroupCommand
 from dimp import QuitGroupCommand, QueryGroupCommand, ResetGroupCommand
 
 
 class ContentFactoryBuilder(ContentFactory):
 
@@ -173,14 +174,17 @@
     """ Register core command factories """
     # Meta Command
     Command.register(cmd=Command.META, factory=CommandFactoryBuilder(command_class=BaseMetaCommand))
 
     # Document Command
     Command.register(cmd=Command.DOCUMENT, factory=CommandFactoryBuilder(command_class=BaseDocumentCommand))
 
+    # Receipt Command
+    Command.register(cmd=Command.RECEIPT, factory=CommandFactoryBuilder(command_class=BaseReceiptCommand))
+
     # Group Commands
     Command.register(cmd='group', factory=GroupCommandFactory())
     Command.register(cmd=GroupCommand.INVITE, factory=CommandFactoryBuilder(command_class=InviteGroupCommand))
     Command.register(cmd=GroupCommand.EXPEL, factory=CommandFactoryBuilder(command_class=ExpelGroupCommand))
     Command.register(cmd=GroupCommand.JOIN, factory=CommandFactoryBuilder(command_class=JoinGroupCommand))
     Command.register(cmd=GroupCommand.QUIT, factory=CommandFactoryBuilder(command_class=QuitGroupCommand))
     Command.register(cmd=GroupCommand.QUERY, factory=CommandFactoryBuilder(command_class=QueryGroupCommand))
```

### Comparing `dimsdk-0.8.5/dimsdk/helper.py` & `dimsdk-0.8.6/dimsdk/mkm/robot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 #   DIM-SDK : Decentralized Instant Messaging Software Development Kit
 #
-#                                Written in 2022 by Moky <albert.moky@gmail.com>
+#                                Written in 2019 by Moky <albert.moky@gmail.com>
 #
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2022 Albert Moky
+# Copyright (c) 2019 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,33 +24,29 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import weakref
+"""
+    Bot User
+    ~~~~~~~~
+"""
 
-from .facebook import Facebook
-from .messenger import Messenger
+from typing import Optional
 
+from dimp import ID, EntityType
+from dimp import BaseUser
 
-class TwinsHelper:
-    """
-        Messenger Shadow
-        ~~~~~~~~~~~~~~~~
 
-        Delegate for Messenger
-    """
+class Bot(BaseUser):
 
-    def __init__(self, facebook: Facebook, messenger: Messenger):
-        super().__init__()
-        self.__facebook = weakref.ref(facebook)
-        self.__messenger = weakref.ref(messenger)
+    def __init__(self, identifier: ID):
+        super().__init__(identifier=identifier)
+        assert identifier.type == EntityType.BOT, 'Bot ID type error: %s' % identifier
 
     @property
-    def messenger(self) -> Messenger:
-        return self.__messenger()
-
-    @property
-    def facebook(self) -> Facebook:
-        return self.__facebook()
+    def provider(self) -> Optional[ID]:
+        doc = self.document(doc_type='*')
+        if doc is not None:
+            return ID.parse(identifier=doc.get_property(key='ICP'))
```

### Comparing `dimsdk-0.8.5/dimsdk/messenger.py` & `dimsdk-0.8.6/dimsdk/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,23 +156,23 @@
     #
 
     # Override
     def deserialize_key(self, data: Optional[bytes], sender: ID, receiver: ID,
                         msg: SecureMessage) -> Optional[SymmetricKey]:
         if data is None:
             # get key from cache
-            return self.cipher_key(sender=sender, receiver=receiver)
+            return self.cipher_key(sender=sender, receiver=receiver, generate=False)
         else:
             return super().deserialize_key(data=data, sender=sender, receiver=receiver, msg=msg)
 
     # Override
     def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
         content = super().deserialize_content(data=data, key=key, msg=msg)
         assert content is not None, 'content error: %d' % len(data)
-        if not is_broadcast(msg=msg):
+        if not is_broadcast(msg=msg) and content is not None:
             # check and cache key for reuse
             group = self.overt_group(content=content)
             if group is None:
                 # personal message or (group) command
                 # cache key with direction (sender -> receiver)
                 self.cache_cipher_key(key=key, sender=msg.sender, receiver=msg.receiver)
             else:
```

### Comparing `dimsdk-0.8.5/dimsdk/mkm/__init__.py` & `dimsdk-0.8.6/dimsdk/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.5/dimsdk/mkm/roles.py` & `dimsdk-0.8.6/dimsdk/mkm/roles.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.5/dimsdk/mkm/station.py` & `dimsdk-0.8.6/dimsdk/mkm/station.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.5/dimsdk/packer.py` & `dimsdk-0.8.6/dimsdk/packer.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,30 @@
 from mkm.crypto import json_encode, json_decode, utf8_encode, utf8_decode
 
 from dimp import ID
 from dimp import Content, Command
 from dimp import InstantMessage, SecureMessage, ReliableMessage
 from dimp import Packer
 
-from .helper import TwinsHelper
+from .cpu import TwinsHelper
+
+from .facebook import Facebook
+from .messenger import Messenger
 
 
 class MessagePacker(TwinsHelper, Packer):
 
+    @property
+    def facebook(self) -> Facebook:
+        return super().facebook
+
+    @property
+    def messenger(self) -> Messenger:
+        return super().messenger
+
     # Override
     def overt_group(self, content: Content) -> Optional[ID]:
         group = content.group
         if group is None:
             return None
         elif group.is_broadcast:
             # broadcast message is always overt
```

### Comparing `dimsdk-0.8.5/dimsdk/proc_content.py` & `dimsdk-0.8.6/dimsdk/cpu/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 #   DIM-SDK : Decentralized Instant Messaging Software Development Kit
 #
-#                                Written in 2022 by Moky <albert.moky@gmail.com>
+#                                Written in 2019 by Moky <albert.moky@gmail.com>
 #
 # ==============================================================================
 # MIT License
 #
-# Copyright (c) 2022 Albert Moky
+# Copyright (c) 2019 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,19 +24,28 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
+"""
+    Content Processor
+    ~~~~~~~~~~~~~~~~~
+
+"""
+
+import weakref
 from abc import ABC, abstractmethod
-from typing import List, Optional, Union
+from typing import Optional, Union, List, Dict
 
-from dimp import Content, ContentType
+from dimp import ID
 from dimp import ReliableMessage
+from dimp import ContentType, Content, Command
+from dimp import TextReceiptCommand
 
 
 class ContentProcessor(ABC):
     """
         CPU: Content Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     """
@@ -49,14 +58,44 @@
         :param content: content received
         :param msg:     reliable message
         :return: responses to sender
         """
         raise NotImplemented
 
 
+class ContentProcessorCreator(ABC):
+    """
+        CPU Creator
+        ~~~~~~~~~~~
+
+        Delegate for CPU Factory
+    """
+
+    @abstractmethod
+    def create_content_processor(self, msg_type: Union[int, ContentType]) -> Optional[ContentProcessor]:
+        """
+        Create content processor with type
+
+        :param msg_type: content type
+        :return ContentProcessor
+        """
+        raise NotImplemented
+
+    @abstractmethod
+    def create_command_processor(self, msg_type: Union[int, ContentType], cmd: str) -> Optional[ContentProcessor]:
+        """
+        Create command processor with name
+
+        :param msg_type: content type
+        :param cmd:      command name
+        :return CommandProcessor
+        """
+        raise NotImplemented
+
+
 class ContentProcessorFactory(ABC):
     """
         CPU Factory
         ~~~~~~~~~~~
 
         Delegate for Message Processor
     """
@@ -76,35 +115,76 @@
         raise NotImplemented
 
     @abstractmethod
     def get_command_processor(self, msg_type: Union[int, ContentType], cmd: str) -> Optional[ContentProcessor]:
         raise NotImplemented
 
 
-class ContentProcessorCreator(ABC):
+class TwinsHelper:
     """
-        CPU Creator
-        ~~~~~~~~~~~
+        Messenger Shadow
+        ~~~~~~~~~~~~~~~~
 
-        Delegate for CPU Factory
+        Delegate for Messenger
     """
 
-    @abstractmethod
-    def create_content_processor(self, msg_type: Union[int, ContentType]) -> Optional[ContentProcessor]:
-        """
-        Create content processor with type
+    def __init__(self, facebook, messenger):
+        super().__init__()
+        self.__facebook = weakref.ref(facebook)
+        self.__messenger = weakref.ref(messenger)
 
-        :param msg_type: content type
-        :return ContentProcessor
-        """
-        raise NotImplemented
+    @property
+    def messenger(self):  # -> Messenger:
+        return self.__messenger()
 
-    @abstractmethod
-    def create_command_processor(self, msg_type: Union[int, ContentType], cmd: str) -> Optional[ContentProcessor]:
-        """
-        Create command processor with name
+    @property
+    def facebook(self):  # -> Facebook:
+        return self.__facebook()
 
-        :param msg_type: content type
-        :param cmd:      command name
-        :return CommandProcessor
-        """
-        raise NotImplemented
+
+#
+#   Implementations
+#
+
+
+class BaseContentProcessor(TwinsHelper, ContentProcessor):
+    """
+        Content Processing Unit
+        ~~~~~~~~~~~~~~~~~~~~~~~
+    """
+
+    # Override
+    def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
+        # override to process this content
+        return self._respond_text(text='Content not support.', group=content.group, extra={
+            'template': 'Content (type: ${type}) not support yet!',
+            'replacements': {
+                'type': content.type,
+            }
+        })
+
+    # noinspection PyMethodMayBeStatic
+    def _respond_text(self, text: str, group: Optional[ID] = None, extra: Dict = None) -> List[Content]:
+        res = TextReceiptCommand.from_text(text=text)
+        if group is not None:
+            res.group = group
+        if extra is not None:
+            for key in extra:
+                res[key] = extra[key]
+        return [res]
+
+
+class BaseCommandProcessor(BaseContentProcessor):
+    """
+        Command Processing Unit
+        ~~~~~~~~~~~~~~~~~~~~~~~
+    """
+
+    # Override
+    def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
+        assert isinstance(content, Command), 'command error: %s' % content
+        return self._respond_text(text='Command not support.', group=content.group, extra={
+            'template': 'Command (name: ${command}) not support yet!',
+            'replacements': {
+                'command': content.cmd,
+            }
+        })
```

### Comparing `dimsdk-0.8.5/dimsdk/processor.py` & `dimsdk-0.8.6/dimsdk/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,31 @@
 
 from typing import List, Union, Optional
 
 from dimp import ContentType, Content, Envelope
 from dimp import InstantMessage, SecureMessage, ReliableMessage
 from dimp import Processor
 
+from .cpu import TwinsHelper
+from .cpu import ContentProcessor, ContentProcessorFactory, ContentProcessorCreator
+
 from .facebook import Facebook
 from .messenger import Messenger
-from .helper import TwinsHelper
-from .proc_content import ContentProcessor, ContentProcessorFactory, ContentProcessorCreator
 
 
 class MessageProcessor(TwinsHelper, Processor):
 
+    @property
+    def facebook(self) -> Facebook:
+        return super().facebook
+
+    @property
+    def messenger(self) -> Messenger:
+        return super().messenger
+
     def __init__(self, facebook: Facebook, messenger: Messenger):
         super().__init__(facebook=facebook, messenger=messenger)
         self.__factory = self._create_factory()
 
     # protected
     def _create_factory(self) -> ContentProcessorFactory:
         creator = self._create_creator()
```

### Comparing `dimsdk-0.8.5/dimsdk.egg-info/PKG-INFO` & `dimsdk-0.8.6/dimsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-0.8.5/setup.py` & `dimsdk-0.8.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.8.5'
+__version__ = '0.8.6'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -37,12 +37,12 @@
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dimp>=0.12.8',
+        'dimp>=0.12.9',
         'dkd>=0.12.7',
         'mkm>=0.12.7',
     ]
 )
```

