# Comparing `tmp/car_sound_dataset-1.3.1.tar.gz` & `tmp/car_sound_dataset-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/szakalosmatyas/Desktop/car_sound_dataset/dist/tmptocft6fz/car_sound_dataset-1.3.1.tar", last modified: Mon Oct 18 18:57:32 2021, max compression
+gzip compressed data, was "car_sound_dataset-1.3.2.tar", last modified: Tue Jun 13 10:51:17 2023, max compression
```

## Comparing `car_sound_dataset-1.3.1.tar` & `car_sound_dataset-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2021-10-18 18:57:32.584372 car_sound_dataset-1.3.1/
--rw-rw-r--   0 szakalosmatyas   (501) staff       (20)     1067 2021-08-09 08:05:58.000000 car_sound_dataset-1.3.1/LICENSE
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)     3595 2021-10-18 18:57:32.584046 car_sound_dataset-1.3.1/PKG-INFO
--rw-rw-r--   0 szakalosmatyas   (501) staff       (20)     2962 2021-08-17 13:57:56.000000 car_sound_dataset-1.3.1/README.md
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)       38 2021-10-18 18:57:32.584488 car_sound_dataset-1.3.1/setup.cfg
--rw-rw-r--   0 szakalosmatyas   (501) staff       (20)     1318 2021-10-18 18:56:38.000000 car_sound_dataset-1.3.1/setup.py
-drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2021-10-18 18:57:32.580107 car_sound_dataset-1.3.1/src/
-drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2021-10-18 18:57:32.581689 car_sound_dataset-1.3.1/src/car_sound_dataset/
--rw-rw-r--   0 szakalosmatyas   (501) staff       (20)        0 2021-07-26 06:29:02.000000 car_sound_dataset-1.3.1/src/car_sound_dataset/__init__.py
--rw-rw-r--   0 szakalosmatyas   (501) staff       (20)    19249 2021-10-18 18:49:28.000000 car_sound_dataset-1.3.1/src/car_sound_dataset/car_dataset.py
-drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2021-10-18 18:57:32.583593 car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)     3595 2021-10-18 18:57:32.000000 car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/PKG-INFO
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)      321 2021-10-18 18:57:32.000000 car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)        1 2021-10-18 18:57:32.000000 car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)       97 2021-10-18 18:57:32.000000 car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/requires.txt
--rw-r--r--   0 szakalosmatyas   (501) staff       (20)       18 2021-10-18 18:57:32.000000 car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2023-06-13 10:51:17.325042 car_sound_dataset-1.3.2/
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)     1068 2023-06-13 09:56:52.000000 car_sound_dataset-1.3.2/LICENSE
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)     3657 2023-06-13 10:51:17.324716 car_sound_dataset-1.3.2/PKG-INFO
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)     3061 2023-06-13 09:56:52.000000 car_sound_dataset-1.3.2/README.md
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)       38 2023-06-13 10:51:17.325159 car_sound_dataset-1.3.2/setup.cfg
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)     1340 2023-06-13 10:49:46.000000 car_sound_dataset-1.3.2/setup.py
+drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2023-06-13 10:51:17.321335 car_sound_dataset-1.3.2/src/
+drwxr-xr-x   0 szakalosmatyas   (501) staff       (20)        0 2023-06-13 10:51:17.324305 car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)     3657 2023-06-13 10:51:17.000000 car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)      250 2023-06-13 10:51:17.000000 car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)        1 2023-06-13 10:51:17.000000 car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)       89 2023-06-13 10:51:17.000000 car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/requires.txt
+-rw-r--r--   0 szakalosmatyas   (501) staff       (20)        1 2023-06-13 10:51:17.000000 car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/top_level.txt
```

### Comparing `car_sound_dataset-1.3.1/LICENSE` & `car_sound_dataset-1.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `car_sound_dataset-1.3.1/PKG-INFO` & `car_sound_dataset-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: car_sound_dataset
-Version: 1.3.1
+Version: 1.3.2
 Summary: You can use the car sound dataset with this Python package.
 Home-page: https://github.com/blahutszabi/car_sound_dataset
 Author: Szabolcs Blahut, Matyas Szakalos, Gyorgy Kalmar
 Author-email: blahutszabi@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/blahutszabi/car_sound_dataset/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # car_sound_dataset
 This repo contains the source code of car sound dataset Python package.
 
+https://pypi.org/project/car-sound-dataset/
+
+# How to install?
+pip install car-sound-dataset
+
 # About the dataset
 The dataset contains 17121 car sound events. Each event is recorded by at least 1 and maximum 6 devices.
 The length of each recording is 3 sec. The sample frequency was 3906 Hz during the measurements.
 You can download the dataset and select different recordings with this package. 
 
 # Class
 
@@ -40,18 +43,17 @@
             
            
 # Methods
 
         download_and_get_dataset()
             Downloads the dataset and the json file, which identifies the events.
 
-
         list_events_of_dict( car_dataset_dict)
             This method prints to console the event IDs of a car_dataset_dict.
-
+            
         plot_event(car_dataset_dict, event_id)
             You can plot an event with this method.
 
         play_event(car_dataset_dict, event_id, nomralize=True)
             You can play the recordings of an event with this method.
 
         filter_by_pattern(car_dataset_dict, pattern)
@@ -78,14 +80,10 @@
             This method loads the recordings into a 3D numpy array. In this case each element
             contains only one recording. The recordings of an event are split to single recordings.
 
         load_dict(car_dataset_dict, is_random = False, device_indexes = [])
             This method loads the recordings into a 3D numpy array. In this case each element
             contains events. One event usually contains more than one recordings.
 
-    
-
 
     
 
-
-
```

### Comparing `car_sound_dataset-1.3.1/README.md` & `car_sound_dataset-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # car_sound_dataset
 This repo contains the source code of car sound dataset Python package.
 
+https://pypi.org/project/car-sound-dataset/
+
+# How to install?
+pip install car-sound-dataset
+
 # About the dataset
 The dataset contains 17121 car sound events. Each event is recorded by at least 1 and maximum 6 devices.
 The length of each recording is 3 sec. The sample frequency was 3906 Hz during the measurements.
 You can download the dataset and select different recordings with this package. 
 
 # Class
 
@@ -23,18 +28,17 @@
             
            
 # Methods
 
         download_and_get_dataset()
             Downloads the dataset and the json file, which identifies the events.
 
-
         list_events_of_dict( car_dataset_dict)
             This method prints to console the event IDs of a car_dataset_dict.
-
+            
         plot_event(car_dataset_dict, event_id)
             You can plot an event with this method.
 
         play_event(car_dataset_dict, event_id, nomralize=True)
             You can play the recordings of an event with this method.
 
         filter_by_pattern(car_dataset_dict, pattern)
@@ -61,12 +65,10 @@
             This method loads the recordings into a 3D numpy array. In this case each element
             contains only one recording. The recordings of an event are split to single recordings.
 
         load_dict(car_dataset_dict, is_random = False, device_indexes = [])
             This method loads the recordings into a 3D numpy array. In this case each element
             contains events. One event usually contains more than one recordings.
 
-    
-
```

### Comparing `car_sound_dataset-1.3.1/setup.py` & `car_sound_dataset-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="car_sound_dataset",
-    version="1.3.1",
+    version="1.3.2",
     author="Szabolcs Blahut, Matyas Szakalos, Gyorgy Kalmar",
     author_email="blahutszabi@gmail.com",
     description="You can use the car sound dataset with this Python package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blahutszabi/car_sound_dataset",
     project_urls={
@@ -23,15 +23,16 @@
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
                         "setuptools>=42",
                         "wheel",
                         "requests",
-                        "googledrivedownloader",
+                        "gdown",
                         "matplotlib",
                         "scipy",
                         "numpy",
                         "sounddevice",
-                        "soundfile"
+                        "soundfile",
+                        "zipfile"
                       ],
-)
+)
```

### Comparing `car_sound_dataset-1.3.1/src/car_sound_dataset.egg-info/PKG-INFO` & `car_sound_dataset-1.3.2/src/car_sound_dataset.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: car-sound-dataset
-Version: 1.3.1
+Version: 1.3.2
 Summary: You can use the car sound dataset with this Python package.
 Home-page: https://github.com/blahutszabi/car_sound_dataset
 Author: Szabolcs Blahut, Matyas Szakalos, Gyorgy Kalmar
 Author-email: blahutszabi@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/blahutszabi/car_sound_dataset/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # car_sound_dataset
 This repo contains the source code of car sound dataset Python package.
 
+https://pypi.org/project/car-sound-dataset/
+
+# How to install?
+pip install car-sound-dataset
+
 # About the dataset
 The dataset contains 17121 car sound events. Each event is recorded by at least 1 and maximum 6 devices.
 The length of each recording is 3 sec. The sample frequency was 3906 Hz during the measurements.
 You can download the dataset and select different recordings with this package. 
 
 # Class
 
@@ -40,18 +43,17 @@
             
            
 # Methods
 
         download_and_get_dataset()
             Downloads the dataset and the json file, which identifies the events.
 
-
         list_events_of_dict( car_dataset_dict)
             This method prints to console the event IDs of a car_dataset_dict.
-
+            
         plot_event(car_dataset_dict, event_id)
             You can plot an event with this method.
 
         play_event(car_dataset_dict, event_id, nomralize=True)
             You can play the recordings of an event with this method.
 
         filter_by_pattern(car_dataset_dict, pattern)
@@ -78,14 +80,10 @@
             This method loads the recordings into a 3D numpy array. In this case each element
             contains only one recording. The recordings of an event are split to single recordings.
 
         load_dict(car_dataset_dict, is_random = False, device_indexes = [])
             This method loads the recordings into a 3D numpy array. In this case each element
             contains events. One event usually contains more than one recordings.
 
-    
-
 
     
 
-
-
```

