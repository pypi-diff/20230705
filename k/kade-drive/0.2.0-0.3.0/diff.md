# Comparing `tmp/kade_drive-0.2.0.tar.gz` & `tmp/kade_drive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kade_drive-0.2.0.tar", max compression
+gzip compressed data, was "kade_drive-0.3.0.tar", max compression
```

## Comparing `kade_drive-0.2.0.tar` & `kade_drive-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.2.0/LICENSE
--rw-r--r--   0        0        0      220 2023-07-04 03:13:39.414643 kade_drive-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-04 16:17:23.029053 kade_drive-0.2.0/kade_drive/__init__.py
--rw-r--r--   0        0        0     1574 2023-07-04 16:17:23.029053 kade_drive-0.2.0/kade_drive/cli.py
--rw-r--r--   0        0        0     6752 2023-07-04 16:41:46.747892 kade_drive-0.2.0/kade_drive/client.py
--rw-r--r--   0        0        0        1 2023-07-04 16:17:23.029053 kade_drive-0.2.0/kade_drive/core/__init__.py
--rw-r--r--   0        0        0     9109 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/crawling.py
--rw-r--r--   0        0        0    18449 2023-07-04 16:51:20.329071 kade_drive-0.2.0/kade_drive/core/network.py
--rw-r--r--   0        0        0     3994 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/node.py
--rw-r--r--   0        0        0     7886 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/protocol.py
--rw-r--r--   0        0        0     8614 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/routing.py
--rw-r--r--   0        0        0     9169 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/storage.py
--rw-r--r--   0        0        0     1340 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/core/utils.py
--rw-r--r--   0        0        0      209 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/main_recv.py
--rw-r--r--   0        0        0      248 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/main_send.py
--rw-r--r--   0        0        0        0 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/message_system/__init__.py
--rw-r--r--   0        0        0     6954 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/message_system/message_system.py
--rw-r--r--   0        0        0     2244 2023-07-04 16:17:23.030053 kade_drive-0.2.0/kade_drive/server.py
--rw-r--r--   0        0        0       25 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/__init__.py
--rw-r--r--   0        0        0     1598 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/conftest.py
--rw-r--r--   0        0        0     3100 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/data_to_split.txt
--rw-r--r--   0        0        0     1785 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_node.py
--rw-r--r--   0        0        0     4520 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_routing.py
--rw-r--r--   0        0        0        1 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_server.py
--rw-r--r--   0        0        0      841 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_splitdata.py
--rw-r--r--   0        0        0     1458 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_storage.py
--rw-r--r--   0        0        0      678 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_store_file.py
--rw-r--r--   0        0        0      717 2023-07-04 16:17:23.031053 kade_drive-0.2.0/kade_drive/tests/test_utils.py
--rw-r--r--   0        0        0      508 2023-07-04 19:15:12.893711 kade_drive-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 kade_drive-0.2.0/setup.py
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 kade_drive-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.3.0/LICENSE
+-rw-r--r--   0        0        0      391 2023-07-05 05:42:42.391327 kade_drive-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 16:17:23.029053 kade_drive-0.3.0/kade_drive/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-05 18:42:18.719455 kade_drive-0.3.0/kade_drive/cli.py
+-rw-r--r--   0        0        0     6860 2023-07-05 19:47:23.095393 kade_drive-0.3.0/kade_drive/client.py
+-rw-r--r--   0        0        0        1 2023-07-04 16:17:23.029053 kade_drive-0.3.0/kade_drive/core/__init__.py
+-rw-r--r--   0        0        0     9628 2023-07-05 19:50:49.320361 kade_drive-0.3.0/kade_drive/core/crawling.py
+-rw-r--r--   0        0        0    19005 2023-07-05 20:17:40.992780 kade_drive-0.3.0/kade_drive/core/network.py
+-rw-r--r--   0        0        0     3994 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/core/node.py
+-rw-r--r--   0        0        0     8137 2023-07-05 20:14:26.342405 kade_drive-0.3.0/kade_drive/core/protocol.py
+-rw-r--r--   0        0        0     8834 2023-07-05 18:42:18.720455 kade_drive-0.3.0/kade_drive/core/routing.py
+-rw-r--r--   0        0        0     9643 2023-07-05 20:13:35.887049 kade_drive-0.3.0/kade_drive/core/storage.py
+-rw-r--r--   0        0        0     1340 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/core/utils.py
+-rw-r--r--   0        0        0      209 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/main_recv.py
+-rw-r--r--   0        0        0      248 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/main_send.py
+-rw-r--r--   0        0        0        0 2023-07-04 16:17:23.030053 kade_drive-0.3.0/kade_drive/message_system/__init__.py
+-rw-r--r--   0        0        0     7085 2023-07-05 20:59:37.300407 kade_drive-0.3.0/kade_drive/message_system/message_system.py
+-rw-r--r--   0        0        0     2366 2023-07-05 18:42:18.720455 kade_drive-0.3.0/kade_drive/server.py
+-rw-r--r--   0        0        0      733 2023-07-05 18:29:56.160697 kade_drive-0.3.0/kade_drive/test_store_file.py
+-rw-r--r--   0        0        0       25 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-05 18:29:45.621586 kade_drive-0.3.0/kade_drive/tests/conftest.py
+-rw-r--r--   0        0        0     3100 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/data_to_split.txt
+-rw-r--r--   0        0        0     1785 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_node.py
+-rw-r--r--   0        0        0     4520 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_routing.py
+-rw-r--r--   0        0        0        1 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_server.py
+-rw-r--r--   0        0        0      841 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_splitdata.py
+-rw-r--r--   0        0        0     1458 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_storage.py
+-rw-r--r--   0        0        0      717 2023-07-04 16:17:23.031053 kade_drive-0.3.0/kade_drive/tests/test_utils.py
+-rw-r--r--   0        0        0      508 2023-07-05 21:04:14.088945 kade_drive-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 kade_drive-0.3.0/setup.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 kade_drive-0.3.0/PKG-INFO
```

### Comparing `kade_drive-0.2.0/LICENSE` & `kade_drive-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/cli.py` & `kade_drive-0.3.0/kade_drive/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 
 import sys
 import logging
 from client import ClientSession
 
 client_session: ClientSession | None = None
 
-
 if __name__ == "__main__":
     ip = None
     port = 8086
 
     if len(sys.argv) == 2:
         ip = sys.argv[1]
 
     if len(sys.argv) == 3:
         ip, port = sys.argv[1], sys.argv[2]
 
     initial_bootstrap_nodes = [(ip, int(port))] if ip else []
     client_session = ClientSession(initial_bootstrap_nodes)
-    logger = logging.getLogger(__name__)
 
     print('Wellcome to CLI interface for distributed Filesystem')
     while True:
 
         response = client_session.connect(
             use_broadcast_if_needed=True)
         if not response:
@@ -42,14 +40,14 @@
             continue
         args = command[1:] if len(command) >= 1 else []
         func = getattr(ClientSession, command[0], None)
         if func is None or not callable(func):
             print(
                 f'command {command[0]} not found, use "help" to see supported commands')
             continue
-        logger.debug(f'calling {func} with arguments: {args}')
+        # logger.debug(f'calling {func} with arguments: {args}')
 
         result = func(client_session, *args)
-        if result:
+        if result is not None:
             print(f'result > {result}')
         # else:
         #     print(f'result > None')
```

### Comparing `kade_drive-0.2.0/kade_drive/client.py` & `kade_drive-0.3.0/kade_drive/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import rpyc
 from time import sleep
 from rpyc.core.protocol import PingError
 from message_system.message_system import Message_System
 
 import logging
 
+logging.basicConfig(level=logging.DEBUG,
+                    format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
+logger.info("TESTTTTTT")
 # rpyc.core.protocol.DEFAULT_CONFIG['allow_pickle'] = True
 
 
 class ClientSession:
     """
     Class to handle connection to the distributed file system
     It is necessary to run ensure_connection or broadcast method before
@@ -69,22 +73,22 @@
                 f"Connection to {ip} failed, removing from bootstrap nodes list.")
             nodes_to_try.pop(0)
             return nodes_to_try, total_attempts_to_reconnect
 
         return nodes_to_try, remaining_attempts_to_reconnect
 
     def get(self, key, apply_hash_to_key=True):
-        logger = logging.getLogger(__name__)
         if not self.connection:
             logger.error(f'No connection stablished to do get')
             return None
         metadata_list = self.connection.root.get(key, apply_hash_to_key)
-        logger = logging.getLogger(__name__)
-
-        logger.debug(f'metadata_list received {str(len(metadata_list) > 0)}')
+        logger.debug(f"METADATAAAAA {metadata_list}")
+        if metadata_list:
+            logger.debug(
+                f'metadata_list received {str(len(metadata_list) > 0)}')
         data_received = []
 
         if metadata_list is None or len(metadata_list) == 0:
             logger.debug(f'No data with key {key}')
             return None
 
         for chunk_key in metadata_list:
@@ -103,51 +107,47 @@
                 if conn:
                     data_received.append(
                         conn.root.rpc_get_file_chunk_value(chunk_key))
                 else:
                     logger.warning('No Servers to get chunk')
 
         # data_recv = bytearray()
-        logger.debug('len data received', len(data_received))
+        logger.debug(f'len data received {len(data_received)}')
         data_received = b''.join(data_received)
         try:
             data_to_return = pickle.loads(data_received)
             return data_to_return
         except pickle.UnpicklingError as e:
             logger.error(e)
             return None
-        
+
     def put(self, key, value: bytes, apply_hash_to_key=True):
-        logger = logging.getLogger(__name__)
-        logger.debug(f'key: {key}, value: {value}')
         # print(self.connection.root.upload_file.)
         if self.connection:
-            self.connection.root.upload_file(key=key, data=value, apply_hash_to_key=apply_hash_to_key)
+            self.connection.root.upload_file(
+                key=key, data=value, apply_hash_to_key=apply_hash_to_key)
             sleep(1)
             logger.info(f'put > Success')
-        else: 
+        else:
             logger.error(f'No connection stablished to do put')
 
     def _update_bootstrap_nodes(self, connection: rpyc.Connection):
-        logger = logging.getLogger(__name__)
-
         nodes_to_add = [node for node in connection.root.find_neighbors(
         ) if node not in self.bootstrap_nodes]
         self.bootstrap_nodes.extend(nodes_to_add)
         logger.debug(f'Neighbors {self.bootstrap_nodes}')
 
     def broadcast(self) -> bool:
         print('Listening broadcasts')
         ms = Message_System()
         try:
-            ip, port = ms.receive().split(" ")
+            ip, port = ms.receive(service_name='dfs').split(" ")
+            print(ip, port)
         except ValueError:
             ip = None
             port = None
         if ip:
             self.bootstrap_nodes.append((ip, int(port)))
             return True
 
         print('No broadcasts received.')
         return False
-
-
```

### Comparing `kade_drive-0.2.0/kade_drive/core/crawling.py` & `kade_drive-0.3.0/kade_drive/core/crawling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from collections import Counter
 import logging
 import rpyc
 from core.node import Node, NodeHeap
 from core.protocol import FileSystemProtocol, ServerSession
 import logging
 
+
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 
 
 class SpiderCrawl:
     """
     Crawl the network and look for given 160-bit keys.
     """
 
@@ -65,18 +71,24 @@
         # perform the rpc protocol method call
         # return the info from those nodes
         found_values = []
         for peer in self.nearest.get_uncontacted()[:count]:
             logger.debug("Peer %s %s", type(peer), peer)
             if peer.ip == '192.168.133.1':
                 continue
-            session = rpyc.connect(host=peer.ip, port=peer.port)
-            conn = session.root
+            try: 
+                session = rpyc.connect(host=peer.ip, port=peer.port)
+                conn = session.root
+            except ConnectionError as e:
+                logger.warning(f'Failed to connect to {peer.id} {peer.ip}, e: {e}')
+                session = None
+                conn = None
+            
             logger.debug(f'Connection is {conn is not None} and self.node is {self.node is not None}')
-            logger.debug("Calling ", rpcmethod)
+            logger.debug(f"Calling : {rpcmethod}")
             if is_metadata is None:
                 response = rpcmethod(conn, peer, self.node)
             else:
                 response = rpcmethod(conn, peer, self.node, is_metadata)
             response_dict[peer.id] = response
             self.nearest.mark_contacted(peer)
             logger.debug("mark contacted successful")
@@ -105,32 +117,30 @@
         """
         return self._find(FileSystemProtocol.call_find_value, is_metadata)
 
     def _nodes_found(self, response_dict: dict):
         """
         Handle the result of an iteration in _find.
         """
-
-
         logger.debug("entry node Found Value Spider")
         toremove = []
         found_values = []
         for peer_id, response in response_dict.items():
             response = RPCFindResponse(response)
             if not response.happened():
                 toremove.append(peer_id)
             elif response.has_value():
                 found_values.append(response.get_value())
             else:
                 peer = self.nearest.get_node(peer_id)
                 self.nearest_without_value.push(peer)
                 self.nearest.push(response.get_node_list())
         self.nearest.remove(toremove)
-
-        if found_values:
+        logger.debug(f"found values in _nodes_found {found_values}")
+        if len(found_values)>0:
             return self._handle_found_values(found_values)
         if self.nearest.have_contacted_all():
             # not found!
             return None
         return self.find()
 
     def _handle_contacts(self):
```

### Comparing `kade_drive-0.2.0/kade_drive/core/network.py` & `kade_drive-0.3.0/kade_drive/core/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Package for interacting on the network at a high level.
 """
+import base64
 import random
 import logging
 from rpyc import Service
 import threading
 from time import sleep
 import rpyc
 import socket
@@ -16,16 +17,21 @@
 from core.routing import RoutingTable
 from core.utils import digest
 from core.storage import PersistentStorage
 from core.node import Node
 from core.crawling import ChunkLocationSpiderCrawl, ValueSpiderCrawl
 from core.crawling import NodeSpiderCrawl
 # from models.file import File
-logger = logging.getLogger(__name__)
 
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 class Server:
     ksize: int
     alpha: int
     storage: PersistentStorage
     node: Node
     routing: RoutingTable
 
@@ -41,18 +47,18 @@
         """
         
         Server.ksize = ksize
         Server.alpha = alpha
         Server.storage = storage or PersistentStorage()
         Server.node = Node(node_id or digest(
             random.getrandbits(255)), ip=ip, port=str(port))
-        logger.debug("NODE ID", Server.node.id)
+        logger.debug(f"NODE ID: {Server.node.id}")
         Server.routing = RoutingTable(Server.ksize, Server.node)
         FileSystemProtocol.init(Server.routing, Server.storage)
-        logger.debug(port, ip)
+        logger.debug(f'{port}, {ip}')
         threading.Thread(target=Server.listen, args=(port, ip)).start()
         refresh_thread = threading.Thread(target=Server._refresh_table)
         refresh_thread.start()
 
     @staticmethod
     def listen(port, interface='0.0.0.0'):
         """
@@ -87,15 +93,14 @@
         nodes = [node for node in cos if node is not None]
         # print(nodes)
         spider = NodeSpiderCrawl(Server.node, nodes,
                                  Server.ksize, Server.alpha)
         # print(spider)
         res = spider.find()
         logger.debug('results of spider find: %s', res)
-        logger.debug(res)
 
         return res
 
     @staticmethod
     def bootstrap_node(addr: tuple[str, str]):
         response = None
         with ServerSession(addr[0], addr[1]) as conn:
@@ -159,25 +164,25 @@
                                  Server.ksize, Server.alpha)
         nodes = spider.find()
         logger.debug("setting '%s' on %s", dkey, list(map(str, nodes)))
 
         # if this node is close too, then store here as well
         biggest = max([n.distance_to(node) for n in nodes])
         if Server.node.distance_to(node) < biggest:
-            if Server.storage.contains(dkey):
+            if Server.storage.contains(dkey, metadata):
                 if metadata:
                     Server.storage.set_metadata(dkey, value, False)
                 else:
                     Server.storage.set_value(dkey, value, False)
 
         any_result = False
         for n in nodes:
             address = (n.ip, n.port)
             with ServerSession(address[0], address[1]) as conn:
-                contains = FileSystemProtocol.call_contains(conn, n, dkey)
+                contains = FileSystemProtocol.call_contains(conn, n, dkey, metadata)
                 if not contains:
                     result = FileSystemProtocol.call_store(
                         conn, n, dkey, value, metadata)
                     if result:
                         any_result = True
 
                 if contains:
@@ -197,15 +202,15 @@
 
         keys_to_find = Server.storage.keys()
         keys_dict = {}
         for n in nodes:
             with ServerSession(n.ip, n.port) as conn:
                 # if len(keys_to_find) > 0:
                 for k, is_metadata in keys_to_find:
-                    contains = FileSystemProtocol.call_contains(conn, n, k)
+                    contains = FileSystemProtocol.call_contains(conn, n, k, is_metadata)
                     if contains:
                         if not (k, is_metadata) in keys_dict:
                             keys_dict[(k, is_metadata)] = 0
                         keys_dict[(k, is_metadata)] += 1
 
         return_list = []
         for k in keys_dict:
@@ -293,32 +298,35 @@
     def rpc_find_value(self, sender: tuple[str, str], nodeid: bytes, key: bytes, metadata=True):
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             FileSystemProtocol.welcome_if_new(conn, source)
         # get value from storage
-        if not FileSystemProtocol.storage.contains(key):
+        if not FileSystemProtocol.storage.contains(key, metadata):
+            logger.debug(f'Value with key {key} not found, calling rpc_find_node')
+            logger.debug(f'type of key is {type(key)}')
             return self.rpc_find_node(sender, nodeid, key)
 
         value = FileSystemProtocol.storage.get(key, None, metadata)
+        logger.debug(f'returning value {value}')
         return {'value': value}
 
     @rpyc.exposed
     def rpc_find_chunk_location(self, sender: tuple[str, str], nodeid: bytes, key: bytes):
         
         logger.debug('entry in rpc_find_chunk_location')
 
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             FileSystemProtocol.welcome_if_new(conn, source)
         # get value from storage
-        if Server.storage.contains(key):
+        if Server.storage.contains(key, False):
             return {'value': (Server.node.ip, Server.node.port)}
         return self.rpc_find_node(sender, nodeid, key)
 
     @rpyc.exposed
     def rpc_ping(self, sender, nodeid: bytes):
         """Probe a Node to see if pc is online
 
@@ -359,22 +367,22 @@
             node, exclude=source)
         # if len(neighbors) == 0:
         #     neighbors = [Server.node]
         logger.debug(f'neighbors of find_node: { neighbors}')
         return list(map(tuple, neighbors))
 
     @rpyc.exposed
-    def rpc_contains(self, sender, nodeid: bytes, key: bytes):
+    def rpc_contains(self, sender, nodeid: bytes, key: bytes, is_metadata=True):
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             FileSystemProtocol.welcome_if_new(conn, source)
         # get value from storage
-        return FileSystemProtocol.storage.contains(key)
+        return FileSystemProtocol.storage.contains(key, is_metadata)
 
     @rpyc.exposed
     def rpc_get_file_chunk_value(self, key):
         return Server.storage.get(key, metadata=False)
 
     @rpyc.exposed
     def bootstrappable_neighbors(self):
@@ -403,35 +411,37 @@
         if apply_hash_to_key:
             key = digest(key)
         
         node = Node(key)
         nearest = FileSystemProtocol.router.find_neighbors(node)
         if not nearest:
             logger.debug(f"There are no known neighbors to get key {key}")
-            if Server.storage.contains(key) is not None:
+            if Server.storage.contains(key):
                 logger.debug(f'Getting key from this same node')
                 return pickle.loads(Server.storage.get(key, True))
             return None
         spider = ValueSpiderCrawl(node, nearest,
                                   Server.ksize, Server.alpha)
         data = spider.find()
         if data is None:
+            logger.debug("NONE DATA")
             return None
+        logger.debug(f"DATA {data}")
         metadata_list = pickle.loads(data)
         return metadata_list
 
     @rpyc.exposed
     def get_file_chunk_location(self, chunk_key):
         logger.debug('looking file chunk location')
         node = Node(chunk_key)
         nearest = FileSystemProtocol.router.find_neighbors(node)
         if not nearest:
             logger.debug(
                 f"There are no known neighbors to get file chunk location {chunk_key}")
-            if Server.storage.contains(chunk_key) is not None:
+            if Server.storage.contains(chunk_key, False) is not None:
                 logger.debug(f'Found in this server, {Server.node.ip}, port, {Server.node.port}')
                 return [(Server.node.ip, Server.node.port)]
             return None
 
         logger.debug('Initiating ChunkLocationSpiderCrawl')
         spider = ChunkLocationSpiderCrawl(
             node, nearest, Server.ksize, Server.alpha)
```

### Comparing `kade_drive-0.2.0/kade_drive/core/node.py` & `kade_drive-0.3.0/kade_drive/core/node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/core/protocol.py` & `kade_drive-0.3.0/kade_drive/core/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 import rpyc
 import logging
 
 from core.node import Node
 # from kademlia.routing import RoutingTable
 from core.storage import PersistentStorage
 from core.utils import digest
-logger = logging.getLogger(__name__)
 
 
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 class FileSystemProtocol:
     source_node: Node
     ksize: int
     storage: PersistentStorage
     router: None = None
     last_response = None
 
@@ -46,20 +51,20 @@
         if conn:
             response = conn.rpc_store(
                 address, FileSystemProtocol.source_node.id, key, value, is_metadata)
 
         return FileSystemProtocol.process_response(conn, response, node_to_ask)
 
     @staticmethod
-    def call_contains(conn, node_to_ask, key: bytes):
+    def call_contains(conn, node_to_ask, key: bytes, is_metadata=True):
         response = None
         if conn:
             address = (node_to_ask.ip, node_to_ask.port)
             response = conn.rpc_contains(
-                address, FileSystemProtocol.source_node.id, key)
+                address, FileSystemProtocol.source_node.id, key, is_metadata)
 
         return FileSystemProtocol.process_response(conn, response, node_to_ask)
 
     @staticmethod
     def call_find_node(conn, node_to_ask: Node, node_to_find: Node):
         """
         async function to call the find node rpc method
@@ -111,15 +116,15 @@
                 address, FileSystemProtocol.source_node.id, node_to_find.id)
         logger.debug(str(response))
         return FileSystemProtocol.process_response(conn, response, node_to_ask)
 
     @staticmethod
     def call_ping(conn, node_to_ask: Node):
         """
-        async function to call the ping rpc method
+        async function to call the ping rpc method 
         """
         response = None
         address = (node_to_ask.ip, node_to_ask.port)
         response = None
         
 
         if conn:
```

### Comparing `kade_drive-0.2.0/kade_drive/core/routing.py` & `kade_drive-0.3.0/kade_drive/core/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 
 from core.protocol import FileSystemProtocol, ServerSession
 from itertools import chain
 from collections import OrderedDict
 from core.utils import shared_prefix, bytes_to_bit_string
 from core.node import Node
 import logging
-logger = logging.getLogger(__name__)
 
+
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 class KBucket:
     '''
     K is the number of entries in a bucket, their node IDs are expected to be randomly distributed within the ID-range the bucket covers
     Each node is putted in a bucket based on how far away they are from the source node.
     This way when you are looking for some node you don't have to bother all possible nodes
     '''
```

### Comparing `kade_drive-0.2.0/kade_drive/core/storage.py` & `kade_drive-0.3.0/kade_drive/core/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 from time import sleep
 from collections import OrderedDict
 from abc import abstractmethod, ABC
 from pathlib import Path
 import threading
 import base64
 import logging
-logger = logging.getLogger(__name__)
 
+
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 class PersistentStorage:
     """
     This class allows to persist files on disk using mongodb.
     The class acts as an OrderedDict that his keys are the hash of an
     specific file chunk and the value is the (ip, port) of the node that
     has the chunk in his mongodb instance. In the current implementation
     the values of the dict are not used. The get method directly access to
@@ -59,15 +65,15 @@
 
     def update_timestamp(self, filename: str, republish_data=False):
         self.ensure_dir_paths()
         # print('timestamp for',filename)
         data = {"date": datetime.now(), "republish": republish_data}
         
 
-        logger.debug('mira ruta %s %s', os.path.join(self.timestamp_path, str(filename)))
+        logger.debug(f'mira ruta {os.path.join(self.timestamp_path, str(filename))}')
         with open(os.path.join(self.timestamp_path, str(filename)), "wb") as f:
             pickle.dump(data, f)
 
     def update_republish(self, key: bytes):
         str_key = str(base64.urlsafe_b64encode(key))
         with open(os.path.join(self.timestamp_path, str_key), "rb") as f:
             data = pickle.load(f)
@@ -174,23 +180,29 @@
         if not path.exists():
             return None
 
         with open(os.path.join(self.keys_path, key), "rb") as f:
             result = f.read()
             return result, os.path.exists(os.path.join(self.metadata_path, key))
 
-    def contains(self, key: bytes):
+    def contains(self, key: bytes, is_metadata=True):
         str_key = str(base64.urlsafe_b64encode(key)) 
+        logger.debug(f'str_key in contains is {str_key}')
         self.cull()
         # self.update_timestamp(key)
-        path = Path(os.path.join(self.values_path, str_key))
-        if not path.exists():
-            return False
+        if is_metadata:
+            path = Path(os.path.join(self.metadata_path, str_key))
+            if not path.exists():
+                return False
+        else:
+            path = Path(os.path.join(self.values_path, str_key))
+            if not path.exists():
+                return False
 
-        self.update_timestamp(str_key)
+        # self.update_timestamp(str_key)
         return True
 
     def __getitem__(self, key: bytes):
         self.cull()
         str_key = str(base64.urlsafe_b64encode(key)) 
         result = self.get_value(str_key)
         if result is None:
```

### Comparing `kade_drive-0.2.0/kade_drive/core/utils.py` & `kade_drive-0.3.0/kade_drive/core/utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/message_system/message_system.py` & `kade_drive-0.3.0/kade_drive/message_system/message_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 import time
 import select
 import threading
 from socket import SHUT_RDWR
 import sys
 from core.utils import get_ips
 import logging
+
+
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
 logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 
 class Message_System:
 
     def __init__(self, host_ip=None, broadcast_addr=None):
         self.host_ip = host_ip
         self.broadcast_addr = broadcast_addr
 
@@ -57,27 +64,26 @@
             return False  # Socket is closed
 
     def stop_listening(self, sock, duration=3):
         threading.Timer(duration, self.close_sock, [sock]).start()
 
     def close_sock(self, sock: socket.socket):
         if Message_System.is_socket_open(sock):
-            
+
             logger.debug(f"closing socket, {str(sock)}")
             try:
                 if sys.platform.startswith('linux'):
                     sock.shutdown(SHUT_RDWR)
                 sock.close()
             except OSError:
                 pass
 
     def _mc_recv(self, fromnicip, mcgrpip, mcport):
         # print("inside rec")
         bufsize = 1024
-        
 
         # This creates a UDP socket
         receiver = socket.socket(family=socket.AF_INET, type=socket.SOCK_DGRAM,
                                  proto=socket.IPPROTO_UDP, fileno=None)
         receiver.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
 
         # This configure the socket to receive datagrams sent to this multicast
@@ -147,47 +153,41 @@
             if i['ip'] == None:
                 # print("sending")
                 for nic_ip in get_ips():
                     self._mc_send(nic_ip, self.broadcast_addr, 50001,
                                   i['message'].encode())
 
     def send_heartbeat(self):
-        
 
         while True:
             try:
                 self.send()
                 time.sleep(0.3)
             except Exception as e:
                 logger.error(f"Exception in heartbeat {str(e)}")
                 # print("Thrown Exception", e)
                 pass
 
-    def receive(self):
-        
+    def receive(self, service_name: str):
 
         to_remove = []
-        if self.host_ip == None:
-            self_host = socket.gethostname()
-            self.host_ip = socket.gethostbyname(self_host)
         # self.host_ip = "192.168.26.1"
+        print("receiving", self.pendig_receive)
         for idx, i in enumerate(self.pendig_receive):
+            # print(i)
             if i['times'] > 0:
-                i -= 1
-            logger.debug(f"listening in {self.host_ip}")
+                i['times'] -= 1
+            logger.info(f"listening in {self.host_ip}")
             for nic_ip in get_ips():
-                logger.debug(f"NIC {nic_ip}")
+                # print(f"NIC {nic_ip}")
                 if 'broadcast' in nic_ip:
                     msg, ip = self._mc_recv(nic_ip, nic_ip['broadcast'], 50001)
-                    if msg:
+                    
+                    if msg is not None and msg.startswith(service_name):
                         logger.info(f">>> Message from {ip}: {msg}\n")
+                        msg = msg.removeprefix(service_name+' ')
                         break
 
-                        # process message
-
-                        if i['times'] == 0:
-                            to_remove.append(idx)
-
         for i in to_remove:
             self.pendig_receive.pop(i)
 
         return msg
```

### Comparing `kade_drive-0.2.0/kade_drive/server.py` & `kade_drive-0.3.0/kade_drive/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,73 +6,79 @@
 import threading
 import time
 import sys
 from message_system.message_system import Message_System
 from core.utils import get_ips
 import logging
 
-logging.basicConfig(level=logging.INFO,
+# Create a file handler
+file_handler = logging.FileHandler('log_file.log')
+
+# Set the logging format
+formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+file_handler.setFormatter(formatter)
+
+# Add the file handler to the logger
+logging.basicConfig(level=logging.DEBUG, 
                     format='%(asctime)s  - %(name)s - %(levelname)s - %(message)s')
 logging.getLogger("SERVER/8086").setLevel(logging.CRITICAL)
 # Create a logger instance
 logger = logging.getLogger(__name__)
+logger.addHandler(file_handler)
 
 
-def start_(host_ip: Optional[str], bootstrap_nodes: Optional[str] = None):
-    # host_ip = socket.gethostbyname(socket.gethostname())
+def start_server(host_ip=None):
+    # host_ip = socket.gethostbynahost_ipme(socket.gethostname())
     broadcast = None
     logger.debug(host_ip)
+    bootstrap_nodes = None
     # print(host_ip)
     if host_ip is None:
         ip_br = get_ips()[0]
         broadcast = ip_br['broadcast']
         host_ip = ip_br['addr']
-    logger.debug(host_ip)
+    logger.info(host_ip)
 
     # print(host_ip)
     ms = Message_System(host_ip, broadcast)
     hosts = []
-    if bootstrap_nodes is None:
-        logger.info("No bootstrap Nodes given, trying to auto-detect")
 
-        msg = ms.receive()
-        logger.debug(msg)
-        if msg:
-            hosts.append(msg)
-            logger.debug("Found ", msg)
-            bootstrap_nodes = msg
-        else:
-            logger.info("No servers answered :(")
-        # time.sleep(1)
+    msg = ms.receive(service_name='dfs')
+    logger.debug(msg)
+    if msg:
+        hosts.append(msg)
+        logger.debug(f"Found {msg}")
+        bootstrap_nodes = msg
+    else:
+        logger.info("No servers answered :(")
+    # time.sleep(1)
 
     if host_ip is None:
+        logger.warning(f"aaa {socket.get_hostname()}")
         host_ip = socket.gethostbyname(socket.gethostname())
         # client_session = ClientSession(ip=host_ip)
 
     Server.init(ip=host_ip.split(" ")[0])
 
     logger.info(f"broadcasting {Server.node.ip} {Server.node.port}")
-    ms.add_to_send(f"{Server.node.ip} {Server.node.port}")
+    ms.add_to_send(f"dfs {Server.node.ip} {Server.node.port}")
     heartbeat_thread = threading.Thread(target=ms.send_heartbeat)
     heartbeat_thread.start()
-    # Server.init(ip="192.168.26.2")
+    # # Server.init(ip="192.168.26.2")
     if bootstrap_nodes:
         target_host, target_port = bootstrap_nodes.split(' ')
         Server.bootstrap([(target_host, target_port)])
 
     logger.info(f'Server started at {host_ip}')
 
 
 app = Typer()
 
 
 @app.command()
-def start(host_ip=Option(None), bootstrap_nodes=Option(None)):
+def _start(host_ip=Option(default=None)):
     logger.debug(host_ip)
-    if bootstrap_nodes:
-        start_(host_ip, bootstrap_nodes)
-    else:
-        start_(host_ip)
+    start_server(host_ip)
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `kade_drive-0.2.0/kade_drive/tests/conftest.py` & `kade_drive-0.3.0/kade_drive/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# import asyncio``
-import random
-import hashlib
-# pylint: disable=no-name-in-module
-from struct import pack
-
-import pytest
-
-from core.network import Server
-from core.node import Node
-from core.routing import RoutingTable
+# # import asyncio``
+# import random
+# import hashlib
+# # pylint: disable=no-name-in-module
+# from struct import pack
 
+# import pytest
 
-# @pytest.fixture()
-# def event_loop():
-#     return asyncio.get_event_loop()
+# from core.network import Server
+# from core.node import Node
+# from core.routing import RoutingTable
+
+
+# # @pytest.fixture()
+# # def event_loop():
+# #     return asyncio.get_event_loop()
+
+
+# # @pytest.fixture()
+# # def bootstrap_node():
+# #     server = Server()
+# #     server.listen(8468)
 
+#     # try:
+#     #     yield ('127.0.0.1', 8468)
+#     # finally:
+#     #     server.stop()
+#     #     event_loop.close()
 
+# # pylint: disable=redefined-outer-name
 # @pytest.fixture()
-# def bootstrap_node():
-#     server = Server()
-#     server.listen(8468)
-
-    # try:
-    #     yield ('127.0.0.1', 8468)
-    # finally:
-    #     server.stop()
-    #     event_loop.close()
-
-# pylint: disable=redefined-outer-name
-@pytest.fixture()
-def mknode():
-    def _mknode(node_id=None, ip_addy=None, port=None, intid=None):
-        """
-        Make a node.  Created a random id if not specified.
-        """
-        if intid is not None:
-            node_id = pack('>l', intid)
-        if not node_id:
-            randbits = str(random.getrandbits(255))
-            node_id = hashlib.sha1(randbits.encode()).digest()
-        return Node(node_id, ip_addy, port)
-    return _mknode
-
-
-# pylint: disable=too-few-public-methods
-class FakeProtocol:  # pylint: disable=too-few-public-methods
-    def __init__(self, source_id, ksize=20):
-        self.router = RoutingTable(ksize, Node(source_id))
-        self.storage = {}
-        self.source_id = source_id
-
-
-# pylint: disable=too-few-public-methods
-class FakeServer:
-    def __init__(self, node_id):
-        self.id = node_id  # pylint: disable=invalid-name
-        self.protocol = FakeProtocol(self.id)
-        self.router = self.protocol.router
-
-
-@pytest.fixture
-def fake_server(mknode):
-    return FakeServer(mknode().id)
+# def mknode():
+#     def _mknode(node_id=None, ip_addy=None, port=None, intid=None):
+#         """
+#         Make a node.  Created a random id if not specified.
+#         """
+#         if intid is not None:
+#             node_id = pack('>l', intid)
+#         if not node_id:
+#             randbits = str(random.getrandbits(255))
+#             node_id = hashlib.sha1(randbits.encode()).digest()
+#         return Node(node_id, ip_addy, port)
+#     return _mknode
+
+
+# # pylint: disable=too-few-public-methods
+# class FakeProtocol:  # pylint: disable=too-few-public-methods
+#     def __init__(self, source_id, ksize=20):
+#         self.router = RoutingTable(ksize, Node(source_id))
+#         self.storage = {}
+#         self.source_id = source_id
+
+
+# # pylint: disable=too-few-public-methods
+# class FakeServer:
+#     def __init__(self, node_id):
+#         self.id = node_id  # pylint: disable=invalid-name
+#         self.protocol = FakeProtocol(self.id)
+#         self.router = self.protocol.router
+
+
+# @pytest.fixture
+# def fake_server(mknode):
+#     return FakeServer(mknode().id)
```

### Comparing `kade_drive-0.2.0/kade_drive/tests/data_to_split.txt` & `kade_drive-0.3.0/kade_drive/tests/data_to_split.txt`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/tests/test_node.py` & `kade_drive-0.3.0/kade_drive/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/tests/test_routing.py` & `kade_drive-0.3.0/kade_drive/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/tests/test_splitdata.py` & `kade_drive-0.3.0/kade_drive/tests/test_splitdata.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/tests/test_storage.py` & `kade_drive-0.3.0/kade_drive/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/kade_drive/tests/test_store_file.py` & `kade_drive-0.3.0/kade_drive/test_store_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from sklearn.datasets import load_diabetes
 import pandas as pd
 import pickle
 from client import ClientSession
+from time import sleep
+
 
 def test_store_df():
     X, y = load_diabetes(return_X_y=True)
 
     X = pd.DataFrame(X)
     y = pd.DataFrame(y)
 
@@ -15,15 +17,18 @@
     initial_bootstrap_nodes = []
     client_session = ClientSession(initial_bootstrap_nodes)
 
     client_session.connect(use_broadcast_if_needed=True)
 
     client_session.put("dataset_diabetes", X_pickle)
 
-
     print("DONE, Getting")
     print()
     print()
+    sleep(5)
     value_getted = client_session.get("dataset_diabetes")
 
     print('value getted ', value_getted)
-    assert X.equals(value_getted)
+    assert X.equals(value_getted)
+
+
+test_store_df()
```

### Comparing `kade_drive-0.2.0/kade_drive/tests/test_utils.py` & `kade_drive-0.3.0/kade_drive/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.2.0/PKG-INFO` & `kade_drive-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 Metadata-Version: 2.1
 Name: kade-drive
-Version: 0.2.0
+Version: 0.3.0
 Summary: distributed file system based on kademlia dht
 License: MIT
 Author: DanielUH2019
 Author-email: danielcardenascabrera2016@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: netifaces (==0.11.0)
 Requires-Dist: rpyc (==5.3.1)
 Requires-Dist: typer (==0.9.0)
 Description-Content-Type: text/markdown
 
-Sistema de ficheros distribuidos immplementado usando el codigo fuente de la implementacion de Kademlia en https://github.com/bmuller/kademlia 
+Distributed file system based on <https://github.com/bmuller/kademlia>
 
+
+## Basic Usage
+
+- Clone the repo and run poetry install
+- Run server.py in one pc or several pc in a local network
+- Run cli.py in any pc of the network and start playing with the system
+
+## Installation
+
+- pip install kade-drive
+  
 ### Tests
-Para Correr los tests se requiere un servidor levantado en la red
+
+To run tests make shure that there is at least one server in the network.
+
```

