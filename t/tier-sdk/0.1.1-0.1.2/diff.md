# Comparing `tmp/tier_sdk-0.1.1.tar.gz` & `tmp/tier_sdk-0.1.2.tar.gz`

## Comparing `tier_sdk-0.1.1.tar` & `tier_sdk-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/.editorconfig
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/.gitattributes
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/py.typed
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/tier.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/tier/types.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/.gitignore
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/README.md
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 tier_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/.editorconfig
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/.gitattributes
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/tier/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/tier/py.typed
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/tier/tier.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/tier/types.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 tier_sdk-0.1.2/PKG-INFO
```

### Comparing `tier_sdk-0.1.1/tier/tier.py` & `tier_sdk-0.1.2/tier/tier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Optional, cast
 
 import requests
 
-from .types import (
-    VehiclesCollection,
-)
+from .types import VehiclesCollection, RootZonesCollection, RootZone, Vehicle
 
 TIMEOUT = 3
 API_BASE_URI = "https://platform.tier-services.io"
 
 
 class TIERException(RuntimeError):
     """Unknown error"""
@@ -25,14 +23,15 @@
 class TIER:
     def __init__(self, api_token: str, base_uri: str = API_BASE_URI) -> None:
         self.api_token: str = api_token
         self.base_uri: str = base_uri
         self.headers: dict = {"X-API-Key": self.api_token}
 
         self.vehicles: Vehicles = Vehicles(self)
+        self.zones: Zones = Zones(self)
 
     def get(self, url: str):
         return self.__request("GET", url)
 
     def post(self, url: str, data: Optional[dict] = None):
         if data is None:
             data = {}
@@ -76,7 +75,33 @@
             ),
         )
 
     def in_zone(self, zone_id: str) -> VehiclesCollection:
         return cast(
             VehiclesCollection, self.client.get(f"/v2/vehicle?zoneId={zone_id}")
         )
+
+    def get(self, identifier: str) -> Vehicle:
+        return cast(
+            Vehicle, self.client.get(f"/v1/vehicle/{identifier}").get("data")[0]
+        )
+
+
+class Zones:
+    def __init__(self, client: TIER):
+        self.client = client
+
+    def all(self) -> RootZonesCollection:
+        return cast(RootZonesCollection, self.client.get(f"/v2/zone/root").get("data"))
+
+    def get(self, identifier: str) -> RootZone:
+        return cast(
+            RootZone, self.client.get(f"/v2/zone/root/{identifier}").get("data")
+        )
+
+    def near(self, latitude: float, longitude: float) -> RootZonesCollection:
+        return cast(
+            RootZonesCollection,
+            self.client.get(f"/v2/zone/root?lat={latitude}&lng={longitude}").get(
+                "data"
+            ),
+        )
```

### Comparing `tier_sdk-0.1.1/LICENSE.md` & `tier_sdk-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tier_sdk-0.1.1/README.md` & `tier_sdk-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -21,18 +21,22 @@
 from tier import TIER
 
 tier = TIER(api_token="your-token")
 
 sites = tier.vehicles.in_radius(52.548977, 13.437837, 500)
 ```
 
-| Available Methods                                      | Description                                                                             |
-|:-------------------------------------------------------|:----------------------------------------------------------------------------------------|
-| `tier.vehicles.in_radius(latitude, longitude, radius)` | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius. |
-| `tier.vehicles.in_zone(zone_id)`                       | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius. |
+| Available Methods                                      | Description                                                                                         |
+|:-------------------------------------------------------|:----------------------------------------------------------------------------------------------------|
+| `tier.vehicles.in_radius(latitude, longitude, radius)` | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius.             |
+| `tier.vehicles.in_zone(zone_id)`                       | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius.             |
+| `tier.vehicles.get(vehicle_id)`                        | Retrieve a `Vehicle` dict with details about a specific vehicle.                                    |
+| `tier.zones.all()`                                     | Retrieve a `RootZonesCollection` dict with details about all zones.                                 |
+| `tier.zones.near(latitude, longitude)`                 | Retrieve a `RootZonesCollection` dict with details about zones within 50km of a set of coordinates. |
+| `tier.zones.get(zone_id)`                              | Retrieve a `RootZone` dict with details about a specific zone.                                      |
 
 ## Change log
 
 Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.
 
 ## Testing
```

### Comparing `tier_sdk-0.1.1/pyproject.toml` & `tier_sdk-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
+requires = ["hatchling>=1.18.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tier-sdk"
 dynamic = ["version"]
 readme = "README.md"
 license = "MIT"
```

### Comparing `tier_sdk-0.1.1/PKG-INFO` & `tier_sdk-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tier-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: TIER Python SDK
 Project-URL: Source Code, https://github.com/owenvoke/tier-python-sdk
 Project-URL: Issues, https://github.com/owenvoke/tier-python-sdk/issues
 Author-email: Owen Voke <development@voke.dev>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: sdk,tier
@@ -38,18 +38,22 @@
 from tier import TIER
 
 tier = TIER(api_token="your-token")
 
 sites = tier.vehicles.in_radius(52.548977, 13.437837, 500)
 ```
 
-| Available Methods                                      | Description                                                                             |
-|:-------------------------------------------------------|:----------------------------------------------------------------------------------------|
-| `tier.vehicles.in_radius(latitude, longitude, radius)` | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius. |
-| `tier.vehicles.in_zone(zone_id)`                       | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius. |
+| Available Methods                                      | Description                                                                                         |
+|:-------------------------------------------------------|:----------------------------------------------------------------------------------------------------|
+| `tier.vehicles.in_radius(latitude, longitude, radius)` | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius.             |
+| `tier.vehicles.in_zone(zone_id)`                       | Retrieve a `VehiclesCollection` dict with details about vehicles for a specific radius.             |
+| `tier.vehicles.get(vehicle_id)`                        | Retrieve a `Vehicle` dict with details about a specific vehicle.                                    |
+| `tier.zones.all()`                                     | Retrieve a `RootZonesCollection` dict with details about all zones.                                 |
+| `tier.zones.near(latitude, longitude)`                 | Retrieve a `RootZonesCollection` dict with details about zones within 50km of a set of coordinates. |
+| `tier.zones.get(zone_id)`                              | Retrieve a `RootZone` dict with details about a specific zone.                                      |
 
 ## Change log
 
 Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.
 
 ## Testing
```

