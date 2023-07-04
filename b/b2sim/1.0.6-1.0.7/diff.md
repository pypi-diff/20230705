# Comparing `tmp/b2sim-1.0.6.tar.gz` & `tmp/b2sim-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.6.tar", last modified: Sun Jul  2 18:50:43 2023, max compression
+gzip compressed data, was "b2sim-1.0.7.tar", last modified: Tue Jul  4 07:53:29 2023, max compression
```

## Comparing `b2sim-1.0.6.tar` & `b2sim-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 18:50:43.673161 b2sim-1.0.6/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.6/LICENSE
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       87 2023-06-20 11:17:51.000000 b2sim-1.0.6/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 18:50:43.672160 b2sim-1.0.6/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    12046 2023-07-02 13:19:26.000000 b2sim-1.0.6/README.md
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 18:50:43.662151 b2sim-1.0.6/b2sim/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       81 2023-06-20 01:13:34.000000 b2sim-1.0.6/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)    10464 2023-07-02 18:23:14.000000 b2sim-1.0.6/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     8687 2023-07-02 18:25:30.000000 b2sim-1.0.6/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)   101854 2023-07-02 18:48:45.000000 b2sim-1.0.6/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     3673 2023-06-21 03:02:53.000000 b2sim-1.0.6/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 18:50:43.671160 b2sim-1.0.6/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.6/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      412 2023-06-19 10:21:44.000000 b2sim-1.0.6/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        0 2023-07-02 18:50:43.668156 b2sim-1.0.6/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      274 2023-07-02 18:50:43.000000 b2sim-1.0.6/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      332 2023-07-02 18:50:43.000000 b2sim-1.0.6/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        1 2023-07-02 18:50:43.000000 b2sim-1.0.6/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       24 2023-07-02 18:50:43.000000 b2sim-1.0.6/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)        6 2023-07-02 18:50:43.000000 b2sim-1.0.6/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)       38 2023-07-02 18:50:43.673161 b2sim-1.0.6/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1001) redlaserbm  (1001)      401 2023-07-02 18:50:38.000000 b2sim-1.0.6/setup.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:21.390490 b2sim-1.0.7/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.7/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.0.7/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-04 23:22:21.384513 b2sim-1.0.7/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    12046 2023-07-02 13:19:26.000000 b2sim-1.0.7/README.md
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:20.872831 b2sim-1.0.7/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.0.7/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10431 2023-07-04 00:29:36.000000 b2sim-1.0.7/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8687 2023-07-04 00:16:01.000000 b2sim-1.0.7/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   102968 2023-07-04 23:16:26.000000 b2sim-1.0.7/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     3818 2023-07-04 23:08:48.000000 b2sim-1.0.7/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:21.329912 b2sim-1.0.7/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.7/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      412 2023-06-19 10:21:44.000000 b2sim-1.0.7/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-04 23:22:21.221090 b2sim-1.0.7/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-04 23:22:20.000000 b2sim-1.0.7/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-04 23:22:19.000000 b2sim-1.0.7/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-04 23:22:21.393490 b2sim-1.0.7/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-04 00:04:31.000000 b2sim-1.0.7/setup.py
```

### Comparing `b2sim-1.0.6/LICENSE` & `b2sim-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.6/README.md` & `b2sim-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.6/b2sim/actions.py` & `b2sim-1.0.7/b2sim/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     return {
         'Type': 'Activate IMF',
         'Index': index,
         'Minimum Buy Time': min_buy_time,
         'Message': 'Take out loan from farm %s'%(index)
     }
 
-#Not yet implemented, don't use
 def sellAllFarms(min_buy_time = 0):
     return {
         'Type': 'Sell All Farms',
         'Minimum Buy Time': min_buy_time #Okay, this might be confusing, but this is actually the minimum *sell* time for this action.
     }
 
 # WARNING: This function is for declaring farms in the initial game state.
```

### Comparing `b2sim-1.0.6/b2sim/info.py` & `b2sim-1.0.7/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.6/b2sim/main.py` & `b2sim-1.0.7/b2sim/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,18 +183,22 @@
         #     'Regrow': regrow,
         #     'Max Eco Amount': max_eco_amount
         # }
 
         # Max send amount is useful if we need to simulate sending a precise number of sets of bloons
         # Max eco amount is useful for eco strategies which may demand strategy decisions like "stop eco at 3000 eco"
 
-        self.changeEcoSend(initial_state.get('Eco Send'))
-
         self.eco_queue = initial_state.get('Eco Queue')
+        if self.eco_queue is None:
+            self.eco_queue = []
         self.number_of_sends = 0
+
+        eco_send = initial_state.get('Eco Send')
+        eco_send['Time'] = 0
+        self.eco_queue.insert(0,eco_send)
         
         #Upgrade queue
         self.buy_queue = initial_state.get('Buy Queue')
         self.buy_cost = None
         self.buffer = 0
         self.min_buy_time = None
 
@@ -219,16 +223,14 @@
         #FAIL-SAFES
         #~~~~~~~~~~
         
         if self.farms is None:
             self.farms = {}
         if self.buy_queue is None:
             self.buy_queue = []
-        if self.eco_queue is None:
-            self.eco_queue = []
         if self.loan is None:
             self.loan = 0
         if self.boat_farms is None:
             self.boat_farms = {}
         if self.druid_farms is None:
             self.druid_farms = {}
         if self.heli_farms is None:
@@ -283,14 +285,15 @@
                 line_color = 'r'
 
             if len(message[1]) > 30:
                 thing_to_say = message[1][0:22] + '...'
             else:
                 thing_to_say = message[1]
             
+            thing_to_say = thing_to_say + ' (R' + str(np.round(self.rounds.getRoundFromTime(message[0], get_frac_part = True),1)) + ')'
             ax[0].plot([message[0],message[0]],[cash_min-1, cash_max+1], label = thing_to_say, linestyle = 'dashed', color = line_color)
             ax[1].plot([message[0],message[0]],[eco_min-1, eco_max+1], label = thing_to_say, linestyle = 'dashed', color = line_color)
 
         #~~~~~~~~~~~~~~~~
         #Label the graphs
         #~~~~~~~~~~~~~~~~
 
@@ -298,16 +301,15 @@
         ax[1].set_title("Eco vs Time")
         
         ax[0].set_ylabel("Cash")
         ax[1].set_ylabel("Eco")
         
         ax[0].set_xlabel("Time (seconds)")
         ax[1].set_xlabel("Time (seconds)")
-        
-        ax[0].legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
+
         ax[1].legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
         
         fig.tight_layout()
 
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         #Create a table that displays the revenue made by each farm
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -401,19 +403,20 @@
                             self.logs.append("Warning! Time %s is too late to call %s. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
                             self.eco_queue.pop(0)
                             
                         else:
                             #No, the send is not too late
                             
                             #Is the eco send too early?
+                            self.logs.append("The candidate round is %s"%(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round']))
                             candidate_time = self.rounds.getTimeFromRound(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round'])
                             if self.eco_queue[0]['Time'] < candidate_time:
                                 #Yes, the send is too early
                                 self.logs.append("Warning! Time %s is too early to call %s. Adjusting the queue time to %s"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name'], candidate_time))
-                                self.eco_queue[0] = (candidate_time, self.eco_queue[0]['Send Name'])
+                                self.eco_queue[0]['Time'] = candidate_time
                                 #Is the adjusted time still valid?
                                 if len(self.eco_queue) < 2 or self.eco_queue[0]['Time'] < self.eco_queue[1]['Time']:
                                     #Yes, it's still valid
                                     self.checkProperties()
                                     break_flag = True
                                 else:
                                     #No, it's not valid
@@ -421,22 +424,25 @@
                                     self.eco_queue.pop(0)
                             else:
                                 #No, the send is not too early
                                 self.checkProperties()
                                 break_flag = True
             
             if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] <= self.current_time:
-                self.changeEcoSend(self.eco_queue[0])
-                self.eco_queue.pop(0)
+                self.changeEcoSend()
             else:
                 future_flag = True
         
-    def changeEcoSend(self,send_info):
-        # NOTE: This function does NOT contain safeguards to prevent the player from changing to unavailable eco sends.
-        # Such safeguards are handled by the ecoQueueCorrection method, which is automatically run when simulating game states.
+    def changeEcoSend(self):
+        # Attempt to change to the first send available in the eco queue
+        # This method is triggered either when reaching the specified time for the next send in the eco queue OR when a break condition (such as max_eco_amount) is satisfied for the current send
+        # Note that if this method is called as a consequence of a break condition being satisfied, it is possible that the safeguard for switching to a send before it becomes available could be triggered.
+
+        send_info = self.eco_queue[0]
+        self.eco_queue.pop(0)
 
         # The send info dictionary looks like this:
         # {
         #     'Time': time,
         #     'Send Name': send_name,
         #     'Max Send Amount': max_send_amount,
         #     'Fortified': fortified,
@@ -450,23 +456,28 @@
         if eco_send_keys.count(send_info['Send Name']) == 0:
             self.logs.append("Warning! The name %s does not correspond with an eco send! Switching to the zero send."%(send_info['Send Name']))
             send_info['Send Name'] = 'Zero'
             self.warnings.append(len(self.logs) - 1)
 
         self.current_round = self.rounds.getRoundFromTime(self.current_time)
 
-        # FAIL SAFE: Switch to the zero send instead if the send is not yet available and reinsert the eco send we wanted to change to into the queue
+        # FAIL SAFE: Switch to the zero send instead if the send is not yet available, and reinsert the send we tried to switch to back into the eco queue.
         if self.current_round < eco_send_info[send_info['Send Name']]['Start Round']:
             self.logs.append("Warning! The eco send %s is not available yet! Switching to the zero send for now, we will attempt to use this send later."%(send_info['Send Name']))
             self.warnings.append(len(self.logs) - 1)
             send_info['Time'] = self.rounds.getTimeFromRound(eco_send_info[send_info['Send Name']]['Start Round'])
-            self.eco_queue.insert(0,send_info)
+            self.logs.append("We are about to insert the following send into the eco queue: ")
+            self.logs.append(str(send_info))
+            self.eco_queue.insert(0,copy.deepcopy(send_info))
+            send_info['Send Name'] = 'Zero'
+            self.logs.append("The next item in the eco queue now looks like this: ")
+            self.logs.append(str(self.eco_queue[0]))
         
         # FAIL SAFE: Switch to the zero send if the send is no longer available.
-        # WARNING: If this fail-safe triggers, something is probably wrong with the code.
+        # The only scenario this should trigger is if the initially specified eco send is no good.
         if self.current_round > eco_send_info[send_info['Send Name']]['End Round']:
             self.logs.append("Warning! The eco send %s is no longer available! Switching to the zero send."%(send_info['Send Name']))
             self.logs.append("Warning! The above message occurred during the changeEcoSend method, which means something's probably wrong with the code!")
             self.warnings.append(len(self.logs) - 1)
             self.warnings.append(len(self.logs) - 2)
             send_info['Send Name'] = 'Zero'
 
@@ -552,16 +563,18 @@
         if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] < target_time:
             #Yes, an eco change will occur
             target_time = self.eco_queue[0]['Time']
 
         # FAIL-SAFE: Check whether the current eco send is valid. If it is not, change the eco send to zero.
         if eco_send_info[self.send_name]['End Round'] < self.current_round:
             self.logs.append("Warning! The eco send %s is no longer available! Switching to the zero send."%(self.send_name))
+            self.logs.append("Warning! This message should not have come up during simulation! Please contact redlaserbm with information on what happened.")
             self.warnings.append(len(self.logs) - 1)
-            self.changeEcoSend({'Send Name': 'Zero'})
+            self.eco_queue.insert(0,{'Time': 0, 'Send Name': 'Zero'})
+            target_time = self.eco_queue[0]['Time']
 
         # FAIL-SAFE: Prevent advanceGameState from using an eco send after it becomes unavailable by terminating early in this case.
         if eco_send_info[self.send_name]['End Round'] + 1 <= self.rounds.getRoundFromTime(target_time):
             target_time = self.rounds.getTimeFromRound(eco_send_info[self.send_name]['End Round'] + 1)
             self.logs.append("Warning! The current eco send will not be available after the conclusion of round %s. Adjusting the target time."%(eco_send_info[self.send_name]['End Round']))
 
         # FAIL-SAFE: Only try to update if we are trying to go into the future. Do NOT try to go back in time!
@@ -597,29 +610,29 @@
             #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
             self.updateEco(payout['Time'])
 
             if (self.max_send_amount is not None and self.number_of_sends == self.max_send_amount) or (self.max_eco_amount is not None and self.eco >= self.max_eco_amount):
                 self.logs.append("Reached the limit on eco'ing for this send! Moving to the next send in the queue.")
 
-                if len(self.eco_queue) > 0:
-                    self.eco_queue[0]['Time'] = self.current_time
-                    self.ecoQueueCorrection()
-                else:
-                    #Switch to the zero send
+                #Switch to the zero send
+                if len(self.eco_queue) == 0:
                     self.logs.append("No more sends in the eco queue! Switching to the zero send.")
                     self.eco_queue.append({
                         'Time': self.current_time,
                         'Send Name': 'Zero',
                         'Max Send Amount': None,
                         'Max Eco Amount': None,
                         'Fortified': False,
                         'Camoflauge': False,
                         'Regrow': False
                     })
+                else:
+                    # Adjust the time of the next eco send so that the simulator attempts to change to it at simulation end
+                    self.eco_queue[0]['Time'] = self.current_time
                 
                 # In rare cases, we may break from the eco queue on exactly same time that we are slated to receive a payment
                 # In that rare case, we need to award the payment for that time and check the buy queue to ensure that we do not "skip" over anything essential.
                 if self.current_time < payout['Time']:
                     break
                 else:
                     made_purchase = True
@@ -762,16 +775,15 @@
 
         while self.rounds.round_starts[self.current_round] <= self.current_time:
             self.current_round += 1
         self.current_round -= 1
         
         #Update the eco send, if necessary
         if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] and target_time >= self.eco_queue[0]['Time']:
-            self.changeEcoSend(self.eco_queue[0])
-            self.eco_queue.pop(0)
+            self.changeEcoSend()
         
         #self.logs.append("Advanced game state to round " + str(self.current_round))
         #self.logs.append("The current time is " + str(self.current_time))
         #self.logs.append("The next round starts at time " + str(self.rounds.round_starts[self.current_round+1]))
         #self.logs.append("Our new cash and eco is given by (%s,%s) \n"%(np.round(self.cash,2),np.round(self.eco,2)))
            
     def computePayoutSchedule(self, target_time):
@@ -1062,15 +1074,15 @@
             # Next, try to add an attack to the attack_queue.
             # Can we send an attack?
             if self.cash >= self.eco_cost and len(self.attack_queue) < 6:
                 # Yes, the queue is empty and we have enough cash
                 if len(self.attack_queue) == 0:
                     self.attack_queue.append(self.current_time + self.eco_time)
                 else:
-                    self.attack_queue.append(self.attack_queue[-1] + self.eco_time)
+                    self.attack_queue.append(max(self.attack_queue[-1] + self.eco_time, self.current_time + self.eco_time))
                 self.cash -= self.eco_cost
                 self.eco += self.eco_gain
                 self.logs.append("Sent a set of %s at time %s"%(self.send_name, self.current_time))
                 self.logs.append("Currently, the send queue looks like this: ")
                 self.logs.append(str(self.attack_queue))
 
                 # Did the attack fill up the eco queue?
```

### Comparing `b2sim-1.0.6/b2sim/rounds.py` & `b2sim-1.0.7/b2sim/rounds.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,19 +45,23 @@
                 #print("Changed stall factor to %s"%(stall_factor))
 
             #Determine the round length based on the current stall factor.
             round_len = self.nat_send_lens[i] + (1-stall_factor)*max_antistall_time + stall_factor*max_stall_times[i]
             val += round_len
             self.round_starts.append(val)            
             
-    def getRoundFromTime(self, time):
+    def getRoundFromTime(self, time, get_frac_part = False):
         ind = 0
         while self.round_starts[ind] <= time and ind < 50:
             ind += 1
-        #self.logs.append("Mapped time %s to round %s"%(time,ind-1))
+        
+        if get_frac_part:
+            frac_part = (time - self.round_starts[ind-1])/(self.round_starts[ind] - self.round_starts[ind-1])
+            ind += frac_part
+            
         return ind - 1
     
     def getTimeFromRound(self, round_val):
         frac_part = round_val - np.floor(round_val)
         time = (1-frac_part)*self.round_starts[int(min(np.floor(round_val),50))] + frac_part*self.round_starts[int(min(np.ceil(round_val),50))]
         #self.logs.append("Mapped round %s to time %s"%(round_val,time))
         return time
```

### Comparing `b2sim-1.0.6/b2sim/templates/eco_send_info.csv` & `b2sim-1.0.7/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

