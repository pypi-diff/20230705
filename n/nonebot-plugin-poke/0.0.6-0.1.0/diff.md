# Comparing `tmp/nonebot_plugin_poke-0.0.6.tar.gz` & `tmp/nonebot_plugin_poke-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.0.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.0.6.tar` & `nonebot_plugin_poke-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/LICENSE
--rw-r--r--   0        0        0     2923 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/README.md
--rw-r--r--   0        0        0     5088 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      753 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     4623 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      922 2023-07-04 16:09:10.873264 nonebot_plugin_poke-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3045 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/README.md
+-rw-r--r--   0        0        0     5053 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      753 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     1234 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/matcher.py
+-rw-r--r--   0        0        0     5068 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0      931 2023-07-05 10:29:18.683132 nonebot_plugin_poke-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.0.6/LICENSE` & `nonebot_plugin_poke-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.6/README.md` & `nonebot_plugin_poke-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_poke
 
-_✨Nonebot & 戳戳✨_
+_✨Nonebot & 自定义戳戳群聊事件✨_
 
 <a href="https://github.com/Agnes4m/nonebot_plugin_poke/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_poke" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_poke/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_poke" alt="issues">
 </a>
@@ -70,14 +70,15 @@
 
 ## 指令
 
 群里双击bot头像，会依次按照配置文件，逐步检查回复
 
 ## 数据结构
 
+
 ```txt
 举例：
 └── data
     └── poke
         ├── poke.txt        # 回复文字
         ├── pic             # 回复图片
             ├── 1.png
@@ -89,12 +90,13 @@
             ├── 2.mp3
             └── ...
 ...
 ```
 
 ## 其他
 
-如果发不出语音，请手动安装ffmpeg
+- 如果发不出语音，请手动安装ffmpeg
+- 当语音，与图或文都为True的时候，则随机发送一种，防止刷屏刷到风控
 
 ## 参考
 
-- [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply) - 配置写法
+- [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply) - 配置写法
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-# nonebot_plugin_poke _â¨Nonebot & æ³æ³â¨_ [GitHub_stars] [GitHub_issues]
-                   [QQ_Chat_Group] [pypi] [python] [NoneBot]
+  # nonebot_plugin_poke _â¨Nonebot & èªå®ä¹æ³æ³ç¾¤èäºä»¶â¨_ [GitHub
+       stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## å®è£ æ¹æ³ä¸ï¼ nb plugin install nonebot_plugin_poke æ¹æ³äºï¼ pip
 install nonebot_plugin_poke
 åæå¨æ·»å `nonebot_plugin_poke`å°botæä»¶ä¸`pyproject.toml`æä»¶ä¸­ ##
 envéç½®é¡¹: # å¨å®å¨ä¸åçæåµä¸ï¼æææ¯æ³æ³ååæ³æ³ #
 æºå¨äººåç§° bot_nickname: str = 'å®å®' # æ¯å¦åå¤å¾ç
 poke_send_pic: bool = False # æ¯å¦åå¤æ³æ³ poke_send_poke: bool = True #
 æ¯å¦åå¤æå­ poke_send_text: bool = False # æ¯å¦åå¤é³é¢
@@ -16,10 +16,12 @@
 é»ååå±è½ç¾¤ç» poke_ban_group:List[str] = [] # ç½åååè®¸ç¾¤ç»
 poke_allow_group:List[str] = [] # æ³æ³ä¼åçº§ poke_priority:int = 1 #
 æ¯å¦é»æ­å¶ä»æä»¤ poke_block:bool = True ## æä»¤
 ç¾¤éåå»botå¤´åï¼ä¼ä¾æ¬¡æç§éç½®æä»¶ï¼éæ­¥æ£æ¥åå¤ ##
 æ°æ®ç»æ ```txt ä¸¾ä¾ï¼ âââ data âââ poke âââ poke.txt
 # åå¤æå­ âââ pic # åå¤å¾ç âââ 1.png âââ 2.jpg
 âââ 3.jpeg âââ ... âââ acc # åå¤é³é¢ âââ 1.acc
-âââ 2.mp3 âââ ... ... ``` ## å¶ä»
-å¦æåä¸åºè¯­é³ï¼è¯·æå¨å®è£ffmpeg ## åè - [æºéåå¤](https:
-//github.com/Special-Week/nonebot_plugin_smart_reply) - éç½®åæ³
+âââ 2.mp3 âââ ... ... ``` ## å¶ä» -
+å¦æåä¸åºè¯­é³ï¼è¯·æå¨å®è£ffmpeg -
+å½è¯­é³ï¼ä¸å¾ææé½ä¸ºTrueçæ¶åï¼åéæºåéä¸ç§ï¼é²æ­¢å·å±å·å°é£æ§
+## åè - [æºéåå¤](https://github.com/Special-Week/
+nonebot_plugin_smart_reply) - éç½®åæ³
```

### Comparing `nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/__init__.py` & `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from nonebot.params import CommandArg
 from nonebot.rule import to_me
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.plugin.on import  on_notice,on_command
 from nonebot.adapters.onebot.v11 import PokeNotifyEvent,MessageEvent
 
-import datetime
+from datetime import datetime
 import imghdr
 
 from .utils import *
+from .matcher import *
 
 logo ="""
     ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
     ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
@@ -42,18 +43,18 @@
     ...... .^...**.O@...\O^ .     \.....`   .^ /.,^.=O@OO`=O@^..OO`.=OO\
     ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
     ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
-__version__ = "0.0.6"
+__version__ = "0.1.0"
 __plugin_meta__ = PluginMetadata(
     name="戳一戳事件",
-    description='自定义戳一戳事件',
+    description='自定义群聊戳一戳事件',
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_poke",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
@@ -62,17 +63,15 @@
 
 poke_ = on_notice(block=config.poke_block, 
                   priority=config.poke_priority, rule=poke_rule)
 
 
 @poke_.handle()
 async def _(event: PokeNotifyEvent,matcher:Matcher):
-    await poke_send(event,matcher)
-    await acc_send(matcher)
-    await pic_text_send(event,matcher)
+    await poke_reply(event,matcher)
     
 
 add_pic = on_command('zq',aliases={'抓图'},priority=30)
 @add_pic.handle()
 async def _(event:MessageEvent,matcher:Matcher):
     images: List[bytes] = []
     images_name: List[str] = []
@@ -109,8 +108,8 @@
             path = config.poke_path.joinpath('pic')
             for i,img in enumerate(images):
                 img_path = path / images_name[i]
                 with img_path.open("wb+") as f:
                     f.write(img)
 
             tosend = f"添加完成，成功{success}张，失败{fail}张，可用于戳戳随机图"
-            await matcher.send(event=event,message=tosend,at_sender=True)
+            await matcher.send(message=tosend,at_sender=True)
```

### Comparing `nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.6/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from nonebot.matcher import Matcher
+from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import PokeNotifyEvent,MessageSegment, Message
 
 import random
 import aiohttp
-from typing import List
+from typing import List,Optional
 from pathlib import Path
 
 from .config import config
 
 async def get_data(url:str):
     """获取url内容"""
     headers = {
@@ -18,87 +19,101 @@
             if response.status == 200:
                 return await response.read()
             else:
                 return None
             
             
 async def acc_send(matcher:Matcher):
-    """音乐部分"""
-    if not config.poke_send_acc:
-        return
-    else:
-        poke_file_path = config.poke_path
-        poke_file_path.joinpath('acc').mkdir(parents=True, exist_ok=True)
-        poke_acc_list = poke_file_path.joinpath('acc').iterdir()
-        acc_file_list:List[str] = []
-        for acc_file in poke_acc_list:
-            if acc_file.is_file() and acc_file.suffix.lower() in [".wav",".mp3",".acc"]:
-                acc_file_list.append(str(acc_file))
-        send_acc = random.choice(acc_file_list)
-        await matcher.send(MessageSegment.record(send_acc))
+    """语音部分"""
+    poke_file_path = config.poke_path
+    poke_file_path.joinpath('acc').mkdir(parents=True, exist_ok=True)
+    poke_acc_list = poke_file_path.joinpath('acc').iterdir()
+    acc_file_list:List[Path] = []
+    for acc_file in poke_acc_list:
+        if acc_file.is_file() and acc_file.suffix.lower() in [".wav",".mp3",".acc"]:
+            acc_file_list.append(acc_file)
+    send_acc = random.choice(acc_file_list)
+    await matcher.send(MessageSegment.record(file=f"file:///{send_acc.resolve()}"))
     
 async def poke_send(event:PokeNotifyEvent,matcher:Matcher):
     if config.poke_send_poke:
+        logger.success('反击戳戳')
         await matcher.send(Message([
         MessageSegment("poke",  {
            "qq": f"{event.user_id}"
        })
     ]))
     else:
         return
     
-async def pic_text_send(event:PokeNotifyEvent,matcher:Matcher):
+async def pic_send(event:PokeNotifyEvent,matcher:Matcher):
     """发送图片和text"""
     pic_file_path = config.poke_path
     pic_file_path.joinpath('pic').mkdir(parents=True, exist_ok=True)
     if config.poke_send_pic:
+        logger.success('发送图片')
         poke_pic_list = pic_file_path.joinpath('pic').iterdir()
-        pic_file_list:List[str] = []
+        pic_file_list:List[Path] = []
         for pic_file in poke_pic_list:
             if pic_file.is_file() and pic_file.suffix.lower() in [".png",".jpg",".jpeg",".webp",".gif"]:
-                pic_file_list.append(str(pic_file))
+                pic_file_list.append(pic_file)
         send_pic = random.choice(pic_file_list)
     else:
-        send_pic:str = ''
-    if config.poke_send_text:
-        if pic_file_path.joinpath('poke.txt').is_file():
-            with open(pic_file_path.joinpath('poke.txt'),mode='r',encoding='utf-8')as f :
-                text_file_list:List[str] = f.read().split('/n')
-                send_text = random.choice(text_file_list)
-        else:
-            with open(pic_file_path.joinpath('poke.txt'),mode='w',encoding='utf-8')as f :
-                text_file_list:List[str] = [
-                "lsp你再戳？",
-                "连个可爱美少女都要戳的肥宅真恶心啊。",
-                "你再戳！",
-                "？再戳试试？",
-                "别戳了别戳了再戳就坏了555",
-                "我爪巴爪巴，球球别再戳了",
-                "你戳你🐎呢？！",
-                "请不要戳我 >_<",
-                "放手啦，不给戳QAQ",
-                "喂(#`O′) 戳我干嘛！",
-                "戳坏了，赔钱！",
-                "戳坏了",
-                "嗯……不可以……啦……不要乱戳",
-                "那...那里...那里不能戳...绝对...",
-                "(。´・ω・)ん?",
-                "有事恁叫我，别天天一个劲戳戳戳！",
-                "欸很烦欸！你戳🔨呢",
-                "再戳一下试试？",
-                "正在关闭对您的所有服务...关闭成功",
-                "啊呜，太舒服刚刚竟然睡着了。什么事？",
-                "正在定位您的真实地址...定位成功。轰炸机已起飞",
-                ]
-                f.write('/n'.join(text_file_list))
-                send_text = random.choice(text_file_list)
-        send_text.replace('我',config.bot_nickname)
+        send_pic = None
+    return send_pic
+        
+async def text_send(event:PokeNotifyEvent,matcher:Matcher):
+    logger.success('发送文字')
+    pic_file_path = config.poke_path
+    if pic_file_path.joinpath('poke.txt').is_file():
+        with open(pic_file_path.joinpath('poke.txt'),mode='r',encoding='utf-8')as f :
+            text_file_list:List[str] = f.read().split('/n')
+            send_text = random.choice(text_file_list)
     else:
-        send_text:str = ''
-    await matcher.send(MessageSegment.image(send_pic)+send_text)
+        with open(pic_file_path.joinpath('poke.txt'),mode='w',encoding='utf-8')as f :
+            text_file_list:List[str] = [
+            "lsp你再戳？",
+            "连个可爱美少女都要戳的肥宅真恶心啊。",
+            "你再戳！",
+            "？再戳试试？",
+            "别戳了别戳了再戳就坏了555",
+            "我爪巴爪巴，球球别再戳了",
+            "你戳你🐎呢？！",
+            "请不要戳我 >_<",
+            "放手啦，不给戳QAQ",
+            "喂(#`O′) 戳我干嘛！",
+            "戳坏了，赔钱！",
+            "戳坏了",
+            "嗯……不可以……啦……不要乱戳",
+            "那...那里...那里不能戳...绝对...",
+            "(。´・ω・)ん?",
+            "有事恁叫我，别天天一个劲戳戳戳！",
+            "欸很烦欸！你戳🔨呢",
+            "再戳一下试试？",
+            "正在关闭对您的所有服务...关闭成功",
+            "啊呜，太舒服刚刚竟然睡着了。什么事？",
+            "正在定位您的真实地址...定位成功。轰炸机已起飞",
+            ]
+            f.write('/n'.join(text_file_list))
+            send_text = random.choice(text_file_list)
+    send_text.replace('我',config.bot_nickname)
+    return send_text
+
+async def pic_or_text(send_pic:Optional[Path],send_text:Optional[str],matcher:Matcher):
+    if send_pic and send_text:
+        await matcher.send(MessageSegment.image(file=f"file:///{send_pic.resolve()}")+send_text)
+        return
+    elif send_pic and not send_text:
+        await matcher.send(MessageSegment.image(file=f"file:///{send_pic.resolve()}"))
+        return
+    elif not send_pic and send_text:
+        await matcher.send(send_text)
+        return
+    else:
+        return
 
 async def poke_rule(event:PokeNotifyEvent):
     """黑白名单判断"""
     if isinstance(event,PokeNotifyEvent) and event.target_id == event.self_id:
         group = event.group_id
         if config.poke_black:
             if group in config.poke_ban_group:
```

### Comparing `nonebot_plugin_poke-0.0.6/pyproject.toml` & `nonebot_plugin_poke-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot_plugin_poke"
-version = "0.0.6"
-description = "群聊戳戳事件 plugin for NoneBot2"
+version = "0.1.0"
+description = "自定义群聊戳戳事件 plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
 repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
 keywords = ["nonebot2", "plugin","event"]
 classifiers = [
```

### Comparing `nonebot_plugin_poke-0.0.6/PKG-INFO` & `nonebot_plugin_poke-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.0.6
-Summary: 群聊戳戳事件 plugin for NoneBot2
+Version: 0.1.0
+Summary: 自定义群聊戳戳事件 plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_poke
 License: MIT
 Keywords: nonebot2,plugin,event
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_poke
 
-_✨Nonebot & 戳戳✨_
+_✨Nonebot & 自定义戳戳群聊事件✨_
 
 <a href="https://github.com/Agnes4m/nonebot_plugin_poke/stargazers">
         <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_poke" alt="stars">
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_poke/issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_poke" alt="issues">
 </a>
@@ -92,14 +92,15 @@
 
 ## 指令
 
 群里双击bot头像，会依次按照配置文件，逐步检查回复
 
 ## 数据结构
 
+
 ```txt
 举例：
 └── data
     └── poke
         ├── poke.txt        # 回复文字
         ├── pic             # 回复图片
             ├── 1.png
@@ -111,12 +112,14 @@
             ├── 2.mp3
             └── ...
 ...
 ```
 
 ## 其他
 
-如果发不出语音，请手动安装ffmpeg
+- 如果发不出语音，请手动安装ffmpeg
+- 当语音，与图或文都为True的时候，则随机发送一种，防止刷屏刷到风控
 
 ## 参考
 
 - [智障回复](https://github.com/Special-Week/nonebot_plugin_smart_reply) - 配置写法
+
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.6 Summary:
-ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/Agnes4m/
-nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event Author:
-Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
-(>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL: Repository,
-https://github.com/Agnes4m/nonebot_plugin_poke Description-Content-Type: text/
-markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.1.0 Summary:
+èªå®ä¹ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/
+Agnes4m/nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event
+Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
+>=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
+adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL:
+Repository, https://github.com/Agnes4m/nonebot_plugin_poke Description-Content-
+Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
-# nonebot_plugin_poke _â¨Nonebot & æ³æ³â¨_ [GitHub_stars] [GitHub_issues]
-                   [QQ_Chat_Group] [pypi] [python] [NoneBot]
+  # nonebot_plugin_poke _â¨Nonebot & èªå®ä¹æ³æ³ç¾¤èäºä»¶â¨_ [GitHub
+       stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## å®è£ æ¹æ³ä¸ï¼ nb plugin install nonebot_plugin_poke æ¹æ³äºï¼ pip
 install nonebot_plugin_poke
 åæå¨æ·»å `nonebot_plugin_poke`å°botæä»¶ä¸`pyproject.toml`æä»¶ä¸­ ##
 envéç½®é¡¹: # å¨å®å¨ä¸åçæåµä¸ï¼æææ¯æ³æ³ååæ³æ³ #
 æºå¨äººåç§° bot_nickname: str = 'å®å®' # æ¯å¦åå¤å¾ç
 poke_send_pic: bool = False # æ¯å¦åå¤æ³æ³ poke_send_poke: bool = True #
 æ¯å¦åå¤æå­ poke_send_text: bool = False # æ¯å¦åå¤é³é¢
@@ -28,10 +28,12 @@
 é»ååå±è½ç¾¤ç» poke_ban_group:List[str] = [] # ç½åååè®¸ç¾¤ç»
 poke_allow_group:List[str] = [] # æ³æ³ä¼åçº§ poke_priority:int = 1 #
 æ¯å¦é»æ­å¶ä»æä»¤ poke_block:bool = True ## æä»¤
 ç¾¤éåå»botå¤´åï¼ä¼ä¾æ¬¡æç§éç½®æä»¶ï¼éæ­¥æ£æ¥åå¤ ##
 æ°æ®ç»æ ```txt ä¸¾ä¾ï¼ âââ data âââ poke âââ poke.txt
 # åå¤æå­ âââ pic # åå¤å¾ç âââ 1.png âââ 2.jpg
 âââ 3.jpeg âââ ... âââ acc # åå¤é³é¢ âââ 1.acc
-âââ 2.mp3 âââ ... ... ``` ## å¶ä»
-å¦æåä¸åºè¯­é³ï¼è¯·æå¨å®è£ffmpeg ## åè - [æºéåå¤](https:
-//github.com/Special-Week/nonebot_plugin_smart_reply) - éç½®åæ³
+âââ 2.mp3 âââ ... ... ``` ## å¶ä» -
+å¦æåä¸åºè¯­é³ï¼è¯·æå¨å®è£ffmpeg -
+å½è¯­é³ï¼ä¸å¾ææé½ä¸ºTrueçæ¶åï¼åéæºåéä¸ç§ï¼é²æ­¢å·å±å·å°é£æ§
+## åè - [æºéåå¤](https://github.com/Special-Week/
+nonebot_plugin_smart_reply) - éç½®åæ³
```

