# Comparing `tmp/segment-geospatial-0.8.3.tar.gz` & `tmp/segment-geospatial-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.8.3.tar", last modified: Wed Jun 21 03:39:32 2023, max compression
+gzip compressed data, was "segment-geospatial-0.8.4.tar", last modified: Wed Jul  5 15:26:29 2023, max compression
```

## Comparing `segment-geospatial-0.8.3.tar` & `segment-geospatial-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92509 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/samgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/samgeo/text_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 03:39:32.000000 segment-geospatial-0.8.3/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-21 03:39:32.241140 segment-geospatial-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-21 03:39:22.000000 segment-geospatial-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:26:29.205231 segment-geospatial-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-05 15:26:29.205231 segment-geospatial-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:26:29.205231 segment-geospatial-0.8.4/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92951 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30723 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19497 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:26:29.205231 segment-geospatial-0.8.4/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-05 15:26:29.000000 segment-geospatial-0.8.4/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-05 15:26:29.000000 segment-geospatial-0.8.4/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 15:26:29.000000 segment-geospatial-0.8.4/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:26:29.000000 segment-geospatial-0.8.4/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 15:26:29.000000 segment-geospatial-0.8.4/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 15:26:29.000000 segment-geospatial-0.8.4/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 15:26:29.205231 segment-geospatial-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-05 15:26:17.000000 segment-geospatial-0.8.4/setup.py
```

### Comparing `segment-geospatial-0.8.3/LICENSE` & `segment-geospatial-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.3/PKG-INFO` & `segment-geospatial-0.8.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.3
+Version: 0.8.4
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -105,14 +105,18 @@
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe) and the [Resources for Unlocking the Power of Deep Learning Applications Using ArcGIS](https://community.esri.com/t5/education-blog/resources-for-unlocking-the-power-of-deep-learning/ba-p/1293098). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
 
 The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
 
+## Legal Notice
+
+This repository and its content are provided for educational purposes only. By using the information and code provided, users acknowledge that they are using the APIs and models at their own risk and agree to comply with any applicable laws and regulations. Users who intend to download a large number of image tiles from any basemap are advised to contact the basemap provider to obtain permission before doing so. Unauthorized use of the basemap or any of its components may be a violation of copyright laws or other applicable laws and regulations.
+
 ## Acknowledgements
 
 This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.8.3/README.md` & `segment-geospatial-0.8.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,18 @@
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe) and the [Resources for Unlocking the Power of Deep Learning Applications Using ArcGIS](https://community.esri.com/t5/education-blog/resources-for-unlocking-the-power-of-deep-learning/ba-p/1293098). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
 
 The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
 
+## Legal Notice
+
+This repository and its content are provided for educational purposes only. By using the information and code provided, users acknowledge that they are using the APIs and models at their own risk and agree to comply with any applicable laws and regulations. Users who intend to download a large number of image tiles from any basemap are advised to contact the basemap provider to obtain permission before doing so. Unauthorized use of the basemap or any of its components may be a violation of copyright laws or other applicable laws and regulations.
+
 ## Acknowledgements
 
 This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.8.3/samgeo/common.py` & `segment-geospatial-0.8.4/samgeo/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1567,15 +1567,18 @@
             cmd = "pip install ."
 
         os.system(cmd)
         os.chdir(work_dir)
 
         if not keep:
             shutil.rmtree(pkg_dir)
-            os.remove(filename)
+            try:
+                os.remove(filename)
+            except:
+                pass
 
         print("Package updated successfully.")
 
     except Exception as e:
         raise Exception(e)
 
 
@@ -1607,15 +1610,15 @@
 
     m = leafmap.Map(repeat_mode=repeat_mode, **kwargs)
     m.default_style = {"cursor": "crosshair"}
     m.add_basemap(basemap, show=False)
 
     # Skip the image layer if localtileserver is not available
     try:
-        m.add_raster(sam.image, layer_name="Image")
+        m.add_raster(sam.source, layer_name="Image")
     except:
         pass
 
     m.fg_markers = []
     m.bg_markers = []
 
     fg_layer = ipyleaflet.LayerGroup(layers=m.fg_markers, name="Foreground")
@@ -1967,15 +1970,18 @@
                             m.remove_layer(m.find_layer("Masks"))
                         if m.find_layer("Regularized") is not None:
                             m.remove_layer(m.find_layer("Regularized"))
 
                         if hasattr(sam, "prediction_fp") and os.path.exists(
                             sam.prediction_fp
                         ):
-                            os.remove(sam.prediction_fp)
+                            try:
+                                os.remove(sam.prediction_fp)
+                            except:
+                                pass
 
                         # Skip the image layer if localtileserver is not available
                         try:
                             m.add_raster(
                                 filename,
                                 nodata=0,
                                 cmap="Blues",
@@ -2087,15 +2093,18 @@
                     m.user_rois = None
                     m.fg_markers = []
                     m.bg_markers = []
                     m.fg_layer.clear_layers()
                     m.bg_layer.clear_layers()
                     fg_count.value = 0
                     bg_count.value = 0
-                os.remove(sam.prediction_fp)
+                try:
+                    os.remove(sam.prediction_fp)
+                except:
+                    pass
             except:
                 pass
 
     reset_button.observe(reset_button_click, "value")
 
     toolbar_control = ipyleaflet.WidgetControl(
         widget=toolbar_widget, position="topright"
@@ -2483,26 +2492,30 @@
                     print("Please run sam.set_image() first.")
                 else:
                     print("Segmenting...")
                     layer_name = text_prompt.value.replace(" ", "_")
                     filename = os.path.join(
                         out_dir, f"{layer_name}_{random_string()}.tif"
                     )
-                    sam.predict(
-                        sam.source,
-                        text_prompt.value,
-                        box_slider.value,
-                        text_slider.value,
-                        output=filename,
-                    )
-                    sam.output = filename
-                    if m.find_layer(layer_name) is not None:
-                        m.remove_layer(m.find_layer(layer_name))
-                    if m.find_layer(f"{layer_name}_rect") is not None:
-                        m.remove_layer(m.find_layer(f"{layer_name} Regularized"))
+                    try:
+                        sam.predict(
+                            sam.source,
+                            text_prompt.value,
+                            box_slider.value,
+                            text_slider.value,
+                            output=filename,
+                        )
+                        sam.output = filename
+                        if m.find_layer(layer_name) is not None:
+                            m.remove_layer(m.find_layer(layer_name))
+                        if m.find_layer(f"{layer_name}_rect") is not None:
+                            m.remove_layer(m.find_layer(f"{layer_name} Regularized"))
+                    except Exception as e:
+                        output.clear_output()
+                        print(e)
                     if os.path.exists(filename):
                         try:
                             m.add_raster(
                                 filename,
                                 layer_name=layer_name,
                                 palette=cmap_dropdown.value,
                                 opacity=opacity_slider.value,
```

### Comparing `segment-geospatial-0.8.3/samgeo/samgeo.py` & `segment-geospatial-0.8.4/samgeo/samgeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     """The main class for segmenting geospatial data with the Segment Anything Model (SAM). See
     https://github.com/facebookresearch/segment-anything for details.
     """
 
     def __init__(
         self,
         model_type="vit_h",
-        checkpoint="sam_vit_h_4b8939.pth",
+        checkpoint=None,
         automatic=True,
         device=None,
         sam_kwargs=None,
     ):
         """Initialize the class.
 
         Args:
             model_type (str, optional): The model type. It can be one of the following: vit_h, vit_l, vit_b.
                 Defaults to 'vit_h'. See https://bit.ly/3VrpxUh for more details.
             checkpoint (str, optional): The path to the model checkpoint. It can be one of the following:
                 sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
-                Defaults to "sam_vit_h_4b8939.pth". See https://bit.ly/3VrpxUh for more details.
+                Defaults to None. See https://bit.ly/3VrpxUh for more details.
             automatic (bool, optional): Whether to use the automatic mask generator or input prompts. Defaults to True.
                 The automatic mask generator will segment the entire image, while the input prompts will segment selected objects.
             device (str, optional): The device to use. It can be one of the following: cpu, cuda.
                 Defaults to None, which will use cuda if available.
             sam_kwargs (dict, optional): Optional arguments for fine-tuning the SAM model. Defaults to None.
                 The available arguments with default values are listed below. See https://bit.ly/410RV0v for more details.
 
@@ -54,20 +54,44 @@
                 output_mode: str = "binary_mask",
 
         """
         # Download the checkpoint if it does not exist
         CACHE_PATH = os.environ.get(
             "TORCH_HOME", os.path.expanduser("~/.cache/torch/hub/checkpoints")
         )
+
+        model_types = {
+            "vit_h": "sam_vit_h_4b8939.pth",
+            "vit_l": "sam_vit_l_0b3195.pth",
+            "vit_b": "sam_vit_b_01ec64.pth",
+        }
+
+        if model_type not in model_types:
+            raise ValueError(
+                f"Model type {model_type} is not supported. It must be one of the following: {model_types}."
+            )
+
+        checkpoints = {
+            "sam_vit_h_4b8939.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
+            "sam_vit_l_0b3195.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
+            "sam_vit_b_01ec64.pth": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
+        }
+
+        if checkpoint is None:
+            url = checkpoints[model_types[model_type]]
+            checkpoint = model_types[model_type]
+        else:
+            url = None
+
         if not os.path.exists(checkpoint):
             basename = os.path.basename(checkpoint)
             checkpoint = os.path.join(CACHE_PATH, basename)
             if not os.path.exists(checkpoint):
                 print(f"Checkpoint {checkpoint} does not exist.")
-                download_checkpoint(output=checkpoint)
+                download_checkpoint(url=url, output=checkpoint)
         self.checkpoint = checkpoint
 
         # Use cuda if available
         if device is None:
             device = "cuda" if torch.cuda.is_available() else "cpu"
             if device == "cuda":
                 torch.cuda.empty_cache()
@@ -405,18 +429,19 @@
         if isinstance(image, str):
             if image.startswith("http"):
                 image = download_file(image)
 
             if not os.path.exists(image):
                 raise ValueError(f"Input path {image} does not exist.")
 
-            self.image = image
+            self.source = image
 
             image = cv2.imread(image)
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+            self.image = image
         elif isinstance(image, np.ndarray):
             pass
         else:
             raise ValueError("Input image must be either a path or a numpy array.")
 
         self.predictor.set_image(image, image_format=image_format)
 
@@ -447,15 +472,15 @@
             raise ValueError("No predictions found. Please run predict() first.")
 
         if index is None:
             index = self.scores.argmax(axis=0)
 
         array = self.masks[index] * mask_multiplier
         self.prediction = array
-        array_to_image(array, output, self.image, dtype=dtype, **kwargs)
+        array_to_image(array, output, self.source, dtype=dtype, **kwargs)
 
         if vector is not None:
             raster_to_vector(output, vector, simplify_tolerance=simplify_tolerance)
 
     def predict(
         self,
         point_coords=None,
@@ -511,15 +536,15 @@
         if hasattr(self, "point_coords"):
             point_coords = self.point_coords
 
         if hasattr(self, "point_labels"):
             point_labels = self.point_labels
 
         if point_crs is not None:
-            point_coords = coords_to_xy(self.image, point_coords, point_crs)
+            point_coords = coords_to_xy(self.source, point_coords, point_crs)
 
         if isinstance(point_coords, list):
             point_coords = np.array(point_coords)
 
         if point_labels is None:
             point_labels = [1] * len(point_coords)
         elif isinstance(point_labels, int):
@@ -532,15 +557,15 @@
                 else:
                     raise ValueError(
                         "The length of point_labels must be equal to the length of point_coords."
                     )
             point_labels = np.array(point_labels)
 
         if isinstance(box, list) and point_crs is not None:
-            box = np.array(bbox_to_xy(self.image, box, point_crs))
+            box = np.array(bbox_to_xy(self.source, box, point_crs))
 
         predictor = self.predictor
         masks, scores, logits = predictor.predict(
             point_coords, point_labels, box, mask_input, multimask_output, return_logits
         )
         self.masks = masks
         self.scores = scores
```

### Comparing `segment-geospatial-0.8.3/samgeo/text_sam.py` & `segment-geospatial-0.8.4/samgeo/text_sam.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,14 +229,15 @@
         box_threshold,
         text_threshold,
         output=None,
         mask_multiplier=255,
         dtype=np.uint8,
         save_args={},
         return_results=False,
+        return_coords=False,
         **kwargs,
     ):
         """
         Run both GroundingDINO and SAM model prediction.
 
         Parameters:
             image (Image): Input PIL Image.
@@ -270,14 +271,15 @@
                 transform = src.transform  # Save georeferencing information
                 crs = src.crs  # Save the Coordinate Reference System
                 image_pil = Image.fromarray(
                     image_np[:, :, :3]
                 )  # Convert numpy array to PIL image, excluding the alpha channel
         else:
             image_pil = image
+            image_np = np.array(image_pil)
 
         self.image = image_pil
 
         boxes, logits, phrases = self.predict_dino(
             image_pil, text_prompt, box_threshold, text_threshold
         )
         masks = torch.tensor([])
@@ -317,14 +319,21 @@
         self.phrases = phrases
         self.logits = logits
         self.prediction = mask_overlay
 
         if return_results:
             return masks, boxes, phrases, logits
 
+        if return_coords:
+            boxlist = []
+            for box in self.boxes:
+                box = box.cpu().numpy()
+                boxlist.append((box[0], box[1]))
+            return boxlist
+
     def predict_batch(
         self,
         images,
         out_dir,
         text_prompt,
         box_threshold,
         text_threshold,
@@ -361,15 +370,17 @@
 
         if not isinstance(images, list):
             raise ValueError("images must be a list or a directory to GeoTIFF files.")
 
         for i, image in enumerate(images):
             basename = os.path.splitext(os.path.basename(image))[0]
             if verbose:
-                print(f"Processing image {str(i+1).zfill(len(str(len(images))))} of {len(images)}: {image}...")
+                print(
+                    f"Processing image {str(i+1).zfill(len(str(len(images))))} of {len(images)}: {image}..."
+                )
             output = os.path.join(out_dir, f"{basename}_mask.tif")
             self.predict(
                 image,
                 text_prompt,
                 box_threshold,
                 text_threshold,
                 output=output,
```

### Comparing `segment-geospatial-0.8.3/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.8.4/segment_geospatial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.3
+Version: 0.8.4
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -105,14 +105,18 @@
 -   **QGIS**: Check out the [Geometric Attributes plugin for QGIS](https://github.com/BjornNyberg/Geometric-Attributes-Toolbox/wiki/User-Guide#segment-anything-model). Credit goes to [Bjorn Nyberg](https://github.com/BjornNyberg).
 -   **ArcGIS**: Check out the [Segment Anything Model (SAM) Toolbox for ArcGIS](https://www.arcgis.com/home/item.html?id=9b67b441f29f4ce6810979f5f0667ebe) and the [Resources for Unlocking the Power of Deep Learning Applications Using ArcGIS](https://community.esri.com/t5/education-blog/resources-for-unlocking-the-power-of-deep-learning/ba-p/1293098). Credit goes to [Esri](https://www.esri.com).
 
 ## Computing Resources
 
 The Segment Anything Model is computationally intensive, and a powerful GPU is recommended to process large datasets. It is recommended to have a GPU with at least 8 GB of GPU memory. You can utilize the free GPU resources provided by Google Colab. Alternatively, you can apply for [AWS Cloud Credit for Research](https://aws.amazon.com/government-education/research-and-technical-computing/cloud-credit-for-research), which offers cloud credits to support academic research. If you are in the Greater China region, apply for the AWS Cloud Credit [here](https://aws.amazon.com/cn/events/educate_cloud/research-credits).
 
+## Legal Notice
+
+This repository and its content are provided for educational purposes only. By using the information and code provided, users acknowledge that they are using the APIs and models at their own risk and agree to comply with any applicable laws and regulations. Users who intend to download a large number of image tiles from any basemap are advised to contact the basemap provider to obtain permission before doing so. Unauthorized use of the basemap or any of its components may be a violation of copyright laws or other applicable laws and regulations.
+
 ## Acknowledgements
 
 This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.8.3/setup.py` & `segment-geospatial-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.8.3',
+    version='0.8.4',
     zip_safe=False,
 )
```

