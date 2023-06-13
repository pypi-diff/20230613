# Comparing `tmp/philbot_voice-1.9.7.tar.gz` & `tmp/philbot_voice-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.9.7.tar", max compression
+gzip compressed data, was "philbot_voice-1.9.8.tar", max compression
```

## Comparing `philbot_voice-1.9.7.tar` & `philbot_voice-1.9.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/philbot-voice/__main__.py
--rw-r--r--   0        0        0    43475 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-12 21:08:36.028691 philbot_voice-1.9.7/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.7/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-13 08:19:09.915010 philbot_voice-1.9.8/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-13 08:19:09.915010 philbot_voice-1.9.8/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    43536 2023-06-13 08:19:09.915010 philbot_voice-1.9.8/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-13 08:19:09.915010 philbot_voice-1.9.8/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.9.8/PKG-INFO
```

### Comparing `philbot_voice-1.9.7/philbot-voice/voice.py` & `philbot_voice-1.9.8/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,24 +260,24 @@
                 return False
             self.last_timestamp = self.buffer[self.last_sequence].get_timestamp() - desired_frame_size
             self.last_sequence = self.last_sequence - 1
         # write packages and fill holes
         do_flush = False
         while len(self.buffer) > too_young_packages or (len(self.buffer) > 0 and self.buffer.get(self.last_sequence + 1)):
             sequence = self.last_sequence + 1
+            while not self.buffer.get(sequence):
+                sequence += 1
             packet = self.buffer.get(sequence)
-            if packet:
-                self.buffer.pop(sequence)
-            else:
-                packet = Packet(sequence, sequence * desired_frame_size, b"\x00" * desired_frame_size * sample_width * channels)
             if packet.get_timestamp() > self.last_timestamp + (desired_frame_size * min_pause_duration // frame_duration):
                 do_flush = True
                 break
+            self.buffer.pop(sequence)
+            self.file.writeframes(b"\x00" * sample_width * channels * desired_frame_size * (sequence - self.last_sequence - 1))
             self.file.writeframes(packet.get_pcm())
-            self.packages += 1
+            self.packages += sequence - self.last_sequence
             self.last_sequence = packet.get_sequence()
             self.last_timestamp = packet.get_timestamp()
         # check whether we ran out completely
         if len(self.buffer) == 0 and too_young_packages == 0:
             do_flush = True
         # flush if necessary
         if do_flush:
```

### Comparing `philbot_voice-1.9.7/pyproject.toml` & `philbot_voice-1.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.9.7"
+version = "1.9.8"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.9.7/PKG-INFO` & `philbot_voice-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.9.7
+Version: 1.9.8
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

