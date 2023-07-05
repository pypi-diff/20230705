# Comparing `tmp/courtvision-0.1.0-py3-none-any.whl.zip` & `tmp/courtvision-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,17 @@
-Zip file size: 27471 bytes, number of entries: 13
--rw-r--r--  2.0 unx      421 b- defN 80-Jan-01 00:00 courtvision/console.py
--rw-r--r--  2.0 unx    15124 b- defN 80-Jan-01 00:00 courtvision/data.py
--rw-r--r--  2.0 unx    43326 b- defN 80-Jan-01 00:00 courtvision/geometry.py
--rw-r--r--  2.0 unx     4082 b- defN 80-Jan-01 00:00 courtvision/models.py
--rw-r--r--  2.0 unx    19991 b- defN 80-Jan-01 00:00 courtvision/pipeline.py
+Zip file size: 33564 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1225 b- defN 80-Jan-01 00:00 courtvision/config.py
+-rw-r--r--  2.0 unx     2245 b- defN 80-Jan-01 00:00 courtvision/console.py
+-rw-r--r--  2.0 unx    30907 b- defN 80-Jan-01 00:00 courtvision/data.py
+-rw-r--r--  2.0 unx    47258 b- defN 80-Jan-01 00:00 courtvision/geometry.py
+-rw-r--r--  2.0 unx     5533 b- defN 80-Jan-01 00:00 courtvision/models.py
+-rw-r--r--  2.0 unx     7137 b- defN 80-Jan-01 00:00 courtvision/pipeline.py
 -rw-r--r--  2.0 unx     2280 b- defN 80-Jan-01 00:00 courtvision/swiss.py
--rw-r--r--  2.0 unx     7410 b- defN 80-Jan-01 00:00 courtvision/trackers.py
--rw-r--r--  2.0 unx     7553 b- defN 80-Jan-01 00:00 courtvision/vis.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 courtvision-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      751 b- defN 80-Jan-01 00:00 courtvision-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 courtvision-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 courtvision-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1035 b- defN 16-Jan-01 00:00 courtvision-0.1.0.dist-info/RECORD
-13 files, 103195 bytes uncompressed, 25759 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx    10385 b- defN 80-Jan-01 00:00 courtvision/trackers.py
+-rw-r--r--  2.0 unx     7559 b- defN 80-Jan-01 00:00 courtvision/trainer.py
+-rw-r--r--  2.0 unx    10646 b- defN 80-Jan-01 00:00 courtvision/vis.py
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 courtvision-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1855 b- defN 80-Jan-01 00:00 courtvision-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 courtvision-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 courtvision-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1195 b- defN 16-Jan-01 00:00 courtvision-0.2.0.dist-info/RECORD
+15 files, 129466 bytes uncompressed, 31614 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: courtvision/config.py
+Comment: 
+
 Filename: courtvision/console.py
 Comment: 
 
 Filename: courtvision/data.py
 Comment: 
 
 Filename: courtvision/geometry.py
@@ -15,26 +18,29 @@
 
 Filename: courtvision/swiss.py
 Comment: 
 
 Filename: courtvision/trackers.py
 Comment: 
 
+Filename: courtvision/trainer.py
+Comment: 
+
 Filename: courtvision/vis.py
 Comment: 
 
-Filename: courtvision-0.1.0.dist-info/LICENSE
+Filename: courtvision-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: courtvision-0.1.0.dist-info/METADATA
+Filename: courtvision-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: courtvision-0.1.0.dist-info/WHEEL
+Filename: courtvision-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: courtvision-0.1.0.dist-info/entry_points.txt
+Filename: courtvision-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: courtvision-0.1.0.dist-info/RECORD
+Filename: courtvision-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## courtvision/console.py

```diff
@@ -1,18 +1,59 @@
+import json
+from pathlib import Path
+
+import cv2
 from textual.app import App, ComposeResult
 from textual.widgets import DirectoryTree
 
-# class DirectoryTreeApp(App):
-#     def compose(self) -> ComposeResult:
-#         yield DirectoryTree("./")
-
+from courtvision.data import PadelDataset, StreamType, frames_from_clip_segments
+from courtvision.swiss import get_latest_file
 
-# if __name__ == "__main__":
-#     app = DirectoryTreeApp()
-#     app.run()
 
+def grab_frames_from_clips(
+    frame_interval: int = 6,
+    max_num_frames: int = 800,
+    output_dir: Path = Path(
+        "/Users/benjamindecharmoy/projects/courtvision/balldataset"
+    ),
+):
+    """Grabs frames from the clips in the dataset and saves every `frame_interval`th
+    frame to `output_dir` for a maximum of `max_num_frames` frames.
 
-def review():
-    """
-    Review the latest match in the database.
+    Args:
+        frame_interval (int, optional): Save every `frame_interval`. Defaults to 6.
+        max_num_frames (int, optional): Max number of frames to save. Defaults to 800.
+        output_dir (Path, optional): Frames are saved to this directory. Defaults to Path( "/Users/benjamindecharmoy/projects/courtvision/balldataset" ).
     """
-    from courtvision.models import get_fasterrcnn_ball_detection_model
+    # TODO: Add these as cli args https://github.com/BenjaminDev/courtvision/issues/10
+    ANNOTATION_PATH = Path(
+        "/Users/benjamindecharmoy/projects/courtvision/datasets/clip_segmentations"
+    )
+    ANNOTATION_DATA_PATH = Path(
+        "/Users/benjamindecharmoy/projects/courtvision/datasets/clip_segmentations/data"
+    )
+    ANNOTATION_DATA_PATH.mkdir(exist_ok=True, parents=True)
+
+    court_mesh_path = Path(
+        "/Users/benjamindecharmoy/projects/courtvision/blender/basic_image.glb"
+    )
+    output_dir.mkdir(exist_ok=True, parents=True)
+    annotations_file = get_latest_file(ANNOTATION_PATH, "json")
+    with open(annotations_file, "r") as f:
+        dataset = PadelDataset(samples=json.load(f))
+    print(f"Found {len(dataset.samples)} clips")
+    for i, (frame, uid, match_id) in enumerate(
+        frames_from_clip_segments(
+            dataset,
+            local_path=ANNOTATION_DATA_PATH,
+            stream_type=StreamType.VIDEO,
+        )
+    ):
+
+        if i % frame_interval == 0:
+            print(f"Processing frame {i} of clip {uid}")
+            cv2.imwrite(
+                (output_dir / f"{uid}_{i:04}.png").as_posix(),
+                frame["data"].permute(1, 2, 0).numpy()[:, :, ::-1],
+            )
+        if i >= max_num_frames:
+            break
```

## courtvision/data.py

```diff
@@ -1,74 +1,97 @@
+import enum
+from dataclasses import dataclass, field
+from hashlib import md5
 from pathlib import Path
-from typing import Optional, Union
+from typing import Callable, Optional, Self, Tuple, Union
 
+import cv2
+import matplotlib.pyplot as plt
 import numpy as np
-from pydantic import BaseModel, Field
+import torch
+import torchvision
+from pydantic import AliasChoices, BaseModel, Field
 from torch.utils.data import DataLoader
+from torchvision.datasets import VisionDataset
 
 from courtvision.models import BallDetector, PlayerDetector
+from courtvision.trackers import ParticleFilter
 
 
 class AnnotationDataPath(BaseModel):
-    video_url: Optional[Path]
-    video_local_path: Optional[Path]
-    image: Optional[Path] = Field(None, alias="img")
+    """Tracks the location of the data for a single data item"""
+
+    video_url: Optional[Path] = None
+    video_local_path: Optional[Path] = None
+    image_local_path: Optional[Path] = None
+    image: Optional[Path] = Field(None, validation_alias=AliasChoices("img", "image"))
+    # TODO: #1 use aliases to have a single source of truth file locations
+    #       both locally and on reomote - eg: s3
 
     class Config:
         allow_population_by_field_name = True
 
 
 class LabelValue(BaseModel):
+    """Specifies a clip segment and it's labels"""
+
     start: float
     end: float
     labels: list[str]
 
 
 class RectValue(BaseModel):
+    """Specifies a rectangle and it's labels"""
+
     x: float
     y: float
     width: float
     height: float
     rectanglelabels: list[str]
 
 
 class KeypointValue(BaseModel):
+    """Specifies a keypoint and it's labels"""
+
     x: float
     y: float
     width: float
     keypointlabels: list[str]
 
 
 class VideoRectSequence(BaseModel):
+    """Specifies a rectangle and it's labels for a frames in a sequence"""
 
     frame: int
     enabled: bool
     rotation: float
     x: float
     y: float
     width: float
     height: float
     time: float
 
 
 class VideoRectValue(BaseModel):
+    """Specifies a sequence of rectangles and it's labels"""
+
+    # TODO: rename to VideoRectSequenceValue https://github.com/BenjaminDev/courtvision/issues/11
     framesCount: int
     duration: float
     sequence: list[VideoRectSequence]
     labels: list[str]
-    # videorectangle: list[str]
 
 
 class PolygonValue(BaseModel):
     points: list[tuple[float, float]]
     polygonlabels: list[str]
 
 
 class ClipSegmentResult(BaseModel):
-    original_length: Optional[float]
+    original_length: Optional[float] = None
     clip_id: str = Field(..., alias="id")
     kind: str = Field(..., alias="type")
     value: Union[
         VideoRectValue,
         LabelValue,
     ]
 
@@ -85,45 +108,351 @@
     to_name: str = ""
     from_name: str
 
 
 class Annotation(BaseModel):
     unique_id: str
     result: Union[
-        list[ClipSegmentResult],
         list[GeneralResult],
+        list[ClipSegmentResult],
     ]
 
 
 class CourtAnnotatedSample(BaseModel):
     idx: int = Field(..., alias="id")
     data: AnnotationDataPath
     annotations: list[Annotation]
 
 
 class PadelDataset(BaseModel):
     samples: list[CourtAnnotatedSample]
+    local_data_dir: Path | None = None
 
 
-from dataclasses import dataclass, field
+@dataclass
+class CameraInfo:
+    """Camera calibration information"""
 
-from courtvision.geometry import CameraInfo, PadelCourt
+    valid_for_clip_ids: set[str]
+    camera_matrix: np.array
+    distortion_coefficients: np.array
+    rotation_vector: np.array
+    translation_vector: np.array
+    image_width: int
+    image_height: int
+    error_in_reprojected_planar_points: float
+    error_in_reprojected_points: float
+
+    def world_space_to_camera_space(self) -> torch.Tensor:
+        rotation_matrix, _ = cv2.Rodrigues(self.rotation_vector)
+        return torch.tensor(
+            np.vstack(
+                [
+                    np.hstack((rotation_matrix, self.translation_vector)),
+                    np.array([0, 0, 0, 1]),
+                ]
+            )
+        )
+
+    def save(self, file_name: Path):
+        """Saves the camera calibration information to a file
+
+        Args:
+            file_name (Path): The file to save the camera calibration information to.
+        """
+        np.savez(
+            file_name,
+            camera_matrix=self.camera_matrix,
+            distortion_coefficients=self.distortion_coefficients,
+            rotation_vector=self.rotation_vector,
+            translation_vector=self.translation_vector,
+            image_width=self.image_width,
+            image_height=self.image_height,
+            error_in_reprojected_planar_points=self.error_in_reprojected_planar_points,
+            error_in_reprojected_points=self.error_in_reprojected_points,
+            valid_for_clip_ids=self.valid_for_clip_ids,
+        )
+
+    @staticmethod
+    def load(file_name: str) -> Self:
+        """Loads the camera calibration information from a file.
+
+        Args:
+            file_name (str): Full path to .npz file
+
+        Returns:
+            CameraInfo: Camera calibration information
+        """
+        data = np.load(file_name, allow_pickle=True)
+        return CameraInfo(
+            camera_matrix=data["camera_matrix"],
+            distortion_coefficients=data["distortion_coefficients"],
+            rotation_vector=data["rotation_vector"],
+            translation_vector=data["translation_vector"],
+            image_width=data["image_width"],
+            image_height=data["image_height"],
+            error_in_reprojected_planar_points=data[
+                "error_in_reprojected_planar_points"
+            ],
+            error_in_reprojected_points=data["error_in_reprojected_points"],
+            valid_for_clip_ids=data["valid_for_clip_ids"].tolist(),
+        )
+
+
+@dataclass
+class PadelCourt:
+    """Padel court dimensions and locations of key points"""
+
+    # The scale of the court is in meters
+    # Setting this to 100.0 means that the court is 1_000cm x 2_000cm
+    court_scale: float = 10.0
+
+    # REF: https://www.lta.org.uk/4ad2a4/siteassets/play/padel/file/lta-padel-court-guidance.pdf
+    width: float = 10.0 * court_scale
+    length: float = 20.0 * court_scale
+    backwall_height: float = 3.0 * court_scale
+    backwall_fence_height: float = 4.0 * court_scale
+    serve_line_from_back_line: float = 3.0 * court_scale
+    line_width: float = 0.05 * court_scale
+    net_height: float = 0.78 * court_scale  # 0.78m
+
+    @classmethod
+    @property
+    def center_line(cls) -> np.array:
+        return np.array(
+            [
+                (cls.width / 2, cls.length - cls.serve_line_from_back_line),
+                (cls.width / 2, cls.serve_line_from_back_line),
+            ],
+            dtype=np.int32,
+        ).reshape(-1, 1, 2)
+
+    @classmethod
+    @property
+    def net_line(cls) -> np.array:
+        return np.array(
+            [(0, cls.length / 2), (cls.width, cls.length / 2)], dtype=np.int64
+        ).reshape(-1, 1, 2)
+
+    @classmethod
+    @property
+    def near_serve_line(cls):
+        return np.array(
+            [
+                (0, cls.length - cls.serve_line_from_back_line),
+                (cls.width, cls.length - cls.serve_line_from_back_line),
+            ],
+            np.int32,
+        ).reshape(-1, 1, 2)
+
+    @classmethod
+    @property
+    def far_serve_line(cls):
+        return np.array(
+            [
+                (0, cls.serve_line_from_back_line),
+                (cls.width, cls.serve_line_from_back_line),
+            ],
+            dtype=np.int32,
+        ).reshape(-1, 1, 2)
+
+    @classmethod
+    @property
+    def front_left(cls):
+        return (0.0, 0.0)
+
+    @classmethod
+    @property
+    def front_right(cls):
+        return (cls.width, 0)
+
+    @classmethod
+    @property
+    def top_front_left_vertical_plane(cls):
+        # x, z
+        return (0.0, cls.backwall_height)
+
+    @classmethod
+    @property
+    def top_front_right_vertical_plane(cls):
+        # x, z
+        return (cls.width, cls.backwall_height)
+
+    @classmethod
+    @property
+    def back_left(cls):
+        return (0.0, cls.length)
+
+    @classmethod
+    @property
+    def back_right(cls):
+        return (cls.width, cls.length)
+
+    @classmethod
+    @property
+    def left_near_serve_line(cls):
+        return (0.0, cls.serve_line_from_back_line)
+
+    @classmethod
+    @property
+    def right_near_serve_line(cls):
+        return (cls.width, cls.serve_line_from_back_line)
+
+    @classmethod
+    @property
+    def left_far_serve_line(cls):
+        return (0.0, cls.length - cls.serve_line_from_back_line)
+
+    @classmethod
+    @property
+    def right_far_serve_line(cls):
+        return (cls.width, cls.length - cls.serve_line_from_back_line)
+
+    @classmethod
+    @property
+    def m_top_front_left(cls):
+        # TODO: add thes
+        raise NotImplementedError()
+
+    @classmethod
+    @property
+    def n_top_front_right(cls):
+        raise NotImplementedError()
+
+    @classmethod
+    @property
+    def o_top_back_left(cls):
+        raise NotImplementedError()
+
+    @classmethod
+    @property
+    def p_top_back_right(cls):
+        raise NotImplementedError()
+
+    @classmethod
+    @property
+    def q_top_net_line_left(cls):
+        raise NotImplementedError()
+
+    @classmethod
+    @property
+    def r_top_net_line_right(cls):
+        raise NotImplementedError()
+
+    # Normalised:
+    @classmethod
+    @property
+    def center_line_n(cls) -> np.array:
+        return np.array(
+            [
+                ((cls.width / 2) / cls.width, cls.length / cls.length),
+                ((cls.width / 2) / cls.width, 0),
+            ],
+            dtype=np.int32,
+        ).reshape(-1, 1, 2)
+
+    @classmethod
+    @property
+    def net_line_n(cls) -> np.array:
+        return np.array(
+            [
+                (0, (cls.length / 2) / cls.length),
+                (cls.width / cls.width, (cls.length / 2) / cls.length),
+            ],
+            dtype=np.int64,
+        ).reshape(-1, 1, 2)
+
+    @classmethod
+    @property
+    def front_left_n(cls):
+        return (cls.front_left[0] / cls.width, cls.front_left[1] / cls.length)
+
+    @classmethod
+    @property
+    def front_right_n(cls):
+        return (cls.front_right[0] / cls.width, cls.front_right[1] / cls.length)
+
+    @classmethod
+    @property
+    def top_front_left_vertical_plane_n(cls):
+        # x, z
+        return (0.0, 0.0)
+
+    @classmethod
+    @property
+    def top_front_right_vertical_plane_n(cls):
+        # x, z
+        return (cls.width / cls.width, 0.0)
+
+    @classmethod
+    @property
+    def front_left_vertical_plane_n(cls):
+        # x, z
+        return (0.0, cls.backwall_height / cls.backwall_height)
+
+    @classmethod
+    @property
+    def front_right_vertical_plane_n(cls):
+        # x, z
+        return (cls.width / cls.width, cls.backwall_height / cls.backwall_height)
+
+    @classmethod
+    @property
+    def back_left_n(cls):
+        return (cls.back_left[0] / cls.width, cls.back_left[1] / cls.length)
+
+    @classmethod
+    @property
+    def back_right_n(cls):
+        return (cls.back_right[0] / cls.width, cls.back_right[1] / cls.length)
+
+    @classmethod
+    @property
+    def left_near_serve_line_n(cls):
+        return (
+            cls.left_near_serve_line[0] / cls.width,
+            cls.left_near_serve_line[1] / cls.length,
+        )
+
+    @classmethod
+    @property
+    def right_near_serve_line_n(cls):
+        return (
+            cls.right_near_serve_line[0] / cls.width,
+            cls.right_near_serve_line[1] / cls.length,
+        )
+
+    @classmethod
+    @property
+    def left_far_serve_line_n(cls):
+        return (
+            cls.left_far_serve_line[0] / cls.width,
+            cls.left_far_serve_line[1] / cls.length,
+        )
+
+    @classmethod
+    @property
+    def right_far_serve_line_n(cls):
+        return (
+            cls.right_far_serve_line[0] / cls.width,
+            cls.right_far_serve_line[1] / cls.length,
+        )
 
 
 @dataclass
 class CourtVisionArtifacts:
+    """Tracks the artifacts used in the pipeline"""
+
     local_cache_path: Path
     dataset: PadelDataset
     ball_detector: BallDetector
+    ball_tracker: ParticleFilter
     player_detector: PlayerDetector
 
     court_layout: PadelCourt
-    # court_detection_model: Path = None
-
-    # camera_info: CameraInfo
     camera_info_path: Path
     _camera_info: CameraInfo = field(init=False, default=None)
 
     @property
     def camera_info(self):
         if self._camera_info is None and self.camera_info_path.exists():
 
@@ -137,25 +466,142 @@
     def camera_info(self, value):
         self._camera_info = value
 
     class Config:
         arbitrary_types_allowed = True
 
 
-from pathlib import Path
-from typing import Callable, Optional
+class CourtVisionBallDataset(VisionDataset):
+    def __init__(
+        self,
+        dataset: PadelDataset,
+        root: str,
+        download: bool = True,
+        show: Callable | None = None,
+        load_from_disk: Callable[[Path], torch.Tensor] | None = None,
+        transforms: Callable | None = None,
+        transform: Callable | None = None,
+        target_transform: Callable | None = None,
+    ):
+        super().__init__(root, transforms, transform, target_transform)
+        # self.root = root  # TODO: See what base class does and if we can use it
+        self.dataset = dataset
+        from rich.progress import track
 
-import matplotlib.pyplot as plt
-import torch
-from torchvision.datasets import VisionDataset
+        if download:
+            for sample in track(dataset.samples, description=f"Downloading data"):
+                sample.data.image_local_path = download_data_item(
+                    s3_uri=sample.data.image,
+                    local_path=self.dataset.local_data_dir
+                    / sample.data.image.parent.name
+                    / sample.data.image.name,
+                )
 
-from courtvision.data import Annotation, CourtAnnotatedSample, KeypointValue, RectValue
-from courtvision.vis import draw_rect, load_timg
+    def __len__(self):
+        return len(self.dataset.samples)
 
+    def __getitem__(self, idx) -> tuple[CourtAnnotatedSample, torch.Tensor]:
+        from courtvision.vis import load_timg
+
+        # TODO: Data module should have IO functions injected into it
+        sample = self.dataset.samples[idx]
+        image = load_timg(sample.data.image_local_path)
+        return (
+            image,
+            sample,
+        )
 
+    @staticmethod
+    def collate_fn(batch):
+        """Collate function for the dataloader"""
+        images, samples = zip(*batch)
+
+        targets = [
+            {
+                "boxes": annotations_to_bbox(sample.annotations),
+                "labels": annotations_to_label(sample.annotations),
+                "file_location": sample.data.image_local_path.as_posix(),
+            }
+            for sample in samples
+        ]
+
+        return [o.squeeze(0) for o in images], targets
+
+    @staticmethod
+    def find_image_path(root: Path | str, sample: CourtAnnotatedSample):
+        """Finds the image path from a sample"""
+        server_file_path = Path(*sample.data.image.parts[2:])  # remove /data/
+        filename = Path(f"{root}/{server_file_path}")
+        return filename
+
+    @staticmethod
+    def show_sample(annotation: list[Annotation], image: torch.Tensor):
+        """Plots an image and its annotation"""
+        # TODO: Data module should have vis functions injected into it
+        from courtvision.vis import draw_rect
+
+        def draw_annotaion(annotation: Annotation, image: torch.Tensor):
+            bboxes = [
+                r.value for r in annotation.result if isinstance(r.value, RectValue)
+            ]
+
+            original_sizes = [
+                (r.original_width, r.original_height)
+                for r in annotation.result
+                if isinstance(r.value, RectValue)
+            ]
+            if bboxes:
+                rects = torch.stack(
+                    [
+                        torch.tensor(
+                            [
+                                (bbox.x / 100.0) * w_h[0],
+                                (bbox.y / 100.0) * w_h[1],
+                                (bbox.x + bbox.width) / 100.0 * w_h[0],
+                                (bbox.y + bbox.height) / 100.0 * w_h[1],
+                            ]
+                        ).unsqueeze(0)
+                        for bbox, w_h in zip(bboxes, original_sizes)
+                    ]
+                ).permute(1, 0, 2)
+                print(rects.shape)
+                draw_rect(image, bboxes=rects)
+
+            keypoints = [
+                r.value for r in annotation.result if isinstance(r.value, KeypointValue)
+            ]
+            original_sizes = [
+                (r.original_width, r.original_height)
+                for r in annotation.result
+                if isinstance(r.value, KeypointValue)
+            ]
+            if keypoints:
+                point_width = 1.0
+                rects = torch.stack(
+                    [
+                        torch.tensor(
+                            [
+                                (point.x / 100.0) * w_h[0],
+                                (point.y / 100.0) * w_h[1],
+                                (point.x + point_width) / 100.0 * w_h[0],
+                                (point.y + point_width) / 100.0 * w_h[1],
+                            ]
+                        ).unsqueeze(0)
+                        for point, w_h in zip(keypoints, original_sizes)
+                    ]
+                ).permute(1, 0, 2)
+
+                draw_rect(image, bboxes=rects)
+
+        for annot in annotation:
+            draw_annotaion(annot, image)
+        plt.imshow(image.squeeze(0).permute(1, 2, 0))
+
+
+# TODO: Remove CourtVisionDataset https://github.com/BenjaminDev/courtvision/issues/12
 class CourtVisionDataset(VisionDataset):
     def __init__(
         self,
         dataset: PadelDataset,
         root: str,
         transforms: Callable | None = None,
         transform: Callable | None = None,
@@ -165,48 +611,49 @@
         self.dataset = dataset
         super().__init__(root, transforms, transform, target_transform)
 
     def __len__(self):
         return len(self.dataset.samples)
 
     def __getitem__(self, idx) -> tuple[CourtAnnotatedSample, torch.Tensor]:
+        from courtvision.vis import load_timg
+
+        # TODO: Data module should have IO functions injected into it
         sample = self.dataset.samples[idx]
         image = load_timg(CourtVisionDataset.find_image_path(self.root, sample=sample))
         return (
             sample,
             image,
         )
 
     @staticmethod
     def collate_fn(batch):
         """Collate function for the dataloader"""
         samples, images = zip(*batch)
-        return samples, torch.stack(images)
+        targets = [
+            {
+                "boxes": annotations_to_bbox(sample.annotations),
+                "labels": torch.ones(1, dtype=torch.int64),
+            }
+            for sample in samples
+        ]
+
+        return targets, [o.squeeze(0) for o in images]
 
     @staticmethod
     def find_image_path(root: Path | str, sample: CourtAnnotatedSample):
-        """Finds the image path from a sample"""
-        #         root = Path(root)
-        #         dir_name, _, frame_idx = sample.data.image.stem.partition("_frame")
-        #         dir_name = dir_name.split("-", 1)[-1]
-        #         filename = root / dir_name / f"{dir_name}_frame{frame_idx}.png"
-        # # /Users/benjamindecharmoy/projects/courtvision/labelstudiodata/media/upload/1/b6f5d028-Highlights-TOLITO-AGUIRRE---TITO-ALLEMANDI-vs-CHIOSTRI---MELGRATTI--Sa_Lwr6ooR.png
-        #         if not filename.exists():
-        #             print(f"{filename=} \n{root=}!")
-        #             print(f"{sample.data.image=}")
-        #             raise Exception("Could not find image")
-        #         return filename
         server_file_path = Path(*sample.data.image.parts[2:])  # remove /data/
         filename = Path(f"{root}/{server_file_path}")
-        # print(f"{filename=}")
         return filename
 
     @staticmethod
     def show_sample(annotation: list[Annotation], image: torch.Tensor):
         """Plots an image and its annotation"""
+        # TODO: Data module should have vis functions injected into it
+        from courtvision.vis import draw_rect
 
         def draw_annotaion(annotation: Annotation, image: torch.Tensor):
             bboxes = [
                 r.value for r in annotation.result if isinstance(r.value, RectValue)
             ]
 
             original_sizes = [
@@ -258,31 +705,61 @@
                 draw_rect(image, bboxes=rects)
 
         for annot in annotation:
             draw_annotaion(annot, image)
         plt.imshow(image.squeeze(0).permute(1, 2, 0))
 
 
-def annotations_to_bbox(annotations: list[Annotation]):
+def annotations_to_label(annotations: list[Annotation]) -> torch.IntTensor:
+    """Grab the labels from the annotations
+    !!! note
+        Currently only supports a single label and rects only!
+
+    Args:
+        annotations (list[Annotation]): Annotations from the dataset.
+
+    Returns:
+        torch.IntTensor: A tensor of labels.
+    """
+    labels = []
+    for annotation in annotations:
+        labels.extend(
+            [
+                r.value.rectanglelabels[0]
+                for r in annotation.result
+                if isinstance(r.value, RectValue)
+            ]
+        )
+
+    return torch.ones(len(labels), dtype=torch.int64)
+
+
+def annotations_to_bbox(annotations: list[Annotation]) -> torch.Tensor:
+    """Grab the bounding boxes from the annotations.
+    !!! note
+        Coordinates are in image coordinates and *not* normalised coordinates.
+    Args:
+        annotations (list[Annotation]): Annotations from the dataset.
+
+    Returns:
+        torch.Tensor: A tensor of bounding boxes in image coordinates.
+    """ """"""
     bboxes = []
     original_sizes = []
     for annotation in annotations:
         bboxes.extend(
             [r.value for r in annotation.result if isinstance(r.value, RectValue)]
         )
         original_sizes.extend(
             [
                 (r.original_width, r.original_height)
                 for r in annotation.result
                 if isinstance(r.value, RectValue)
             ]
         )
-    # if not bboxes:
-    # raise ValueError("No bounding boxes in annotation")
-
     return torch.stack(
         [
             torch.tensor(
                 [
                     (bbox.x / 100.0) * w_h[0],
                     (bbox.y / 100.0) * w_h[1],
                     (bbox.x + bbox.width) / 100.0 * w_h[0],
@@ -305,17 +782,27 @@
         for sample in samples
     ]
 
     return targets, [o.squeeze(0) for o in images]
 
 
 def validate_dataloader(dataloader: DataLoader):
-    for (targets, images) in dataloader:
+    """Runs over all items in a dataloader and validates the annotations.
+
+    Args:
+        dataloader (DataLoader): A dataloader with a collate_fn that returns a
+                                list of annotations and a list of images.
+    """ """"""
+    for (images, targets) in dataloader:
         assert all(o["boxes"].shape for o in targets)
         assert all(o.shape for o in images)
+        for image, target in zip(images, targets):
+            height, width = image.shape[1:]
+            assert all(x > 0 and x < width for x in target["boxes"][0][::2])
+            assert all(y > 0 and y < height for y in target["boxes"][0][1::2])
 
 
 def get_keypoints_as_dict(
     results: list[GeneralResult],
 ) -> dict[str, tuple[float, float]]:
     """Go through the results and return a dict of keypoints
 
@@ -346,16 +833,31 @@
     Returns:
         np.array, list[str]: Nx2 array of points and list of labels
     """
     keypoints = dict(sorted(keypoints.items(), key=lambda x: x[0]))
     return np.array(list(keypoints.values())).astype(np.float32), list(keypoints.keys())
 
 
-def download_data_item(s3_uri: str, local_path: Path, s3_client=None, use_cached=True):
+def download_data_item(
+    s3_uri: str, local_path: Path, s3_client=None, use_cached=True
+) -> Path:
+    """
+
+    !!! note
+        `courtvision-padel-dataset` profile must be configured in ~/.aws/credentials
+
+    Args:
+        s3_uri (str): S3 uri to file
+        local_path (Path): Path to file on local filesystem
+        s3_client (_type_, optional): A suitable s3_client (access to s3). Defaults to None.
+        use_cached (bool, optional): If True and the file exists uses the one on disk. Defaults to True.
 
+    Returns:
+        Path: Path to the data item on local filesystem
+    """
     if use_cached and local_path.exists():
         return local_path
 
     if s3_client is None:
         import boto3
 
         session = boto3.Session(profile_name="courtvision-padel-dataset")
@@ -365,47 +867,43 @@
     local_path.parent.mkdir(parents=True, exist_ok=True)
 
     with open(local_path, "wb") as fp:
         s3_client.download_fileobj(bucket_name, object_name, fp)
     return local_path
 
 
-import enum
-from hashlib import md5
-
-import torchvision
-
-
 class StreamType(enum.Enum):
     VIDEO = "video"
     AUDIO = "image"
 
 
 def frames_from_clip_segments(
-    dataset: PadelDataset, local_path: Path, stream_type: StreamType = StreamType.VIDEO
-) -> tuple[dict[str, torch.Tensor], str]:
+    dataset: PadelDataset,
+    local_path: Path,
+    stream_type: StreamType = StreamType.VIDEO,
+) -> Tuple[dict[str, torch.Tensor], str]:
     """
     Graps frames for each clip segment in the dataset. A unique id is generated for each clip segment.
     Frames can be either audio or video frames.
 
     Args:
         dataset (PadelDataset): A dataset of annotated clips
         local_path (Path): if the file is not already downloaded, it will be downloaded to this path
         stream_type (StreamType, optional): Either `StreamType.VIDEO` or `StreamType.AUDIO`. Defaults to StreamType.VIDEO.
 
-    Returns:
-        tuple[dict[str, torch.Tensor], str]: returns `{"data": torch.Tensor, "pts": torch.Tensor}, unique_id`
-
+    Yields:
+        `{"data": torch.Tensor, "pts": torch.Tensor}, unique_id, match_id`
         where `unique_id` is the md5 of the annotation unique_id and the start and end times of the clip.
         And `pts` is a presentation timestamp of the frame expressed in seconds.
-
-    Yields:
-        Iterator[tuple[dict[str, torch.Tensor], str]]: yeilds `{"data": torch.Tensor, "pts": torch.Tensor}, unique_id`
+        `match_id` is the parent folder of the clip.
     """
-    for sample in dataset.samples:
+    from rich.progress import track
+
+    for sample in track(dataset.samples, description=f"Downloading data"):
+        # for sample in dataset.samples:
         sample.data.video_local_path = download_data_item(
             s3_uri=sample.data.video_url,
             local_path=local_path
             / sample.data.video_url.parent.name
             / sample.data.video_url.name,
         )
     for sample in dataset.samples:
@@ -414,35 +912,41 @@
                 if isinstance(result.value, LabelValue):
                     start_time = result.value.start
                     end_time = result.value.end
                     reader = torchvision.io.VideoReader(
                         sample.data.video_local_path.as_posix(), stream_type.value
                     )
                     reader.seek(start_time)
+                try:
                     while frame := next(reader):
                         if frame["pts"] < start_time:
                             # seeks is not always accuarte!
                             # burn frames until we get to the right time.
-                            # Alternative - build torchvison from source with video_reader backend
+                            # Alternative - build torchvision from source with video_reader backend
                             continue
                         if frame["pts"] > end_time:
                             break
                         yield frame, md5(
                             f"{start_time}{end_time}{annotation.unique_id}".encode()
-                        ).hexdigest()
+                        ).hexdigest(), f"{sample.data.video_local_path.parent.name}"
+                except Exception as e:
+                    print(f"{sample.data.video_local_path=} has invalid data {e=}")
+                    continue
 
 
 def get_normalized_calibration_image_points_and_clip_ids(
     dataset: PadelDataset,
 ) -> tuple[dict[str, tuple[float, float]], set[str]]:
     """
-    Note: This assumes that the calibration points are the only annotations with a VideoRectValue
-    and the points of the same label are in the same place as the last one which will be used.
+    !!! note
+        This assumes that the calibration points are the only annotations with a VideoRectValue
+        and the points of the same label are in the same place as the last one which will be used.
 
-    Note: Points are normalized to 0-1. Not -1 to 1 like in kornia.
+    !!! note
+        Points are normalized to 0-1. Not -1 to 1 like in kornia.
     Args:
         dataset (PadelDataset): Dataset descibing a video with calibration points.
 
     Returns:
         image_points (dict[str, tuple[float, float]]): Returns a dict of image points in normalized coordinates. And
         the clip_ids (set[str]) that are accociated with the calibration points.
     """
```

## courtvision/geometry.py

```diff
@@ -1,267 +1,250 @@
 from dataclasses import dataclass
+from itertools import chain, combinations, product
+from pathlib import Path
+from typing import Literal
 
+import cv2
 import numpy as np
+import structlog
 
-court_scale = 10
-
-
-@dataclass
-class PadelCourt:
-    # REF: https://www.lta.org.uk/4ad2a4/siteassets/play/padel/file/lta-padel-court-guidance.pdf
-    width: float = 10.0 * court_scale
-    length: float = 20.0 * court_scale
-    backwall_height: float = 3.0 * court_scale
-    backall_fence_height: float = 4.0 * court_scale
-    serve_line_from_back_line: float = 3.0 * court_scale
-    line_width: float = 0.05 * court_scale
-    net_height: float = 0.78 * court_scale  # 0.78m
-
-    @classmethod
-    @property
-    def center_line(cls) -> np.array:
-        return np.array(
-            [
-                (cls.width / 2, cls.length - cls.serve_line_from_back_line),
-                (cls.width / 2, cls.serve_line_from_back_line),
-            ],
-            dtype=np.int32,
-        ).reshape(-1, 1, 2)
-
-    @classmethod
-    @property
-    def net_line(cls) -> np.array:
-        return np.array(
-            [(0, cls.length / 2), (cls.width, cls.length / 2)], dtype=np.int64
-        ).reshape(-1, 1, 2)
-
-    @classmethod
-    @property
-    def near_serve_line(cls):
-        return np.array(
-            [
-                (0, cls.length - cls.serve_line_from_back_line),
-                (cls.width, cls.length - cls.serve_line_from_back_line),
-            ],
-            np.int32,
-        ).reshape(-1, 1, 2)
-
-    @classmethod
-    @property
-    def far_serve_line(cls):
-        return np.array(
-            [
-                (0, cls.serve_line_from_back_line),
-                (cls.width, cls.serve_line_from_back_line),
-            ],
-            dtype=np.int32,
-        ).reshape(-1, 1, 2)
-
-    @classmethod
-    @property
-    def front_left(cls):
-        return (0.0, 0.0)
-
-    @classmethod
-    @property
-    def front_right(cls):
-        return (cls.width, 0)
-
-    @classmethod
-    @property
-    def top_front_left_vertical_plane(cls):
-        # x, z
-        return (0.0, cls.backwall_height)
-
-    @classmethod
-    @property
-    def top_front_right_vertical_plane(cls):
-        # x, z
-        return (cls.width, cls.backwall_height)
-
-    @classmethod
-    @property
-    def back_left(cls):
-        return (0.0, cls.length)
-
-    @classmethod
-    @property
-    def back_right(cls):
-        return (cls.width, cls.length)
-
-    @classmethod
-    @property
-    def left_near_serve_line(cls):
-        return (0.0, cls.serve_line_from_back_line)
-
-    @classmethod
-    @property
-    def right_near_serve_line(cls):
-        return (cls.width, cls.serve_line_from_back_line)
-
-    @classmethod
-    @property
-    def left_far_serve_line(cls):
-        return (0.0, cls.length - cls.serve_line_from_back_line)
-
-    @classmethod
-    @property
-    def right_far_serve_line(cls):
-        return (cls.width, cls.length - cls.serve_line_from_back_line)
-
-    @classmethod
-    @property
-    def m_top_front_left(cls):
-        # TODO: add thes
-        raise NotImplementedError()
-
-    @classmethod
-    @property
-    def n_top_front_right(cls):
-        raise NotImplementedError()
-
-    @classmethod
-    @property
-    def o_top_back_left(cls):
-        raise NotImplementedError()
-
-    @classmethod
-    @property
-    def p_top_back_right(cls):
-        raise NotImplementedError()
-
-    @classmethod
-    @property
-    def q_top_net_line_left(cls):
-        raise NotImplementedError()
-
-    @classmethod
-    @property
-    def r_top_net_line_right(cls):
-        raise NotImplementedError()
-
-    # Normalised:
-    @classmethod
-    @property
-    def center_line_n(cls) -> np.array:
-        return np.array(
-            [
-                ((cls.width / 2) / cls.width, cls.length / cls.length),
-                ((cls.width / 2) / cls.width, 0),
-            ],
-            dtype=np.int32,
-        ).reshape(-1, 1, 2)
-
-    @classmethod
-    @property
-    def net_line_n(cls) -> np.array:
-        return np.array(
-            [
-                (0, (cls.length / 2) / cls.length),
-                (cls.width / cls.width, (cls.length / 2) / cls.length),
-            ],
-            dtype=np.int64,
-        ).reshape(-1, 1, 2)
-
-    @classmethod
-    @property
-    def front_left_n(cls):
-        return (cls.front_left[0] / cls.width, cls.front_left[1] / cls.length)
-
-    @classmethod
-    @property
-    def front_right_n(cls):
-        return (cls.front_right[0] / cls.width, cls.front_right[1] / cls.length)
-
-    @classmethod
-    @property
-    def top_front_left_vertical_plane_n(cls):
-        # x, z
-        return (0.0, 0.0)
-
-    @classmethod
-    @property
-    def top_front_right_vertical_plane_n(cls):
-        # x, z
-        return (cls.width / cls.width, 0.0)
-
-    @classmethod
-    @property
-    def front_left_vertical_plane_n(cls):
-        # x, z
-        return (0.0, cls.backwall_height / cls.backwall_height)
-
-    @classmethod
-    @property
-    def front_right_vertical_plane_n(cls):
-        # x, z
-        return (cls.width / cls.width, cls.backwall_height / cls.backwall_height)
-
-    @classmethod
-    @property
-    def back_left_n(cls):
-        return (cls.back_left[0] / cls.width, cls.back_left[1] / cls.length)
-
-    @classmethod
-    @property
-    def back_right_n(cls):
-        return (cls.back_right[0] / cls.width, cls.back_right[1] / cls.length)
-
-    @classmethod
-    @property
-    def left_near_serve_line_n(cls):
-        return (
-            cls.left_near_serve_line[0] / cls.width,
-            cls.left_near_serve_line[1] / cls.length,
-        )
-
-    @classmethod
-    @property
-    def right_near_serve_line_n(cls):
-        return (
-            cls.right_near_serve_line[0] / cls.width,
-            cls.right_near_serve_line[1] / cls.length,
-        )
-
-    @classmethod
-    @property
-    def left_far_serve_line_n(cls):
-        return (
-            cls.left_far_serve_line[0] / cls.width,
-            cls.left_far_serve_line[1] / cls.length,
-        )
-
-    @classmethod
-    @property
-    def right_far_serve_line_n(cls):
-        return (
-            cls.right_far_serve_line[0] / cls.width,
-            cls.right_far_serve_line[1] / cls.length,
-        )
-
-    # a_front_left
-    # b_front_right
-    # c_back_left
-    # d_back_right
-    # e_left_near_serve_line
-    # f_right_near_serve_line
-    # g_left_far_serve_line
-    # h_right_far_serve_line
-    # i_center_line_far
-    # j_net_line_left
-    # k_center_line_right
-    # l_net_line_right
-
-    # m_top_front_left
-    # n_top_front_right
-    # o_top_back_left
-    # p_top_back_right
-    # q_top_net_line_left
-    # r_top_net_line_right
+from courtvision.data import CameraInfo, PadelCourt
 
+# @dataclass
+# class PadelCourt:
+#     # REF: https://www.lta.org.uk/4ad2a4/siteassets/play/padel/file/lta-padel-court-guidance.pdf
+#     width: float = 10.0 * court_scale
+#     length: float = 20.0 * court_scale
+#     backwall_height: float = 3.0 * court_scale
+#     backall_fence_height: float = 4.0 * court_scale
+#     serve_line_from_back_line: float = 3.0 * court_scale
+#     line_width: float = 0.05 * court_scale
+#     net_height: float = 0.78 * court_scale  # 0.78m
+
+#     @classmethod
+#     @property
+#     def center_line(cls) -> np.array:
+#         return np.array(
+#             [
+#                 (cls.width / 2, cls.length - cls.serve_line_from_back_line),
+#                 (cls.width / 2, cls.serve_line_from_back_line),
+#             ],
+#             dtype=np.int32,
+#         ).reshape(-1, 1, 2)
+
+#     @classmethod
+#     @property
+#     def net_line(cls) -> np.array:
+#         return np.array(
+#             [(0, cls.length / 2), (cls.width, cls.length / 2)], dtype=np.int64
+#         ).reshape(-1, 1, 2)
+
+#     @classmethod
+#     @property
+#     def near_serve_line(cls):
+#         return np.array(
+#             [
+#                 (0, cls.length - cls.serve_line_from_back_line),
+#                 (cls.width, cls.length - cls.serve_line_from_back_line),
+#             ],
+#             np.int32,
+#         ).reshape(-1, 1, 2)
+
+#     @classmethod
+#     @property
+#     def far_serve_line(cls):
+#         return np.array(
+#             [
+#                 (0, cls.serve_line_from_back_line),
+#                 (cls.width, cls.serve_line_from_back_line),
+#             ],
+#             dtype=np.int32,
+#         ).reshape(-1, 1, 2)
+
+#     @classmethod
+#     @property
+#     def front_left(cls):
+#         return (0.0, 0.0)
+
+#     @classmethod
+#     @property
+#     def front_right(cls):
+#         return (cls.width, 0)
+
+#     @classmethod
+#     @property
+#     def top_front_left_vertical_plane(cls):
+#         # x, z
+#         return (0.0, cls.backwall_height)
+
+#     @classmethod
+#     @property
+#     def top_front_right_vertical_plane(cls):
+#         # x, z
+#         return (cls.width, cls.backwall_height)
+
+#     @classmethod
+#     @property
+#     def back_left(cls):
+#         return (0.0, cls.length)
+
+#     @classmethod
+#     @property
+#     def back_right(cls):
+#         return (cls.width, cls.length)
+
+#     @classmethod
+#     @property
+#     def left_near_serve_line(cls):
+#         return (0.0, cls.serve_line_from_back_line)
+
+#     @classmethod
+#     @property
+#     def right_near_serve_line(cls):
+#         return (cls.width, cls.serve_line_from_back_line)
+
+#     @classmethod
+#     @property
+#     def left_far_serve_line(cls):
+#         return (0.0, cls.length - cls.serve_line_from_back_line)
+
+#     @classmethod
+#     @property
+#     def right_far_serve_line(cls):
+#         return (cls.width, cls.length - cls.serve_line_from_back_line)
+
+#     @classmethod
+#     @property
+#     def m_top_front_left(cls):
+#         # TODO: add thes
+#         raise NotImplementedError()
+
+#     @classmethod
+#     @property
+#     def n_top_front_right(cls):
+#         raise NotImplementedError()
+
+#     @classmethod
+#     @property
+#     def o_top_back_left(cls):
+#         raise NotImplementedError()
+
+#     @classmethod
+#     @property
+#     def p_top_back_right(cls):
+#         raise NotImplementedError()
+
+#     @classmethod
+#     @property
+#     def q_top_net_line_left(cls):
+#         raise NotImplementedError()
+
+#     @classmethod
+#     @property
+#     def r_top_net_line_right(cls):
+#         raise NotImplementedError()
+
+#     # Normalised:
+#     @classmethod
+#     @property
+#     def center_line_n(cls) -> np.array:
+#         return np.array(
+#             [
+#                 ((cls.width / 2) / cls.width, cls.length / cls.length),
+#                 ((cls.width / 2) / cls.width, 0),
+#             ],
+#             dtype=np.int32,
+#         ).reshape(-1, 1, 2)
+
+#     @classmethod
+#     @property
+#     def net_line_n(cls) -> np.array:
+#         return np.array(
+#             [
+#                 (0, (cls.length / 2) / cls.length),
+#                 (cls.width / cls.width, (cls.length / 2) / cls.length),
+#             ],
+#             dtype=np.int64,
+#         ).reshape(-1, 1, 2)
+
+#     @classmethod
+#     @property
+#     def front_left_n(cls):
+#         return (cls.front_left[0] / cls.width, cls.front_left[1] / cls.length)
+
+#     @classmethod
+#     @property
+#     def front_right_n(cls):
+#         return (cls.front_right[0] / cls.width, cls.front_right[1] / cls.length)
+
+#     @classmethod
+#     @property
+#     def top_front_left_vertical_plane_n(cls):
+#         # x, z
+#         return (0.0, 0.0)
+
+#     @classmethod
+#     @property
+#     def top_front_right_vertical_plane_n(cls):
+#         # x, z
+#         return (cls.width / cls.width, 0.0)
+
+#     @classmethod
+#     @property
+#     def front_left_vertical_plane_n(cls):
+#         # x, z
+#         return (0.0, cls.backwall_height / cls.backwall_height)
+
+#     @classmethod
+#     @property
+#     def front_right_vertical_plane_n(cls):
+#         # x, z
+#         return (cls.width / cls.width, cls.backwall_height / cls.backwall_height)
+
+#     @classmethod
+#     @property
+#     def back_left_n(cls):
+#         return (cls.back_left[0] / cls.width, cls.back_left[1] / cls.length)
+
+#     @classmethod
+#     @property
+#     def back_right_n(cls):
+#         return (cls.back_right[0] / cls.width, cls.back_right[1] / cls.length)
+
+#     @classmethod
+#     @property
+#     def left_near_serve_line_n(cls):
+#         return (
+#             cls.left_near_serve_line[0] / cls.width,
+#             cls.left_near_serve_line[1] / cls.length,
+#         )
+
+#     @classmethod
+#     @property
+#     def right_near_serve_line_n(cls):
+#         return (
+#             cls.right_near_serve_line[0] / cls.width,
+#             cls.right_near_serve_line[1] / cls.length,
+#         )
+
+#     @classmethod
+#     @property
+#     def left_far_serve_line_n(cls):
+#         return (
+#             cls.left_far_serve_line[0] / cls.width,
+#             cls.left_far_serve_line[1] / cls.length,
+#         )
+
+#     @classmethod
+#     @property
+#     def right_far_serve_line_n(cls):
+#         return (
+#             cls.right_far_serve_line[0] / cls.width,
+#             cls.right_far_serve_line[1] / cls.length,
+#         )
 
 corners_world = {
     "a_front_left": PadelCourt.front_left,
     "b_front_right": PadelCourt.front_right,
     "c_back_left": PadelCourt.back_left,
     "d_back_right": PadelCourt.back_right,
     "e_left_near_serve_line": PadelCourt.left_near_serve_line,
@@ -300,21 +283,21 @@
     ),
     "s_top_net_center": (
         PadelCourt.width / 2,
         PadelCourt.length / 2,
         PadelCourt.net_height,
     ),
     "t_center_center": (PadelCourt.width / 2, PadelCourt.length / 2, 0),
-    "u_topfence_front_left": (0, 0, PadelCourt.backall_fence_height),
-    "v_topfence_front_right": (PadelCourt.width, 0, PadelCourt.backall_fence_height),
-    "w_topfence_back_left": (0, PadelCourt.length, PadelCourt.backall_fence_height),
+    "u_topfence_front_left": (0, 0, PadelCourt.backwall_fence_height),
+    "v_topfence_front_right": (PadelCourt.width, 0, PadelCourt.backwall_fence_height),
+    "w_topfence_back_left": (0, PadelCourt.length, PadelCourt.backwall_fence_height),
     "x_topfence_back_right": (
         PadelCourt.width,
         PadelCourt.length,
-        PadelCourt.backall_fence_height,
+        PadelCourt.backwall_fence_height,
     ),
     "y_top_center_left": (0, PadelCourt.length / 2, PadelCourt.backwall_height),
     "z_top_center_right": (
         PadelCourt.width,
         PadelCourt.length / 2,
         PadelCourt.backwall_height,
     ),
@@ -397,22 +380,34 @@
 from kornia.geometry.homography import (
     convert_points_from_homogeneous,
     convert_points_to_homogeneous,
 )
 
 
 def project_points_to_base_plane(points: torch.tensor, H: torch.tensor) -> torch.tensor:
+    """Given homogeneous points or 2D points and a homography, project the points to the base plane
+
+    Args:
+        points (torch.tensor): Homogeneous points or 2D points
+        H (torch.tensor): Homography 3x3 matrix
+
+    Raises:
+        ValueError: If `points` is not of length 2 or 3
+
+    Returns:
+        torch.tensor: Projected points in either homogeneous or 2D corrdinates. Same as `points`
+    """
     if len(points.shape) == 2:
         return convert_points_from_homogeneous(
             convert_points_to_homogeneous(points) @ H.T
         )
     elif len(points.shape) == 3:
         return points @ H.T
     else:
-        raise RuntimeError(f"{points.shape=} must be of length 2 or 3.")
+        raise ValueError(f"{points.shape=} must be of length 2 or 3.")
 
 
 def convert_corners_to_vec(corners: dict) -> dict:
     """Convert `corners_world_xx_n` to a dict of vectors
 
     Args:
         corners (dict):
@@ -495,18 +490,14 @@
                 (vec["z"][10], vec["z"][11]),
             ]
         )
 
     return {"xs": xs, "ys": ys, "zs": zs}
 
 
-from pathlib import Path
-from typing import Literal
-
-
 def get_corners_verital_plane_on_image(
     file_name: str, plane: Literal["front", "back"]
 ) -> dict:
     file_path = Path(file_name)
     frame_name = "/".join([file_path.parent.name, file_path.stem])
     annotated_images = {
         "curated_001/curated_001_frame_0001": {
@@ -782,20 +773,17 @@
                 (47.97507788161994 / 100.0),
             ),
         }
     }
     return annotated_images[frame_name]
 
 
-import cv2
-
-from courtvision.vis import load_timg
-
-
 def compute_homography(annotated_frame, src_corners_n, dst_corners_n):
+    from courtvision.vis import load_timg
+
     src_img_t = load_timg(annotated_frame)
     src_img = src_img_t.squeeze(0).numpy().transpose(1, 2, 0)
     src_img_height, src_img_width, _ = src_img.shape
     dst_points = torch.tensor(
         [
             (x, PadelCourt.length - y)
             for x, y in zip(
@@ -817,14 +805,17 @@
         raise AssertionError(f"{dst_points.shape=} must equal {src_points.shape=}")
     homography, _ = cv2.findHomography(src_points.numpy(), dst_points.numpy())
     # TODO: compute distortion and intrnics
     return homography, None, None
 
 
 def compute_homography_to_vertical_plane(annotated_frame, src_corners_n, dst_corners_n):
+    # TODO: geometry modulke should not be doing IO
+    from courtvision.vis import load_timg
+
     src_img_t = load_timg(annotated_frame)
     src_img = src_img_t.squeeze(0).numpy().transpose(1, 2, 0)
     src_img_height, src_img_width, _ = src_img.shape
     dst_points = torch.tensor(
         [
             (x, y)
             for x, y in zip(
@@ -1072,66 +1063,14 @@
             object_points[:, [i for i in range(3) if i != common_axis]],
             np.zeros((object_points.shape[0], 1)),
         ],
         axis=1,
     ).astype(np.float32)
 
 
-@dataclass
-class CameraInfo:
-    valid_for_clip_ids: set[str]
-    camera_matrix: np.array
-    distortion_coefficients: np.array
-    rotation_vector: np.array
-    translation_vector: np.array
-    image_width: int
-    image_height: int
-    error_in_reprojecred_planar_points: float
-    error_in_reprojecred_points: float
-
-    def save(self, file_name: Path):
-        import numpy as np
-
-        # if isinstance(file_name, Path):
-        #     _file_name = file_name.parent /f"error_{self.error_in_reprojecred_points:02f}{file_name.stem}.npz"
-        # else:
-        #     raise NotImplementedError()
-        np.savez(
-            file_name,
-            camera_matrix=self.camera_matrix,
-            distortion_coefficients=self.distortion_coefficients,
-            rotation_vector=self.rotation_vector,
-            translation_vector=self.translation_vector,
-            image_width=self.image_width,
-            image_height=self.image_height,
-            error_in_reprojecred_planar_points=self.error_in_reprojecred_planar_points,
-            error_in_reprojecred_points=self.error_in_reprojecred_points,
-            valid_for_clip_ids=self.valid_for_clip_ids,
-        )
-
-    @staticmethod
-    def load(file_name: str):
-        import numpy as np
-
-        data = np.load(file_name, allow_pickle=True)
-        return CameraInfo(
-            camera_matrix=data["camera_matrix"],
-            distortion_coefficients=data["distortion_coefficients"],
-            rotation_vector=data["rotation_vector"],
-            translation_vector=data["translation_vector"],
-            image_width=data["image_width"],
-            image_height=data["image_height"],
-            error_in_reprojecred_planar_points=data[
-                "error_in_reprojecred_planar_points"
-            ],
-            error_in_reprojecred_points=data["error_in_reprojecred_points"],
-            valid_for_clip_ids=data["valid_for_clip_ids"].tolist(),
-        )
-
-
 def calibrate_and_evaluate(
     valid_clip_ids: set[str],
     *,
     calibration_correspondences_selected,
     pose_correspondences_selected,
     image_width,
     image_height,
@@ -1186,22 +1125,105 @@
     return CameraInfo(
         camera_matrix=optimal_camera_matrix,
         distortion_coefficients=dist_coeffs,
         rotation_vector=rvec,
         translation_vector=tvec,
         image_width=image_width,
         image_height=image_height,
-        error_in_reprojecred_planar_points=repo_erro,
-        error_in_reprojecred_points=reprojection_error,
+        error_in_reprojected_planar_points=repo_erro,
+        error_in_reprojected_points=reprojection_error,
         valid_for_clip_ids=valid_clip_ids,
     )
 
 
-from dataclasses import dataclass
-from itertools import chain, combinations, product
+from typing import Any, Optional
+
+from courtvision.data import (
+    CourtVisionArtifacts,
+    StreamType,
+    dict_to_points,
+    frames_from_clip_segments,
+    get_normalized_calibration_image_points_and_clip_ids,
+)
+
+
+def calibrate_camera(
+    artifacts: CourtVisionArtifacts, logger: Optional[Any] = None
+) -> CourtVisionArtifacts:
+    if logger is None:
+        logger = structlog.get_logger(__name__)
+
+    if artifacts.camera_info:
+        logger.info(
+            "Camera already calibrated - using supplied camera_info",
+            camera_info=artifacts.camera_info,
+        )
+        return artifacts
+    if artifacts.camera_info_path.is_file():
+        artifacts.camera_info = CameraInfo.load(artifacts.camera_info_path)
+        logger.info(
+            "Camera already calibrated - using cached version",
+            camera_info=artifacts.camera_info,
+        )
+        return artifacts
+
+    frame, uid = next(
+        frames_from_clip_segments(
+            artifacts.dataset,
+            local_path=artifacts.local_cache_path,
+            stream_type=StreamType.VIDEO,
+        )
+    )
+
+    image_width, image_height = frame["data"].shape[2], frame["data"].shape[1]
+    logger.info(
+        "Calibrating camera using:", image_width=image_width, image_height=image_height
+    )
+    if image_height < 100 or image_width < 100:
+        logger.warn("Image dimensions look wrong! Check it out.")
+
+    (
+        normalised_named_points,
+        valid_clip_ids,
+    ) = get_normalized_calibration_image_points_and_clip_ids(artifacts.dataset)
+    calibration_image_points = denormalize_as_named_points(
+        normalised_named_points=normalised_named_points,
+        image_width=image_width,
+        image_height=image_height,
+    )
+
+    calibration_correspondences = get_planar_point_correspondences(
+        image_points=calibration_image_points,
+        world_points=corners_world_3d.copy(),
+        minimal_set_count=4,
+    )
+
+    pose_correspondences = get_planar_point_correspondences(
+        image_points=calibration_image_points,
+        world_points=corners_world_3d.copy(),
+        minimal_set_count=6,
+    )
+
+    all_world_points, all_labels = dict_to_points(corners_world_3d.copy())
+    all_image_points, _ = dict_to_points(calibration_image_points.copy())
+    logger.info("Calibrating camera...")
+
+    camera_info = find_optimal_calibration_and_pose(
+        valid_clip_ids=valid_clip_ids,
+        calibration_correspondences=calibration_correspondences,
+        pose_correspondences=pose_correspondences,
+        image_height=image_height,
+        image_width=image_width,
+        all_image_points=all_image_points,
+        all_world_points=all_world_points,
+    )
+    logger.info("Calibrated camera", camera_info=camera_info)
+    artifacts.camera_info = camera_info
+    artifacts.camera_info.save(artifacts.camera_info_path)
+    return artifacts
 
 
 def find_optimal_calibration_and_pose(
     valid_clip_ids: set[str],
     calibration_correspondences: list[tuple[np.array, np.array]],
     pose_correspondences: list[tuple[np.array, np.array]],
     image_width: int,
@@ -1248,15 +1270,15 @@
     pose_selected_pairs: list[tuple[int, ...]] = list(
         chain.from_iterable(
             (combinations(pose_indexes, num_pairs_to_use))
             for num_pairs_to_use in range(POSE_MIN_PAIRS, POSE_MAX_PAIRS)
         )
     )
 
-    best_error_in_reprojecred_points = 10000.0
+    best_error_in_reprojected_points = 10000.0
     best_camera_info = None
 
     for calibration_pair, pose_pair in product(
         calibration_selected_pairs, pose_selected_pairs
     ):
         calibration_correspondences_selection = [
             calibration_correspondences[o] for o in calibration_pair
@@ -1268,18 +1290,77 @@
             calibration_correspondences_selected=calibration_correspondences_selection,
             pose_correspondences_selected=pose_correspondences_selection,
             image_width=image_width,
             image_height=image_height,
             all_image_points=all_image_points,
             all_world_points=all_world_points,
         )
-        if camera_info.error_in_reprojecred_points < best_error_in_reprojecred_points:
+        if camera_info.error_in_reprojected_points < best_error_in_reprojected_points:
             best_camera_info = camera_info
     if best_camera_info is None:
         raise RuntimeError("Failed to find optimal calibration and pose")
     return best_camera_info
 
 
-if __name__ == "__main__":
-    import rerun as rr
+def camera_space_to_world_space(
+    camera_point: np.array,
+    translation_vector: np.array,
+    rotation_vector: np.array,
+) -> np.array:
+    """Transform a point from camera space to world space.
+
+    Args:
+        camera_point (np.array): 3D point in camera space with shape (3,)
+        translation_vector (np.array): Translation vector of the camera with shape (3,)
+        rotation_vector (np.array): Rotation vector of the camera with shape (3,)
+
+    Raises:
+        ValueError: If the camera point is not a 3D point with shape (3,)
+
+    Returns:
+        np.array: 3D point in world space with shape (3,)
+    """
+    if not camera_point.shape[0] == 3:
+        raise ValueError("Camera point must be a 3D point with shape (3,)")
+    R, _ = cv2.Rodrigues(rotation_vector)
+    world_point = (R.T @ (camera_point - translation_vector)).T
+    return world_point
+
+
+def compute_ray_intersecting_plane(
+    point_a_on_ray: np.array,
+    point_b_on_ray: np.array,
+    plane_normal: np.array = np.array([[0, 0, 1]]),
+    plane_point: np.array = np.array([0, 0, 0]),
+):
+    """Given two points on a ray, compute the point of intersection with a plane.
+    The plane is defined as a normal vector and a point on the plane.
+
+    Args:
+        point_a_on_ray (np.array): 3D point on the ray with shape (3, 1)
+        point_b_on_ray (np.array): 3D point on the ray with shape (3, 1)
+        plane_normal (np.array, optional): Unit vector pointing out the plane. Defaults to np.array([[0, 0, 1]]). Shape (1, 3)
+        plane_point (np.array, optional): Point on the plane. Defaults to np.array([0, 0, 0]). Shape (3,)
+
+    Returns:
+        np.array: Returns the 3D point of intersection with shape (3,)
+    """
+    # Vector along the ray direction A -> B
+    if not (point_a_on_ray.shape == point_b_on_ray.shape == (3, 1)):
+        raise ValueError(
+            f"Point A and B must be 3D points with shape (3, 1). {point_a_on_ray.shape=} {point_b_on_ray.shape=}"
+        )
+    if not plane_normal.shape == (1, 3) and np.linalg.norm(plane_normal) == 1:
+        raise ValueError(
+            "Plane normal must be a unit vector with shape (1, 3) and norm 1"
+        )
+    if not plane_point.shape == (3,):
+        raise ValueError("Plane point must be a 3D point with shape (3,)")
 
-    rr.init("geometry", spawn=True)
+    ray_direction = point_b_on_ray - point_a_on_ray
+    # Finding parameter t
+    t = -(np.dot(plane_normal, point_a_on_ray) + plane_point) / np.dot(
+        plane_normal, ray_direction
+    )
+    # Finding point of intersection
+    intersection = (point_a_on_ray.T + t * ray_direction.T).squeeze(0)
+    return intersection
```

## courtvision/models.py

```diff
@@ -1,80 +1,114 @@
 from pathlib import Path
+from typing import Any
 
 import structlog
 import torch
 import torchvision
-from torchvision.models.detection.faster_rcnn import FastRCNNPredictor
+from torchvision.models.detection.faster_rcnn import FasterRCNN, FastRCNNPredictor
 
 from courtvision.swiss import get_latest_file
 
 logger = structlog.get_logger("courtvision.models")
 
 
-def get_fasterrcnn_ball_detection_model(model_path: None | Path = None):
-    # return torch.load(model_path)
+def get_fasterrcnn_ball_detection_model(model_path: None | Path = None) -> FasterRCNN:
+    """Fetches a FasterRCNN model for ball detection.
+    If model_path is None, the model is pretrained on COCO.
+    If model_path is a Path, the model is loaded from the path.
+
+    Args:
+        model_path (None | Path, optional): Path do model weights that will be loaded. Defaults to None.
+
+    Returns:
+        FasterRCNN: A ball detection model using FasterRCNN
+    """
+
     pretrained = model_path is None
-    # raise NotImplementedError()
 
     model = torchvision.models.detection.fasterrcnn_resnet50_fpn(
-        weights=None, weights_backbone=None, pretrained=False
+        weights=None, weights_backbone=None, pretrained=pretrained
     )
     num_classes = 2  # 1 class (ball) + background
     # get number of input features for the classifier
     in_features = model.roi_heads.box_predictor.cls_score.in_features
     # replace the pre-trained head with a new one
     model.roi_heads.box_predictor = FastRCNNPredictor(in_features, num_classes)
     if model_path is not None:
-        model.load_state_dict(torch.load(model_path))
+        model.load_state_dict(torch.load(model_path, map_location=torch.device("cpu")))
     return model
 
 
-def get_yolo_player_detection_model(model_path: None | Path = None):
-    import torch
+def get_yolo_player_detection_model(model_path: None | Path = None) -> Any:
+    """Fetches a pretrained YOLO model for player detection.
+
+    Args:
+        model_path (None | Path, optional): Unused!. Defaults to None.
 
-    # Model
+    Returns:
+        Any: Yolo model
+    """
     model = torch.hub.load("ultralytics/yolov5", "yolov5s", pretrained=True)
     return model
 
 
 def get_yolov8_player_detection_model(model_path: None | Path = None):
     from ultralytics import YOLO
 
     model = YOLO("yolov8n.pt", task="detect")
 
     model.classes = [0]
     model.conf = 0.6
     model.max_det = 4
-    model.tracker = "/Users/benjamindecharmoy/projects/courtvision/botsort.yml"
-    # results = model.track(
-    #     source=RAW_CLIP_PATH.as_posix(),
-    #     # tracker="/Users/benjamindecharmoy/projects/courtvision/bytetrack.yaml",
-    #     tracker="/Users/benjamindecharmoy/projects/courtvision/botsort.yml",
-    #     classes=[0],
-    #     max_det=4,
-    #     save=True,
-    # )
+    model.tracker = "courtvision/models/botsort.yml"
     return model
 
 
+def get_ball_detection_model(model_path: Path) -> "BallDetectorModel":
+    """Grabs a trained ball detection model from a path.
+
+    Args:
+        model_path (Path): Path to the model weights. A .ckpt file.
+
+    Returns:
+        BallDetectorModel: A trained BallDetectorModel from a checkpoint.
+    """
+    from courtvision.trainer import BallDetectorModel  # TODO: move to models.py
+
+    device = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
+    return BallDetectorModel.load_from_checkpoint(model_path, map_location=device)
+
+
 class BallDetector:
     PIPELINE_NAME = "ball_detection"
 
     def __init__(self, model_file_or_dir: Path, cache_dir: Path):
         if model_file_or_dir.is_dir():
             self.model_path = get_latest_file(model_file_or_dir)
         else:
             self.model_path = model_file_or_dir
-        self.model = get_fasterrcnn_ball_detection_model(model_path=self.model_path)
+
+        self.model = get_ball_detection_model(model_path=self.model_path)
         self.cache_dir = cache_dir
         self.model.eval()
 
     def predict(
         self, image: torch.Tensor, frame_idx: int, clip_uid: str
-    ) -> torch.Tensor:
+    ) -> dict[str, torch.Tensor]:
+        """Predicts ball detections for a given frame.
+        !!! note
+            This method caches the detections on disk.
+        Args:
+            image (torch.Tensor): Image tensor of shape (1,3,H,W)
+            frame_idx (int): frame index
+            clip_uid (str): clip uid that identifies the clip uniquely.
+
+        Returns:
+            dict[str, torch.Tensor]: A dict tensor ball detections.
+        """
         cache_path = (
             self.cache_dir
             / self.PIPELINE_NAME
             / clip_uid
             / f"detections_at_{frame_idx}.pt"
         )
         if not cache_path.is_dir():
@@ -95,30 +129,37 @@
         self.model_path = get_latest_file(model_dir)
         self.cache_dir = cache_dir
         self.model = get_yolov8_player_detection_model(model_path=self.model_path)
         # self.model.eval()
 
     def predict(
         self, image: torch.Tensor, frame_idx: int, clip_uid: str
-    ) -> torch.Tensor:
-        from torchvision.transforms.functional import resize
-
-        resized_image = image  # resize(image, (320,640))
+    ) -> dict[str, torch.Tensor]:
+        """Predicts player detections for a given frame.
+        !!! note
+            This method caches the detections on disk.
+        Args:
+            image (torch.Tensor): Image tensor of shape (1,3,H,W)
+            frame_idx (int): frame index
+            clip_uid (str): clip uid that identifies the clip uniquely.
+
+        Returns:
+            dict[str, torch.Tensor]: Dict of player detections.
+        """
         cache_path = (
             self.cache_dir
             / self.PIPELINE_NAME
             / clip_uid
             / f"detections_at_{frame_idx}.pt"
         )
         if not cache_path.is_dir():
             cache_path.parent.mkdir(parents=True, exist_ok=True)
-        if cache_path.is_file() and False:
+        if cache_path.is_file():
             return torch.load(cache_path)
         else:
             with torch.no_grad():
                 detections = self.model.track(
-                    source=resized_image.squeeze(0).permute(1, 2, 0).numpy(),
+                    source=image.squeeze(0).permute(1, 2, 0).numpy(),
                     persist=True,
                 )
-            print(detections[0].boxes)
-            # torch.save(detections, cache_path)
+            torch.save(detections, cache_path)
             return detections
```

## courtvision/pipeline.py

```diff
@@ -9,16 +9,18 @@
 import boto3
 import cv2
 import numpy as np
 import rerun as rr
 import structlog
 import torch
 import torchvision
+import ultralytics
 from kornia.geometry import unproject_points
 from structlog import wrap_logger
+from torch.functional import F
 
 from courtvision.data import (
     Annotation,
     ClipSegmentResult,
     CourtAnnotatedSample,
     CourtVisionArtifacts,
     KeypointValue,
@@ -31,541 +33,178 @@
     frames_from_clip_segments,
     get_normalized_calibration_image_points_and_clip_ids,
 )
 from courtvision.geometry import (
     CameraInfo,
     PadelCourt,
     calibrate_and_evaluate,
+    calibrate_camera,
     convert_obj_points_to_planar,
     corners_world_3d,
-    court_scale,
     denormalize_as_named_points,
     find_optimal_calibration_and_pose,
     get_planar_point_correspondences,
     get_planar_points_padel_court,
+    project_points_to_base_plane,
 )
 from courtvision.models import BallDetector, PlayerDetector
 from courtvision.swiss import get_latest_file, mark_as_deprecated
-from courtvision.vis import log_court_layout
+from courtvision.trackers import ParticleFilter
+from courtvision.vis import (
+    colours_per_player_idx,
+    log_ball_detections,
+    log_court_layout,
+    log_player_detections,
+)
 
 logger = structlog.get_logger()
 
 
 class Verbosity(Enum):
     SILENT = 0
     PROGRESS = 1
     DEBUG = 2
 
 
-def log_ball_detections(
-    detections: dict[str, torch.Tensor],
-    clip_uid: str,
-):
-    boxes = detections[0]["boxes"]
-    scores = detections[0]["scores"]
-    labels = detections[0]["labels"]
-    for i, (box, score, label) in enumerate(zip(boxes, scores, labels)):
-        rr.log_rect(
-            "world/camera/image/ball_detections",
-            rect=(
-                box[0].item(),
-                box[1].item(),
-                box[2].item() - box[0].item(),
-                box[3].item() - box[1].item(),
-            ),
-            # score=score.item(),
-            # label=label.item(),
-            timeless=True,
-        )
-
-
-def point_of_intersection(
-    translation_vector: np.array,
-    unprojected_point_world_coordinate: np.array,
-):
-    import numpy as np
-
-    if translation_vector.shape[0] == 3:
-        translation_vector = translation_vector.T
-
-    # Calculate direction of the ray from camera's position to the 3D point
-    ray_direction = unprojected_point_world_coordinate - translation_vector
-
-    # Define vectors in the plane
-    v1 = np.array([1, 0, 0])
-    v2 = np.array([0, 1, 0])
-
-    # Compute normal to the plane as cross product of v1 and v2
-    normal = np.cross(v1, v2)
-
-    # Assuming the plane passes through the origin
-    point_on_plane = np.array([0, 0, 0])
-
-    # Equation of the plane: (r - point_on_plane) . normal = 0
-    # Substituting r = tvec + t*ray_direction in the plane equation, we get (tvec + t*ray_direction - point_on_plane) . normal = 0
-
-    # Solving for t
-    t = np.dot((point_on_plane - translation_vector), normal) / np.dot(
-        ray_direction, normal
-    )
-
-    # Compute the intersection point
-    intersection = translation_vector + t * ray_direction
-    return intersection
-
-
-def image_point_to_world_court_point(
-    image_point: torch.Tensor,
-    camera_matrix: torch.Tensor,
-    translation_vector: torch.Tensor,
-    rotation_vector: torch.Tensor,
-):
-    import cv2
-    import numpy as np
-    from torch.nn.functional import pad
-
-    # Ensure the correct shape of input tensors
-    # image_point = image_point.view(-1, 1)
-    # translation_vector = translation_vector.view(3, 1)
-    # rotation_vector = rotation_vector.view(3, 1)
-    # # Convert tensors to numpy arrays for processing
-    # image_point = image_point.numpy()
-    # camera_matrix = camera_matrix.numpy()
-    # translation_vector = translation_vector.numpy()
-    # rotation_vector = rotation_vector.numpy()
-    image_point = image_point.numpy()
-    # Convert to homogenous
-    point_2D_hom = np.vstack([image_point.T, np.array([[1]])])
-
-    # Apply inverse camera matrix to get ray direction in camera coords.
-    ray_direction_cam = np.linalg.inv(camera_matrix) @ point_2D_hom
-
-    # Convert ray direction to world coordinates
-    R, _ = cv2.Rodrigues(rotation_vector)
-    ray_direction_world = np.dot(R.T, ray_direction_cam)
-
-    # Normalize the ray direction
-    ray_direction_world /= np.linalg.norm(ray_direction_world)
-
-    # Define the plane
-    # Normal vector for plane (1,0,0) cross (0,1,0) = (0,0,1)
-    normal = np.array([[0], [1], [0]])
-
-    # Assuming the plane passes through the origin
-    point_on_plane = np.array([[0], [0], [0]])
-
-    # Compute intersection
-    numerator = np.dot((point_on_plane - translation_vector).T, normal)
-    denominator = np.dot(ray_direction_world.T, normal)
-    t = numerator / denominator
-
-    intersection = translation_vector + t * ray_direction_world
-
-    return intersection, ray_direction_world
-
-
-import ultralytics
-from torch.functional import F
-
-from courtvision.geometry import project_points_to_base_plane
-from courtvision.vis import colours_per_player_idx
-
-# def image_point_to_world_court_point(
-#         image_point: torch.Tensor,
-#         camera_matrix: torch.Tensor,
-#         translation_vector: torch.Tensor,
-#         rotation_vector: torch.Tensor,
-# ):
-#     import numpy as np
-#     import cv2
-
-#     if translation_vector.shape[0] == 3:
-#         translation_vector = translation_vector.T
-#     # Convert to homogenous
-#     point_2D_hom = F.pad(image_point, [0, 1], "constant", 1.0).squeeze(0).numpy()
-
-#     # Apply inverse camera matrix to get ray direction in camera coords.
-#     ray_direction_cam = np.linalg.inv(camera_matrix) @ point_2D_hom
-
-#     # Convert ray direction to world coordinates
-#     R, _ = cv2.Rodrigues(rotation_vector)
-#     ray_direction_world = R.T @ ray_direction_cam
-
-#     # Normalize the ray direction
-#     ray_direction_world /= np.linalg.norm(ray_direction_world)
-
-#     # Define the plane
-#     # Normal vector for plane (1,0,0) cross (0,1,0) = (0,0,1)
-#     normal = np.array([0, 0, 1])
-
-#     # Assuming the plane passes through the origin
-#     point_on_plane = np.array([0, 0, 0])
-
-#     # Compute intersection
-#     t = np.dot((point_on_plane - translation_vector), normal) / np.dot(ray_direction_world, normal)
-#     intersection = translation_vector + t * ray_direction_world
-#     return intersection.squeeze(0)
-
-
-def apply_camera_to_world_transform(
-    point_in_camera_space: np.array,
-    translation_vector: np.array,
-    rotation_vector: np.array,
-):
-    """transform a point in camera space to world space"""
-    import cv2
-
-    if translation_vector.shape[0] == 3:
-        translation_vector = translation_vector.T
-    if rotation_vector.shape[0] == 3:
-        rotation_vector = rotation_vector.T
-
-    R, _ = cv2.Rodrigues(rotation_vector)
-
-    # Convert 3D point to world's coordinate system
-    point_3D_world = np.dot(R.T, point_in_camera_space) + translation_vector
-
-    return point_3D_world
-    # rotation_matrix, _ = cv2.Rodrigues(rotation_vector)
-    # T = np.concatenate((rotation_matrix.T, -translation_vector.T), axis=1)
-
-    # point_in_camera_space_homogeneous= F.pad(point_in_camera_space, [0,1], "constant", 1.0)
-    # point_in_world_space = np.matmul(T, point_in_camera_space_homogeneous)
-    # point_in_world_space = np.matmul(rotation_matrix.T, (point_in_camera_space.T - translation_vector).squeeze(0))
-    # point_in_world_space =  point_in_camera_space + translation_vector
-    # breakpoint()
-    # return point_in_world_space
-
-
-def camera_space_to_world_space(
-    camera_point: np.array,
-    translation_vector: np.array,
-    rotation_vector: np.array,
-):
-    if not camera_point.shape[0] == 3:
-        raise ValueError("Camera point must be a 3D point with shape (3,)")
-    R, _ = cv2.Rodrigues(rotation_vector)
-    world_point = (R.T @ (camera_point - translation_vector)).T
-    return world_point
-
-
-def compute_ray_intersecting_plane(
-    point_a_on_ray: np.array,
-    point_b_on_ray: np.array,
-    plane_normal: np.array = np.array([[0, 0, 1]]),
-    plane_point: np.array = np.array([0, 0, 0]),
-):
-    """Given two points on a ray, compute the point of intersection with a plane.
-    The plane is defined as a normal vector and a point on the plane.
-
-    Args:
-        point_a_on_ray (np.array): 3D point on the ray with shape (3, 1)
-        point_b_on_ray (np.array): 3D point on the ray with shape (3, 1)
-        plane_normal (np.array, optional): Unit vector pointing out the plane. Defaults to np.array([[0, 0, 1]]). Shape (1, 3)
-        plane_point (np.array, optional): Point on the plane. Defaults to np.array([0, 0, 0]). Shape (3,)
-
-    Returns:
-        np.array: Returns the 3D point of intersection with shape (3,)
-    """
-    # Vector along the ray direction A -> B
-    if not (point_a_on_ray.shape == point_b_on_ray.shape == (3, 1)):
-        raise ValueError(
-            f"Point A and B must be 3D points with shape (3, 1). {point_a_on_ray.shape=} {point_b_on_ray.shape=}"
-        )
-    if not plane_normal.shape == (1, 3) and np.linalg.norm(plane_normal) == 1:
-        raise ValueError(
-            "Plane normal must be a unit vector with shape (1, 3) and norm 1"
-        )
-    if not plane_point.shape == (3,):
-        raise ValueError("Plane point must be a 3D point with shape (3,)")
-
-    ray_direction = point_b_on_ray - point_a_on_ray
-    # Finding parameter t
-    t = -(np.dot(plane_normal, point_a_on_ray) + plane_point) / np.dot(
-        plane_normal, ray_direction
-    )
-    # Finding point of intersection
-    intersection = (point_a_on_ray.T + t * ray_direction.T).squeeze(0)
-    return intersection
-
-
-def log_player_detections(
-    detections: list[ultralytics.yolo.engine.results.Results],
-    camera_matrix: np.array,
-    translation_vector: np.array,
-    rotation_vector: np.array,
-    clip_uid: str,
-):
-    player_maker_radius = 5.0
-    if len(detections) > 1:
-        raise NotImplementedError("Only batches of size 1 are supported for now")
-    result = detections[0]
-
-    for det in result.boxes.data:
-        # TODO: Fix this hack. Use?
-        # x1, y1, x2, y2, idx, *_ = det
-        if len(det) == 7:
-            x1, y1, x2, y2, idx, conf, cls = det
-        else:
-            x1, y1, x2, y2, idx, conf = det
-            cls = 0
-        rr.log_rect(
-            f"world/camera/image/Player_{int(idx)}",
-            (x1, y1, (x2 - x1), (y2 - y1)),
-            color=colours_per_player_idx[int(idx)],
-        )
-        # Compute the 3D point of the player's feet
-        # Use 2 depth values to unproject the point from the image plane to the camera plane
-        depths = torch.tensor(
-            [[1.0 * court_scale, 20.0 * court_scale]]
-        ).T  # Depth values in [mm * court_scale]
-        mid_feets = torch.tensor([((x1 + x2) / 2, (y2 + y2) / 2)]).repeat(
-            depths.shape[0], 1
-        )
-        mid_feets_base_camera_space = unproject_points(
-            point_2d=mid_feets, camera_matrix=camera_matrix, depth=depths
-        ).squeeze(0)
-        # Using the Translation and Rotation Vector of the camera, transform the point from camera space to world space
-        mid_feet_base_world_space = camera_space_to_world_space(
-            mid_feets_base_camera_space.squeeze(0).numpy().T,
-            translation_vector,
-            rotation_vector,
-        )
-        # Compute the intersection of the ray formed by the camera position and the 3D point with the plane
-        intersection = compute_ray_intersecting_plane(
-            point_a_on_ray=mid_feet_base_world_space[0].reshape(3, 1),
-            point_b_on_ray=mid_feet_base_world_space[1].reshape(3, 1),
-        )
-        # rr.log_points(f"world/camera/Player_{int(idx)}", mid_feet_base_camera_space,  )
-        rr.log_point(
-            f"world/Player_{int(idx)}",
-            intersection,
-            radius=player_maker_radius,
-            color=colours_per_player_idx[int(idx)],
-        )
-        # rr.log_arrow(
-        #     "world/camera/ray",
-        #     origin=translation_vector.squeeze(),
-        #     vector=rotation_vector.squeeze(),
-        #     # length=100,
-        #     width_scale=100.0,
-        # )
-        # mid_feet_base_3d, ray_direction_world = image_point_to_world_court_point(
-        #     image_point=mid_feet,
-        #     camera_matrix=camera_matrix,
-        #     translation_vector=translation_vector,
-        #     rotation_vector=rotation_vector,
-        # )
-        # rr.log_arrow(
-        #     "world/camera/ray_world",
-        #     origin=translation_vector.squeeze(),
-        #     vector=ray_direction_world.squeeze(),
-        #     width_scale=10.0,
-        # )
-        # from kornia.geometry import unproject_points
-        # mid_feet_base_camera_space = unproject_points(point_2d=mid_feet, camera_matrix=camera_matrix,depth=torch.tensor([10.0])).squeeze(0)
-        # mid_feet_base = apply_camera_to_world_transform(
-        #     mid_feet_base_camera_space,
-        #     translation_vector=translation_vector,
-        #     rotation_vector=rotation_vector,
-        # )
-        # mid_feet_base_3d = point_of_intersection(
-        #     translation_vector=translation_vector,
-        #     unprojected_point_world_coordinate=mid_feet_base.numpy(),
-        # ).squeeze(0)
-
-        # mid_feet_base_3d = mid_feet_base
-        # (
-        # F.pad(mid_feet_base, (0, 1), mode="constant", value=0.0) / 10.0
-        # )
-        # Switch Y and Z axis
-        # x = mid_feet_base_3d[0].item()
-        # y = mid_feet_base_3d[1].item()
-        # z = mid_feet_base_3d[2].item()
-        # mid_feet_base_3d[2] = player_maker_radius
-        # mid_feet_base_3d[1] = mid_feet_base_3d[1]
-        # mid_feet_base_3d[0] = mid_feet_base_3d[0]
-        # # rr.log_point("world/debug",mid_feet_base, radius=10)
-        # rr.log_point(
-        #     f"world/camera/Player_{int(idx)}",
-        #     mid_feet_base_3d,
-        #     radius=player_maker_radius,
-        #     color=colours_per_player_idx[int(idx)],
-        # )
-
-
-def pipeline(
-    artifacts: CourtVisionArtifacts,
-):
-    # Calibrate camera
-    artifacts = calibrate_camera(artifacts)
-
-    # Detect ball and players in the image plane
-    # for artifacts.dataset
-
-
-def calibrate_camera(
-    artifacts: CourtVisionArtifacts, verbose: Verbosity = Verbosity.PROGRESS
-) -> CourtVisionArtifacts:
-    if artifacts.camera_info:
-        logger.info(
-            "Camera already calibrated - using supplied camera_info",
-            camera_info=artifacts.camera_info,
-        )
-        return artifacts
-    if artifacts.camera_info_path.is_file():
-        artifacts.camera_info = CameraInfo.load(artifacts.camera_info_path)
-        logger.info(
-            "Camera already calibrated - using cached version",
-            camera_info=artifacts.camera_info,
-        )
-        return artifacts
-
-    frame, uid = next(
-        frames_from_clip_segments(
-            artifacts.dataset,
-            local_path=artifacts.local_cache_path,
-            stream_type=StreamType.VIDEO,
-        )
-    )
-
-    image_width, image_height = frame["data"].shape[2], frame["data"].shape[1]
-    logger.info(
-        "Calibrating camera using:", image_width=image_width, image_height=image_height
-    )
-    if image_height < 100 or image_width < 100:
-        logger.warn("Image dimensions look wrong! Check it out.")
-
-    (
-        normalised_named_points,
-        valid_clip_ids,
-    ) = get_normalized_calibration_image_points_and_clip_ids(artifacts.dataset)
-    calibration_image_points = denormalize_as_named_points(
-        normalised_named_points=normalised_named_points,
-        image_width=image_width,
-        image_height=image_height,
-    )
-
-    calibration_correspondences = get_planar_point_correspondences(
-        image_points=calibration_image_points,
-        world_points=corners_world_3d.copy(),
-        minimal_set_count=4,
-    )
-
-    pose_correspondences = get_planar_point_correspondences(
-        image_points=calibration_image_points,
-        world_points=corners_world_3d.copy(),
-        minimal_set_count=6,
-    )
-
-    all_world_points, all_labels = dict_to_points(corners_world_3d.copy())
-    all_image_points, _ = dict_to_points(calibration_image_points.copy())
-    logger.info("Calibrating camera...")
-
-    camera_info = find_optimal_calibration_and_pose(
-        valid_clip_ids=valid_clip_ids,
-        calibration_correspondences=calibration_correspondences,
-        pose_correspondences=pose_correspondences,
-        image_height=image_height,
-        image_width=image_width,
-        all_image_points=all_image_points,
-        all_world_points=all_world_points,
-    )
-    logger.info("Calibrated camera", camera_info=camera_info)
-    artifacts.camera_info = camera_info
-    artifacts.camera_info.save(artifacts.camera_info_path)
-    return artifacts
-
-
 if __name__ == "__main__":
-    ANNOTATION_PATH = Path(
-        "/Users/benjamindecharmoy/projects/courtvision/datasets/clip_segmentations"
-    )
-    ANNOTATION_DATA_PATH = Path(
-        "/Users/benjamindecharmoy/projects/courtvision/datasets/clip_segmentations/data"
-    )
+    # TODO: Make this a proper CLI using Typer. https://github.com/BenjaminDev/courtvision/issues/4
+
+    ANNOTATION_PATH = Path("../datasets/clip_segmentations")
+    ANNOTATION_DATA_PATH = Path("../datasets/clip_segmentations/data")
     ANNOTATION_DATA_PATH.mkdir(exist_ok=True, parents=True)
 
-    court_mesh_path = Path(
-        "/Users/benjamindecharmoy/projects/courtvision/blender/basic_image.glb"
-    )
+    court_mesh_path = Path("../blender/basic_image.glb")
 
     annotations_file = get_latest_file(ANNOTATION_PATH, "json")
     with open(annotations_file, "r") as f:
         dataset = PadelDataset(samples=json.load(f))
 
     artifacts = CourtVisionArtifacts(
         local_cache_path=ANNOTATION_DATA_PATH / "cache",
         dataset=dataset,
         ball_detector=BallDetector(
             model_file_or_dir=Path(
-                "/Users/benjamindecharmoy/projects/courtvision/models/ball_detector/fasterrcnn_resnet50_fpn_project-1-at-2023-05-23-14-38-c467b6ad-67.pt"
+                "/Users/benjamindecharmoy/projects/courtvision/models/ball_detector/epoch=7-step=368.ckpt"
             ),
             cache_dir=ANNOTATION_DATA_PATH / "cache",
         ),
-        player_detector=PlayerDetector(
-            model_dir=Path(
-                "/Users/benjamindecharmoy/projects/courtvision/models/player_detection"
+        ball_tracker=ParticleFilter(
+            num_particles=100_000,
+            court_size=torch.tensor(
+                [PadelCourt.width, PadelCourt.length, PadelCourt.backwall_fence_height]
             ),
+        ),
+        player_detector=PlayerDetector(
+            model_dir=Path("../models/player_detection"),
             cache_dir=ANNOTATION_DATA_PATH / "cache",
         ),
-        # camera_info=None,
         camera_info_path=ANNOTATION_DATA_PATH / "cache" / "camera_info.npz",
         court_layout=PadelCourt(),
     )
-    breakpoint()
-    artifacts = calibrate_camera(artifacts, verbose=True)
 
+    # Calibrate camera from annotations in the dataset
+    artifacts = calibrate_camera(artifacts, logger=logger)
+    artifacts.ball_tracker.reset(
+        num_particles=100_000,
+        court_size=torch.tensor(
+            [PadelCourt.width, PadelCourt.length, PadelCourt.backwall_fence_height]
+        ),
+        world_to_cam=artifacts.camera_info.world_space_to_camera_space(),
+        cam_to_image=torch.tensor(artifacts.camera_info.camera_matrix),
+    )
     rr.init(
         "courtvision",
         spawn=False,
     )
-    ip, port = "127.0.0.1", "9876"
+    ip, port = (
+        "127.0.0.1",
+        "9876",
+    )  # TODO: Make this configurable https://github.com/BenjaminDev/courtvision/issues/4
     rr.connect(f"{ip}:{port}")
     current_uid = None
-    for i, (frame, uid) in enumerate(
+    for i, (frame, uid, match_id) in enumerate(
         frames_from_clip_segments(
             artifacts.dataset,
             local_path=artifacts.local_cache_path,
             stream_type=StreamType.VIDEO,
         )
     ):
 
         rr.set_time_sequence(uid, i)
         if uid != current_uid:
+            if current_uid is not None:
+                break
             log_court_layout(
                 camera_matrix=artifacts.camera_info.camera_matrix,
                 image_width=artifacts.camera_info.image_width,
                 image_height=artifacts.camera_info.image_height,
                 translation_vector=artifacts.camera_info.translation_vector,
                 rotation_vector=artifacts.camera_info.rotation_vector,
                 court_mesh_path=court_mesh_path,
             )
             current_uid = uid
         rr.log_image(
             "world/camera/image",
             frame["data"].permute(1, 2, 0).numpy().astype(np.uint8),
         )
+
         # Detect and log ball detections
         ball_detections = artifacts.ball_detector.predict(
             frame["data"].unsqueeze(0).float() / 255.0,
             frame_idx=i,
             clip_uid=uid,
         )
         log_ball_detections(
             detections=ball_detections,
             clip_uid=uid,
         )
-
+        # TODO: use variable dt for prediction. Use frame["pts"]
         # Detect and log player detections
         player_detections = artifacts.player_detector.predict(
             frame["data"].unsqueeze(0),
             frame_idx=i,
             clip_uid=uid,
         )
+        artifacts.ball_tracker.predict(dt=1 / 30.0)
+        for ball_detection in ball_detections:
+            for (bx1, by1, bx2, by2), ball_score in zip(
+                ball_detection["boxes"][:4], ball_detection["scores"]
+            ):
+                obs_state = torch.tensor(
+                    [
+                        (bx1 + bx2) / 2.0,
+                        (by1 + by2) / 2.0,
+                    ]
+                ).to(dtype=torch.float32)
+                for _ in range(10):
+                    artifacts.ball_tracker.update(obs_state, ball_score)
+                    # TODO: Move this to a separate function in vis.py
+                    rr.log_points(
+                        "world/ball_state",
+                        positions=artifacts.ball_tracker.xyz,
+                    )
+                    rr.log_point(
+                        "world/tracker_mean",
+                        artifacts.ball_tracker.xyz_mean,
+                        color=(255, 222, 0),
+                        radius=2.0,
+                    )
+                    ball_mean_estimate = artifacts.ball_tracker.state_to_observation(
+                        artifacts.ball_tracker.xyz_mean,
+                        world_to_cam=artifacts.ball_tracker.world_to_cam,
+                        cam_to_image=artifacts.ball_tracker.cam_to_image,
+                    )
+                    rr.log_point(
+                        "world/camera/image/ball_mean_estimate",
+                        ball_mean_estimate,
+                        color=(255, 222, 0),
+                        radius=2.0,
+                    )
+                break
+
         log_player_detections(
             detections=player_detections,
             clip_uid=uid,
             camera_matrix=artifacts.camera_info.camera_matrix,
             translation_vector=artifacts.camera_info.translation_vector,
             rotation_vector=artifacts.camera_info.rotation_vector,
         )
```

## courtvision/trackers.py

```diff
@@ -1,53 +1,73 @@
-# Define a type for a named tensor with two dimensions
-# ImagePlaneDetections = torch.TensorType[("x", float), ("y", float)]
 import enum
 from enum import Enum, IntEnum, auto
 from typing import Any
 
 import torch
 from kornia.geometry import (
     convert_points_from_homogeneous,
     convert_points_to_homogeneous,
 )
-from torch import tensor
-
-from courtvision.geometry import PadelCourt
 
 
 class StateIdx:
+    """
+    Named indices for the state tensor.
+    """
+
     x: int = 0
     y: int = 1
     z: int = 2
     vx: int = 3
     vy: int = 4
     vz: int = 5
     ax: int = 6
     ay: int = 7
     az: int = 8
     weight: int = 9
 
 
-class Tracker:
+class ParticleFilter:
+    """
+    Particle filter tracker.
+    """
+
     def __init__(
         self,
-        num_particles: int = 1000,
+        *,
+        num_particles: int,
+        court_size: torch.Tensor,
+        world_to_cam: torch.Tensor | None = None,
+        cam_to_image: torch.Tensor | None = None,
+    ) -> None:
+        self.reset(
+            num_particles=num_particles,
+            court_size=court_size,
+            world_to_cam=world_to_cam,
+            cam_to_image=cam_to_image,
+        )
+
+    def reset(
+        self,
+        *,
+        num_particles: int,
+        court_size: torch.tensor,
         world_to_cam: torch.Tensor | None = None,
         cam_to_image: torch.Tensor | None = None,
-        court_size: torch.tensor = torch.tensor(
-            [PadelCourt.width, PadelCourt.length, PadelCourt.backall_fence_height]
-        ),
     ) -> None:
         self.num_particles = num_particles
+        # Court size is a tensor of the form [width, length, height]
+        self.court_size = court_size
+
         # state: [x, y, z, vx, vy, zv, ax, ay, az, ax, ay, az, weight]
         self.states = torch.randn(
             (num_particles, 3 * 3 + 1),
             names=["num_particles", "state"],
         )
-        # Place a prior on the initial state X, Y, Z to be on the court
+
         self.states[:, StateIdx.x] = (
             self.states[:, StateIdx.x] * court_size[StateIdx.x]
             + court_size[StateIdx.x] / 2
         )
         self.states[:, StateIdx.y] = (
             self.states[:, StateIdx.y] * court_size[StateIdx.y]
             + court_size[StateIdx.y] / 2
@@ -57,62 +77,96 @@
             + court_size[StateIdx.z] / 2
         )
         self.states[:, StateIdx.weight] = torch.abs(
             self.normalized_weights(self.states)
         )
         # Set the initial velocity to be zero
         self.states[:, StateIdx.vx : StateIdx.vz + 1] = 0.0
-        # Set the initial acceleration to be zero but -9.8 in the z direction
+        # Set the initial acceleration to be zero but -9.8 m/s^2 in the z direction
         self.states[:, StateIdx.ax : StateIdx.az + 1] = 0.0
-        self.states[:, StateIdx.az] = -9.8
+        self.states[:, StateIdx.az] = -0.98  # Note: units are in 1e-1 m/s^2
 
-        self.cam_to_image = torch.randn((3, 4))
+        self.cam_to_image = torch.randn((3, 3))
         if cam_to_image is not None:
             self.cam_to_image = cam_to_image.to(dtype=torch.float32)
         self.world_to_cam = torch.randn((4, 4))
         if world_to_cam is not None:
             self.world_to_cam = world_to_cam.to(dtype=torch.float32)
-        # self.H = self.cam_to_image @ self.world_to_cam
 
     def set_states_to(self, point: torch.tensor):
-        # tracker.states[:,0:3] = torch.tensor([1.0, 2.0, 3.0]).repeat((1000,1))
+        """Set the state of the tracker to a single point.
+
+        Args:
+            point (torch.tensor): point in the world space. Shape: [3]
+        """
         self.states[:, StateIdx.x : StateIdx.z + 1] = point.repeat(
             (self.num_particles, 1)
         )
 
     @property
     def xyz(self) -> torch.tensor:
+        """Grab the xyz coordinates of the tracker.
+
+        Returns:
+            torch.tensor: [X,Y,Z] coordinates of the tracker. Shape: [N, 3]
+        """
         return self.states[:, StateIdx.x : StateIdx.z + 1].clone()
 
     @property
     def mean_image_plane_prediction(self) -> torch.tensor:
+        """Computes the weighted mean of the trackers state and
+        projects it to the image plane.
+
+        Returns:
+            torch.tensor: [x,y] coordinates of the tracker mean estimate in the image plane. Shape: [1, 2]
+        """
         return self.state_to_observation(
             self.xyz_mean,
             world_to_cam=self.world_to_cam,
             cam_to_image=self.cam_to_image,
         )
 
     @property
     def xyz_mean(self) -> torch.tensor:
+        """Grab the weighted mean of the xyz coordinates of the tracker.
 
+        Returns:
+            torch.tensor: Weighted mean of the [X,Y,Z] coordinates of the tracker. Shape: [1, 3]
+        """
         xyz_mean = (
             self.xyz.rename(None).T @ self.states[:, StateIdx.weight].rename(None)
-        ) / self.states[:, StateIdx.weight].sum()
+        ) / self.states[:, StateIdx.weight].rename(None).sum()
         return xyz_mean.unsqueeze(0)
 
     @staticmethod
     def normalized_weights(states: torch.tensor) -> torch.tensor:
+
         return (
-            states.select("state", StateIdx.weight)
-            / states.select("state", StateIdx.weight).sum()
+            states.select("state", StateIdx.weight).rename(None)
+            / states.select("state", StateIdx.weight).rename(None).sum()
         )
 
     @staticmethod
-    def state_to_observation(state, *, world_to_cam, cam_to_image):
-
+    def state_to_observation(
+        state: torch.Tensor,
+        *,
+        world_to_cam: torch.Tensor,
+        cam_to_image: torch.Tensor,
+    ) -> torch.Tensor:
+        """Map the state to the observation space.
+        This is from the 3D world space to the 2D image plane.
+
+        Args:
+            state (torch.Tensor): Tracker state. Shape: [N, state_dim]
+            world_to_cam (torch.Tensor): _description_
+            cam_to_image (torch.Tensor): _description_
+
+        Returns:
+            torch.Tensor: _description_
+        """
         x_y_z_1_positions = convert_points_to_homogeneous(
             state[:, : StateIdx.z + 1].rename(None)
         )
         x_y_z_1_positions_cam = convert_points_from_homogeneous(
             x_y_z_1_positions @ world_to_cam.T
         )
         return convert_points_from_homogeneous(x_y_z_1_positions_cam @ cam_to_image.T)
@@ -120,83 +174,127 @@
     def likelihood_in_state_space(
         self, obs_state: torch.tensor, pred_state: torch.tensor
     ):
         # unproject_points
         ...
 
     # # Define the likelihood function
-    def likelihood(self, obs_state: torch.tensor, pred_state: torch.tensor):
+    def likelihood(
+        self, obs_state: torch.tensor, pred_state: torch.tensor
+    ) -> torch.tensor:
+        """Compute the likelihood of the observation given the predicted state.
+
+        Args:
+            obs_state (torch.tensor): Observation in the image plane. Shape: [2]
+            pred_state (torch.tensor): Predicted state. Shape: [N, state_dim]
+
+        Returns:
+            orch.tensor: likelihood of the observation given the predicted state. Shape: [N]
+        """
         sigma = 20.1  # Standard deviation of the observation noise
         from torch.nn.functional import mse_loss
 
         pred_obs = self.state_to_observation(
             pred_state, world_to_cam=self.world_to_cam, cam_to_image=self.cam_to_image
         )
         mse = mse_loss(pred_obs, obs_state.expand_as(pred_obs), reduction="none").sum(
             dim=1
         )
-        # p = torch.exp(-0.5 * mse / sigma)
         p = torch.max(torch.exp(-0.5 * mse / sigma) ** 2, torch.tensor(1e-3))
         return p
 
     def predict(self, dt: float = 1.0 / 30.0):
-        # Define the transition model
+        """
+        Predict the next state using the current state and the time step.
+        `p(x_t | x_{t-1}) ~ N(x_t; x_{t-1} + v_{t-1} * dt, sigma^2)`
+
+
+        Args:
+            dt (float, optional): Time step in [s]. Defaults to 1.0/30.0.
+        """
+
         # state: [x, y, z, vx, vy, zv, ax, ay, az, ax, ay, az, weight]
+        # Random walk in the x, y, and z directions
+        # self.states[:, StateIdx.x : StateIdx.z + 1] = (
+        #     self.states[:, StateIdx.x : StateIdx.z + 1]
+        #     + torch.randn((self.num_particles, 3)) * 5.0
+        # )
 
-        self.states[:, StateIdx.x : StateIdx.z + 1] = (
-            self.states[:, StateIdx.x : StateIdx.z + 1]
-            + torch.randn((self.num_particles, 3)) * 5.0
-        )
-        # Ensure state is on the court using clamp
+        # Update the state using the velocity
+        self.states[:, StateIdx.x : StateIdx.z + 1] += (
+            self.states[:, StateIdx.vx : StateIdx.vz + 1] * dt
+        ) + 0.5 * (self.states[:, StateIdx.ax : StateIdx.az + 1] * dt**2)
+
+        # Ensure state is on the court using clamp.
         self.states[:, StateIdx.x] = torch.clamp(
-            self.states[:, StateIdx.x], 0.0, PadelCourt.width
+            self.states[:, StateIdx.x], 0.0, self.court_size[StateIdx.x]
         )
         self.states[:, StateIdx.y] = torch.clamp(
-            self.states[:, StateIdx.y], 0.0, PadelCourt.length
+            self.states[:, StateIdx.y], 0.0, self.court_size[StateIdx.y]
         )
         self.states[:, StateIdx.z] = torch.clamp(
-            self.states[:, StateIdx.z], 0.0, PadelCourt.backall_fence_height * 1.5
+            self.states[:, StateIdx.z], 0.0, self.court_size[StateIdx.z] * 1.5
         )
 
-        # self.states[:, StateIdx.x : StateIdx.z + 1] += (
-        #     self.states[:, StateIdx.vx : StateIdx.vz + 1] * dt + torch.randn(
-        #         (self.num_particles, 3)
-        #     )*5.0
-        # )
-        # # Z cannot be less than zero
-        # self.states[:, StateIdx.z] = torch.max(self.states[:, StateIdx.z].rename(None), torch.tensor(0.0))
+        # Update the velocity using the acceleration + jitter
+        self.states[:, StateIdx.vx : StateIdx.vz + 1] += (
+            self.states[:, StateIdx.ax : StateIdx.az + 1] * dt
+            + torch.randn((self.num_particles, 3)) * 1.5
+        )
 
-        # self.states[:, StateIdx.vx : StateIdx.vz + 1] += (
-        #     self.states[:, StateIdx.ax : StateIdx.az + 1] * dt
-        # )
-        # randomize the acceleration in the x and y directions
-        # self.states[:, StateIdx.ax : StateIdx.az + 1] += torch.randn(
-        #     (self.num_particles, 3)
-        # )
-        # Set the acceleration in the z direction to be -9.8
-        # and the acceleration in the x and y directions to be zero
-        # self.states[:, StateIdx.ax : StateIdx.az + 1] = 0.0
-        # self.states[:, StateIdx.az] = -9.8
+        self.states[:, StateIdx.ax : StateIdx.az + 1] = (
+            torch.randn((self.num_particles, 3)) * 0.9
+        )
+        self.states[:, StateIdx.az] = -0.98  # Note: units are in 1e-1 m/s^2
 
     def update(self, obs_state: torch.tensor, score: torch.tensor = torch.tensor(1.0)):
-        # Define the likelihood function
-        likelihoods = self.likelihood(obs_state, self.states)
+        """Update the state using the observation and it's associated score.
+
+        Args:
+            obs_state (torch.tensor): measurement in the image plane. Shape: [2]
+            score (torch.tensor, optional): If the detector assigns a score this
+                                            can be used in the update step.
+                                            Defaults to torch.tensor(1.0).
+        """
+        likelihoods = self.likelihood(obs_state, self.states) * score
         self.states[:, StateIdx.weight] = self.update_weights(
             self.states[:, StateIdx.weight], likelihoods
         )
         self.states = self.resample(self.states, self.states[:, StateIdx.weight])
 
     @staticmethod
     def update_weights(
         weights: torch.tensor, likelihoods: torch.tensor
     ) -> torch.tensor:
-        return weights * likelihoods / (weights * likelihoods).sum()
+        """Given the current weights and the likelihoods, update the weights.
+
+        Args:
+            weights (torch.tensor): Nx1 tensor of weights
+            likelihoods (torch.tensor): Nx1 tensor of likelihoods
+
+        Returns:
+            torch.tensor: Nx1 tensor of updated weights
+        """
+        return (
+            weights.rename(None)
+            * likelihoods
+            / (weights.rename(None) * likelihoods).sum()
+        )
 
     @staticmethod
     def resample(states: torch.tensor, weights: torch.tensor) -> torch.tensor:
+        """Given a set of states and associated weights, resample the states.
+
+        Args:
+            states (torch.tensor): Tracker state. Shape: [N, state_dim]
+            weights (torch.tensor): weights associated with each state. Shape: [N x 1]
+
+        Returns:
+            torch.tensor: returns the resampled states. Shape: [N, state_dim]
+        """
         if weights.names is not None:
             weights = weights.rename(None)
         if states.names is not None:
             states = states.rename(None)
 
         return states[
             torch.multinomial(weights, len(weights), replacement=True)
```

## courtvision/vis.py

```diff
@@ -4,20 +4,26 @@
 from typing import Union
 
 import cv2
 import kornia as K
 import matplotlib.pyplot as plt
 import numpy as np
 import rerun as rr
-
-# import rerun_sdk
 import torch
+import ultralytics
+from kornia.geometry import unproject_points
 from mpl_toolkits.mplot3d import Axes3D
 from scipy import ndimage
 
+from courtvision.data import PadelCourt
+from courtvision.geometry import (
+    camera_space_to_world_space,
+    compute_ray_intersecting_plane,
+)
+
 colours_per_player_idx = defaultdict(lambda: (255, 255, 255))
 colours_per_player_idx.update(
     {
         0: (0, 255, 0),
         1: (0, 0, 255),
         2: (255, 0, 0),
         3: (255, 255, 0),
@@ -58,24 +64,105 @@
         transform=rr.TranslationAndMat3(
             translation=translation_vector.squeeze(),
             matrix=rotation_matrix,
         ),
         from_parent=True,
     )
     rr.log_point("world/front_left", np.array([0, 0, 0]))
+    # TODO: this should be refectored to use the court_size
     rr.log_point("world/front_right", np.array([100, 0, 0]))
     rr.log_mesh_file(
         "world",
         mesh_format=rr.MeshFormat("GLB"),
         mesh_path=court_mesh_path,
     )
 
 
+def log_player_detections(
+    detections: list[ultralytics.yolo.engine.results.Results],
+    camera_matrix: np.array,
+    translation_vector: np.array,
+    rotation_vector: np.array,
+    clip_uid: str,
+):
+    player_maker_radius = 5.0
+    if len(detections) > 1:
+        raise NotImplementedError("Only batches of size 1 are supported for now")
+    result = detections[0]
+
+    for det in result.boxes.data:
+        # TODO: Fix this hack. Use?
+        # x1, y1, x2, y2, idx, *_ = det
+        if len(det) == 7:
+            x1, y1, x2, y2, idx, conf, cls = det
+        else:
+            x1, y1, x2, y2, idx, conf = det
+            cls = 0
+        rr.log_rect(
+            f"world/camera/image/player_{int(idx)}",
+            (x1, y1, (x2 - x1), (y2 - y1)),
+            color=colours_per_player_idx[int(idx)],
+        )
+        # Compute the 3D point of the player's feet
+        # Use 2 depth values to unproject the point from the image plane to the camera plane
+        depths = torch.tensor(
+            [[1.0 * PadelCourt.court_scale, 20.0 * PadelCourt.court_scale]]
+        ).T  # Depth values in [mm * PadelCourt.court_scale]
+        mid_feets = torch.tensor([((x1 + x2) / 2, (y2 + y2) / 2)]).repeat(
+            depths.shape[0], 1
+        )
+        mid_feets_base_camera_space = unproject_points(
+            point_2d=mid_feets, camera_matrix=camera_matrix, depth=depths
+        ).squeeze(0)
+        # Using the Translation and Rotation Vector of the camera, transform the point from camera space to world space
+        mid_feet_base_world_space = camera_space_to_world_space(
+            mid_feets_base_camera_space.squeeze(0).numpy().T,
+            translation_vector,
+            rotation_vector,
+        )
+        # Compute the intersection of the ray formed by the camera position and the 3D point with the plane
+        intersection = compute_ray_intersecting_plane(
+            point_a_on_ray=mid_feet_base_world_space[0].reshape(3, 1),
+            point_b_on_ray=mid_feet_base_world_space[1].reshape(3, 1),
+        )
+
+        rr.log_point(
+            f"world/player_{int(idx)}",
+            intersection,
+            radius=player_maker_radius,
+            color=colours_per_player_idx[int(idx)],
+        )
+
+
+def log_ball_detections(
+    detections: list[dict[str, torch.Tensor]],
+    clip_uid: str,
+):
+    boxes = detections[0]["boxes"]
+    scores = detections[0]["scores"]
+    labels = detections[0]["labels"]
+    rects = []
+    for i, (box, score, label) in enumerate(zip(boxes, scores, labels)):
+        rects.append(
+            (
+                box[0].item(),
+                box[1].item(),
+                box[2].item() - box[0].item(),
+                box[3].item() - box[1].item(),
+            )
+        )
+    rr.log_rects(
+        "world/camera/image/ball_detections",
+        rects,
+        timeless=False,
+    )
+
+
 def plot_coords(img: np.array, src_coords: np.array, show: bool = True, thickness=2):
-    """Draws lines on 'img'
+    """Draws lines on 'img'.
 
     Args:
         img (np.array): _description_
         src_coords (np.array): _description_
         show (bool, optional): _description_. Defaults to True.
     """
     src_coords = src_coords.astype(int)
```

## Comparing `courtvision-0.1.0.dist-info/LICENSE` & `courtvision-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

