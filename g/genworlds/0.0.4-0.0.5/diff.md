# Comparing `tmp/genworlds-0.0.4.tar.gz` & `tmp/genworlds-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genworlds-0.0.4.tar", max compression
+gzip compressed data, was "genworlds-0.0.5.tar", max compression
```

## Comparing `genworlds-0.0.4.tar` & `genworlds-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.372707 genworlds-0.0.4/genworlds/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.373706 genworlds-0.0.4/genworlds/agents/__init__.py
--rw-r--r--   0        0        0     6841 2023-06-20 08:42:39.832885 genworlds-0.0.4/genworlds/agents/memory_processors/nmk_world_memory.py
--rw-r--r--   0        0        0        0 2023-06-05 22:23:56.859363 genworlds-0.0.4/genworlds/agents/tree_agent/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 08:42:39.833912 genworlds-0.0.4/genworlds/agents/tree_agent/brains/__init__.py
--rw-r--r--   0        0        0      201 2023-06-20 08:42:39.833912 genworlds-0.0.4/genworlds/agents/tree_agent/brains/brain.py
--rw-r--r--   0        0        0     6234 2023-06-28 09:44:45.886363 genworlds-0.0.4/genworlds/agents/tree_agent/brains/multi_eval_brain.py
--rw-r--r--   0        0        0     5470 2023-06-28 09:44:45.887367 genworlds-0.0.4/genworlds/agents/tree_agent/brains/single_eval_brain.py
--rw-r--r--   0        0        0     2978 2023-06-28 09:44:45.887367 genworlds-0.0.4/genworlds/agents/tree_agent/brains/zero_shot_brain.py
--rw-r--r--   0        0        0        0 2023-06-05 22:23:56.865347 genworlds-0.0.4/genworlds/agents/tree_agent/prompts/__init__.py
--rw-r--r--   0        0        0     6766 2023-06-28 09:44:45.888373 genworlds-0.0.4/genworlds/agents/tree_agent/prompts/execution_generator_prompt.py
--rw-r--r--   0        0        0     6336 2023-06-28 09:44:45.888373 genworlds-0.0.4/genworlds/agents/tree_agent/prompts/navigation_generator_prompt.py
--rw-r--r--   0        0        0    17998 2023-06-28 18:27:24.625552 genworlds-0.0.4/genworlds/agents/tree_agent/tree_agent.py
--rw-r--r--   0        0        0     7151 2023-06-06 11:21:08.414369 genworlds-0.0.4/genworlds/agents/tree_agent/tree_of_thoughts.py
--rw-r--r--   0        0        0     2770 2023-06-20 08:42:39.836907 genworlds-0.0.4/genworlds/agents/world_listeners/listening_antenna.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.373706 genworlds-0.0.4/genworlds/agents/yeager_autogpt/__init__.py
--rw-r--r--   0        0        0    16775 2023-06-20 08:42:39.837905 genworlds-0.0.4/genworlds/agents/yeager_autogpt/agent.py
--rw-r--r--   0        0        0     1103 2023-06-01 00:06:30.374704 genworlds-0.0.4/genworlds/agents/yeager_autogpt/memory.py
--rw-r--r--   0        0        0      983 2023-06-20 08:42:39.837905 genworlds-0.0.4/genworlds/agents/yeager_autogpt/memory_summarizers.py
--rw-r--r--   0        0        0     1898 2023-06-05 22:23:15.260525 genworlds-0.0.4/genworlds/agents/yeager_autogpt/output_parser.py
--rw-r--r--   0        0        0     6374 2023-06-20 08:42:39.838902 genworlds-0.0.4/genworlds/agents/yeager_autogpt/prompt.py
--rw-r--r--   0        0        0     6947 2023-06-05 22:23:15.261522 genworlds-0.0.4/genworlds/agents/yeager_autogpt/prompt_generator.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.377696 genworlds-0.0.4/genworlds/events/__init__.py
--rw-r--r--   0        0        0     2260 2023-06-06 11:21:08.416363 genworlds-0.0.4/genworlds/events/basic_events.py
--rw-r--r--   0        0        0     2966 2023-06-06 11:21:08.417963 genworlds-0.0.4/genworlds/events/websocket_event_handler.py
--rw-r--r--   0        0        0       46 2023-06-06 11:21:08.417963 genworlds-0.0.4/genworlds/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 11:21:08.417963 genworlds-0.0.4/genworlds/interfaces/cli/__init__.py
--rw-r--r--   0        0        0     2812 2023-06-20 08:42:39.838902 genworlds-0.0.4/genworlds/interfaces/cli/cli.py
--rw-r--r--   0        0        0     2486 2023-07-03 15:18:40.004464 genworlds-0.0.4/genworlds/interfaces/cli/event_processors.py
--rw-r--r--   0        0        0     1590 2023-07-03 15:18:40.004464 genworlds-0.0.4/genworlds/interfaces/cli/formatted_buffer.py
--rw-r--r--   0        0        0     4352 2023-06-06 17:42:30.494394 genworlds-0.0.4/genworlds/interfaces/cli/initial_setup_layout_screen.py
--rw-r--r--   0        0        0     2055 2023-06-06 17:42:30.494394 genworlds-0.0.4/genworlds/interfaces/cli/render_help_screen.py
--rw-r--r--   0        0        0     3659 2023-07-03 15:18:40.005436 genworlds-0.0.4/genworlds/interfaces/cli/render_main_screen.py
--rw-r--r--   0        0        0      145 2023-06-06 11:21:08.420958 genworlds-0.0.4/genworlds/interfaces/cli/run.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.379691 genworlds-0.0.4/genworlds/objects/__init__.py
--rw-r--r--   0        0        0     1156 2023-07-03 15:18:40.005436 genworlds-0.0.4/genworlds/objects/base_object.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.380687 genworlds-0.0.4/genworlds/simulation/__init__.py
--rw-r--r--   0        0        0     1649 2023-06-05 22:23:15.263517 genworlds-0.0.4/genworlds/simulation/simulation.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.380687 genworlds-0.0.4/genworlds/sockets/__init__.py
--rw-r--r--   0        0        0     1975 2023-06-01 00:06:30.381917 genworlds-0.0.4/genworlds/sockets/test_client.py
--rw-r--r--   0        0        0     2067 2023-06-12 08:00:25.676275 genworlds-0.0.4/genworlds/sockets/world_socket_client.py
--rw-r--r--   0        0        0     4242 2023-06-06 11:21:08.421955 genworlds-0.0.4/genworlds/sockets/world_socket_server.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.383229 genworlds-0.0.4/genworlds/utils/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-12 08:00:25.677244 genworlds-0.0.4/genworlds/utils/logging_factory.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.384228 genworlds-0.0.4/genworlds/worlds/__init__.py
--rw-r--r--   0        0        0     7749 2023-06-28 18:27:24.626553 genworlds-0.0.4/genworlds/worlds/base_world.py
--rw-r--r--   0        0        0      330 2023-06-05 22:23:15.265511 genworlds-0.0.4/genworlds/worlds/base_world_entity.py
--rw-r--r--   0        0        0        0 2023-06-01 00:06:30.385226 genworlds-0.0.4/genworlds/worlds/world_2d/__init__.py
--rw-r--r--   0        0        0     2827 2023-07-03 15:18:40.006435 genworlds-0.0.4/genworlds/worlds/world_2d/world_2d.py
--rw-r--r--   0        0        0     1086 2023-06-01 00:06:30.371425 genworlds-0.0.4/LICENSE
--rw-r--r--   0        0        0      793 2023-07-03 15:34:04.654649 genworlds-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 genworlds-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.372707 genworlds-0.0.5/genworlds/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.373706 genworlds-0.0.5/genworlds/agents/__init__.py
+-rw-r--r--   0        0        0     6841 2023-06-20 08:42:39.832885 genworlds-0.0.5/genworlds/agents/memory_processors/nmk_world_memory.py
+-rw-r--r--   0        0        0        0 2023-06-05 22:23:56.859363 genworlds-0.0.5/genworlds/agents/tree_agent/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:42:39.833912 genworlds-0.0.5/genworlds/agents/tree_agent/brains/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-20 08:42:39.833912 genworlds-0.0.5/genworlds/agents/tree_agent/brains/brain.py
+-rw-r--r--   0        0        0     6234 2023-06-28 09:44:45.886363 genworlds-0.0.5/genworlds/agents/tree_agent/brains/multi_eval_brain.py
+-rw-r--r--   0        0        0     5470 2023-06-28 09:44:45.887367 genworlds-0.0.5/genworlds/agents/tree_agent/brains/single_eval_brain.py
+-rw-r--r--   0        0        0     2978 2023-06-28 09:44:45.887367 genworlds-0.0.5/genworlds/agents/tree_agent/brains/zero_shot_brain.py
+-rw-r--r--   0        0        0        0 2023-06-05 22:23:56.865347 genworlds-0.0.5/genworlds/agents/tree_agent/prompts/__init__.py
+-rw-r--r--   0        0        0     6646 2023-07-05 15:25:25.606698 genworlds-0.0.5/genworlds/agents/tree_agent/prompts/execution_generator_prompt.py
+-rw-r--r--   0        0        0     6336 2023-06-28 09:44:45.888373 genworlds-0.0.5/genworlds/agents/tree_agent/prompts/navigation_generator_prompt.py
+-rw-r--r--   0        0        0    17998 2023-06-28 18:27:24.625552 genworlds-0.0.5/genworlds/agents/tree_agent/tree_agent.py
+-rw-r--r--   0        0        0     7151 2023-06-06 11:21:08.414369 genworlds-0.0.5/genworlds/agents/tree_agent/tree_of_thoughts.py
+-rw-r--r--   0        0        0     3782 2023-07-05 15:25:25.607700 genworlds-0.0.5/genworlds/agents/world_listeners/listening_antenna.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.373706 genworlds-0.0.5/genworlds/agents/yeager_autogpt/__init__.py
+-rw-r--r--   0        0        0    16775 2023-06-20 08:42:39.837905 genworlds-0.0.5/genworlds/agents/yeager_autogpt/agent.py
+-rw-r--r--   0        0        0     1103 2023-06-01 00:06:30.374704 genworlds-0.0.5/genworlds/agents/yeager_autogpt/memory.py
+-rw-r--r--   0        0        0      983 2023-06-20 08:42:39.837905 genworlds-0.0.5/genworlds/agents/yeager_autogpt/memory_summarizers.py
+-rw-r--r--   0        0        0     1898 2023-06-05 22:23:15.260525 genworlds-0.0.5/genworlds/agents/yeager_autogpt/output_parser.py
+-rw-r--r--   0        0        0     6374 2023-06-20 08:42:39.838902 genworlds-0.0.5/genworlds/agents/yeager_autogpt/prompt.py
+-rw-r--r--   0        0        0     6947 2023-06-05 22:23:15.261522 genworlds-0.0.5/genworlds/agents/yeager_autogpt/prompt_generator.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.377696 genworlds-0.0.5/genworlds/events/__init__.py
+-rw-r--r--   0        0        0     2260 2023-06-06 11:21:08.416363 genworlds-0.0.5/genworlds/events/basic_events.py
+-rw-r--r--   0        0        0     2966 2023-06-06 11:21:08.417963 genworlds-0.0.5/genworlds/events/websocket_event_handler.py
+-rw-r--r--   0        0        0       46 2023-06-06 11:21:08.417963 genworlds-0.0.5/genworlds/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:21:08.417963 genworlds-0.0.5/genworlds/interfaces/cli/__init__.py
+-rw-r--r--   0        0        0     2812 2023-06-20 08:42:39.838902 genworlds-0.0.5/genworlds/interfaces/cli/cli.py
+-rw-r--r--   0        0        0     2486 2023-07-03 15:18:40.004464 genworlds-0.0.5/genworlds/interfaces/cli/event_processors.py
+-rw-r--r--   0        0        0     1590 2023-07-03 15:18:40.004464 genworlds-0.0.5/genworlds/interfaces/cli/formatted_buffer.py
+-rw-r--r--   0        0        0     4352 2023-06-06 17:42:30.494394 genworlds-0.0.5/genworlds/interfaces/cli/initial_setup_layout_screen.py
+-rw-r--r--   0        0        0     2055 2023-06-06 17:42:30.494394 genworlds-0.0.5/genworlds/interfaces/cli/render_help_screen.py
+-rw-r--r--   0        0        0     3659 2023-07-03 15:18:40.005436 genworlds-0.0.5/genworlds/interfaces/cli/render_main_screen.py
+-rw-r--r--   0        0        0      145 2023-06-06 11:21:08.420958 genworlds-0.0.5/genworlds/interfaces/cli/run.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.379691 genworlds-0.0.5/genworlds/objects/__init__.py
+-rw-r--r--   0        0        0     1156 2023-07-03 15:18:40.005436 genworlds-0.0.5/genworlds/objects/base_object.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.380687 genworlds-0.0.5/genworlds/simulation/__init__.py
+-rw-r--r--   0        0        0     1649 2023-06-05 22:23:15.263517 genworlds-0.0.5/genworlds/simulation/simulation.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.380687 genworlds-0.0.5/genworlds/sockets/__init__.py
+-rw-r--r--   0        0        0     1975 2023-06-01 00:06:30.381917 genworlds-0.0.5/genworlds/sockets/test_client.py
+-rw-r--r--   0        0        0     2067 2023-06-12 08:00:25.676275 genworlds-0.0.5/genworlds/sockets/world_socket_client.py
+-rw-r--r--   0        0        0     4242 2023-06-06 11:21:08.421955 genworlds-0.0.5/genworlds/sockets/world_socket_server.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.383229 genworlds-0.0.5/genworlds/utils/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-12 08:00:25.677244 genworlds-0.0.5/genworlds/utils/logging_factory.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.384228 genworlds-0.0.5/genworlds/worlds/__init__.py
+-rw-r--r--   0        0        0     7749 2023-06-28 18:27:24.626553 genworlds-0.0.5/genworlds/worlds/base_world.py
+-rw-r--r--   0        0        0      330 2023-06-05 22:23:15.265511 genworlds-0.0.5/genworlds/worlds/base_world_entity.py
+-rw-r--r--   0        0        0        0 2023-06-01 00:06:30.385226 genworlds-0.0.5/genworlds/worlds/world_2d/__init__.py
+-rw-r--r--   0        0        0     2827 2023-07-03 15:18:40.006435 genworlds-0.0.5/genworlds/worlds/world_2d/world_2d.py
+-rw-r--r--   0        0        0     1086 2023-06-01 00:06:30.371425 genworlds-0.0.5/LICENSE
+-rw-r--r--   0        0        0      793 2023-07-05 15:25:25.607700 genworlds-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 genworlds-0.0.5/PKG-INFO
```

### Comparing `genworlds-0.0.4/genworlds/agents/memory_processors/nmk_world_memory.py` & `genworlds-0.0.5/genworlds/agents/memory_processors/nmk_world_memory.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/brains/multi_eval_brain.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/brains/multi_eval_brain.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/brains/single_eval_brain.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/brains/single_eval_brain.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/brains/zero_shot_brain.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/brains/zero_shot_brain.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/prompts/execution_generator_prompt.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/prompts/execution_generator_prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,22 +119,16 @@
             plan = "\n".join([f"{i+1}. {goal}" for i, goal in enumerate(kwargs["plan"])]) 
             plan_message = SystemMessage(content=f"## Your Plan:\n{plan}")
             messages.append(plan_message)
             used_tokens += len(plan_message.content)   
 
         if "personality_db" in kwargs and kwargs["personality_db"] is not None:
             personality_db: VectorStore = kwargs["personality_db"]
-            past_statements = list(
-                map(
-                    lambda d: d.page_content,
-                    personality_db.similarity_search(
-                        kwargs["previous_brain_outputs"][-1]
-                    ),
-                )
-            )
+            past_statements = [document.page_content for document in personality_db.similarity_search(str(kwargs["previous_brain_outputs"][-1]))]
+            
             if len(past_statements) > 0:
                 past_statements_bullet_list = "\n".join(map(lambda s: f'- {s}', past_statements))
                 past_statements_format = f"You have said the following things on this topic in the past:\n{past_statements_bullet_list}\n\n"
                 personality_message = SystemMessage(content=past_statements_format)
                 messages.append(personality_message)
                 used_tokens += len(personality_message.content)
```

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/prompts/navigation_generator_prompt.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/prompts/navigation_generator_prompt.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/tree_agent.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/tree_agent.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/tree_agent/tree_of_thoughts.py` & `genworlds-0.0.5/genworlds/agents/tree_agent/tree_of_thoughts.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/world_listeners/listening_antenna.py` & `genworlds-0.0.5/genworlds/agents/world_listeners/listening_antenna.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,35 @@
         self.important_event_types = self.special_events.copy()
         self.important_event_types.update(important_event_types)
 
         self.agent_name = agent_name
         self.agent_id = agent_id
 
     def process_event(self, event):
+        match event:
+            case {"event_type": "world_sends_schemas_event"}:
+                self.schemas = event["schemas"]
+            case {"event_type": "entity_world_state_update_event", "target_id": self.agent_id}:
+                self.agent_world_state = event["entity_world_state"]
+            case {"event_type": "world_sends_nearby_entities_event", "target_id": self.agent_id}:
+                self.nearby_entities = event["nearby_entities"]
+            case {"event_type": event_type} if event_type in self.special_events:
+                pass
+            case event:
+                if (
+                    event["sender_id"] != self.agent_id 
+                    and
+                    (event["target_id"] == self.agent_id or 
+                    event["target_id"] == None or
+                    event["event_type"] in self.important_event_types)
+                ):
+                    self.last_events.append(event)
+                    self.all_events.append(event)
+
+
         if event["event_type"] == "world_sends_schemas_event":
             self.schemas = event["schemas"]
         elif event["event_type"] == "entity_world_state_update_event":
             if event["target_id"] == self.agent_id:
                 self.agent_world_state = event["entity_world_state"]
         elif event["event_type"] == "world_sends_nearby_entities_event":
             if event["target_id"] == self.agent_id:
```

### Comparing `genworlds-0.0.4/genworlds/agents/yeager_autogpt/agent.py` & `genworlds-0.0.5/genworlds/agents/yeager_autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/yeager_autogpt/memory.py` & `genworlds-0.0.5/genworlds/agents/yeager_autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/yeager_autogpt/memory_summarizers.py` & `genworlds-0.0.5/genworlds/agents/yeager_autogpt/memory_summarizers.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/yeager_autogpt/output_parser.py` & `genworlds-0.0.5/genworlds/agents/yeager_autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/yeager_autogpt/prompt.py` & `genworlds-0.0.5/genworlds/agents/yeager_autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/agents/yeager_autogpt/prompt_generator.py` & `genworlds-0.0.5/genworlds/agents/yeager_autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/events/basic_events.py` & `genworlds-0.0.5/genworlds/events/basic_events.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/events/websocket_event_handler.py` & `genworlds-0.0.5/genworlds/events/websocket_event_handler.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/interfaces/cli/cli.py` & `genworlds-0.0.5/genworlds/interfaces/cli/cli.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/interfaces/cli/event_processors.py` & `genworlds-0.0.5/genworlds/interfaces/cli/event_processors.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/interfaces/cli/formatted_buffer.py` & `genworlds-0.0.5/genworlds/interfaces/cli/formatted_buffer.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/interfaces/cli/initial_setup_layout_screen.py` & `genworlds-0.0.5/genworlds/interfaces/cli/initial_setup_layout_screen.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/interfaces/cli/render_help_screen.py` & `genworlds-0.0.5/genworlds/interfaces/cli/render_help_screen.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/interfaces/cli/render_main_screen.py` & `genworlds-0.0.5/genworlds/interfaces/cli/render_main_screen.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/objects/base_object.py` & `genworlds-0.0.5/genworlds/objects/base_object.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/simulation/simulation.py` & `genworlds-0.0.5/genworlds/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/sockets/test_client.py` & `genworlds-0.0.5/genworlds/sockets/test_client.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/sockets/world_socket_client.py` & `genworlds-0.0.5/genworlds/sockets/world_socket_client.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/sockets/world_socket_server.py` & `genworlds-0.0.5/genworlds/sockets/world_socket_server.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/utils/logging_factory.py` & `genworlds-0.0.5/genworlds/utils/logging_factory.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/worlds/base_world.py` & `genworlds-0.0.5/genworlds/worlds/base_world.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/genworlds/worlds/world_2d/world_2d.py` & `genworlds-0.0.5/genworlds/worlds/world_2d/world_2d.py`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/LICENSE` & `genworlds-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `genworlds-0.0.4/pyproject.toml` & `genworlds-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "genworlds"
-version = "0.0.4"
+version = "0.0.5"
 description = "GenWorlds by YeagerAI: Pioneering AI-based simulations based on collaborative autonomous agents."
 authors = []
 
 [tool.poetry.dependencies]
 python = ">=3.11.3,<3.12"
 click="8.1.3"
 colorama="0.4.6"
```

### Comparing `genworlds-0.0.4/PKG-INFO` & `genworlds-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genworlds
-Version: 0.0.4
+Version: 0.0.5
 Summary: GenWorlds by YeagerAI: Pioneering AI-based simulations based on collaborative autonomous agents.
 Requires-Python: >=3.11.3,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: click (==8.1.3)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: colorlog (==6.7.0)
 Requires-Dist: fastapi (==0.88.0)
```

