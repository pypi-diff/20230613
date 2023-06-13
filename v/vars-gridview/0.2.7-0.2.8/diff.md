# Comparing `tmp/vars_gridview-0.2.7.tar.gz` & `tmp/vars_gridview-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.2.7.tar", max compression
+gzip compressed data, was "vars_gridview-0.2.8.tar", max compression
```

## Comparing `vars_gridview-0.2.7.tar` & `vars_gridview-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1104 2022-11-08 18:34:42.170730 vars_gridview-0.2.7/LICENSE
--rw-r--r--   0        0        0     1194 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/README.md
--rw-r--r--   0        0        0      862 2023-06-08 21:20:02.027612 vars_gridview-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.7/vars_gridview/__init__.py
--rw-r--r--   0        0        0      865 2023-03-24 17:40:22.606615 vars_gridview-0.2.7/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    24010 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0    31829 2022-11-08 18:34:42.170730 vars_gridview-0.2.7/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.162730 vars_gridview-0.2.7/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     4963 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     6242 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0      633 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    27206 2023-06-08 21:20:02.027612 vars_gridview-0.2.7/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1733 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     1680 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5174 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0     7188 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2645 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     3815 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3008 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0     1887 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/lib/util.py
--rw-r--r--   0        0        0    10153 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.170730 vars_gridview-0.2.7/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    22676 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     2932 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    16306 2023-03-24 17:40:22.606615 vars_gridview-0.2.7/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0        0 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     2790 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.7/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0      710 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2004 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1194 2023-02-03 23:04:10.385326 vars_gridview-0.2.8/README.md
+-rw-r--r--   0        0        0      862 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-22 18:43:10.077134 vars_gridview-0.2.8/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    24010 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0    31829 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.185892 vars_gridview-0.2.8/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     4963 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     6242 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0      633 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    28311 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1733 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     1680 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5174 2023-06-13 16:10:14.348688 vars_gridview-0.2.8/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0     7188 2023-06-13 16:10:14.348688 vars_gridview-0.2.8/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2645 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     3815 2023-06-12 16:29:02.472896 vars_gridview-0.2.8/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3008 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     1887 2023-06-12 16:29:22.672801 vars_gridview-0.2.8/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    10361 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.2.8/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    22075 2023-06-13 17:16:13.762346 vars_gridview-0.2.8/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     2932 2023-02-17 22:27:04.731716 vars_gridview-0.2.8/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    16306 2023-03-22 18:43:10.077134 vars_gridview-0.2.8/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0        0 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     2790 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.2.8/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0      710 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2004 2023-02-17 22:27:04.735716 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0        0 2023-02-03 23:02:37.189892 vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 vars_gridview-0.2.8/setup.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.8/PKG-INFO
```

### Comparing `vars_gridview-0.2.7/LICENSE` & `vars_gridview-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/README.md` & `vars_gridview-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/pyproject.toml` & `vars_gridview-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.2.7"
+version = "0.2.8"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
```

### Comparing `vars_gridview-0.2.7/vars_gridview/assets/base_query.sql` & `vars_gridview-0.2.8/vars_gridview/assets/base_query.sql`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/assets/gridview.ui` & `vars_gridview-0.2.8/vars_gridview/assets/gridview.ui`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.2.8/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/annotation.py` & `vars_gridview-0.2.8/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/boxes.py` & `vars_gridview-0.2.8/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/constants.py` & `vars_gridview-0.2.8/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.2.8/vars_gridview/lib/image_mosaic.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,18 +57,21 @@
         self._init_graphics()
 
         self.verifier = verifier
 
         self.moment_image_data = {}
         self.moment_localizations = {}
         self.moment_video_data = {}
+        self.moment_mp4_data = {}
+        self.moment_timestamps = {}
         self.observation_data = {}
         self.moment_image_map = {}  # Big
         
         self.video_reference_uuid_to_mp4_video_reference = {}
+        self.video_sequences_by_name = {}
 
         self.moment_localizations = {}
         self.moment_ancillary_data = {}
 
         self.beholder_url = beholder_url
         self.beholder_api_key = beholder_api_key
 
@@ -138,60 +141,69 @@
                         "video_start_timestamp",
                         "video_uri",
                         "video_container",
                         "video_reference_uuid",
                         "video_sequence_name"
                     )
                 }
-
-                # Tag in video data where appropriate
+                
+                # Tag in video data
                 if video_data.get("video_uri", None) is not None:  # valid video
                     if imaged_moment_uuid not in self.moment_video_data:
                         self.moment_video_data[imaged_moment_uuid] = video_data
-
-                # Find the corresponding MP4 video reference for this video reference, if there is one
-                video_reference_uuid = query_item["video_reference_uuid"]
-                video_sequence_name = query_item["video_sequence_name"]
                 
-                original_video_start_timestamp = video_data["video_start_timestamp"]
-                    
-                elapsed_time_millis = video_data.get(
-                    "index_elapsed_time_millis", None
-                )
-                timecode = video_data.get("index_timecode", None)
-                recorded_timestamp = video_data.get("index_recorded_timestamp", None)
-
-                # Get annotation video time index
-                annotation_timestamp = get_timestamp(original_video_start_timestamp, recorded_timestamp, elapsed_time_millis, timecode)
+                # Observation data
+                recorded_timestamp = video_data["index_recorded_timestamp"]
+                elapsed_time_millis = video_data["index_elapsed_time_millis"]
+                timecode = video_data["index_timecode"]
+                
+                # Video sequence data
+                video_sequence_name = video_data["video_sequence_name"]
                 
-                if annotation_timestamp is not None and video_reference_uuid is not None and video_reference_uuid not in self.video_reference_uuid_to_mp4_video_reference:
+                # Video data
+                video_start_timestamp = video_data["video_start_timestamp"]
+                
+                # ------------------
+                
+                # Get full video sequence data if not already fetched
+                if video_sequence_name not in self.video_sequences_by_name:
+                    # Try to fetch
                     try:
-                        video_sequence = operations.get_video_sequence_by_name(video_sequence_name)
-                        for video in video_sequence["videos"]:
-                            # Extract video time bounds
-                            if "start_timestamp" not in video or "duration_millis" not in video:  # invalid video, can't use
-                                continue
-                            
-                            video_start_timestamp = parse_iso(video["start_timestamp"])
-                            video_end_timestamp = video_start_timestamp + timedelta(milliseconds=video["duration_millis"])
-                            
-                            if not (video_start_timestamp <= annotation_timestamp <= video_end_timestamp):  # Annotation is not in this video
-                                continue
-                            
-                            for video_reference in video["video_references"]:
-                                if video_reference.get("container", None) == "video/mp4":
-                                    self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = video_reference
-                                    video_data["proxy_mp4"] = video
-                                    break
-                            else:
-                                self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = None
-                    except requests.exceptions.HTTPError as e:
-                        LOGGER.error(f"Could not get video sequence data for name {video_sequence_name}: {e}")
-                        self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = None
+                        video_sequence_data = operations.get_video_sequence_by_name(
+                            video_sequence_name
+                        )
+                    except Exception as e:
+                        LOGGER.error(f"Failed to get video sequence data for {video_sequence_name}: {e}")
+                        video_sequence_data = None
+                    
+                    # Store in dict
+                    self.video_sequences_by_name[video_sequence_name] = video_sequence_data
+                
+                # ------------------
 
+                if imaged_moment_uuid not in self.moment_mp4_data:
+                    # Get imaged moment's time index
+                    moment_timestamp = get_timestamp(video_start_timestamp, recorded_timestamp, elapsed_time_millis, timecode)
+                    self.moment_timestamps[imaged_moment_uuid] = moment_timestamp
+                    
+                    if moment_timestamp is None:  # No timestamp, can't use
+                        continue
+                    
+                    # Find the corresponding MP4 video reference (in the same video sequence) for this imaged moment, if there is one
+                    mp4_video_data = self.find_mp4_video_data(video_sequence_name, moment_timestamp)
+                    
+                    if mp4_video_data is not None:
+                        LOGGER.debug(f"Found MP4 video reference {mp4_video_data['video_reference']['uuid']} for imaged moment {imaged_moment_uuid}")
+                    else:
+                        LOGGER.warning(f"Could not find MP4 video reference for imaged moment {imaged_moment_uuid}")
+                    
+                    self.moment_mp4_data[imaged_moment_uuid] = mp4_video_data
+                
+                # ------------------
+                
                 # Collect bounding boxes
                 if link_name == "bounding box":
                     if association_uuid in seen_associations:
                         continue
                     seen_associations.add(association_uuid)
 
                     json_loc = link_value
@@ -231,63 +243,42 @@
                 if (
                     imaged_moment_uuid in self.moment_image_map
                 ):  # Already downloaded, skip
                     LOGGER.debug("Skipping, already downloaded image for moment: {}".format(imaged_moment_uuid))
                     continue
 
                 if url is None:  # No image reference, need to use beholder
-                    original_video_data = self.moment_video_data[imaged_moment_uuid]
+                    video_data = self.moment_video_data[imaged_moment_uuid]
                     
                     # Find the video URI of the MP4 video
-                    video_uri = None
-                    original_video_reference_uuid = original_video_data["video_reference_uuid"]
-                    if original_video_reference_uuid is not None and original_video_reference_uuid in self.video_reference_uuid_to_mp4_video_reference:
-                        mp4_video_reference = self.video_reference_uuid_to_mp4_video_reference[original_video_reference_uuid]
-                        if mp4_video_reference is not None:
-                            video_uri = mp4_video_reference["uri"]
-                        else:
-                            LOGGER.warning(
-                                "No web video available for capture for moment: {}, skipping".format(
-                                    imaged_moment_uuid
-                                )
-                            )
-                            continue
-
-                    video_start_timestamp = original_video_data["video_start_timestamp"]  # TODO check this
-                    
-                    elapsed_time_millis = original_video_data.get(
-                        "index_elapsed_time_millis", None
-                    )
-                    timecode = original_video_data.get("index_timecode", None)
-                    recorded_timestamp = original_video_data.get("index_recorded_timestamp", None)
-
-                    # Get annotation video time index
-                    annotation_timestamp = get_timestamp(video_start_timestamp, recorded_timestamp, elapsed_time_millis, timecode)
+                    original_video_reference_uuid = video_data["video_reference_uuid"]
+                    if original_video_reference_uuid is None:
+                        LOGGER.error(f"Imaged moment {imaged_moment_uuid} has no video reference, skipping")
+                        continue
                     
-                    if annotation_timestamp is None:
-                        LOGGER.error(
-                            "No time index available for moment: {}, skipping".format(
-                                imaged_moment_uuid
-                            )
-                        )
+                    mp4_video_data = self.moment_mp4_data.get(imaged_moment_uuid, None)
+                    if mp4_video_data is None:
+                        LOGGER.warning(f"Imaged moment {imaged_moment_uuid} has no MP4 video reference, skipping")
                         continue
-
-                    # Compute the elapsed time in milliseconds
-                    elapsed_time_millis = round(
-                        (annotation_timestamp - video_start_timestamp).total_seconds()
-                        * 1000
-                    )
                     
+                    # Get the MP4 video data
+                    mp4_video_reference_uri = mp4_video_data["video_reference"]["uri"]
+                    mp4_video_start_timestamp = parse_iso(mp4_video_data["video"]["start_timestamp"])  # datetime
+                    moment_timestamp = self.moment_timestamps[imaged_moment_uuid]
+                    
+                    # Compute the offset in milliseconds
+                    elapsed_time_millis = round((moment_timestamp - mp4_video_start_timestamp).total_seconds() * 1000)
+
                     # Get the capture from beholder
-                    LOGGER.debug(f"Getting capture from beholder for moment: {imaged_moment_uuid} ({video_uri} @ {elapsed_time_millis} ms)")
+                    LOGGER.debug(f"Getting capture from beholder for moment: {imaged_moment_uuid} ({mp4_video_reference_uri} @ {elapsed_time_millis} ms)")
                     try:
                         res = requests.post(
                             beholder_url + "/capture",
                             json={
-                                "videoUrl": video_uri,
+                                "videoUrl": mp4_video_reference_uri,
                                 "elapsedTimeMillis": int(elapsed_time_millis),
                             },
                             headers={"X-Api-Key": self.beholder_api_key},
                         )
                         res.raise_for_status()
                     except Exception as e:
                         LOGGER.error(
@@ -359,14 +350,65 @@
                 rw.clicked.connect(rect_clicked_slot)
                 self._rect_widgets.append(rw)
 
                 localization.rect = rw  # Back reference
 
                 self.n_localizations += 1
 
+    def find_mp4_video_data(self, video_sequence_name: str, timestamp: datetime) -> Optional[dict]:
+        """
+        Find a video with an MP4 video reference for the given video sequence name and timestamp.
+        
+        Args:
+            video_sequence_name: The video sequence name
+            timestamp: The timestamp
+        
+        Returns:
+            The matching video data dict, or None if no match found
+        """
+        if video_sequence_name not in self.video_sequences_by_name:  # Video sequence not encountered
+            return None
+
+        video_sequence = self.video_sequences_by_name[video_sequence_name]
+        
+        if video_sequence is None:  # No info about this video sequence
+            return None
+        
+        videos = video_sequence.get("videos", [])
+        for video in videos:
+            video_duration_millis = video.get("duration_millis", None)
+            if video_duration_millis is None:  # No duration
+                continue
+            
+            video_start_timestamp = video.get("start_timestamp", None)
+            if video_start_timestamp is None:  # No start timestamp
+                continue
+            
+            # Compute datetime start-end range
+            video_start_timestamp = parse_iso(video_start_timestamp)
+            video_end_timestamp = video_start_timestamp + timedelta(milliseconds=video_duration_millis)
+            
+            if not (video_start_timestamp <= timestamp <= video_end_timestamp):  # Timestamp not in range
+                continue
+            
+            video_references = video.get("video_references", [])
+            for video_reference in video_references:
+                container = video_reference.get("container", None)
+                if container is None:  # No container
+                    continue
+                
+                if container != "video/mp4":  # Unsupported container
+                    continue
+                
+                return {
+                    "video": video,
+                    "video_reference": video_reference,
+                }
+        
+
     def sort_rect_widgets(self, sort_method: SortMethod):
         """
         Sort the rect widgets
         
         Args:
             sort_method: The sort method to use
         """
```

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/log.py` & `vars_gridview-0.2.8/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.2.8/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.2.8/vars_gridview/lib/m3/clients.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.2.8/vars_gridview/lib/m3/operations.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/raziel.py` & `vars_gridview-0.2.8/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/settings.py` & `vars_gridview-0.2.8/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.2.8/vars_gridview/lib/sort_methods.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/sql.py` & `vars_gridview-0.2.8/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/util.py` & `vars_gridview-0.2.8/vars_gridview/lib/util.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/lib/widgets.py` & `vars_gridview-0.2.8/vars_gridview/lib/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,21 @@
                 self.deleted = True
             except Exception as e:
                 LOGGER.error(f"Error deleting association {self.association_uuid} from rect widget: {e}")
         
         return self.deleted
 
     @property
+    def imaged_moment_uuid(self) -> str:
+        """
+        Get the UUID of the imaged moment associated with this rect widget.
+        """
+        return self.localization.imaged_moment_uuid
+
+    @property
     def observation_uuid(self) -> str:
         """
         Get the UUID of the observation associated with this rect widget.
         """
         return self.localization.observation_uuid
     
     @property
```

### Comparing `vars_gridview-0.2.7/vars_gridview/scripts/run.py` & `vars_gridview-0.2.8/vars_gridview/scripts/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -533,47 +533,36 @@
         """
         Open the video of the last selected ROI, if available
         """
         if not self.last_selected_rect:
             QtWidgets.QMessageBox.warning(self, "No ROI Selected", "No ROI selected.")
             return
 
-        # Get the annotation recorded datetime
-        annotation_datetime = self.last_selected_rect.annotation_datetime()
+        # Get the annotation imaged moment UUID
+        imaged_moment_uuid = self.last_selected_rect.imaged_moment_uuid
         
-        # Get the annotation video reference UUID and start timestamp
-        video_reference_uuid = self.last_selected_rect.video_data.get("video_reference_uuid", None)
-        proxy_mp4 = self.last_selected_rect.video_data.get("proxy_mp4", None)
-        if proxy_mp4 is None:
+        # Get the annotation MP4 video data
+        mp4_video_data = self.image_mosaic.moment_mp4_data.get(imaged_moment_uuid, None)
+        if mp4_video_data is None:
             QtWidgets.QMessageBox.warning(
                 self, "Missing Video", "ROI lacks MP4 video."
             )
             return
-            
-        video_start_datetime = proxy_mp4.get("start_timestamp", None)
         
-        # Exit if we don't have what we need
-        if annotation_datetime is None or video_reference_uuid is None or video_start_datetime is None:
-            QtWidgets.QMessageBox.warning(
-                self, "Missing Info", "ROI lacks necessary information to link video."
-            )
-            return
-        
-        # Get the MP4 video reference from the image mosaic, if available
-        mp4_video_reference = self.image_mosaic.video_reference_uuid_to_mp4_video_reference.get(video_reference_uuid, None)
-        if mp4_video_reference is None:
-            QtWidgets.QMessageBox.warning(
-                self, "Missing Video", "ROI lacks MP4 video."
-            )
-            return
+        mp4_video = mp4_video_data["video"]
+        mp4_video_reference = mp4_video_data["video_reference"]
 
         mp4_video_url = mp4_video_reference.get("uri", None)
+        mp4_start_timestamp = parse_iso(mp4_video["start_timestamp"])
+
+        # Get the annotation timestamp
+        annotation_datetime = self.image_mosaic.moment_timestamps[imaged_moment_uuid]
 
         # Compute the timedelta between the annotation and video start
-        annotation_timedelta = annotation_datetime - parse_iso(video_start_datetime)
+        annotation_timedelta = annotation_datetime - mp4_start_timestamp
 
         # Open the MP4 video at the computed timedelta (in seconds)
         annotation_seconds = max(annotation_timedelta.total_seconds(), 0)
         url = mp4_video_url + "#t={},{}".format(
             annotation_seconds, annotation_seconds + 1e-3
         )  # "pause" at the annotation
         webbrowser.open(url)
```

### Comparing `vars_gridview-0.2.7/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.2.8/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.2.8/vars_gridview/ui/QueryDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.2.8/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.2.8/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.7/PKG-INFO` & `vars_gridview-0.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.2.7
+Version: 0.2.8
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
```

