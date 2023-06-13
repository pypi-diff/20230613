# Comparing `tmp/byteblowerll-2.20.0-cp39-cp39-win_amd64.whl.zip` & `tmp/byteblowerll-2.21.0a1757-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2741888 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-13 08:55 byteblowerll/__init__.py
--rw-rw-rw-  2.0 fat 10728448 b- defN 23-Feb-13 09:03 byteblowerll/_byteblower.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  1292853 b- defN 23-Feb-13 08:59 byteblowerll/byteblower.py
--rw-rw-rw-  2.0 fat       29 b- defN 23-Feb-13 09:03 byteblowerll-2.20.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5072 b- defN 23-Feb-13 09:03 byteblowerll-2.20.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Feb-13 09:03 byteblowerll-2.20.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Feb-13 09:03 byteblowerll-2.20.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      683 b- defN 23-Feb-13 09:03 byteblowerll-2.20.0.dist-info/RECORD
-8 files, 12027198 bytes uncompressed, 2740694 bytes compressed:  77.2%
+Zip file size: 2744822 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 07:06 byteblowerll/__init__.py
+-rw-rw-rw-  2.0 fat 10735104 b- defN 23-Jun-13 07:40 byteblowerll/_byteblower.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1293710 b- defN 23-Jun-13 07:35 byteblowerll/byteblower.py
+-rw-rw-rw-  2.0 fat       29 b- defN 23-Jun-13 07:40 byteblowerll-2.21.0a1757.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5077 b- defN 23-Jun-13 07:40 byteblowerll-2.21.0a1757.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-13 07:40 byteblowerll-2.21.0a1757.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-13 07:40 byteblowerll-2.21.0a1757.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      709 b- defN 23-Jun-13 07:40 byteblowerll-2.21.0a1757.dist-info/RECORD
+8 files, 12034744 bytes uncompressed, 2743576 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: byteblowerll/__init__.py
 Comment: 
 
-Filename: byteblowerll/_byteblower.cp39-win_amd64.pyd
+Filename: byteblowerll/_byteblower.cp311-win_amd64.pyd
 Comment: 
 
 Filename: byteblowerll/byteblower.py
 Comment: 
 
-Filename: byteblowerll-2.20.0.dist-info/LICENSE
+Filename: byteblowerll-2.21.0a1757.dist-info/LICENSE
 Comment: 
 
-Filename: byteblowerll-2.20.0.dist-info/METADATA
+Filename: byteblowerll-2.21.0a1757.dist-info/METADATA
 Comment: 
 
-Filename: byteblowerll-2.20.0.dist-info/WHEEL
+Filename: byteblowerll-2.21.0a1757.dist-info/WHEEL
 Comment: 
 
-Filename: byteblowerll-2.20.0.dist-info/top_level.txt
+Filename: byteblowerll-2.21.0a1757.dist-info/top_level.txt
 Comment: 
 
-Filename: byteblowerll-2.20.0.dist-info/RECORD
+Filename: byteblowerll-2.21.0a1757.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## byteblowerll/byteblower.py

```diff
@@ -27978,14 +27978,20 @@
         	print(outOfSequenceResult.PacketCountInvalidGet())
 
 
 
         """
         return _byteblower.OutOfSequenceResultSnapshot_PacketCountInvalidGet(self)
 
+    def PacketCountMissingGet(self):
+        return _byteblower.OutOfSequenceResultSnapshot_PacketCountMissingGet(self)
+
+    def BiggestSequenceNumberGapGet(self):
+        return _byteblower.OutOfSequenceResultSnapshot_BiggestSequenceNumberGapGet(self)
+
     def IntervalDurationGet(self):
         r"""
 
         Gets the *configured* duration of this results snapshot [NS].
 
         .. versionadded:: 2.3.0
 
@@ -28238,14 +28244,20 @@
         	print(outOfSequenceresultData.PacketCountInvalidGet())
 
 
 
         """
         return _byteblower.OutOfSequenceResultData_PacketCountInvalidGet(self)
 
+    def PacketCountMissingGet(self):
+        return _byteblower.OutOfSequenceResultData_PacketCountMissingGet(self)
+
+    def BiggestSequenceNumberGapGet(self):
+        return _byteblower.OutOfSequenceResultData_BiggestSequenceNumberGapGet(self)
+
     def IntervalDurationGet(self):
         r"""
 
         Gets the *configured* duration of this results snapshot [NS].
 
         .. versionadded:: 2.3.0
 
@@ -35744,14 +35756,17 @@
 
         	users = meetingpoint.UsersGet()
 
 
         """
         return _byteblower.MeetingPoint_UsersGet(self)
 
+    def ResultsRefreshAll(self):
+        return _byteblower.MeetingPoint_ResultsRefreshAll(self)
+
     def DevicesStart(self, inDevices):
         r"""
 
         Starts all the given Wireless Endpoints.
 
         :param endpoints: a list on which to start the traffic, triggers and HTTPClients
         :type endpoints: :class:`.WirelessEndpointList`
@@ -36943,17 +36958,20 @@
         return _byteblower.WirelessEndpoint_ScenarioHeartbeatIntervalGet(self)
 
     def ScenarioHeartbeatIntervalSet(self, arg2):
         r"""
 
         Sets the heartbeat interval to be used when a scenario is running.
 
-        .. note:: Setting the value to 0 will disable heartbeating.
+        The allowed value range is 0 (disabled, default) and maximum 86400000000000 (1 day).
+
+        When a value is below the minimum value supported by a specific Endpoint device, the supported value is taken.
+        When a value is above the upper threshold of 1 day, 1 day will be used.
 
-        .. note:: Setting the interval a value which is not supported by the WirelessEndpoint will set the interval to the lowest supported value.
+        .. note:: A value of max int64 (9223372036854775807) will disable heartbeating during scenarios.  From 2.22.0 on, this value will be a normal valid value.
 
         Example
 
         .. code-block:: python
            :emphasize-lines: 1
 
            self.wireless_endpoint.ScenarioHeartbeatIntervalSet(50000000000)
```

## Comparing `byteblowerll-2.20.0.dist-info/METADATA` & `byteblowerll-2.21.0a1757.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byteblowerll
-Version: 2.20.0
+Version: 2.21.0a1757
 Summary: Python API for the ByteBlower Traffic Generator
 Home-page: https://byteblower.com
 Author: ByteBlower
 Author-email: support.byteblower@excentis.com
 License: ByteBlower End User License Agreement
 Project-URL: API Documentation, https://api.byteblower.com
 Project-URL: Python example scripts, https://www.github.com/excentis/byteblower_python_examples
```

