# Comparing `tmp/musicpy-6.77.tar.gz` & `tmp/musicpy-6.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\musicpy-6.77.tar", last modified: Sun Jun 11 16:03:43 2023, max compression
+gzip compressed data, was "dist\musicpy-6.78.tar", last modified: Tue Jun 13 15:18:26 2023, max compression
```

## Comparing `musicpy-6.77.tar` & `musicpy-6.78.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:03:43.000000 musicpy-6.77/
--rw-rw-rw-   0        0        0    27030 2021-09-24 07:05:14.000000 musicpy-6.77/LICENSE
--rw-rw-rw-   0        0        0       40 2021-10-04 19:46:56.000000 musicpy-6.77/MANIFEST.in
--rw-rw-rw-   0        0        0    16335 2023-06-11 16:03:44.000000 musicpy-6.77/PKG-INFO
--rw-rw-rw-   0        0        0    14214 2023-04-18 07:20:38.000000 musicpy-6.77/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 16:03:43.000000 musicpy-6.77/musicpy/
--rw-rw-rw-   0        0        0       90 2022-05-24 06:43:42.000000 musicpy-6.77/musicpy/__init__.py
--rw-rw-rw-   0        0        0   112637 2023-03-17 16:11:10.000000 musicpy-6.77/musicpy/algorithms.py
--rw-rw-rw-   0        0        0    10087 2023-05-15 13:49:00.000000 musicpy-6.77/musicpy/control.py
--rw-rw-rw-   0        0        0    21720 2023-03-06 07:58:48.000000 musicpy-6.77/musicpy/database.py
--rw-rw-rw-   0        0        0    59875 2023-05-04 08:43:22.000000 musicpy-6.77/musicpy/daw.py
--rw-rw-rw-   0        0        0    81582 2023-06-06 13:53:58.000000 musicpy-6.77/musicpy/musicpy.py
--rw-rw-rw-   0        0        0       38 2023-03-06 07:58:48.000000 musicpy-6.77/musicpy/requirements for musicpy daw.txt
--rw-rw-rw-   0        0        0       18 2022-10-11 02:50:12.000000 musicpy-6.77/musicpy/requirements.txt
--rw-rw-rw-   0        0        0   256516 2023-06-11 15:56:34.000000 musicpy-6.77/musicpy/structures.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:03:43.000000 musicpy-6.77/musicpy.egg-info/
--rw-rw-rw-   0        0        0    16335 2023-06-11 16:03:44.000000 musicpy-6.77/musicpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-11 16:03:44.000000 musicpy-6.77/musicpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:03:44.000000 musicpy-6.77/musicpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-11 16:03:44.000000 musicpy-6.77/musicpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 16:03:44.000000 musicpy-6.77/musicpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-11 16:03:44.000000 musicpy-6.77/setup.cfg
--rw-rw-rw-   0        0        0     1402 2023-06-11 15:57:18.000000 musicpy-6.77/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:18:26.000000 musicpy-6.78/
+-rw-rw-rw-   0        0        0    27030 2021-09-24 07:05:14.000000 musicpy-6.78/LICENSE
+-rw-rw-rw-   0        0        0       40 2021-10-04 19:46:56.000000 musicpy-6.78/MANIFEST.in
+-rw-rw-rw-   0        0        0    16335 2023-06-13 15:18:28.000000 musicpy-6.78/PKG-INFO
+-rw-rw-rw-   0        0        0    14214 2023-04-18 07:20:38.000000 musicpy-6.78/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 15:18:26.000000 musicpy-6.78/musicpy/
+-rw-rw-rw-   0        0        0       90 2022-05-24 06:43:42.000000 musicpy-6.78/musicpy/__init__.py
+-rw-rw-rw-   0        0        0   112637 2023-03-17 16:11:10.000000 musicpy-6.78/musicpy/algorithms.py
+-rw-rw-rw-   0        0        0    10087 2023-05-15 13:49:00.000000 musicpy-6.78/musicpy/control.py
+-rw-rw-rw-   0        0        0    21720 2023-03-06 07:58:48.000000 musicpy-6.78/musicpy/database.py
+-rw-rw-rw-   0        0        0    59875 2023-05-04 08:43:22.000000 musicpy-6.78/musicpy/daw.py
+-rw-rw-rw-   0        0        0    81582 2023-06-06 13:53:58.000000 musicpy-6.78/musicpy/musicpy.py
+-rw-rw-rw-   0        0        0       38 2023-03-06 07:58:48.000000 musicpy-6.78/musicpy/requirements for musicpy daw.txt
+-rw-rw-rw-   0        0        0       18 2022-10-11 02:50:12.000000 musicpy-6.78/musicpy/requirements.txt
+-rw-rw-rw-   0        0        0   257163 2023-06-13 14:17:38.000000 musicpy-6.78/musicpy/structures.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:18:26.000000 musicpy-6.78/musicpy.egg-info/
+-rw-rw-rw-   0        0        0    16335 2023-06-13 15:18:28.000000 musicpy-6.78/musicpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-13 15:18:28.000000 musicpy-6.78/musicpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:18:28.000000 musicpy-6.78/musicpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-13 15:18:28.000000 musicpy-6.78/musicpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 15:18:28.000000 musicpy-6.78/musicpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 15:18:28.000000 musicpy-6.78/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-06-13 14:19:58.000000 musicpy-6.78/setup.py
```

### Comparing `musicpy-6.77/LICENSE` & `musicpy-6.78/LICENSE`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/PKG-INFO` & `musicpy-6.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: musicpy
-Version: 6.77
+Version: 6.78
 Summary: Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms.
 Home-page: https://github.com/Rainbow-Dreamer/musicpy.git
 Author: Rainbow-Dreamer
 Author-email: 1036889495@qq.com
 License: LGPLv2.1
-Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.77.tar.gz
+Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.78.tar.gz
 Description: musicpy
         =======
         [中文](https://github.com/Rainbow-Dreamer/musicpy/blob/master/README_cn.md)
         
         Have you ever thought about writing music with codes in a very concise, human-readable syntax?
         
         Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms. It is easy to learn and write, easy to read, and incorporates a fully computerized music theory system.
```

### Comparing `musicpy-6.77/README.md` & `musicpy-6.78/README.md`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/musicpy/algorithms.py` & `musicpy-6.78/musicpy/algorithms.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/musicpy/control.py` & `musicpy-6.78/musicpy/control.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/musicpy/database.py` & `musicpy-6.78/musicpy/database.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/musicpy/daw.py` & `musicpy-6.78/musicpy/daw.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/musicpy/musicpy.py` & `musicpy-6.78/musicpy/musicpy.py`

 * *Files identical despite different names*

### Comparing `musicpy-6.77/musicpy/structures.py` & `musicpy-6.78/musicpy/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,16 @@
 
     def cut(self,
             ind1=0,
             ind2=None,
             start_time=0,
             cut_extra_duration=False,
             cut_extra_interval=False,
-            round_duration=False):
+            round_duration=False,
+            round_cut_interval=False):
         # get parts of notes between two bars
         temp = copy(self)
         find_start = False
         if ind1 <= start_time:
             find_start = True
             actual_start_time = start_time - ind1
         else:
@@ -325,14 +326,16 @@
         notes = temp.notes
         intervals = temp.interval
         length = len(notes)
         start_ind = 0
         to_ind = length
         for i in range(length):
             current_bar += intervals[i]
+            if round_cut_interval:
+                current_bar = float(Fraction(current_bar).limit_denominator())
             if (not find_start) and current_bar >= ind1:
                 start_ind = i + 1
                 find_start = True
                 actual_start_time = current_bar - ind1
             elif current_bar >= ind2:
                 to_ind = i + 1
                 break
@@ -382,34 +385,37 @@
                  bpm,
                  time1=0,
                  time2=None,
                  start_time=0,
                  normalize_tempo=False,
                  cut_extra_duration=False,
                  cut_extra_interval=False,
-                 round_duration=False):
+                 round_duration=False,
+                 round_cut_interval=False):
         if normalize_tempo:
             temp = copy(self)
             temp.normalize_tempo(bpm)
             return temp.cut_time(bpm=bpm,
                                  time1=time1,
                                  time2=time2,
                                  start_time=start_time,
                                  normalize_tempo=False,
                                  cut_extra_duration=cut_extra_duration,
                                  cut_extra_interval=cut_extra_interval,
-                                 round_duration=round_duration)
+                                 round_duration=round_duration,
+                                 round_cut_interval=round_cut_interval)
         bar_left = time1 / ((60 / bpm) * 4)
         bar_right = time2 / ((60 / bpm) * 4) if time2 is not None else None
         result = self.cut(ind1=bar_left,
                           ind2=bar_right,
                           start_time=start_time,
                           cut_extra_duration=cut_extra_duration,
                           cut_extra_interval=cut_extra_interval,
-                          round_duration=round_duration)
+                          round_duration=round_duration,
+                          round_cut_interval=round_cut_interval)
         return result
 
     def last_note_standardize(self):
         self.interval[-1] = self.notes[-1].duration
 
     def bars(self, start_time=0, mode=1, audio_mode=0, bpm=None):
         if mode == 0:
@@ -2127,26 +2133,27 @@
         return temp
 
     def from_rhythm(self, current_rhythm, set_duration=True):
         return mp.get_chords_from_rhythm(chords=self,
                                          current_rhythm=current_rhythm,
                                          set_duration=set_duration)
 
-    def fix_length(self, n, round_duration=False):
+    def fix_length(self, n, round_duration=False, round_cut_interval=False):
         current_bar = self.bars(mode=2, start_time=self.start_time)
         if current_bar < n:
             extra = n - current_bar
             result = self | extra
         elif current_bar > n:
             result = self.cut(0,
                               n,
                               start_time=self.start_time,
                               cut_extra_duration=True,
                               cut_extra_interval=True,
-                              round_duration=round_duration)
+                              round_duration=round_duration,
+                              round_cut_interval=round_cut_interval)
         else:
             result = copy(self)
         return result
 
     def is_empty(self):
         return not self.notes and not self.tempos and not self.pitch_bends and not self.other_messages
 
@@ -3790,24 +3797,26 @@
 
     def cut(self,
             ind1=0,
             ind2=None,
             correct=False,
             cut_extra_duration=False,
             cut_extra_interval=False,
-            round_duration=False):
+            round_duration=False,
+            round_cut_interval=False):
         merged_result, temp_bpm, start_time = self.merge()
         if ind1 < 0:
             ind1 = 0
         result = merged_result.cut(ind1,
                                    ind2,
                                    start_time,
                                    cut_extra_duration=cut_extra_duration,
                                    cut_extra_interval=cut_extra_interval,
-                                   round_duration=round_duration)
+                                   round_duration=round_duration,
+                                   round_cut_interval=round_cut_interval)
         offset = ind1
         temp = copy(self)
         start_time -= ind1
         if start_time < 0:
             start_time = 0
         temp.reconstruct(track=result,
                          start_time=start_time,
@@ -3847,29 +3856,31 @@
     def cut_time(self,
                  time1=0,
                  time2=None,
                  bpm=None,
                  start_time=0,
                  cut_extra_duration=False,
                  cut_extra_interval=False,
-                 round_duration=False):
+                 round_duration=False,
+                 round_cut_interval=False):
         temp = copy(self)
         temp.normalize_tempo()
         if bpm is not None:
             temp_bpm = bpm
         else:
             temp_bpm = temp.bpm
         bar_left = time1 / ((60 / temp_bpm) * 4)
         bar_right = time2 / (
             (60 / temp_bpm) * 4) if time2 is not None else temp.bars()
         result = temp.cut(bar_left,
                           bar_right,
                           cut_extra_duration=cut_extra_duration,
                           cut_extra_interval=cut_extra_interval,
-                          round_duration=round_duration)
+                          round_duration=round_duration,
+                          round_cut_interval=round_cut_interval)
         return result
 
     def get_bar(self, n):
         start_time = min(self.start_times)
         return self.cut(n + start_time, n + start_time)
 
     def firstnbars(self, n):
```

### Comparing `musicpy-6.77/musicpy.egg-info/PKG-INFO` & `musicpy-6.78/musicpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: musicpy
-Version: 6.77
+Version: 6.78
 Summary: Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms.
 Home-page: https://github.com/Rainbow-Dreamer/musicpy.git
 Author: Rainbow-Dreamer
 Author-email: 1036889495@qq.com
 License: LGPLv2.1
-Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.77.tar.gz
+Download-URL: https://github.com/Rainbow-Dreamer/musicpy/archive/6.78.tar.gz
 Description: musicpy
         =======
         [中文](https://github.com/Rainbow-Dreamer/musicpy/blob/master/README_cn.md)
         
         Have you ever thought about writing music with codes in a very concise, human-readable syntax?
         
         Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms. It is easy to learn and write, easy to read, and incorporates a fully computerized music theory system.
```

### Comparing `musicpy-6.77/setup.py` & `musicpy-6.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='musicpy',
     packages=find_packages(),
     package_data={'musicpy': ['./*']},
-    version='6.77',
+    version='6.78',
     license='LGPLv2.1',
     description=
     'Musicpy is a music programming language in Python designed to write music in very handy syntax through music theory and algorithms.',
     author='Rainbow-Dreamer',
     author_email='1036889495@qq.com',
     url='https://github.com/Rainbow-Dreamer/musicpy.git',
     download_url=
-    'https://github.com/Rainbow-Dreamer/musicpy/archive/6.77.tar.gz',
+    'https://github.com/Rainbow-Dreamer/musicpy/archive/6.78.tar.gz',
     keywords=[
         'music language', 'use codes to write music', 'music language for AI'
     ],
     install_requires=['mido-fix', 'pygame', 'dataclasses'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

