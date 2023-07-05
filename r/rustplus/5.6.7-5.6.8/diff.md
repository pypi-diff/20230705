# Comparing `tmp/rustplus-5.6.7.tar.gz` & `tmp/rustplus-5.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustplus-5.6.7.tar", last modified: Tue Jun 27 14:50:47 2023, max compression
+gzip compressed data, was "rustplus-5.6.8.tar", last modified: Wed Jul  5 19:24:14 2023, max compression
```

## Comparing `rustplus-5.6.7.tar` & `rustplus-5.6.8.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.197667 rustplus-5.6.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-27 14:50:35.000000 rustplus-5.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-27 14:50:35.000000 rustplus-5.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-27 14:50:47.197667 rustplus-5.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-06-27 14:50:35.000000 rustplus-5.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.189666 rustplus-5.6.7/rustplus/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.189666 rustplus-5.6.7/rustplus/api/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20421 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/base_rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/api/icons/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/airfield.png
--rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/arctic_base.png
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/bandit.png
--rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/barn.png
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/cargo.png
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/chinook.png
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/chinook_blades.png
--rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/crate.png
--rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/desert_base.png
--rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/dome.png
--rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/excavator.png
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/explosion.png
--rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/fishing.png
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/harbour.png
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/icon.png
--rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/junkyard.png
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/large_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/launchsite.png
--rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/lighthouse.png
--rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/military_tunnels.png
--rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/mining_outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/outpost.png
--rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/oxums.png
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/patrol.png
--rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/power_plant.png
--rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/quarry.png
--rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/satellite.png
--rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/sewer.png
--rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/small_oil_rig.png
--rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/stable.png
--rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/supermarket.png
--rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/swamp.png
--rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/train.png
--rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/train_yard.png
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/underwater_lab.png
--rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/vending_machine.png
--rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/icons/water_treatment.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/api/remote/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/api/remote/camera/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/camera/camera_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5711 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/camera/camera_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/camera/camera_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/camera/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/api/remote/events/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/event_loop_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/handler_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/map_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/events/registered_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/expo_bundle_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/fcm_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/rust_remote_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/api/remote/rustplus_proto/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/rustplus_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/rustplus_proto/rustplus.py
--rw-r--r--   0 runner    (1001) docker     (122)    12816 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/rustws.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/remote/server_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)    13828 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/rust_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/api/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_contents.py
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_entity_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_map.py
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_team_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/rust_time.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/api/structures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/commands/command_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/commands/command_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/commands/command_options.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.193667 rustplus-5.6.7/rustplus/conversation/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/conversation/conversation_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/conversation/conversation_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.197667 rustplus-5.6.7/rustplus/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.197667 rustplus-5.6.7/rustplus/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.197667 rustplus-5.6.7/rustplus/utils/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/fonts/PermanentMarker.ttf
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27724 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/grab_items.py
--rw-r--r--   0 runner    (1001) docker     (122)     5388 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/server_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-27 14:50:35.000000 rustplus-5.6.7/rustplus/utils/yielding_event.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 14:50:47.189666 rustplus-5.6.7/rustplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-06-27 14:50:47.000000 rustplus-5.6.7/rustplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-06-27 14:50:47.000000 rustplus-5.6.7/rustplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 14:50:47.000000 rustplus-5.6.7/rustplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-27 14:50:47.000000 rustplus-5.6.7/rustplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-27 14:50:47.000000 rustplus-5.6.7/rustplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-27 14:50:47.197667 rustplus-5.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-27 14:50:35.000000 rustplus-5.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-05 19:24:06.000000 rustplus-5.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-05 19:24:06.000000 rustplus-5.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-05 19:24:14.875584 rustplus-5.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-05 19:24:06.000000 rustplus-5.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.867584 rustplus-5.6.8/rustplus/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.867584 rustplus-5.6.8/rustplus/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/base_rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23598 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/airfield.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13944 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/arctic_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/bandit.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35348 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/barn.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/cargo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/chinook.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/chinook_blades.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23420 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/crate.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12339 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/desert_base.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34156 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/dome.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34662 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/excavator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/explosion.png
+-rw-r--r--   0 runner    (1001) docker     (122)    24176 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/fishing.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/harbour.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41087 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/junkyard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/large_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23696 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/launchsite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27391 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/lighthouse.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23532 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/military_tunnels.png
+-rw-r--r--   0 runner    (1001) docker     (122)    27923 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/mining_outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30573 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/outpost.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/oxums.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/patrol.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23513 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/power_plant.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36433 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/quarry.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28365 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/satellite.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17804 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/sewer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8114 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/small_oil_rig.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30710 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/stable.png
+-rw-r--r--   0 runner    (1001) docker     (122)    28458 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/supermarket.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2049 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/swamp.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5300 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/train.png
+-rw-r--r--   0 runner    (1001) docker     (122)    20587 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/train_yard.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/underwater_lab.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5705 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/vending_machine.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23907 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/icons/water_treatment.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/remote/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   118649 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/camera_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/camera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24457 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/camera_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/camera/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.871584 rustplus-5.6.8/rustplus/api/remote/events/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/event_loop_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/handler_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/map_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/events/registered_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/expo_bundle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/fcm_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rust_remote_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/api/remote/rustplus_proto/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rustplus_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16144 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rustplus_proto/rustplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12828 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/rustws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/remote/server_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13358 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/rust_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/api/structures/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_contents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_entity_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_team_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/rust_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/api/structures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/commands/command_options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/conversation/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/conversation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/conversation/conversation_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.875584 rustplus-5.6.8/rustplus/utils/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)    74752 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/fonts/PermanentMarker.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27771 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/grab_items.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6950 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-05 19:24:06.000000 rustplus-5.6.8/rustplus/utils/yielding_event.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:24:14.867584 rustplus-5.6.8/rustplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3536 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-05 19:24:14.000000 rustplus-5.6.8/rustplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-05 19:24:14.875584 rustplus-5.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-05 19:24:06.000000 rustplus-5.6.8/setup.py
```

### Comparing `rustplus-5.6.7/LICENSE` & `rustplus-5.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/PKG-INFO` & `rustplus-5.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.7
+Version: 5.6.8
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.6.7/README.md` & `rustplus-5.6.8/README.md`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/__init__.py` & `rustplus-5.6.8/rustplus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .commands import CommandOptions, Command
 from .exceptions import *
 from .conversation import ConversationFactory, Conversation, ConversationPrompt
 from .utils import *
 
 __name__ = "rustplus"
 __author__ = "olijeffers0n"
-__version__ = "5.6.7"
+__version__ = "5.6.8"
 __support__ = "Discord: https://discord.gg/nQqJe8qvP8"
```

### Comparing `rustplus-5.6.7/rustplus/api/base_rust_api.py` & `rustplus-5.6.8/rustplus/api/base_rust_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,14 @@
 
         :return: None
         """
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
         app_request.get_time = AppEmpty()
-        app_request.get_time._serialized_on_wire = True
 
         await self.remote.add_ignored_response(app_request.seq)
 
         await self.remote.send_message(app_request)
 
     async def switch_server(
         self,
@@ -441,14 +440,15 @@
 
         :returns Nothing, This will never return
         """
 
         while True:
             await asyncio.sleep(1)
 
+    @deprecated("Implement this yourself. This will be removed in thed future")
     def get_conversation_factory(self) -> ConversationFactory:
         """
         Gets the current ConversationFactory object
 
         :returns ConversationFactory: the factory
         """
         return self.remote.conversation_factory
```

### Comparing `rustplus-5.6.7/rustplus/api/icons/airfield.png` & `rustplus-5.6.8/rustplus/api/icons/airfield.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/arctic_base.png` & `rustplus-5.6.8/rustplus/api/icons/arctic_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/bandit.png` & `rustplus-5.6.8/rustplus/api/icons/bandit.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/barn.png` & `rustplus-5.6.8/rustplus/api/icons/barn.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/cargo.png` & `rustplus-5.6.8/rustplus/api/icons/cargo.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/chinook.png` & `rustplus-5.6.8/rustplus/api/icons/chinook.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/chinook_blades.png` & `rustplus-5.6.8/rustplus/api/icons/chinook_blades.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/crate.png` & `rustplus-5.6.8/rustplus/api/icons/crate.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/desert_base.png` & `rustplus-5.6.8/rustplus/api/icons/desert_base.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/dome.png` & `rustplus-5.6.8/rustplus/api/icons/dome.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/excavator.png` & `rustplus-5.6.8/rustplus/api/icons/excavator.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/explosion.png` & `rustplus-5.6.8/rustplus/api/icons/explosion.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/fishing.png` & `rustplus-5.6.8/rustplus/api/icons/fishing.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/harbour.png` & `rustplus-5.6.8/rustplus/api/icons/harbour.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/icon.png` & `rustplus-5.6.8/rustplus/api/icons/icon.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/junkyard.png` & `rustplus-5.6.8/rustplus/api/icons/junkyard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/large_oil_rig.png` & `rustplus-5.6.8/rustplus/api/icons/large_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/launchsite.png` & `rustplus-5.6.8/rustplus/api/icons/launchsite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/lighthouse.png` & `rustplus-5.6.8/rustplus/api/icons/lighthouse.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/military_tunnels.png` & `rustplus-5.6.8/rustplus/api/icons/military_tunnels.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/mining_outpost.png` & `rustplus-5.6.8/rustplus/api/icons/mining_outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/outpost.png` & `rustplus-5.6.8/rustplus/api/icons/outpost.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/oxums.png` & `rustplus-5.6.8/rustplus/api/icons/oxums.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/patrol.png` & `rustplus-5.6.8/rustplus/api/icons/patrol.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/power_plant.png` & `rustplus-5.6.8/rustplus/api/icons/power_plant.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/quarry.png` & `rustplus-5.6.8/rustplus/api/icons/quarry.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/satellite.png` & `rustplus-5.6.8/rustplus/api/icons/satellite.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/sewer.png` & `rustplus-5.6.8/rustplus/api/icons/sewer.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/small_oil_rig.png` & `rustplus-5.6.8/rustplus/api/icons/small_oil_rig.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/stable.png` & `rustplus-5.6.8/rustplus/api/icons/stable.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/supermarket.png` & `rustplus-5.6.8/rustplus/api/icons/supermarket.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/swamp.png` & `rustplus-5.6.8/rustplus/api/icons/swamp.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/train.png` & `rustplus-5.6.8/rustplus/api/icons/train.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/train_yard.png` & `rustplus-5.6.8/rustplus/api/icons/train_yard.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/underwater_lab.png` & `rustplus-5.6.8/rustplus/api/icons/underwater_lab.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/vending_machine.png` & `rustplus-5.6.8/rustplus/api/icons/vending_machine.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/icons/water_treatment.png` & `rustplus-5.6.8/rustplus/api/icons/water_treatment.png`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/camera/camera_constants.py` & `rustplus-5.6.8/rustplus/api/remote/camera/camera_constants.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/camera/camera_manager.py` & `rustplus-5.6.8/rustplus/api/remote/camera/camera_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import time
-from typing import Iterable, Union, List, Coroutine, TypeVar, Set, Callable
+from typing import Iterable, Union, List, Coroutine, Set, Callable
 
 from PIL import Image
 
 from .camera_parser import Parser
 from ..rustplus_proto import (
     AppCameraInput,
     Vector2,
     AppEmpty,
     AppRequest,
     AppCameraInfo,
 )
 from ...structures import Vector
 from .structures import CameraInfo, Entity, LimitedQueue
 
-RS = TypeVar("RS", bound="RustSocket")
-
 
 class CameraManager:
     def __init__(
-        self, rust_socket: RS, cam_id: str, cam_info_message: AppCameraInfo
+        self, rust_socket, cam_id: str, cam_info_message: AppCameraInfo
     ) -> None:
-        self.rust_socket: RS = rust_socket
+        self.rust_socket = rust_socket
         self._cam_id: str = cam_id
         self._last_packets: LimitedQueue = LimitedQueue(6)
         self._cam_info_message: CameraInfo = CameraInfo(cam_info_message)
         self._open: bool = True
         self.parser: Parser = Parser(
             self._cam_info_message.width, self._cam_info_message.height
         )
@@ -136,15 +134,14 @@
         await self.rust_socket.remote.send_message(app_request)
         await self.rust_socket.remote.add_ignored_response(app_request.seq)
 
     async def exit_camera(self) -> None:
         await self.rust_socket._handle_ratelimit()
         app_request: AppRequest = self.rust_socket._generate_protobuf()
         app_request.camera_unsubscribe = AppEmpty()
-        app_request.camera_unsubscribe._serialized_on_wire = True
 
         await self.rust_socket.remote.send_message(app_request)
         await self.rust_socket.remote.add_ignored_response(app_request.seq)
 
         self._open = False
         self._last_packets.clear()
```

### Comparing `rustplus-5.6.7/rustplus/api/remote/camera/camera_parser.py` & `rustplus-5.6.8/rustplus/api/remote/camera/camera_parser.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/camera/structures.py` & `rustplus-5.6.8/rustplus/api/remote/camera/structures.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/events/event_handler.py` & `rustplus-5.6.8/rustplus/api/remote/events/event_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,36 +15,30 @@
             server_id
         ).get(str(name))
 
         if handlers is None:
             return
 
         for handler in handlers.copy():
-            coro, event_type = handler.data
-
-            await coro(EntityEvent(app_message, event_type))
+            await handler.get_coro()(
+                EntityEvent(app_message, handler.get_entity_type())
+            )
 
     @staticmethod
     async def run_team_event(app_message: AppMessage, server_id: ServerID) -> None:
         handlers: Set[RegisteredListener] = TeamEvent.handlers.get_handlers(server_id)
         for handler in handlers.copy():
-            coro = handler.data
-
-            await coro(TeamEvent(app_message))
+            await handler.get_coro()(TeamEvent(app_message))
 
     @staticmethod
     async def run_chat_event(app_message: AppMessage, server_id: ServerID) -> None:
         handlers: Set[RegisteredListener] = ChatEvent.handlers.get_handlers(server_id)
         for handler in handlers.copy():
-            coro = handler.data
-
-            await coro(ChatEvent(app_message))
+            await handler.get_coro()(ChatEvent(app_message))
 
     @staticmethod
     async def run_proto_event(byte_data: bytes, server_id: ServerID) -> None:
         handlers: Set[RegisteredListener] = ProtobufEvent.handlers.get_handlers(
             server_id
         )
         for handler in handlers.copy():
-            coro = handler.data
-
-            await coro(ProtobufEvent(byte_data))
+            await handler.get_coro()(ProtobufEvent(byte_data))
```

### Comparing `rustplus-5.6.7/rustplus/api/remote/events/event_loop_manager.py` & `rustplus-5.6.8/rustplus/api/remote/events/event_loop_manager.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/events/events.py` & `rustplus-5.6.8/rustplus/api/remote/events/events.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/events/handler_list.py` & `rustplus-5.6.8/rustplus/api/remote/events/handler_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self, server_id: ServerID
     ) -> Dict[ServerID, Set[RegisteredListener]]:
         return self._handlers.get(server_id, set())
 
 
 class EntityHandlerList(HandlerList):
     def __init__(self) -> None:
+        super().__init__()
         self._handlers: Dict[
             ServerID, Dict[str, Set[RegisteredListener]]
         ] = defaultdict(dict)
 
     def unregister(self, listener: RegisteredListener, server_id: ServerID) -> None:
         if listener.listener_id in self._handlers.get(server_id):
             self._handlers.get(server_id).get(listener.listener_id).remove(listener)
```

### Comparing `rustplus-5.6.7/rustplus/api/remote/events/map_event_listener.py` & `rustplus-5.6.8/rustplus/api/remote/events/map_event_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/expo_bundle_handler.py` & `rustplus-5.6.8/rustplus/api/remote/expo_bundle_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import requests
 import logging
 
 
 class MagicValueGrabber:
     @staticmethod
     def get_magic_value() -> int:
-
-        data = requests.get(
-            "https://companion-rust.facepunch.com/api/version"
-        )
+        data = requests.get("https://companion-rust.facepunch.com/api/version")
 
         if data.status_code == 200:
             data = data.json()
             time = data.get("minPublishedTime", None)
             if time is not None:
                 return time + 1
```

### Comparing `rustplus-5.6.7/rustplus/api/remote/fcm_listener.py` & `rustplus-5.6.8/rustplus/api/remote/fcm_listener.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/heartbeat.py` & `rustplus-5.6.8/rustplus/api/remote/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/ratelimiter.py` & `rustplus-5.6.8/rustplus/api/remote/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/rust_remote_interface.py` & `rustplus-5.6.8/rustplus/api/remote/rust_remote_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,14 @@
 
         async def get_entity_info(remote: RustRemote, eid):
             await remote.api._handle_ratelimit()
 
             app_request: AppRequest = remote.api._generate_protobuf()
             app_request.entity_id = eid
             app_request.get_entity_info = AppEmpty()
-            app_request.get_entity_info._serialized_on_wire = True
 
             await remote.send_message(app_request)
 
             return await remote.get_response(app_request.seq, app_request, False)
 
         def entity_event_callback(future_inner: Future) -> None:
             entity_info: AppMessage = future_inner.result()
@@ -192,15 +191,15 @@
             if betterproto.serialized_on_wire(entity_info.response.error):
                 raise SmartDeviceRegistrationError(
                     f"Entity: '{entity_id}' has not been found"
                 )
 
             EntityEvent.handlers.register(
                 RegisteredListener(
-                    entity_id, (coroutine, entity_info.response.entity_info.type)
+                    entity_id, coroutine, entity_info.response.entity_info.type
                 ),
                 self.server_id,
             )
 
         future = asyncio.run_coroutine_threadsafe(
             get_entity_info(self, entity_id), EventLoopManager.get_loop(self.server_id)
         )
```

### Comparing `rustplus-5.6.7/rustplus/api/remote/rustplus_proto/rustplus.py` & `rustplus-5.6.8/rustplus/api/remote/rustplus_proto/rustplus.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/remote/rustws.py` & `rustplus-5.6.8/rustplus/api/remote/rustws.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,27 +302,27 @@
         return betterproto.serialized_on_wire(app_message.broadcast.team_changed)
 
     @staticmethod
     def get_proto_cost(app_request: AppRequest) -> int:
         """
         Gets the cost of an AppRequest
         """
-        costs = {
-            app_request.get_time: 1,
-            app_request.send_team_message: 2,
-            app_request.get_info: 1,
-            app_request.get_team_chat: 1,
-            app_request.get_team_info: 1,
-            app_request.get_map_markers: 1,
-            app_request.get_map: 5,
-            app_request.set_entity_value: 1,
-            app_request.get_entity_info: 1,
-            app_request.promote_to_leader: 1,
-        }
-        for request, cost in costs.items():
+        costs = [
+            (app_request.get_time, 1),
+            (app_request.send_team_message, 2),
+            (app_request.get_info, 1),
+            (app_request.get_team_chat, 1),
+            (app_request.get_team_info, 1),
+            (app_request.get_map_markers, 1),
+            (app_request.get_map, 5),
+            (app_request.set_entity_value, 1),
+            (app_request.get_entity_info, 1),
+            (app_request.promote_to_leader, 1),
+        ]
+        for request, cost in costs:
             if betterproto.serialized_on_wire(request):
                 return cost
 
         raise ValueError()
 
     @staticmethod
     def error_present(message) -> bool:
```

### Comparing `rustplus-5.6.7/rustplus/api/remote/server_checker.py` & `rustplus-5.6.8/rustplus/api/remote/server_checker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/rust_api.py` & `rustplus-5.6.8/rustplus/api/rust_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         )
 
     async def get_time(self) -> RustTime:
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
         app_request.get_time = AppEmpty()
-        app_request.get_time._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         response = await self.remote.get_response(app_request.seq, app_request)
 
         return format_time(response)
 
@@ -98,71 +97,66 @@
         await self.remote.send_message(app_request)
 
     async def get_info(self) -> RustInfo:
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
         app_request.get_info = AppEmpty()
-        app_request.get_info._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         response = await self.remote.get_response(app_request.seq, app_request)
 
         return RustInfo(response.response.info)
 
     async def get_team_chat(self) -> List[RustChatMessage]:
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
         app_request.get_team_chat = AppEmpty()
-        app_request.get_team_chat._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         messages = (
             await self.remote.get_response(app_request.seq, app_request)
         ).response.team_chat.messages
 
         return [RustChatMessage(message) for message in messages]
 
     async def get_team_info(self) -> RustTeamInfo:
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
         app_request.get_team_info = AppEmpty()
-        app_request.get_team_info._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         return RustTeamInfo(app_message.response.team_info)
 
     async def get_markers(self) -> List[RustMarker]:
         await self._handle_ratelimit()
 
         app_request = self._generate_protobuf()
         app_request.get_map_markers = AppEmpty()
-        app_request.get_map_markers._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         return [
             RustMarker(marker) for marker in app_message.response.map_markers.markers
         ]
 
     async def get_raw_map_data(self) -> RustMap:
         await self._handle_ratelimit(5)
 
         app_request = self._generate_protobuf()
         app_request.get_map = AppEmpty()
-        app_request.get_map._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         return RustMap(app_message.response.map)
 
@@ -186,15 +180,14 @@
                 if [add_icons, add_events, add_vending_machines].count(True) >= 1
                 else 0
             )
         )
 
         app_request = self._generate_protobuf()
         app_request.get_map = AppEmpty()
-        app_request.get_map._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         game_map = app_message.response.map
         monuments = list(game_map.monuments)
@@ -291,15 +284,14 @@
 
         if eid is None:
             raise ValueError("EID cannot be None")
 
         app_request = self._generate_protobuf()
         app_request.entity_id = eid
         app_request.get_entity_info = AppEmpty()
-        app_request.get_entity_info._serialized_on_wire = True
 
         await self.remote.send_message(app_request)
 
         app_message = await self.remote.get_response(app_request.seq, app_request)
 
         return RustEntityInfo(app_message.response.entity_info)
```

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_chat_message.py` & `rustplus-5.6.8/rustplus/api/structures/rust_chat_message.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_contents.py` & `rustplus-5.6.8/rustplus/api/structures/rust_contents.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_entity_info.py` & `rustplus-5.6.8/rustplus/api/structures/rust_entity_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_info.py` & `rustplus-5.6.8/rustplus/api/structures/rust_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_item.py` & `rustplus-5.6.8/rustplus/api/structures/rust_item.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_map.py` & `rustplus-5.6.8/rustplus/api/structures/rust_map.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_marker.py` & `rustplus-5.6.8/rustplus/api/structures/rust_marker.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_team_info.py` & `rustplus-5.6.8/rustplus/api/structures/rust_team_info.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/api/structures/rust_time.py` & `rustplus-5.6.8/rustplus/api/structures/rust_time.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/commands/command.py` & `rustplus-5.6.8/rustplus/commands/command.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/commands/command_data.py` & `rustplus-5.6.8/rustplus/commands/command_data.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/commands/command_handler.py` & `rustplus-5.6.8/rustplus/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/conversation/conversation.py` & `rustplus-5.6.8/rustplus/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/conversation/conversation_factory.py` & `rustplus-5.6.8/rustplus/conversation/conversation_factory.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/exceptions/exceptions.py` & `rustplus-5.6.8/rustplus/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/utils/deprecated.py` & `rustplus-5.6.8/rustplus/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/utils/fonts/PermanentMarker.ttf` & `rustplus-5.6.8/rustplus/utils/fonts/PermanentMarker.ttf`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/utils/grab_items.py` & `rustplus-5.6.8/rustplus/utils/grab_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,15 +736,15 @@
     "2087678962": "Search Light",
     "2090395347": "Large Solar Panel",
     "2100007442": "Audio Alarm",
     "2104517339": "Strobe Light",
     "2106561762": "Decorative Tinsel",
     "2114754781": "Water Purifier",
     "2126889441": "Santa Beard",
-    "2133269020": "Red Berry Clone"
+    "2133269020": "Red Berry Clone",
 }
 stack_to_id = {}
 
 
 def translate_id_to_stack(value_id: Union[str, int]) -> str:
     global item_ids
     try:
@@ -761,32 +761,36 @@
             stack_to_id[item_ids[i].lower()] = i
     try:
         return stack_to_id[item.lower()]
     except KeyError:
         return "Not Found"
 
 
-def grab_items(reversed = False) -> None:
+def grab_items(reversed=False) -> None:
     data = {}
 
     for line in (
         requests.get(
             "https://raw.githubusercontent.com/olijeffers0n/RustItems/master/data/items.md"
         )
         .content.decode()
         .splitlines(False)[2:]
     ):
-        if len(line) == 0: continue
+        if len(line) == 0:
+            continue
 
         item = line.split("|")[1:-1]
 
-        if item[1] == "" or item[2] == "N/A": continue
+        if item[1] == "" or item[2] == "N/A":
+            continue
 
-        if not reversed: data[int(item[2])] = item[0]
-        else: data[str(item[0])] = int(item[2])
+        if not reversed:
+            data[int(item[2])] = item[0]
+        else:
+            data[str(item[0])] = int(item[2])
 
     with open("rust_items.json", "w") as output:
         json.dump(data, output, indent=4, sort_keys=True)
 
 
 if __name__ == "__main__":
     grab_items()
```

### Comparing `rustplus-5.6.7/rustplus/utils/rust_utils.py` & `rustplus-5.6.8/rustplus/utils/rust_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import string
 
 from ..api.remote.rustplus_proto import AppMessage
 from ..api.structures import RustTime
 
 icons_path = "rustplus.api.icons"
+GRID_DIAMETER = 146.28571428571428
 
 
 def format_time(protobuf: AppMessage) -> RustTime:
     def convert_time(time) -> str:
         hours, minutes = divmod(time * 60, 60)
 
         return (
@@ -153,20 +154,81 @@
         return "Alarm"
     elif id == 3:
         return "Storage Monitor"
     else:
         raise ValueError("Not Valid type")
 
 
+def _get_grid_x(x):
+    counter = 1
+    start_grid = 0
+    while start_grid < x + GRID_DIAMETER:
+        if start_grid <= x <= (start_grid + GRID_DIAMETER):
+            # We're at the correct grid!
+            return _number_to_letters(counter)
+
+        counter += 1
+        start_grid += GRID_DIAMETER
+
+
+def _get_grid_y(y, map_size):
+    counter = 1
+    number_of_grids = map_size // GRID_DIAMETER
+    start_grid = 0
+    while start_grid < y + GRID_DIAMETER:
+        if start_grid <= y <= (start_grid + GRID_DIAMETER):
+            return number_of_grids - counter
+        counter += 1
+        start_grid += GRID_DIAMETER
+
+
+def _number_to_letters(num):
+    power, mod = divmod(num, 26)
+    out = chr(64 + mod) if mod else (power, "Z")
+    return _number_to_letters(power) + out if power else out
+
+
+def _get_corrected_map_size(map_size):
+    remainder = map_size % GRID_DIAMETER
+    offset = GRID_DIAMETER - remainder
+    return map_size - remainder if remainder < 120 else map_size + offset
+
+
+def _is_outside_grid_system(x, y, map_size, offset=0):
+    return (
+        x < -offset or x > (map_size + offset) or y < -offset or y > (map_size + offset)
+    )
+
+
+class HackyBackwardsCompatCoordClass:
+    def __init__(self, x, y):
+        self.x = x
+        self.y = y
+
+    def __getitem__(self, item):
+        if item == 0:
+            return self.x
+        elif item == 1:
+            return self.y
+        else:
+            raise IndexError("Index out of range")
+
+    def __iter__(self):
+        yield self.x
+        yield self.y
+
+    def __repr__(self):
+        return f"{self.x}{self.y}"
+
+    def __str__(self):
+        return self.__repr__()
+
+
 def convert_xy_to_grid(
     coords: tuple, map_size: float, catch_out_of_bounds: bool = True
-) -> Tuple[int, int]:
-    grid_size = 146.3
-    grids = list(string.ascii_uppercase) + [
-        f"A{letter}" for letter in list(string.ascii_uppercase)
-    ]
-
-    if coords[0] > map_size or coords[0] < 0 or coords[1] > map_size or coords[1] < 0:
-        if catch_out_of_bounds:
-            raise ValueError("Out of bounds")
+) -> HackyBackwardsCompatCoordClass:
+    corrected_map_size = _get_corrected_map_size(map_size)
+
+    grid_pos_letters = _get_grid_x(coords[0])
+    grid_pos_number = str(int(_get_grid_y(coords[1], corrected_map_size)))
 
-    return grids[int(coords[0] // grid_size)], int((map_size - coords[1]) // grid_size)
+    return HackyBackwardsCompatCoordClass(grid_pos_letters, grid_pos_number)
```

### Comparing `rustplus-5.6.7/rustplus/utils/server_id.py` & `rustplus-5.6.8/rustplus/utils/server_id.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus/utils/yielding_event.py` & `rustplus-5.6.8/rustplus/utils/yielding_event.py`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/rustplus.egg-info/PKG-INFO` & `rustplus-5.6.8/rustplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustplus
-Version: 5.6.7
+Version: 5.6.8
 Summary: A python wrapper for the Rust Plus API
 Home-page: https://github.com/olijeffers0n/rustplus
 Author: olijeffers0n
 License: MIT
 Project-URL: Issue tracker, https://github.com/olijeffers0n/rustplus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `rustplus-5.6.7/rustplus.egg-info/SOURCES.txt` & `rustplus-5.6.8/rustplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustplus-5.6.7/setup.py` & `rustplus-5.6.8/setup.py`

 * *Files identical despite different names*

