# Comparing `tmp/google-maps-routing-0.6.0.tar.gz` & `tmp/google-maps-routing-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-routing-0.6.0.tar", last modified: Thu Jun 29 16:30:01 2023, max compression
+gzip compressed data, was "google-maps-routing-0.6.1.tar", last modified: Wed Jul  5 15:57:19 2023, max compression
```

## Comparing `google-maps-routing-0.6.0.tar` & `google-maps-routing-0.6.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.050019 google-maps-routing-0.6.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4657 2023-06-29 16:30:01.050019 google-maps-routing-0.6.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3751 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.034021 google-maps-routing-0.6.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/routing/
--rw-rw-r--   0 root         (0)     1003     4023 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/routing_v2/
--rw-rw-r--   0 root         (0)     1003     3360 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1387 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.038021 google-maps-routing-0.6.0/google/maps/routing_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.042020 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/
--rw-rw-r--   0 root         (0)     1003      737 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/__init__.py
--rw-rw-r--   0 root         (0)     1003    18889 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/async_client.py
--rw-rw-r--   0 root         (0)     1003    27740 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.042020 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6500 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17041 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17278 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17558 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/google/maps/routing_v2/types/
--rw-rw-r--   0 root         (0)     1003     2685 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3426 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/fallback_info.py
--rw-rw-r--   0 root         (0)     1003     4200 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/geocoding_results.py
--rw-rw-r--   0 root         (0)     1003     1659 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/localized_time.py
--rw-rw-r--   0 root         (0)     1003     2027 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/location.py
--rw-rw-r--   0 root         (0)     1003     2766 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/maneuver.py
--rw-rw-r--   0 root         (0)     1003     1685 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/navigation_instruction.py
--rw-rw-r--   0 root         (0)     1003     3876 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/polyline.py
--rw-rw-r--   0 root         (0)     1003    31508 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route.py
--rw-rw-r--   0 root         (0)     1003     1856 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route_label.py
--rw-rw-r--   0 root         (0)     1003     3600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route_modifiers.py
--rw-rw-r--   0 root         (0)     1003     1962 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/route_travel_mode.py
--rw-rw-r--   0 root         (0)     1003    29064 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/routes_service.py
--rw-rw-r--   0 root         (0)     1003     2609 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/routing_preference.py
--rw-rw-r--   0 root         (0)     1003     2809 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/speed_reading_interval.py
--rw-rw-r--   0 root         (0)     1003     1886 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_info.py
--rw-rw-r--   0 root         (0)     1003    11021 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_passes.py
--rw-rw-r--   0 root         (0)     1003     2240 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/traffic_model.py
--rw-rw-r--   0 root         (0)     1003     7327 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/transit.py
--rw-rw-r--   0 root         (0)     1003     3209 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/transit_preferences.py
--rw-rw-r--   0 root         (0)     1003     1337 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/units.py
--rw-rw-r--   0 root         (0)     1003     1609 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_emission_type.py
--rw-rw-r--   0 root         (0)     1003     1502 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_info.py
--rw-rw-r--   0 root         (0)     1003     4688 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/google/maps/routing_v2/types/waypoint.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/google_maps_routing.egg-info/
--rw-r--r--   0 root         (0)     1003     4657 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2346 2023-06-29 16:30:01.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       19 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      348 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-29 16:30:00.000000 google-maps-routing-0.6.0/google_maps_routing.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-29 16:30:01.050019 google-maps-routing-0.6.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2965 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:30:01.046020 google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    73205 2023-06-29 16:26:38.000000 google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/test_routes.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.024684 google-maps-routing-0.6.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4657 2023-07-05 15:57:19.024684 google-maps-routing-0.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3751 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.012679 google-maps-routing-0.6.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.012679 google-maps-routing-0.6.1/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.016681 google-maps-routing-0.6.1/google/maps/routing/
+-rw-rw-r--   0 root         (0)     1003     4023 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.016681 google-maps-routing-0.6.1/google/maps/routing_v2/
+-rw-rw-r--   0 root         (0)     1003     3360 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1387 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.016681 google-maps-routing-0.6.1/google/maps/routing_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.016681 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/
+-rw-rw-r--   0 root         (0)     1003      737 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18912 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27740 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.016681 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6500 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17041 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17278 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17558 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.020682 google-maps-routing-0.6.1/google/maps/routing_v2/types/
+-rw-rw-r--   0 root         (0)     1003     2685 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3426 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/fallback_info.py
+-rw-rw-r--   0 root         (0)     1003     4200 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/geocoding_results.py
+-rw-rw-r--   0 root         (0)     1003     1659 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/localized_time.py
+-rw-rw-r--   0 root         (0)     1003     2027 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/location.py
+-rw-rw-r--   0 root         (0)     1003     2766 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/maneuver.py
+-rw-rw-r--   0 root         (0)     1003     1685 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/navigation_instruction.py
+-rw-rw-r--   0 root         (0)     1003     3876 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/polyline.py
+-rw-rw-r--   0 root         (0)     1003    31508 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/route.py
+-rw-rw-r--   0 root         (0)     1003     1856 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/route_label.py
+-rw-rw-r--   0 root         (0)     1003     3600 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/route_modifiers.py
+-rw-rw-r--   0 root         (0)     1003     1962 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/route_travel_mode.py
+-rw-rw-r--   0 root         (0)     1003    29064 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/routes_service.py
+-rw-rw-r--   0 root         (0)     1003     2609 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/routing_preference.py
+-rw-rw-r--   0 root         (0)     1003     2809 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/speed_reading_interval.py
+-rw-rw-r--   0 root         (0)     1003     1886 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/toll_info.py
+-rw-rw-r--   0 root         (0)     1003    11021 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/toll_passes.py
+-rw-rw-r--   0 root         (0)     1003     2240 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/traffic_model.py
+-rw-rw-r--   0 root         (0)     1003     7327 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/transit.py
+-rw-rw-r--   0 root         (0)     1003     3209 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/transit_preferences.py
+-rw-rw-r--   0 root         (0)     1003     1337 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/units.py
+-rw-rw-r--   0 root         (0)     1003     1609 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/vehicle_emission_type.py
+-rw-rw-r--   0 root         (0)     1003     1502 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/vehicle_info.py
+-rw-rw-r--   0 root         (0)     1003     4688 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/google/maps/routing_v2/types/waypoint.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.020682 google-maps-routing-0.6.1/google_maps_routing.egg-info/
+-rw-r--r--   0 root         (0)     1003     4657 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2346 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       19 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      348 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:57:18.000000 google-maps-routing-0.6.1/google_maps_routing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:57:19.024684 google-maps-routing-0.6.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2965 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.020682 google-maps-routing-0.6.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.020682 google-maps-routing-0.6.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.024684 google-maps-routing-0.6.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:57:19.024684 google-maps-routing-0.6.1/tests/unit/gapic/routing_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/tests/unit/gapic/routing_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73205 2023-07-05 15:46:59.000000 google-maps-routing-0.6.1/tests/unit/gapic/routing_v2/test_routes.py
```

### Comparing `google-maps-routing-0.6.0/LICENSE` & `google-maps-routing-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/MANIFEST.in` & `google-maps-routing-0.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/PKG-INFO` & `google-maps-routing-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-routing
-Version: 0.6.0
+Version: 0.6.1
 Summary: Google Maps Routing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-routing-0.6.0/README.rst` & `google-maps-routing-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing/__init__.py` & `google-maps-routing-0.6.1/google/maps/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing/gapic_version.py` & `google-maps-routing-0.6.1/google/maps/routing/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.0"  # {x-release-please-version}
+__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/__init__.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/gapic_metadata.json` & `google-maps-routing-0.6.1/google/maps/routing_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/gapic_version.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.0"  # {x-release-please-version}
+__version__ = "0.6.1"  # {x-release-please-version}
```

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/__init__.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/__init__.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/async_client.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RoutesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/client.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/client.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/__init__.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/base.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/services/routes/transports/rest.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/services/routes/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/__init__.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/fallback_info.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/fallback_info.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/geocoding_results.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/geocoding_results.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/localized_time.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/localized_time.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/location.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/location.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/maneuver.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/maneuver.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/navigation_instruction.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/navigation_instruction.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/polyline.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/polyline.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/route.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/route.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/route_label.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/route_label.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/route_modifiers.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/route_modifiers.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/route_travel_mode.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/route_travel_mode.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/routes_service.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/routes_service.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/routing_preference.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/routing_preference.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/speed_reading_interval.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/speed_reading_interval.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_info.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/toll_info.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/toll_passes.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/toll_passes.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/traffic_model.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/traffic_model.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/transit.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/transit.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/transit_preferences.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/transit_preferences.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/units.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/units.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_emission_type.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/vehicle_emission_type.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/vehicle_info.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/vehicle_info.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google/maps/routing_v2/types/waypoint.py` & `google-maps-routing-0.6.1/google/maps/routing_v2/types/waypoint.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/google_maps_routing.egg-info/PKG-INFO` & `google-maps-routing-0.6.1/google_maps_routing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-routing
-Version: 0.6.0
+Version: 0.6.1
 Summary: Google Maps Routing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-routing-0.6.0/google_maps_routing.egg-info/SOURCES.txt` & `google-maps-routing-0.6.1/google_maps_routing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/setup.py` & `google-maps-routing-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/tests/__init__.py` & `google-maps-routing-0.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/tests/unit/__init__.py` & `google-maps-routing-0.6.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/tests/unit/gapic/__init__.py` & `google-maps-routing-0.6.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/__init__.py` & `google-maps-routing-0.6.1/tests/unit/gapic/routing_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-routing-0.6.0/tests/unit/gapic/routing_v2/test_routes.py` & `google-maps-routing-0.6.1/tests/unit/gapic/routing_v2/test_routes.py`

 * *Files identical despite different names*

