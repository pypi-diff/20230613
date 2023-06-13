# Comparing `tmp/sleap_anipose-0.1.6-py3-none-any.whl.zip` & `tmp/sleap_anipose-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 38838 bytes, number of entries: 9
--rw-r--r--  2.0 unx      310 b- defN 23-Feb-07 02:08 sleap_anipose/__init__.py
--rw-r--r--  2.0 unx    23044 b- defN 23-Feb-07 02:08 sleap_anipose/calibration.py
--rw-r--r--  2.0 unx    16020 b- defN 23-Feb-07 02:08 sleap_anipose/triangulation.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Feb-07 02:09 sleap_anipose-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    47440 b- defN 23-Feb-07 02:09 sleap_anipose-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-07 02:09 sleap_anipose-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      258 b- defN 23-Feb-07 02:09 sleap_anipose-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Feb-07 02:09 sleap_anipose-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      775 b- defN 23-Feb-07 02:09 sleap_anipose-0.1.6.dist-info/RECORD
-9 files, 123102 bytes uncompressed, 37496 bytes compressed:  69.5%
+Zip file size: 38923 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-13 03:55 sleap_anipose/__init__.py
+-rw-r--r--  2.0 unx    23027 b- defN 23-Jun-13 03:55 sleap_anipose/calibration.py
+-rw-r--r--  2.0 unx    16596 b- defN 23-Jun-13 03:55 sleap_anipose/triangulation.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-13 03:56 sleap_anipose-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    47425 b- defN 23-Jun-13 03:56 sleap_anipose-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 03:56 sleap_anipose-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-13 03:56 sleap_anipose-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-13 03:56 sleap_anipose-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      775 b- defN 23-Jun-13 03:56 sleap_anipose-0.1.7.dist-info/RECORD
+9 files, 123646 bytes uncompressed, 37581 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: sleap_anipose/calibration.py
 Comment: 
 
 Filename: sleap_anipose/triangulation.py
 Comment: 
 
-Filename: sleap_anipose-0.1.6.dist-info/LICENSE
+Filename: sleap_anipose-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: sleap_anipose-0.1.6.dist-info/METADATA
+Filename: sleap_anipose-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: sleap_anipose-0.1.6.dist-info/WHEEL
+Filename: sleap_anipose-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: sleap_anipose-0.1.6.dist-info/entry_points.txt
+Filename: sleap_anipose-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: sleap_anipose-0.1.6.dist-info/top_level.txt
+Filename: sleap_anipose-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: sleap_anipose-0.1.6.dist-info/RECORD
+Filename: sleap_anipose-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sleap_anipose/__init__.py

```diff
@@ -1,7 +1,7 @@
 """High-level imports."""
 from sleap_anipose.calibration import calibrate, draw_board
 from sleap_anipose.triangulation import load_view, load_tracks, triangulate, reproject
 
 # Define package version.
 # This is read dynamically by setuptools in setup.cfg to determine the release version.
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

## sleap_anipose/calibration.py

```diff
@@ -189,15 +189,15 @@
             view_corners[view_idxs]
             for view_corners, view_idxs in zip(raw_detections, idxs_per_view)
         ],
         axis=0,
     )
 
     corners_3d = cgroup.triangulate_optim(common_corners)
-    corners_reproj = cgroup.project(corners_3d.reshape((-1, 2))).reshape(
+    corners_reproj = cgroup.project(corners_3d).reshape(
         (len(raw_detections), len(common_frames), -1, 2)
     )
 
     if len(save_path) > 0:
         cam_names = cgroup.get_names()
         with h5py.File(save_path, "w") as f:
             f.create_dataset(
```

## sleap_anipose/triangulation.py

```diff
@@ -40,43 +40,45 @@
 
     Args:
         session: The path pointing to the session directory (relative to the
             working directory).
         frames: A tuple structured as (start_frame, end_frame) containing the frame
             range to load from each video. The range is (inclusive, exclusive) and will
             be considered as the entire video if not otherwise specified.
-        cams: Tuple of camera names specifying order of views to load tracks in. If not
-            given, will load views in the alphabetic order of the folders found in the
-            given session.
+        cams: Tuple of camera names (strings) specifying order of views to load tracks
+            in. If not given, will load views in the order of the cameras in the
+            session's calibration file.
         excluded_views: Names (not paths) of camera views to be excluded. If not given,
             all views will be used.
 
     Returns:
         tracks: A (n_views, n_frames, n_tracks, n_nodes, 2) shape ndarray of 2D poses.
         views: A list of the camera views accessed in the order they were accessed in.
+        If the camera order can not be deduced, None will be returned.
     """
     if cams:
         views = [Path(session) / x for x in cams if x not in excluded_views]
     else:
-        views = sorted(
-            [
-                x
-                for x in Path(session).iterdir()
-                if x.is_dir() and x.name not in excluded_views
-            ]
-        )
+        calib = Path(session) / "calibration.toml"
+        if not calib.exists():
+            return None
+        else:
+            order = CameraGroup.load(calib).get_names()
+            views = [Path(session) / x for x in order if x not in excluded_views]
+
     tracks = np.stack([load_view(view, frames) for view in views], axis=0)
     return tracks, views
 
 
 def triangulate(
     p2d: Union[np.ndarray, str],
     calib: Union[CameraGroup, str],
     frames: Tuple[int] = (),
     excluded_views: Tuple[str] = (),
+    ransac: bool = False,
     fname: str = "",
     disp_progress: bool = False,
     **kwargs,
 ) -> np.ndarray:
     """Triangulate 3D points for a given session.
 
     Args:
@@ -88,14 +90,16 @@
             the CameraGroup object must be the same as the order of the arrays
             along the camera axis.
         frames: A tuple structured as (start_frame, end_frame) containing the frame
             range to triangulate. The range is (inclusive, exclusive) and will be
             considered as the entire video if not otherwise specified.
         excluded_views: Names (not paths) of camera views to be excluded from
             triangulation. If not given, all views will be used.
+        ransac: A flag determining whether or not to use RANSAC based triangulation,
+            false by default.
         fname: The file path to save the triangulated points to (must end in .h5). Will
             not save unless a non-empty string is given.
         disp_progress: A flag determining whether or not to show triangulation
             progress, false by default.
         kwargs: Arguments related to filtering and limb constraints. Below are some of
             the more useful arguments, see the aniposelib for more details.
                 constraints: A Kx2 array for rigid limb constraints, default empty. An
@@ -167,15 +171,18 @@
         kwargs["constraints_weak"] = (
             [] if kwargs["constraints_weak"] is None else kwargs["constraints_weak"]
         )
 
     points_3d = np.stack(
         [
             cgroup.triangulate_optim(
-                points_2d[:, :, track], init_progress=disp_progress, **kwargs
+                points_2d[:, :, track],
+                init_ransac=ransac,
+                init_progress=disp_progress,
+                **kwargs,
             )
             for track in range(n_tracks)
         ],
         axis=1,
     )  # (n_frames, n_tracks, n_nodes, 3)
 
     if len(fname) > 0:
@@ -244,14 +251,23 @@
     help=(
         "Names (not paths) of camera views to be excluded from triangulation. Specified"
         " via multiple calls, i.e. --excluded_views top --excluded_views side. If not "
         "specified, all views will be used."
     ),
 )
 @click.option(
+    "--ransac",
+    is_flag=True,
+    default=False,
+    help=(
+        "Flag determining whether or not to use RANSAC based triangulation, "
+        "false by default."
+    ),
+)
+@click.option(
     "--disp_progress",
     is_flag=True,
     default=False,
     help="Flag determining whether or not to display triangulation progress.",
 )
 @click.option(
     "--constraints",
@@ -312,14 +328,15 @@
 )
 def triangulate_cli(
     p2d,
     calib,
     fname,
     frames,
     excluded_views,
+    ransac,
     disp_progress,
     constraints,
     constraints_weak,
     scale_smooth,
     scale_length,
     scale_length_weak,
     reproj_error_threshold,
@@ -338,14 +355,15 @@
 
     return triangulate(
         p2d,
         calib,
         frames,
         excluded_views,
         fname,
+        ransac,
         disp_progress,
         constraints=constraints,
         constraints_weak=constraints_weak,
         scale_smooth=scale_smooth,
         scale_length=scale_length,
         scale_length_weak=scale_length_weak,
         reproj_error_threshold=reproj_error_threshold,
```

## Comparing `sleap_anipose-0.1.6.dist-info/LICENSE` & `sleap_anipose-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sleap_anipose-0.1.6.dist-info/METADATA` & `sleap_anipose-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleap-anipose
-Version: 0.1.6
+Version: 0.1.7
 Summary: SLEAP to Anipose triangulation pipeline for 3D multi-animal pose tracking.
 Home-page: https://github.com/talmolab/sleap-anipose
 Author: Sean Afshar
 Author-email: safshar@salk.edu
 Maintainer: Talmo Pereira
 Maintainer-email: talmo@salk.edu
 License: BSD 3-Clause License
@@ -123,15 +123,15 @@
 The `metadata_fname` argument specifies the path to save the calibration metadata and it must end in .h5. This file contains some useful information about the board detections that were used for calibration, and more importantly, these board detections can later be used to assess the quality of calibration. **It is important to note that this file will not save unless the user inputs a path to save it to.**
 
 The `histogram_path` argument points to the path to save the histogram of reprojection errors to. Lastly, the `reproj_path` argument points to the session to save the images contrasting calibration board corner detections against reprojected corner positions. **It is important to note that neither of these files will save unless the user inputs a path to save them to.**
 
 8. Generate the triangulated 3D points based on your tracking and calibration:
 
 ```
-slap-triangulate --p2d my/path --calib my/path/calibration.toml --fname p3d.h5 --frames 1000 2000 --excluded_views side --excluded_view top --fname my/path/points3d.h5 --disp_progress True \
+slap-triangulate --p2d my/path --calib my/path/calibration.toml --fname my/path/points3d.h5 --frames 1000 2000 --excluded_views side --excluded_view top --disp_progress True \
 --constraints 0 1 --constraints 2 3 --weak_constraints 4 5 --scale_smooth 3 --scale_length 4 --scale_length_weak 1 --reproj_error_threshold 10 --reproj_loss l2 --n_deriv_smooth 2
 ```
 
 The required `p2d` argument points to the session containing the tracked and proofread files to be used for triangulation. 
 
 The required `calib` argument is a path pointing to the .toml file containing the results of calibration.
```

## Comparing `sleap_anipose-0.1.6.dist-info/RECORD` & `sleap_anipose-0.1.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-sleap_anipose/__init__.py,sha256=OzGszccL_t_my8aOA-7CpgtuntXs1lyGq42OmvLwZ1U,310
-sleap_anipose/calibration.py,sha256=dQgWc4cd0LRKQL2J-jK3BIoeHFRP6ytBH1V_hHHcKJ0,23044
-sleap_anipose/triangulation.py,sha256=mXpnzeaVCkYgIFkrGDNIXJpgYLUfm_HHrDceuJwOuEM,16020
-sleap_anipose-0.1.6.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-sleap_anipose-0.1.6.dist-info/METADATA,sha256=ExGdsHxeNjcK7AHFn6wSF0HUkoW4ArRH-upTSDvtJek,47440
-sleap_anipose-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sleap_anipose-0.1.6.dist-info/entry_points.txt,sha256=tBKkPWoPH6zHxjmdRRfRkdxhSuusz-OaYlUbxaC45lA,258
-sleap_anipose-0.1.6.dist-info/top_level.txt,sha256=tYlinljYJues5e7nUuFOb5B514t70h5KTMk54uG9-BA,14
-sleap_anipose-0.1.6.dist-info/RECORD,,
+sleap_anipose/__init__.py,sha256=69Os1mQU1iaTNQyxJsRPY0BxgG7Snx5h1inNrNSKZuk,310
+sleap_anipose/calibration.py,sha256=srkf9_F7IbcFW6of05h0fN5kdavf9tdW7zBZb3hFDDg,23027
+sleap_anipose/triangulation.py,sha256=_Z2_2IvQaxt5aA1zDl6mvD07F0zv4zJmshgLvl6pN3U,16596
+sleap_anipose-0.1.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+sleap_anipose-0.1.7.dist-info/METADATA,sha256=hYurw8k4pfxAHd0_zgrDPfyOu82ilSc6c862c0j7sno,47425
+sleap_anipose-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sleap_anipose-0.1.7.dist-info/entry_points.txt,sha256=tBKkPWoPH6zHxjmdRRfRkdxhSuusz-OaYlUbxaC45lA,258
+sleap_anipose-0.1.7.dist-info/top_level.txt,sha256=tYlinljYJues5e7nUuFOb5B514t70h5KTMk54uG9-BA,14
+sleap_anipose-0.1.7.dist-info/RECORD,,
```

