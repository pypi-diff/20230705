# Comparing `tmp/reddit_decider-1.3.1.tar.gz` & `tmp/reddit_decider-1.4.0.tar.gz`

## Comparing `reddit_decider-1.3.1.tar` & `reddit_decider-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.3.1/local_dependencies/decider/Cargo.toml
--rw-r--r--   0        0        0       19 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/.gitignore
--rw-r--r--   0        0        0      323 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/Makefile
--rw-r--r--   0        0        0      710 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/README.md
--rw-r--r--   0        0        0     6097 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/benches/decider.rs
--rw-r--r--   0        0        0     9514 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/src/context.rs
--rw-r--r--   0        0        0    48184 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/src/events.rs
--rw-r--r--   0        0        0   108905 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/local_dependencies/decider/src/lib.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.3.1/Cargo.toml
--rw-r--r--   0        0        0      112 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/.gitignore
--rw-r--r--   0        0        0      786 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/Makefile
--rw-r--r--   0        0        0     6041 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/README.md
--rw-r--r--   0        0        0      273 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    22412 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/python/rust_decider/__init__.py
--rw-r--r--   0        0        0      259 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/python/rust_decider/prometheus_metrics.py
--rw-r--r--   0        0        0      177 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/requirements-dev.txt
--rw-r--r--   0        0        0       40 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/setup.cfg
--rw-r--r--   0        0        0     1300 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/setup.py
--rw-r--r--   0        0        0    34812 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/src/lib.rs
--rw-r--r--   0        0        0    40918 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/test/decider_unit_test.py
--rw-r--r--   0        0        0    10110 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/test/integration_test.py
--rw-r--r--   0        0        0     2903 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/test/test_rust.py
--rw-r--r--   0        0        0    34104 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/test/unit_test.py
--rw-r--r--   0        0        0     3088 2023-06-15 06:48:58.000000 reddit_decider-1.3.1/test/utils.py
--rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.4.0/local_dependencies/decider/Cargo.toml
+-rw-r--r--   0        0        0       19 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/.gitignore
+-rw-r--r--   0        0        0      323 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/Makefile
+-rw-r--r--   0        0        0      710 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/README.md
+-rw-r--r--   0        0        0     6097 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/benches/decider.rs
+-rw-r--r--   0        0        0     9514 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/src/context.rs
+-rw-r--r--   0        0        0    48184 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/src/events.rs
+-rw-r--r--   0        0        0   110863 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/src/lib.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.4.0/Cargo.toml
+-rw-r--r--   0        0        0      112 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/.gitignore
+-rw-r--r--   0        0        0      786 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/Makefile
+-rw-r--r--   0        0        0     6041 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/README.md
+-rw-r--r--   0        0        0      273 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    22412 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/python/rust_decider/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/python/rust_decider/prometheus_metrics.py
+-rw-r--r--   0        0        0      177 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0       40 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/setup.cfg
+-rw-r--r--   0        0        0     1300 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/setup.py
+-rw-r--r--   0        0        0    34812 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/src/lib.rs
+-rw-r--r--   0        0        0    40966 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/decider_unit_test.py
+-rw-r--r--   0        0        0    10110 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/integration_test.py
+-rw-r--r--   0        0        0     2903 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/test_rust.py
+-rw-r--r--   0        0        0    34128 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/unit_test.py
+-rw-r--r--   0        0        0     3088 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/utils.py
+-rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.4.0/PKG-INFO
```

### Comparing `reddit_decider-1.3.1/local_dependencies/decider/Cargo.toml` & `reddit_decider-1.4.0/local_dependencies/decider/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "decider"
-version = "1.3.1"
+version = "1.4.0"
 edition = "2021"
 description = "a package for AB-testing and dynamic config"
 homepage = "https://mattknox.com"
 license = "MIT"
 documentation = "https://mattknox.com/decider"
 readme = "README.md"
```

### Comparing `reddit_decider-1.3.1/local_dependencies/decider/README.md` & `reddit_decider-1.4.0/local_dependencies/decider/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/local_dependencies/decider/benches/decider.rs` & `reddit_decider-1.4.0/local_dependencies/decider/benches/decider.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/local_dependencies/decider/src/context.rs` & `reddit_decider-1.4.0/local_dependencies/decider/src/context.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/local_dependencies/decider/src/events.rs` & `reddit_decider-1.4.0/local_dependencies/decider/src/events.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/local_dependencies/decider/src/lib.rs` & `reddit_decider-1.4.0/local_dependencies/decider/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -888,14 +888,21 @@
     #[error("Dynamic Configuration Feature type mismatch")]
     DcTypeMismatch,
     #[error("Number deserialization failed")]
     NumberDeserializationError,
     #[error("Decider returned malformed event: {0}")]
     MalformedEventError(#[source] Box<dyn Error>),
 }
+#[derive(Debug, Error)]
+pub enum ConfigError {
+    #[error("Manifest parsing error: {0}")]
+    ParsingError(serde_json::Error),
+    #[error("Missing bucketing_field for range_variant")]
+    MissingBucketingField,
+}
 
 #[derive(Debug, Error)]
 pub enum DeciderInitError {
     #[error("Std io error: {0}")]
     IoError(
         #[from]
         #[source]
@@ -906,15 +913,15 @@
         #[from]
         #[source]
         serde_json::Error,
     ),
     #[error("Invalid decisionmaker: {0:?}")]
     InvalidDecisionMaker(String),
     #[error("Partially loaded Decider: {} features failed to load", .1.len())]
-    PartialLoad(Decider, HashMap<String, serde_json::Error>),
+    PartialLoad(Decider, HashMap<String, ConfigError>),
 }
 
 /// An `Event` holds a hydrated exposure event, serialized as a json string, as well as an explicit
 /// `DecisionKind`. The kind can be used by the client to choose whether to expose this event.
 #[derive(Serialize, Debug, Clone, PartialEq, Eq)]
 pub struct Event {
     pub kind: DecisionKind,
@@ -1230,19 +1237,32 @@
 }
 
 struct ExperimentConfig {
     experiments: HashMap<String, Experiment>,
     override_groups: HashMap<String, OverrideGroup>,
 }
 
-fn experiment_config_to_features(ec: &ExperimentConfig) -> Vec<Feature> {
-    ec.experiments
+fn experiment_config_to_features(
+    ec: &ExperimentConfig,
+    errs: HashMap<String, ConfigError>,
+) -> (Vec<Feature>, HashMap<String, ConfigError>) {
+    let mut errs = errs;
+    let features = ec
+        .experiments
         .values()
-        .map(|exp| experiment_to_feature(exp, ec))
-        .collect()
+        .filter_map(|exp| match experiment_to_feature(exp, ec) {
+            Ok(f) => Some(f),
+            Err(e) => {
+                errs.insert(exp.name.clone(), e);
+                None
+            }
+        })
+        .collect();
+
+    (features, errs)
 }
 
 /// An intermediate struct representing a raw experiment config. The experiments are parsed as
 /// JSON values.
 ///
 /// This struct allows us to partially load [`Decider`]. When deserializing into a specific type,
 /// serde will return an error if any part of the type can't be properly deserialized. This means
@@ -1265,36 +1285,36 @@
 }
 
 static OVERRIDE_GROUPS: &str = "$override_groups";
 
 impl RawConfig {
     /// Deserializes the raw config into a list of valid features. Any features that can't be
     /// successfully deserialized are returned in the `HashMap`.
-    fn features(self) -> (Vec<Feature>, HashMap<String, serde_json::Error>) {
+    fn features(self) -> (Vec<Feature>, HashMap<String, ConfigError>) {
         let mut ec = HashMap::new();
-        let mut errs = HashMap::new();
+        let mut errs: HashMap<String, ConfigError> = HashMap::new();
 
         for (name, feature_json) in self.raw_experiments {
             match serde_json::from_value::<Experiment>(feature_json) {
                 Ok(exp) if name != OVERRIDE_GROUPS => {
                     ec.insert(name, exp);
                 }
                 Err(err) => {
-                    errs.insert(name, err);
+                    errs.insert(name, ConfigError::ParsingError(err));
                 }
                 _ => (),
             }
         }
 
         let cfg = ExperimentConfig {
             experiments: ec,
             override_groups: self.override_groups.map(|f| f.groups).unwrap_or_default(),
         };
 
-        (experiment_config_to_features(&cfg), errs)
+        experiment_config_to_features(&cfg, errs)
     }
 }
 
 #[derive(Deserialize, Debug, Clone)]
 struct Experiment {
     id: u32,
     name: String,
@@ -1402,87 +1422,86 @@
             Value::Bool(_) => ValueType::Boolean,
             Value::Null => ValueType::Null,
             _ => panic!("value {value} are not supported", value = value),
         }
     }
 }
 
-fn experiment_to_dynamic_config(exp: &Experiment) -> DynamicConfig {
+fn experiment_to_dynamic_config(exp: &Experiment) -> Result<DynamicConfig, ConfigError> {
     let value = exp
         .value
         .clone()
         .map(Value::from)
         .unwrap_or_else(|| Value::from(exp.value_type.unwrap_or(ValueType::Null)));
     let value_type = value.borrow().into();
 
-    DynamicConfig {
+    Ok(DynamicConfig {
         metadata: exp.into(),
         value,
         value_type,
-    }
+    })
 }
 
-fn experiment_to_multivariant_choice(exp: &Experiment, ec: &ExperimentConfig) -> RangeVariant {
-    let holdout = match &exp.parent_hg_name {
-        None => None,
-        Some(name) => ec.experiments.get(name).map(|e| {
-            Box::new(Feature::RangeVariant(experiment_to_multivariant_choice(
-                e, ec,
-            )))
-        }),
+fn experiment_to_multivariant_choice(
+    exp: &Experiment,
+    ec: &ExperimentConfig,
+) -> Result<RangeVariant, ConfigError> {
+    let get_inner = |name: Option<&String>| -> Result<Option<Feature>, ConfigError> {
+        name.and_then(|n| {
+            ec.experiments
+                .get(n)
+                .map(|e| experiment_to_multivariant_choice(e, ec))
+        })
+        .map_or(Ok(None), |r| r.map(Feature::RangeVariant).map(Some))
     };
 
-    let mutex_group = match &exp.parent_meg_name {
-        None => None,
-        Some(name) => ec.experiments.get(name).map(|e| {
-            Box::new(Feature::RangeVariant(experiment_to_multivariant_choice(
-                e, ec,
-            )))
-        }),
-    };
+    let holdout = get_inner(exp.parent_hg_name.as_ref())?.map(Box::new);
+    let mutex_group = get_inner(exp.parent_meg_name.as_ref())?.map(Box::new);
 
     let variant_set = VariantSet {
         start_ts: exp.start_ts,
         stop_ts: exp.stop_ts,
         shuffle_version: exp.experiment.shuffle_version,
         variants: exp.experiment.variants.clone(),
         bucketing_field: exp
             .experiment
             .bucketing_field
             .clone()
-            .expect("missing bucketing_field for range variant"),
+            .ok_or(ConfigError::MissingBucketingField)?,
         holdout,
         mutex_group,
     };
 
     let overrides = exp.experiment.overrides.as_ref().map(|ov| {
         ov.iter()
             .map(|hm| {
                 hm.iter()
                     .map(|(k, v)| (k.to_string(), v.unroll_groups(&ec.override_groups)))
                     .collect()
             })
             .collect()
     });
 
-    RangeVariant {
+    Ok(RangeVariant {
         metadata: exp.into(),
         emit_event: exp.emit_event,
         variant_set,
         enabled: exp.enabled,
         targeting: exp.experiment.targeting.clone(),
         overrides,
-    }
+    })
 }
 
-fn experiment_to_feature(exp: &Experiment, ec: &ExperimentConfig) -> Feature {
+fn experiment_to_feature(exp: &Experiment, ec: &ExperimentConfig) -> Result<Feature, ConfigError> {
     match exp.experiment_type {
-        ExperimentType::DynamicConfig => Feature::DynamicConfig(experiment_to_dynamic_config(exp)),
+        ExperimentType::DynamicConfig => {
+            experiment_to_dynamic_config(exp).map(Feature::DynamicConfig)
+        }
         ExperimentType::RangeVariant | ExperimentType::FeatureRollout => {
-            Feature::RangeVariant(experiment_to_multivariant_choice(exp, ec))
+            experiment_to_multivariant_choice(exp, ec).map(Feature::RangeVariant)
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use proptest::prelude::*;
@@ -1762,14 +1781,55 @@
         let ctx = make_ctx(None)?;
         let d = build_decider(None, None, None)?;
         assert!(d.choose("first_feature", &ctx, None).is_ok());
         Ok(())
     }
 
     #[test]
+    fn test_missing_bucketing_field() {
+        let cgf = json!({
+            "x0": {
+                "id": 1,
+                "name": "x0",
+                "enabled": true,
+                "owner": "test",
+                "version": "4",
+                "type": "range_variant",
+                "emit_event": true,
+                "experiment": {
+                "variants": [
+                    {
+                    "name": "enabled",
+                    "size": 1,
+                    "range_end": 1,
+                    "range_start": 0.0
+                    }
+                ],
+                "experiment_version": 4,
+                "shuffle_version": 1,
+                "overrides": []
+                },
+                "start_ts": 0,
+                "stop_ts": 2147483647,
+                "value": "range_variant"
+            }
+        });
+
+        let json_str = serde_json::to_string(&cgf).unwrap();
+        let json_bytes = json_str.as_bytes();
+
+        let errs = match Decider::from_bytes(json_bytes) {
+            Err(DeciderInitError::PartialLoad(_, errs)) => errs,
+            _ => unreachable!("Constructor should return a partial load!"),
+        };
+
+        assert!(matches!(errs.get("x0"), Some(ConfigError::MissingBucketingField)));
+    }
+
+    #[test]
     fn decider_errors_on_missing_name() -> Result<(), DeciderInitError> {
         let ctx = make_ctx(None)?;
         let d = build_decider(None, None, None)?;
         let r = d.choose("missing", &ctx, None);
         match r {
             Ok(_) => panic!(),
             Err(e) => println!("got expected error: {:#?}", e),
@@ -2169,15 +2229,16 @@
                 ("second".to_string(), e2),
                 ("meg".to_string(), meg),
                 ("hg".to_string(), hg),
             ]),
             override_groups: HashMap::new(),
         };
 
-        let fv: Vec<Feature> = experiment_config_to_features(&ec);
+        let errs = HashMap::new();
+        let (fv, _) = experiment_config_to_features(&ec, errs);
         let f1 = fv.iter().find(|&f| f.metadata().name == "first").unwrap();
         let f2 = fv.iter().find(|&f| f.metadata().name == "second").unwrap();
         let fmeg = fv.iter().find(|&f| f.metadata().name == "meg").unwrap();
         let fhg = fv.iter().find(|&f| f.metadata().name == "hg").unwrap();
         assert_eq!(
             get_fp(f1, FeatureParent::Holdout).unwrap().metadata().name,
             fhg.metadata().name
@@ -2915,15 +2976,15 @@
         assert_eq!(decision.feature_version, 3);
         assert_eq!(decision.variant_name, Some("variant_0".to_string()));
 
         // Check errors.
         assert_eq!(errs.len(), 1);
         assert!(matches!(
             errs.get("invalid_exp"),
-            Some(serde_json::Error { .. }),
+            Some(ConfigError::ParsingError(serde_json::Error { .. })),
         ));
     }
 
     mod regression {
         use crate::{Context, Decider, DecisionKind};
         use serde_json::json;
```

### Comparing `reddit_decider-1.3.1/Makefile` & `reddit_decider-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/README.md` & `reddit_decider-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/python/rust_decider/__init__.py` & `reddit_decider-1.4.0/python/rust_decider/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/setup.py` & `reddit_decider-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/src/lib.rs` & `reddit_decider-1.4.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/test/decider_unit_test.py` & `reddit_decider-1.4.0/test/decider_unit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,30 +202,30 @@
         }
 
         with create_temp_config_file(cfg) as f:
             with self.assertLogs() as captured:
                 setup_decider_class(f.name)
 
             assert any(
-                "Partially loaded Decider: 1 features failed to load: {'exp_0': 'invalid type: string \"3248\", expected u32'}"
+                "Partially loaded Decider: 1 features failed to load: {'exp_0': 'Manifest parsing error: invalid type: string \"3248\", expected u32'}"
                 in x.getMessage()
                 for x in captured.records
             )
 
     def test_init_partially_bad_cfg(self):
         cfg = self.genexp_0_cfg
         invalid_exp = {"some_key": [1, 2, 3]}
         cfg.update(invalid_exp)
 
         with create_temp_config_file(cfg) as f:
             with self.assertLogs() as captured:
                 decider = setup_decider_class(f.name)
 
                 assert any(
-                    "Partially loaded Decider: 1 features failed to load: {'some_key': 'invalid type: integer `2`, expected a string'}"
+                    "Partially loaded Decider: 1 features failed to load: {'some_key': 'Manifest parsing error: invalid type: integer `2`, expected a string'}"
                     in x.getMessage()
                     for x in captured.records
                 )
 
                 choice = decider.choose("genexp_0", self.valid_ctx_dict)
 
                 self.assertEqual(
```

### Comparing `reddit_decider-1.3.1/test/integration_test.py` & `reddit_decider-1.4.0/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/test/test_rust.py` & `reddit_decider-1.4.0/test/test_rust.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/test/unit_test.py` & `reddit_decider-1.4.0/test/unit_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
                 },
             }
         }
 
         with create_temp_config_file(cfg) as f:
             decider = setup_decider(f.name)
             assert (
-                "Decider initialization failed: Partially loaded Decider: 1 features failed to load: { 'exp_0': invalid type: string \"3248\", expected u32 }."
+                "Decider initialization failed: Partially loaded Decider: 1 features failed to load: { 'exp_0': Manifest parsing error: invalid type: string \"3248\", expected u32 }."
                 in decider.err()
             )
 
     def test_make_ctx(self):
         ctx = rust_decider.make_ctx(self.valid_ctx_dict)
         self.assertEqual(ctx.err(), None)
```

### Comparing `reddit_decider-1.3.1/test/utils.py` & `reddit_decider-1.4.0/test/utils.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.3.1/PKG-INFO` & `reddit_decider-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-decider
-Version: 1.3.1
+Version: 1.4.0
 Requires-Dist: prometheus-client>=0.12.0,<1.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rust_decider
 
 Rust implementation of bucketing, targeting, overrides, and dynamic config logic.
```

