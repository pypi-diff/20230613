# Comparing `tmp/renats-0.2.2a1.tar.gz` & `tmp/renats-0.2.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renats-0.2.2a1.tar", max compression
+gzip compressed data, was "renats-0.2.2a2.tar", max compression
```

## Comparing `renats-0.2.2a1.tar` & `renats-0.2.2a2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a1/README.md
--rw-r--r--   0        0        0      404 2023-06-12 13:58:33.138625 renats-0.2.2a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/__init__.py
--rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/__init__.py
--rw-r--r--   0        0        0      203 2023-06-09 15:07:54.484606 renats-0.2.2a1/renats/client/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4428 2023-06-12 10:50:01.221016 renats-0.2.2a1/renats/client/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      583 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/client/__pycache__/message.cpython-310.pyc
--rw-r--r--   0        0        0     1087 2023-06-12 10:50:01.229016 renats-0.2.2a1/renats/client/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0     1355 2023-06-12 10:56:15.311568 renats-0.2.2a1/renats/client/__pycache__/subscription.cpython-310.pyc
--rw-r--r--   0        0        0      809 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/base.py
--rw-r--r--   0        0        0     6389 2023-06-12 13:58:33.138625 renats-0.2.2a1/renats/client/client.py
--rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/handler.py
--rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/message.py
--rw-r--r--   0        0        0      937 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/parser.py
--rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/subscription.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/connection/__init__.py
--rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a1/renats/connection/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1693 2023-06-12 10:50:01.229016 renats-0.2.2a1/renats/connection/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2003 2023-06-12 10:50:01.233016 renats-0.2.2a1/renats/connection/__pycache__/tcp.cpython-310.pyc
--rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/connection/base.py
--rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/connection/connection.py
--rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/connection/tcp.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/protocol/__init__.py
--rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a1/renats/protocol/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      925 2023-06-09 14:42:32.158897 renats-0.2.2a1/renats/protocol/__pycache__/protocol.cpython-310.pyc
--rw-r--r--   0        0        0     2335 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/protocol/messages/__init__.py
--rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a1/renats/protocol/messages/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      863 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
--rw-r--r--   0        0        0     1926 2023-06-09 15:04:32.367916 renats-0.2.2a1/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
--rw-r--r--   0        0        0     2651 2023-06-09 15:41:51.790249 renats-0.2.2a1/renats/protocol/messages/__pycache__/service.cpython-310.pyc
--rw-r--r--   0        0        0     1711 2023-06-09 15:07:48.276584 renats-0.2.2a1/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
--rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a1/renats/protocol/messages/base.py
--rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/msg.py
--rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/pub.py
--rw-r--r--   0        0        0     1749 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/service.py
--rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/sub.py
--rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/protocol.py
--rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/utils.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a2/README.md
+-rw-r--r--   0        0        0      431 2023-06-13 13:46:33.268272 renats-0.2.2a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-13 13:17:27.752054 renats-0.2.2a2/renats/client/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1467 2023-06-13 13:28:47.718277 renats-0.2.2a2/renats/client/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     5403 2023-06-13 13:18:15.172206 renats-0.2.2a2/renats/client/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0      588 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/client/__pycache__/message.cpython-310.pyc
+-rw-r--r--   0        0        0     1107 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/client/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2399 2023-06-13 13:18:15.192206 renats-0.2.2a2/renats/client/__pycache__/subscription.cpython-310.pyc
+-rw-r--r--   0        0        0      912 2023-06-13 13:46:24.528236 renats-0.2.2a2/renats/client/base.py
+-rw-r--r--   0        0        0     6372 2023-06-13 13:46:37.700290 renats-0.2.2a2/renats/client/client.py
+-rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/handler.py
+-rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/message.py
+-rw-r--r--   0        0        0      937 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/parser.py
+-rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/client/subscription.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/connection/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a2/renats/connection/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1693 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/connection/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2003 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/connection/__pycache__/tcp.cpython-310.pyc
+-rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/connection/base.py
+-rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/connection/connection.py
+-rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/connection/tcp.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/protocol/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a2/renats/protocol/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/protocol/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      925 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/protocol/__pycache__/protocol.cpython-310.pyc
+-rw-r--r--   0        0        0     2335 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/protocol/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a2/renats/protocol/messages/__init__.py
+-rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a2/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a2/renats/protocol/messages/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      863 2023-06-13 13:17:27.772054 renats-0.2.2a2/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
+-rw-r--r--   0        0        0     1926 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
+-rw-r--r--   0        0        0     2341 2023-06-13 13:09:10.690155 renats-0.2.2a2/renats/protocol/messages/__pycache__/service.cpython-310.pyc
+-rw-r--r--   0        0        0     1650 2023-06-13 13:28:47.722277 renats-0.2.2a2/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
+-rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a2/renats/protocol/messages/base.py
+-rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/messages/msg.py
+-rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/messages/pub.py
+-rw-r--r--   0        0        0     1702 2023-06-13 13:46:24.528236 renats-0.2.2a2/renats/protocol/messages/service.py
+-rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/messages/sub.py
+-rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/protocol.py
+-rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a2/renats/protocol/utils.py
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a2/PKG-INFO
```

### Comparing `renats-0.2.2a1/README.md` & `renats-0.2.2a2/README.md`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/client/__pycache__/message.cpython-310.pyc` & `renats-0.2.2a2/renats/client/__pycache__/message.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 13:19:02 2023 UTC, .py size: 249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 6f0d 0d0a 0000 0000 c626 8364 f900 0000  o........&.d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 0801 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 000b 0000 0040 0000 0073 3000 0000  .......@...s0...
 00000060: 6500 5a01 6400 5a02 6408 6402 6503 6403  e.Z.d.Z.d.d.e.d.
 00000070: 6504 6404 6503 6405 6505 6503 6503 6602  e.d.e.d.e.e.e.f.
 00000080: 1900 6608 6406 6407 8405 5a06 6401 5300  ..f.d.d...Z.d.S.
 00000090: 2909 da07 4d65 7373 6167 654e da07 7375  )...MessageN..su
-000000a0: 626a 6563 74da 0770 6179 6c6f 6164 da08  bject..payload..
-000000b0: 7265 706c 795f 746f da07 6865 6164 6572  reply_to..header
-000000c0: 7363 0500 0000 0000 0000 0000 0000 0500  sc..............
-000000d0: 0000 0200 0000 4300 0000 731c 0000 007c  ......C...s....|
-000000e0: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
-000000f0: 027c 047c 005f 0364 0053 0029 014e 2904  .|.|._.d.S.).N).
-00000100: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00000110: 0500 0000 2905 da04 7365 6c66 7202 0000  ....)...selfr...
-00000120: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
-00000130: a900 7207 0000 00fa 442f 686f 6d65 2f72  ..r.....D/home/r
-00000140: 6573 7069 7265 6e73 2f68 616e 6469 6365  espirens/handice
-00000150: 652f 6465 7665 6c6f 702f 7765 622f 5265  e/develop/web/Re
-00000160: 4e41 5453 2f72 656e 6174 732f 636c 6965  NATS/renats/clie
-00000170: 6e74 2f6d 6573 7361 6765 2e70 79da 085f  nt/message.py.._
-00000180: 5f69 6e69 745f 5f02 0000 0073 0800 0000  _init__....s....
-00000190: 0601 0601 0601 0a01 7a10 4d65 7373 6167  ........z.Messag
-000001a0: 652e 5f5f 696e 6974 5f5f 2902 4e4e 2907  e.__init__).NN).
-000001b0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000001c0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000001d0: 6d65 5f5f da03 7374 72da 0562 7974 6573  me__..str..bytes
-000001e0: da04 6469 6374 7209 0000 0072 0700 0000  ..dictr....r....
-000001f0: 7207 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000200: 0100 0000 0100 0000 7304 0000 0008 0028  ........s......(
-00000210: 0172 0100 0000 4e29 0172 0100 0000 7207  .r....N).r....r.
-00000220: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
-00000230: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000240: 7302 0000 0012 00                        s......
+000000a0: 626a 6563 74da 0770 6179 6c6f 6164 da0d  bject..payload..
+000000b0: 7265 706c 795f 7375 626a 6563 74da 0768  reply_subject..h
+000000c0: 6561 6465 7273 6305 0000 0000 0000 0000  eadersc.........
+000000d0: 0000 0005 0000 0002 0000 0043 0000 0073  ...........C...s
+000000e0: 1c00 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
+000000f0: 7c03 7c00 5f02 7c04 7c00 5f03 6400 5300  |.|._.|.|._.d.S.
+00000100: 2901 4e29 0472 0200 0000 7203 0000 0072  ).N).r....r....r
+00000110: 0400 0000 7205 0000 0029 05da 0473 656c  ....r....)...sel
+00000120: 6672 0200 0000 7203 0000 0072 0400 0000  fr....r....r....
+00000130: 7205 0000 00a9 0072 0700 0000 fa44 2f68  r......r.....D/h
+00000140: 6f6d 652f 7265 7370 6972 656e 732f 6861  ome/respirens/ha
+00000150: 6e64 6963 6565 2f64 6576 656c 6f70 2f77  ndicee/develop/w
+00000160: 6562 2f52 654e 4154 532f 7265 6e61 7473  eb/ReNATS/renats
+00000170: 2f63 6c69 656e 742f 6d65 7373 6167 652e  /client/message.
+00000180: 7079 da08 5f5f 696e 6974 5f5f 0200 0000  py..__init__....
+00000190: 7308 0000 0006 0106 0106 010a 017a 104d  s............z.M
+000001a0: 6573 7361 6765 2e5f 5f69 6e69 745f 5f29  essage.__init__)
+000001b0: 024e 4e29 07da 085f 5f6e 616d 655f 5fda  .NN)...__name__.
+000001c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000001d0: 7561 6c6e 616d 655f 5fda 0373 7472 da05  ualname__..str..
+000001e0: 6279 7465 73da 0464 6963 7472 0900 0000  bytes..dictr....
+000001f0: 7207 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
+00000200: 0800 0000 7201 0000 0001 0000 0073 0400  ....r........s..
+00000210: 0000 0800 2801 7201 0000 004e 2901 7201  ....(.r....N).r.
+00000220: 0000 0072 0700 0000 7207 0000 0072 0700  ...r....r....r..
+00000230: 0000 7208 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000240: 3e01 0000 0073 0200 0000 1200            >....s......
```

### Comparing `renats-0.2.2a1/renats/client/__pycache__/parser.cpython-310.pyc` & `renats-0.2.2a2/renats/client/__pycache__/parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 10:01:18 2023 UTC, .py size: 914 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 eeec 8664 9203 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 a903 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6500 a00a 6406  m.Z.m.Z...e...d.
 00000070: a101 5a0b 6407 650c 6408 6502 6409 6508  ..Z.d.e.d.e.d.e.
@@ -43,26 +43,28 @@
 000002a0: 6365 652f 6465 7665 6c6f 702f 7765 622f  cee/develop/web/
 000002b0: 5265 4e41 5453 2f72 656e 6174 732f 636c  ReNATS/renats/cl
 000002c0: 6965 6e74 2f70 6172 7365 722e 7079 da09  ient/parser.py..
 000002d0: 7061 7273 655f 6d73 670b 0000 0073 1a00  parse_msg....s..
 000002e0: 0000 0280 0c01 0801 0801 1201 1a01 0201  ................
 000002f0: 0201 0201 0201 0601 0201 06fb 7219 0000  ............r...
 00000300: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00000310: 0000 0100 0000 c300 0000 7306 0000 0081  ..........s.....
-00000320: 0164 0053 0029 014e 7217 0000 0029 0272  .d.S.).Nr....).r
-00000330: 0700 0000 7208 0000 0072 1700 0000 7217  ....r....r....r.
-00000340: 0000 0072 1800 0000 da0a 7061 7273 655f  ...r......parse_
-00000350: 686d 7367 1a00 0000 7304 0000 0002 8004  hmsg....s.......
-00000360: 0172 1a00 0000 290f 720f 0000 00da 1672  .r....).r......r
-00000370: 656e 6174 732e 636f 6e6e 6563 7469 6f6e  enats.connection
-00000380: 2e62 6173 6572 0200 0000 da0f 7265 6e61  .baser......rena
-00000390: 7473 2e70 726f 746f 636f 6c72 0300 0000  ts.protocolr....
-000003a0: da1a 7265 6e61 7473 2e70 726f 746f 636f  ..renats.protoco
-000003b0: 6c2e 6578 6365 7074 696f 6e73 7204 0000  l.exceptionsr...
-000003c0: 00da 1c72 656e 6174 732e 7072 6f74 6f63  ...renats.protoc
-000003d0: 6f6c 2e6d 6573 7361 6765 732e 6d73 6772  ol.messages.msgr
-000003e0: 0500 0000 7206 0000 00da 0763 6f6d 7069  ....r......compi
-000003f0: 6c65 7211 0000 00da 0562 7974 6573 7219  ler......bytesr.
-00000400: 0000 0072 1a00 0000 7217 0000 0072 1700  ...r....r....r..
-00000410: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
-00000420: 6f64 756c 653e 0100 0000 7310 0000 0008  odule>....s.....
-00000430: 000c 020c 010c 0110 010a 0216 031a 0f    ...............
+00000310: 0000 0100 0000 c300 0000 7308 0000 0081  ..........s.....
+00000320: 0174 0083 0082 0129 014e 2901 da13 4e6f  .t.....).N)...No
+00000330: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00000340: 7229 0272 0700 0000 7208 0000 0072 1700  r).r....r....r..
+00000350: 0000 7217 0000 0072 1800 0000 da0a 7061  ..r....r......pa
+00000360: 7273 655f 686d 7367 1a00 0000 7304 0000  rse_hmsg....s...
+00000370: 0002 8006 0172 1b00 0000 290f 720f 0000  .....r....).r...
+00000380: 00da 1672 656e 6174 732e 636f 6e6e 6563  ...renats.connec
+00000390: 7469 6f6e 2e62 6173 6572 0200 0000 da0f  tion.baser......
+000003a0: 7265 6e61 7473 2e70 726f 746f 636f 6c72  renats.protocolr
+000003b0: 0300 0000 da1a 7265 6e61 7473 2e70 726f  ......renats.pro
+000003c0: 746f 636f 6c2e 6578 6365 7074 696f 6e73  tocol.exceptions
+000003d0: 7204 0000 00da 1c72 656e 6174 732e 7072  r......renats.pr
+000003e0: 6f74 6f63 6f6c 2e6d 6573 7361 6765 732e  otocol.messages.
+000003f0: 6d73 6772 0500 0000 7206 0000 00da 0763  msgr....r......c
+00000400: 6f6d 7069 6c65 7211 0000 00da 0562 7974  ompiler......byt
+00000410: 6573 7219 0000 0072 1b00 0000 7217 0000  esr....r....r...
+00000420: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000430: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+00000440: 0000 0008 000c 020c 010c 0110 010a 0216  ................
+00000450: 031a 0f                                  ...
```

### Comparing `renats-0.2.2a1/renats/client/client.py` & `renats-0.2.2a2/renats/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 from asyncio import Task
 from typing import Final
 
 import msgspec.json
 from typing_extensions import Self
 
 from . import parser
-from .base import NATS
+from .base import NATS, HeadersType
 from .message import Message
 from .subscription import Subscription, SubscriptionManager, SubscriptionCallbackType
 from ..connection.base import Connection
 from ..connection.tcp import TcpConnection
 from ..protocol import protocol
 from ..protocol.messages.msg import MsgProtocolMessage, HMsgProtocolMessage
 from ..protocol.messages.pub import PubProtocolMessage, HPubProtocolMessage
 from ..protocol.messages.service import InfoProtocolMessage, ConnectProtocolMessage
 from ..protocol.messages.sub import SubProtocolMessage, UnsubProtocolMessage
 
 DEFAULT_CONNECTION_TIMEOUT: Final[float] = 2
 DEFAULT_INFO_WAITING_TIMEOUT: Final[float] = 2
 
 CLIENT_LANGUAGE: Final[str] = "python3"
-CLIENT_VERSION: Final[str] = "0.2.2-alpha-1"
+CLIENT_VERSION: Final[str] = "0.2.2-alpha-2"
 
 CLIENT_CONNECTION_VERBOSE: Final[bool] = False
 CLIENT_CONNECTION_PEDANTIC: Final[bool] = True
 CLIENT_SUPPORT_HEADERS: Final[bool] = False
 
-HeadersType = dict[str, str]
-
 
 class NATSClient(NATS):
     def __init__(self):
         self._logger: logging.Logger = logging.getLogger(__name__)
         self._connection: Connection | None = None
         self._connection_info: InfoProtocolMessage | None = None
         self._handler_task: Task | None = None
```

### Comparing `renats-0.2.2a1/renats/client/handler.py` & `renats-0.2.2a2/renats/client/handler.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/client/parser.py` & `renats-0.2.2a2/renats/client/parser.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/client/subscription.py` & `renats-0.2.2a2/renats/client/subscription.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/connection/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a2/renats/connection/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 10:32:03 2023 UTC, .py size: 951 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 23f4 8664 b703 0000  o.......#..d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 b703 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
 00000040: 6402 6403 8400 6403 6501 8303 5a03 6404  d.d...d.e...Z.d.
 00000050: 5300 2905 e900 0000 0029 02da 0341 4243  S.)......)...ABC
 00000060: da0e 6162 7374 7261 6374 6d65 7468 6f64  ..abstractmethod
 00000070: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
```

### Comparing `renats-0.2.2a1/renats/connection/__pycache__/tcp.cpython-310.pyc` & `renats-0.2.2a2/renats/connection/__pycache__/tcp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 10:32:07 2023 UTC, .py size: 1099 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 27f4 8664 4b04 0000  o.......'..dK...
+00000000: 6f0d 0d0a 0000 0000 2923 8764 4b04 0000  o.......)#.dK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 6d02 5a02 0100 6403 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000060: 5a05 6401 5300 2907 e900 0000 004e 2902  Z.d.S.)......N).
 00000070: da0c 5374 7265 616d 5265 6164 6572 da0c  ..StreamReader..
```

### Comparing `renats-0.2.2a1/renats/connection/base.py` & `renats-0.2.2a2/renats/connection/base.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/connection/tcp.py` & `renats-0.2.2a2/renats/connection/tcp.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/protocol/__pycache__/exceptions.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/__pycache__/exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 14:32:00 2023 UTC, .py size: 530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e037 8364 1202 0000  o........7.d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 1202 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 4700  .....@...s4...G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 4700  d.d...d.e...Z.G.
 00000040: 6402 6403 8400 6403 6500 8303 5a02 4700  d.d...d.e...Z.G.
 00000050: 6404 6405 8400 6405 6500 8303 5a03 6406  d.d...d.e...Z.d.
 00000060: 5300 2907 6300 0000 0000 0000 0000 0000  S.).c...........
 00000070: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
```

### Comparing `renats-0.2.2a1/renats/protocol/__pycache__/protocol.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/__pycache__/protocol.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 13:31:51 2023 UTC, .py size: 668 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c729 8364 9c02 0000  o........).d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 9c02 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 2e01 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 6d03 5a03 0100 6403 5a04 6501 6505  l.m.Z...d.Z.e.e.
 00000050: 1900 6506 6404 3c00 6405 5a07 6501 6505  ..e.d.<.d.Z.e.e.
 00000060: 1900 6506 6406 3c00 6407 5a08 6501 6505  ..e.d.<.d.Z.e.e.
 00000070: 1900 6506 6408 3c00 6409 5a09 6501 6505  ..e.d.<.d.Z.e.e.
```

### Comparing `renats-0.2.2a1/renats/protocol/__pycache__/utils.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 14:44:25 2023 UTC, .py size: 1591 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c93a 8364 3706 0000  o........:.d7...
+00000000: 6f0d 0d0a 0000 0000 2923 8764 3706 0000  o.......)#.d7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 b600 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 5a00 6400 6402 6c01 6d02  d.d.l.Z.d.d.l.m.
 00000040: 5a02 0100 6403 5a03 6502 6504 1900 6505  Z...d.Z.e.e...e.
 00000050: 6404 3c00 6506 6503 8301 5a07 6502 6508  d.<.e.e...Z.e.e.
 00000060: 1900 6505 6405 3c00 6406 6509 650a 650a  ..e.d.<.d.e.e.e.
 00000070: 6602 1900 6407 6509 6504 6504 6602 1900  f...d.e.e.e.f...
```

### Comparing `renats-0.2.2a1/renats/protocol/exceptions.py` & `renats-0.2.2a2/renats/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/protocol/messages/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/messages/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/protocol/messages/__pycache__/msg.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/messages/__pycache__/msg.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 14:36:47 2023 UTC, .py size: 390 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ff38 8364 8601 0000  o........8.d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 8601 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 4700 6404 6405  ..d.e...Z.G.d.d.
 00000050: 8400 6405 6501 8303 5a03 6406 5300 2907  ..d.e...Z.d.S.).
 00000060: e900 0000 0029 01da 0653 7472 7563 7463  .....)...Structc
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `renats-0.2.2a1/renats/protocol/messages/__pycache__/pub.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/messages/__pycache__/pub.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 15:04:22 2023 UTC, .py size: 1574 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 763f 8364 2606 0000  o.......v?.d&...
+00000000: 6f0d 0d0a 0000 0000 2923 8764 2606 0000  o.......)#.d&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000050: 8400 6405 6501 8303 5a05 4700 6406 6407  ..d.e...Z.G.d.d.
 00000060: 8400 6407 6501 8303 5a06 6408 5300 2909  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 0653 7472 7563 74e9  .....)...Struct.
```

### Comparing `renats-0.2.2a1/renats/protocol/messages/__pycache__/service.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/messages/__pycache__/service.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 15:41:50 2023 UTC, .py size: 1872 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,166 +1,147 @@
-00000000: 6f0d 0d0a 0000 0000 3e48 8364 5007 0000  o.......>H.dP...
+00000000: 6f0d 0d0a 0000 0000 7e64 8864 a606 0000  o.......~d.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
+00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6500 a007 6405  d.l.m.Z...e...d.
-00000060: a101 5a08 4700 6406 6407 8400 6407 6503  ..Z.G.d.d...d.e.
-00000070: 8303 5a09 4700 6408 6409 8400 6409 6503  ..Z.G.d.d...d.e.
-00000080: 640a 640b 8d04 5a0a 4700 640c 640d 8400  d.d...Z.G.d.d...
-00000090: 640d 6503 8303 5a0b 6401 5300 290e e900  d.e...Z.d.S.)...
-000000a0: 0000 004e 2902 da06 5374 7275 6374 da05  ...N)...Struct..
-000000b0: 6669 656c 64e9 0100 0000 2901 da1b 5365  field.....)...Se
-000000c0: 7269 616c 697a 6162 6c65 5072 6f74 6f63  rializableProtoc
-000000d0: 6f6c 4d65 7373 6167 6573 1100 0000 5e49  olMessages....^I
-000000e0: 4e46 4f5c 732b 282e 2b29 5c72 5c6e 2463  NFO\s+(.+)\r\n$c
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0300 0000 4000 0000 734e 0100 0065 005a  ....@...sN...e.Z
-00000110: 0164 005a 0255 0064 015a 0365 0465 0564  .d.Z.U.d.Z.e.e.d
-00000120: 023c 0065 0465 0564 033c 0065 0465 0564  .<.e.e.d.<.e.e.d
-00000130: 043c 0065 0465 0564 053c 0065 0465 0564  .<.e.e.d.<.e.e.d
-00000140: 063c 0065 0665 0564 073c 0065 0765 0564  .<.e.e.d.<.e.e.d
-00000150: 083c 0065 0665 0564 093c 0065 0665 0564  .<.e.e.d.<.e.e.d
-00000160: 0a3c 0064 0b5a 0865 0664 0b42 0065 0564  .<.d.Z.e.d.B.e.d
-00000170: 0c3c 0064 0b5a 0965 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
-00000180: 0d3c 0064 0b5a 0a65 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
-00000190: 0e3c 0064 0b5a 0b65 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
-000001a0: 0f3c 0064 0b5a 0c65 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
-000001b0: 103c 0064 0b5a 0d65 0e65 0419 0064 0b42  .<.d.Z.e.e...d.B
-000001c0: 0065 0564 113c 0064 0b5a 0f65 0764 0b42  .e.d.<.d.Z.e.d.B
-000001d0: 0065 0564 123c 0064 0b5a 1065 0464 0b42  .e.d.<.d.Z.e.d.B
-000001e0: 0065 0564 133c 0064 0b5a 1165 0764 0b42  .e.d.<.d.Z.e.d.B
-000001f0: 0065 0564 143c 0064 0b5a 1265 0464 0b42  .e.d.<.d.Z.e.d.B
-00000200: 0065 0564 153c 0064 0b5a 1365 0464 0b42  .e.d.<.d.Z.e.d.B
-00000210: 0065 0564 163c 0064 0b5a 1465 0464 0b42  .e.d.<.d.Z.e.d.B
-00000220: 0065 0564 173c 0064 0b5a 1565 0464 0b42  .e.d.<.d.Z.e.d.B
-00000230: 0065 0564 183c 0064 0b5a 1665 0464 0b42  .e.d.<.d.Z.e.d.B
-00000240: 0065 0564 193c 0064 0b5a 1765 0464 0b42  .e.d.<.d.Z.e.d.B
-00000250: 0065 0564 1a3c 0064 0b53 0029 1bda 1349  .e.d.<.d.S.)...I
-00000260: 6e66 6f50 726f 746f 636f 6c4d 6573 7361  nfoProtocolMessa
-00000270: 6765 7a36 0a20 2020 204e 4154 5320 7072  gez6.    NATS pr
-00000280: 6f74 6f63 6f6c 206d 6573 7361 6765 206d  otocol message m
-00000290: 6f64 656c 2066 6f72 2049 4e46 4f20 6d65  odel for INFO me
-000002a0: 7373 6167 650a 2020 2020 da09 7365 7276  ssage.    ..serv
-000002b0: 6572 5f69 64da 0b73 6572 7665 725f 6e61  er_id..server_na
-000002c0: 6d65 da07 7665 7273 696f 6eda 0267 6fda  me..version..go.
-000002d0: 0468 6f73 74da 0470 6f72 74da 0768 6561  .host..port..hea
-000002e0: 6465 7273 da0b 6d61 785f 7061 796c 6f61  ders..max_payloa
-000002f0: 64da 0570 726f 746f 4eda 0963 6c69 656e  d..protoN..clien
-00000300: 745f 6964 da0d 6175 7468 5f72 6571 7569  t_id..auth_requi
-00000310: 7265 64da 0c74 6c73 5f72 6571 7569 7265  red..tls_require
-00000320: 64da 0a74 6c73 5f76 6572 6966 79da 0d74  d..tls_verify..t
-00000330: 6c73 5f61 7661 696c 6162 6c65 da0c 636f  ls_available..co
-00000340: 6e6e 6563 745f 7572 6c73 da03 6c64 6dda  nnect_urls..ldm.
-00000350: 0a67 6974 5f63 6f6d 6d69 74da 096a 6574  .git_commit..jet
-00000360: 7374 7265 616d da02 6970 da0d 636c 6965  stream..ip..clie
-00000370: 6e74 5f69 645f 7374 72da 0963 6c69 656e  nt_id_str..clien
-00000380: 745f 6970 da05 6e6f 6e63 65da 0763 6c75  t_ip..nonce..clu
-00000390: 7374 6572 da06 646f 6d61 696e 2918 da08  ster..domain)...
-000003a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000003b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000003c0: 5f5f da07 5f5f 646f 635f 5fda 0373 7472  __..__doc__..str
-000003d0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-000003e0: 5fda 0369 6e74 da04 626f 6f6c 7210 0000  _..int..boolr...
-000003f0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000400: 7214 0000 0072 1500 0000 da04 6c69 7374  r....r......list
-00000410: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000420: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
-00000430: 0000 0072 1d00 0000 721e 0000 00a9 0072  ...r....r......r
-00000440: 2800 0000 7228 0000 00fa 4f2f 686f 6d65  (...r(....O/home
-00000450: 2f72 6573 7069 7265 6e73 2f68 616e 6469  /respirens/handi
-00000460: 6365 652f 6465 7665 6c6f 702f 7765 622f  cee/develop/web/
-00000470: 5265 4e41 5453 2f72 656e 6174 732f 7072  ReNATS/renats/pr
-00000480: 6f74 6f63 6f6c 2f6d 6573 7361 6765 732f  otocol/messages/
-00000490: 7365 7276 6963 652e 7079 7206 0000 000b  service.pyr.....
-000004a0: 0000 0073 3400 0000 0a00 0401 0803 0801  ...s4...........
-000004b0: 0801 0801 0801 0801 0801 0801 0801 1001  ................
-000004c0: 1001 1001 1001 1001 1401 1001 1001 1001  ................
-000004d0: 1001 1001 1001 1001 1001 1401 7206 0000  ............r...
-000004e0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000004f0: 0000 0400 0000 4000 0000 7300 0100 0065  ......@...s....e
-00000500: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000510: 0564 023c 0065 0465 0564 033c 0065 0465  .d.<.e.e.d.<.e.e
-00000520: 0564 043c 0065 0665 0564 053c 0065 0665  .d.<.e.e.d.<.e.e
-00000530: 0564 063c 0064 075a 0765 0664 0742 0065  .d.<.d.Z.e.d.B.e
-00000540: 0564 083c 0064 075a 0865 0664 0742 0065  .d.<.d.Z.e.d.B.e
-00000550: 0564 093c 0065 0964 0764 0a64 0b8d 025a  .d.<.e.d.d.d...Z
-00000560: 0a65 0664 0742 0065 0564 0c3c 0064 075a  .e.d.B.e.d.<.d.Z
-00000570: 0b65 0664 0742 0065 0564 0d3c 0064 075a  .e.d.B.e.d.<.d.Z
-00000580: 0c65 0d64 0742 0065 0564 0e3c 0064 075a  .e.d.B.e.d.<.d.Z
-00000590: 0e65 0464 0742 0065 0564 0f3c 0064 075a  .e.d.B.e.d.<.d.Z
-000005a0: 0f65 0664 0742 0065 0564 103c 0064 075a  .e.d.B.e.d.<.d.Z
-000005b0: 1065 0664 0742 0065 0564 113c 0064 075a  .e.d.B.e.d.<.d.Z
-000005c0: 1165 0464 0742 0065 0564 123c 0064 075a  .e.d.B.e.d.<.d.Z
-000005d0: 1265 0464 0742 0065 0564 133c 0064 075a  .e.d.B.e.d.<.d.Z
-000005e0: 1365 0664 0742 0065 0564 143c 0064 1565  .e.d.B.e.d.<.d.e
-000005f0: 1466 0264 1664 1784 045a 1564 0753 0029  .f.d.d...Z.d.S.)
-00000600: 18da 1643 6f6e 6e65 6374 5072 6f74 6f63  ...ConnectProtoc
-00000610: 6f6c 4d65 7373 6167 657a 390a 2020 2020  olMessagez9.    
-00000620: 4e41 5453 2070 726f 746f 636f 6c20 6d65  NATS protocol me
-00000630: 7373 6167 6520 6d6f 6465 6c20 666f 7220  ssage model for 
-00000640: 434f 4e4e 4543 5420 6d65 7373 6167 650a  CONNECT message.
-00000650: 2020 2020 da07 7665 7262 6f73 65da 0870      ..verbose..p
-00000660: 6564 616e 7469 6372 1200 0000 da04 6c61  edanticr......la
-00000670: 6e67 7209 0000 004e da0a 6175 7468 5f74  ngr....N..auth_t
-00000680: 6f6b 656e da04 7573 6572 da04 7061 7373  oken..user..pass
-00000690: 2902 da07 6465 6661 756c 74da 046e 616d  )...default..nam
-000006a0: 65da 0870 6173 7377 6f72 6472 3200 0000  e..passwordr2...
-000006b0: da08 7072 6f74 6f63 6f6c da04 6563 686f  ..protocol..echo
-000006c0: da03 7369 67da 036a 7774 da0d 6e6f 5f72  ..sig..jwt..no_r
-000006d0: 6573 706f 6e64 6572 7372 0d00 0000 da04  espondersr......
-000006e0: 6e6b 6579 da06 7265 7475 726e 6301 0000  nkey..returnc...
-000006f0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000700: 0043 0000 0073 1400 0000 6401 7400 6a01  .C...s....d.t.j.
-00000710: a002 7c00 a101 1700 6402 1700 5300 2903  ..|.....d...S.).
-00000720: 7a84 0a20 2020 2020 2020 2044 756d 7020  z..        Dump 
-00000730: 4e41 5453 2070 726f 746f 636f 6c20 434f  NATS protocol CO
-00000740: 4e4e 4543 5420 6d65 7373 6167 6520 746f  NNECT message to
-00000750: 2062 7974 6573 0a20 2020 2020 2020 203a   bytes.        :
-00000760: 7265 7475 726e 3a20 4e41 5453 2070 726f  return: NATS pro
-00000770: 746f 636f 6c20 434f 4e4e 4543 5420 6d65  tocol CONNECT me
-00000780: 7373 6167 6520 6173 2062 7974 6573 2d65  ssage as bytes-e
-00000790: 6e63 6f64 6564 2073 7472 696e 670a 2020  ncoded string.  
-000007a0: 2020 2020 2020 7308 0000 0043 4f4e 4e45        s....CONNE
-000007b0: 4354 2073 0200 0000 0d0a 2903 da07 6d73  CT s......)...ms
-000007c0: 6773 7065 63da 046a 736f 6eda 0665 6e63  gspec..json..enc
-000007d0: 6f64 6529 01da 0473 656c 6672 2800 0000  ode)...selfr(...
-000007e0: 7228 0000 0072 2900 0000 da04 6475 6d70  r(...r).....dump
-000007f0: 3e00 0000 7302 0000 0014 057a 1b43 6f6e  >...s......z.Con
-00000800: 6e65 6374 5072 6f74 6f63 6f6c 4d65 7373  nectProtocolMess
-00000810: 6167 652e 6475 6d70 2916 721f 0000 0072  age.dump).r....r
-00000820: 2000 0000 7221 0000 0072 2200 0000 7226   ...r!...r"...r&
-00000830: 0000 0072 2400 0000 7223 0000 0072 2e00  ...r$...r#...r..
-00000840: 0000 722f 0000 0072 0300 0000 7233 0000  ..r/...r....r3..
-00000850: 0072 3200 0000 7234 0000 0072 2500 0000  .r2...r4...r%...
-00000860: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00000870: 3800 0000 720d 0000 0072 3900 0000 da05  8...r....r9.....
-00000880: 6279 7465 7372 3f00 0000 7228 0000 0072  bytesr?...r(...r
-00000890: 2800 0000 7228 0000 0072 2900 0000 722a  (...r(...r)...r*
-000008a0: 0000 0029 0000 0073 2600 0000 0a00 0401  ...)...s&.......
-000008b0: 0803 0801 0801 0801 0801 1001 1001 1801  ................
-000008c0: 1001 1001 1001 1001 1001 1001 1001 1001  ................
-000008d0: 1202 722a 0000 0054 2901 da0d 6f6d 6974  ..r*...T)...omit
-000008e0: 5f64 6566 6175 6c74 7363 0000 0000 0000  _defaultsc......
-000008f0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000900: 0000 731a 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-00000910: 0064 015a 0365 0465 0564 023c 0064 0353  .d.Z.e.e.d.<.d.S
-00000920: 0029 04da 1245 7272 5072 6f74 6f63 6f6c  .)...ErrProtocol
-00000930: 4d65 7373 6167 657a 350a 2020 2020 4e41  Messagez5.    NA
-00000940: 5453 2070 726f 746f 636f 6c20 6d65 7373  TS protocol mess
-00000950: 6167 6520 6d6f 6465 6c20 666f 7220 4552  age model for ER
-00000960: 5220 6d65 7373 6167 650a 2020 2020 da0d  R message.    ..
-00000970: 6572 726f 725f 6d65 7373 6167 654e 2906  error_messageN).
-00000980: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00000990: 2200 0000 7223 0000 0072 2400 0000 7228  "...r#...r$...r(
-000009a0: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-000009b0: 0000 7242 0000 0046 0000 0073 0600 0000  ..rB...F...s....
-000009c0: 0a00 0401 0c03 7242 0000 0029 0cda 0272  ......rB...)...r
-000009d0: 65da 0c6d 7367 7370 6563 2e6a 736f 6e72  e..msgspec.jsonr
-000009e0: 3b00 0000 7202 0000 0072 0300 0000 da04  ;...r....r......
-000009f0: 6261 7365 7205 0000 00da 0763 6f6d 7069  baser......compi
-00000a00: 6c65 da11 494e 464f 5f48 4541 445f 5041  le..INFO_HEAD_PA
-00000a10: 5454 4552 4e72 0600 0000 722a 0000 0072  TTERNr....r*...r
-00000a20: 4200 0000 7228 0000 0072 2800 0000 7228  B...r(...r(...r(
-00000a30: 0000 0072 2900 0000 da08 3c6d 6f64 756c  ...r).....<modul
-00000a40: 653e 0100 0000 7310 0000 0008 0008 0210  e>....s.........
-00000a50: 010c 020a 0210 0314 1e14 1d              ...........
+00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6500  d.l.m.Z.m.Z...e.
+00000050: a005 6403 a101 5a06 4700 6404 6405 8400  ..d...Z.G.d.d...
+00000060: 6405 6503 8303 5a07 4700 6406 6407 8400  d.e...Z.G.d.d...
+00000070: 6407 6503 6408 6409 8d04 5a08 6401 5300  d.e.d.d...Z.d.S.
+00000080: 290a e900 0000 004e 2902 da06 5374 7275  )......N)...Stru
+00000090: 6374 da05 6669 656c 6473 1100 0000 5e49  ct..fields....^I
+000000a0: 4e46 4f5c 732b 282e 2b29 5c72 5c6e 2463  NFO\s+(.+)\r\n$c
+000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000c0: 0300 0000 4000 0000 734e 0100 0065 005a  ....@...sN...e.Z
+000000d0: 0164 005a 0255 0064 015a 0365 0465 0564  .d.Z.U.d.Z.e.e.d
+000000e0: 023c 0065 0465 0564 033c 0065 0465 0564  .<.e.e.d.<.e.e.d
+000000f0: 043c 0065 0465 0564 053c 0065 0465 0564  .<.e.e.d.<.e.e.d
+00000100: 063c 0065 0665 0564 073c 0065 0765 0564  .<.e.e.d.<.e.e.d
+00000110: 083c 0065 0665 0564 093c 0065 0665 0564  .<.e.e.d.<.e.e.d
+00000120: 0a3c 0064 0b5a 0865 0664 0b42 0065 0564  .<.d.Z.e.d.B.e.d
+00000130: 0c3c 0064 0b5a 0965 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
+00000140: 0d3c 0064 0b5a 0a65 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
+00000150: 0e3c 0064 0b5a 0b65 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
+00000160: 0f3c 0064 0b5a 0c65 0764 0b42 0065 0564  .<.d.Z.e.d.B.e.d
+00000170: 103c 0064 0b5a 0d65 0e65 0419 0064 0b42  .<.d.Z.e.e...d.B
+00000180: 0065 0564 113c 0064 0b5a 0f65 0764 0b42  .e.d.<.d.Z.e.d.B
+00000190: 0065 0564 123c 0064 0b5a 1065 0464 0b42  .e.d.<.d.Z.e.d.B
+000001a0: 0065 0564 133c 0064 0b5a 1165 0764 0b42  .e.d.<.d.Z.e.d.B
+000001b0: 0065 0564 143c 0064 0b5a 1265 0464 0b42  .e.d.<.d.Z.e.d.B
+000001c0: 0065 0564 153c 0064 0b5a 1365 0464 0b42  .e.d.<.d.Z.e.d.B
+000001d0: 0065 0564 163c 0064 0b5a 1465 0464 0b42  .e.d.<.d.Z.e.d.B
+000001e0: 0065 0564 173c 0064 0b5a 1565 0464 0b42  .e.d.<.d.Z.e.d.B
+000001f0: 0065 0564 183c 0064 0b5a 1665 0464 0b42  .e.d.<.d.Z.e.d.B
+00000200: 0065 0564 193c 0064 0b5a 1765 0464 0b42  .e.d.<.d.Z.e.d.B
+00000210: 0065 0564 1a3c 0064 0b53 0029 1bda 1349  .e.d.<.d.S.)...I
+00000220: 6e66 6f50 726f 746f 636f 6c4d 6573 7361  nfoProtocolMessa
+00000230: 6765 7a36 0a20 2020 204e 4154 5320 7072  gez6.    NATS pr
+00000240: 6f74 6f63 6f6c 206d 6573 7361 6765 206d  otocol message m
+00000250: 6f64 656c 2066 6f72 2049 4e46 4f20 6d65  odel for INFO me
+00000260: 7373 6167 650a 2020 2020 da09 7365 7276  ssage.    ..serv
+00000270: 6572 5f69 64da 0b73 6572 7665 725f 6e61  er_id..server_na
+00000280: 6d65 da07 7665 7273 696f 6eda 0267 6fda  me..version..go.
+00000290: 0468 6f73 74da 0470 6f72 74da 0768 6561  .host..port..hea
+000002a0: 6465 7273 da0b 6d61 785f 7061 796c 6f61  ders..max_payloa
+000002b0: 64da 0570 726f 746f 4eda 0963 6c69 656e  d..protoN..clien
+000002c0: 745f 6964 da0d 6175 7468 5f72 6571 7569  t_id..auth_requi
+000002d0: 7265 64da 0c74 6c73 5f72 6571 7569 7265  red..tls_require
+000002e0: 64da 0a74 6c73 5f76 6572 6966 79da 0d74  d..tls_verify..t
+000002f0: 6c73 5f61 7661 696c 6162 6c65 da0c 636f  ls_available..co
+00000300: 6e6e 6563 745f 7572 6c73 da03 6c64 6dda  nnect_urls..ldm.
+00000310: 0a67 6974 5f63 6f6d 6d69 74da 096a 6574  .git_commit..jet
+00000320: 7374 7265 616d da02 6970 da0d 636c 6965  stream..ip..clie
+00000330: 6e74 5f69 645f 7374 72da 0963 6c69 656e  nt_id_str..clien
+00000340: 745f 6970 da05 6e6f 6e63 65da 0763 6c75  t_ip..nonce..clu
+00000350: 7374 6572 da06 646f 6d61 696e 2918 da08  ster..domain)...
+00000360: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000370: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000380: 5f5f da07 5f5f 646f 635f 5fda 0373 7472  __..__doc__..str
+00000390: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+000003a0: 5fda 0369 6e74 da04 626f 6f6c 720e 0000  _..int..boolr...
+000003b0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+000003c0: 7212 0000 0072 1300 0000 da04 6c69 7374  r....r......list
+000003d0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+000003e0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+000003f0: 0000 0072 1b00 0000 721c 0000 00a9 0072  ...r....r......r
+00000400: 2600 0000 7226 0000 00fa 4f2f 686f 6d65  &...r&....O/home
+00000410: 2f72 6573 7069 7265 6e73 2f68 616e 6469  /respirens/handi
+00000420: 6365 652f 6465 7665 6c6f 702f 7765 622f  cee/develop/web/
+00000430: 5265 4e41 5453 2f72 656e 6174 732f 7072  ReNATS/renats/pr
+00000440: 6f74 6f63 6f6c 2f6d 6573 7361 6765 732f  otocol/messages/
+00000450: 7365 7276 6963 652e 7079 7204 0000 0009  service.pyr.....
+00000460: 0000 0073 3400 0000 0a00 0401 0803 0801  ...s4...........
+00000470: 0801 0801 0801 0801 0801 0801 0801 1001  ................
+00000480: 1001 1001 1001 1001 1401 1001 1001 1001  ................
+00000490: 1001 1001 1001 1001 1001 1401 7204 0000  ............r...
+000004a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000004b0: 0000 0400 0000 4000 0000 7300 0100 0065  ......@...s....e
+000004c0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+000004d0: 0564 023c 0065 0465 0564 033c 0065 0465  .d.<.e.e.d.<.e.e
+000004e0: 0564 043c 0065 0665 0564 053c 0065 0665  .d.<.e.e.d.<.e.e
+000004f0: 0564 063c 0064 075a 0765 0664 0742 0065  .d.<.d.Z.e.d.B.e
+00000500: 0564 083c 0064 075a 0865 0664 0742 0065  .d.<.d.Z.e.d.B.e
+00000510: 0564 093c 0065 0964 0764 0a64 0b8d 025a  .d.<.e.d.d.d...Z
+00000520: 0a65 0664 0742 0065 0564 0c3c 0064 075a  .e.d.B.e.d.<.d.Z
+00000530: 0b65 0664 0742 0065 0564 0d3c 0064 075a  .e.d.B.e.d.<.d.Z
+00000540: 0c65 0d64 0742 0065 0564 0e3c 0064 075a  .e.d.B.e.d.<.d.Z
+00000550: 0e65 0464 0742 0065 0564 0f3c 0064 075a  .e.d.B.e.d.<.d.Z
+00000560: 0f65 0664 0742 0065 0564 103c 0064 075a  .e.d.B.e.d.<.d.Z
+00000570: 1065 0664 0742 0065 0564 113c 0064 075a  .e.d.B.e.d.<.d.Z
+00000580: 1165 0464 0742 0065 0564 123c 0064 075a  .e.d.B.e.d.<.d.Z
+00000590: 1265 0464 0742 0065 0564 133c 0064 075a  .e.d.B.e.d.<.d.Z
+000005a0: 1365 0664 0742 0065 0564 143c 0064 1565  .e.d.B.e.d.<.d.e
+000005b0: 1466 0264 1664 1784 045a 1564 0753 0029  .f.d.d...Z.d.S.)
+000005c0: 18da 1643 6f6e 6e65 6374 5072 6f74 6f63  ...ConnectProtoc
+000005d0: 6f6c 4d65 7373 6167 657a 390a 2020 2020  olMessagez9.    
+000005e0: 4e41 5453 2070 726f 746f 636f 6c20 6d65  NATS protocol me
+000005f0: 7373 6167 6520 6d6f 6465 6c20 666f 7220  ssage model for 
+00000600: 434f 4e4e 4543 5420 6d65 7373 6167 650a  CONNECT message.
+00000610: 2020 2020 da07 7665 7262 6f73 65da 0870      ..verbose..p
+00000620: 6564 616e 7469 6372 1000 0000 da04 6c61  edanticr......la
+00000630: 6e67 7207 0000 004e da0a 6175 7468 5f74  ngr....N..auth_t
+00000640: 6f6b 656e da04 7573 6572 da04 7061 7373  oken..user..pass
+00000650: 2902 da07 6465 6661 756c 74da 046e 616d  )...default..nam
+00000660: 65da 0870 6173 7377 6f72 6472 3000 0000  e..passwordr0...
+00000670: da08 7072 6f74 6f63 6f6c da04 6563 686f  ..protocol..echo
+00000680: da03 7369 67da 036a 7774 da0d 6e6f 5f72  ..sig..jwt..no_r
+00000690: 6573 706f 6e64 6572 7372 0b00 0000 da04  espondersr......
+000006a0: 6e6b 6579 da06 7265 7475 726e 6301 0000  nkey..returnc...
+000006b0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+000006c0: 0043 0000 0073 1400 0000 6401 7400 6a01  .C...s....d.t.j.
+000006d0: a002 7c00 a101 1700 6402 1700 5300 2903  ..|.....d...S.).
+000006e0: 7a84 0a20 2020 2020 2020 2044 756d 7020  z..        Dump 
+000006f0: 4e41 5453 2070 726f 746f 636f 6c20 434f  NATS protocol CO
+00000700: 4e4e 4543 5420 6d65 7373 6167 6520 746f  NNECT message to
+00000710: 2062 7974 6573 0a20 2020 2020 2020 203a   bytes.        :
+00000720: 7265 7475 726e 3a20 4e41 5453 2070 726f  return: NATS pro
+00000730: 746f 636f 6c20 434f 4e4e 4543 5420 6d65  tocol CONNECT me
+00000740: 7373 6167 6520 6173 2062 7974 6573 2d65  ssage as bytes-e
+00000750: 6e63 6f64 6564 2073 7472 696e 670a 2020  ncoded string.  
+00000760: 2020 2020 2020 7308 0000 0043 4f4e 4e45        s....CONNE
+00000770: 4354 2073 0200 0000 0d0a 2903 da07 6d73  CT s......)...ms
+00000780: 6773 7065 63da 046a 736f 6eda 0665 6e63  gspec..json..enc
+00000790: 6f64 6529 01da 0473 656c 6672 2600 0000  ode)...selfr&...
+000007a0: 7226 0000 0072 2700 0000 da04 6475 6d70  r&...r'.....dump
+000007b0: 3c00 0000 7302 0000 0014 057a 1b43 6f6e  <...s......z.Con
+000007c0: 6e65 6374 5072 6f74 6f63 6f6c 4d65 7373  nectProtocolMess
+000007d0: 6167 652e 6475 6d70 2916 721d 0000 0072  age.dump).r....r
+000007e0: 1e00 0000 721f 0000 0072 2000 0000 7224  ....r....r ...r$
+000007f0: 0000 0072 2200 0000 7221 0000 0072 2c00  ...r"...r!...r,.
+00000800: 0000 722d 0000 0072 0300 0000 7231 0000  ..r-...r....r1..
+00000810: 0072 3000 0000 7232 0000 0072 2300 0000  .r0...r2...r#...
+00000820: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
+00000830: 3600 0000 720b 0000 0072 3700 0000 da05  6...r....r7.....
+00000840: 6279 7465 7372 3d00 0000 7226 0000 0072  bytesr=...r&...r
+00000850: 2600 0000 7226 0000 0072 2700 0000 7228  &...r&...r'...r(
+00000860: 0000 0027 0000 0073 2600 0000 0a00 0401  ...'...s&.......
+00000870: 0803 0801 0801 0801 0801 1001 1001 1801  ................
+00000880: 1001 1001 1001 1001 1001 1001 1001 1001  ................
+00000890: 1202 7228 0000 0054 2901 da0d 6f6d 6974  ..r(...T)...omit
+000008a0: 5f64 6566 6175 6c74 7329 09da 0272 65da  _defaults)...re.
+000008b0: 0c6d 7367 7370 6563 2e6a 736f 6e72 3900  .msgspec.jsonr9.
+000008c0: 0000 7202 0000 0072 0300 0000 da07 636f  ..r....r......co
+000008d0: 6d70 696c 65da 1149 4e46 4f5f 4845 4144  mpile..INFO_HEAD
+000008e0: 5f50 4154 5445 524e 7204 0000 0072 2800  _PATTERNr....r(.
+000008f0: 0000 7226 0000 0072 2600 0000 7226 0000  ..r&...r&...r&..
+00000900: 0072 2700 0000 da08 3c6d 6f64 756c 653e  .r'.....<module>
+00000910: 0100 0000 730c 0000 0008 0008 0210 010a  ....s...........
+00000920: 0210 0318 1e                             .....
```

### Comparing `renats-0.2.2a1/renats/protocol/messages/__pycache__/sub.cpython-310.pyc` & `renats-0.2.2a2/renats/protocol/messages/__pycache__/sub.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 15:04:22 2023 UTC, .py size: 1213 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,107 +1,104 @@
-00000000: 6f0d 0d0a 0000 0000 763f 8364 bd04 0000  o.......v?.d....
+00000000: 6f0d 0d0a 0000 0000 2923 8764 8f04 0000  o.......)#.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
+00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
-00000060: 6501 8303 5a07 4700 6408 6409 8400 6409  e...Z.G.d.d...d.
-00000070: 6501 8303 5a08 640a 5300 290b e900 0000  e...Z.d.S.).....
-00000080: 0029 01da 0653 7472 7563 74e9 0100 0000  .)...Struct.....
-00000090: 2901 da1b 5365 7269 616c 697a 6162 6c65  )...Serializable
-000000a0: 5072 6f74 6f63 6f6c 4d65 7373 6167 65e9  ProtocolMessage.
-000000b0: 0200 0000 2902 da05 7574 696c 73da 0870  ....)...utils..p
-000000c0: 726f 746f 636f 6c63 0000 0000 0000 0000  rotocolc........
-000000d0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000000e0: 7340 0000 0065 005a 0164 005a 0255 0064  s@...e.Z.d.Z.U.d
-000000f0: 015a 0365 0465 0564 023c 0065 0465 0564  .Z.e.e.d.<.e.e.d
-00000100: 033c 0064 045a 0665 0464 0442 0065 0564  .<.d.Z.e.d.B.e.d
-00000110: 053c 0064 0665 0766 0264 0764 0884 045a  .<.d.e.f.d.d...Z
-00000120: 0864 0453 0029 09da 1253 7562 5072 6f74  .d.S.)...SubProt
-00000130: 6f63 6f6c 4d65 7373 6167 657a 350a 2020  ocolMessagez5.  
-00000140: 2020 4e41 5453 2070 726f 746f 636f 6c20    NATS protocol 
-00000150: 6d65 7373 6167 6520 6d6f 6465 6c20 666f  message model fo
-00000160: 7220 5355 4220 6d65 7373 6167 650a 2020  r SUB message.  
-00000170: 2020 da07 7375 626a 6563 74da 0373 6964    ..subject..sid
-00000180: 4eda 0b71 7565 7565 5f67 726f 7570 da06  N..queue_group..
-00000190: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-000001a0: 0000 0002 0000 0007 0000 0043 0000 0073  ...........C...s
-000001b0: 3c00 0000 7400 a001 7402 6a03 7c00 6a04  <...t...t.j.|.j.
-000001c0: a005 a100 7c00 6a06 6401 7500 720f 6402  ....|.j.d.u.r.d.
-000001d0: 6e04 7c00 6a06 a005 a100 7c00 6a07 a005  n.|.j.....|.j...
-000001e0: a100 a104 7d01 7c01 7400 6a08 1700 5300  ....}.|.t.j...S.
-000001f0: 2903 7a7c 0a20 2020 2020 2020 2044 756d  ).z|.        Dum
-00000200: 7020 4e41 5453 2070 726f 746f 636f 6c20  p NATS protocol 
-00000210: 5355 4220 6d65 7373 6167 6520 746f 2062  SUB message to b
-00000220: 7974 6573 0a20 2020 2020 2020 203a 7265  ytes.        :re
-00000230: 7475 726e 3a20 4e41 5453 2070 726f 746f  turn: NATS proto
-00000240: 636f 6c20 5355 4220 6d65 7373 6167 6520  col SUB message 
-00000250: 6173 2062 7974 6573 2d65 6e63 6f64 6564  as bytes-encoded
-00000260: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-00000270: 4ef3 0000 0000 2909 7206 0000 00da 0a62  N.....).r......b
-00000280: 7569 6c64 5f68 6561 6472 0700 0000 da03  uild_headr......
-00000290: 5355 4272 0900 0000 da06 656e 636f 6465  SUBr......encode
-000002a0: 720b 0000 0072 0a00 0000 da04 4352 4c46  r....r......CRLF
-000002b0: a902 da04 7365 6c66 da04 6865 6164 a900  ....self..head..
-000002c0: 7215 0000 00fa 4b2f 686f 6d65 2f72 6573  r.....K/home/res
-000002d0: 7069 7265 6e73 2f68 616e 6469 6365 652f  pirens/handicee/
-000002e0: 6465 7665 6c6f 702f 7765 622f 5265 4e41  develop/web/ReNA
-000002f0: 5453 2f72 656e 6174 732f 7072 6f74 6f63  TS/renats/protoc
-00000300: 6f6c 2f6d 6573 7361 6765 732f 7375 622e  ol/messages/sub.
-00000310: 7079 da04 6475 6d70 0f00 0000 730e 0000  py..dump....s...
-00000320: 0004 0504 0108 0116 0108 0104 fc0a 067a  ...............z
-00000330: 1753 7562 5072 6f74 6f63 6f6c 4d65 7373  .SubProtocolMess
-00000340: 6167 652e 6475 6d70 2909 da08 5f5f 6e61  age.dump)...__na
-00000350: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000360: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000370: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
-00000380: 616e 6e6f 7461 7469 6f6e 735f 5f72 0b00  annotations__r..
-00000390: 0000 da05 6279 7465 7372 1700 0000 7215  ....bytesr....r.
-000003a0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000003b0: 0000 7208 0000 0007 0000 0073 0c00 0000  ..r........s....
-000003c0: 0a00 0401 0803 0801 1001 1202 7208 0000  ............r...
-000003d0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000003e0: 0000 0300 0000 4000 0000 7338 0000 0065  ......@...s8...e
-000003f0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000400: 0564 023c 0064 035a 0665 0764 0342 0065  .d.<.d.Z.e.d.B.e
-00000410: 0564 043c 0064 0565 0866 0264 0664 0784  .d.<.d.e.f.d.d..
-00000420: 045a 0964 0353 0029 08da 1455 6e73 7562  .Z.d.S.)...Unsub
-00000430: 5072 6f74 6f63 6f6c 4d65 7373 6167 657a  ProtocolMessagez
-00000440: 370a 2020 2020 4e41 5453 2070 726f 746f  7.    NATS proto
-00000450: 636f 6c20 6d65 7373 6167 6520 6d6f 6465  col message mode
-00000460: 6c20 666f 7220 554e 5355 4220 6d65 7373  l for UNSUB mess
-00000470: 6167 650a 2020 2020 720a 0000 004e da08  age.    r....N..
-00000480: 6d61 785f 6d73 6773 720c 0000 0063 0100  max_msgsr....c..
-00000490: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000004a0: 0000 4300 0000 7338 0000 0074 00a0 0174  ..C...s8...t...t
-000004b0: 026a 037c 006a 04a0 05a1 007c 006a 0664  .j.|.j.....|.j.d
-000004c0: 0175 0072 0f64 026e 0674 077c 006a 0683  .u.r.d.n.t.|.j..
-000004d0: 01a0 05a1 00a1 037d 017c 0174 006a 0817  .......}.|.t.j..
-000004e0: 0053 0029 037a 800a 2020 2020 2020 2020  .S.).z..        
-000004f0: 4475 6d70 204e 4154 5320 7072 6f74 6f63  Dump NATS protoc
-00000500: 6f6c 2055 4e53 5542 206d 6573 7361 6765  ol UNSUB message
-00000510: 2074 6f20 6279 7465 730a 2020 2020 2020   to bytes.      
-00000520: 2020 3a72 6574 7572 6e3a 204e 4154 5320    :return: NATS 
-00000530: 7072 6f74 6f63 6f6c 2055 4e53 5542 206d  protocol UNSUB m
-00000540: 6573 7361 6765 2061 7320 6279 7465 732d  essage as bytes-
-00000550: 656e 636f 6465 6420 7374 7269 6e67 0a20  encoded string. 
-00000560: 2020 2020 2020 204e 720d 0000 0029 0972         Nr....).r
-00000570: 0600 0000 720e 0000 0072 0700 0000 da05  ....r....r......
-00000580: 554e 5355 4272 0a00 0000 7210 0000 0072  UNSUBr....r....r
-00000590: 2000 0000 721c 0000 0072 1100 0000 7212   ...r....r....r.
-000005a0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000005b0: 0000 7217 0000 0024 0000 0073 0c00 0000  ..r....$...s....
-000005c0: 0405 0401 0801 1a01 04fd 0a05 7a19 556e  ............z.Un
-000005d0: 7375 6250 726f 746f 636f 6c4d 6573 7361  subProtocolMessa
-000005e0: 6765 2e64 756d 7029 0a72 1800 0000 7219  ge.dump).r....r.
-000005f0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000600: 0000 721d 0000 0072 2000 0000 da03 696e  ..r....r .....in
-00000610: 7472 1e00 0000 7217 0000 0072 1500 0000  tr....r....r....
-00000620: 7215 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000630: 1f00 0000 1d00 0000 730a 0000 000a 0004  ........s.......
-00000640: 0108 0310 0112 0272 1f00 0000 4e29 09da  .......r....N)..
-00000650: 076d 7367 7370 6563 7202 0000 00da 0462  .msgspecr......b
-00000660: 6173 6572 0400 0000 da00 7206 0000 0072  aser......r....r
-00000670: 0700 0000 7208 0000 0072 1f00 0000 7215  ....r....r....r.
-00000680: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000690: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000006a0: 730a 0000 000c 000c 0210 0110 0314 16    s..............
+00000040: 6d03 5a03 6d04 5a04 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
+00000050: 8400 6405 6501 8303 5a05 4700 6406 6407  ..d.e...Z.G.d.d.
+00000060: 8400 6407 6501 8303 5a06 6408 5300 2909  ..d.e...Z.d.S.).
+00000070: e900 0000 0029 01da 0653 7472 7563 74e9  .....)...Struct.
+00000080: 0200 0000 2902 da05 7574 696c 73da 0870  ....)...utils..p
+00000090: 726f 746f 636f 6c63 0000 0000 0000 0000  rotocolc........
+000000a0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+000000b0: 7340 0000 0065 005a 0164 005a 0255 0064  s@...e.Z.d.Z.U.d
+000000c0: 015a 0365 0465 0564 023c 0065 0465 0564  .Z.e.e.d.<.e.e.d
+000000d0: 033c 0064 045a 0665 0464 0442 0065 0564  .<.d.Z.e.d.B.e.d
+000000e0: 053c 0064 0665 0766 0264 0764 0884 045a  .<.d.e.f.d.d...Z
+000000f0: 0864 0453 0029 09da 1253 7562 5072 6f74  .d.S.)...SubProt
+00000100: 6f63 6f6c 4d65 7373 6167 657a 350a 2020  ocolMessagez5.  
+00000110: 2020 4e41 5453 2070 726f 746f 636f 6c20    NATS protocol 
+00000120: 6d65 7373 6167 6520 6d6f 6465 6c20 666f  message model fo
+00000130: 7220 5355 4220 6d65 7373 6167 650a 2020  r SUB message.  
+00000140: 2020 da07 7375 626a 6563 74da 0373 6964    ..subject..sid
+00000150: 4eda 0b71 7565 7565 5f67 726f 7570 da06  N..queue_group..
+00000160: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000170: 0000 0002 0000 0007 0000 0043 0000 0073  ...........C...s
+00000180: 3c00 0000 7400 a001 7402 6a03 7c00 6a04  <...t...t.j.|.j.
+00000190: a005 a100 7c00 6a06 6401 7500 720f 6402  ....|.j.d.u.r.d.
+000001a0: 6e04 7c00 6a06 a005 a100 7c00 6a07 a005  n.|.j.....|.j...
+000001b0: a100 a104 7d01 7c01 7400 6a08 1700 5300  ....}.|.t.j...S.
+000001c0: 2903 7a7c 0a20 2020 2020 2020 2044 756d  ).z|.        Dum
+000001d0: 7020 4e41 5453 2070 726f 746f 636f 6c20  p NATS protocol 
+000001e0: 5355 4220 6d65 7373 6167 6520 746f 2062  SUB message to b
+000001f0: 7974 6573 0a20 2020 2020 2020 203a 7265  ytes.        :re
+00000200: 7475 726e 3a20 4e41 5453 2070 726f 746f  turn: NATS proto
+00000210: 636f 6c20 5355 4220 6d65 7373 6167 6520  col SUB message 
+00000220: 6173 2062 7974 6573 2d65 6e63 6f64 6564  as bytes-encoded
+00000230: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00000240: 4ef3 0000 0000 2909 7204 0000 00da 0a62  N.....).r......b
+00000250: 7569 6c64 5f68 6561 6472 0500 0000 da03  uild_headr......
+00000260: 5355 4272 0700 0000 da06 656e 636f 6465  SUBr......encode
+00000270: 7209 0000 0072 0800 0000 da04 4352 4c46  r....r......CRLF
+00000280: a902 da04 7365 6c66 da04 6865 6164 a900  ....self..head..
+00000290: 7213 0000 00fa 4b2f 686f 6d65 2f72 6573  r.....K/home/res
+000002a0: 7069 7265 6e73 2f68 616e 6469 6365 652f  pirens/handicee/
+000002b0: 6465 7665 6c6f 702f 7765 622f 5265 4e41  develop/web/ReNA
+000002c0: 5453 2f72 656e 6174 732f 7072 6f74 6f63  TS/renats/protoc
+000002d0: 6f6c 2f6d 6573 7361 6765 732f 7375 622e  ol/messages/sub.
+000002e0: 7079 da04 6475 6d70 0e00 0000 730e 0000  py..dump....s...
+000002f0: 0004 0504 0108 0116 0108 0104 fc0a 067a  ...............z
+00000300: 1753 7562 5072 6f74 6f63 6f6c 4d65 7373  .SubProtocolMess
+00000310: 6167 652e 6475 6d70 2909 da08 5f5f 6e61  age.dump)...__na
+00000320: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000330: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000340: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
+00000350: 616e 6e6f 7461 7469 6f6e 735f 5f72 0900  annotations__r..
+00000360: 0000 da05 6279 7465 7372 1500 0000 7213  ....bytesr....r.
+00000370: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00000380: 0000 7206 0000 0006 0000 0073 0c00 0000  ..r........s....
+00000390: 0a00 0401 0803 0801 1001 1202 7206 0000  ............r...
+000003a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000003b0: 0000 0300 0000 4000 0000 7338 0000 0065  ......@...s8...e
+000003c0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
+000003d0: 0564 023c 0064 035a 0665 0764 0342 0065  .d.<.d.Z.e.d.B.e
+000003e0: 0564 043c 0064 0565 0866 0264 0664 0784  .d.<.d.e.f.d.d..
+000003f0: 045a 0964 0353 0029 08da 1455 6e73 7562  .Z.d.S.)...Unsub
+00000400: 5072 6f74 6f63 6f6c 4d65 7373 6167 657a  ProtocolMessagez
+00000410: 370a 2020 2020 4e41 5453 2070 726f 746f  7.    NATS proto
+00000420: 636f 6c20 6d65 7373 6167 6520 6d6f 6465  col message mode
+00000430: 6c20 666f 7220 554e 5355 4220 6d65 7373  l for UNSUB mess
+00000440: 6167 650a 2020 2020 7208 0000 004e da08  age.    r....N..
+00000450: 6d61 785f 6d73 6773 720a 0000 0063 0100  max_msgsr....c..
+00000460: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000470: 0000 4300 0000 7338 0000 0074 00a0 0174  ..C...s8...t...t
+00000480: 026a 037c 006a 04a0 05a1 007c 006a 0664  .j.|.j.....|.j.d
+00000490: 0175 0072 0f64 026e 0674 077c 006a 0683  .u.r.d.n.t.|.j..
+000004a0: 01a0 05a1 00a1 037d 017c 0174 006a 0817  .......}.|.t.j..
+000004b0: 0053 0029 037a 800a 2020 2020 2020 2020  .S.).z..        
+000004c0: 4475 6d70 204e 4154 5320 7072 6f74 6f63  Dump NATS protoc
+000004d0: 6f6c 2055 4e53 5542 206d 6573 7361 6765  ol UNSUB message
+000004e0: 2074 6f20 6279 7465 730a 2020 2020 2020   to bytes.      
+000004f0: 2020 3a72 6574 7572 6e3a 204e 4154 5320    :return: NATS 
+00000500: 7072 6f74 6f63 6f6c 2055 4e53 5542 206d  protocol UNSUB m
+00000510: 6573 7361 6765 2061 7320 6279 7465 732d  essage as bytes-
+00000520: 656e 636f 6465 6420 7374 7269 6e67 0a20  encoded string. 
+00000530: 2020 2020 2020 204e 720b 0000 0029 0972         Nr....).r
+00000540: 0400 0000 720c 0000 0072 0500 0000 da05  ....r....r......
+00000550: 554e 5355 4272 0800 0000 720e 0000 0072  UNSUBr....r....r
+00000560: 1e00 0000 721a 0000 0072 0f00 0000 7210  ....r....r....r.
+00000570: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00000580: 0000 7215 0000 0023 0000 0073 0c00 0000  ..r....#...s....
+00000590: 0405 0401 0801 1a01 04fd 0a05 7a19 556e  ............z.Un
+000005a0: 7375 6250 726f 746f 636f 6c4d 6573 7361  subProtocolMessa
+000005b0: 6765 2e64 756d 7029 0a72 1600 0000 7217  ge.dump).r....r.
+000005c0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
+000005d0: 0000 721b 0000 0072 1e00 0000 da03 696e  ..r....r......in
+000005e0: 7472 1c00 0000 7215 0000 0072 1300 0000  tr....r....r....
+000005f0: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000600: 1d00 0000 1c00 0000 730a 0000 000a 0004  ........s.......
+00000610: 0108 0310 0112 0272 1d00 0000 4e29 07da  .......r....N)..
+00000620: 076d 7367 7370 6563 7202 0000 00da 0072  .msgspecr......r
+00000630: 0400 0000 7205 0000 0072 0600 0000 721d  ....r....r....r.
+00000640: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
+00000650: 0000 7214 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000660: 3e01 0000 0073 0800 0000 0c00 1002 1003  >....s..........
+00000670: 1416                                     ..
```

### Comparing `renats-0.2.2a1/renats/protocol/messages/pub.py` & `renats-0.2.2a2/renats/protocol/messages/pub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/protocol/messages/service.py` & `renats-0.2.2a2/renats/protocol/messages/service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 
 import msgspec.json
 from msgspec import Struct, field
 
-from .base import SerializableProtocolMessage
-
 INFO_HEAD_PATTERN = re.compile(br"^INFO\s+(.+)\r\n$")
 
 
 class InfoProtocolMessage(Struct):
     """
     NATS protocol message model for INFO message
     """
```

### Comparing `renats-0.2.2a1/renats/protocol/messages/sub.py` & `renats-0.2.2a2/renats/protocol/messages/sub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/protocol/protocol.py` & `renats-0.2.2a2/renats/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/renats/protocol/utils.py` & `renats-0.2.2a2/renats/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a1/PKG-INFO` & `renats-0.2.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renats
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: 
 Author: Respirens
 Author-email: thesergiyprotsanin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: msgspec (>=0.15.1,<0.16.0)
+Requires-Dist: msgspec (>=0.16.0,<0.17.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: uuid6 (>=2023.5.2,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # ReNATS
 
 > Elegant, modern and asynchronous NATS Client API library written in pure Python
```

