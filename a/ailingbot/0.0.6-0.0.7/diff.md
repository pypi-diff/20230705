# Comparing `tmp/ailingbot-0.0.6.tar.gz` & `tmp/ailingbot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.6.tar", max compression
+gzip compressed data, was "ailingbot-0.0.7.tar", max compression
```

## Comparing `ailingbot-0.0.6.tar` & `ailingbot-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.6/LICENSE
--rw-r--r--   0        0        0    25129 2023-06-30 10:12:59.159678 ailingbot-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.6/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.6/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     3343 2023-06-30 08:53:14.045465 ailingbot-0.0.6/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.6/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.6/ailingbot/channels/dingtalk/agent.py
--rw-r--r--   0        0        0      799 2023-06-29 04:26:54.854394 ailingbot-0.0.6/ailingbot/channels/dingtalk/render.py
--rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.6/ailingbot/channels/dingtalk/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.6/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.6/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.6/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.6/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.6/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-30 09:13:29.198690 ailingbot-0.0.6/ailingbot/channels/slack/agent.py
--rw-r--r--   0        0        0     4299 2023-06-30 09:45:05.574135 ailingbot-0.0.6/ailingbot/channels/slack/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.6/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.6/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.6/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.6/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.6/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.6/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     2067 2023-06-29 05:19:20.215510 ailingbot-0.0.6/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.6/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.6/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     5436 2023-06-29 06:24:43.133890 ailingbot-0.0.6/ailingbot/chat/policies/langchain.py
--rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.6/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.6/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0     9511 2023-06-29 08:39:29.182555 ailingbot-0.0.6/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.6/ailingbot/cli/options.py
--rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.6/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.6/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.6/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.6/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.6/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.6/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.6/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1115 2023-06-30 10:13:19.023174 ailingbot-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    26697 1970-01-01 00:00:00.000000 ailingbot-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.7/LICENSE
+-rw-r--r--   0        0        0    30572 2023-07-05 05:45:21.083788 ailingbot-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.7/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.7/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     3343 2023-06-30 08:53:14.045465 ailingbot-0.0.7/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.7/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.7/ailingbot/channels/dingtalk/agent.py
+-rw-r--r--   0        0        0      758 2023-07-03 06:42:19.271831 ailingbot-0.0.7/ailingbot/channels/dingtalk/render.py
+-rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.7/ailingbot/channels/dingtalk/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.7/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.7/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.7/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.7/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.7/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-30 09:13:29.198690 ailingbot-0.0.7/ailingbot/channels/slack/agent.py
+-rw-r--r--   0        0        0     4291 2023-07-03 06:42:26.641074 ailingbot-0.0.7/ailingbot/channels/slack/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.7/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.7/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.7/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     1251 2023-07-03 06:41:46.703144 ailingbot-0.0.7/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.7/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.7/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-29 05:19:20.215510 ailingbot-0.0.7/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     2318 2023-07-03 06:37:54.116046 ailingbot-0.0.7/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.7/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     2147 2023-07-05 04:01:50.888063 ailingbot-0.0.7/ailingbot/chat/policies/conversation.py
+-rw-r--r--   0        0        0     3502 2023-07-05 04:01:50.889513 ailingbot-0.0.7/ailingbot/chat/policies/document_qa.py
+-rw-r--r--   0        0        0     1669 2023-07-05 04:01:50.890389 ailingbot-0.0.7/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.7/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0     8827 2023-07-05 04:01:50.891165 ailingbot-0.0.7/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.7/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     4051 2023-07-03 06:42:26.636556 ailingbot-0.0.7/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.7/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.7/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.7/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.7/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.7/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.7/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1115 2023-07-05 05:59:13.000686 ailingbot-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    32140 1970-01-01 00:00:00.000000 ailingbot-0.0.7/PKG-INFO
```

### Comparing `ailingbot-0.0.6/LICENSE` & `ailingbot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/README.md` & `ailingbot-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,104 @@
+🇨🇳[简体中文](https://github.com/ericzhang-cn/ailingbot/blob/main/README.md)
+🇬🇧[English](https://github.com/ericzhang-cn/ailingbot/blob/main/README_en.md)
+
+---
+
 ![Python package workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/python-package.yml/badge.svg)
 ![Pylint workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/pylint.yml/badge.svg)
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/logo.png" alt="AilingBot" width="300">
 </p>
 
 <p align="center"><b>AilingBot - 一站式解决方案，为你的IM机器人接入AI强大能力。</b></p>
 
+# 目录
+
+* [AilingBot是什么](#ailingbot是什么)
+* [特点](#特点)
+* [<g-emoji class="g-emoji" alias="rocket" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f680.png">🚀</g-emoji>快速开始](#快速开始)
+    * [5分钟启动一个AI聊天机器人](#5分钟启动一个ai聊天机器人)
+        * [通过Docker](#通过docker)
+        * [通过PIP](#通过pip)
+            * [安装](#安装)
+            * [生成配置文件](#生成配置文件)
+            * [启动机器人](#启动机器人)
+    * [接入企业微信](#接入企业微信)
+        * [通过Docker](#通过docker-1)
+        * [通过PIP](#通过pip-1)
+            * [安装](#安装-1)
+            * [生成配置文件](#生成配置文件-1)
+            * [修改配置文件](#修改配置文件)
+            * [启动服务](#启动服务)
+    * [接入飞书](#接入飞书)
+        * [通过Docker](#通过docker-2)
+        * [通过PIP](#通过pip-2)
+            * [安装](#安装-2)
+            * [生成配置文件](#生成配置文件-2)
+            * [修改配置文件](#修改配置文件-1)
+            * [启动服务](#启动服务-1)
+    * [接入钉钉](#接入钉钉)
+        * [通过Docker](#通过docker-3)
+        * [通过PIP](#通过pip-3)
+            * [安装](#安装-3)
+            * [生成配置文件](#生成配置文件-3)
+            * [修改配置文件](#修改配置文件-2)
+            * [启动服务](#启动服务-2)
+    * [接入Slack](#接入slack)
+        * [通过Docker](#通过docker-4)
+        * [通过PIP](#通过pip-4)
+            * [安装](#安装-4)
+            * [生成配置文件](#生成配置文件-4)
+            * [修改配置文件](#修改配置文件-3)
+            * [启动服务](#启动服务-3)
+* [<g-emoji class="g-emoji" alias="book" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d6.png">📖</g-emoji>使用指南](#使用指南)
+    * [主要流程](#主要流程)
+    * [主要概念](#主要概念)
+    * [配置](#配置)
+        * [配置方式](#配置方式)
+        * [配置映射关系](#配置映射关系)
+        * [配置项](#配置项)
+            * [通用](#通用)
+            * [内置会话策略配置](#内置会话策略配置)
+                * [conversation](#conversation)
+                * [document_qa](#document_qa)
+            * [模型配置](#模型配置)
+                * [OpenAI](#openai)
+            * [内置Channel配置](#内置channel配置)
+                * [企业微信](#企业微信)
+                * [飞书](#飞书)
+                * [钉钉](#钉钉)
+                * [Slack](#slack)
+    * [命令行工具](#命令行工具)
+        * [初始化配置文件（init）](#初始化配置文件init)
+            * [使用方法](#使用方法)
+            * [Options](#options)
+        * [查看当前配置（config）](#查看当前配置config)
+            * [使用方法](#使用方法-1)
+            * [Options](#options-1)
+        * [启动命令行机器人（chat）](#启动命令行机器人chat)
+            * [使用方法](#使用方法-2)
+            * [Options](#options-2)
+        * [启动Webhook服务（serve）](#启动webhook服务serve)
+            * [使用方法](#使用方法-3)
+            * [Options](#options-3)
+* [💻开发指南](#开发指南)
+    * [开发总则](#开发总则)
+    * [开发对话策略](#开发对话策略)
+    * [开发Channel](#开发channel)
+* [<g-emoji class="g-emoji" alias="thinking" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f914.png">🤔</g-emoji>常见问题](#常见问题)
+* [🎯发展计划](#发展计划)
+
 # AilingBot是什么
 
 AilingBot是一个开源的工程开发框架，同时也是IM机器人接入AI模型的一站式解决方案。通过AilingBot你可以：
 
-- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
+- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉、Slack等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
 - 🛠️**二次开发**：AilingBot提供了一套清晰的工程架构、接口定义和必需基础组件，无需从头开始重复开发大模型服务的工程框架，只需实现自己Chat
   Policy，并通过一些简单的配置，就能完成端到端的AI模型对IM机器人的赋能。同时也支持通过开发自己的Channel扩展到你自己的端（如自己的IM、Web应用或移动端应用）
 
 # 特点
 
 - 💯**开源&免费**：完全开源且免费
 - 📦**开箱即用**：无需开发，预置接入现有主流IM及AI模型的能力
@@ -91,15 +173,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_conversation \
+  -e AILINGBOT_POLICY__NAME=conversation \
   -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_CHANNEL__NAME=wechatwork \
   -e AILINGBOT_CHANNEL__CORPID={你的企业微信机器人corpid} \
   -e AILINGBOT_CHANNEL__CORPSECRET={你的企业微信机器人corpsecret} \
   -e AILINGBOT_CHANNEL__AGENTID={你的企业微信机器人agentid} \
   -e AILINGBOT_CHANNEL__TOKEN={你的企业微信机器人webhook token} \
@@ -168,15 +250,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_document_qa \
+  -e AILINGBOT_POLICY__NAME=document_qa \
   -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
   -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
   -e AILINGBOT_CHANNEL__NAME=feishu \
   -e AILINGBOT_CHANNEL__APP_ID={你的飞书机器人app id} \
   -e AILINGBOT_CHANNEL__APP_SECRET={你的飞书机器人app secret} \
@@ -211,15 +293,15 @@
 verification_token = "" # 填写真实信息
 ```
 
 将policy部分替换为文档问答策略：
 
 ```toml
 [policy]
-name = "lc_document_qa"
+name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 5
 ```
 
 最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
 
 ```toml
@@ -252,15 +334,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_conversation \
+  -e AILINGBOT_POLICY__NAME=conversation \
   -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_CHANNEL__NAME=dingtalk \
   -e AILINGBOT_CHANNEL__APP_KEY={你的钉钉机器人app key} \
   -e AILINGBOT_CHANNEL__APP_SECRET={你的钉钉机器人app secret} \
   -e AILINGBOT_CHANNEL__ROBOT_CODE={你的钉钉机器人robot code} \
   -p 8080:8080
@@ -315,15 +397,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_document_qa \
+  -e AILINGBOT_POLICY__NAME=document_qa \
   -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
   -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
   -e AILINGBOT_CHANNEL__NAME=slack \
   -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={你的Slack App webhook verification token} \
   -e AILINGBOT_CHANNEL__OAUTH_TOKEN={你的Slack App oauth token} \
@@ -356,15 +438,15 @@
 oauth_token = "" # 填写真实信息
 ```
 
 将policy部分替换为文档问答策略：
 
 ```toml
 [policy]
-name = "lc_document_qa"
+name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 5
 ```
 
 最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
 
 ```toml
@@ -380,15 +462,15 @@
 ```shell
 ailingbot serve
 ```
 
 最后我们需要去Slack的管理后台，将webhook地址配置好。
 飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/slack/event/`
 
-完成以上配置后，就可以在飞书中找到机器人，进行对话了：
+完成以上配置后，就可以在Slack中找到机器人，进行对话了：
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/slack-screenshot.png" alt="Slack机器人" width="1000"/>
 </p>
 
 # 📖使用指南
 
@@ -454,24 +536,24 @@
 |-----------|----------------------------------------------------------------------------------------|----------------------|---------------------------------|
 | 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）                              | lang                 | AILINGBOT_LANG                  |
 | 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones                    | tz                   | AILINGBOT_TZ                    |
 | 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                                                 | policy.name          | AILINGBOT_POLICY__NAME          |
 | Channel名称 | 预置Channel名称                                                                            | channel.name         | AILINGBOT_CHANNEL__NAME         |
 | Webhook路径 | 非预置Channel webhook的完整class路径                                                           | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
 | Agent路径   | 非预置Channel agent的完整class路径                                                             | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
-| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_CHANNEL__UVICORN__*   |
+| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_UVICORN__*            |
 
 配置示例：
 
 ```toml
 lang = "zh_CN"
 tz = "Asia/Shanghai"
 
 [policy]
-name = "lc_conversation"
+name = "conversation"
 # 更多policy配置
 
 [policy.llm]
 # 模型配置
 
 [channel]
 name = "wechatwork"
@@ -480,47 +562,47 @@
 [uvicorn]
 host = "0.0.0.0"
 port = 8080
 ```
 
 #### 内置会话策略配置
 
-##### lc_conversation
+##### conversation
 
-lc_conversation使用LangChain的Conversation作为会话策略，其效果为直接和LLM对话，且带有对话历史上下文，因此可以进行多轮会话。
+conversation使用LangChain的Conversation作为会话策略，其效果为直接和LLM对话，且带有对话历史上下文，因此可以进行多轮会话。
 
 | 配置项    | 说明          | TOML                | 环境变量                           |
 |--------|-------------|---------------------|--------------------------------|
 | 会话历史长度 | 表示保留多少轮历史会话 | policy.history_size | AILINGBOT_POLICY__HISTORY_SIZE |
 
 配置示例：
 
 ```toml
-# 使用lc_conversation策略，保留5轮历史会话
+# 使用conversation策略，保留5轮历史会话
 [policy]
-name = "lc_conversation"
+name = "conversation"
 history_size = 5
 ```
 
-##### lc_document_qa
+##### document_qa
 
-lc_document_qa使用LangChain的[Stuff](https://python.langchain.com/docs/modules/chains/document/stuff)作为对话策略。
+document_qa使用LangChain的[Stuff](https://python.langchain.com/docs/modules/chains/document/stuff)作为对话策略。
 用户可上传一个文档，然后针对文档内容进行提问。
 
 | 配置项     | 说明                                 | TOML                 | 环境变量                            |
 |---------|------------------------------------|----------------------|---------------------------------|
 | 文档切分块大小 | 对应LangChain Splitter的chunk_size    | policy.chunk_size    | AILINGBOT_POLICY__CHUNK_SIZE    |
 | 文档切重叠   | 对应LangChain Splitter的chunk_overlap | policy.chunk_overlap | AILINGBOT_POLICY__CHUNK_OVERLAP |
 
 配置示例：
 
 ```toml
-# 使用lc_document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
+# 使用document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
 [policy]
-name = "lc_document_qa"
+name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 0
 ```
 
 #### 模型配置
 
 模型配置与LangChain保持一致，下面给出示例。
@@ -591,14 +673,30 @@
 [channel]
 name = "dingtalk"
 app_key = "dingi**********wymdr"
 app_secret = "ombrcUp****************************************GL2AwObLjILUY1MzD"
 robot_code = "ding**********owymdr"
 ```
 
+##### Slack
+
+| 配置项                | 说明                         | TOML                       | 环境变量                                  |
+|--------------------|----------------------------|----------------------------|---------------------------------------|
+| Verification Token | Slack应用的verification token | channel.verification_token | AILINGBOT_CHANNEL__VERIFICATION_TOKEN |
+| OAuth token        | Slack应用的oauth token        | channel.oauth_token        | AILINGBOT_CHANNEL__OAUTH_TOKEN        |
+
+配置示例：
+
+```toml
+[channel]
+name = "slack"
+verification_token = "HzBGs1**********39gZG2P0"
+oauth_token = "xoxb-2**********27-5**********23-if**********H1QEGUItx2Yz"
+```
+
 ## 命令行工具
 
 ### 初始化配置文件（init）
 
 #### 使用方法
 
 `init`命令将在当前目录生成配置文件settings.toml。默认情况下，将以交互方式询问用户，
@@ -709,33 +807,49 @@
 
 ## 开发Channel
 
 TBD
 
 # 🤔常见问题
 
-- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的lc_document_qa策略
+- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的document_qa策略
 - 各个IM的webhook需要公网IP，如果你暂时没有，可以考虑通过"内网穿透"方案在本地测试，具体方法请参考网上资料
+- 我们预期chat policy应该是无状态的，状态应该保存在外部，但是具体实现时policy仍然有可能存在本地状态（如在本地变量中存储了对话历史）。因此当uvicorn有多个worker进程时，由于没一个进程都有单独的chat
+  policy实例，所以这些本地状态无法共享，而同一个用户的请求可能会被不同worker响应，因此导致预期之外的行为。要避免这种行为，请保证一下两个条件至少有一个被满足：
+    - Chat policy不使用本地状态
+    - 只启动一个uvicorn worker
 
 # 🎯发展计划
 
 - [ ] 提供完善的使用文档和开发者文档
 - [ ] 支持更多的Channel
     - [x] 企业微信
     - [x] 飞书
     - [x] 钉钉
-    - [ ] Slack
+    - [x] Slack
+- [ ] 更多请求消息类型的支持
+    - [x] 文本请求
+    - [ ] 图片请求
+    - [x] 文件请求
+- [ ] 更多响应消息类型的支持
+    - [x] 文本响应
+    - [ ] 图片响应
+    - [ ] 文件响应
+    - [ ] Markdown响应
+    - [ ] 表格响应
 - [ ] 开发更多的开箱即用的对话策略
     - [x] 多轮会话策略
-    - [ ] 文档问答策略
+    - [x] 文档问答策略
     - [ ] 数据库问答策略
     - [ ] 在线搜索问答策略
+- [ ] 支持通过HTTP调用独立的对话策略服务
 - [ ] 基础组件抽象
     - [ ] 大语言模型
     - [ ] 知识库
+    - [ ] Tools
 - [ ] 支持本地模型部署
     - [ ] ChatGLM-6B
 - [ ] 支持通过API调用
 - [ ] Web管理后台及可视化配置管理
 - [x] 提供基于Docker容器的部署能力
 - [ ] 增强系统的可观测性和可治理性
 - [ ] 完善的测试用例
```

### Comparing `ailingbot-0.0.6/ailingbot/channels/channel.py` & `ailingbot-0.0.7/ailingbot/channels/channel.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/dingtalk/agent.py` & `ailingbot-0.0.7/ailingbot/channels/dingtalk/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/dingtalk/render.py` & `ailingbot-0.0.7/ailingbot/channels/dingtalk/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import functools
-import json
 
 from ailingbot.chat.messages import (
     ResponseMessage,
     TextResponseMessage,
-    FallbackResponseMessage,
 )
 
 
 @functools.singledispatch
 async def render(response: ResponseMessage) -> tuple[dict, str]:
     """Virtual function of all response message renders.
```

### Comparing `ailingbot-0.0.6/ailingbot/channels/dingtalk/webhook.py` & `ailingbot-0.0.7/ailingbot/channels/dingtalk/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.7/ailingbot/channels/feishu/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/feishu/render.py` & `ailingbot-0.0.7/ailingbot/channels/feishu/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/feishu/webhook.py` & `ailingbot-0.0.7/ailingbot/channels/feishu/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/slack/agent.py` & `ailingbot-0.0.7/ailingbot/channels/slack/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/slack/webhook.py` & `ailingbot-0.0.7/ailingbot/channels/slack/webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         @self.app.on_event('shutdown')
         async def shutdown() -> None:
             await self.agent.finalize()
             await self.bot.finalize()
 
         @self.app.post('/webhook/slack/event/', status_code=status.HTTP_200_OK)
         async def handle_event(
-                request: Request,
-                background_tasks: BackgroundTasks,
+            request: Request,
+            background_tasks: BackgroundTasks,
         ) -> dict | Response:
             """Handle the event request from Slack.
 
             :return: Empty dict.
             :rtype: dict
             """
             message = await request.json()
```

### Comparing `ailingbot-0.0.6/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.7/ailingbot/channels/wechatwork/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.7/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.7/ailingbot/chat/chatbot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,74 @@
 from __future__ import annotations
 
-import functools
+import asyncio
+import typing
+import uuid
+
+from loguru import logger
 
 from ailingbot.chat.messages import (
-    ResponseMessage,
-    TextResponseMessage,
+    RequestMessage,
     FallbackResponseMessage,
-    InputResponseMessage,
-    OptionsResponseMessage,
+    ResponseMessage,
 )
+from ailingbot.chat.policy import ChatPolicy
+from ailingbot.config import settings
+from ailingbot.shared.abc import AbstractAsyncComponent
+
+
+class ChatBot(AbstractAsyncComponent):
+    """ChatBot is core component that responsible for retrieve request and make response."""
+
+    def __init__(
+        self,
+        *,
+        debug: bool = False,
+    ):
+        super(ChatBot, self).__init__()
+
+        self.debug = debug
+
+        self.locks: dict[str, asyncio.Lock] = {}
+        self.policy: typing.Optional[ChatPolicy] = None
+
+    async def chat(
+        self, *, conversation_id: str, message: RequestMessage
+    ) -> ResponseMessage:
+        """Run chat pipeline, and replies messages to sender.
+
+        :param conversation_id: Conversation id.
+        :type conversation_id: str
+        :param message: Reqeust message.
+        :type message: RequestMessage
+        """
+        if conversation_id not in self.locks:
+            self.locks[conversation_id] = asyncio.Lock()
+        lock = self.locks[conversation_id]
+
+        async with lock:
+            try:
+                r = await self.policy.respond(
+                    conversation_id=conversation_id, message=message
+                )
+            except Exception as e:
+                logger.error(e)
+                r = FallbackResponseMessage(
+                    reason=str(e),
+                )
+            r.uuid = str(uuid.uuid4())
+            r.ack_uuid = message.uuid
+            r.receiver_id = message.sender_id
+            r.scope = message.scope
+            r.echo = message.echo
+
+            return r
+
+    async def _initialize(self) -> None:
+        self.policy = ChatPolicy.get_policy(
+            name=settings.policy.name,
+            debug=self.debug,
+        )
+        await self.policy.initialize()
 
-
-@functools.singledispatch
-async def render(response: ResponseMessage) -> tuple[dict, str]:
-    """Virtual function of all response message renders.
-
-    Converts response message to Wechatwork content.
-
-    :param response: Response message.
-    :type response: ResponseMessage
-    :return: Render result and Wechatwork message type.
-    :rtype: typing.Tuple[dict, str]:
-    """
-    raise NotImplementedError
-
-
-@render.register
-async def _render(response: TextResponseMessage) -> tuple[dict, str]:
-    """Renders text response message."""
-    content = {
-        'text': {
-            'content': response.text,
-        }
-    }
-    message_type = 'text'
-    return content, message_type
-
-
-@render.register
-async def _render(response: FallbackResponseMessage) -> tuple[dict, str]:
-    """Renders error fallback response message."""
-    content = {
-        'markdown': {
-            'content': f"""<font color="warning">Error occurred</font>
-Cause: {response.reason}
-Suggestion: {response.suggestion}"""
-        }
-    }
-    message_type = 'markdown'
-    return content, message_type
-
-
-@render.register
-async def _render(response: InputResponseMessage) -> tuple[dict, str]:
-    """Renders input prompt response message."""
-    content = {
-        'text': {
-            'content': response.title,
-        }
-    }
-    message_type = 'text'
-    return content, message_type
-
-
-@render.register
-async def _render(response: OptionsResponseMessage) -> tuple[dict, str]:
-    """Renders input prompt response message."""
-    content = {
-        'template_card': {
-            'card_type': 'vote_interaction',
-            'main_title': {
-                'title': response.title,
-            },
-            'task_id': response.uuid,
-            'checkbox': {
-                'question_key': response.uuid,
-                'option_list': [
-                    {
-                        'id': x.value,
-                        'text': x.text,
-                        'is_checked': False,
-                    }
-                    for x in response.options
-                ],
-                'mode': 0,
-            },
-        }
-    }
-    message_type = 'template_card'
-    return content, message_type
+    async def _finalize(self):
+        await self.policy.finalize()
```

### Comparing `ailingbot-0.0.6/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.7/ailingbot/channels/wechatwork/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/chat/messages.py` & `ailingbot-0.0.7/ailingbot/chat/messages.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,31 +39,26 @@
     """File request message."""
 
     content: bytes
     file_type: str
     file_name: str
 
 
-class InputRequestMessage(RequestMessage):
-    """Input request message."""
-
-    value: typing.Any = None
-
-
 class ResponseMessage(BaseModel, abc.ABC):
     """Base class of response messages."""
 
     uuid: str = ''
     ack_uuid: str = ''
     receiver_id: typing.Union[str, list[str]] = ''
     scope: typing.Optional[MessageScope] = None
     meta: dict = {}
     echo: dict = {}
 
     def _downgrade(self) -> str:
+        """Default downgrade method: use the JSON representation."""
         return self.json(ensure_ascii=False)
 
     def downgrade_to_text_message(self) -> TextResponseMessage:
         """When the channel does not support rendering this type of message, how to downgrade it to a text message."""
         return TextResponseMessage(
             uuid=self.uuid,
             ack_uuid=self.ack_uuid,
@@ -71,89 +66,35 @@
             scope=self.scope,
             meta=self.meta,
             echo=self.echo,
             text=self._downgrade(),
         )
 
 
-class ContentResponseMessage(ResponseMessage, abc.ABC):
-    """Base class of response message that outputs content."""
-
-    pass
-
-
-class SilenceResponseMessage(ContentResponseMessage):
+class SilenceResponseMessage(ResponseMessage):
     """Response message that outputs nothing."""
 
     def _downgrade(self) -> str:
         return ''
 
 
-class TextResponseMessage(ContentResponseMessage):
+class TextResponseMessage(ResponseMessage):
     """Plain text response message."""
 
     text: str = ''
 
     def _downgrade(self) -> str:
         return self.text
 
 
-class TabularResponseMessage(ContentResponseMessage):
-    """Tabular response message."""
-
-    title: str = ''
-    headers: list[str] = []
-    data: list[list] = []
-
-
-class FallbackResponseMessage(ContentResponseMessage):
+class FallbackResponseMessage(ResponseMessage):
     """Fallback response message.
 
     Send this message when error occurred.
     """
 
     reason: str = ''
     suggestion: str = ''
 
     def _downgrade(self) -> str:
         return f"""{self.reason}
 {self.suggestion}"""
-
-
-class FormResponseMessage(ResponseMessage, abc.ABC):
-    """Base class of form response messages."""
-
-    title: str = ''
-
-
-class InputResponseMessage(FormResponseMessage):
-    """Input prompt response message.
-
-    Ask for user input.
-    """
-
-    required: bool = True
-    visible: bool = True
-
-    def _downgrade(self) -> str:
-        return self.title
-
-
-class Option(BaseModel):
-    """Option for OptionsResponseMessage."""
-
-    text: str = ''
-    value: typing.Any = None
-
-
-class OptionsResponseMessage(FormResponseMessage):
-    """Options prompt response message.
-
-    Give options for the user to make a choice.
-    """
-
-    options: list[Option] = []
-
-    def _downgrade(self) -> str:
-        nl = '\n'
-        return f"""{self.title}
-{nl.join([f'{x.text}[{str(x.value)}]' for x in self.options])}"""
```

### Comparing `ailingbot-0.0.6/ailingbot/chat/policies/langchain.py` & `ailingbot-0.0.7/ailingbot/chat/policies/document_qa.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,56 @@
 import copy
 import tempfile
 
-from langchain import ConversationChain
 from langchain.chains import RetrievalQA
 from langchain.chains.base import Chain
 from langchain.document_loaders import PyPDFLoader
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms.loading import load_llm_from_config
-from langchain.memory import ConversationBufferWindowMemory
-from langchain.memory.chat_memory import BaseChatMemory
 from langchain.text_splitter import CharacterTextSplitter
 from langchain.vectorstores import Chroma
 from langchain.vectorstores.base import VectorStoreRetriever
 
-import ailingbot
 from ailingbot.chat.messages import (
     RequestMessage,
     ResponseMessage,
     TextRequestMessage,
-    TextResponseMessage,
     FallbackResponseMessage,
+    TextResponseMessage,
     FileRequestMessage,
 )
 from ailingbot.chat.policy import ChatPolicy
 from ailingbot.config import settings
 from ailingbot.shared.errors import ChatPolicyError
 
 
-class LCConversationChatPolicy(ChatPolicy):
-    """Having a direct conversation with a large language model."""
-
-    def __init__(
-        self,
-        *,
-        debug: bool = False,
-    ):
-        super(LCConversationChatPolicy, self).__init__(
-            debug=debug,
-        )
-
-        llm_config = copy.deepcopy(settings.policy.llm)
-        llm = load_llm_from_config(llm_config)
-        self.chain = ConversationChain(llm=llm, verbose=debug)
-        self.history_size = settings.policy.get('history_size', 5)
-        self.memories: dict[str, BaseChatMemory] = {}
-
-    async def _load_memory(self, *, conversation_id: str) -> BaseChatMemory:
-        """Load memory for conversation. Create a new memory if not exists.
-
-        :param conversation_id: Conversation ID.
-        :type conversation_id: str
-        :return: Chat memory.
-        :rtype: BaseChatMemory
-        """
-        if conversation_id not in self.memories:
-            self.memories[conversation_id] = ConversationBufferWindowMemory(
-                k=self.history_size
-            )
-        return self.memories[conversation_id]
-
-    async def respond(
-        self, *, conversation_id: str, message: RequestMessage
-    ) -> ResponseMessage:
-        if not isinstance(message, TextRequestMessage):
-            response = FallbackResponseMessage()
-            response.reason = '不支持的消息类型'
-        else:
-            if conversation_id not in self.chain:
-                self.chain.memory = await self._load_memory(
-                    conversation_id=conversation_id
-                )
-            response = TextResponseMessage()
-            response.text = await self.chain.arun(message.text)
-
-        return response
-
-
-class LCDocumentQAPolicy(ChatPolicy):
+class DocumentQAPolicy(ChatPolicy):
     """Question-Answering based on documents."""
 
     def __init__(
         self,
         *,
         debug: bool = False,
     ):
-        super(LCDocumentQAPolicy, self).__init__(
+        super().__init__(
             debug=debug,
         )
 
         llm_config = copy.deepcopy(settings.policy.llm)
         self.llm = load_llm_from_config(llm_config)
         self.chains: dict[str, Chain] = {}
         self.chunk_size = settings.policy.get('chunk_size', 1000)
         self.chunk_overlap = settings.policy.get('chunk_overlap', 0)
 
     def _build_documents_index(
         self, *, content: bytes, file_type: str
     ) -> VectorStoreRetriever:
         """Load document and build index."""
         if file_type.lower() != 'pdf':
-            raise ailingbot.shared.errors.ChatPolicyError(
+            raise ChatPolicyError(
                 reason='目前只支持PDF文档',
                 suggestion='请上传PDF文档',
             )
 
         with tempfile.NamedTemporaryFile(delete=True) as tf:
             tf.write(content)
             loader = PyPDFLoader(file_path=tf.name)
```

### Comparing `ailingbot-0.0.6/ailingbot/chat/policy.py` & `ailingbot-0.0.7/ailingbot/chat/policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,23 +35,23 @@
         :param name: Built-in policy name or full path of policy class.
         :type name: str
         :param debug:
         :type debug:
         :return: Policy instance.
         :rtype: ChatPolicy
         """
-        if name.lower() == 'lc_conversation':
-            from ailingbot.chat.policies.langchain import (
-                LCConversationChatPolicy,
+        if name.lower() == 'conversation':
+            from ailingbot.chat.policies.conversation import (
+                ConversationChatPolicy,
             )
 
-            instance = LCConversationChatPolicy(debug=debug)
-        elif name.lower() == 'lc_document_qa':
-            from ailingbot.chat.policies.langchain import (
-                LCDocumentQAPolicy,
+            instance = ConversationChatPolicy(debug=debug)
+        elif name.lower() == 'document_qa':
+            from ailingbot.chat.policies.document_qa import (
+                DocumentQAPolicy,
             )
 
-            instance = LCDocumentQAPolicy(debug=debug)
+            instance = DocumentQAPolicy(debug=debug)
         else:
             instance = get_class_dynamically(name)(debug=debug)
 
         return instance
```

### Comparing `ailingbot-0.0.6/ailingbot/cli/cli.py` & `ailingbot-0.0.7/ailingbot/cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 
 import ailingbot.shared.errors
 from ailingbot.channels.channel import ChannelWebhookFactory
 from ailingbot.chat.chatbot import ChatBot
 from ailingbot.chat.messages import (
     TextRequestMessage,
     FallbackResponseMessage,
-    OptionsResponseMessage,
-    InputRequestMessage,
-    InputResponseMessage,
     MessageScope,
 )
 from ailingbot.cli import options
 from ailingbot.cli.render import render, display_radio_prompt
 from ailingbot.config import settings
 
 
@@ -129,30 +126,15 @@
 
         # Sends request and processes different types response.
         try:
             response = await chatbot.chat(
                 conversation_id=conversation_id, message=request
             )
             request = None
-            if isinstance(response, OptionsResponseMessage):
-                selected_value = await render(response)
-                if selected_value is None:
-                    continue
-                request = InputRequestMessage(
-                    value=selected_value,
-                )
-            elif isinstance(response, InputResponseMessage):
-                text = await render(response)
-                if text is None:
-                    continue
-                request = InputRequestMessage(
-                    value=text,
-                )
-            else:
-                await render(response)
+            await render(response)
         except ailingbot.shared.errors.AilingBotError as e:
             if e.critical:
                 raise click.exceptions.ClickException(e.reason)
             else:
                 request = None
 
                 response = FallbackResponseMessage(
@@ -241,15 +223,15 @@
         'uvicorn': {
             'host': '0.0.0.0',
             'port': 8080,
         },
     }
     if silence:
         config['policy'] = {
-            'name': 'lc_conversation',
+            'name': 'conversation',
             'history_size': 5,
             'llm': {
                 '_type': 'openai',
                 'model_name': 'gpt-3.5-turbo',
                 'openai_api_key': '',
                 'temperature': 0,
             },
@@ -264,35 +246,35 @@
         }
     else:
         policy = await display_radio_prompt(
             title='Select chat policy:',
             values=[
                 (x, x)
                 for x in [
-                    'lc_conversation',
-                    'lc_document_qa',
+                    'conversation',
+                    'document_qa',
                     'Configure Later',
                 ]
             ],
             cancel_value='Configure Later',
         )
-        if policy == 'lc_conversation':
+        if policy == 'conversation':
             config['policy'] = {
-                'name': 'lc_conversation',
+                'name': 'conversation',
                 'history_size': 5,
                 'llm': {
                     '_type': 'openai',
                     'model_name': 'gpt-3.5-turbo-16k',
                     'openai_api_key': '',
                     'temperature': 0,
                 },
             }
-        elif policy == 'lc_document_qa':
+        elif policy == 'document_qa':
             config['policy'] = {
-                'name': 'lc_document_qa',
+                'name': 'document_qa',
                 'chunk_size': 1000,
                 'chunk_overlap': 0,
                 'llm': {
                     '_type': 'openai',
                     'model_name': 'gpt-3.5-turbo-16k',
                     'openai_api_key': '',
                     'temperature': 0,
```

### Comparing `ailingbot-0.0.6/ailingbot/cli/options.py` & `ailingbot-0.0.7/ailingbot/cli/options.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/config.py` & `ailingbot-0.0.7/ailingbot/config.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/shared/abc.py` & `ailingbot-0.0.7/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/shared/errors.py` & `ailingbot-0.0.7/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/ailingbot/shared/misc.py` & `ailingbot-0.0.7/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.6/pyproject.toml` & `ailingbot-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.6"
+version = "0.0.7"
 description = "An all-in-one solution to empower your IM bot with AI."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `ailingbot-0.0.6/PKG-INFO` & `ailingbot-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailingbot
-Version: 0.0.6
+Version: 0.0.7
 Summary: An all-in-one solution to empower your IM bot with AI.
 License: MIT
 Author: ericzhang-cn
 Author-email: ericzhang.buaa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,29 +34,111 @@
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Requires-Dist: uvicorn (>=0.19.0,<0.20.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
+🇨🇳[简体中文](https://github.com/ericzhang-cn/ailingbot/blob/main/README.md)
+🇬🇧[English](https://github.com/ericzhang-cn/ailingbot/blob/main/README_en.md)
+
+---
+
 ![Python package workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/python-package.yml/badge.svg)
 ![Pylint workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/pylint.yml/badge.svg)
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/logo.png" alt="AilingBot" width="300">
 </p>
 
 <p align="center"><b>AilingBot - 一站式解决方案，为你的IM机器人接入AI强大能力。</b></p>
 
+# 目录
+
+* [AilingBot是什么](#ailingbot是什么)
+* [特点](#特点)
+* [<g-emoji class="g-emoji" alias="rocket" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f680.png">🚀</g-emoji>快速开始](#快速开始)
+    * [5分钟启动一个AI聊天机器人](#5分钟启动一个ai聊天机器人)
+        * [通过Docker](#通过docker)
+        * [通过PIP](#通过pip)
+            * [安装](#安装)
+            * [生成配置文件](#生成配置文件)
+            * [启动机器人](#启动机器人)
+    * [接入企业微信](#接入企业微信)
+        * [通过Docker](#通过docker-1)
+        * [通过PIP](#通过pip-1)
+            * [安装](#安装-1)
+            * [生成配置文件](#生成配置文件-1)
+            * [修改配置文件](#修改配置文件)
+            * [启动服务](#启动服务)
+    * [接入飞书](#接入飞书)
+        * [通过Docker](#通过docker-2)
+        * [通过PIP](#通过pip-2)
+            * [安装](#安装-2)
+            * [生成配置文件](#生成配置文件-2)
+            * [修改配置文件](#修改配置文件-1)
+            * [启动服务](#启动服务-1)
+    * [接入钉钉](#接入钉钉)
+        * [通过Docker](#通过docker-3)
+        * [通过PIP](#通过pip-3)
+            * [安装](#安装-3)
+            * [生成配置文件](#生成配置文件-3)
+            * [修改配置文件](#修改配置文件-2)
+            * [启动服务](#启动服务-2)
+    * [接入Slack](#接入slack)
+        * [通过Docker](#通过docker-4)
+        * [通过PIP](#通过pip-4)
+            * [安装](#安装-4)
+            * [生成配置文件](#生成配置文件-4)
+            * [修改配置文件](#修改配置文件-3)
+            * [启动服务](#启动服务-3)
+* [<g-emoji class="g-emoji" alias="book" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d6.png">📖</g-emoji>使用指南](#使用指南)
+    * [主要流程](#主要流程)
+    * [主要概念](#主要概念)
+    * [配置](#配置)
+        * [配置方式](#配置方式)
+        * [配置映射关系](#配置映射关系)
+        * [配置项](#配置项)
+            * [通用](#通用)
+            * [内置会话策略配置](#内置会话策略配置)
+                * [conversation](#conversation)
+                * [document_qa](#document_qa)
+            * [模型配置](#模型配置)
+                * [OpenAI](#openai)
+            * [内置Channel配置](#内置channel配置)
+                * [企业微信](#企业微信)
+                * [飞书](#飞书)
+                * [钉钉](#钉钉)
+                * [Slack](#slack)
+    * [命令行工具](#命令行工具)
+        * [初始化配置文件（init）](#初始化配置文件init)
+            * [使用方法](#使用方法)
+            * [Options](#options)
+        * [查看当前配置（config）](#查看当前配置config)
+            * [使用方法](#使用方法-1)
+            * [Options](#options-1)
+        * [启动命令行机器人（chat）](#启动命令行机器人chat)
+            * [使用方法](#使用方法-2)
+            * [Options](#options-2)
+        * [启动Webhook服务（serve）](#启动webhook服务serve)
+            * [使用方法](#使用方法-3)
+            * [Options](#options-3)
+* [💻开发指南](#开发指南)
+    * [开发总则](#开发总则)
+    * [开发对话策略](#开发对话策略)
+    * [开发Channel](#开发channel)
+* [<g-emoji class="g-emoji" alias="thinking" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f914.png">🤔</g-emoji>常见问题](#常见问题)
+* [🎯发展计划](#发展计划)
+
 # AilingBot是什么
 
 AilingBot是一个开源的工程开发框架，同时也是IM机器人接入AI模型的一站式解决方案。通过AilingBot你可以：
 
-- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
+- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉、Slack等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
 - 🛠️**二次开发**：AilingBot提供了一套清晰的工程架构、接口定义和必需基础组件，无需从头开始重复开发大模型服务的工程框架，只需实现自己Chat
   Policy，并通过一些简单的配置，就能完成端到端的AI模型对IM机器人的赋能。同时也支持通过开发自己的Channel扩展到你自己的端（如自己的IM、Web应用或移动端应用）
 
 # 特点
 
 - 💯**开源&免费**：完全开源且免费
 - 📦**开箱即用**：无需开发，预置接入现有主流IM及AI模型的能力
@@ -131,15 +213,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_conversation \
+  -e AILINGBOT_POLICY__NAME=conversation \
   -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_CHANNEL__NAME=wechatwork \
   -e AILINGBOT_CHANNEL__CORPID={你的企业微信机器人corpid} \
   -e AILINGBOT_CHANNEL__CORPSECRET={你的企业微信机器人corpsecret} \
   -e AILINGBOT_CHANNEL__AGENTID={你的企业微信机器人agentid} \
   -e AILINGBOT_CHANNEL__TOKEN={你的企业微信机器人webhook token} \
@@ -208,15 +290,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_document_qa \
+  -e AILINGBOT_POLICY__NAME=document_qa \
   -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
   -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
   -e AILINGBOT_CHANNEL__NAME=feishu \
   -e AILINGBOT_CHANNEL__APP_ID={你的飞书机器人app id} \
   -e AILINGBOT_CHANNEL__APP_SECRET={你的飞书机器人app secret} \
@@ -251,15 +333,15 @@
 verification_token = "" # 填写真实信息
 ```
 
 将policy部分替换为文档问答策略：
 
 ```toml
 [policy]
-name = "lc_document_qa"
+name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 5
 ```
 
 最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
 
 ```toml
@@ -292,15 +374,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_conversation \
+  -e AILINGBOT_POLICY__NAME=conversation \
   -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_CHANNEL__NAME=dingtalk \
   -e AILINGBOT_CHANNEL__APP_KEY={你的钉钉机器人app key} \
   -e AILINGBOT_CHANNEL__APP_SECRET={你的钉钉机器人app secret} \
   -e AILINGBOT_CHANNEL__ROBOT_CODE={你的钉钉机器人robot code} \
   -p 8080:8080
@@ -355,15 +437,15 @@
 ### 通过Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=lc_document_qa \
+  -e AILINGBOT_POLICY__NAME=document_qa \
   -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
   -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
   -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
   -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
   -e AILINGBOT_CHANNEL__NAME=slack \
   -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={你的Slack App webhook verification token} \
   -e AILINGBOT_CHANNEL__OAUTH_TOKEN={你的Slack App oauth token} \
@@ -396,15 +478,15 @@
 oauth_token = "" # 填写真实信息
 ```
 
 将policy部分替换为文档问答策略：
 
 ```toml
 [policy]
-name = "lc_document_qa"
+name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 5
 ```
 
 最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
 
 ```toml
@@ -420,15 +502,15 @@
 ```shell
 ailingbot serve
 ```
 
 最后我们需要去Slack的管理后台，将webhook地址配置好。
 飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/slack/event/`
 
-完成以上配置后，就可以在飞书中找到机器人，进行对话了：
+完成以上配置后，就可以在Slack中找到机器人，进行对话了：
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/slack-screenshot.png" alt="Slack机器人" width="1000"/>
 </p>
 
 # 📖使用指南
 
@@ -494,24 +576,24 @@
 |-----------|----------------------------------------------------------------------------------------|----------------------|---------------------------------|
 | 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）                              | lang                 | AILINGBOT_LANG                  |
 | 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones                    | tz                   | AILINGBOT_TZ                    |
 | 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                                                 | policy.name          | AILINGBOT_POLICY__NAME          |
 | Channel名称 | 预置Channel名称                                                                            | channel.name         | AILINGBOT_CHANNEL__NAME         |
 | Webhook路径 | 非预置Channel webhook的完整class路径                                                           | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
 | Agent路径   | 非预置Channel agent的完整class路径                                                             | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
-| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_CHANNEL__UVICORN__*   |
+| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_UVICORN__*            |
 
 配置示例：
 
 ```toml
 lang = "zh_CN"
 tz = "Asia/Shanghai"
 
 [policy]
-name = "lc_conversation"
+name = "conversation"
 # 更多policy配置
 
 [policy.llm]
 # 模型配置
 
 [channel]
 name = "wechatwork"
@@ -520,47 +602,47 @@
 [uvicorn]
 host = "0.0.0.0"
 port = 8080
 ```
 
 #### 内置会话策略配置
 
-##### lc_conversation
+##### conversation
 
-lc_conversation使用LangChain的Conversation作为会话策略，其效果为直接和LLM对话，且带有对话历史上下文，因此可以进行多轮会话。
+conversation使用LangChain的Conversation作为会话策略，其效果为直接和LLM对话，且带有对话历史上下文，因此可以进行多轮会话。
 
 | 配置项    | 说明          | TOML                | 环境变量                           |
 |--------|-------------|---------------------|--------------------------------|
 | 会话历史长度 | 表示保留多少轮历史会话 | policy.history_size | AILINGBOT_POLICY__HISTORY_SIZE |
 
 配置示例：
 
 ```toml
-# 使用lc_conversation策略，保留5轮历史会话
+# 使用conversation策略，保留5轮历史会话
 [policy]
-name = "lc_conversation"
+name = "conversation"
 history_size = 5
 ```
 
-##### lc_document_qa
+##### document_qa
 
-lc_document_qa使用LangChain的[Stuff](https://python.langchain.com/docs/modules/chains/document/stuff)作为对话策略。
+document_qa使用LangChain的[Stuff](https://python.langchain.com/docs/modules/chains/document/stuff)作为对话策略。
 用户可上传一个文档，然后针对文档内容进行提问。
 
 | 配置项     | 说明                                 | TOML                 | 环境变量                            |
 |---------|------------------------------------|----------------------|---------------------------------|
 | 文档切分块大小 | 对应LangChain Splitter的chunk_size    | policy.chunk_size    | AILINGBOT_POLICY__CHUNK_SIZE    |
 | 文档切重叠   | 对应LangChain Splitter的chunk_overlap | policy.chunk_overlap | AILINGBOT_POLICY__CHUNK_OVERLAP |
 
 配置示例：
 
 ```toml
-# 使用lc_document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
+# 使用document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
 [policy]
-name = "lc_document_qa"
+name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 0
 ```
 
 #### 模型配置
 
 模型配置与LangChain保持一致，下面给出示例。
@@ -631,14 +713,30 @@
 [channel]
 name = "dingtalk"
 app_key = "dingi**********wymdr"
 app_secret = "ombrcUp****************************************GL2AwObLjILUY1MzD"
 robot_code = "ding**********owymdr"
 ```
 
+##### Slack
+
+| 配置项                | 说明                         | TOML                       | 环境变量                                  |
+|--------------------|----------------------------|----------------------------|---------------------------------------|
+| Verification Token | Slack应用的verification token | channel.verification_token | AILINGBOT_CHANNEL__VERIFICATION_TOKEN |
+| OAuth token        | Slack应用的oauth token        | channel.oauth_token        | AILINGBOT_CHANNEL__OAUTH_TOKEN        |
+
+配置示例：
+
+```toml
+[channel]
+name = "slack"
+verification_token = "HzBGs1**********39gZG2P0"
+oauth_token = "xoxb-2**********27-5**********23-if**********H1QEGUItx2Yz"
+```
+
 ## 命令行工具
 
 ### 初始化配置文件（init）
 
 #### 使用方法
 
 `init`命令将在当前目录生成配置文件settings.toml。默认情况下，将以交互方式询问用户，
@@ -749,33 +847,49 @@
 
 ## 开发Channel
 
 TBD
 
 # 🤔常见问题
 
-- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的lc_document_qa策略
+- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的document_qa策略
 - 各个IM的webhook需要公网IP，如果你暂时没有，可以考虑通过"内网穿透"方案在本地测试，具体方法请参考网上资料
+- 我们预期chat policy应该是无状态的，状态应该保存在外部，但是具体实现时policy仍然有可能存在本地状态（如在本地变量中存储了对话历史）。因此当uvicorn有多个worker进程时，由于没一个进程都有单独的chat
+  policy实例，所以这些本地状态无法共享，而同一个用户的请求可能会被不同worker响应，因此导致预期之外的行为。要避免这种行为，请保证一下两个条件至少有一个被满足：
+    - Chat policy不使用本地状态
+    - 只启动一个uvicorn worker
 
 # 🎯发展计划
 
 - [ ] 提供完善的使用文档和开发者文档
 - [ ] 支持更多的Channel
     - [x] 企业微信
     - [x] 飞书
     - [x] 钉钉
-    - [ ] Slack
+    - [x] Slack
+- [ ] 更多请求消息类型的支持
+    - [x] 文本请求
+    - [ ] 图片请求
+    - [x] 文件请求
+- [ ] 更多响应消息类型的支持
+    - [x] 文本响应
+    - [ ] 图片响应
+    - [ ] 文件响应
+    - [ ] Markdown响应
+    - [ ] 表格响应
 - [ ] 开发更多的开箱即用的对话策略
     - [x] 多轮会话策略
-    - [ ] 文档问答策略
+    - [x] 文档问答策略
     - [ ] 数据库问答策略
     - [ ] 在线搜索问答策略
+- [ ] 支持通过HTTP调用独立的对话策略服务
 - [ ] 基础组件抽象
     - [ ] 大语言模型
     - [ ] 知识库
+    - [ ] Tools
 - [ ] 支持本地模型部署
     - [ ] ChatGLM-6B
 - [ ] 支持通过API调用
 - [ ] Web管理后台及可视化配置管理
 - [x] 提供基于Docker容器的部署能力
 - [ ] 增强系统的可观测性和可治理性
 - [ ] 完善的测试用例
```

