# Comparing `tmp/scospus-0.1.0.tar.gz` & `tmp/scospus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scospus-0.1.0.tar", last modified: Thu Feb 23 14:03:53 2023, max compression
+gzip compressed data, was "scospus-0.2.0.tar", last modified: Tue Jun 13 10:28:08 2023, max compression
```

## Comparing `scospus-0.1.0.tar` & `scospus-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 14:03:53.114613 scospus-0.1.0/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1097 2023-02-23 14:00:35.000000 scospus-0.1.0/LICENSE
--rw-r--r--   0 robertl   (1000) robertl   (1000)      669 2023-02-23 14:03:53.114613 scospus-0.1.0/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)     2601 2023-02-23 14:01:42.000000 scospus-0.1.0/README.md
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 14:03:53.111279 scospus-0.1.0/scospus/
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1832 2022-10-11 10:22:35.000000 scospus-0.1.0/scospus/__init__.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     3551 2023-01-24 13:25:55.000000 scospus-0.1.0/scospus/airbuscsv.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     2473 2022-08-18 15:45:55.000000 scospus-0.1.0/scospus/crc16.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     7920 2023-01-31 14:30:44.000000 scospus-0.1.0/scospus/dds.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)      518 2022-08-18 15:47:53.000000 scospus-0.1.0/scospus/enums.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1126 2022-10-11 10:23:58.000000 scospus-0.1.0/scospus/guess.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     1775 2022-10-10 08:57:20.000000 scospus-0.1.0/scospus/internal.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    12478 2023-01-31 14:13:25.000000 scospus-0.1.0/scospus/pus.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)      182 2022-08-18 15:58:37.000000 scospus-0.1.0/scospus/tc.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    12542 2023-02-16 15:34:54.000000 scospus-0.1.0/scospus/tm.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)       22 2022-08-18 15:39:39.000000 scospus-0.1.0/scospus/version.py
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-02-23 14:03:53.114613 scospus-0.1.0/scospus.egg-info/
--rw-r--r--   0 robertl   (1000) robertl   (1000)      669 2023-02-23 14:03:53.000000 scospus-0.1.0/scospus.egg-info/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)      379 2023-02-23 14:03:53.000000 scospus-0.1.0/scospus.egg-info/SOURCES.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2023-02-23 14:03:53.000000 scospus-0.1.0/scospus.egg-info/dependency_links.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       40 2023-02-23 14:03:53.000000 scospus-0.1.0/scospus.egg-info/requires.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)        8 2023-02-23 14:03:53.000000 scospus-0.1.0/scospus.egg-info/top_level.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)      786 2023-02-23 14:03:53.114613 scospus-0.1.0/setup.cfg
--rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2022-08-18 15:36:44.000000 scospus-0.1.0/setup.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-06-13 10:28:08.307147 scospus-0.2.0/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1097 2023-05-17 13:46:21.000000 scospus-0.2.0/LICENSE
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      720 2023-06-13 10:28:08.307147 scospus-0.2.0/PKG-INFO
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     2601 2023-05-17 13:46:21.000000 scospus-0.2.0/README.md
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-06-13 10:28:08.303814 scospus-0.2.0/scospus/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1832 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/__init__.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     3551 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/airbuscsv.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     2473 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/crc16.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     9649 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/dds.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      518 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/enums.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1126 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/guess.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1775 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/internal.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    12865 2023-06-09 10:04:56.000000 scospus-0.2.0/scospus/pus.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      182 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/tc.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)    12542 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/tm.py
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       21 2023-05-17 13:46:21.000000 scospus-0.2.0/scospus/version.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-06-13 10:28:08.307147 scospus-0.2.0/scospus.egg-info/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      720 2023-06-13 10:28:08.000000 scospus-0.2.0/scospus.egg-info/PKG-INFO
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      401 2023-06-13 10:28:08.000000 scospus-0.2.0/scospus.egg-info/SOURCES.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2023-06-13 10:28:08.000000 scospus-0.2.0/scospus.egg-info/dependency_links.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       40 2023-06-13 10:28:08.000000 scospus-0.2.0/scospus.egg-info/requires.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)        8 2023-06-13 10:28:08.000000 scospus-0.2.0/scospus.egg-info/top_level.txt
+-rw-r--r--   0 robertl   (1000) robertl   (1000)      861 2023-06-13 10:28:08.310480 scospus-0.2.0/setup.cfg
+-rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2023-05-17 13:46:21.000000 scospus-0.2.0/setup.py
+drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2023-06-13 10:28:08.307147 scospus-0.2.0/tests/
+-rw-r--r--   0 robertl   (1000) robertl   (1000)     1946 2023-05-17 13:46:21.000000 scospus-0.2.0/tests/test_parsing.py
```

### Comparing `scospus-0.1.0/LICENSE` & `scospus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/PKG-INFO` & `scospus-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: scospus
-Version: 0.1.0
+Version: 0.2.0
 Summary: PUS packet parsing with SCOS backing
 Home-page: https://gitlab.irf.se/irf/scospus
 Author: Robert Labudda
 Author-email: robert.labudda@irf.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
+
+README.md
```

### Comparing `scospus-0.1.0/README.md` & `scospus-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/__init__.py` & `scospus-0.2.0/scospus/__init__.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/airbuscsv.py` & `scospus-0.2.0/scospus/airbuscsv.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/crc16.py` & `scospus-0.2.0/scospus/crc16.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/dds.py` & `scospus-0.2.0/scospus/dds.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 You usually just want to use a ``DDSReader`` instance like this::
 
     for ddspacket in DDSReader('thatfile.dds'):
         print("Packet's timestamp:", ddspacket.timestamp)
         # extract a usable PUS packet using your SCOS instance:
         packet = ddspacket.payload.interprete(my_scos)
 
+DDS packets are represented by ``DDSPacket``. The PUS packet wrapped
+by the DDS packet are accessible by the ``payload`` member.
+
+To wrap a PUS packet in an DDS packet, use the ``DDSBuilder``.
+
 """
 import datetime
 import struct
 import enum
 import io
 from collections import namedtuple
 from pathlib import Path
@@ -50,68 +55,40 @@
 
 
 class TimeQuality(enum.Enum):
     """DDS packet time quality"""
     GOOD = 0
     INACCURATE = 1
     BAD = 2
+    UNKNOWN = -1
 
 
 class DDSPacket:
     """A DDS header with payload"""
 
+    FORMAT = ">IIIHHBB"
+
     def __init__(self, header):
         self.dds = header
-        self.payload = None
-        self._timestamp = None
+        self.payload = b''
         self.offset = -1
         """Byte offset position of this DDS packet in the source data stream"""
 
-    @property
-    def coarse_time(self):
-        return struct.unpack(">I", self.dds[0:4])[0]
-
-    @property
-    def fine_time(self):
-        return struct.unpack(">I", self.dds[4:8])[0]
-
-    @property
-    def timestamp(self):
-        """The DDS timestamp"""
-        if self._timestamp is None:
-            self._timestamp = datetime.datetime.fromtimestamp(self.coarse_time,
-                                                              tz=datetime.timezone.utc) + \
-                              datetime.timedelta(microseconds=self.fine_time)
-        return self._timestamp
-
-    @property
-    def groundstation(self):
-        """The ground station this packet is coming from"""
-        gsid = struct.unpack(">H", self.dds[12:14])
-        return GROUNDSTATIONS.get(gsid, GroundStation(gsid, '', 'Unknown'))
-
-    @property
-    def virtual_channel(self):
-        """Virtual Channel ID"""
-        return struct.unpack(">H", self.dds[14:16])
-
-    @property
-    def SLE(self):
-        """The packet's 'SLE' field"""
-        return self.dds[16]
-
-    @property
-    def time_quality(self):
-        """Time quality"""
-        return TimeQuality(self.dds[17])
-
-    @property
-    def length(self):
-        """The packet's 'length' field"""
-        return struct.unpack(">I", self.dds[8:12])[0]
+        self.coarse_time = 0
+        self.fine_time = 0
+        self.timestamp = datetime.datetime(1, 1, 1, 0, 0, 0,
+                                           tzinfo=datetime.timezone.utc)
+        self.groundstation = GROUNDSTATIONS[0]
+        self.virtual_channel = 0
+        self.SLE = 0
+        self.time_quality = TimeQuality.BAD
+        self.length = 0
+
+        if len(self.dds) > 0:
+            self.do_parse()
 
     def __len__(self):
         len_ = len(self.dds)
         if self.payload is not None:
             len_ += len(self.payload)
         return len_
 
@@ -124,14 +101,64 @@
             return [self.timestamp] + self.payload.sorting()
         return [self.timestamp]
 
     def __bytes__(self):
         return self.dds + bytes(self.payload)
 
     @classmethod
+    def wrap(cls, packet,
+             timestamp=None,
+             groundstation=None,
+             virtual_channel=None,
+             SLE=None,
+             time_quality=None):
+        """Create a new DDS packet that wraps the given packet"""
+        dds = cls(b'')
+
+        if timestamp is None:
+            timestamp = datetime.datetime.now(datetime.timezone.utc)
+
+        assert isinstance(timestamp, datetime.datetime)
+        assert timestamp.tzinfo is not None
+
+        coarse_time = int(timestamp.timestamp())
+        fine_time = int((timestamp.timestamp() - coarse_time)*1000000)
+
+        if groundstation is None:
+            groundstation = GROUNDSTATIONS[0]
+
+        if isinstance(groundstation, GroundStation):
+            groundstation = groundstation.id
+
+        if virtual_channel is None:
+            virtual_channel = 0
+
+        if SLE is None:
+            SLE = 0
+
+        if time_quality is None:
+            time_quality = TimeQuality.INACCURATE
+
+        if isinstance(time_quality, TimeQuality):
+            time_quality = time_quality.value
+
+        length = len(bytes(packet))
+
+        dds.dds = struct.pack(cls.FORMAT,
+                              coarse_time, fine_time,
+                              length,
+                              groundstation,
+                              virtual_channel,
+                              SLE,
+                              time_quality)
+        dds.do_parse()
+        dds.payload = packet
+        return dds
+
+    @classmethod
     def parse(cls, stream):
         """Parse a DDS packet from the ``stream``
 
         This will read out only the DDS header. It's up to you to read the
         remaining packet using ``DDSPacket.length`` as an indicator how long
         the following packet is.
         """
@@ -139,14 +166,33 @@
         blob = stream.read(18)
         if len(blob) < 18:
             raise EOFError()
         packet = DDSPacket(blob)
         packet.offset = offset
         return packet
 
+    def do_parse(self):
+        """Parse the usable values from the internal binary representation of the DDS header"""
+        values = struct.unpack(self.FORMAT, self.dds)
+        self.coarse_time = values[0]
+        self.fine_time = values[1]
+        self.length = values[2]
+        self.timestamp = datetime.datetime.fromtimestamp(self.coarse_time,
+                                                         tz=datetime.timezone.utc) + \
+                         datetime.timedelta(microseconds=self.fine_time)
+        gsid = values[3]
+        self.groundstation = GROUNDSTATIONS.get(gsid,
+                                                GroundStation(gsid, '', 'Unknown'))
+        self.virtual_channel = values[4]
+        self.SLE = values[5]
+        try:
+            self.time_quality = TimeQuality(values[6])
+        except ValueError:
+            self.time_quality = TimeQuality.UNKNOWN
+
     def __str__(self):
         return f"<DDS {self.timestamp} payload: {len(self.payload)} bytes>"
 
 
 class DDSReader:
     """State-aware reader for DDS files
```

### Comparing `scospus-0.1.0/scospus/enums.py` & `scospus-0.2.0/scospus/enums.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/guess.py` & `scospus-0.2.0/scospus/guess.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/internal.py` & `scospus-0.2.0/scospus/internal.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus/pus.py` & `scospus-0.2.0/scospus/pus.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def read_next(self):
         """Read the next PUS packet from the stream"""
         assert self.stream is not None
         self.position = self.stream.tell()
         try:
             return PUSPacket.parse(self.stream)
-        except EOFError:
+        except (EOFError, ValueError):
             return None
 
     def __next__(self):
         if self.stream is None:
             self.open()
         packet = self.read_next()
         if packet is None:
@@ -136,16 +136,15 @@
 
         return offset + self.as_interval()
 
     def as_interval(self):
         """Return the timestamp as an interval
 
         This function assumes that the timestamp really not absolute"""
-        return datetime.timedelta(seconds=self.coarse(),
-                                  microseconds=self.fine())
+        return datetime.timedelta(seconds=self.coarse() + self.fine()/0x10000)
 
     def strftime(self, pattern, offset=None):
         """Format the time according to `pattern`
 
         ``offset`` is passed into ``as_datetime``. It defines the offset to be
         used in case the timestamp is not absolute.
 
@@ -156,14 +155,22 @@
         if isinstance(other, datetime.datetime):
             return self.as_datetime() < other
         if isinstance(other, datetime.timedelta):
             return self.as_interval() < other
         assert isinstance(other, PUSTimestamp)
         return self.as_datetime() < other.as_datetime()
 
+    def __gt__(self, other):
+        if isinstance(other, datetime.datetime):
+            return self.as_datetime() > other
+        if isinstance(other, datetime.timedelta):
+            return self.as_interval() > other
+        assert isinstance(other, PUSTimestamp)
+        return self.as_datetime() > other.as_datetime()
+
     def __str__(self):
         return self.strftime('%Y-%m-%d %H:%M:%S')
 
 
 class PUSPacket:
     """A PUS packet"""
     def __init__(self):
@@ -269,16 +276,16 @@
 
         unpackbitwidth = bitwidth
         while unpackbitwidth not in uint_types and unpackbitwidth < 32:
             unpackbitwidth += 1
 
         if unpackbitwidth not in uint_types:
             # TODO - fix this code in case bit_offset != 0 and/or bits % 8 != 0
-            assert bit_offset == 0
-            assert bits % 8 == 0
+            # assert bit_offset == 0
+            # assert bits % 8 == 0
             return data
 
         value = uint_types[unpackbitwidth].unpack(data)
         value = (value >> (len(data)*8 - bit_offset - bits)) & (2**bits - 1)
 
         databytesize = math.ceil(bits/8.)
         exporttypestr, exportbytesize = unpack_uint_format(bits)
@@ -324,15 +331,15 @@
 
         if len(raw) < 6:
             raise EOFError()
 
         pus = PUSPacket()
         pus.version = (raw[0] & 0xe0) >> 5
         pus.type = PUSType((raw[0] & 0x10) >> 4)
-        has_dfh = ((raw[0] & 4) >> 2) == 1
+        has_dfh = ((raw[0] & 8) >> 3) == 1
         pus.apid = struct.unpack_from('>H', raw)[0] & 0x07ff
 
         pus.grouping = Grouping((raw[2] & 0xc0) >> 6)
         pus.sequence_count = struct.unpack_from('>H', raw[2:4])[0] & 0x3f
         pus.df_len = struct.unpack_from('>H', raw[4:6])[0] + 1
 
         payload = stream.read(pus.df_len)
@@ -358,15 +365,16 @@
         """What version this PUS packet is"""
         self.servicetype = (0, 0)
         """The (type, subtype) of this packet"""
         self.raw = b''
 
     def parse(self, data):
         """Extract PUS version and type/subtype from the header"""
-        assert len(data) >= 3
+        if len(data) < 3:
+            raise ValueError(f"Not enough data to parse a datafieldheader {len(data)}")
         self.raw = data[:]
         self.pus_version = (self.raw[0] >> 4) & 7
         self.servicetype = (self.raw[1], self.raw[2])
 
     def copy(self):
         """Create a deep copy of ``self``"""
         other = type(self)()
@@ -414,8 +422,8 @@
         self.header_flag = (self.raw[0] >> 7) & 1
         self.ack_flags = AckFlags(self.raw[0] & 0xf)
 
     def copy(self):
         other = super().copy()
         other.header_flag = self.header_flag
         other.ack_flags = self.ack_flags
-        return other
+        return other
```

### Comparing `scospus-0.1.0/scospus/tm.py` & `scospus-0.2.0/scospus/tm.py`

 * *Files identical despite different names*

### Comparing `scospus-0.1.0/scospus.egg-info/PKG-INFO` & `scospus-0.2.0/scospus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: scospus
-Version: 0.1.0
+Version: 0.2.0
 Summary: PUS packet parsing with SCOS backing
 Home-page: https://gitlab.irf.se/irf/scospus
 Author: Robert Labudda
 Author-email: robert.labudda@irf.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
+
+README.md
```

