# Comparing `tmp/velikafkaclient-1.0.0.tar.gz` & `tmp/velikafkaclient-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.0.tar", last modified: Tue Jul  4 11:28:43 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.1.tar", last modified: Wed Jul  5 13:40:40 2023, max compression
```

## Comparing `velikafkaclient-1.0.0.tar` & `velikafkaclient-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 11:28:43.687027 velikafkaclient-1.0.0/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 velikafkaclient-1.0.0/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 11:28:43.686907 velikafkaclient-1.0.0/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 velikafkaclient-1.0.0/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 11:28:43.687057 velikafkaclient-1.0.0/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-04 11:28:32.000000 velikafkaclient-1.0.0/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 11:28:43.684865 velikafkaclient-1.0.0/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-04 09:18:27.000000 velikafkaclient-1.0.0/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-04 09:40:08.000000 velikafkaclient-1.0.0/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-04 09:42:26.000000 velikafkaclient-1.0.0/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 11:28:43.685981 velikafkaclient-1.0.0/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 velikafkaclient-1.0.0/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 velikafkaclient-1.0.0/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-04 10:05:53.000000 velikafkaclient-1.0.0/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-06-19 11:33:35.000000 velikafkaclient-1.0.0/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1173 2023-07-04 09:38:07.000000 velikafkaclient-1.0.0/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 11:28:43.686725 velikafkaclient-1.0.0/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 velikafkaclient-1.0.0/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 velikafkaclient-1.0.0/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-04 09:40:08.000000 velikafkaclient-1.0.0/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 11:28:43.685481 velikafkaclient-1.0.0/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 11:28:43.000000 velikafkaclient-1.0.0/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-04 11:28:43.000000 velikafkaclient-1.0.0/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 11:28:43.000000 velikafkaclient-1.0.0/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-04 11:28:43.000000 velikafkaclient-1.0.0/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.651752 velikafkaclient-1.0.1/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-05 13:40:40.651605 velikafkaclient-1.0.1/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-05 13:40:40.651793 velikafkaclient-1.0.1/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-05 13:40:31.000000 velikafkaclient-1.0.1/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.649869 velikafkaclient-1.0.1/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.650937 velikafkaclient-1.0.1/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1179 2023-07-05 13:39:50.000000 velikafkaclient-1.0.1/velikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.651375 velikafkaclient-1.0.1/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.650421 velikafkaclient-1.0.1/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.0/PKG-INFO` & `velikafkaclient-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.0/readme.md` & `velikafkaclient-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.0/velikafkaclient/consumer.py` & `velikafkaclient-1.0.1/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.0/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.1/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.0/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.1/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.0/velikafkaclient/producer.py` & `velikafkaclient-1.0.1/velikafkaclient/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 
     async def produce_event(self, topic: KafkaTopic, event: KafkaEvent):
         if topic not in self.kafka_topic_events.topic_event_models:
             raise InvalidEventTopicException(f"Topic {topic} not found")
         topic_event_model = self.kafka_topic_events.topic_event_models[topic]
         if not isinstance(event, topic_event_model):
             raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
-        await self.producer.send(topic, json.dumps(event.dict()).encode())
+        await self.producer.send(topic.value, json.dumps(event.dict()).encode())
```

### Comparing `velikafkaclient-1.0.0/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.1/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.0/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.0.1/velikafkaclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.0/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.1/velikafkaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

