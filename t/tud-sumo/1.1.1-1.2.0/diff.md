# Comparing `tmp/tud_sumo-1.1.1.tar.gz` & `tmp/tud_sumo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-1.1.1.tar", last modified: Fri May 26 14:47:57 2023, max compression
+gzip compressed data, was "tud_sumo-1.2.0.tar", last modified: Wed Jul  5 12:19:47 2023, max compression
```

## Comparing `tud_sumo-1.1.1.tar` & `tud_sumo-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:47:57.433461 tud_sumo-1.1.1/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.1.1/.gitattributes
--rw-r--r--   0 callumevans (50765939) 1653728465       58 2023-05-26 14:42:14.000000 tud_sumo-1.1.1/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.1.1/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     2552 2023-05-26 14:47:57.433336 tud_sumo-1.1.1/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      945 2023-05-26 14:45:46.000000 tud_sumo-1.1.1/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-05-26 14:39:45.000000 tud_sumo-1.1.1/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-05-26 14:47:57.433500 tud_sumo-1.1.1/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.1.1/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:47:57.432304 tud_sumo-1.1.1/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    15851 2023-05-26 14:39:21.000000 tud_sumo-1.1.1/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:47:57.433166 tud_sumo-1.1.1/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     2552 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-05 12:19:47.466483 tud_sumo-1.2.0/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.2.0/.gitattributes
+-rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.2.0/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.2.0/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     2849 2023-07-05 12:19:47.466357 tud_sumo-1.2.0/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465     1242 2023-05-26 14:58:45.000000 tud_sumo-1.2.0/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-07-05 12:17:49.000000 tud_sumo-1.2.0/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-07-05 12:19:47.466525 tud_sumo-1.2.0/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.2.0/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-05 12:19:47.465475 tud_sumo-1.2.0/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    18021 2023-07-05 12:08:53.000000 tud_sumo-1.2.0/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-05 12:19:47.466161 tud_sumo-1.2.0/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     2849 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-07-05 12:19:47.000000 tud_sumo-1.2.0/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-1.1.1/LICENSE` & `tud_sumo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.1.1/PKG-INFO` & `tud_sumo-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud_sumo
-Version: 1.1.1
+Version: 1.2.0
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,7 +56,9 @@
 sim.start("files/_____.sumocfg", gui=True)
 
 sim_data = sim.step_to(end_step=3600)                    # End siulation at step 3600
 sim_data = sim.step_to(n_steps=3600, prev_data=sim_data) # Run for 3600 steps (use prev_data to append)
 
 sim.end()
 ```
+
+`example_data.json` shows the output of the `step_to` function. Limiting the API calls to traci will improve performance, which can be done by using `vTypes` to only collect vehicle data for specific types or by setting `get_individual_vehicles` to False to only collect aggregated vehicle data.
```

### Comparing `tud_sumo-1.1.1/README.md` & `tud_sumo-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 sim.set_phases(phase_dictionary)
 sim.start("files/_____.sumocfg", gui=True)
 
 sim_data = sim.step_to(end_step=3600)                    # End siulation at step 3600
 sim_data = sim.step_to(n_steps=3600, prev_data=sim_data) # Run for 3600 steps (use prev_data to append)
 
 sim.end()
-```
+```
+
+`example_data.json` shows the output of the `step_to` function. Limiting the API calls to traci will improve performance, which can be done by using `vTypes` to only collect vehicle data for specific types or by setting `get_individual_vehicles` to False to only collect aggregated vehicle data.
```

### Comparing `tud_sumo-1.1.1/pyproject.toml` & `tud_sumo-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
-version = "1.1.1"
+version = "1.2.0"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `tud_sumo-1.1.1/tud_sumo/tud_sumo.py` & `tud_sumo-1.2.0/tud_sumo/tud_sumo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 
-import os, sys, traci, json
+import os, sys, traci, json, warnings, math
 from functools import reduce
 from tqdm import tqdm
 from random import randint
+from copy import copy
 import matplotlib.pyplot as plt
-import math
 
 class Simulation:
     def __init__(self, main_junction = None, verbose = False) -> None:
         path_tools = os.path.join(os.environ.get("SUMO_HOME"), 'tools')
 
         if path_tools in sys.path: pass
         else: sys.path.append(path_tools)
 
+        self.running = False
         self.gui = False
         self.verbose = verbose or '-v' in sys.argv
 
         self.junc_phases = None
         self.def_junc = main_junction
 
         self.available_detectors = {}
         self.step_length = 0.5
 
+        self.get_individual_vehicle_data = True
         self.known_vehicles = {}
         self.light_changes = 0
 
     def start(self, config_file = None, net_file = None, route_file = None, add_file = None, cmd_options = None, step_len = None, warnings = False, gui = False) -> None:
         """
         Intialises SUMO simulation.
         :param config_file: Location of '.sumocfg' file (can be given instead of net_file)
@@ -53,37 +55,46 @@
             if cmd_options != None: sumoCMD += cmd_options
         
         if step_len != None: self.step_length = step_len
         sumoCMD += ["--step-length", str(self.step_length)]
         if not warnings or not self.verbose: sumoCMD.append("--no-warnings")
 
         traci.start(sumoCMD)
-        
+        self.running = True
+
         if self.junc_phases != None: self.update_lights()
         self.curr_step = 0
         self.time_val = traci.simulation.getTime()
 
         self.available_detectors = {detector_id: 'multientryexit' for detector_id in list(traci.multientryexit.getIDList())}
         self.available_detectors.update({detector_id: 'inductionloop' for detector_id in list(traci.inductionloop.getIDList())})
     
+    def is_running(self, close=True):
+        if traci.simulation.getMinExpectedNumber() == 0:
+            if close: self.end()
+            print('Ended simulation early: no vehicles remaining.')
+            return False
+        
+        return True
+
     def end(self):
         traci.close()
+        self.running = False
 
-    def step_to(self, end_step = None, n_steps = None, sim_dur = None, n_light_changes = None, detector_list = None, prev_data = None, vTypes = None, get_individual_vehicles = True, cumulative_data = False) -> dict:
+    def step_to(self, end_step = None, n_steps = None, sim_dur = None, n_light_changes = None, detector_list = None, prev_data = None, vTypes = None, cumulative_data = False) -> dict:
         """
         Step through simulation from the current time until end_step, aggregating
         data during this period.
         :param end_step:        End point for stepping through simulation
         :param n_steps:         Perform n steps of the simulation (given instead of end_steps)
         :param sim_dur:         Simulation duration
         :param n_light_changes: Run for n light changes (across all junctions)
         :param detector_list:   List of detector IDs to collect data from (defaults to all)
         :param prev_data:       If given, new data is appended to this dictionary
         :param vTypes:          Vehicle type(s) to collect data of (list of types or string, defaults to all)
-        :param get_individual_vehicles: Collect all individual vehicle data
         :param cumulative_data: Denotes whether to get cumulative veh count and TTS values
         :return dict:           All data collected through the time period, separated by detector
         """
 
         if detector_list == None: detector_list = list(self.available_detectors.keys())
         start_time = self.curr_step
 
@@ -103,35 +114,30 @@
             else:
                 prev_steps = prev_steps.pop()
                 all_data = prev_data
 
         if self.verbose: pbar = tqdm(desc="Running simulation", total=end_step - self.curr_step)
         while self.curr_step < end_step:
 
-            last_step_data, all_v_data = self.step(detector_list, vTypes, get_individual_vehicles)
-            if get_individual_vehicles: all_data["data"]["all_vehicles"].append(all_v_data)
+            last_step_data, all_v_data = self.step(detector_list, vTypes)
+            all_data["data"]["all_vehicles"].append(all_v_data)
 
             if len(all_data["data"]["detector"]) == 0:
                 for detector_id in detector_list:
                     all_data["data"]["detector"][detector_id] = {"type": self.available_detectors[detector_id], "speeds": [], "veh_counts": [], "occupancies": []}
                 all_data["data"]["vehicle"] = {"no_vehicles": [], "tts": [], "delay": []}
 
             for detector_id in last_step_data["detector"].keys():
                 if detector_id not in all_data["data"]["detector"].keys(): raise KeyError("Unrecognised detector ID found: "+detector_id)
                 for data_key, data_val in last_step_data["detector"][detector_id].items():
                     all_data["data"]["detector"][detector_id][data_key].append(data_val)
 
             for data_key, data_val in last_step_data["vehicle"].items():
                 all_data["data"]["vehicle"][data_key].append(data_val)
 
-            if traci.simulation.getMinExpectedNumber() == 0:
-                traci.close()
-                print('Ended simulation early: no vehicles remaining.')
-                break
-
             if self.verbose: pbar.update(1)
 
             if end_step == math.inf and n_light_changes != None:
                 if self.light_changes - init_changes >= n_light_changes: break
 
         if cumulative_data:
             for detector_data in all_data["data"]["detector"].values():
@@ -139,15 +145,15 @@
             all_data["data"]["vehicle"]["no_vehicles"] = get_cumulative_arr(all_data["data"]["vehicle"]["no_vehicles"], prev_steps)
             all_data["data"]["vehicle"]["tts"] = get_cumulative_arr(all_data["data"]["vehicle"]["tts"], prev_steps)
 
         all_data["end"] = self.curr_step
 
         return all_data
 
-    def step(self, detector_list = None, vTypes = None, get_individual_vehicles = True) -> dict:
+    def step(self, detector_list = None, vTypes = None) -> dict:
         """
         Increment simulation by one time step, updating light state.
         :param detector_list: List of detector IDs to collect data from
         :param vTypes:        Vehicle type(s) to collect data of (list of types or string, defaults to all)
         :return dict:         Simulation data
         """
 
@@ -170,23 +176,26 @@
                     update_junc_lights.append(junction_id)
 
             self.update_lights(update_junc_lights)
 
         if detector_list == None: detector_list = list(self.available_detectors.keys())
         for detector_id in detector_list:
             data["detector"][detector_id] = {}
+            if detector_id not in self.available_detectors.keys(): raise KeyError("KeyError: Unknown detector_id '"+detector_id+"'")
             if self.available_detectors[detector_id] == "multientryexit":
                 data["detector"][detector_id]["speeds"] = traci.multientryexit.getLastStepMeanSpeed(detector_id)
                 data["detector"][detector_id]["veh_counts"] = traci.multientryexit.getLastStepVehicleNumber(detector_id)
             elif self.available_detectors[detector_id] == "inductionloop":
                 data["detector"][detector_id]["speeds"] = traci.inductionloop.getLastStepMeanSpeed(detector_id)
                 data["detector"][detector_id]["veh_counts"] = traci.inductionloop.getLastStepVehicleNumber(detector_id)
                 data["detector"][detector_id]["occupancies"] = traci.inductionloop.getLastStepOccupancy(detector_id)
+            else:
+                print("Warning: Unknown detector type '"+self.available_detectors[detector_id]+"'")
 
-        total_v_data, all_v_data = self.get_vehicle_data(types=vTypes, get_individual_data=get_individual_vehicles)
+        total_v_data, all_v_data = self.get_all_vehicle_data(types=vTypes)
         data["vehicle"]["no_vehicles"] = total_v_data["no_vehicles"]
         data["vehicle"]["tts"] = total_v_data["no_vehicles"] * self.step_length
         data["vehicle"]["delay"] = total_v_data["no_waiting"] * self.step_length
 
         self.curr_step += 1
 
         return data, all_v_data
@@ -253,60 +262,106 @@
             self.light_changes += 1
             new_phase = self.junc_phases[junction_id]["phases"][self.junc_phases[junction_id]["curr_phase"]].lower()
             if '-' in new_phase:
                 new_phase = new_phase.split()
                 new_phase = "".join([new_phase[i] if new_phase[i] != '-' else curr_setting[i] for i in range(len(new_phase))])
             traci.trafficlight.setRedYellowGreenState(junction_id, new_phase)
 
-    def get_vehicle_data(self, ids = None, types = None, get_individual_data = True) -> dict:
+    def get_last_step_vehicles(self, detector_ids = None) -> dict:
+        """
+        Get the IDs of vehicles that passed over the specified detectors
+        :param detector_ids: detector ID or list of detector IDs (defaults to all)
+        :return dict: Dict containing vehicle IDs for each detector
+        """
+
+        detector_ids = list(self.available_detectors.keys()) if detector_ids == None else detector_ids
+        detector_ids = [detector_ids] if not isinstance(detector_ids, list) else detector_ids
+
+        vehicle_ids = {}
+        for detector_id in detector_ids:
+            
+            if detector_id not in self.available_detectors.keys(): raise KeyError("KeyError: Unknown detector_id '"+detector_id+"'")
+            detector_type = self.available_detectors[detector_id]
+
+            if detector_type == "inductionloop":
+                vehicle_ids[detector_id] = list(traci.inductionloop.getLastStepVehicleIDs(detector_id))
+            elif detector_type == "multientryexit":
+                vehicle_ids[detector_id] = list(traci.multientryexit.getLastStepVehicleIDs(detector_id))
+            else:
+                print("Warning: Unknown detector type '"+detector_type+"'")
+
+        return vehicle_ids
+    
+    def get_vehicle_data(self, vehicle_id, vehicle_type = None):
+        """
+        Get data for specified vehicle, updating known_vehicles dict
+        :param vehicle_id: vehicle ID
+        :param vehicle_type: Vehicle type if known
+        :return dict: Vehicle data dictionary
+        """
+
+        if vehicle_type == None:
+            if "cbikes" in vehicle_id: vehicle_type = "cbikes"
+            elif "bikes" in vehicle_id: vehicle_type = "bikes"
+            else: vehicle_type = "cars"
+
+        speed = traci.vehicle.getSpeed(vehicle_id)
+        lon, lat, alt = traci.vehicle.getPosition3D(vehicle_id)
+
+        if vehicle_id not in self.known_vehicles.keys():
+            self.known_vehicles[vehicle_id] = {"type": vehicle_type,
+                                               "longitude": lon,
+                                               "latitude": lat,
+                                               "speed": speed,
+                                               "length": traci.vehicle.getLength(vehicle_id),
+                                               "heading": traci.vehicle.getAngle(vehicle_id),
+                                               "ts": traci.vehicle.getDeparture(vehicle_id),
+                                               "altitude": alt,
+                                               "last_seen": self.curr_step
+                                              }
+        else:
+            self.known_vehicles[vehicle_id]["speed"] = speed
+            self.known_vehicles[vehicle_id]["longitude"] = lon
+            self.known_vehicles[vehicle_id]["latitude"] = lat
+            self.known_vehicles[vehicle_id]["altitude"] = alt
+            self.known_vehicles[vehicle_id]["last_seen"] = self.curr_step
+
+        vehicle_data = copy(self.known_vehicles[vehicle_id])
+        del vehicle_data['last_seen']
+
+        return vehicle_data
+
+    def get_all_vehicle_data(self, ids = None, types = None, type_from_id = True) -> dict:
         """
         Collects vehicle data from SUMO, by id and/or type (defaults to all vehicles)
         :param ids: IDs of vehicles to fetch
         :param types: Type(s) of vehicles to fetch
-        :param get_individual_data: Denotes whether to get individual speed, location & heading data
         :return dict: Vehicle data by id
         """
         if ids == None: ids = list(traci.vehicle.getIDList())
 
         all_vehicle_data = {}
         total_vehicle_data = {"no_vehicles": 0, "no_waiting": 0}
 
         for vehicle_id in ids:
 
             # Saving known vehicles reduces calls to traci by not
             # fetching already known data
             if vehicle_id in self.known_vehicles.keys(): vehicle_type = self.known_vehicles[vehicle_id]["type"]
             else:
                 vehicle_type = traci.vehicle.getVehicleClass(vehicle_id)
-                self.known_vehicles[vehicle_id] = {"type": vehicle_type}
 
             if types is None or (isinstance(types, list) and vehicle_type in types) or (isinstance(types, str) and vehicle_type == types):
-                speed = traci.vehicle.getSpeed(vehicle_id)
-                lon, lat, alt = traci.vehicle.getPosition3D(vehicle_id)
-
-                if get_individual_data:
 
-                    if vehicle_id in self.known_vehicles.keys() and "length" in self.known_vehicles[vehicle_id].keys():
-                        length = self.known_vehicles[vehicle_id]["length"]
-                    else:
-                        length = traci.vehicle.getLength(vehicle_id)
-                        self.known_vehicles[vehicle_id]["length"] = length
+                if self.get_individual_vehicle_data: vehicle_data = self.get_vehicle_data(vehicle_id, vehicle_type)
                 
-                    all_vehicle_data[vehicle_id] = {"type": vehicle_type,
-                                                "longitude": lon,
-                                                "latitude": lat,
-                                                "speed": speed,
-                                                "length": length,
-                                                "heading": traci.vehicle.getAngle(vehicle_id),
-                                                "ts": traci.vehicle.getDeparture(vehicle_id),
-                                                "altitude": alt
-                                            }
+                all_vehicle_data[vehicle_id] = vehicle_data
                     
                 total_vehicle_data["no_vehicles"] += 1
-                if speed < 0.1: total_vehicle_data["no_waiting"] += 1
+                if vehicle_data["speed"] < 0.1: total_vehicle_data["no_waiting"] += 1
 
         return total_vehicle_data, all_vehicle_data
     
 def get_cumulative_arr(arr, start) -> list:
     for i in range(start, len(arr)):
         arr[i] += arr[i - 1]
     return arr
```

### Comparing `tud_sumo-1.1.1/tud_sumo.egg-info/PKG-INFO` & `tud_sumo-1.2.0/tud_sumo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud-sumo
-Version: 1.1.1
+Version: 1.2.0
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,7 +56,9 @@
 sim.start("files/_____.sumocfg", gui=True)
 
 sim_data = sim.step_to(end_step=3600)                    # End siulation at step 3600
 sim_data = sim.step_to(n_steps=3600, prev_data=sim_data) # Run for 3600 steps (use prev_data to append)
 
 sim.end()
 ```
+
+`example_data.json` shows the output of the `step_to` function. Limiting the API calls to traci will improve performance, which can be done by using `vTypes` to only collect vehicle data for specific types or by setting `get_individual_vehicles` to False to only collect aggregated vehicle data.
```

