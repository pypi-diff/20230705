# Comparing `tmp/pokers-0.1.0.tar.gz` & `tmp/pokers-0.1.1.tar.gz`

## Comparing `pokers-0.1.0.tar` & `pokers-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 pokers-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     4507 2023-07-04 15:04:20.000000 pokers-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      696 2023-07-04 15:04:20.000000 pokers-0.1.0/.gitignore
--rw-r--r--   0     1001      123     3732 2023-07-04 15:04:20.000000 pokers-0.1.0/README.md
--rw-r--r--   0     1001      123      985 2023-07-04 15:04:20.000000 pokers-0.1.0/play.py
--rw-r--r--   0     1001      123     2570 2023-07-04 15:04:20.000000 pokers-0.1.0/pokers.pyi
--rw-r--r--   0     1001      123     1185 2023-07-04 15:04:20.000000 pokers-0.1.0/proptest-regressions/game_logic.txt
--rw-r--r--   0     1001      123      588 2023-07-04 15:04:20.000000 pokers-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123    19542 2023-07-04 15:04:20.000000 pokers-0.1.0/src/game_logic.rs
--rw-r--r--   0     1001      123      839 2023-07-04 15:04:20.000000 pokers-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123      321 2023-07-04 15:04:20.000000 pokers-0.1.0/src/parallel.rs
--rw-r--r--   0     1001      123     1056 2023-07-04 15:04:20.000000 pokers-0.1.0/src/state/action.rs
--rw-r--r--   0     1001      123     2905 2023-07-04 15:04:20.000000 pokers-0.1.0/src/state/card.rs
--rw-r--r--   0     1001      123      290 2023-07-04 15:04:20.000000 pokers-0.1.0/src/state/stage.rs
--rw-r--r--   0     1001      123     1677 2023-07-04 15:04:20.000000 pokers-0.1.0/src/state.rs
--rw-r--r--   0     1001      123     2279 2023-07-04 15:04:20.000000 pokers-0.1.0/src/visualization.rs
--rw-r--r--   0     1001      123 13997102 2023-07-04 15:04:20.000000 pokers-0.1.0/tests/test_files/pluribus_logs.json
--rw-r--r--   0     1001      123     3947 2023-07-04 15:04:20.000000 pokers-0.1.0/tests/test_game_logic.py
--rw-r--r--   0     1001      123     3176 2023-07-04 15:04:20.000000 pokers-0.1.0/tests/test_parallel.py
--rw-r--r--   0     1001      123    19142 2023-07-04 15:04:27.000000 pokers-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 pokers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 pokers-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     4507 2023-07-05 08:20:52.000000 pokers-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      696 2023-07-05 08:20:52.000000 pokers-0.1.1/.gitignore
+-rw-r--r--   0     1001      123     3688 2023-07-05 08:20:52.000000 pokers-0.1.1/README.md
+-rw-r--r--   0     1001      123      985 2023-07-05 08:20:52.000000 pokers-0.1.1/play.py
+-rw-r--r--   0     1001      123     2570 2023-07-05 08:20:52.000000 pokers-0.1.1/pokers.pyi
+-rw-r--r--   0     1001      123     1705 2023-07-05 08:20:52.000000 pokers-0.1.1/proptest-regressions/game_logic.txt
+-rw-r--r--   0     1001      123      588 2023-07-05 08:20:52.000000 pokers-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123    19458 2023-07-05 08:20:52.000000 pokers-0.1.1/src/game_logic.rs
+-rw-r--r--   0     1001      123      839 2023-07-05 08:20:52.000000 pokers-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123      321 2023-07-05 08:20:52.000000 pokers-0.1.1/src/parallel.rs
+-rw-r--r--   0     1001      123     1056 2023-07-05 08:20:52.000000 pokers-0.1.1/src/state/action.rs
+-rw-r--r--   0     1001      123     2905 2023-07-05 08:20:52.000000 pokers-0.1.1/src/state/card.rs
+-rw-r--r--   0     1001      123      290 2023-07-05 08:20:52.000000 pokers-0.1.1/src/state/stage.rs
+-rw-r--r--   0     1001      123     1665 2023-07-05 08:20:52.000000 pokers-0.1.1/src/state.rs
+-rw-r--r--   0     1001      123     2279 2023-07-05 08:20:52.000000 pokers-0.1.1/src/visualization.rs
+-rw-r--r--   0     1001      123 13996575 2023-07-05 08:20:52.000000 pokers-0.1.1/tests/test_files/pluribus_logs.json
+-rw-r--r--   0     1001      123     3800 2023-07-05 08:20:52.000000 pokers-0.1.1/tests/test_game_logic.py
+-rw-r--r--   0     1001      123     3176 2023-07-05 08:20:52.000000 pokers-0.1.1/tests/test_parallel.py
+-rw-r--r--   0     1001      123    19142 2023-07-05 08:20:58.000000 pokers-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     4295 1970-01-01 00:00:00.000000 pokers-0.1.1/PKG-INFO
```

### Comparing `pokers-0.1.0/.github/workflows/CI.yml` & `pokers-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/.gitignore` & `pokers-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/README.md` & `pokers-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 As a bonus you can print the entire hand as text. Who wants GUIs anyway?
 ```python
 print(pkrs.visualize_trace(trace))
 ```
 
 ### Error handling
 
-There are three possible types of erroneous states: when an illegal action is performed, when a player bets less than the minimum and when a player bets more chips than he has. These cases are represented by the enum `StateStatus` with the values `IllegalAction`, `LowBet` and `HighBet`, the value `Ok` is used for correct states. This information is stored in the field `status` of the state so you can filter them.
+There are two possible types of erroneous states: when an illegal action is performed and when a player bets more chips than he has available. These cases are represented by the enum `StateStatus` with the values `IllegalAction` and `HighBet`, the value `Ok` is used for correct states. This information is stored in the field `status` of the state so you can filter them.
 
 Every erroneous state is also final. So applying an action over it will return the same exact state.
 
 
 ### Parallel actions
 
 If you have a bunch of independent states and want to perform multiple actions in parallel you can easily trick the GIL with `parallel_apply_action()`.
```

### Comparing `pokers-0.1.0/play.py` & `pokers-0.1.1/play.py`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/pokers.pyi` & `pokers-0.1.1/pokers.pyi`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/proptest-regressions/game_logic.txt` & `pokers-0.1.1/proptest-regressions/game_logic.txt`

 * *Files 27% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 #
 # It is recommended to check this file in to source control so that
 # everyone who runs the test benefits from these saved cases.
 cc b3da9bb2183857c7064be605a6dde110806878dafcb262ba3b4b5344ad193ab0 # shrinks to n_players = 0, seed = 0, sb = 0.5, bb_mult = 2, stake_mult = 100, actions = [Action { action: Fold, amount: 0.0 }]
 cc 297734a9898f11b09729690475c86a173c90acfa04d65c15eea85ebbc06f1f49 # shrinks to n_players = 27, seed = 0, sb = 0.5, bb_mult = 2, stake_mult = 100, actions = [Action { action: Fold, amount: -0.0 }]
 cc 61e2819ee09243f5a2b6b642ac81999ebd79511cadcaadbba6830f76ba7d7cef # shrinks to n_players = 4, seed = 0, sb = 0.5, bb_mult = 2, stake_mult = 100, actions = [Action { action: Fold, amount: 0.0 }, Action { action: Call, amount: 0.0 }, Action { action: Fold, amount: 0.0 }]
 cc f09281a07bc71a545a2af2406d90e889b10d1fad1bc1d45dab27496608df0232 # shrinks to n_players = 2, sb = 0.5, bb_mult = 2, stake_mult = 100, actions = [Action { action: Call, amount: 0.0 }, Action { action: Fold, amount: 0.0 }]
+cc c25ff90b9786db4103c019bbcb56cb0123f827fd7129854ea7e3d6da610e0397 # shrinks to n_players = 7, seed = 0, sb = 0.5, bb_mult = 2, stake_mult = 100, actions = [Action { action: Fold, amount: -0.0 }, Action { action: Fold, amount: 0.0 }, Action { action: Raise, amount: -4.086458672170214e67 }, Action { action: Fold, amount: 0.0 }, Action { action: Call, amount: 0.0 }, Action { action: Fold, amount: 0.0 }, Action { action: Call, amount: 0.0 }, Action { action: Fold, amount: 0.0 }, Action { action: Call, amount: 0.0 }]
```

### Comparing `pokers-0.1.0/pyproject.toml` & `pokers-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/src/game_logic.rs` & `pokers-0.1.1/src/game_logic.rs`

 * *Files 3% similar despite different names*

```diff
@@ -159,30 +159,25 @@
                 let raised_chips = self.min_bet - self.players_state[player].bet_chips;
                 new_state.players_state[player].bet_chips += raised_chips;
                 new_state.players_state[player].stake -= raised_chips;
                 new_state.pot += raised_chips;
             }
 
             ActionEnum::Raise => {
-                if action.amount < self.min_bet - self.players_state[player].bet_chips {
-                    return State {
-                        status: StateStatus::LowBet,
-                        final_state: true,
-                        ..self.clone()
-                    };
-                } else if action.amount > self.players_state[player].stake {
+                let bet = (self.min_bet - self.players_state[player].bet_chips) + action.amount;
+                if bet > self.players_state[player].stake {
                     return State {
                         status: StateStatus::HighBet,
                         final_state: true,
                         ..self.clone()
                     };
                 }
-                new_state.players_state[player].bet_chips += action.amount;
-                new_state.players_state[player].stake -= action.amount;
-                new_state.pot += action.amount;
+                new_state.players_state[player].bet_chips += bet;
+                new_state.players_state[player].stake -= bet;
+                new_state.pot += bet;
                 new_state.min_bet = new_state.players_state[player].bet_chips
             }
 
             ActionEnum::Check => (),
         };
 
         new_state.from_action = Some(ActionRecord {
@@ -481,22 +476,24 @@
                 },
                 Err(_) => return Ok(())
             };
 
         }
 
         #[test]
-        fn zero_sum_game(n_players in 2..26, seed: u64, sb in 0.5_f64..100.0_f64, bb_mult in 2..5, stake_mult in 100..1000, actions in prop::collection::vec(Action::arbitrary_with(((), ())), 1..100)) {
+        fn zero_sum_game(n_players in 2..26, seed: u64, sb in 0.5_f64..100.0_f64, bb_mult in 2..5, stake_mult in 100..1000, actions in prop::collection::vec(Action::arbitrary_with(((), ())).prop_filter("Raise abs amount bellow 1e12",
+        |a| a.amount.abs() < 1e12), 1..100)) {
             let initial_state = State::from_seed(n_players as u64, 0, sb, sb * bb_mult as f64, sb * stake_mult as f64, seed);
             match initial_state {
                 Ok(mut s) => {
                     for a in actions {
                         s = s.apply_action(a);
                         if s.final_state {
                             let sum_rewards = s.players_state.iter().map(|ps| ps.reward).fold(0_f64, |r1, r2| r1 + r2);
+                            println!("sum_rewards = {sum_rewards}");
                             prop_assert!(sum_rewards < 1e-12);
                         }
                     }
                 },
                 Err(err) => {
                     println!("{}", err.msg);
                     prop_assert!(false);
```

### Comparing `pokers-0.1.0/src/lib.rs` & `pokers-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/src/state/action.rs` & `pokers-0.1.1/src/state/action.rs`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/src/state/card.rs` & `pokers-0.1.1/src/state/card.rs`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/src/state.rs` & `pokers-0.1.1/src/state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -87,10 +87,9 @@
 
 #[pyclass]
 #[derive(Debug, Clone, Copy)]
 #[cfg_attr(test, derive(Arbitrary))]
 pub enum StateStatus {
     Ok,
     IllegalAction,
-    LowBet,
     HighBet,
 }
```

### Comparing `pokers-0.1.0/src/visualization.rs` & `pokers-0.1.1/src/visualization.rs`

 * *Files identical despite different names*

### Comparing `pokers-0.1.0/tests/test_files/pluribus_logs.json` & `pokers-0.1.1/tests/test_files/pluribus_logs.json`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -196,15 +196,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -317,15 +317,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -430,15 +430,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -537,15 +537,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -613,20 +613,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -695,20 +695,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 681.0
+          "amount": 481.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -837,15 +837,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -955,15 +955,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -1034,28 +1034,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -1123,15 +1123,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -1195,15 +1195,15 @@
       "turn": "5h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -1308,15 +1308,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -1417,15 +1417,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -1497,24 +1497,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -1582,20 +1582,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -1676,15 +1676,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -1784,15 +1784,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -1897,15 +1897,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -1965,15 +1965,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -2048,28 +2048,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -2085,15 +2085,15 @@
           "player": 3,
           "action": "raise",
           "amount": 850.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 8950.0
+          "amount": 8100.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -2157,15 +2157,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -2233,24 +2233,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -2314,29 +2314,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1850.0
+          "amount": 850.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -2403,20 +2403,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -2440,15 +2440,15 @@
           "player": 4,
           "action": "raise",
           "amount": 625.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 3375.0
+          "amount": 2750.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -2521,15 +2521,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -2626,15 +2626,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -2721,15 +2721,15 @@
       "turn": "4d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -2830,15 +2830,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -2898,20 +2898,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 800.0
+          "amount": 590.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -2988,15 +2988,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -3101,15 +3101,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -3200,28 +3200,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -3277,24 +3277,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -3438,15 +3438,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -3717,20 +3717,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -3880,15 +3880,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -3979,15 +3979,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -4013,15 +4013,15 @@
           "player": 5,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1550.0
+          "amount": 1175.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -4156,15 +4156,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -4232,15 +4232,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -4384,15 +4384,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -4420,15 +4420,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1625.0
+          "amount": 1175.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -4527,15 +4527,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -4648,15 +4648,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -4750,15 +4750,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -4826,20 +4826,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -4912,15 +4912,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -5038,37 +5038,37 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 612.0
+          "amount": 402.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1700.0
+          "amount": 1298.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -5143,15 +5143,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -5222,15 +5222,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -5313,34 +5313,34 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 575.0
+          "amount": 325.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1275.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 9750.0
+          "amount": 8150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 1,
@@ -5396,37 +5396,37 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1996.0
+          "amount": 1396.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 5,
@@ -5490,15 +5490,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -5575,15 +5575,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -5704,15 +5704,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -5819,15 +5819,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -6007,28 +6007,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -6118,15 +6118,15 @@
       "river": "5h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -6139,15 +6139,15 @@
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1050.0
         },
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 0,
@@ -6253,15 +6253,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -6355,15 +6355,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -6447,15 +6447,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -6566,15 +6566,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -6730,15 +6730,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -6819,24 +6819,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 950.0
+          "amount": 850.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -7016,15 +7016,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -7203,15 +7203,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -7275,15 +7275,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -7469,15 +7469,15 @@
       "turn": "3h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -7645,15 +7645,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -7713,41 +7713,41 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2025.0
+          "amount": 1550.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -7818,20 +7818,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 400.0
+          "amount": 250.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -7898,20 +7898,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -8176,15 +8176,15 @@
       "turn": "8c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -8362,15 +8362,15 @@
       "river": "9h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -8423,15 +8423,15 @@
           "player": 1,
           "action": "raise",
           "amount": 920.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 6117.0
+          "amount": 5197.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -8496,15 +8496,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -8625,25 +8625,25 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1800.0
+          "amount": 1050.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -8884,15 +8884,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -9035,15 +9035,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -9153,15 +9153,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -9415,15 +9415,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -9525,15 +9525,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -9567,15 +9567,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1012.0
+          "amount": 787.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -9639,29 +9639,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 975.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2420.0
+          "amount": 1620.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -9721,20 +9721,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -9881,15 +9881,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 300.0
+          "amount": 250.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -9949,15 +9949,15 @@
       "turn": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -10271,15 +10271,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -10385,15 +10385,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -10492,15 +10492,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -10598,15 +10598,15 @@
       "river": "8c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -10788,15 +10788,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -10887,15 +10887,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -10967,15 +10967,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -11050,15 +11050,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -11145,15 +11145,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -11214,15 +11214,15 @@
       "river": "Ad"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -11346,15 +11346,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -11459,15 +11459,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -11575,15 +11575,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -11696,15 +11696,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -11744,20 +11744,20 @@
           "player": 0,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 675.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 3525.0
+          "amount": 3050.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -11968,15 +11968,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -12067,15 +12067,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -12162,15 +12162,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -12250,15 +12250,15 @@
       "river": "Ks"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -12375,24 +12375,24 @@
       "river": "Qd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 800.0
+          "amount": 550.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -12401,15 +12401,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 1639.0
+          "amount": 1089.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -12492,15 +12492,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -12651,15 +12651,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -12732,15 +12732,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -12864,15 +12864,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -12966,24 +12966,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 810.0
+          "amount": 649.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -13055,15 +13055,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 350.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -13132,15 +13132,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -13160,15 +13160,15 @@
           "player": 4,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 525.0
+          "amount": 375.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -13258,15 +13258,15 @@
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -13326,37 +13326,37 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 946.0
+          "amount": 721.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2150.0
+          "amount": 1304.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
@@ -13429,15 +13429,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -13559,15 +13559,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -13576,15 +13576,15 @@
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1325.0
+          "amount": 1150.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -13739,15 +13739,15 @@
       "river": "3d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -13872,15 +13872,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -13990,15 +13990,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -14098,15 +14098,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -14194,20 +14194,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -14225,15 +14225,15 @@
           "player": 0,
           "action": "raise",
           "amount": 550.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1575.0
+          "amount": 1025.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -14380,15 +14380,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -14474,15 +14474,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -14566,15 +14566,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -14660,15 +14660,15 @@
       "river": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -14787,15 +14787,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -14878,15 +14878,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -14963,15 +14963,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -15079,24 +15079,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 750.0
+          "amount": 600.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -15214,20 +15214,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -15333,20 +15333,20 @@
       "river": "4h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 681.0
+          "amount": 481.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -15467,24 +15467,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -15517,15 +15517,15 @@
           "player": 0,
           "action": "raise",
           "amount": 2700.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 8700.0
+          "amount": 6000.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -15592,24 +15592,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -15684,15 +15684,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -15773,15 +15773,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -15887,15 +15887,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -15989,15 +15989,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -16096,20 +16096,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -16208,15 +16208,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -16328,15 +16328,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -16510,15 +16510,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -16617,15 +16617,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -16714,24 +16714,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -16799,15 +16799,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -16867,15 +16867,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -16956,15 +16956,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -17164,24 +17164,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 770.0
+          "amount": 570.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -17264,15 +17264,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -17343,24 +17343,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -17423,15 +17423,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -17518,15 +17518,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -17606,20 +17606,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -17808,15 +17808,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -17876,28 +17876,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 725.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -17981,15 +17981,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -18082,15 +18082,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -18179,20 +18179,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -18264,15 +18264,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -18324,15 +18324,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -18408,15 +18408,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -18493,15 +18493,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -18604,15 +18604,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -18719,20 +18719,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -18799,15 +18799,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -18911,15 +18911,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -19013,15 +19013,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -19140,15 +19140,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -19256,15 +19256,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -19349,20 +19349,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -19553,15 +19553,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -19653,15 +19653,15 @@
       "river": "9d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -19768,15 +19768,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -19896,15 +19896,15 @@
           "player": 0,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 670.0
+          "amount": 520.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -19965,15 +19965,15 @@
       "river": "9c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -20214,15 +20214,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -20342,15 +20342,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -20466,15 +20466,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -20558,15 +20558,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -20658,15 +20658,15 @@
       "river": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -20774,15 +20774,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -20850,15 +20850,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -20939,15 +20939,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -21068,15 +21068,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -21151,15 +21151,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -21254,15 +21254,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -21352,15 +21352,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -21420,15 +21420,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -21500,15 +21500,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -21568,15 +21568,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -21715,15 +21715,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -21799,29 +21799,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 770.0
+          "amount": 570.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2175.0
+          "amount": 1505.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -21961,15 +21961,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -22160,15 +22160,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -22269,15 +22269,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -22371,15 +22371,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -22472,15 +22472,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -22580,28 +22580,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -22681,24 +22681,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -22803,37 +22803,37 @@
       "river": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1100.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 5,
@@ -22949,15 +22949,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -23306,15 +23306,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -23390,15 +23390,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -23482,15 +23482,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -23571,29 +23571,29 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 612.0
+          "amount": 412.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1650.0
+          "amount": 1088.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -23665,15 +23665,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -23742,15 +23742,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -23871,15 +23871,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -24004,15 +24004,15 @@
       "river": "8s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -24139,15 +24139,15 @@
       "turn": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -24281,15 +24281,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -24325,15 +24325,15 @@
           "player": 5,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1500.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -24396,15 +24396,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -24499,15 +24499,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 350.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -24568,15 +24568,15 @@
       "river": "5d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -24690,24 +24690,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -24788,15 +24788,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -24822,15 +24822,15 @@
           "player": 5,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 962.0
+          "amount": 712.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -24904,15 +24904,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -24983,15 +24983,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -25085,15 +25085,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -25172,15 +25172,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -25244,15 +25244,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -25261,15 +25261,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 1025.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -25340,15 +25340,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -25545,20 +25545,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 705.0
+          "amount": 505.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -25626,15 +25626,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -25702,33 +25702,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 875.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2150.0
+          "amount": 1275.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -25868,15 +25868,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -25948,15 +25948,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -25998,15 +25998,15 @@
           "player": 3,
           "action": "raise",
           "amount": 675.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 2193.0
+          "amount": 1518.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -26079,15 +26079,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -26107,15 +26107,15 @@
           "player": 4,
           "action": "raise",
           "amount": 111.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 500.0
+          "amount": 389.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -26210,15 +26210,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -26313,15 +26313,15 @@
       "river": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -26436,29 +26436,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2400.0
+          "amount": 1600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -26695,15 +26695,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -26869,15 +26869,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -26956,15 +26956,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -27081,15 +27081,15 @@
           "player": 1,
           "action": "raise",
           "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 400.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -27141,15 +27141,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -27225,15 +27225,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -27312,15 +27312,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -27479,15 +27479,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -27594,15 +27594,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -27744,15 +27744,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -27835,15 +27835,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -27957,15 +27957,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -27988,15 +27988,15 @@
           "player": 1,
           "action": "raise",
           "amount": 900.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 2700.0
+          "amount": 1800.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "river": [
@@ -28147,20 +28147,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 770.0
+          "amount": 570.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -28287,15 +28287,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -28311,15 +28311,15 @@
           "player": 5,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 725.0
+          "amount": 525.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -28382,15 +28382,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -28486,15 +28486,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -28720,15 +28720,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -28941,15 +28941,15 @@
       "river": "4d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -29080,15 +29080,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -29179,15 +29179,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -29264,20 +29264,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -29390,15 +29390,15 @@
       "river": "5c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -29658,20 +29658,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -29739,15 +29739,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 350.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -29811,15 +29811,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -29875,15 +29875,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -29970,15 +29970,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -30074,15 +30074,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -30169,15 +30169,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -30241,15 +30241,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -30332,15 +30332,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -30419,15 +30419,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -30504,15 +30504,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -30741,15 +30741,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -30805,15 +30805,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -30892,15 +30892,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -30982,15 +30982,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -31094,15 +31094,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -31218,15 +31218,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -31351,15 +31351,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -31521,15 +31521,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -31604,15 +31604,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -31702,15 +31702,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -31805,15 +31805,15 @@
       "turn": "8h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -31918,15 +31918,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -32018,15 +32018,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -32136,15 +32136,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -32221,20 +32221,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -32334,15 +32334,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -32474,15 +32474,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -32578,15 +32578,15 @@
       "turn": "4c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -32682,15 +32682,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -32790,24 +32790,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 700.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -32914,15 +32914,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -33033,15 +33033,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -33208,15 +33208,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -33351,15 +33351,15 @@
           "player": 1,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1350.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -33448,20 +33448,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 715.0
+          "amount": 515.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -33533,15 +33533,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -33601,15 +33601,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -33694,15 +33694,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -33922,15 +33922,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -34015,15 +34015,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -34155,15 +34155,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -34329,15 +34329,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -34422,15 +34422,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -34630,15 +34630,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -34705,15 +34705,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -34722,15 +34722,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1075.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 5,
@@ -34953,20 +34953,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -35054,15 +35054,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -35138,15 +35138,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -35214,33 +35214,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 740.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1890.0
+          "amount": 1150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -35311,15 +35311,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -35335,15 +35335,15 @@
           "player": 5,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 547.0
+          "amount": 397.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -35418,15 +35418,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -35497,33 +35497,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 737.0
+          "amount": 487.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2150.0
+          "amount": 1663.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -35701,15 +35701,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -35910,15 +35910,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -36014,41 +36014,41 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 850.0
+          "amount": 640.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2240.0
+          "amount": 1600.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -36113,15 +36113,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -36241,24 +36241,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -36335,24 +36335,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1050.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -36462,15 +36462,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -36640,15 +36640,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -36840,15 +36840,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -36936,15 +36936,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -37038,15 +37038,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -37137,15 +37137,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -37209,15 +37209,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -37478,15 +37478,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -37516,15 +37516,15 @@
           "player": 4,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1312.0
+          "amount": 937.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -37705,15 +37705,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -37932,15 +37932,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -38011,15 +38011,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -38115,15 +38115,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -38261,15 +38261,15 @@
           "player": 1,
           "action": "raise",
           "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 355.0
+          "amount": 255.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -38336,15 +38336,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -38427,15 +38427,15 @@
       "turn": "6d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -38612,15 +38612,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -38700,15 +38700,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -38764,24 +38764,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -38870,15 +38870,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -38907,15 +38907,15 @@
           "player": 0,
           "action": "raise",
           "amount": 400.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2000.0
+          "amount": 1600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -39128,15 +39128,15 @@
           "player": 0,
           "action": "raise",
           "amount": 450.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2375.0
+          "amount": 1925.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -39196,15 +39196,15 @@
       "turn": "3s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -39302,24 +39302,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 750.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -39391,15 +39391,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -39471,15 +39471,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -39548,15 +39548,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -39660,15 +39660,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -39803,15 +39803,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -39895,15 +39895,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -40010,15 +40010,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -40118,15 +40118,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -40198,15 +40198,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -40307,15 +40307,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -40549,15 +40549,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -40659,15 +40659,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -40767,28 +40767,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -40865,24 +40865,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 775.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -40982,15 +40982,15 @@
       "turn": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -41018,15 +41018,15 @@
           "player": 2,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 425.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -41101,15 +41101,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -41190,15 +41190,15 @@
           "player": 1,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1050.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -41426,15 +41426,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -41605,15 +41605,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -41711,15 +41711,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -41941,15 +41941,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -42030,15 +42030,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -42134,15 +42134,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -42210,15 +42210,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -42306,15 +42306,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -42402,15 +42402,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -42434,15 +42434,15 @@
           "player": 3,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 750.0
+          "amount": 600.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -42511,15 +42511,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -42631,20 +42631,20 @@
       "river": "Kh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 818.0
+          "amount": 568.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -42755,24 +42755,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1135.0
+          "amount": 948.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -42832,15 +42832,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -42913,15 +42913,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -43041,24 +43041,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -43149,20 +43149,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 818.0
+          "amount": 568.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -43272,15 +43272,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -43363,15 +43363,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -43456,15 +43456,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -43559,15 +43559,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -43640,20 +43640,20 @@
       "river": "Kc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -43756,20 +43756,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -43837,15 +43837,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -43929,15 +43929,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -44022,15 +44022,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -44094,15 +44094,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -44115,15 +44115,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 825.0
+          "amount": 725.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -44192,15 +44192,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -44375,15 +44375,15 @@
       "turn": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -44472,15 +44472,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -44571,15 +44571,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -44661,15 +44661,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -44748,15 +44748,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -44867,15 +44867,15 @@
           "player": 1,
           "action": "raise",
           "amount": 350.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 700.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -44938,28 +44938,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -45105,24 +45105,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -45257,28 +45257,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -45330,20 +45330,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 805.0
+          "amount": 605.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -45411,15 +45411,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -45500,20 +45500,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -45611,28 +45611,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1090.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -45701,15 +45701,15 @@
       "river": "8s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -45813,20 +45813,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 825.0
+          "amount": 625.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -45939,15 +45939,15 @@
           "player": 1,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 750.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "turn": [
@@ -46037,24 +46037,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -46117,15 +46117,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -46216,15 +46216,15 @@
       "turn": "2c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -46237,15 +46237,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "flop": [
@@ -46326,15 +46326,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -46406,15 +46406,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -46491,15 +46491,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -46599,15 +46599,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -46683,20 +46683,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 963.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -46765,15 +46765,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -46815,15 +46815,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1020.0
+          "amount": 680.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "river": [
@@ -46893,15 +46893,15 @@
       "turn": "Ac"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -47024,15 +47024,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -47058,15 +47058,15 @@
           "player": 5,
           "action": "raise",
           "amount": 125.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1125.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -47224,15 +47224,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -47331,15 +47331,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -47373,15 +47373,15 @@
           "player": 3,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1400.0
+          "amount": 1025.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -47441,28 +47441,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -47712,15 +47712,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -47792,15 +47792,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -47868,15 +47868,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -47941,15 +47941,15 @@
       "river": "6h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -48078,20 +48078,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -48151,20 +48151,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 520.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -48232,15 +48232,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -48304,37 +48304,37 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1875.0
+          "amount": 1400.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -48407,15 +48407,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -48514,15 +48514,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -48621,15 +48621,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -48701,15 +48701,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -48915,20 +48915,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1025.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -49063,15 +49063,15 @@
       "turn": "2h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -49160,15 +49160,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -49261,15 +49261,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -49378,20 +49378,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 244.0
+          "amount": 144.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 956.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -49490,15 +49490,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -49566,15 +49566,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -49646,15 +49646,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -49723,15 +49723,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -49772,15 +49772,15 @@
           "player": 1,
           "action": "raise",
           "amount": 777.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2004.0
+          "amount": 1227.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -49841,15 +49841,15 @@
       "river": "5c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -49952,15 +49952,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -50111,15 +50111,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -50192,28 +50192,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 875.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -50310,15 +50310,15 @@
       "river": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -50438,15 +50438,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -50553,15 +50553,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -50621,15 +50621,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -50772,15 +50772,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -50844,15 +50844,15 @@
       "turn": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -51021,15 +51021,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -51097,15 +51097,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -51182,15 +51182,15 @@
       "river": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -51199,15 +51199,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 775.0
+          "amount": 625.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -51310,15 +51310,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -51342,15 +51342,15 @@
           "player": 3,
           "action": "raise",
           "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 425.0
+          "amount": 290.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -51414,15 +51414,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -51490,24 +51490,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 1050.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -51574,24 +51574,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -51658,15 +51658,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -51675,15 +51675,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -51755,15 +51755,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -51919,15 +51919,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -52003,15 +52003,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -52232,15 +52232,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -52315,15 +52315,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -52406,15 +52406,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -52486,20 +52486,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 775.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -52555,15 +52555,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -52646,15 +52646,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -52674,15 +52674,15 @@
           "player": 4,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 600.0
+          "amount": 450.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -52747,15 +52747,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -52870,15 +52870,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -52961,15 +52961,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -53108,15 +53108,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -53176,15 +53176,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -53252,15 +53252,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -53349,15 +53349,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -53452,15 +53452,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -53545,15 +53545,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -53675,15 +53675,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -53865,15 +53865,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -53948,15 +53948,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -54031,15 +54031,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -54276,15 +54276,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -54397,29 +54397,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2175.0
+          "amount": 1275.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -54515,15 +54515,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -54625,15 +54625,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -54710,15 +54710,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -54824,15 +54824,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -54892,15 +54892,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -55003,15 +55003,15 @@
           "player": 1,
           "action": "raise",
           "amount": 174.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 585.0
+          "amount": 411.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "turn": [
@@ -55081,15 +55081,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -55180,15 +55180,15 @@
       "turn": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -55289,15 +55289,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -55306,15 +55306,15 @@
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1125.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -55374,29 +55374,29 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1900.0
+          "amount": 1200.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -55460,24 +55460,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 720.0
+          "amount": 495.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -55565,15 +55565,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -55747,15 +55747,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -55924,15 +55924,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -56030,15 +56030,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -56111,15 +56111,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -56230,15 +56230,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -56327,15 +56327,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -56494,15 +56494,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -56574,28 +56574,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -56667,20 +56667,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -56744,15 +56744,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -56823,15 +56823,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -56914,15 +56914,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -56991,15 +56991,15 @@
       "river": "3h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -57119,15 +57119,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -57183,15 +57183,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -57408,15 +57408,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -57582,15 +57582,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -57689,15 +57689,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -57757,15 +57757,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -57852,15 +57852,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -57927,15 +57927,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -58014,15 +58014,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -58101,15 +58101,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -58189,15 +58189,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -58335,15 +58335,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -58430,15 +58430,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -58505,15 +58505,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -58691,24 +58691,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 550.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -58847,15 +58847,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -58950,15 +58950,15 @@
       "river": "6d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -59084,15 +59084,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -59112,15 +59112,15 @@
           "player": 4,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 450.0
+          "amount": 300.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -59209,15 +59209,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -59241,15 +59241,15 @@
           "player": 3,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 525.0
+          "amount": 375.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -59309,15 +59309,15 @@
       "turn": "5c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -59406,15 +59406,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -59490,15 +59490,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -59571,28 +59571,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -59679,28 +59679,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 725.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -59773,15 +59773,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -60018,15 +60018,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -60112,15 +60112,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -60215,15 +60215,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -60308,20 +60308,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 780.0
+          "amount": 555.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -60469,15 +60469,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -60549,15 +60549,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -60632,15 +60632,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -60724,15 +60724,15 @@
       "river": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 350.0
+          "amount": 250.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -60782,15 +60782,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2200.0
+          "amount": 1375.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "river": [
@@ -60873,24 +60873,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1123.0
+          "amount": 936.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -61059,15 +61059,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -61152,15 +61152,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -61249,15 +61249,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -61368,15 +61368,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -61447,15 +61447,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -61594,15 +61594,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -61670,15 +61670,15 @@
       "turn": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -61787,15 +61787,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -61905,15 +61905,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -61988,15 +61988,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -62064,15 +62064,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -62247,29 +62247,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1825.0
+          "amount": 1125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -62353,15 +62353,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -62387,15 +62387,15 @@
           "player": 1,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "river": [
@@ -62468,15 +62468,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -62563,15 +62563,15 @@
       "turn": "4h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -62681,15 +62681,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -62766,20 +62766,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -62959,15 +62959,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -63252,15 +63252,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -63348,15 +63348,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -63452,15 +63452,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -63772,15 +63772,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -64074,24 +64074,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 750.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -64196,15 +64196,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -64329,15 +64329,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -64449,15 +64449,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -64565,15 +64565,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -64672,15 +64672,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -64689,15 +64689,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -64847,15 +64847,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -64911,15 +64911,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -64928,15 +64928,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -65000,15 +65000,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -65076,15 +65076,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -65148,15 +65148,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -65307,24 +65307,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 875.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -65413,15 +65413,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -65504,15 +65504,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -65662,28 +65662,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 540.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -65766,15 +65766,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -65880,15 +65880,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -65993,15 +65993,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -66097,15 +66097,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -66211,15 +66211,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -66288,15 +66288,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -66414,15 +66414,15 @@
       "river": "6h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -66431,15 +66431,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 700.0
+          "amount": 525.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -66528,28 +66528,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 440.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -66632,20 +66632,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -66733,15 +66733,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -66843,15 +66843,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -66975,15 +66975,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -67168,15 +67168,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -67274,15 +67274,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -67353,24 +67353,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -67452,15 +67452,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -67535,15 +67535,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -67623,15 +67623,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -67732,15 +67732,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -67854,15 +67854,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -67967,20 +67967,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -68130,15 +68130,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -68230,20 +68230,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 700.0
+          "amount": 528.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -68345,15 +68345,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -68622,15 +68622,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -68639,15 +68639,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 525.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -68712,15 +68712,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -68765,15 +68765,15 @@
           "player": 1,
           "action": "raise",
           "amount": 2120.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 9320.0
+          "amount": 7200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -68832,15 +68832,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -68849,15 +68849,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 840.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -68936,15 +68936,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -69009,15 +69009,15 @@
       "river": "Kh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -69087,15 +69087,15 @@
           "player": 3,
           "action": "raise",
           "amount": 1836.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 9013.0
+          "amount": 7177.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ]
     }
@@ -69163,24 +69163,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "call"
         },
         {
           "player": 4,
@@ -69281,15 +69281,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -69370,24 +69370,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -69455,15 +69455,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -69527,15 +69527,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -69610,15 +69610,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -69726,15 +69726,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -69845,15 +69845,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -69988,15 +69988,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -70064,15 +70064,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -70085,15 +70085,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 1000.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
@@ -70156,15 +70156,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -70345,15 +70345,15 @@
       "river": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -70472,24 +70472,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 700.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "call"
         },
         {
           "player": 4,
@@ -70585,15 +70585,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -70840,20 +70840,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -70964,15 +70964,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -71087,15 +71087,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -71111,15 +71111,15 @@
           "player": 5,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 750.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -71183,15 +71183,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 220.0
+          "amount": 120.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -71306,15 +71306,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -71402,15 +71402,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -71490,15 +71490,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -71633,24 +71633,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 925.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -71714,15 +71714,15 @@
       "turn": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -71819,15 +71819,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 224.0
+          "amount": 124.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -72021,20 +72021,20 @@
       "turn": "4d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -72132,15 +72132,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -72220,15 +72220,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -72542,15 +72542,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -72736,15 +72736,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -72820,15 +72820,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -72926,24 +72926,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -73024,15 +73024,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -73137,15 +73137,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -73261,15 +73261,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -73363,15 +73363,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -73446,15 +73446,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -73545,15 +73545,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -73617,33 +73617,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 875.0
+          "amount": 700.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2200.0
+          "amount": 1500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -73703,15 +73703,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -73922,15 +73922,15 @@
       "river": "5h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -74051,15 +74051,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 208.0
+          "amount": 108.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -74146,15 +74146,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -74223,15 +74223,15 @@
       "river": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -74259,15 +74259,15 @@
           "player": 2,
           "action": "raise",
           "amount": 350.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 960.0
+          "amount": 610.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -74348,24 +74348,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 925.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -74430,15 +74430,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -74549,15 +74549,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -74624,15 +74624,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 208.0
+          "amount": 108.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -74740,15 +74740,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -74913,15 +74913,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -75090,15 +75090,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -75158,15 +75158,15 @@
       "turn": "Kc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -75175,15 +75175,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -75393,15 +75393,15 @@
       "river": "3h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -75516,15 +75516,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -75566,15 +75566,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2375.0
+          "amount": 1850.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -75697,28 +75697,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 850.0
+          "amount": 625.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -75797,15 +75797,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -75889,24 +75889,24 @@
       "river": "Tc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -76005,15 +76005,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -76081,28 +76081,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 975.0
+          "amount": 750.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -76183,15 +76183,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 265.0
+          "amount": 165.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -76289,15 +76289,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -76365,24 +76365,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 775.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -76442,28 +76442,28 @@
       "turn": "4h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -76635,15 +76635,15 @@
       "turn": "7h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -76754,15 +76754,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -76865,15 +76865,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -76944,15 +76944,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -77054,24 +77054,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1100.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -77147,15 +77147,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -77284,24 +77284,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -77375,20 +77375,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 775.0
+          "amount": 525.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -77477,20 +77477,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -77582,15 +77582,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -77599,15 +77599,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -77682,15 +77682,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -77769,15 +77769,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -78027,15 +78027,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -78138,20 +78138,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 510.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -78230,15 +78230,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -78321,15 +78321,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -78404,24 +78404,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -78492,24 +78492,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -78702,20 +78702,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 700.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -78794,15 +78794,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -78976,15 +78976,15 @@
       "river": "Tc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -79103,15 +79103,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -79170,15 +79170,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -79210,15 +79210,15 @@
           "player": 2,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 9775.0
+          "amount": 9475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -79290,15 +79290,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -79459,33 +79459,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 750.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2300.0
+          "amount": 1550.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -79545,33 +79545,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 925.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2250.0
+          "amount": 1325.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -79747,15 +79747,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -79835,15 +79835,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -79904,15 +79904,15 @@
       "river": "7h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -79921,15 +79921,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -80039,15 +80039,15 @@
       "river": "5s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -80167,15 +80167,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -80187,15 +80187,15 @@
           "player": 1,
           "action": "raise",
           "amount": 140.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 870.0
+          "amount": 730.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "turn": [
@@ -80284,20 +80284,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -80306,15 +80306,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1225.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -80400,24 +80400,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 750.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -80477,15 +80477,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -80566,20 +80566,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -80687,15 +80687,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -80794,15 +80794,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -80815,15 +80815,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -80945,15 +80945,15 @@
           "player": 1,
           "action": "raise",
           "amount": 1850.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 9500.0
+          "amount": 7650.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -81114,20 +81114,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 775.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -81195,15 +81195,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -81280,15 +81280,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -81384,15 +81384,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -81477,15 +81477,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -81668,15 +81668,15 @@
       "turn": "8d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -81765,15 +81765,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -81860,15 +81860,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -82070,15 +82070,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -82147,15 +82147,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -82267,24 +82267,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 875.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -82423,15 +82423,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -82525,15 +82525,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -82616,15 +82616,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -82688,15 +82688,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -82848,15 +82848,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -82964,15 +82964,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -83044,15 +83044,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -83129,15 +83129,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -83246,15 +83246,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -83278,15 +83278,15 @@
           "player": 3,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 650.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "turn": [
@@ -83381,15 +83381,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -83484,15 +83484,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -83565,15 +83565,15 @@
       "river": "Ac"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -83618,15 +83618,15 @@
           "player": 2,
           "action": "raise",
           "amount": 460.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 3175.0
+          "amount": 2715.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ]
     }
@@ -83685,15 +83685,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -83797,15 +83797,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -83904,20 +83904,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -83993,20 +83993,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 642.0
+          "amount": 507.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -84074,15 +84074,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -84183,15 +84183,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -84255,15 +84255,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -84344,15 +84344,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -84389,15 +84389,15 @@
           "player": 1,
           "action": "raise",
           "amount": 575.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2050.0
+          "amount": 1475.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -84449,15 +84449,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -84536,15 +84536,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -84839,15 +84839,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -84941,15 +84941,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -85064,15 +85064,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -85174,15 +85174,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -85282,15 +85282,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -85428,15 +85428,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -85528,15 +85528,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -85686,15 +85686,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -85793,15 +85793,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -85891,24 +85891,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -85976,15 +85976,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -86078,15 +86078,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -86189,15 +86189,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -86265,15 +86265,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -86337,15 +86337,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -86524,20 +86524,20 @@
       "river": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 612.0
+          "amount": 412.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -86649,28 +86649,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -86845,20 +86845,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 813.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -86934,15 +86934,15 @@
       "river": "6c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -87071,15 +87071,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -87179,15 +87179,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -87300,15 +87300,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -87416,15 +87416,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -87499,20 +87499,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -87524,15 +87524,15 @@
           "player": 0,
           "action": "raise",
           "amount": 800.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2750.0
+          "amount": 1950.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -87584,15 +87584,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -87673,15 +87673,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -87705,15 +87705,15 @@
           "player": 3,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 675.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "turn": [
@@ -87785,15 +87785,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -87951,15 +87951,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -88030,15 +88030,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -88130,15 +88130,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -88224,15 +88224,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -88256,15 +88256,15 @@
           "player": 3,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 675.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "turn": [
@@ -88354,15 +88354,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -88439,15 +88439,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -88619,15 +88619,15 @@
       "river": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -88640,15 +88640,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "flop": [
@@ -88750,15 +88750,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -88857,15 +88857,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -88929,20 +88929,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -89027,15 +89027,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -89235,15 +89235,15 @@
       "river": "8c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -89362,15 +89362,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -89461,15 +89461,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -89546,15 +89546,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -89580,15 +89580,15 @@
           "player": 5,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1555.0
+          "amount": 1180.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -89660,15 +89660,15 @@
       "river": "Kh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -89713,15 +89713,15 @@
           "player": 2,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 750.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -89790,15 +89790,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -89920,15 +89920,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -90015,20 +90015,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -90107,15 +90107,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -90219,15 +90219,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -90330,20 +90330,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 750.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -90495,15 +90495,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -90602,15 +90602,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -90675,15 +90675,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -90692,15 +90692,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 1000.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -90802,15 +90802,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -90910,15 +90910,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -91027,20 +91027,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 700.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -91193,15 +91193,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -91295,15 +91295,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -91391,15 +91391,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -91506,15 +91506,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -91583,15 +91583,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -91697,15 +91697,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -91773,20 +91773,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -91858,15 +91858,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -91963,15 +91963,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -92027,15 +92027,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -92120,15 +92120,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -92247,15 +92247,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -92320,15 +92320,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -92438,41 +92438,41 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1075.0
+          "amount": 850.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2062.0
+          "amount": 1212.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -92563,15 +92563,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -92658,25 +92658,25 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1050.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -92787,20 +92787,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -93004,15 +93004,15 @@
       "river": "Ac"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -93139,15 +93139,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -93266,15 +93266,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -93352,15 +93352,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -93373,15 +93373,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 1000.0
         },
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 5,
@@ -93461,28 +93461,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -93588,15 +93588,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -93636,15 +93636,15 @@
           "player": 0,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 500.0
+          "amount": 350.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ]
     }
@@ -93708,15 +93708,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -93784,20 +93784,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -93866,15 +93866,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -93969,15 +93969,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -94054,15 +94054,15 @@
       "river": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -94286,15 +94286,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -94394,15 +94394,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -94513,20 +94513,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -94594,15 +94594,15 @@
       "turn": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -94695,15 +94695,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -94767,15 +94767,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -94860,24 +94860,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 725.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "call"
         },
         {
           "player": 4,
@@ -94977,15 +94977,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -95061,15 +95061,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -95093,15 +95093,15 @@
           "player": 3,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 625.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "turn": [
@@ -95176,20 +95176,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -95333,15 +95333,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -95460,15 +95460,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -95572,15 +95572,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -95684,15 +95684,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -95791,28 +95791,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 700.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -95868,15 +95868,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -95949,15 +95949,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -95985,15 +95985,15 @@
           "player": 2,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 712.0
+          "amount": 562.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -96138,15 +96138,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -96222,25 +96222,25 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 2200.0
+          "amount": 1550.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -96387,15 +96387,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -96569,20 +96569,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -96734,15 +96734,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -96768,15 +96768,15 @@
           "player": 5,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1125.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -96843,20 +96843,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -96865,15 +96865,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 2025.0
+          "amount": 1550.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -96925,15 +96925,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -97017,15 +97017,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -97120,15 +97120,15 @@
       "river": "Kh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -97236,15 +97236,15 @@
       "river": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -97373,15 +97373,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -97474,15 +97474,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -97592,20 +97592,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -97669,15 +97669,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -97754,15 +97754,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -97874,24 +97874,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 950.0
+          "amount": 725.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -97915,15 +97915,15 @@
           "player": 5,
           "action": "raise",
           "amount": 1100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2400.0
+          "amount": 1300.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -97987,20 +97987,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 728.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -98069,15 +98069,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -98201,15 +98201,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -98310,15 +98310,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -98389,15 +98389,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -98489,15 +98489,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -98592,15 +98592,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -98675,15 +98675,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -98707,15 +98707,15 @@
           "player": 2,
           "action": "raise",
           "amount": 175.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 525.0
+          "amount": 350.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -98786,15 +98786,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -98877,15 +98877,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -98949,15 +98949,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -99026,15 +99026,15 @@
       "river": "8s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -99159,15 +99159,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -99258,20 +99258,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -99360,15 +99360,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -99394,15 +99394,15 @@
           "player": 5,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 850.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -99619,15 +99619,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -99725,15 +99725,15 @@
       "river": "3s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -99953,15 +99953,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -100044,20 +100044,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 675.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -100121,15 +100121,15 @@
       "turn": "9h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -100153,15 +100153,15 @@
           "player": 2,
           "action": "raise",
           "amount": 450.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 750.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -100173,15 +100173,15 @@
           "player": 3,
           "action": "raise",
           "amount": 750.0
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 3000.0
+          "amount": 2250.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -100249,15 +100249,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -100320,15 +100320,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -100422,15 +100422,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -100529,15 +100529,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -100643,15 +100643,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -100738,15 +100738,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -100889,15 +100889,15 @@
       "turn": "2d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -100987,15 +100987,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -101063,24 +101063,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -101089,15 +101089,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2025.0
+          "amount": 1550.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -101165,15 +101165,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -101245,15 +101245,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -101330,15 +101330,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -101498,15 +101498,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -101522,15 +101522,15 @@
           "player": 5,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "turn": [
@@ -101610,15 +101610,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -101694,15 +101694,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -101774,15 +101774,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -101875,33 +101875,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1850.0
+          "amount": 1350.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -101986,20 +101986,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -102067,24 +102067,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 750.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -102148,15 +102148,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -102229,15 +102229,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -102348,28 +102348,28 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -102444,15 +102444,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -102532,20 +102532,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 728.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -102613,15 +102613,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -102698,15 +102698,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -102881,15 +102881,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -102953,15 +102953,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -103037,15 +103037,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -103099,25 +103099,25 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1400.0
+          "amount": 900.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 2850.0
+          "amount": 1950.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 5700.0
+          "amount": 3750.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -103178,15 +103178,15 @@
       "river": "5h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -103365,15 +103365,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -103437,15 +103437,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -103522,24 +103522,24 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 800.0
+          "amount": 550.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -103651,28 +103651,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -103775,28 +103775,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 950.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -103887,15 +103887,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -103963,15 +103963,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -104107,15 +104107,15 @@
       "river": "6c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -104162,15 +104162,15 @@
           "player": 5,
           "action": "raise",
           "amount": 975.0
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2925.0
+          "amount": 1950.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -104249,15 +104249,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -104320,15 +104320,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -104415,15 +104415,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -104492,15 +104492,15 @@
       "river": "5c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -104528,15 +104528,15 @@
           "player": 2,
           "action": "raise",
           "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 525.0
+          "amount": 390.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -104628,20 +104628,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 700.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -104720,15 +104720,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -104752,15 +104752,15 @@
           "player": 3,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 750.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "turn": [
@@ -104839,20 +104839,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 728.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -104929,15 +104929,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -105031,24 +105031,24 @@
       "turn": "Jd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -105151,15 +105151,15 @@
       "river": "6c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -105172,15 +105172,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1150.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 5,
@@ -105277,24 +105277,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -105497,15 +105497,15 @@
       "river": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -105622,15 +105622,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -105776,15 +105776,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -105852,15 +105852,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -106053,20 +106053,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -106139,15 +106139,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -106242,15 +106242,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -106322,15 +106322,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -106399,15 +106399,15 @@
       "river": "8s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -106521,28 +106521,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1025.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -106626,15 +106626,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -106643,15 +106643,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 900.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -106747,15 +106747,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -106857,15 +106857,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -107059,15 +107059,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -107138,15 +107138,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -107218,20 +107218,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 728.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -107294,15 +107294,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -107408,24 +107408,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 725.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -107500,28 +107500,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1350.0
+          "amount": 1175.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -107593,24 +107593,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 1050.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -107775,15 +107775,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -107854,15 +107854,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -107949,15 +107949,15 @@
       "turn": "7s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -107985,15 +107985,15 @@
           "player": 2,
           "action": "raise",
           "amount": 175.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 675.0
+          "amount": 500.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -108005,15 +108005,15 @@
           "player": 2,
           "action": "raise",
           "amount": 600.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2500.0
+          "amount": 1900.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -108072,15 +108072,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -108358,28 +108358,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -108450,15 +108450,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -108558,15 +108558,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -108662,15 +108662,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -108755,15 +108755,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -108867,15 +108867,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -109019,15 +109019,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -109135,15 +109135,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -109218,20 +109218,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 675.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -109305,15 +109305,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -109404,24 +109404,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 750.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -109485,28 +109485,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1075.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -109571,28 +109571,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -109741,15 +109741,15 @@
           "player": 0,
           "action": "raise",
           "amount": 100.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 500.0
+          "amount": 400.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -109820,15 +109820,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -110031,20 +110031,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 975.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -110121,24 +110121,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -110238,15 +110238,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -110431,15 +110431,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -110521,15 +110521,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -110620,15 +110620,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -110688,15 +110688,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -110769,15 +110769,15 @@
       "river": "4d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -110805,15 +110805,15 @@
           "player": 2,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 675.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -110894,15 +110894,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -111064,15 +111064,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -111151,20 +111151,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 975.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -111258,15 +111258,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 300.0
+          "amount": 250.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -111350,15 +111350,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -111461,15 +111461,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -111576,15 +111576,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -111689,15 +111689,15 @@
       "river": "7h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -111796,15 +111796,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -111880,15 +111880,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -111961,24 +111961,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 400.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -112156,37 +112156,37 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 2200.0
+          "amount": 1100.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -112260,15 +112260,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -112368,15 +112368,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -112488,15 +112488,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -112596,15 +112596,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -112672,15 +112672,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -112752,20 +112752,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1248.0
+          "amount": 1023.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -112900,15 +112900,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -113056,20 +113056,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 400.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -113183,15 +113183,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -113285,15 +113285,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -113368,24 +113368,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 950.0
+          "amount": 825.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -113445,20 +113445,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -113542,15 +113542,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 300.0
+          "amount": 250.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -113741,15 +113741,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -113758,29 +113758,29 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2300.0
+          "amount": 1475.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 8950.0
+          "amount": 7475.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -113857,15 +113857,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -113959,20 +113959,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 700.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -114036,15 +114036,15 @@
       "turn": "2h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -114157,15 +114157,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -114259,15 +114259,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -114359,20 +114359,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -114484,15 +114484,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -114592,29 +114592,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 6200.0
+          "amount": 5200.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -114678,15 +114678,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -114754,15 +114754,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -114951,15 +114951,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -115047,15 +115047,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -115068,15 +115068,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1050.0
         },
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 3,
@@ -115167,15 +115167,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -115486,20 +115486,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -115606,20 +115606,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1248.0
+          "amount": 1023.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -115700,20 +115700,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 650.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -115806,15 +115806,15 @@
       "river": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -116049,15 +116049,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -116164,33 +116164,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 490.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1840.0
+          "amount": 1350.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -116250,15 +116250,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -116339,15 +116339,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -116442,15 +116442,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -116535,15 +116535,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -116714,15 +116714,15 @@
       "river": "5c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -116903,15 +116903,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -116924,15 +116924,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 940.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -116993,15 +116993,15 @@
       "river": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -117054,15 +117054,15 @@
           "player": 2,
           "action": "raise",
           "amount": 750.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 3150.0
+          "amount": 2400.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -117127,15 +117127,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -117313,15 +117313,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -117415,15 +117415,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -117491,15 +117491,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -117584,15 +117584,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -117691,15 +117691,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -117780,15 +117780,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -117903,15 +117903,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -118010,15 +118010,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -118049,15 +118049,15 @@
           "player": 5,
           "action": "raise",
           "amount": 850.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 3075.0
+          "amount": 2225.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -118116,15 +118116,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -118152,15 +118152,15 @@
           "player": 2,
           "action": "raise",
           "amount": 235.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 600.0
+          "amount": 365.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -118224,15 +118224,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -118334,28 +118334,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -118411,15 +118411,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -118565,15 +118565,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -118676,15 +118676,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -118768,15 +118768,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -118879,15 +118879,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -118972,15 +118972,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -118989,15 +118989,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 600.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -119071,15 +119071,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -119229,20 +119229,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 625.0
+          "amount": 420.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -119342,15 +119342,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -119449,15 +119449,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -119530,15 +119530,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -119645,30 +119645,30 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1950.0
+          "amount": 1350.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 9100.0
+          "amount": 7750.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -119737,15 +119737,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -119997,15 +119997,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -120152,15 +120152,15 @@
       "river": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -120267,15 +120267,15 @@
       "river": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -120403,15 +120403,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -120456,15 +120456,15 @@
           "player": 4,
           "action": "raise",
           "amount": 425.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 3410.0
+          "amount": 2985.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ]
     }
@@ -120533,33 +120533,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 775.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2518.0
+          "amount": 1743.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -120649,15 +120649,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -120733,20 +120733,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -120885,15 +120885,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -120998,24 +120998,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -121079,15 +121079,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -121162,15 +121162,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -121252,15 +121252,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -121284,15 +121284,15 @@
           "player": 3,
           "action": "raise",
           "amount": 362.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1811.0
+          "amount": 1449.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -121348,15 +121348,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -121499,15 +121499,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -121578,15 +121578,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -121614,15 +121614,15 @@
           "player": 2,
           "action": "raise",
           "amount": 470.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 630.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -121682,15 +121682,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -121762,15 +121762,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -121864,15 +121864,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -121951,15 +121951,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -122118,15 +122118,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -122247,15 +122247,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -122359,15 +122359,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -122452,15 +122452,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -122630,15 +122630,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -122745,15 +122745,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -122826,20 +122826,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -122889,15 +122889,15 @@
           "player": 5,
           "action": "raise",
           "amount": 5062.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 6700.0
+          "amount": 1638.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -122970,15 +122970,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -123145,15 +123145,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -123234,15 +123234,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -123370,15 +123370,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -123386,15 +123386,15 @@
           "player": 0,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -123458,24 +123458,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -123539,15 +123539,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -123627,15 +123627,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 235.0
+          "amount": 185.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -123734,15 +123734,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -123842,15 +123842,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -123929,15 +123929,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -124028,15 +124028,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -124284,15 +124284,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -124352,15 +124352,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -124439,24 +124439,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 680.0
+          "amount": 520.0
         },
         {
           "player": 1,
           "action": "call"
         },
         {
           "player": 4,
@@ -124535,20 +124535,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -124623,15 +124623,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -124715,15 +124715,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -124904,15 +124904,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -125008,15 +125008,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -125127,15 +125127,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -125226,15 +125226,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -125315,15 +125315,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -125531,15 +125531,15 @@
       "river": "Kc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -125718,15 +125718,15 @@
       "river": "4c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -125861,15 +125861,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -125938,15 +125938,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -125966,15 +125966,15 @@
           "player": 4,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -126056,15 +126056,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -126195,15 +126195,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -126412,20 +126412,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -126493,24 +126493,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 900.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -126566,15 +126566,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -126646,15 +126646,15 @@
       "turn": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -126839,15 +126839,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -126887,15 +126887,15 @@
           "player": 4,
           "action": "raise",
           "amount": 350.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2750.0
+          "amount": 2400.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -127055,24 +127055,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 525.0
+          "amount": 300.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -127147,15 +127147,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -127227,15 +127227,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -127244,15 +127244,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 644.0
+          "amount": 544.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -127386,15 +127386,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -127482,15 +127482,15 @@
       "river": "9d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -127612,15 +127612,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -127695,15 +127695,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -127808,15 +127808,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -127902,24 +127902,24 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -127928,15 +127928,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 1804.0
+          "amount": 1354.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -127944,15 +127944,15 @@
           "player": 2,
           "action": "raise",
           "amount": 1039.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 7996.0
+          "amount": 6957.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -128012,15 +128012,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -128099,15 +128099,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -128261,15 +128261,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -128332,28 +128332,28 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -128428,15 +128428,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -128700,24 +128700,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -128901,15 +128901,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -128980,15 +128980,15 @@
       "turn": "3d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -129102,15 +129102,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -129174,24 +129174,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1125.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -129252,15 +129252,15 @@
       "river": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -129305,20 +129305,20 @@
           "player": 1,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1550.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 4737.0
+          "amount": 3187.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -129378,24 +129378,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -129466,15 +129466,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -129632,15 +129632,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -129758,20 +129758,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -129852,15 +129852,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -129959,15 +129959,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -130066,15 +130066,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -130239,24 +130239,24 @@
       "river": "8s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 637.0
+          "amount": 427.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -130365,20 +130365,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -130453,15 +130453,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -130470,15 +130470,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -130534,15 +130534,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -130734,15 +130734,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -130770,15 +130770,15 @@
           "player": 2,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1312.0
+          "amount": 937.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -130863,15 +130863,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -131109,15 +131109,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -131229,15 +131229,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -131454,15 +131454,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -131554,15 +131554,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -131737,15 +131737,15 @@
       "river": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -131793,15 +131793,15 @@
           "player": 2,
           "action": "raise",
           "amount": 235.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 3300.0
+          "amount": 3065.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -131870,15 +131870,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -131915,15 +131915,15 @@
           "player": 0,
           "action": "raise",
           "amount": 720.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 3040.0
+          "amount": 2320.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -131975,15 +131975,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -131992,15 +131992,15 @@
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1350.0
+          "amount": 1175.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -132085,15 +132085,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -132184,15 +132184,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -132267,15 +132267,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -132383,15 +132383,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -132491,15 +132491,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -132576,15 +132576,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -132697,15 +132697,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -132893,20 +132893,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1255.0
+          "amount": 1030.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -132978,20 +132978,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -133062,15 +133062,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -133149,15 +133149,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -133217,15 +133217,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -133314,15 +133314,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -133435,15 +133435,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -133565,20 +133565,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -133658,15 +133658,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -133765,15 +133765,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -133857,15 +133857,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -133955,15 +133955,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -133972,15 +133972,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 750.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -134075,15 +134075,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -134146,15 +134146,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -134241,15 +134241,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -134330,15 +134330,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -134441,20 +134441,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -134541,15 +134541,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -134630,15 +134630,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -134746,24 +134746,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -134873,15 +134873,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -134985,15 +134985,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -135069,15 +135069,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -135142,15 +135142,15 @@
       "river": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -135203,15 +135203,15 @@
           "player": 2,
           "action": "raise",
           "amount": 675.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 4350.0
+          "amount": 3675.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ]
     }
@@ -135342,15 +135342,15 @@
       "turn": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -135378,15 +135378,15 @@
           "player": 2,
           "action": "raise",
           "amount": 115.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 500.0
+          "amount": 385.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -135474,15 +135474,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -135586,28 +135586,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1175.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -135714,15 +135714,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -135816,15 +135816,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -135872,15 +135872,15 @@
           "player": 4,
           "action": "raise",
           "amount": 680.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1888.0
+          "amount": 1208.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -135936,20 +135936,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -136032,15 +136032,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -136115,15 +136115,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -136203,15 +136203,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -136316,15 +136316,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -136434,15 +136434,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -136536,20 +136536,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 490.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -136720,15 +136720,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -136898,20 +136898,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 950.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -137046,25 +137046,25 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 440.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1800.0
+          "amount": 1200.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -137203,15 +137203,15 @@
       "turn": "7s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -137239,15 +137239,15 @@
           "player": 2,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 425.0
+          "amount": 275.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -137331,15 +137331,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -137450,15 +137450,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -137546,20 +137546,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 490.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -137659,15 +137659,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -137762,15 +137762,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -137905,15 +137905,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -137982,15 +137982,15 @@
       "river": "Th"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -138101,15 +138101,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -138188,15 +138188,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -138346,29 +138346,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2000.0
+          "amount": 1350.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -138440,15 +138440,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -138517,15 +138517,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -138634,15 +138634,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -138849,15 +138849,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -138957,15 +138957,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -139135,15 +139135,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -139222,15 +139222,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -139325,15 +139325,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -139419,24 +139419,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 710.0
+          "amount": 505.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -139513,15 +139513,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -139626,15 +139626,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -139740,15 +139740,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -139842,15 +139842,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -139933,15 +139933,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -140014,15 +140014,15 @@
       "river": "Jd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -140128,15 +140128,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -140204,15 +140204,15 @@
       "turn": "7h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -140309,15 +140309,15 @@
       "turn": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -140436,15 +140436,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -140553,15 +140553,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -140581,15 +140581,15 @@
           "player": 4,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -140662,15 +140662,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -140777,15 +140777,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -140924,28 +140924,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 700.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -141019,15 +141019,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -141108,15 +141108,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -141237,24 +141237,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 725.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -141359,15 +141359,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -141444,15 +141444,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -141679,15 +141679,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -141771,15 +141771,15 @@
       "river": "6c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -141807,15 +141807,15 @@
           "player": 2,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 712.0
+          "amount": 562.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -141892,24 +141892,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -141990,15 +141990,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 350.0
+          "amount": 250.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -142117,15 +142117,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -142206,29 +142206,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2200.0
+          "amount": 1200.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -142284,15 +142284,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -142360,15 +142360,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -142456,15 +142456,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -142480,15 +142480,15 @@
           "player": 5,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "turn": [
@@ -142634,15 +142634,15 @@
       "turn": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -142779,15 +142779,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -142854,15 +142854,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -142938,15 +142938,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -143046,15 +143046,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -143074,15 +143074,15 @@
           "player": 4,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 675.0
+          "amount": 525.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -143150,15 +143150,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -143255,20 +143255,20 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 525.0
+          "amount": 300.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -143359,28 +143359,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 700.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -143441,15 +143441,15 @@
       "river": "7s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -143557,28 +143557,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -143650,20 +143650,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -143724,15 +143724,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -143843,15 +143843,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -144074,15 +144074,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -144187,15 +144187,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -144286,15 +144286,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -144478,15 +144478,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -144566,15 +144566,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -144586,15 +144586,15 @@
           "player": 1,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 500.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "turn": [
@@ -144674,20 +144674,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -144811,15 +144811,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -144991,15 +144991,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -145091,15 +145091,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -145178,15 +145178,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -145250,15 +145250,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -145466,20 +145466,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -145574,15 +145574,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -145659,15 +145659,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -145895,20 +145895,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -146025,15 +146025,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -146097,15 +146097,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -146259,15 +146259,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -146351,15 +146351,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -146467,15 +146467,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -146556,20 +146556,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 725.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -146747,15 +146747,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -146826,15 +146826,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -146921,15 +146921,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -146993,20 +146993,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 728.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -147078,28 +147078,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 750.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 0,
@@ -147199,15 +147199,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -147286,15 +147286,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -147373,15 +147373,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -147548,15 +147548,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -147617,15 +147617,15 @@
       "river": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -147747,15 +147747,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -147827,15 +147827,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -147895,33 +147895,33 @@
       "turn": "2s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1762.0
+          "amount": 1012.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -148014,15 +148014,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -148213,20 +148213,20 @@
       "turn": "4d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 525.0
+          "amount": 300.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -148335,15 +148335,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -148434,15 +148434,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -148675,15 +148675,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 275.0
+          "amount": 225.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -148795,15 +148795,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -148890,28 +148890,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1450.0
+          "amount": 1275.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -149019,15 +149019,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -149104,15 +149104,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -149148,15 +149148,15 @@
           "player": 5,
           "action": "raise",
           "amount": 247.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 741.0
+          "amount": 494.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ]
     }
@@ -149333,15 +149333,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -149533,15 +149533,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -149616,15 +149616,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -149699,20 +149699,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -149776,24 +149776,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -149878,15 +149878,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -149923,15 +149923,15 @@
           "player": 1,
           "action": "raise",
           "amount": 618.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1648.0
+          "amount": 1030.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ]
     }
@@ -149999,20 +149999,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -150118,15 +150118,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -150221,15 +150221,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -150314,15 +150314,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -150429,28 +150429,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 255.0
+          "amount": 155.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1262.0
+          "amount": 1057.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -150538,15 +150538,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -150680,15 +150680,15 @@
           "player": 1,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 525.0
+          "amount": 375.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -150882,15 +150882,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -150973,15 +150973,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -151071,15 +151071,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -151167,24 +151167,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -151286,15 +151286,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -151322,15 +151322,15 @@
           "player": 2,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 875.0
+          "amount": 500.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -151382,15 +151382,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -151604,20 +151604,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 625.0
+          "amount": 425.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -151782,15 +151782,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -151826,15 +151826,15 @@
           "player": 5,
           "action": "raise",
           "amount": 185.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1490.0
+          "amount": 1305.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ]
     }
@@ -151893,15 +151893,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -152071,20 +152071,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 600.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -152157,15 +152157,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -152181,15 +152181,15 @@
           "player": 5,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 750.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "turn": [
@@ -152376,15 +152376,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -152469,15 +152469,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -152580,15 +152580,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -152664,20 +152664,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 600.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -152748,15 +152748,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -152827,15 +152827,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -152911,33 +152911,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 716.0
+          "amount": 501.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1762.0
+          "amount": 1261.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -153005,15 +153005,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -153131,15 +153131,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -153247,15 +153247,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -153358,15 +153358,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -153461,24 +153461,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 875.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -153555,15 +153555,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -153670,15 +153670,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 255.0
+          "amount": 155.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -153788,15 +153788,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -153874,15 +153874,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -154071,15 +154071,15 @@
       "river": "8c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -154194,15 +154194,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -154258,15 +154258,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -154425,29 +154425,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1248.0
+          "amount": 1011.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2238.0
+          "amount": 1227.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -154470,15 +154470,15 @@
           "player": 0,
           "action": "raise",
           "amount": 1925.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 6200.0
+          "amount": 4275.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -154601,15 +154601,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -154697,15 +154697,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -154815,15 +154815,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -154926,15 +154926,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -155020,15 +155020,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -155100,20 +155100,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 625.0
+          "amount": 425.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -155194,15 +155194,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -155323,15 +155323,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -155399,15 +155399,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -155488,15 +155488,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -155584,15 +155584,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -155671,15 +155671,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -155770,15 +155770,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 243.0
+          "amount": 143.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -155913,15 +155913,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -155985,15 +155985,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -156163,15 +156163,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -156266,15 +156266,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -156346,15 +156346,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -156443,15 +156443,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -156560,15 +156560,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -156655,15 +156655,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -156735,15 +156735,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -156824,29 +156824,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 725.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1500.0
+          "amount": 825.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -156943,24 +156943,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 525.0
+          "amount": 300.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -157035,15 +157035,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -157127,15 +157127,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -157187,15 +157187,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -157286,15 +157286,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -157378,24 +157378,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 627.0
+          "amount": 477.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -157481,15 +157481,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -157582,15 +157582,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -157691,15 +157691,15 @@
       "river": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -157826,15 +157826,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -157940,15 +157940,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -158038,25 +158038,25 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 520.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1975.0
+          "amount": 1305.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -158128,15 +158128,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -158238,15 +158238,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -158274,15 +158274,15 @@
           "player": 3,
           "action": "raise",
           "amount": 506.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1650.0
+          "amount": 1144.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -158375,15 +158375,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -158485,15 +158485,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -158521,15 +158521,15 @@
           "player": 2,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1312.0
+          "amount": 937.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -158593,15 +158593,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -158678,20 +158678,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -158788,15 +158788,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -158868,28 +158868,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1075.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -158953,15 +158953,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -159050,15 +159050,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -159148,15 +159148,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -159225,15 +159225,15 @@
       "river": "9d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -159332,15 +159332,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -159416,24 +159416,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 925.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -159572,15 +159572,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -159649,24 +159649,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 612.0
+          "amount": 412.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -159765,15 +159765,15 @@
       "turn": "Td"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -159874,20 +159874,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -159952,15 +159952,15 @@
       "river": "Th"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -160067,15 +160067,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -160276,15 +160276,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -160380,24 +160380,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -160461,15 +160461,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -160660,15 +160660,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -160755,15 +160755,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -160835,15 +160835,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -160999,15 +160999,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -161100,15 +161100,15 @@
       "river": "Jd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -161234,15 +161234,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -161302,33 +161302,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 550.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2130.0
+          "amount": 1580.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -161405,15 +161405,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -161687,24 +161687,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 875.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -161764,15 +161764,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -161840,20 +161840,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -161933,15 +161933,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -162026,15 +162026,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -162113,20 +162113,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1025.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -162205,24 +162205,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 989.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -162287,15 +162287,15 @@
       "river": "6c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -162473,15 +162473,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -162549,20 +162549,20 @@
       "turn": "9s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 720.0
+          "amount": 520.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -162597,15 +162597,15 @@
           "player": 2,
           "action": "raise",
           "amount": 596.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 3278.0
+          "amount": 2682.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -162657,15 +162657,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -162758,15 +162758,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -162950,15 +162950,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -163026,15 +163026,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -163095,15 +163095,15 @@
       "river": "9c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -163293,15 +163293,15 @@
       "river": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -163346,15 +163346,15 @@
           "player": 2,
           "action": "raise",
           "amount": 600.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2280.0
+          "amount": 1680.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -163410,20 +163410,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -163495,24 +163495,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -163592,15 +163592,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -163608,15 +163608,15 @@
           "player": 0,
           "action": "raise",
           "amount": 175.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 625.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "turn": [
@@ -163770,15 +163770,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -163880,15 +163880,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -164024,15 +164024,15 @@
       "river": "Qc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -164140,15 +164140,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -164224,15 +164224,15 @@
       "turn": "Qs"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -164443,15 +164443,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -164532,15 +164532,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -164634,15 +164634,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -164726,15 +164726,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -164866,15 +164866,15 @@
       "river": "8h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -164989,24 +164989,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -165071,15 +165071,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -165186,20 +165186,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -165268,15 +165268,15 @@
       "river": "8s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -165388,15 +165388,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -165409,15 +165409,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 750.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -165473,15 +165473,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -165553,15 +165553,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -165636,15 +165636,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -165874,15 +165874,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -165996,28 +165996,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 890.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -166214,15 +166214,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -166301,24 +166301,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 725.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -166382,15 +166382,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -166625,15 +166625,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -166720,15 +166720,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -166795,24 +166795,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 495.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -166832,15 +166832,15 @@
           "player": 5,
           "action": "raise",
           "amount": 550.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1895.0
+          "amount": 1345.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -166892,15 +166892,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -166987,15 +166987,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 224.0
+          "amount": 124.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -167082,15 +167082,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -167154,15 +167154,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -167231,15 +167231,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -167342,15 +167342,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -167414,15 +167414,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -167494,20 +167494,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -167588,15 +167588,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -167708,20 +167708,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -167789,15 +167789,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -167870,28 +167870,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 900.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -168064,15 +168064,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -168172,15 +168172,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -168256,15 +168256,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -168333,15 +168333,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -168460,15 +168460,15 @@
       "river": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -168587,15 +168587,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -168887,20 +168887,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -168977,15 +168977,15 @@
       "river": "5h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -169088,24 +169088,24 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 612.0
+          "amount": 412.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -169169,15 +169169,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -169335,15 +169335,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -169439,20 +169439,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 725.0
+          "amount": 550.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -169543,15 +169543,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -169628,20 +169628,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -169749,15 +169749,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -169868,15 +169868,15 @@
           "player": 1,
           "action": "raise",
           "amount": 400.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1500.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -169943,15 +169943,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 220.0
+          "amount": 120.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -170109,15 +170109,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -170181,15 +170181,15 @@
       "turn": "Ad"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -170302,15 +170302,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -170401,24 +170401,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -170498,20 +170498,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -170538,15 +170538,15 @@
           "player": 1,
           "action": "raise",
           "amount": 1350.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 7300.0
+          "amount": 5950.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -170610,15 +170610,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -170758,15 +170758,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -170790,15 +170790,15 @@
           "player": 4,
           "action": "raise",
           "amount": 570.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1425.0
+          "amount": 855.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -170891,15 +170891,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -170987,15 +170987,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 350.0
+          "amount": 250.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -171188,15 +171188,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -171282,24 +171282,24 @@
       "river": "9s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -171411,15 +171411,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -171521,15 +171521,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -171597,24 +171597,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -171686,15 +171686,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -171800,15 +171800,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -172022,20 +172022,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 700.0
+          "amount": 528.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -172162,15 +172162,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -172242,15 +172242,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -172329,20 +172329,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -172540,15 +172540,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -172615,15 +172615,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -172735,15 +172735,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -172851,15 +172851,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -173038,15 +173038,15 @@
       "river": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -173104,15 +173104,15 @@
           "player": 2,
           "action": "raise",
           "amount": 2275.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 8675.0
+          "amount": 6400.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -173172,28 +173172,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 863.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -173261,15 +173261,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -173383,15 +173383,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -173485,15 +173485,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -173609,15 +173609,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -173710,15 +173710,15 @@
       "river": "8c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -173763,20 +173763,20 @@
           "player": 2,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 925.0
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 4625.0
+          "amount": 3700.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -173844,15 +173844,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -173950,15 +173950,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -174143,15 +174143,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -174387,15 +174387,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -174477,15 +174477,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -174557,20 +174557,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 600.0
+          "amount": 400.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -174579,15 +174579,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1700.0
+          "amount": 1300.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -174842,24 +174842,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 890.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -175002,15 +175002,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -175070,15 +175070,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -175138,15 +175138,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -175214,15 +175214,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -175294,24 +175294,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 220.0
+          "amount": 120.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -175384,15 +175384,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -175513,15 +175513,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -175629,15 +175629,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -175777,15 +175777,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -175893,15 +175893,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -176140,25 +176140,25 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 2700.0
+          "amount": 1900.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -176254,24 +176254,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 875.0
+          "amount": 700.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -176331,15 +176331,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -176412,15 +176412,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -176527,28 +176527,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -176625,15 +176625,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -176737,15 +176737,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -177133,15 +177133,15 @@
       "river": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -177323,15 +177323,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -177398,24 +177398,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 705.0
+          "amount": 480.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -177494,37 +177494,37 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1950.0
+          "amount": 1475.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -177588,28 +177588,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 208.0
+          "amount": 108.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 742.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -177813,15 +177813,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -177889,15 +177889,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -177972,15 +177972,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 267.0
+          "amount": 167.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -178062,15 +178062,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -178166,15 +178166,15 @@
       "river": "4c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -178286,15 +178286,15 @@
       "river": "6h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -178414,15 +178414,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -178526,15 +178526,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -178695,15 +178695,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -178807,15 +178807,15 @@
       "river": "6c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -178935,15 +178935,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -179011,15 +179011,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -179166,15 +179166,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -179511,15 +179511,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -179626,24 +179626,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1102.0
+          "amount": 952.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -179741,15 +179741,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -179869,15 +179869,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 265.0
+          "amount": 165.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -180035,15 +180035,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -180119,29 +180119,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 875.0
+          "amount": 650.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2409.0
+          "amount": 1634.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -180212,15 +180212,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -180307,24 +180307,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -180384,15 +180384,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -180464,15 +180464,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -180561,15 +180561,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 208.0
+          "amount": 108.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -180646,15 +180646,15 @@
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -180775,15 +180775,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -181027,15 +181027,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -181143,20 +181143,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -181260,15 +181260,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -181380,28 +181380,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 862.0
+          "amount": 687.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -181483,15 +181483,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -181678,15 +181678,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -181766,15 +181766,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -181935,15 +181935,15 @@
       "river": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -182059,15 +182059,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -182146,15 +182146,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -182217,15 +182217,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -182318,15 +182318,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -182421,20 +182421,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -182490,15 +182490,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -182583,15 +182583,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -182787,15 +182787,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -182860,15 +182860,15 @@
       "river": "Qd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -182979,15 +182979,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -183068,15 +183068,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -183176,15 +183176,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -183248,15 +183248,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -183316,15 +183316,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -183404,20 +183404,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -183473,15 +183473,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -183564,29 +183564,29 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2050.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -183665,15 +183665,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -183887,15 +183887,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -183959,24 +183959,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -184039,15 +184039,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -184248,15 +184248,15 @@
       "turn": "Th"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -184349,15 +184349,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -184450,15 +184450,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -184553,15 +184553,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -184570,15 +184570,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 890.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -184649,15 +184649,15 @@
       "turn": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -184758,15 +184758,15 @@
       "turn": "7s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -184794,15 +184794,15 @@
           "player": 2,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 500.0
+          "amount": 300.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "turn": [
@@ -184884,15 +184884,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -184971,15 +184971,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -185066,15 +185066,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -185148,15 +185148,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -185259,15 +185259,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -185371,15 +185371,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -185450,15 +185450,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -185662,15 +185662,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -185760,15 +185760,15 @@
       "river": "Ac"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -185867,15 +185867,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -186067,15 +186067,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -186139,15 +186139,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -186273,15 +186273,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -186387,15 +186387,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -186666,15 +186666,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -186755,15 +186755,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -187015,15 +187015,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -187087,15 +187087,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -187172,20 +187172,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 244.0
+          "amount": 144.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 806.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -187217,15 +187217,15 @@
           "player": 0,
           "action": "raise",
           "amount": 1350.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 4775.0
+          "amount": 3425.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -187525,15 +187525,15 @@
       "river": "6s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -187780,20 +187780,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -187884,15 +187884,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -187983,15 +187983,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -188066,15 +188066,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -188201,15 +188201,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -188277,15 +188277,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -188362,15 +188362,15 @@
       "river": "2d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -188485,24 +188485,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 775.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -188712,15 +188712,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -188825,15 +188825,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -189004,15 +189004,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -189194,20 +189194,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 700.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -189268,15 +189268,15 @@
       "river": "8d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -189517,15 +189517,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -189656,15 +189656,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -189753,15 +189753,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -189833,15 +189833,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -189906,15 +189906,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -190020,24 +190020,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 775.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -190097,15 +190097,15 @@
       "turn": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -190206,15 +190206,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -190378,15 +190378,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -190460,15 +190460,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -190561,15 +190561,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -190677,15 +190677,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -190741,15 +190741,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -190967,20 +190967,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 612.0
+          "amount": 412.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -191004,15 +191004,15 @@
           "player": 4,
           "action": "raise",
           "amount": 687.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 1550.0
+          "amount": 863.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -191020,20 +191020,20 @@
           "player": 3,
           "action": "raise",
           "amount": 100.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2437.0
+          "amount": 2337.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 7738.0
+          "amount": 5401.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -191085,28 +191085,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 520.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -191174,15 +191174,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -191242,15 +191242,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -191326,15 +191326,15 @@
       "turn": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -191566,15 +191566,15 @@
           "player": 1,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1000.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "river": [
@@ -191649,15 +191649,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -191726,15 +191726,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -191849,15 +191849,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -192003,28 +192003,28 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 825.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -192127,15 +192127,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -192247,20 +192247,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 770.0
+          "amount": 570.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -192356,15 +192356,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -192481,24 +192481,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1100.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -192589,15 +192589,15 @@
       "river": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -192709,15 +192709,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -192781,15 +192781,15 @@
       "turn": "2c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -192896,15 +192896,15 @@
       "river": "Td"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -193027,28 +193027,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -193153,15 +193153,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -193267,15 +193267,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -193358,15 +193358,15 @@
       "turn": "Kd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -193472,15 +193472,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -193553,15 +193553,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -193669,15 +193669,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -193753,15 +193753,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -193840,15 +193840,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -193856,15 +193856,15 @@
           "player": 0,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 750.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -193991,15 +193991,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -194063,15 +194063,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -194151,15 +194151,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -194227,15 +194227,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -194300,15 +194300,15 @@
       "river": "Ks"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -194321,15 +194321,15 @@
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 1000.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
@@ -194441,15 +194441,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -194521,15 +194521,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -194632,15 +194632,15 @@
       "river": "5d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -194759,15 +194759,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -194870,15 +194870,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -194918,15 +194918,15 @@
           "player": 4,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ]
     }
@@ -194987,15 +194987,15 @@
       "river": "Tc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -195103,15 +195103,15 @@
       "river": "2d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -195223,15 +195223,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -195347,15 +195347,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -195411,15 +195411,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -195502,15 +195502,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -195590,15 +195590,15 @@
       "river": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -195722,15 +195722,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -195770,15 +195770,15 @@
           "player": 4,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1625.0
+          "amount": 1400.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ]
     }
@@ -195851,15 +195851,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -195893,15 +195893,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1068.0
+          "amount": 843.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "river": [
@@ -195988,15 +195988,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -196081,15 +196081,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -196253,15 +196253,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -196353,15 +196353,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -196415,15 +196415,15 @@
           "player": 3,
           "action": "raise",
           "amount": 2250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 8625.0
+          "amount": 6375.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -196500,15 +196500,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -196601,15 +196601,15 @@
       "river": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -196618,24 +196618,24 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 1937.0
+          "amount": 1287.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -196730,24 +196730,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -196822,15 +196822,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -196922,15 +196922,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -196952,15 +196952,15 @@
           "player": 0,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 575.0
+          "amount": 425.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "river": [
@@ -197142,15 +197142,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -197223,15 +197223,15 @@
       "river": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -197331,15 +197331,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -197416,15 +197416,15 @@
       "river": "7c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -197558,28 +197558,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1337.0
+          "amount": 1162.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -197754,15 +197754,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -197864,20 +197864,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 703.0
+          "amount": 503.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -197962,15 +197962,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 350.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -198137,15 +198137,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -198251,24 +198251,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 869.0
+          "amount": 769.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -198328,20 +198328,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 770.0
+          "amount": 570.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -198401,15 +198401,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -198485,15 +198485,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -198603,15 +198603,15 @@
           "player": 0,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 700.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -198663,15 +198663,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -198758,15 +198758,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -198954,24 +198954,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -199040,15 +199040,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -199155,15 +199155,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -199240,24 +199240,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1100.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -199350,15 +199350,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -199426,15 +199426,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -199502,28 +199502,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1075.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -199595,20 +199595,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 183.0
+          "amount": 133.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 638.0
+          "amount": 505.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -199672,15 +199672,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -199823,15 +199823,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -199861,15 +199861,15 @@
           "player": 4,
           "action": "raise",
           "amount": 375.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1625.0
+          "amount": 1250.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -199925,15 +199925,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -200005,15 +200005,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -200085,15 +200085,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 224.0
+          "amount": 124.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -200149,28 +200149,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -200238,15 +200238,15 @@
       "turn": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -200348,15 +200348,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -200481,15 +200481,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -200589,15 +200589,15 @@
       "river": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -200703,15 +200703,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -200815,20 +200815,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1025.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -200865,15 +200865,15 @@
           "player": 5,
           "action": "raise",
           "amount": 4000.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 8075.0
+          "amount": 4075.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ]
     }
@@ -200933,28 +200933,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 989.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -201119,28 +201119,28 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 520.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -201240,15 +201240,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -201353,15 +201353,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -201437,15 +201437,15 @@
       "river": "5c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -201570,15 +201570,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -201642,15 +201642,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -201710,15 +201710,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -201799,15 +201799,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -201867,15 +201867,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 2125.0
+          "amount": 1700.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ]
     }
@@ -201944,15 +201944,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 362.0
+          "amount": 262.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -201997,15 +201997,15 @@
           "player": 4,
           "action": "raise",
           "amount": 982.0
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2619.0
+          "amount": 1637.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -202082,15 +202082,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -202194,15 +202194,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -202519,15 +202519,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -202752,15 +202752,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -202843,15 +202843,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -202919,15 +202919,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -202991,28 +202991,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -203262,15 +203262,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -203367,15 +203367,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -203475,15 +203475,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -203578,15 +203578,15 @@
       "turn": "Js"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -203688,15 +203688,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -203769,15 +203769,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -203891,15 +203891,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -203982,28 +203982,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 725.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -204068,15 +204068,15 @@
       "river": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -204124,15 +204124,15 @@
           "player": 4,
           "action": "raise",
           "amount": 275.0
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 1650.0
+          "amount": 1375.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -204272,15 +204272,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -204370,15 +204370,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -204466,15 +204466,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -204570,15 +204570,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -204649,15 +204649,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -204729,15 +204729,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -204801,15 +204801,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -204968,15 +204968,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -205057,20 +205057,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -205153,24 +205153,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1230.0
+          "amount": 1105.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -205237,24 +205237,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -205330,20 +205330,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 535.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -205432,15 +205432,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -205521,15 +205521,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -205633,15 +205633,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -205701,15 +205701,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -205793,20 +205793,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 669.0
+          "amount": 534.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -205858,15 +205858,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -205946,15 +205946,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -206052,15 +206052,15 @@
       "river": "7c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -206191,24 +206191,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -206314,15 +206314,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -206454,15 +206454,15 @@
           "player": 1,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1050.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -206541,20 +206541,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 725.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -206606,15 +206606,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -206690,20 +206690,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -206778,15 +206778,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -206865,15 +206865,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -206953,15 +206953,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -207076,24 +207076,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -207198,15 +207198,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -207311,15 +207311,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -207401,38 +207401,38 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2000.0
+          "amount": 1500.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 3750.0
+          "amount": 2250.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -207501,15 +207501,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -207623,20 +207623,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 669.0
+          "amount": 534.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -207730,24 +207730,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -207844,15 +207844,15 @@
       "river": "8h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -207958,28 +207958,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 625.0
+          "amount": 500.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -208119,20 +208119,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -208242,15 +208242,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 224.0
+          "amount": 124.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -208335,15 +208335,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -208422,15 +208422,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -208513,28 +208513,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 625.0
+          "amount": 500.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -208607,15 +208607,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -208722,15 +208722,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -208799,15 +208799,15 @@
       "river": "Kd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -208816,15 +208816,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1075.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -208918,15 +208918,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -209032,15 +209032,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -209052,15 +209052,15 @@
           "player": 1,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -209127,15 +209127,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -209222,20 +209222,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -209316,15 +209316,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -209428,15 +209428,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -209545,15 +209545,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -209656,24 +209656,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 989.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -209746,15 +209746,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -209862,15 +209862,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -209962,15 +209962,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -210062,15 +210062,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -210155,15 +210155,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -210354,15 +210354,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -210462,24 +210462,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 720.0
+          "amount": 495.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -210604,15 +210604,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -210696,15 +210696,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -210793,15 +210793,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -210891,15 +210891,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -210980,15 +210980,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -211109,15 +211109,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -211198,15 +211198,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -211297,15 +211297,15 @@
       "river": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -211411,15 +211411,15 @@
       "turn": "2s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -211527,15 +211527,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -211623,15 +211623,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -211751,28 +211751,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "flop": [
@@ -211866,15 +211866,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -211947,24 +211947,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 224.0
+          "amount": 124.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 975.0
+          "amount": 851.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -212069,15 +212069,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -212177,15 +212177,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -212258,15 +212258,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -212361,15 +212361,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -212378,15 +212378,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 1025.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -212530,15 +212530,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 224.0
+          "amount": 124.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -212632,15 +212632,15 @@
       "turn": "Tc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -212737,20 +212737,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 766.0
+          "amount": 555.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -212825,15 +212825,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -212928,15 +212928,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -213001,15 +213001,15 @@
       "river": "Jd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -213200,15 +213200,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -213268,15 +213268,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 211.0
+          "amount": 111.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -213340,15 +213340,15 @@
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 350.0
+          "amount": 250.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -213433,15 +213433,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -213620,15 +213620,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -213707,15 +213707,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -213794,15 +213794,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -213862,15 +213862,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -213945,28 +213945,28 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 525.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -214112,15 +214112,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -214208,24 +214208,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 875.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -214318,15 +214318,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -214406,15 +214406,15 @@
       "river": "6d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -214452,15 +214452,15 @@
           "player": 2,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1555.0
+          "amount": 1305.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "river": [
@@ -214607,15 +214607,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -214709,15 +214709,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -214797,15 +214797,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -214884,15 +214884,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -214900,15 +214900,15 @@
           "player": 0,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -214969,15 +214969,15 @@
       "river": "7h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -215075,15 +215075,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -215239,15 +215239,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -215277,15 +215277,15 @@
           "player": 0,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1380.0
+          "amount": 1130.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -215483,15 +215483,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -215572,15 +215572,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -215683,15 +215683,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -215790,15 +215790,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -215902,15 +215902,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -216004,15 +216004,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 300.0
+          "amount": 200.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -216097,15 +216097,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -216138,15 +216138,15 @@
           "player": 0,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1800.0
+          "amount": 1500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -216206,15 +216206,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -216289,15 +216289,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -216396,15 +216396,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -216501,15 +216501,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -216580,15 +216580,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -216652,15 +216652,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -216803,15 +216803,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -216946,15 +216946,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -217018,15 +217018,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -217098,15 +217098,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -217190,15 +217190,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -217291,15 +217291,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -217312,15 +217312,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 775.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "flop": [
@@ -217383,15 +217383,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -217475,20 +217475,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 350.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -217556,15 +217556,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -217616,41 +217616,41 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1025.0
+          "amount": 815.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2040.0
+          "amount": 1225.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -217773,15 +217773,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -217862,15 +217862,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -217982,15 +217982,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -218065,15 +218065,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -218153,24 +218153,24 @@
       "river": "2d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 730.0
+          "amount": 520.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -218284,15 +218284,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -218378,15 +218378,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -218477,20 +218477,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 350.0
+          "amount": 300.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -218561,15 +218561,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -218663,15 +218663,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -218746,15 +218746,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -218830,15 +218830,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -218923,20 +218923,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -219028,15 +219028,15 @@
       "river": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -219171,20 +219171,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 780.0
+          "amount": 555.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -219290,15 +219290,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -219406,15 +219406,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -219495,15 +219495,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -219725,20 +219725,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 862.0
+          "amount": 687.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -219811,15 +219811,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -219931,15 +219931,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -219995,15 +219995,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -220012,24 +220012,24 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 925.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2275.0
+          "amount": 1350.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -220106,15 +220106,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -220207,15 +220207,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -220314,15 +220314,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -220395,15 +220395,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -220495,15 +220495,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -220571,20 +220571,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 720.0
+          "amount": 520.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -220660,24 +220660,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 835.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -220745,24 +220745,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -220830,20 +220830,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -220907,15 +220907,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -220992,24 +220992,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -221111,15 +221111,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -221143,15 +221143,15 @@
           "player": 3,
           "action": "raise",
           "amount": 175.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 600.0
+          "amount": 425.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -221211,15 +221211,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -221288,15 +221288,15 @@
       "river": "8c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -221416,15 +221416,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -221530,15 +221530,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -221558,15 +221558,15 @@
           "player": 4,
           "action": "raise",
           "amount": 225.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -221704,15 +221704,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -221788,15 +221788,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -221868,20 +221868,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 660.0
+          "amount": 445.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -221970,15 +221970,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -222137,15 +222137,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -222248,15 +222248,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -222457,15 +222457,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -222537,15 +222537,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -222616,24 +222616,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "flop": [
@@ -222711,15 +222711,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -222739,15 +222739,15 @@
           "player": 4,
           "action": "raise",
           "amount": 175.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 550.0
+          "amount": 375.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -222882,24 +222882,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 975.0
+          "amount": 825.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -222993,15 +222993,15 @@
           "player": 1,
           "action": "raise",
           "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 424.0
+          "amount": 324.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -223069,15 +223069,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -223183,15 +223183,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -223291,24 +223291,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -223373,15 +223373,15 @@
       "river": "Qd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -223496,15 +223496,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -223572,24 +223572,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -223657,15 +223657,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -223736,15 +223736,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -223844,20 +223844,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -223877,15 +223877,15 @@
           "player": 5,
           "action": "raise",
           "amount": 700.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2050.0
+          "amount": 1350.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "turn": [
@@ -223981,15 +223981,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -224005,15 +224005,15 @@
           "player": 5,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 575.0
+          "amount": 425.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -224077,15 +224077,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -224250,15 +224250,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -224367,15 +224367,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -224615,15 +224615,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -224743,15 +224743,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -224846,15 +224846,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -225033,15 +225033,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -225121,15 +225121,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -225198,15 +225198,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -225328,15 +225328,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -225439,20 +225439,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -225528,15 +225528,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -225605,15 +225605,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -225650,15 +225650,15 @@
           "player": 4,
           "action": "raise",
           "amount": 600.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 9475.0
+          "amount": 8875.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -225718,15 +225718,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -225786,15 +225786,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -226008,15 +226008,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -226159,15 +226159,15 @@
       "turn": "7s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -226275,15 +226275,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -226383,15 +226383,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -226497,20 +226497,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 900.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -226589,15 +226589,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -226662,15 +226662,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -226728,15 +226728,15 @@
           "player": 2,
           "action": "raise",
           "amount": 2700.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 8675.0
+          "amount": 5975.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ]
     }
@@ -226799,15 +226799,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -226905,15 +226905,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -226988,15 +226988,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -227060,15 +227060,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -227216,15 +227216,15 @@
       "river": "Td"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -227277,15 +227277,15 @@
           "player": 2,
           "action": "raise",
           "amount": 675.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 4500.0
+          "amount": 3825.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -227345,24 +227345,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1400.0
+          "amount": 1163.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -227431,15 +227431,15 @@
       "river": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -227555,15 +227555,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -227587,15 +227587,15 @@
           "player": 3,
           "action": "raise",
           "amount": 500.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1587.0
+          "amount": 1087.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "turn": [
@@ -227689,15 +227689,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -227770,15 +227770,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -227868,15 +227868,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -228072,15 +228072,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -228089,15 +228089,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1115.0
+          "amount": 990.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 5,
@@ -228172,20 +228172,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 675.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -228264,15 +228264,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -228343,33 +228343,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1050.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2500.0
+          "amount": 1450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -228461,15 +228461,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -228560,15 +228560,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -228657,15 +228657,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -228696,15 +228696,15 @@
           "player": 5,
           "action": "raise",
           "amount": 1100.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2605.0
+          "amount": 1505.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "river": [
@@ -228776,15 +228776,15 @@
       "river": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -228903,15 +228903,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 270.0
+          "amount": 170.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -229089,28 +229089,28 @@
       "turn": "9s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 550.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -229199,28 +229199,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -229288,15 +229288,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -229360,20 +229360,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 675.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -229449,15 +229449,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -229634,15 +229634,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -229883,15 +229883,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -229974,15 +229974,15 @@
       "turn": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -230084,15 +230084,15 @@
       "river": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -230199,20 +230199,20 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 800.0
+          "amount": 550.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -230295,15 +230295,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -230386,15 +230386,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -230461,15 +230461,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -230560,20 +230560,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1255.0
+          "amount": 1030.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -230649,15 +230649,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -230755,15 +230755,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -230865,15 +230865,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -230936,28 +230936,28 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -231184,15 +231184,15 @@
           "player": 1,
           "action": "raise",
           "amount": 175.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -231274,15 +231274,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -231436,24 +231436,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -231513,15 +231513,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -231590,15 +231590,15 @@
       "river": "8d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -231709,15 +231709,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -231784,28 +231784,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 745.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -231817,15 +231817,15 @@
           "player": 0,
           "action": "raise",
           "amount": 1000.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 2725.0
+          "amount": 1725.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -231888,15 +231888,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -232070,15 +232070,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -232173,15 +232173,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -232281,15 +232281,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -232376,15 +232376,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -232455,15 +232455,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -232531,20 +232531,20 @@
       "turn": "Ad"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 725.0
+          "amount": 500.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -232645,24 +232645,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 800.0
+          "amount": 650.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -232797,15 +232797,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -232865,28 +232865,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 775.0
+          "amount": 620.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -232950,15 +232950,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -233111,15 +233111,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -233231,15 +233231,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -233413,15 +233413,15 @@
       "river": "Ks"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -233528,15 +233528,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -233604,15 +233604,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -233680,15 +233680,15 @@
       "turn": "Qs"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -233701,15 +233701,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 875.0
         },
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 5,
@@ -233795,15 +233795,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -233875,15 +233875,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -233959,24 +233959,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -234040,15 +234040,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -234112,15 +234112,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -234209,15 +234209,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -234308,15 +234308,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -234424,15 +234424,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -234521,15 +234521,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -234620,15 +234620,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -234715,15 +234715,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -234798,24 +234798,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -234955,15 +234955,15 @@
       "river": "Jc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -235077,15 +235077,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -235172,15 +235172,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -235249,15 +235249,15 @@
       "river": "Qh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -235377,15 +235377,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -235489,15 +235489,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -235578,15 +235578,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -235685,15 +235685,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 225.0
+          "amount": 175.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -236010,15 +236010,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -236198,15 +236198,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -236299,15 +236299,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -236603,15 +236603,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -236682,15 +236682,15 @@
       "turn": "3s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -236797,15 +236797,15 @@
       "river": "2c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -236849,15 +236849,15 @@
           "player": 2,
           "action": "raise",
           "amount": 350.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1302.0
+          "amount": 952.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ]
     }
@@ -236924,15 +236924,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -237139,15 +237139,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -237224,15 +237224,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -237262,15 +237262,15 @@
           "player": 0,
           "action": "raise",
           "amount": 472.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1540.0
+          "amount": 1068.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -237353,15 +237353,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -237425,20 +237425,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 550.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -237515,24 +237515,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1025.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -237565,15 +237565,15 @@
           "player": 0,
           "action": "raise",
           "amount": 1550.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 6900.0
+          "amount": 5350.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -237645,15 +237645,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -237755,15 +237755,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -237819,15 +237819,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -237898,15 +237898,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -237919,15 +237919,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1400.0
+          "amount": 1300.0
         },
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 5,
@@ -238120,15 +238120,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -238223,15 +238223,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -238308,15 +238308,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -238419,20 +238419,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 490.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -238504,15 +238504,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -238576,15 +238576,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -238655,15 +238655,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -238687,15 +238687,15 @@
           "player": 3,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 800.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -238747,15 +238747,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -238902,15 +238902,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -238990,15 +238990,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -239087,15 +239087,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -239159,15 +239159,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -239351,15 +239351,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -239427,28 +239427,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 950.0
+          "amount": 840.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -239511,24 +239511,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 440.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -239626,15 +239626,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -239718,15 +239718,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -239900,15 +239900,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -239975,15 +239975,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -240083,15 +240083,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -240199,15 +240199,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -240351,15 +240351,15 @@
       "river": "4h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -240474,15 +240474,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -240561,15 +240561,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -240663,15 +240663,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -240763,15 +240763,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -240867,15 +240867,15 @@
       "river": "2s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -240986,20 +240986,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 490.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -241070,15 +241070,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -241165,15 +241165,15 @@
       "turn": "2h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -241461,15 +241461,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -241624,15 +241624,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -241730,28 +241730,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 995.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -241823,20 +241823,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 605.0
+          "amount": 470.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -242006,15 +242006,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -242191,15 +242191,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -242426,15 +242426,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -242545,15 +242545,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -242630,15 +242630,15 @@
       "river": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -242753,15 +242753,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -242834,15 +242834,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -242946,15 +242946,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -243033,15 +243033,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -243116,15 +243116,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -243262,15 +243262,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -243358,15 +243358,15 @@
       "river": "3s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -243402,15 +243402,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 650.0
+          "amount": 350.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "turn": [
@@ -243499,28 +243499,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 1025.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 0,
@@ -243628,15 +243628,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -243804,15 +243804,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -243825,15 +243825,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 850.0
+          "amount": 725.0
         },
         {
           "player": 2,
           "action": "call"
         },
         {
           "player": 5,
@@ -243909,20 +243909,20 @@
       "river": "Th"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -244104,15 +244104,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -244187,15 +244187,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -244215,15 +244215,15 @@
           "player": 4,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 750.0
+          "amount": 500.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -244295,15 +244295,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -244319,15 +244319,15 @@
           "player": 5,
           "action": "raise",
           "amount": 350.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1025.0
+          "amount": 675.0
         },
         {
           "player": 5,
           "action": "call"
         }
       ],
       "turn": [
@@ -244406,25 +244406,25 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 650.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1650.0
+          "amount": 1150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -244559,20 +244559,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 875.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -244636,15 +244636,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -244729,20 +244729,20 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 605.0
+          "amount": 470.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -244987,15 +244987,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -245093,15 +245093,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -245252,15 +245252,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -245351,28 +245351,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -245439,15 +245439,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -245533,15 +245533,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -245637,15 +245637,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -245755,15 +245755,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -245926,15 +245926,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -246039,15 +246039,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -246119,15 +246119,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -246198,15 +246198,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -246290,15 +246290,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -246405,15 +246405,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -246473,15 +246473,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -246566,20 +246566,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -246591,15 +246591,15 @@
           "player": 0,
           "action": "raise",
           "amount": 700.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1050.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "turn": [
@@ -246692,15 +246692,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -246800,15 +246800,15 @@
       "river": "Kh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -246920,15 +246920,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -247000,15 +247000,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -247089,15 +247089,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -247129,15 +247129,15 @@
           "player": 1,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 900.0
+          "amount": 750.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ]
     }
@@ -247197,24 +247197,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 890.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -247383,15 +247383,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 215.0
+          "amount": 115.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -247463,15 +247463,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -247540,24 +247540,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 675.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -247801,15 +247801,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -247955,15 +247955,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -248043,20 +248043,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1275.0
+          "amount": 1100.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -248124,15 +248124,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -248332,28 +248332,28 @@
       "river": "7h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -248469,15 +248469,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -248588,15 +248588,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -248669,15 +248669,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -248775,15 +248775,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -248855,24 +248855,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 975.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -248939,15 +248939,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -249033,15 +249033,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -249147,15 +249147,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 275.0
+          "amount": 175.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -249226,15 +249226,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -249311,15 +249311,15 @@
       "river": "9c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -249433,15 +249433,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -249525,15 +249525,15 @@
       "river": "3c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -249648,15 +249648,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -249852,15 +249852,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -249929,28 +249929,28 @@
       "river": "Th"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 550.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -250142,15 +250142,15 @@
       "turn": "9d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -250256,15 +250256,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -250341,15 +250341,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -250449,15 +250449,15 @@
       "turn": "6h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -250554,15 +250554,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -250626,15 +250626,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -250790,15 +250790,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -250890,15 +250890,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -250983,15 +250983,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -251095,15 +251095,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -251167,15 +251167,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -251247,20 +251247,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 950.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -251323,15 +251323,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -251431,15 +251431,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -251551,15 +251551,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -251654,28 +251654,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 1025.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -251756,15 +251756,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -251872,15 +251872,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -251962,28 +251962,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 825.0
+          "amount": 715.0
         },
         {
           "player": 4,
           "action": "fold"
         }
       ]
     }
@@ -252051,15 +252051,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -252180,15 +252180,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -252261,15 +252261,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -252435,15 +252435,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -252526,15 +252526,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -252605,15 +252605,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -252698,15 +252698,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -252802,15 +252802,15 @@
       "turn": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -252919,15 +252919,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -252987,20 +252987,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 440.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -253200,15 +253200,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -253272,15 +253272,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -253340,15 +253340,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -253428,15 +253428,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -253500,20 +253500,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 950.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -253581,20 +253581,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 800.0
+          "amount": 625.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -253766,15 +253766,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -253854,20 +253854,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -253930,15 +253930,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -254042,15 +254042,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -254207,15 +254207,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 205.0
+          "amount": 105.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -254287,15 +254287,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -254355,15 +254355,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -254431,15 +254431,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -254531,15 +254531,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -254620,15 +254620,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -254709,15 +254709,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -254821,15 +254821,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -255007,15 +255007,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -255200,15 +255200,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -255296,15 +255296,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -255403,15 +255403,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 185.0
+          "amount": 135.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -255476,28 +255476,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1300.0
+          "amount": 1125.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -255610,15 +255610,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -255745,15 +255745,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -255829,15 +255829,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -255901,33 +255901,33 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1150.0
+          "amount": 950.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2500.0
+          "amount": 1400.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 0,
@@ -255994,15 +255994,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -256089,15 +256089,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -256166,15 +256166,15 @@
       "river": "Th"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -256300,15 +256300,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -256372,15 +256372,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -256452,15 +256452,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -256469,15 +256469,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -256533,15 +256533,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -256612,15 +256612,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -256836,15 +256836,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -256935,15 +256935,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -257026,15 +257026,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -257129,15 +257129,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -257216,15 +257216,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 200.0
+          "amount": 150.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -257287,15 +257287,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -257443,15 +257443,15 @@
       "river": "7d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -257483,15 +257483,15 @@
           "player": 5,
           "action": "raise",
           "amount": 365.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1095.0
+          "amount": 730.0
         },
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 5,
@@ -257589,15 +257589,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -257772,15 +257772,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -257979,15 +257979,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -258075,15 +258075,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -258191,15 +258191,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -258280,15 +258280,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -258321,15 +258321,15 @@
           "player": 0,
           "action": "raise",
           "amount": 600.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 3600.0
+          "amount": 3000.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -258392,15 +258392,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -258492,15 +258492,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -258509,15 +258509,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 825.0
+          "amount": 725.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -258550,15 +258550,15 @@
           "player": 1,
           "action": "raise",
           "amount": 2625.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 8275.0
+          "amount": 5650.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -258619,28 +258619,28 @@
       "river": "4h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -258732,15 +258732,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -258892,15 +258892,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -259084,15 +259084,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -259284,15 +259284,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -259396,15 +259396,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -259508,15 +259508,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -259580,20 +259580,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 525.0
+          "amount": 300.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -259606,15 +259606,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 1750.0
+          "amount": 1450.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -259666,15 +259666,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -259761,15 +259761,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -259852,20 +259852,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 850.0
+          "amount": 675.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -259921,15 +259921,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -259942,15 +259942,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1100.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -260077,15 +260077,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -260164,15 +260164,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -260264,15 +260264,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -260368,15 +260368,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -260469,15 +260469,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -260560,20 +260560,20 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 825.0
+          "amount": 600.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -260728,15 +260728,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -260896,15 +260896,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -260972,15 +260972,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -261048,15 +261048,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -261125,15 +261125,15 @@
       "river": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -261369,24 +261369,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 975.0
+          "amount": 825.0
         },
         {
           "player": 5,
           "action": "fold"
         }
       ]
     }
@@ -261463,15 +261463,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -261574,29 +261574,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 813.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2163.0
+          "amount": 1350.0
         },
         {
           "player": 0,
           "action": "call"
         }
       ],
       "flop": [
@@ -261692,15 +261692,15 @@
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 450.0
+          "amount": 350.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -261787,15 +261787,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -261803,15 +261803,15 @@
           "player": 0,
           "action": "raise",
           "amount": 450.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1950.0
+          "amount": 1500.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -261863,15 +261863,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -261963,15 +261963,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -262063,20 +262063,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -262151,15 +262151,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -262238,15 +262238,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 240.0
+          "amount": 140.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -262518,15 +262518,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -262599,15 +262599,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -262710,15 +262710,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -262844,15 +262844,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -262909,15 +262909,15 @@
           "player": 3,
           "action": "raise",
           "amount": 900.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 4250.0
+          "amount": 3350.0
         },
         {
           "player": 3,
           "action": "fold"
         }
       ]
     }
@@ -263072,15 +263072,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -263168,15 +263168,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -263282,15 +263282,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -263375,24 +263375,24 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 900.0
+          "amount": 675.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -263456,15 +263456,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -263536,15 +263536,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -263604,15 +263604,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -263680,15 +263680,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -263848,15 +263848,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -264091,20 +264091,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1000.0
+          "amount": 825.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -264179,15 +264179,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -264255,28 +264255,28 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 990.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 0,
@@ -264336,15 +264336,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -264526,15 +264526,15 @@
       "river": "Kc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -264649,15 +264649,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -264728,15 +264728,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -264820,15 +264820,15 @@
       "river": "8d"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -264935,15 +264935,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -265012,28 +265012,28 @@
       "river": "7c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 875.0
+          "amount": 665.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -265148,15 +265148,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -265235,15 +265235,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -265320,15 +265320,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "call"
         },
         {
           "player": 5,
@@ -265453,15 +265453,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -265550,15 +265550,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -265622,15 +265622,15 @@
       "turn": "Td"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -265730,15 +265730,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -265829,29 +265829,29 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 900.0
+          "amount": 775.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 2100.0
+          "amount": 1325.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -265928,15 +265928,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -266107,15 +266107,15 @@
       "turn": "Jd"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -266212,15 +266212,15 @@
       "turn": "3h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -266329,24 +266329,24 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1050.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -266423,15 +266423,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -266531,28 +266531,28 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 750.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -266616,15 +266616,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -266700,15 +266700,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -266781,15 +266781,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -266924,15 +266924,15 @@
           "player": 1,
           "action": "raise",
           "amount": 200.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 650.0
+          "amount": 450.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "turn": [
@@ -267018,15 +267018,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -267101,15 +267101,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -267193,15 +267193,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -267305,28 +267305,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 740.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -267391,15 +267391,15 @@
       "river": "9c"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -267607,15 +267607,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -267679,15 +267679,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -267767,15 +267767,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -267839,15 +267839,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -267923,15 +267923,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -268024,15 +268024,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -268113,15 +268113,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -268133,15 +268133,15 @@
           "player": 1,
           "action": "raise",
           "amount": 300.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 600.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "turn": [
@@ -268218,15 +268218,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -268290,15 +268290,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -268375,15 +268375,15 @@
       "river": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -268501,15 +268501,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -268616,15 +268616,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -268727,15 +268727,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -268799,15 +268799,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -269009,15 +269009,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -269126,15 +269126,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -269154,15 +269154,15 @@
           "player": 4,
           "action": "raise",
           "amount": 135.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 495.0
+          "amount": 360.0
         },
         {
           "player": 4,
           "action": "call"
         }
       ],
       "turn": [
@@ -269256,15 +269256,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -269359,15 +269359,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -269470,15 +269470,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -269496,15 +269496,15 @@
           "player": 0,
           "action": "raise",
           "amount": 450.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 750.0
         },
         {
           "player": 0,
           "action": "fold"
         }
       ]
     }
@@ -269571,15 +269571,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
@@ -269599,15 +269599,15 @@
           "player": 4,
           "action": "raise",
           "amount": 250.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 550.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -269763,15 +269763,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -269874,24 +269874,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1250.0
+          "amount": 1075.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -269991,15 +269991,15 @@
       "river": "Jh"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -270048,15 +270048,15 @@
           "player": 2,
           "action": "raise",
           "amount": 150.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ]
     }
@@ -270108,15 +270108,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -270125,15 +270125,15 @@
         {
           "player": 5,
           "action": "call"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1350.0
+          "amount": 1200.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -270205,15 +270205,15 @@
       "turn": "Ts"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -270335,15 +270335,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -270442,15 +270442,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -270554,20 +270554,20 @@
       "turn": "Qs"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 850.0
+          "amount": 650.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -270580,15 +270580,15 @@
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
           "action": "raise",
-          "amount": 2200.0
+          "amount": 1550.0
         },
         {
           "player": 3,
           "action": "call"
         }
       ],
       "flop": [
@@ -270671,15 +270671,15 @@
       "river": "Ah"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -270722,15 +270722,15 @@
           "player": 2,
           "action": "raise",
           "amount": 765.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2055.0
+          "amount": 1290.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "river": [
@@ -270913,28 +270913,28 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 925.0
+          "amount": 765.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 3,
@@ -271026,25 +271026,25 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 550.0
+          "amount": 450.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1725.0
+          "amount": 1275.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -271353,15 +271353,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -271464,15 +271464,15 @@
       "river": "5s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -271580,15 +271580,15 @@
       "river": "4h"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -271702,15 +271702,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -271789,15 +271789,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -271868,15 +271868,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -271963,15 +271963,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -272056,15 +272056,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -272177,20 +272177,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 1025.0
+          "amount": 850.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -272255,15 +272255,15 @@
       "river": "As"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -272272,15 +272272,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 950.0
+          "amount": 800.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 2,
@@ -272385,15 +272385,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -272500,15 +272500,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -272572,20 +272572,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 800.0
+          "amount": 575.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -272653,15 +272653,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -272938,15 +272938,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 250.0
+          "amount": 200.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -273036,15 +273036,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -273125,15 +273125,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -273315,15 +273315,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -273402,15 +273402,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -273482,24 +273482,24 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 725.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 4,
@@ -273574,15 +273574,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -273786,20 +273786,20 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 825.0
+          "amount": 625.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -273906,15 +273906,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -274132,15 +274132,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -274204,15 +274204,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -274221,15 +274221,15 @@
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1200.0
+          "amount": 1075.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 0,
@@ -274297,20 +274297,20 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 222.0
+          "amount": 122.0
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 900.0
+          "amount": 728.0
         },
         {
           "player": 1,
           "action": "fold"
         },
         {
           "player": 5,
@@ -274382,15 +274382,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -274482,15 +274482,15 @@
       ]
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -274593,15 +274593,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -274691,15 +274691,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -274771,15 +274771,15 @@
       "turn": "Qc"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -274880,33 +274880,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1125.0
+          "amount": 1000.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2250.0
+          "amount": 1250.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -274970,15 +274970,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -275034,15 +275034,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -275119,15 +275119,15 @@
       "river": "Ac"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -275165,15 +275165,15 @@
           "player": 2,
           "action": "raise",
           "amount": 675.0
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 2475.0
+          "amount": 1800.0
         },
         {
           "player": 2,
           "action": "call"
         }
       ],
       "river": [
@@ -275260,15 +275260,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -275369,15 +275369,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 287.0
+          "amount": 187.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -275458,25 +275458,25 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 700.0
+          "amount": 475.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 1525.0
+          "amount": 825.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -275564,15 +275564,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 0,
           "action": "call"
         },
         {
           "player": 1,
@@ -275661,33 +275661,33 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1100.0
+          "amount": 950.0
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 2770.0
+          "amount": 1820.0
         },
         {
           "player": 1,
           "action": "fold"
         }
       ]
     }
@@ -275748,28 +275748,28 @@
       "river": "2s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 700.0
+          "amount": 500.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -275940,15 +275940,15 @@
       "river": "3s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "call"
         },
         {
           "player": 4,
@@ -276058,15 +276058,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -276143,24 +276143,24 @@
       "river": "4s"
     },
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 210.0
+          "amount": 110.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 700.0
+          "amount": 490.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -276272,15 +276272,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 250.0
+          "amount": 150.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -276386,15 +276386,15 @@
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
@@ -276507,15 +276507,15 @@
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
@@ -276616,15 +276616,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 4,
           "action": "fold"
         },
         {
           "player": 5,
@@ -276727,15 +276727,15 @@
         {
           "player": 5,
           "action": "fold"
         },
         {
           "player": 0,
           "action": "raise",
-          "amount": 150.0
+          "amount": 100.0
         },
         {
           "player": 1,
           "action": "call"
         }
       ],
       "flop": [
@@ -276808,15 +276808,15 @@
       ]
     ],
     "actions": {
       "preflop": [
         {
           "player": 2,
           "action": "raise",
-          "amount": 225.0
+          "amount": 125.0
         },
         {
           "player": 3,
           "action": "fold"
         },
         {
           "player": 4,
@@ -276829,15 +276829,15 @@
         {
           "player": 0,
           "action": "fold"
         },
         {
           "player": 1,
           "action": "raise",
-          "amount": 1050.0
+          "amount": 925.0
         },
         {
           "player": 2,
           "action": "fold"
         }
       ]
     }
@@ -277025,15 +277025,15 @@
         {
           "player": 2,
           "action": "fold"
         },
         {
           "player": 3,
           "action": "raise",
-          "amount": 200.0
+          "amount": 100.0
         },
         {
           "player": 4,
         },
       ],