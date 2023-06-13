# Comparing `tmp/azure-communication-rooms-1.0.0b2.zip` & `tmp/azure-communication-rooms-1.0.0b3.zip`

## zipinfo {}

```diff
@@ -1,87 +1,80 @@
-Zip file size: 96822 bytes, number of entries: 85
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/
--rw-rw-r--  2.0 unx      202 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/MANIFEST.in
--rw-rw-r--  2.0 unx       38 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/setup.cfg
--rw-rw-r--  2.0 unx      454 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx     6036 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/README.md
--rw-rw-r--  2.0 unx     6902 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/PKG-INFO
--rw-rw-r--  2.0 unx     2558 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/setup.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/LICENSE
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/tests/_shared/
--rw-rw-r--  2.0 unx    23423 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/test_rooms_client_async_e2e.py
--rw-rw-r--  2.0 unx     9697 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/test_rooms_client_async.py
--rw-rw-r--  2.0 unx      983 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/testcase.py
--rw-rw-r--  2.0 unx     1308 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/test_hmac.py
--rw-rw-r--  2.0 unx    19452 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/test_rooms_client_e2e.py
--rw-rw-r--  2.0 unx      889 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/unittest_helpers.py
--rw-rw-r--  2.0 unx      840 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/testcase_async.py
--rw-rw-r--  2.0 unx     1344 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/helper.py
--rw-rw-r--  2.0 unx    10691 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/test_rooms_client.py
--rw-rw-r--  2.0 unx      538 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/async_fake_token_credential.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/asynctestcase.py
--rw-rw-r--  2.0 unx     3787 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/testcase.py
--rw-rw-r--  2.0 unx      325 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/__init__.py
--rw-rw-r--  2.0 unx     2674 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/utils.py
--rw-rw-r--  2.0 unx     3139 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/helper.py
--rw-rw-r--  2.0 unx      527 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/fake_token_credential.py
--rw-rw-r--  2.0 unx      431 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/tests/_shared/communication_service_preparer.py
--rw-rw-r--  2.0 unx     6818 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/samples/rooms_client_sample.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/
--rw-rw-r--  2.0 unx       65 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/
--rw-rw-r--  2.0 unx       65 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/py.typed
--rw-rw-r--  2.0 unx    12940 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_rooms_client.py
--rw-rw-r--  2.0 unx      722 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/__init__.py
--rw-rw-r--  2.0 unx      400 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_version.py
--rw-rw-r--  2.0 unx      455 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_api_versions.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/
--rw-rw-r--  2.0 unx      843 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_vendor.py
--rw-rw-r--  2.0 unx     2648 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_patch.py
--rw-rw-r--  2.0 unx     3652 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_client.py
--rw-rw-r--  2.0 unx      859 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/__init__.py
--rw-rw-r--  2.0 unx    77452 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_serialization.py
--rw-rw-r--  2.0 unx    19492 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_models.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_patch.py
--rw-rw-r--  2.0 unx      954 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_enums.py
--rw-rw-r--  2.0 unx     1696 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx      786 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx    44687 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/
--rw-rw-r--  2.0 unx     2614 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     3698 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_client.py
--rw-rw-r--  2.0 unx      859 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      786 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    36282 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     8489 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/_models.py
--rw-rw-r--  2.0 unx      656 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/__init__.py
--rw-rw-r--  2.0 unx     6682 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/user_credential_async.py
--rw-rw-r--  2.0 unx     1008 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/utils_async.py
--rw-rw-r--  2.0 unx     3045 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/policy.py
--rw-rw-r--  2.0 unx      310 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/__init__.py
--rw-rw-r--  2.0 unx     5589 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/utils.py
--rw-rw-r--  2.0 unx     6391 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/user_credential.py
--rw-rw-r--  2.0 unx     8216 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/models.py
--rw-rw-r--  2.0 unx    13192 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/_rooms_client_async.py
--rw-rw-r--  2.0 unx       79 b- defN 22-Sep-01 17:45 azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/__init__.py
--rw-rw-r--  2.0 unx       95 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/requires.txt
--rw-rw-r--  2.0 unx     6902 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     2748 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 22-Sep-01 17:46 azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/top_level.txt
-85 files, 383939 bytes uncompressed, 78292 bytes compressed:  79.6%
+Zip file size: 94674 bytes, number of entries: 78
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/
+-rw-rw-r--  2.0 unx     8034 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/README.md
+-rw-rw-r--  2.0 unx       99 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/pyproject.toml
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/LICENSE
+-rw-rw-r--  2.0 unx     2558 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/setup.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/CHANGELOG.md
+-rw-rw-r--  2.0 unx      202 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/MANIFEST.in
+-rw-rw-r--  2.0 unx       38 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/setup.cfg
+-rw-rw-r--  2.0 unx     8900 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/PKG-INFO
+-rw-rw-r--  2.0 unx     6641 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/samples/rooms_client_sample_async.py
+-rw-rw-r--  2.0 unx     6297 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/samples/rooms_client_sample.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/
+-rw-rw-r--  2.0 unx      383 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_api_versions.py
+-rw-rw-r--  2.0 unx     1378 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/py.typed
+-rw-rw-r--  2.0 unx      400 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_version.py
+-rw-rw-r--  2.0 unx    11258 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_rooms_client.py
+-rw-rw-r--  2.0 unx     4974 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/_models.py
+-rw-rw-r--  2.0 unx      642 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/__init__.py
+-rw-rw-r--  2.0 unx     1008 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/utils_async.py
+-rw-rw-r--  2.0 unx     5265 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/utils.py
+-rw-rw-r--  2.0 unx     6682 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/user_credential_async.py
+-rw-rw-r--  2.0 unx     6391 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/user_credential.py
+-rw-rw-r--  2.0 unx    14820 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/models.py
+-rw-rw-r--  2.0 unx      310 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/__init__.py
+-rw-rw-r--  2.0 unx     3045 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/policy.py
+-rw-rw-r--  2.0 unx    11541 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/_rooms_client_async.py
+-rw-rw-r--  2.0 unx       79 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/
+-rw-rw-r--  2.0 unx      874 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_vendor.py
+-rw-rw-r--  2.0 unx     2510 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_patch.py
+-rw-rw-r--  2.0 unx      749 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/__init__.py
+-rw-rw-r--  2.0 unx     3668 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_client.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_serialization.py
+-rw-rw-r--  2.0 unx    50329 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx      747 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/
+-rw-rw-r--  2.0 unx     2520 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      749 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     3780 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_client.py
+-rw-rw-r--  2.0 unx    43677 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      747 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-May-17 18:56 azure-communication-rooms-1.0.0b3/tests/_shared/
+-rw-rw-r--  2.0 unx     3179 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/conftest.py
+-rw-rw-r--  2.0 unx    21550 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/test_rooms_client_async.py
+-rw-rw-r--  2.0 unx    18582 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/test_rooms_client.py
+-rw-rw-r--  2.0 unx     1174 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/test_hmac.py
+-rw-rw-r--  2.0 unx     1038 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/acs_rooms_test_case.py
+-rw-rw-r--  2.0 unx      527 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/fake_token_credential.py
+-rw-rw-r--  2.0 unx     2674 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/utils.py
+-rw-rw-r--  2.0 unx     4449 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/testcase.py
+-rw-rw-r--  2.0 unx      431 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/communication_service_preparer.py
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/asynctestcase.py
+-rw-rw-r--  2.0 unx     3139 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/helper.py
+-rw-rw-r--  2.0 unx      325 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/__init__.py
+-rw-rw-r--  2.0 unx      538 b- defN 23-May-17 18:54 azure-communication-rooms-1.0.0b3/tests/_shared/async_fake_token_credential.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     2476 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx       95 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     8900 b- defN 23-May-17 18:56 azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/PKG-INFO
+78 files, 365447 bytes uncompressed, 77772 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -1,256 +1,235 @@
-Filename: azure-communication-rooms-1.0.0b2/
+Filename: azure-communication-rooms-1.0.0b3/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/
+Filename: azure-communication-rooms-1.0.0b3/samples/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/samples/
+Filename: azure-communication-rooms-1.0.0b3/azure/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/
+Filename: azure-communication-rooms-1.0.0b3/tests/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/MANIFEST.in
+Filename: azure-communication-rooms-1.0.0b3/README.md
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/setup.cfg
+Filename: azure-communication-rooms-1.0.0b3/pyproject.toml
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/CHANGELOG.md
+Filename: azure-communication-rooms-1.0.0b3/LICENSE
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/README.md
+Filename: azure-communication-rooms-1.0.0b3/setup.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/PKG-INFO
+Filename: azure-communication-rooms-1.0.0b3/CHANGELOG.md
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/setup.py
+Filename: azure-communication-rooms-1.0.0b3/MANIFEST.in
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/LICENSE
+Filename: azure-communication-rooms-1.0.0b3/setup.cfg
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/
+Filename: azure-communication-rooms-1.0.0b3/PKG-INFO
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/test_rooms_client_async_e2e.py
+Filename: azure-communication-rooms-1.0.0b3/samples/rooms_client_sample_async.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/test_rooms_client_async.py
+Filename: azure-communication-rooms-1.0.0b3/samples/rooms_client_sample.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/testcase.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/test_hmac.py
+Filename: azure-communication-rooms-1.0.0b3/azure/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/test_rooms_client_e2e.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/unittest_helpers.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/testcase_async.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/helper.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/test_rooms_client.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/async_fake_token_credential.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/asynctestcase.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_api_versions.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/testcase.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/py.typed
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/utils.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_version.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/helper.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_rooms_client.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/fake_token_credential.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/_models.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/tests/_shared/communication_service_preparer.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/samples/rooms_client_sample.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/utils_async.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/utils.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/user_credential_async.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/user_credential.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/models.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/policy.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/_rooms_client_async.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/py.typed
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_rooms_client.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_vendor.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_version.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_configuration.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_api_versions.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_patch.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_client.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_serialization.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_vendor.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/_operations.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_configuration.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_patch.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_client.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_serialization.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_models.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_patch.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_client.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_enums.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/_patch.py
+Filename: azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/_operations.py
+Filename: azure-communication-rooms-1.0.0b3/tests/conftest.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/
+Filename: azure-communication-rooms-1.0.0b3/tests/test_rooms_client_async.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_configuration.py
+Filename: azure-communication-rooms-1.0.0b3/tests/test_rooms_client.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_patch.py
+Filename: azure-communication-rooms-1.0.0b3/tests/test_hmac.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_client.py
+Filename: azure-communication-rooms-1.0.0b3/tests/acs_rooms_test_case.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/fake_token_credential.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/_patch.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/utils.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/testcase.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/operations/_operations.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/communication_service_preparer.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/_models.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/asynctestcase.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/helper.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/user_credential_async.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/__init__.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/utils_async.py
+Filename: azure-communication-rooms-1.0.0b3/tests/_shared/async_fake_token_credential.py
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/policy.py
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/__init__.py
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/utils.py
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/user_credential.py
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/models.py
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/requires.txt
 Comment: 
 
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/_rooms_client_async.py
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/__init__.py
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/requires.txt
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/PKG-INFO
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/SOURCES.txt
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/dependency_links.txt
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/not-zip-safe
-Comment: 
-
-Filename: azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/top_level.txt
+Filename: azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-communication-rooms-1.0.0b2/README.md` & `azure-communication-rooms-1.0.0b3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -38,96 +38,142 @@
 ```
 ## Examples
 
 ### Key parameters
 
 - `valid_from`: A datetime object from which room will start existing
 - `valid_until`: A datetime object after which room meeting would end
-- `room_join_policy`: The join policy of the room. Allows only participants or any communication
-        service users to join
-- `participants`: A list of RoomParticipant containing MRI's of invitees to the room
+- `participants`: A list of `RoomParticipant`s containing MRI's of invitees to the room as well as optional `ParticipantRole`. If `ParticipantRole` is not specified, then it will be `Attendee` by default.
 All the above attributes are optional. The service provides default values of valid_until and
-valid_from if they are missing.
+valid_from if they are missing. The default for`valid_from` is current date time and the default for `valid_until` is `valid_from + 180 days`.
+
+### Create a room
+To create a room, call the `create_room` function from `RoomsClient`. The `valid_from`, `valid_until`, and `participants` arguments are all optional.
 
-### Create Room
 ```python
-from azure.communication.rooms import RoomsClient
 from azure.core.exceptions import HttpResponseError
 from datetime import datetime, timedelta
+from azure.communication.rooms import (
+    RoomsClient,
+    RoomParticipant,
+    ParticipantRole
+)
+from azure.communication.identity import CommunicationUserIdentifier
 
 client = RoomsClient.from_connection_string(conn_str='<connection_str>')
+valid_from = datetime.now()
+valid_until = valid_from + relativedelta(months=+1)
+participants = []
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 1>")))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 2>"), ParticipantRole.CONSUMER))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 3>"), ParticipantRole.PRESENTER))
+
 try:
-    response = client.create_room(
-        valid_from=datetime.now(),
-        valid_until=valid_from + timedelta(weeks=4)
-        participants=["first-participant", "second-participant"]
+    create_room_response = client.create_room(
+        valid_from=valid_from,
+        valid_until=valid_until,
+        participants=participants
     )
-except HttpResponseError as e:
-    print('service responds error: {}'.format(e))
-
+except HttpResponseError as ex:
+    print(ex)
 ```
-### Update Room
-```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
-from datetime import datetime, timedelta
+### Update a room
+The `valid_from` and `valid_until` properties of a created room can be updated by calling the `update_room` function from `RoomsClient`.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>')
+```python
 try:
-    response = client.update_room(
+    update_room_response = client.update_room(
         room_id="id of the room to be updated",
         valid_from=datetime.now(),
         valid_until=valid_from + timedelta(weeks=4)
     )
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
 
 ```
 
-### Delete a Room
+### Get a room
+A created room can be retrieved by calling the `get_room` function from `RoomsClient` and passing in the associated `room_id`.
+
 ```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
+try:
+    get_room_response = client.get_room(room_id="id of the room to get")
+except HttpResponseError as ex:
+    print(ex)
+```
+
+### List rooms
+Retrieve all valid rooms created with an ACS resource by calling the `list_rooms` function from `RoomsClient`.
+
+```python
+try:
+    list_room_response = client.list_rooms()
+except HttpResponseError as ex:
+    print(ex)
+```
+
+### Delete a room
+To delete a room, call the `delete_room` function from RoomsClient.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>' )
+```python
 try:
     client.delete_room(
         room_id="id of the room to be deleted")
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
 
 ```
 
-### Add participants to Room
-```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
+### Add or update participants in a room
+In order to insert new participants or update existing participants, call the `add_or_update_participants` function from RoomsClient.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>' )
+```python
+participants = []
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 1>")))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 2>"), ParticipantRole.ATTENDEE))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 3>"), ParticipantRole.CONSUMER))
 try:
-    response = client.add_participants(
+    response = client.add_or_update_participants(
         room_id="id of the room to be updated",
-        participants=["new-participant-one", "new-participant-two"]
+        participants=participants
     )
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
-
 ```
 
-Please take a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms/samples) directory for detailed examples of how to use this library to create and manage rooms.
+### Remove participants
+Remove participants from a room by calling the `remove_participants` function from RoomsClient.
+
+```python
+communication_identifiers = [CommunicationUserIdentifier("<ACS User MRI identity 2>")]
 
+try:
+    remove_participants_response = client.remove_participants(
+        room_id=room_id,
+        participants=communication_identifiers
+    )
+except HttpResponseError as ex:
+    print(ex)
+```
+### List participants
+Retrieve the list of participants for an existing room by referencing the `room_id`:
+
+```python
+try:
+    participants = self.rooms_client.list_participants(room_id)
+except HttpResponseError as ex:
+    print(ex)
+```
 ## Troubleshooting
 
 Rooms operations will throw an exception if the request to the server fails. The Rooms client will raise exceptions defined in [Azure Core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md).
 
-
 ## Next steps
 ### More sample code
-
-More examples are coming soon...
+Please take a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms/samples) directory for detailed examples of how to use this library to create and manage rooms.
 
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the [Issues](https://github.com/Azure/azure-sdk-for-python/issues) section of the project
 
 ## Contributing
```

## Comparing `azure-communication-rooms-1.0.0b2/PKG-INFO` & `azure-communication-rooms-1.0.0b3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-communication-rooms
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Microsoft Communication Rooms Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -59,96 +59,142 @@
 ```
 ## Examples
 
 ### Key parameters
 
 - `valid_from`: A datetime object from which room will start existing
 - `valid_until`: A datetime object after which room meeting would end
-- `room_join_policy`: The join policy of the room. Allows only participants or any communication
-        service users to join
-- `participants`: A list of RoomParticipant containing MRI's of invitees to the room
+- `participants`: A list of `RoomParticipant`s containing MRI's of invitees to the room as well as optional `ParticipantRole`. If `ParticipantRole` is not specified, then it will be `Attendee` by default.
 All the above attributes are optional. The service provides default values of valid_until and
-valid_from if they are missing.
+valid_from if they are missing. The default for`valid_from` is current date time and the default for `valid_until` is `valid_from + 180 days`.
+
+### Create a room
+To create a room, call the `create_room` function from `RoomsClient`. The `valid_from`, `valid_until`, and `participants` arguments are all optional.
 
-### Create Room
 ```python
-from azure.communication.rooms import RoomsClient
 from azure.core.exceptions import HttpResponseError
 from datetime import datetime, timedelta
+from azure.communication.rooms import (
+    RoomsClient,
+    RoomParticipant,
+    ParticipantRole
+)
+from azure.communication.identity import CommunicationUserIdentifier
 
 client = RoomsClient.from_connection_string(conn_str='<connection_str>')
+valid_from = datetime.now()
+valid_until = valid_from + relativedelta(months=+1)
+participants = []
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 1>")))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 2>"), ParticipantRole.CONSUMER))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 3>"), ParticipantRole.PRESENTER))
+
 try:
-    response = client.create_room(
-        valid_from=datetime.now(),
-        valid_until=valid_from + timedelta(weeks=4)
-        participants=["first-participant", "second-participant"]
+    create_room_response = client.create_room(
+        valid_from=valid_from,
+        valid_until=valid_until,
+        participants=participants
     )
-except HttpResponseError as e:
-    print('service responds error: {}'.format(e))
-
+except HttpResponseError as ex:
+    print(ex)
 ```
-### Update Room
-```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
-from datetime import datetime, timedelta
+### Update a room
+The `valid_from` and `valid_until` properties of a created room can be updated by calling the `update_room` function from `RoomsClient`.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>')
+```python
 try:
-    response = client.update_room(
+    update_room_response = client.update_room(
         room_id="id of the room to be updated",
         valid_from=datetime.now(),
         valid_until=valid_from + timedelta(weeks=4)
     )
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
 
 ```
 
-### Delete a Room
+### Get a room
+A created room can be retrieved by calling the `get_room` function from `RoomsClient` and passing in the associated `room_id`.
+
 ```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
+try:
+    get_room_response = client.get_room(room_id="id of the room to get")
+except HttpResponseError as ex:
+    print(ex)
+```
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>' )
+### List rooms
+Retrieve all valid rooms created with an ACS resource by calling the `list_rooms` function from `RoomsClient`.
+
+```python
+try:
+    list_room_response = client.list_rooms()
+except HttpResponseError as ex:
+    print(ex)
+```
+
+### Delete a room
+To delete a room, call the `delete_room` function from RoomsClient.
+
+```python
 try:
     client.delete_room(
         room_id="id of the room to be deleted")
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
 
 ```
 
-### Add participants to Room
-```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
+### Add or update participants in a room
+In order to insert new participants or update existing participants, call the `add_or_update_participants` function from RoomsClient.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>' )
+```python
+participants = []
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 1>")))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 2>"), ParticipantRole.ATTENDEE))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 3>"), ParticipantRole.CONSUMER))
 try:
-    response = client.add_participants(
+    response = client.add_or_update_participants(
         room_id="id of the room to be updated",
-        participants=["new-participant-one", "new-participant-two"]
+        participants=participants
     )
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
-
 ```
 
-Please take a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms/samples) directory for detailed examples of how to use this library to create and manage rooms.
+### Remove participants
+Remove participants from a room by calling the `remove_participants` function from RoomsClient.
 
+```python
+communication_identifiers = [CommunicationUserIdentifier("<ACS User MRI identity 2>")]
+
+try:
+    remove_participants_response = client.remove_participants(
+        room_id=room_id,
+        participants=communication_identifiers
+    )
+except HttpResponseError as ex:
+    print(ex)
+```
+### List participants
+Retrieve the list of participants for an existing room by referencing the `room_id`:
+
+```python
+try:
+    participants = self.rooms_client.list_participants(room_id)
+except HttpResponseError as ex:
+    print(ex)
+```
 ## Troubleshooting
 
 Rooms operations will throw an exception if the request to the server fails. The Rooms client will raise exceptions defined in [Azure Core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md).
 
-
 ## Next steps
 ### More sample code
-
-More examples are coming soon...
+Please take a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms/samples) directory for detailed examples of how to use this library to create and manage rooms.
 
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the [Issues](https://github.com/Azure/azure-sdk-for-python/issues) section of the project
 
 ## Contributing
```

## Comparing `azure-communication-rooms-1.0.0b2/setup.py` & `azure-communication-rooms-1.0.0b3/setup.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/LICENSE` & `azure-communication-rooms-1.0.0b3/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/tests/test_hmac.py` & `azure-communication-rooms-1.0.0b3/tests/test_hmac.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # coding: utf-8
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-import unittest
 from azure.communication.rooms._shared.policy import HMACCredentialsPolicy
-from devtools_testutils import AzureTestCase
-
-class HMACTest(AzureTestCase):
-    def setUp(self):
-        super(HMACTest, self).setUp()
 
+class TestHMAC():
     def test_correct_hmac(self):
         auth_policy = HMACCredentialsPolicy("contoso.communicationservices.azure.com", "pw==")
 
         sha_val = auth_policy._compute_hmac("banana")
 
         #[SuppressMessage("Microsoft.Security", "CS002:SecretInNextLine", Justification="unit test with fake keys")]
         assert sha_val == "88EC05aAS9iXnaimtNO78JLjiPtfWryQB/5QYEzEsu8="
```

## Comparing `azure-communication-rooms-1.0.0b2/tests/test_rooms_client_e2e.py` & `azure-communication-rooms-1.0.0b3/tests/test_rooms_client_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,490 +2,501 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import pytest
 from datetime import datetime, timedelta
-
+import unittest
 from azure.core.exceptions import HttpResponseError
 from azure.communication.identity import CommunicationIdentityClient
+from azure.communication.rooms._shared.models import CommunicationUserIdentifier
+from azure.communication.rooms.aio import RoomsClient
 from azure.communication.rooms import (
-    RoomsClient,
-    RoomParticipant,
-    RoomJoinPolicy,
-    RoleType
+    ParticipantRole,
+    RoomParticipant
 )
-from azure.communication.rooms._shared.models import CommunicationUserIdentifier
-
+from acs_rooms_test_case import ACSRoomsTestCase
 from _shared.utils import get_http_logging_policy
-from _shared.testcase import (
-    CommunicationTestCase,
-    ResponseReplacerProcessor
-)
-from helper import URIIdentityReplacer, RequestBodyIdentityReplacer
+from devtools_testutils.aio import recorded_by_proxy_async
+from devtools_testutils import is_live, add_general_regex_sanitizer
 
-class RoomsClientTest(CommunicationTestCase):
-    def __init__(self, method_name):
-        super(RoomsClientTest, self).__init__(method_name)
-
-    def setUp(self):
-        super(RoomsClientTest, self).setUp()
-        if not self.is_playback():
-            self.recording_processors.extend([
-                ResponseReplacerProcessor(keys=[self._resource_name, "8:acs:[A-Za-z0-9-_]+"]),
-                URIIdentityReplacer(),
-                RequestBodyIdentityReplacer()])
-        # create multiple users users
-        self.identity_client = CommunicationIdentityClient.from_connection_string(
-            self.connection_str)
 
-        self.users = {
-            "john" : RoomParticipant(
-                communication_identifier=CommunicationUserIdentifier(
-                    self.identity_client.create_user().properties["id"]
-                ),
-                role=RoleType.PRESENTER
-            ),
-            "fred" : RoomParticipant(
-                communication_identifier=CommunicationUserIdentifier(
-                    self.identity_client.create_user().properties["id"]
-                ),
-                role=RoleType.CONSUMER
-            ),
-            "chris" : RoomParticipant(
-                communication_identifier=CommunicationUserIdentifier(
-                    self.identity_client.create_user().properties["id"]
-                ),
-                role=RoleType.ATTENDEE
-            )
-        }
+@pytest.mark.asyncio
+class TestRoomsClientAsync(ACSRoomsTestCase):
+    def setup_method(self):
+        super().setUp()
+        sanitizedId1 = "8:acs:sanitized1"
+        sanitizedId2 = "8:acs:sanitized2"
+        sanitizedId3 = "8:acs:sanitized3"
+        sanitizedId4 = "8:acs:sanitized4"
+        if is_live():
+            self.identity_client = CommunicationIdentityClient.from_connection_string(
+                self.connection_str)
+
+
+            self.id1 = self.identity_client.create_user().properties["id"]
+            self.id2 = self.identity_client.create_user().properties["id"]
+            self.id3 = self.identity_client.create_user().properties["id"]
+            self.id4 = self.identity_client.create_user().properties["id"]
+            add_general_regex_sanitizer(regex=self.id1, value=sanitizedId1)
+            add_general_regex_sanitizer(regex=self.id2, value=sanitizedId2)
+            add_general_regex_sanitizer(regex=self.id3, value=sanitizedId3)
+            add_general_regex_sanitizer(regex=self.id4, value=sanitizedId4)
+        else:
+            self.id1 = sanitizedId1
+            self.id2 = sanitizedId2
+            self.id3 = sanitizedId3
+            self.id4 = sanitizedId4
+
         self.rooms_client = RoomsClient.from_connection_string(
             self.connection_str,
             http_logging_policy=get_http_logging_policy()
         )
+        self.users = {
+                "john" : RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id1),
+                    role=ParticipantRole.PRESENTER
+                ),
+                "fred" : RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id2),
+                    role=ParticipantRole.CONSUMER
+                ),
+                "chris" : RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id3),
+                    role=ParticipantRole.ATTENDEE
+                )
+            }
+
+    @recorded_by_proxy_async
+    async def test_create_room_no_attributes_async(self):
+        async with self.rooms_client:
+            response = await self.rooms_client.create_room()
+            # delete created room
+            await self.rooms_client.delete_room(room_id=response.id)
 
-    def tearDown(self):
-        super(RoomsClientTest, self).tearDown()
-
-        # delete created users and chat threads
-        if not self.is_playback():
-            for user in self.users.values():
-                self.identity_client.delete_user(user.communication_identifier)
-
-    def test_create_room_no_attributes(self):
-        response = self.rooms_client.create_room()
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
-
-    @pytest.mark.live_test_only
-    def test_create_room_only_validFrom(self):
-        # room attributes
-        valid_from =  datetime.now() + timedelta(days=3)
-        response = self.rooms_client.create_room(valid_from=valid_from)
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
-
-        # verify room is valid for 180 days
-        valid_until = datetime.utcnow() + timedelta(days=180)
-        self.assertEqual(valid_until.date(), response.valid_until.date())
-
-    @pytest.mark.live_test_only
-    def test_create_room_only_validUntil(self):
-        # room attributes
-        valid_until =  datetime.now() + timedelta(weeks=3)
-        response = self.rooms_client.create_room(valid_until=valid_until)
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
-        self.verify_successful_room_response(response=response, valid_until=valid_until)
-
-    @pytest.mark.live_test_only
-    def test_create_room_only_participants(self):
+    @recorded_by_proxy_async
+    async def test_create_room_only_participants_async(self):
         # add john and chris to room
         participants = [
             self.users["john"],
             self.users["chris"]
         ]
 
-        response = self.rooms_client.create_room(participants=participants)
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
+        async with self.rooms_client:
+            response = await self.rooms_client.create_room(participants=participants)
 
-        self.verify_successful_room_response(response=response, participants=participants)
+            # delete created room
+            await self.rooms_client.delete_room(room_id=response.id)
+            self.verify_successful_room_response(response=response)
 
-    def test_create_room_validUntil_7Months(self):
+    @recorded_by_proxy_async
+    async def test_create_room_validUntil_7Months_async(self):
         # room attributes
         valid_from =  datetime.now() + timedelta(days=3)
         valid_until = valid_from + timedelta(weeks=29)
 
         with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until)
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
+            async with self.rooms_client:
+                await self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until)
+                assert str(ex.value.status_code) == "400"
+                assert ex.value.message is not None
 
-    def test_create_room_validFrom_7Months(self):
+    @recorded_by_proxy_async
+    async def test_create_room_validFrom_7Months_async(self):
         # room attributes
         valid_from = datetime.now() + timedelta(weeks=29)
 
         with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.create_room(valid_from=valid_from)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
+            async with self.rooms_client:
+                await self.rooms_client.create_room(valid_from=valid_from)
+                assert str(ex.value.status_code) == "400"
+                assert ex.value.message is not None
 
     @pytest.mark.live_test_only
-    def test_create_room_correct_timerange(self):
+    @recorded_by_proxy_async
+    async def test_create_room_correct_timerange_async(self):
         # room attributes
         valid_from =  datetime.now() + timedelta(days=3)
         valid_until = valid_from + timedelta(weeks=4)
 
-        response = self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until)
-        self.verify_successful_room_response(response=response, valid_from=valid_from, valid_until=valid_until)
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
+        async with self.rooms_client:
+            response = await self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until)
+
+            # delete created room
+            await self.rooms_client.delete_room(room_id=response.id)
+            self.verify_successful_room_response(response=response, valid_from=valid_from, valid_until=valid_until)
 
-    def test_create_room_incorrectMri(self):
+    @recorded_by_proxy_async
+    async def test_create_room_incorrectMri_async(self):
         # room attributes
         participants = [
             RoomParticipant(
                 communication_identifier=CommunicationUserIdentifier("wrong_mri"),
-                role='Attendee'),
+                role=ParticipantRole.ATTENDEE
+            ),
             self.users["john"]
         ]
 
         with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.create_room(participants=participants)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
-
-    @pytest.mark.live_test_only
-    def test_create_room_open_room(self):
-        # room attributes
-        valid_from =  datetime.now() + timedelta(days=3)
-        valid_until = valid_from + timedelta(weeks=4)
-        room_join_policy = RoomJoinPolicy.COMMUNICATION_SERVICE_USERS
+            async with self.rooms_client:
+                await self.rooms_client.create_room(participants=participants)
 
-        response = self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until, room_join_policy=room_join_policy)
-        self.verify_successful_room_response(response=response, valid_from=valid_from, valid_until=valid_until, room_join_policy=room_join_policy)
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
+                assert str(ex.value.status_code) == "400"
+                assert ex.value.message is not None
 
     @pytest.mark.live_test_only
-    def test_create_room_all_attributes(self):
+    @recorded_by_proxy_async
+    async def test_create_room_all_attributes_async(self):
         # room attributes
         valid_from =  datetime.now() + timedelta(days=3)
         valid_until = valid_from + timedelta(weeks=4)
+        # add john to room
         participants = [
             self.users["john"]
         ]
 
-        response = self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until, participants=participants)
+        async with self.rooms_client:
+            response = await self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until, participants=participants)
 
-        # delete created room
-        self.rooms_client.delete_room(room_id=response.id)
-
-        self.verify_successful_room_response(
-            response=response, valid_from=valid_from, valid_until=valid_until, participants=participants)
+            # delete created room
+            await self.rooms_client.delete_room(room_id=response.id)
+            self.verify_successful_room_response(
+            response=response, valid_from=valid_from, valid_until=valid_until)
 
     @pytest.mark.live_test_only
-    def test_get_room(self):
+    @recorded_by_proxy_async
+    async def test_get_room_async(self):
         # room attributes
         valid_from =  datetime.now() + timedelta(days=3)
         valid_until = valid_from + timedelta(weeks=2)
+
         # add john to room
         participants = [
             self.users["john"]
         ]
+        async with self.rooms_client:
+            # create a room first
+            create_response = await self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until, participants=participants)
+
+            get_response = await self.rooms_client.get_room(room_id=create_response.id)
+
+            # delete created room
+            await self.rooms_client.delete_room(room_id=create_response.id)
+            self.verify_successful_room_response(
+                response=get_response, valid_from=valid_from, valid_until=valid_until, room_id=create_response.id)
 
-        # create a room first
-        create_response = self.rooms_client.create_room(valid_from=valid_from, valid_until=valid_until, participants=participants)
-
-        get_response = self.rooms_client.get_room(room_id=create_response.id)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-        self.verify_successful_room_response(
-            response=get_response, valid_from=valid_from, valid_until=valid_until, room_id=create_response.id, participants=participants)
-
-    def test_get_invalid_room(self):
+    @recorded_by_proxy_async
+    async def test_get_invalid_room_async(self):
         # random room id
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.get_room(room_id="89469124725336262")
-
-        # Resource not found
-        assert str(ex.value.status_code) == "404"
-        assert ex.value.message is not None
-
-    def test_delete_invalid_room(self):
-        # random room id
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.delete_room(room_id="78469124725336262")
-
-        # Resource not found
-        assert str(ex.value.status_code) == "404"
-        assert ex.value.message is not None
-
-    def test_update_room_only_ValidFrom(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        # update room attributes
-        valid_from =  datetime.now() + timedelta(weeks=2)
-
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
-
-    def test_update_room_only_ValidUntil(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        # update room attributes
-        valid_until =  datetime.now() + timedelta(weeks=2)
-
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id, valid_until=valid_until)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
-
-    def test_update_room_ValidFrom_7Months(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        # update room attributes
-        valid_from =  datetime.now() + timedelta(weeks=29)
-
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
-
-    def test_update_room_ValidUntil_7Months(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        # update room attributes
-        valid_until =  datetime.now() + timedelta(weeks=29)
-
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id, valid_until=valid_until)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
-
-    def test_update_room_incorrect_timerange(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        # update room attributes
-        valid_from =  datetime.now() + timedelta(days=3)
-        valid_until =  datetime.now() + timedelta(weeks=29)
-
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
 
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
+            # delete created room
+            await self.rooms_client.delete_room(room_id=create_response.id)
+            with pytest.raises(HttpResponseError) as ex:
 
-    @pytest.mark.live_test_only
-    def test_update_room_correct_timerange(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        # update room attributes
-        valid_from =  datetime.now() + timedelta(days=3)
-        valid_until =  datetime.now() + timedelta(weeks=4)
-
-        update_response = self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until)
-
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-        self.verify_successful_room_response(
-            response=update_response, valid_from=valid_from, valid_until=valid_until, room_id=create_response.id)
+                await self.rooms_client.get_room(room_id=create_response.id)
+                # Resource not found
+            assert str(ex.value.status_code) == "404"
+            assert ex.value.message is not None
+            await self.rooms_client.delete_room(room_id=create_response.id)
 
-    @pytest.mark.live_test_only
-    def test_update_room_change_open_room_in_past(self):
+    @recorded_by_proxy_async
+    async def test_update_room_exceed_max_timerange_async(self):
         # room with no attributes
-        create_response = self.rooms_client.create_room()
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
 
-        # room attributes
-        valid_from =  datetime.now() + timedelta(days=-1)
-        valid_until = valid_from + timedelta(weeks=4)
-        room_join_policy = RoomJoinPolicy.COMMUNICATION_SERVICE_USERS
+            # update room attributes
+            valid_from =  datetime.now() + timedelta(days=3)
+            valid_until =  datetime.now() + timedelta(weeks=29)
 
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until, room_join_policy=room_join_policy)
+            with pytest.raises(HttpResponseError) as ex:
+                await self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until)
 
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
+                # delete created room
+                await self.rooms_client.delete_room(room_id=create_response.id)
 
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
+                assert str(ex.value.status_code) == "400"
+                assert ex.value.message is not None
 
     @pytest.mark.live_test_only
-    def test_update_room_change_open_room_in_future(self):
+    @recorded_by_proxy_async
+    async def test_update_room_correct_timerange_async(self):
         # room with no attributes
-        create_response = self.rooms_client.create_room()
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
 
-        # room attributes
-        valid_from =  datetime.now() + timedelta(days=3)
-        valid_until = valid_from + timedelta(weeks=4)
-        room_join_policy = RoomJoinPolicy.COMMUNICATION_SERVICE_USERS
-
-        response = self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until, room_join_policy=room_join_policy)
-        self.verify_successful_room_response(response=response, valid_from=valid_from, valid_until=valid_until, room_join_policy=room_join_policy)
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-
-    @pytest.mark.live_test_only
-    def test_add_participants(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
+            # update room attributes
+            valid_from =  datetime.now() + timedelta(days=3)
+            valid_until =  datetime.now() + timedelta(weeks=4)
 
-        # update room attributes
-        participants = [
-            self.users["john"]
-        ]
-        self.rooms_client.add_participants(room_id=create_response.id, participants=participants)
-        update_response = self.rooms_client.get_participants(room_id=create_response.id)
+            update_response = await self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until)
 
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-        self.assertListEqual(participants, update_response.participants)
+            # delete created room
+            await self.rooms_client.delete_room(room_id=create_response.id)
+            self.verify_successful_room_response(
+                response=update_response, valid_from=valid_from, valid_until=valid_until, room_id=create_response.id)
 
-    @pytest.mark.live_test_only
-    def test_update_participants(self):
+    @recorded_by_proxy_async
+    async def test_add_or_update_participant_async(self):
         # add john and chris to room
         create_participants = [
             self.users["john"],
             self.users["chris"]
         ]
-        create_response = self.rooms_client.create_room(participants=create_participants)
-
-        # participants to be updated
-        self.users["john"].role = RoleType.CONSUMER
-        self.users["chris"].role = RoleType.CONSUMER
-
+        # update join to consumer and add fred to room
+        self.users["john"].role = ParticipantRole.CONSUMER
         update_participants = [
             self.users["john"],
-            self.users["chris"]
+            self.users["fred"]
+        ]
+        expected_participants = [
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id1),
+                role=ParticipantRole.CONSUMER
+            ),
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id2),
+                role=ParticipantRole.CONSUMER
+            ),
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id3),
+                role=ParticipantRole.ATTENDEE
+            )
         ]
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room(participants=create_participants)
+            await self.rooms_client.add_or_update_participants(room_id=create_response.id, participants=update_participants)
+            update_response = self.rooms_client.list_participants(room_id=create_response.id)
+            participants = []
+            async for participant in update_response:
+                participants.append(participant)
+            assert len(participants) == 3
+            case = unittest.TestCase()
+            case.assertCountEqual(expected_participants, participants)
+            # delete created room
+            await self.rooms_client.delete_room(room_id=create_response.id)
 
-        self.rooms_client.update_participants(room_id=create_response.id, participants=update_participants)
-        update_response = self.rooms_client.get_participants(room_id=create_response.id)
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
+    @recorded_by_proxy_async
+    async def test_add_or_update_participant_with_null_roles_async(self):
+        create_participants = [
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id1),
+                role=None
+            ),
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id2)
+            ),
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id3),
+                role=ParticipantRole.PRESENTER
+            )
+        ]
 
-        self.assertListEqual(update_participants, update_response.participants)
+        expected_participants = [
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id1),
+                role=ParticipantRole.ATTENDEE
+            ),
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id2),
+                role=ParticipantRole.ATTENDEE
+            ),
+            RoomParticipant(
+                communication_identifier=CommunicationUserIdentifier(self.id3),
+                role=ParticipantRole.PRESENTER
+            )
+        ]
+        async with self.rooms_client:
+            # Check participants with null roles were added in created room
+            create_response = await self.rooms_client.create_room(participants=create_participants)
+            list_participants_response = self.rooms_client.list_participants(room_id=create_response.id)
+            participants = []
+            async for participant in list_participants_response:
+                participants.append(participant)
+            assert len(participants) == 3
+            case = unittest.TestCase()
+            case.assertCountEqual(expected_participants, participants)
+
+            # Check participants were added or updated properly
+            add_or_update_participants = [
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id1),
+                    role=None
+                ),
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id2),
+                    role=ParticipantRole.CONSUMER
+                ),
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id3)
+                ),
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id4)
+                )]
+
+            expected_participants = [
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id1),
+                    role=ParticipantRole.ATTENDEE
+                ),
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id2),
+                    role=ParticipantRole.CONSUMER
+                ),
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id3),
+                    role=ParticipantRole.ATTENDEE
+                ),
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier(self.id4),
+                    role=ParticipantRole.ATTENDEE
+                )
+            ]
+            await self.rooms_client.add_or_update_participants(room_id=create_response.id, participants=add_or_update_participants)
+            update_response = self.rooms_client.list_participants(room_id=create_response.id)
+            updated_participants = []
+            async for participant in update_response:
+                updated_participants.append(participant)
+            assert len(updated_participants) == 4
+            case = unittest.TestCase()
+            case.assertCountEqual(expected_participants, updated_participants)
+            # delete created room
+            await self.rooms_client.delete_room(room_id=create_response.id)
 
-    @pytest.mark.live_test_only
-    def test_remove_participants(self):
+    @recorded_by_proxy_async
+    async def test_remove_participant_async(self):
         # add john and chris to room
         create_participants = [
             self.users["john"],
             self.users["chris"]
         ]
-        create_response = self.rooms_client.create_room(participants=create_participants)
-
-        # participants to be removed
-        removed_participants = [
+        remove_participants = [
             self.users["john"].communication_identifier
         ]
-
-        self.rooms_client.remove_participants(room_id=create_response.id, communication_identifiers=removed_participants)
-        update_response = self.rooms_client.get_participants(room_id=create_response.id)
-        # delete created room
-        self.rooms_client.delete_room(room_id=create_response.id)
-        participants = [
-            self.users["chris"]
-        ]
-
-        self.assertListEqual(participants, update_response.participants)
-
-    def test_add_participants_incorrectMri(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        participants = [
-            RoomParticipant(
-                communication_identifier=CommunicationUserIdentifier("wrong_mri"),
-                role=RoleType.ATTENDEE),
-            self.users["john"]
-        ]
-
-        # update room attributes
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.add_participants(room_id=create_response.id, participants=participants)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
-
-    def test_update_room_wrongRoleName(self):
-        # room with no attributes
-        create_response = self.rooms_client.create_room()
-
-        participants = [
+        expected_participants = [
             RoomParticipant(
-                communication_identifier=self.users["john"].communication_identifier,
-                role='Kafka'),
+                communication_identifier=CommunicationUserIdentifier(self.id3),
+                role=ParticipantRole.ATTENDEE
+            )
         ]
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room(participants=create_participants)
+            await self.rooms_client.remove_participants(room_id=create_response.id, participants=remove_participants)
+            update_response = self.rooms_client.list_participants(room_id=create_response.id)
+            participants = []
+            async for participant in update_response:
+                participants.append(participant)
+            assert len(participants) == 1
+            case = unittest.TestCase()
+            case.assertCountEqual(expected_participants, participants)
+            # delete created room
+            await self.rooms_client.delete_room(room_id=create_response.id)
+
+    @recorded_by_proxy_async
+    async def test_add_or_update_participants_incorrectMri_async(self):
+        # room with no attributes
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
+
+            participants = [
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier("wrong_mri"),
+                    role=ParticipantRole.ATTENDEE),
+                self.users["john"]
+            ]
+
+            # update room attributes
+            with pytest.raises(HttpResponseError) as ex:
+                await self.rooms_client.add_or_update_participants(room_id=create_response.id, participants=participants)
+
+            assert str(ex.value.status_code) == "400"
+            assert ex.value.message is not None
+
+    @recorded_by_proxy_async
+    async def test_add_participants_wrongRoleName_async(self):
+        # room with no attributes
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
+
+            participants = [
+                RoomParticipant(
+                    communication_identifier=CommunicationUserIdentifier("chris"),
+                    role='kafka'),
+                self.users["john"]
+            ]
+
+            # update room attributes
+            with pytest.raises(HttpResponseError) as ex:
+                await self.rooms_client.add_or_update_participants(room_id=create_response.id, participants=participants)
 
-        # update room attributes
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.add_participants(room_id=create_response.id, participants=participants)
-
-        assert str(ex.value.status_code) == "400"
-        assert ex.value.message is not None
+            assert str(ex.value.status_code) == "400"
+            assert ex.value.message is not None
 
-    def test_update_room_incorrect_roomId(self):
+    @recorded_by_proxy_async
+    async def test_update_room_incorrect_roomId_async(self):
         # try to update room with random room_id
         with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=78469124725336262)
+            async with self.rooms_client:
+                valid_from =  datetime.now() + timedelta(days=3)
+                valid_until = valid_from + timedelta(days=4)
+                await self.rooms_client.update_room(room_id=78469124725336262, valid_from=valid_from, valid_until=valid_until)
+
+                #  assert error is Resource not found
+                assert str(ex.value.status_code) == "404"
+                assert ex.value.message is not None
 
-        #  assert error is Resource not found
-        assert str(ex.value.status_code) == "404"
-        assert ex.value.message is not None
-
-    def test_update_room_deleted_room(self):
+    @recorded_by_proxy_async
+    async def test_update_room_deleted_room_async(self):
         # create a room -> delete it -> try to update it
-        create_response = self.rooms_client.create_room()
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
 
-        # delete the room
-        self.rooms_client.delete_room(room_id=create_response.id)
-        with pytest.raises(HttpResponseError) as ex:
-            self.rooms_client.update_room(room_id=create_response.id)
+            # delete the room
+            await self.rooms_client.delete_room(room_id=create_response.id)
+
+            with pytest.raises(HttpResponseError) as ex:
+                valid_from =  datetime.now() + timedelta(days=3)
+                valid_until = valid_from + timedelta(days=4)
+                await self.rooms_client.update_room(room_id=create_response.id, valid_from=valid_from, valid_until=valid_until)
+
+            #  assert error is Resource not found
+            assert str(ex.value.status_code) == "404"
+            assert ex.value.message is not None
+
+    @recorded_by_proxy_async
+    async def test_list_rooms_first_room_is_not_null_success_async(self):
+        # create a room -> list all rooms -> delete room
+        async with self.rooms_client:
+            create_response = await self.rooms_client.create_room()
+
+            all_rooms = self.rooms_client.list_rooms()
+            first_room = None
+            count = 0
+            async for room in all_rooms:
+                if count == 1:
+                    break
+                first_room = room
+                count += 1
 
-        #  assert error is Resource not found
-        assert str(ex.value.status_code) == "404"
-        assert ex.value.message is not None
+            assert first_room is not None
+            self.verify_successful_room_response(first_room)
 
-    def verify_successful_room_response(self, response, valid_from=None, valid_until=None, room_id=None, participants=None, room_join_policy=None):
+            # delete the room
+            await self.rooms_client.delete_room(room_id=create_response.id)
+
+    def verify_successful_room_response(self, response, valid_from=None, valid_until=None, room_id=None):
         if room_id is not None:
-            self.assertEqual(room_id, response.id)
+            assert room_id == response.id
         if valid_from is not None:
-            self.assertEqual(valid_from.replace(tzinfo=None), response.valid_from.replace(tzinfo=None))
+            assert valid_from.replace(tzinfo=None) == datetime.strptime(
+                response.valid_from, "%Y-%m-%dT%H:%M:%S.%f%z").replace(tzinfo=None)
         if valid_until is not None:
-            self.assertEqual(valid_until.replace(tzinfo=None), response.valid_until.replace(tzinfo=None))
-        if participants is not None:
-            self.assertListEqual(participants, response.participants)
-        if room_join_policy is not None:
-            self.assertEqual(room_join_policy, response.room_join_policy)
+            assert valid_until.replace(tzinfo=None) == datetime.strptime(
+                response.valid_until, "%Y-%m-%dT%H:%M:%S.%f%z").replace(tzinfo=None)
+        assert response.created_at is not None
+        assert response.id is not None
+        assert response.valid_from is not None
+        assert response.valid_until is not None
+
```

## Comparing `azure-communication-rooms-1.0.0b2/tests/_shared/async_fake_token_credential.py` & `azure-communication-rooms-1.0.0b3/tests/_shared/async_fake_token_credential.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/tests/_shared/asynctestcase.py` & `azure-communication-rooms-1.0.0b3/tests/_shared/asynctestcase.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/tests/_shared/utils.py` & `azure-communication-rooms-1.0.0b3/tests/_shared/utils.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/tests/_shared/helper.py` & `azure-communication-rooms-1.0.0b3/tests/_shared/helper.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/tests/_shared/fake_token_credential.py` & `azure-communication-rooms-1.0.0b3/tests/_shared/fake_token_credential.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/samples/rooms_client_sample.py` & `azure-communication-rooms-1.0.0b3/samples/rooms_client_sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,48 +27,45 @@
 import os
 import sys
 
 from datetime import datetime, timedelta
 from azure.core.exceptions import HttpResponseError
 from azure.communication.identity import CommunicationIdentityClient
 from azure.communication.rooms import (
+    ParticipantRole,
     RoomsClient,
-    RoomParticipant,
-    RoleType
-)
-from azure.communication.rooms._shared.models import(
-    CommunicationUserIdentifier
+    RoomParticipant
 )
 
 sys.path.append("..")
 
 class RoomsSample(object):
 
     def setUp(self):
         self.connection_string = os.getenv("COMMUNICATION_SAMPLES_CONNECTION_STRING")
 
         self.rooms_client = RoomsClient.from_connection_string(self.connection_string)
         self.identity_client = CommunicationIdentityClient.from_connection_string(
             self.connection_string)
         self.rooms = []
         self.participant_1 = RoomParticipant(
-            communication_identifier=CommunicationUserIdentifier(self.identity_client.create_user().properties["id"]))
+            communication_identifier=self.identity_client.create_user(),
+            role=ParticipantRole.PRESENTER)
         self.participant_2 = RoomParticipant(
-            communication_identifier=CommunicationUserIdentifier(self.identity_client.create_user().properties["id"]))
+            communication_identifier=self.identity_client.create_user(),
+            role=ParticipantRole.CONSUMER)
 
     def tearDown(self):
         self.delete_room_all_rooms()
 
     def create_single_room(self):
 
         valid_from =  datetime.now()
         valid_until = valid_from + timedelta(weeks=4)
-        participants = []
-
-        participants.append(self.participant_1)
+        participants = [self.participant_1]
 
         try:
             create_room_response = self.rooms_client.create_room(
                 valid_from=valid_from,
                 valid_until=valid_until,
                 participants=participants)
             self.printRoom(response=create_room_response)
@@ -76,18 +73,16 @@
             # all created room to a list
             self.rooms.append(create_room_response.id)
 
         except HttpResponseError as ex:
             print(ex)
 
     def create_single_room_with_default_attributes(self):
-        rooms_client = RoomsClient.from_connection_string(self.connection_string)
-
         try:
-            create_room_response = rooms_client.create_room()
+            create_room_response = self.rooms_client.create_room()
             self.printRoom(response=create_room_response)
             # all created room to a list
             self.rooms.append(create_room_response.id)
 
         except HttpResponseError as ex:
             print(ex)
 
@@ -98,44 +93,38 @@
 
         try:
             update_room_response = self.rooms_client.update_room(room_id=room_id, valid_from=valid_from, valid_until=valid_until)
             self.printRoom(response=update_room_response)
         except HttpResponseError as ex:
             print(ex)
 
-    def add_participants(self, room_id):
-        participants = [self.participant_2]
-
-        try:
-            self.rooms_client.add_participants(room_id=room_id, participants=participants)
-        except HttpResponseError as ex:
-            print(ex)
-
-    def update_participants(self, room_id):
-        participants = [RoomParticipant(
-            communication_identifier=self.participant_1.communication_identifier,
-            role=RoleType.PRESENTER)]
+    def add_or_update_participants(self, room_id):
+        self.participant_1.role = ParticipantRole.ATTENDEE
+        participants = [
+            self.participant_1, # Update participant_1 role from Presenter to Attendee
+            self.participant_2  # Add participant_2 to room
+            ]
 
         try:
-            self.rooms_client.update_participants(room_id=room_id, participants=participants)
+            self.rooms_client.add_or_update_participants(room_id=room_id, participants=participants)
         except HttpResponseError as ex:
             print(ex)
 
-    def get_participants(self, room_id):
+    def list_participants(self, room_id):
         try:
-            get_participants_response = self.rooms_client.get_participants(room_id=room_id)
-            print("participants: \n", self.convert_participant_list_to_string(get_participants_response.participants))
+            get_participants_response = self.rooms_client.list_participants(room_id=room_id)
+            print("participants: \n", self.convert_participant_list_to_string(get_participants_response))
         except HttpResponseError as ex:
             print(ex)
 
     def remove_participants(self, room_id):
         participants = [self.participant_1.communication_identifier]
 
         try:
-            self.rooms_client.remove_participants(room_id=room_id, communication_identifiers=participants)
+            self.rooms_client.remove_participants(room_id=room_id, participants=participants)
         except HttpResponseError as ex:
             print(ex)
 
     def delete_room_all_rooms(self):
         for room in self.rooms:
             print("deleting: ", room)
             self.rooms_client.delete_room(room_id=room)
@@ -147,18 +136,17 @@
             self.printRoom(response=get_room_response)
 
         except HttpResponseError as ex:
             print(ex)
 
     def printRoom(self, response):
         print("room_id: ", response.id)
-        print("created_on: ", response.created_on)
+        print("created_at: ", response.created_at)
         print("valid_from: ", response.valid_from)
         print("valid_until: ", response.valid_until)
-        print("participants: \n", self.convert_participant_list_to_string(response.participants))
 
     def convert_participant_list_to_string(self, participants):
         result = ''
         for p in participants:
             result += "id: {}\n role: {}\n".format(
                 p.communication_identifier.properties["id"], p.role)
         return result
@@ -167,13 +155,12 @@
     sample = RoomsSample()
     sample.setUp()
     sample.create_single_room()
     sample.create_single_room_with_default_attributes()
     if len(sample.rooms) > 0:
         sample.get_room(room_id=sample.rooms[0] )
         sample.update_single_room(room_id=sample.rooms[0])
-        sample.add_participants(room_id=sample.rooms[0])
-        sample.update_participants(room_id=sample.rooms[0])
-        sample.get_participants(room_id=sample.rooms[0])
+        sample.add_or_update_participants(room_id=sample.rooms[0])
+        sample.list_participants(room_id=sample.rooms[0])
         sample.remove_participants(room_id=sample.rooms[0])
         sample.get_room(room_id=sample.rooms[0])
     sample.tearDown()
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_rooms_client.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_rooms_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union, Any
 import uuid
-from azure.core.credentials import AzureKeyCredential
+from azure.core.credentials import AzureKeyCredential, TokenCredential
+from azure.core.paging import ItemPaged
 from azure.core.tracing.decorator import distributed_trace
+
 from azure.communication.rooms._models import (
-    CommunicationRoom,
     RoomParticipant,
-    ParticipantsCollection
+    CommunicationRoom
 )
 from azure.communication.rooms._shared.models import CommunicationIdentifier
-from azure.communication.rooms._shared.policy import HMACCredentialsPolicy
 from ._generated._client import AzureCommunicationRoomsService
-from ._generated.models import (
-    CreateRoomRequest,
-    UpdateRoomRequest,
-    RemoveParticipantsRequest,
-    AddParticipantsRequest,
-    UpdateParticipantsRequest,
-    RoomJoinPolicy
-)
-
-from ._shared.utils import parse_connection_str, verify_datetime_format
+from ._shared.utils import parse_connection_str, get_authentication_policy
 from ._version import SDK_MONIKER
 from ._api_versions import DEFAULT_VERSION
 
-class RoomsClient(object): # pylint: disable=client-accepts-api-version-keyword
+class RoomsClient(object):
     """A client to interact with the AzureCommunicationService Rooms gateway.
 
     This client provides operations to manage rooms.
 
+    This client provides operations to manage rooms.
+
     :param str endpoint:
         The endpoint url for Azure Communication Service resource.
-    :param ~azure.core.credentials.AzureKeyCredential credential:
+    param Union[TokenCredential, AzureKeyCredential] credential:
         The access key we use to authenticate against the service.
+    :keyword api_version: Azure Communication Rooms API version.
+        Default value is "2023-03-31-preview".
+        Note that overriding this default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
     def __init__(
-            self, endpoint: str,
-            credential: AzureKeyCredential,
+            self,
+            endpoint: str,
+            credential: Union[TokenCredential, AzureKeyCredential],
             **kwargs
     ) -> None:
         try:
             if not endpoint.lower().startswith('http'):
                 endpoint = "https://" + endpoint
         except AttributeError:
             raise ValueError("Account URL must be a string.")
 
         if not credential:
             raise ValueError(
                 "invalid credential from connection string.")
 
-        # TokenCredential not supported at the moment
-        if hasattr(credential, "get_token"):
-            raise TypeError("Unsupported credential: {}. Use an AzureKeyCredential to use HMACCredentialsPolicy"
-            " for authentication".format(type(credential)))
+        if endpoint.endswith("/"):
+            endpoint = endpoint[:-1]
 
         self._endpoint = endpoint
         self._api_version = kwargs.pop("api_version", DEFAULT_VERSION)
-        self._authentication_policy = HMACCredentialsPolicy(endpoint, credential.key)
+        self._authentication_policy = get_authentication_policy(endpoint, credential, decode_url=True)
         self._rooms_service_client = AzureCommunicationRoomsService(
             self._endpoint,
-            api_version = self._api_version,
+            api_version=self._api_version,
             authentication_policy=self._authentication_policy,
             sdk_moniker=SDK_MONIKER,
             **kwargs)
 
     @classmethod
     def from_connection_string(cls, conn_str: str,
             **kwargs
@@ -95,50 +91,46 @@
 
     @distributed_trace
     def create_room(
         self,
         *,
         valid_from: Optional[datetime] = None,
         valid_until: Optional[datetime] = None,
-        room_join_policy: Optional[RoomJoinPolicy] = None,
         participants: Optional[List[RoomParticipant]]=None,
         **kwargs
     ) -> CommunicationRoom:
         """Create a new room.
 
         :param valid_from: The timestamp from when the room is open for joining. Optional.
         :type valid_from: ~datetime.datetime
         :param valid_until: The timestamp from when the room can no longer be joined. Optional.
         :type valid_until: ~datetime.datetime
-        :param room_join_policy: The join policy of the room. Optional.
-        :type room_join_policy: ~azure.communication.rooms.models.RoomJoinPolicy
         :param participants: Collection of identities invited to the room. Optional.
         :type participants: List[~azure.communication.rooms.RoomParticipant]
         :returns: Created room.
         :rtype: ~azure.communication.rooms.CommunicationRoom
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        if verify_datetime_format(valid_from) and verify_datetime_format(valid_until):
-            create_room_request = CreateRoomRequest(
-                valid_from=valid_from,
-                valid_until=valid_until,
-                room_join_policy=room_join_policy,
-                # pylint: disable=protected-access
-                participants=[p._to_room_participant_internal() for p in participants] if participants else None
-            )
-
-            repeatability_request_id = uuid.uuid1()
-            repeatability_first_sent = datetime.utcnow()
-
-            create_room_response = self._rooms_service_client.rooms.create_room(
-                create_room_request=create_room_request,
-                repeatability_request_id=repeatability_request_id,
-                repeatability_first_sent=repeatability_first_sent,
-                **kwargs)
-            return CommunicationRoom._from_room_response(create_room_response) # pylint: disable=protected-access
+        create_room_request = {
+            "validFrom": valid_from,
+            "validUntil": valid_until
+        }
+        if participants:
+            create_room_request["participants"] ={
+                p.communication_identifier.raw_id: {"role": p.role} for p in participants
+            }
+
+        repeatability_request_id = uuid.uuid1()
+        repeatability_first_sent = datetime.utcnow()
+        create_room_response = self._rooms_service_client.rooms.create(
+            create_room_request=create_room_request,
+            repeatability_request_id=repeatability_request_id,
+            repeatability_first_sent=repeatability_first_sent,
+            **kwargs)
+        return CommunicationRoom(create_room_response)
 
     @distributed_trace
     def delete_room(
         self,
         room_id: str,
         **kwargs
     ) -> None:
@@ -148,57 +140,45 @@
         :param room_id: Required. Id of room to be deleted
         :type room_id: str
         :returns: None.
         :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError
 
         """
-        self._rooms_service_client.rooms.delete_room(room_id=room_id, **kwargs)
+        return self._rooms_service_client.rooms.delete(room_id=room_id, **kwargs)
 
     @distributed_trace
     def update_room(
         self,
         *,
         room_id: str,
-        valid_from: Optional[datetime] = None,
-        valid_until: Optional[datetime] = None,
-        room_join_policy: Optional[RoomJoinPolicy] = None,
-        participants: Optional[List[RoomParticipant]] = None,
-        **kwargs
+        valid_from: datetime,
+        valid_until: datetime,
+        **kwargs: Any
     ) -> CommunicationRoom:
         """Update a valid room's attributes. For any argument that is passed
         in, the corresponding room property will be replaced with the new value.
 
-        :param room_id: Required. Id of room to be updated
+        :keyword room_id: Required. Id of room to be updated
         :type room_id: str
-        :param valid_from: The timestamp from when the room is open for joining.Optional
+        :keyword valid_from: Required. The timestamp from when the room is open for joining.
         :type valid_from: ~datetime.datetime
-        :param valid_until: The timestamp from when the room can no longer be joined. Optional.
+        :keyword valid_until: Required. The timestamp from when the room can no longer be joined.
         :type valid_until: ~datetime.datetime
-        :param room_join_policy: The join policy of the room.Optional.
-        :type room_join_policy: ~azure.communication.rooms.models.RoomJoinPolicy
-        :param participants: Collection of identities invited to the room. Optional.
-        :type participants: List[~azure.communication.rooms.RoomParticipant]
         :returns: Updated room.
         :rtype: ~azure.communication.rooms.CommunicationRoom
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
-
         """
-        if verify_datetime_format(valid_from) and verify_datetime_format(valid_until):
-            update_room_request = UpdateRoomRequest(
-                valid_from=valid_from,
-                valid_until=valid_until,
-                room_join_policy=room_join_policy,
-                # pylint: disable=protected-access
-                participants=[p._to_room_participant_internal() for p in participants] if participants else None
-            )
-            update_room_response = self._rooms_service_client.rooms.update_room(
-                room_id=room_id, patch_room_request=update_room_request, **kwargs)
-            # pylint: disable=protected-access
-            return CommunicationRoom._from_room_response(update_room_response)
+        update_room_request = {
+            "validFrom": valid_from,
+            "validUntil": valid_until
+        }
+        update_room_response = self._rooms_service_client.rooms.update(
+            room_id=room_id, update_room_request=update_room_request, **kwargs)
+        return CommunicationRoom(update_room_response)
 
     @distributed_trace
     def get_room(
         self,
         room_id: str,
         **kwargs
     ) -> CommunicationRoom:
@@ -207,104 +187,111 @@
         :param room_id: Required. Id of room to be fetched
         :type room_id: str
         :returns: Room with current attributes.
         :rtype: ~azure.communication.rooms.CommunicationRoom
         :raises: ~azure.core.exceptions.HttpResponseError
 
         """
-        get_room_response = self._rooms_service_client.rooms.get_room(room_id=room_id, **kwargs)
-        return CommunicationRoom._from_room_response(get_room_response) # pylint: disable=protected-access
+        get_room_response = self._rooms_service_client.rooms.get(room_id=room_id, **kwargs)
+        return CommunicationRoom(get_room_response)
 
     @distributed_trace
-    def add_participants(
+    def list_rooms(
         self,
-        *,
-        room_id: str,
-        participants: List[RoomParticipant],
         **kwargs
-    ) -> None:
-        """Add participants to a room. Maximum room size is 350 participants. Adding more participants
-        will result in exceptions. Existing participants cannot be added again.
+    ) -> ItemPaged[CommunicationRoom]:
+        """List all rooms
+
+        :returns: An iterator like instance of CommunicationRoom.
+        :rtype: ~azure.core.paging.ItemPaged[~azure.communication.rooms.CommunicationRoom]
+        :raises: ~azure.core.exceptions.HttpResponseError
 
-        :param room_id: Required. Id of room to be updated
-        :type room_id: str
-        :param participants: Required. Collection of identities invited to the room.
-        :type participants: List[~azure.communication.rooms.RoomParticipant]
-        :return: None
-        :raises: ~azure.core.exceptions.HttpResponseError, ValueError
         """
-        add_participants_request = AddParticipantsRequest(
-            # pylint: disable=protected-access
-            participants=[p._to_room_participant_internal() for p in participants]
+        return self._rooms_service_client.rooms.list(
+            cls=lambda rooms: [CommunicationRoom(r) for r in rooms],
+            **kwargs
         )
-        self._rooms_service_client.rooms.add_participants(
-            room_id=room_id, add_participants_request=add_participants_request, **kwargs)
 
     @distributed_trace
-    def update_participants(
+    def add_or_update_participants(
         self,
         *,
         room_id: str,
         participants: List[RoomParticipant],
         **kwargs
     ) -> None:
         """Update participants to a room. It looks for the room participants based on their
         communication identifier and replace the existing participants with the value passed in
         this API.
         :param room_id: Required. Id of room to be updated
         :type room_id: str
         :param participants: Required. Collection of identities invited to be updated
         :type participants: List[~azure.communication.rooms.RoomParticipant]
-        :return: None
+        :returns: None.
+        :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
         """
-        update_participants_request = UpdateParticipantsRequest(
-            # pylint: disable=protected-access
-            participants=[p._to_room_participant_internal() for p in participants]
-        )
-        self._rooms_service_client.rooms.update_participants(
+        update_participants_request = {
+            "participants": {p.communication_identifier.raw_id: {"role": p.role} for p in participants}
+        }
+        self._rooms_service_client.participants.update(
             room_id=room_id, update_participants_request=update_participants_request, **kwargs)
 
     @distributed_trace
     def remove_participants(
         self,
         *,
         room_id: str,
-        communication_identifiers: List[CommunicationIdentifier],
+        participants: List[Union[RoomParticipant, CommunicationIdentifier]],
         **kwargs
     ) -> None:
         """Remove participants from a room
         :param room_id: Required. Id of room to be updated
         :type room_id: str
-        :param communication_identifiers: Required. Collection of identities to be removed from the room.
-        :type communication_identifiers: List[~azure.communication.rooms._shared.models.CommunicationIdentifier]
-        :return: None
+        :param participants: Required. Collection of identities to be removed from the room.
+        :type participants:
+         List[Union[~azure.communication.rooms.RoomParticipant, ~azure.communication.rooms.CommunicationIdentifier]]
+        :returns: None.
+        :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
         """
-        participants = [
-            # pylint: disable=protected-access
-            RoomParticipant(communication_identifier=id)._to_room_participant_internal()
-            for id in communication_identifiers
-        ]
-
-        remove_participants_request = RemoveParticipantsRequest(
-            participants=participants
-        )
-        self._rooms_service_client.rooms.remove_participants(
-            room_id=room_id, remove_participants_request=remove_participants_request, **kwargs)
+        remove_participants_request = {
+            "participants": {}
+        }
+        for participant in participants:
+            try:
+                remove_participants_request["participants"][participant.communication_identifier.raw_id] = None
+            except AttributeError:
+                remove_participants_request["participants"][participant.raw_id] = None
+        self._rooms_service_client.participants.update(
+            room_id=room_id, update_participants_request=remove_participants_request, **kwargs)
 
     @distributed_trace
-    def get_participants(
+    def list_participants(
         self,
         room_id: str,
         **kwargs
-    ) -> ParticipantsCollection:
+    )-> ItemPaged[RoomParticipant]:
         """Get participants of a room
         :param room_id: Required. Id of room whose participants to be fetched.
         :type room_id: str
-        :returns: ParticipantsCollection containing all participants in the room.
-        :rtype: ~azure.communication.rooms.ParticipantsCollection
+        :returns: An iterator like instance of RoomParticipant.
+        :rtype: ~azure.core.paging.ItemPaged[~azure.communication.rooms.RoomParticipant]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        get_participants_response = self._rooms_service_client.rooms.get_participants(
-            room_id=room_id, **kwargs)
-        return ParticipantsCollection(participants=get_participants_response.participants)
+        return self._rooms_service_client.participants.list(
+            room_id=room_id,
+            cls=lambda objs: [RoomParticipant(x) for x in objs],
+            **kwargs)
+
+    def __enter__(self) -> "RoomsClient":
+        self._rooms_service_client.__enter__()
+        return self
+
+    def __exit__(self, *args: "Any") -> None:
+        self.close()
+
+    def close(self) -> None:
+        """Close the :class:
+        `~azure.communication.rooms.RoomsClient` session.
+        """
+        self._rooms_service_client.__exit__()
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_vendor.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_vendor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# Code generated by Microsoft (R) AutoRest Code Generator.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.3, generator: @autorest/python@6.4.10)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from typing import List, cast
+
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_configuration.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# Code generated by Microsoft (R) AutoRest Code Generator.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.3, generator: @autorest/python@6.4.10)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
@@ -18,37 +16,34 @@
     """Configuration for AzureCommunicationRoomsService.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2022-02-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-03-31-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
         super(AzureCommunicationRoomsServiceConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-02-01")  # type: str
+        api_version: str = kwargs.pop("api_version", "2023-03-31-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "communication-rooms/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_patch.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_client.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,79 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# Code generated by Microsoft (R) AutoRest Code Generator.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.3, generator: @autorest/python@6.4.10)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any
+from typing import Any, Awaitable
 
-from azure.core import PipelineClient
-from azure.core.rest import HttpRequest, HttpResponse
+from azure.core import AsyncPipelineClient
+from azure.core.rest import AsyncHttpResponse, HttpRequest
 
-from . import models
+from .._serialization import Deserializer, Serializer
 from ._configuration import AzureCommunicationRoomsServiceConfiguration
-from ._serialization import Deserializer, Serializer
-from .operations import RoomsOperations
+from .operations import ParticipantsOperations, RoomsOperations
 
 
 class AzureCommunicationRoomsService:  # pylint: disable=client-accepts-api-version-keyword
     """Azure Communication Room Service.
 
     :ivar rooms: RoomsOperations operations
-    :vartype rooms: azure.communication.rooms.operations.RoomsOperations
+    :vartype rooms: azure.communication.rooms.aio.operations.RoomsOperations
+    :ivar participants: ParticipantsOperations operations
+    :vartype participants: azure.communication.rooms.aio.operations.ParticipantsOperations
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2022-02-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-03-31-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
         _endpoint = "{endpoint}"
         self._config = AzureCommunicationRoomsServiceConfiguration(endpoint=endpoint, **kwargs)
-        self._client = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
-        self._serialize = Serializer(client_models)
-        self._deserialize = Deserializer(client_models)
+        self._serialize = Serializer()
+        self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.rooms = RoomsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.participants = ParticipantsOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = client.send_request(request)
-        <HttpResponse: 200 OK>
+        >>> response = await client.send_request(request)
+        <AsyncHttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.HttpResponse
+        :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
 
         request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self):
-        # type: () -> None
-        self._client.close()
-
-    def __enter__(self):
-        # type: () -> AzureCommunicationRoomsService
-        self._client.__enter__()
+    async def close(self) -> None:
+        await self._client.close()
+
+    async def __aenter__(self) -> "AzureCommunicationRoomsService":
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
-        self._client.__exit__(*exc_details)
+    async def __aexit__(self, *exc_details: Any) -> None:
+        await self._client.__aexit__(*exc_details)
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/_serialization.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,56 +21,71 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # pylint: skip-file
+# pyright: reportUnnecessaryTypeIgnoreComment=false
 
 from base64 import b64decode, b64encode
 import calendar
 import datetime
 import decimal
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
-    from urllib.parse import quote  # type: ignore
+    from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
-import isodate
-
-from typing import Dict, Any, cast, TYPE_CHECKING
+import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
-if TYPE_CHECKING:
-    from typing import Optional, Union, AnyStr, IO, Mapping
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
 
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
     CONTEXT_NAME = "deserialized_data"
 
     @classmethod
-    def deserialize_from_text(cls, data, content_type=None):
-        # type: (Optional[Union[AnyStr, IO]], Optional[str]) -> Any
+    def deserialize_from_text(cls, data: Optional[Union[AnyStr, IO]], content_type: Optional[str] = None) -> Any:
         """Decode data according to content-type.
 
         Accept a stream of data as well, but will be load at once in memory for now.
 
         If no content-type, will return the string version (not bytes, not stream)
 
         :param data: Input, could be bytes or stream (will be decoded with UTF8) or text
@@ -128,16 +143,15 @@
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
                 raise_with_traceback(DeserializationError, "XML is invalid")
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
-    def deserialize_from_http_generics(cls, body_bytes, headers):
-        # type: (Optional[Union[AnyStr, IO]], Mapping) -> Any
+    def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
         specific implementation.
         Headers will tested for "content-type"
         """
         # Try to use content-type from headers if available
@@ -156,16 +170,16 @@
         return None
 
 
 try:
     basestring  # type: ignore
     unicode_str = unicode  # type: ignore
 except NameError:
-    basestring = str  # type: ignore
-    unicode_str = str  # type: ignore
+    basestring = str
+    unicode_str = str
 
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
@@ -184,15 +198,15 @@
 
     def dst(self, dt):
         """No daylight saving for UTC."""
         return datetime.timedelta(hours=1)
 
 
 try:
-    from datetime import timezone as _FixedOffset
+    from datetime import timezone as _FixedOffset  # type: ignore
 except ImportError:  # Python 2.7
 
     class _FixedOffset(datetime.tzinfo):  # type: ignore
         """Fixed offset in minutes east from UTC.
         Copy/pasted from Python doc
         :param datetime.timedelta offset: offset in timedelta format
         """
@@ -215,15 +229,15 @@
         def __getinitargs__(self):
             return (self.__offset,)
 
 
 try:
     from datetime import timezone
 
-    TZ_UTC = timezone.utc  # type: ignore
+    TZ_UTC = timezone.utc
 except ImportError:
     TZ_UTC = UTC()  # type: ignore
 
 _FLATTEN = re.compile(r"(?<!\\)\.")
 
 
 def attribute_transformer(key, attr_desc, value):
@@ -272,79 +286,84 @@
 
 
 class Model(object):
     """Mixin for all client request body/response body models to support
     serialization and deserialization.
     """
 
-    _subtype_map = {}  # type: Dict[str, Dict[str, Any]]
-    _attribute_map = {}  # type: Dict[str, Dict[str, Any]]
-    _validation = {}  # type: Dict[str, Dict[str, Any]]
+    _subtype_map: Dict[str, Dict[str, Any]] = {}
+    _attribute_map: Dict[str, Dict[str, Any]] = {}
+    _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
-            cls._xml_map
+            cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
     def _create_xml_node(cls):
         """Create XML node."""
         try:
-            xml_map = cls._xml_map
+            xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -383,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -449,15 +473,15 @@
             if subtype_value:
                 # Try to match base class. Can be class name only
                 # (bug to fix in Autorest to support x-ms-discriminator-name)
                 if cls.__name__ == subtype_value:
                     return cls
                 flatten_mapping_type = cls._flatten_subtype(subtype_key, objects)
                 try:
-                    return objects[flatten_mapping_type[subtype_value]]
+                    return objects[flatten_mapping_type[subtype_value]]  # type: ignore
                 except KeyError:
                     _LOGGER.warning(
                         "Subtype value %s has no mapping, use base class %s.",
                         subtype_value,
                         cls.__name__,
                     )
                     break
@@ -517,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -533,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -601,47 +625,46 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
-                            serialized.set(xml_name, new_attr)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+                            serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
-                            serialized.text = new_attr
+                            serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
-                            serialized.extend(new_attr)
+                            serialized.extend(new_attr)  # type: ignore
                         elif isinstance(new_attr, ET.Element):
                             # If the down XML has no XML/Name, we MUST replace the tag with the local tag. But keeping the namespaces.
                             if "name" not in getattr(orig_attr, "_xml_map", {}):
                                 splitted_tag = new_attr.tag.split("}")
                                 if len(splitted_tag) == 2:  # Namespace
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
-                            serialized.append(new_attr)
+                            serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
-                            serialized.append(local_node)
+                            serialized.append(local_node)  # type: ignore
                     else:  # JSON
-                        for k in reversed(keys):
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                        for k in reversed(keys):  # type: ignore
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
-                        for k in keys:
+                        for k in keys:  # type: ignore
                             if k not in _serialized:
-                                _serialized.update(_new_attr)
-                            _new_attr = _new_attr[k]
+                                _serialized.update(_new_attr)  # type: ignore
+                            _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
                 except ValueError:
                     continue
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
@@ -655,31 +678,31 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
         if internal_data_type and not isinstance(internal_data_type, Enum):
             try:
                 deserializer = Deserializer(self.dependencies)
                 # Since it's on serialization, it's almost sure that format is not JSON REST
                 # We're not able to deal with additional properties for now.
                 deserializer.additional_properties_detection = False
                 if is_xml_model_serialization:
-                    deserializer.key_extractors = [
+                    deserializer.key_extractors = [  # type: ignore
                         attribute_key_case_insensitive_extractor,
                     ]
                 else:
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
@@ -776,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -839,15 +864,15 @@
         """
         try:  # If I received an enum, return its value
             return data.value
         except AttributeError:
             pass
 
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 # Don't change it, JSON and XML ElementTree are totally able
                 # to serialize correctly u'' strings
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
@@ -997,18 +1022,18 @@
     @staticmethod
     def serialize_enum(attr, enum_obj=None):
         try:
             result = attr.value
         except AttributeError:
             result = attr
         try:
-            enum_obj(result)
+            enum_obj(result)  # type: ignore
             return result
         except ValueError:
-            for enum_value in enum_obj:
+            for enum_value in enum_obj:  # type: ignore
                 if enum_value.value.lower() == str(attr).lower():
                     return enum_value.value
             error = "{!r} is not valid value for enum {!r}"
             raise SerializationError(error.format(attr, enum_obj))
 
     @staticmethod
     def serialize_bytearray(attr, **kwargs):
@@ -1160,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1241,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1265,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1331,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1351,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1412,15 +1438,15 @@
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
-            attributes = response._attribute_map
+            attributes = response._attribute_map  # type: ignore
             d_attrs = {}
             for attr, attr_desc in attributes.items():
                 # Check empty string. If it's not empty, someone has a real "additionalProperties"...
                 if attr == "additional_properties" and attr_desc["key"] == "":
                     continue
                 raw_value = None
                 # Enhance attr_desc with some dynamic data
@@ -1440,15 +1466,15 @@
                             _LOGGER.warning(msg, found_value, key_extractor, attr)
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
-            msg = "Unable to deserialize to object: " + class_name
+            msg = "Unable to deserialize to object: " + class_name  # type: ignore
             raise_with_traceback(DeserializationError, msg, err)
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
@@ -1470,46 +1496,46 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
-            _LOGGER.warning(
+            _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
             )
             return None
 
     @staticmethod
     def _unpack_content(raw_data, content_type=None):
         """Extract the correct structure for deserialization.
@@ -1539,15 +1565,15 @@
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
         if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
-            return RawDeserializer.deserialize_from_text(raw_data, content_type)
+            return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
         :param d_attrs: The deserialized response attributes.
@@ -1561,15 +1587,15 @@
                 response_obj = response(**kwargs)
                 for attr in readonly:
                     setattr(response_obj, attr, attrs.get(attr))
                 if additional_properties:
                     response_obj.additional_properties = additional_properties
                 return response_obj
             except TypeError as err:
-                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)
+                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)  # type: ignore
                 raise DeserializationError(msg + str(err))
         else:
             try:
                 for attr, value in attrs.items():
                     setattr(response, attr, value)
                 return response
             except Exception as exp:
@@ -1743,15 +1769,15 @@
         # We might be here because we have an enum modeled as string,
         # and we try to deserialize a partial dict with enum inside
         if isinstance(data, Enum):
             return data
 
         # Consider this is real string
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
 
     @staticmethod
@@ -1794,58 +1820,58 @@
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return bytearray(b64decode(attr))
+        return bytearray(b64decode(attr))  # type: ignore
 
     @staticmethod
     def deserialize_base64(attr):
         """Deserialize base64 encoded string into string.
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        padding = "=" * (3 - (len(attr) + 3) % 4)
-        attr = attr + padding
+        padding = "=" * (3 - (len(attr) + 3) % 4)  # type: ignore
+        attr = attr + padding  # type: ignore
         encoded = attr.replace("-", "+").replace("_", "/")
         return b64decode(encoded)
 
     @staticmethod
     def deserialize_decimal(attr):
         """Deserialize string into Decimal object.
 
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)
+            return decimal.Decimal(attr)  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise_with_traceback(DeserializationError, msg, err)
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
         :raises: ValueError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return _long_type(attr)
+        return _long_type(attr)  # type: ignore
 
     @staticmethod
     def deserialize_duration(attr):
         """Deserialize ISO-8601 formatted string into TimeDelta object.
 
         :param str attr: response string to be deserialized.
         :rtype: TimeDelta
@@ -1867,45 +1893,45 @@
 
         :param str attr: response string to be deserialized.
         :rtype: Date
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
         return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         return isodate.parse_time(attr)
 
     @staticmethod
     def deserialize_rfc(attr):
         """Deserialize RFC-1123 formatted string into Datetime object.
 
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            parsed_date = email.utils.parsedate_tz(attr)
+            parsed_date = email.utils.parsedate_tz(attr)  # type: ignore
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
@@ -1920,15 +1946,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            attr = attr.upper()
+            attr = attr.upper()  # type: ignore
             match = Deserializer.valid_date.match(attr)
             if not match:
                 raise ValueError("Invalid datetime string: " + attr)
 
             check_decimal = attr.split(".")
             if len(check_decimal) > 1:
                 decimal_str = ""
@@ -1956,15 +1982,15 @@
         This is represented as seconds.
 
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
-            attr = int(attr.text)
+            attr = int(attr.text)  # type: ignore
         try:
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/models/_patch.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/_patch.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/operations/_operations.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,1036 +1,1016 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# Code generated by Microsoft (R) AutoRest Code Generator.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.3, generator: @autorest/python@6.4.10)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import datetime
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+from io import IOBase
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
+    ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _format_url_section
+from ...operations._operations import (
+    build_participants_list_request,
+    build_participants_update_request,
+    build_rooms_create_request,
+    build_rooms_delete_request,
+    build_rooms_get_request,
+    build_rooms_list_request,
+    build_rooms_update_request,
+)
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
+JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_rooms_create_room_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    repeatability_request_id = kwargs.pop(
-        "repeatability_request_id", _headers.pop("Repeatability-Request-ID", None)
-    )  # type: Optional[str]
-    repeatability_first_sent = kwargs.pop(
-        "repeatability_first_sent", _headers.pop("Repeatability-First-Sent", None)
-    )  # type: Optional[datetime.datetime]
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms"
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if repeatability_request_id is not None:
-        _headers["Repeatability-Request-ID"] = _SERIALIZER.header(
-            "repeatability_request_id", repeatability_request_id, "str"
-        )
-    if repeatability_first_sent is not None:
-        _headers["Repeatability-First-Sent"] = _SERIALIZER.header(
-            "repeatability_first_sent", repeatability_first_sent, "iso-8601"
-        )
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_get_room_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_update_room_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_delete_room_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_get_participants_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}/participants"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_add_participants_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}/participants:add"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_update_participants_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}/participants:update"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_rooms_remove_participants_request(room_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-    api_version = kwargs.pop("api_version", _params.pop("api-version", "2022-02-01"))  # type: str
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/rooms/{roomId}/participants:remove"
-    path_format_arguments = {
-        "roomId": _SERIALIZER.url("room_id", room_id, "str"),
-    }
-
-    _url = _format_url_section(_url, **path_format_arguments)
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class RoomsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.communication.rooms.AzureCommunicationRoomsService`'s
+        :class:`~azure.communication.rooms.aio.AzureCommunicationRoomsService`'s
         :attr:`rooms` attribute.
     """
 
-    models = _models
-
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
-    def create_room(
+    async def create(
         self,
-        create_room_request: _models.CreateRoomRequest,
+        create_room_request: JSON,
         *,
         repeatability_request_id: Optional[str] = None,
         repeatability_first_sent: Optional[datetime.datetime] = None,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.RoomModel:
+    ) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
         :param create_room_request: The create room request body. Required.
-        :type create_room_request: ~azure.communication.rooms.models.CreateRoomRequest
+        :type create_room_request: JSON
         :keyword repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
-         Repeatability-Request-Id and get back an appropriate response without the server executing the
-         request multiple times. The value of the Repeatability-Request-Id is an opaque string
+         Repeatability-Request-ID and get back an appropriate response without the server executing the
+         request multiple times. The value of the Repeatability-Request-ID is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :paramtype repeatability_request_id: str
         :keyword repeatability_first_sent: If Repeatability-Request-ID header is specified, then
          Repeatability-First-Sent header must also be specified. The value should be the date and time
          at which the request was first created, expressed using the IMF-fixdate form of HTTP-date.
          Default value is None.
         :paramtype repeatability_first_sent: ~datetime.datetime
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                create_room_request = {
+                    "participants": {
+                        "str": {
+                            "role": "str"  # Optional. The role of a room participant.
+                              The default value is Attendee. Known values are: "Presenter", "Attendee",
+                              and "Consumer".
+                        }
+                    },
+                    "validFrom": "2020-02-20 00:00:00",  # Optional. The timestamp from when the
+                      room is open for joining. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. The default value is the current date time.
+                    "validUntil": "2020-02-20 00:00:00"  # Optional. The timestamp from when the
+                      room can no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. The default value is the current date time plus 180
+                      days.
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
         """
 
     @overload
-    def create_room(
+    async def create(
         self,
         create_room_request: IO,
         *,
         repeatability_request_id: Optional[str] = None,
         repeatability_first_sent: Optional[datetime.datetime] = None,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.RoomModel:
+    ) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
         :param create_room_request: The create room request body. Required.
         :type create_room_request: IO
         :keyword repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
-         Repeatability-Request-Id and get back an appropriate response without the server executing the
-         request multiple times. The value of the Repeatability-Request-Id is an opaque string
+         Repeatability-Request-ID and get back an appropriate response without the server executing the
+         request multiple times. The value of the Repeatability-Request-ID is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :paramtype repeatability_request_id: str
         :keyword repeatability_first_sent: If Repeatability-Request-ID header is specified, then
          Repeatability-First-Sent header must also be specified. The value should be the date and time
          at which the request was first created, expressed using the IMF-fixdate form of HTTP-date.
          Default value is None.
         :paramtype repeatability_first_sent: ~datetime.datetime
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 201
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
         """
 
-    @distributed_trace
-    def create_room(
+    @distributed_trace_async
+    async def create(
         self,
-        create_room_request: Union[_models.CreateRoomRequest, IO],
+        create_room_request: Union[JSON, IO],
         *,
         repeatability_request_id: Optional[str] = None,
         repeatability_first_sent: Optional[datetime.datetime] = None,
         **kwargs: Any
-    ) -> _models.RoomModel:
+    ) -> JSON:
         """Creates a new room.
 
         Creates a new room.
 
-        :param create_room_request: The create room request body. Is either a model type or a IO type.
+        :param create_room_request: The create room request body. Is either a JSON type or a IO type.
          Required.
-        :type create_room_request: ~azure.communication.rooms.models.CreateRoomRequest or IO
+        :type create_room_request: JSON or IO
         :keyword repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
-         Repeatability-Request-Id and get back an appropriate response without the server executing the
-         request multiple times. The value of the Repeatability-Request-Id is an opaque string
+         Repeatability-Request-ID and get back an appropriate response without the server executing the
+         request multiple times. The value of the Repeatability-Request-ID is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :paramtype repeatability_request_id: str
         :keyword repeatability_first_sent: If Repeatability-Request-ID header is specified, then
          Repeatability-First-Sent header must also be specified. The value should be the date and time
          at which the request was first created, expressed using the IMF-fixdate form of HTTP-date.
          Default value is None.
         :paramtype repeatability_first_sent: ~datetime.datetime
         :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
          Default value is None.
         :paramtype content_type: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                create_room_request = {
+                    "participants": {
+                        "str": {
+                            "role": "str"  # Optional. The role of a room participant.
+                              The default value is Attendee. Known values are: "Presenter", "Attendee",
+                              and "Consumer".
+                        }
+                    },
+                    "validFrom": "2020-02-20 00:00:00",  # Optional. The timestamp from when the
+                      room is open for joining. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. The default value is the current date time.
+                    "validUntil": "2020-02-20 00:00:00"  # Optional. The timestamp from when the
+                      room can no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. The default value is the current date time plus 180
+                      days.
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = kwargs.pop("params", {}) or {}
 
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.RoomModel]
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(create_room_request, (IO, bytes)):
+        if isinstance(create_room_request, (IOBase, bytes)):
             _content = create_room_request
         else:
-            _json = self._serialize.body(create_room_request, "CreateRoomRequest")
+            _json = create_room_request
 
-        request = build_rooms_create_room_request(
+        request = build_rooms_create_request(
             repeatability_request_id=repeatability_request_id,
             repeatability_first_sent=repeatability_first_sent,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
+            raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("RoomModel", pipeline_response)
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return deserialized
+        return cast(JSON, deserialized)
 
     @distributed_trace
-    def get_room(self, room_id: str, **kwargs: Any) -> _models.RoomModel:
+    def list(self, **kwargs: Any) -> AsyncIterable[JSON]:
+        """Retrieves all created rooms.
+
+        Retrieves all created rooms.
+
+        :return: An iterator like instance of JSON object
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                request = build_rooms_list_request(
+                    api_version=self._config.api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            return request
+
+        async def extract_data(pipeline_response):
+            deserialized = pipeline_response.http_response.json()
+            list_of_elem = deserialized["value"]
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.get("nextLink") or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    @distributed_trace_async
+    async def get(self, room_id: str, **kwargs: Any) -> JSON:
         """Retrieves an existing room by id.
 
         Retrieves an existing room by id.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.RoomModel]
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        request = build_rooms_get_room_request(
+        request = build_rooms_get_request(
             room_id=room_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
+            raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("RoomModel", pipeline_response)
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return deserialized
+        return cast(JSON, deserialized)
 
     @overload
-    def update_room(
+    async def update(
         self,
         room_id: str,
-        patch_room_request: Optional[_models.UpdateRoomRequest] = None,
+        update_room_request: JSON,
         *,
-        content_type: str = "application/json",
+        content_type: str = "application/merge-patch+json",
         **kwargs: Any
-    ) -> _models.RoomModel:
+    ) -> JSON:
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
-        :param patch_room_request: The patch room request. Default value is None.
-        :type patch_room_request: ~azure.communication.rooms.models.UpdateRoomRequest
+        :param update_room_request: The update room request. Required.
+        :type update_room_request: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
+         Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                update_room_request = {
+                    "validFrom": "2020-02-20 00:00:00",  # Optional. (Optional) The timestamp
+                      from when the room is open for joining. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``.
+                    "validUntil": "2020-02-20 00:00:00"  # Optional. (Optional) The timestamp
+                      from when the room can no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``.
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
         """
 
     @overload
-    def update_room(
+    async def update(
         self,
         room_id: str,
-        patch_room_request: Optional[IO] = None,
+        update_room_request: IO,
         *,
-        content_type: str = "application/json",
+        content_type: str = "application/merge-patch+json",
         **kwargs: Any
-    ) -> _models.RoomModel:
+    ) -> JSON:
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
-        :param patch_room_request: The patch room request. Default value is None.
-        :type patch_room_request: IO
+        :param update_room_request: The update room request. Required.
+        :type update_room_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Known values are: 'application/json', 'application/merge-patch+json'. Default value is
-         "application/json".
+         Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
         """
 
-    @distributed_trace
-    def update_room(
-        self, room_id: str, patch_room_request: Optional[Union[_models.UpdateRoomRequest, IO]] = None, **kwargs: Any
-    ) -> _models.RoomModel:
+    @distributed_trace_async
+    async def update(self, room_id: str, update_room_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update a room with given changes.
 
         Update a room with given changes.
 
         :param room_id: The id of the room requested. Required.
         :type room_id: str
-        :param patch_room_request: The patch room request. Is either a model type or a IO type. Default
-         value is None.
-        :type patch_room_request: ~azure.communication.rooms.models.UpdateRoomRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
+        :param update_room_request: The update room request. Is either a JSON type or a IO type.
+         Required.
+        :type update_room_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are:
          'application/merge-patch+json'. Default value is None.
         :paramtype content_type: str
-        :return: RoomModel
-        :rtype: ~azure.communication.rooms.models.RoomModel
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                update_room_request = {
+                    "validFrom": "2020-02-20 00:00:00",  # Optional. (Optional) The timestamp
+                      from when the room is open for joining. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``.
+                    "validUntil": "2020-02-20 00:00:00"  # Optional. (Optional) The timestamp
+                      from when the room can no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``.
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "createdAt": "2020-02-20 00:00:00",  # The timestamp when the room was
+                      created at the server. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                    "id": "str",  # Unique identifier of a room. This id is server generated.
+                      Required.
+                    "validFrom": "2020-02-20 00:00:00",  # The timestamp from when the room is
+                      open for joining. The timestamp is in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+                      Required.
+                    "validUntil": "2020-02-20 00:00:00"  # The timestamp from when the room can
+                      no longer be joined. The timestamp is in RFC3339 format:
+                      ``yyyy-MM-ddTHH:mm:ssZ``. Required.
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = kwargs.pop("params", {}) or {}
 
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.RoomModel]
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        content_type = content_type or "application/json"
+        content_type = content_type or "application/merge-patch+json"
         _json = None
         _content = None
-        if isinstance(patch_room_request, (IO, bytes)):
-            _content = patch_room_request
+        if isinstance(update_room_request, (IOBase, bytes)):
+            _content = update_room_request
         else:
-            if patch_room_request is not None:
-                _json = self._serialize.body(patch_room_request, "UpdateRoomRequest")
-            else:
-                _json = None
+            _json = update_room_request
 
-        request = build_rooms_update_room_request(
+        request = build_rooms_update_request(
             room_id=room_id,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
+            raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("RoomModel", pipeline_response)
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return deserialized
+        return cast(JSON, deserialized)
 
-    @distributed_trace
-    def delete_room(self, room_id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
+    @distributed_trace_async
+    async def delete(self, room_id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
         """Delete a room.
 
         Delete a room.
 
         :param room_id: The id of the room to be deleted. Required.
         :type room_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[None]
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_rooms_delete_room_request(
+        request = build_rooms_delete_request(
             room_id=room_id,
             api_version=self._config.api_version,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
+            raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})
 
+
+class ParticipantsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~azure.communication.rooms.aio.AzureCommunicationRoomsService`'s
+        :attr:`participants` attribute.
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
     @distributed_trace
-    def get_participants(self, room_id: str, **kwargs: Any) -> _models.ParticipantsCollection:
+    def list(self, room_id: str, **kwargs: Any) -> AsyncIterable[JSON]:
         """Get participants in a room.
 
         Get participants in a room.
 
         :param room_id: The id of the room to get participants from. Required.
         :type room_id: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
+        :return: An iterator like instance of JSON object
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
-        error_map.update(kwargs.pop("error_map", {}) or {})
 
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "rawId": "str",  # Raw ID representation of the communication identifier.
+                      Please refer to the following document for additional information on Raw ID.
+                      :code:`<br>`
+                      https://learn.microsoft.com/azure/communication-services/concepts/identifiers?pivots=programming-language-rest#raw-id-representation.
+                      Required.
+                    "role": "str"  # The role of a room participant. The default value is
+                      Attendee. Required. Known values are: "Presenter", "Attendee", and "Consumer".
+                }
+        """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ParticipantsCollection]
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        request = build_rooms_get_participants_request(
-            room_id=room_id,
-            api_version=self._config.api_version,
-            headers=_headers,
-            params=_params,
-        )
-        path_format_arguments = {
-            "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
-
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        response = pipeline_response.http_response
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
+                request = build_participants_list_request(
+                    room_id=room_id,
+                    api_version=self._config.api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        deserialized = self._deserialize("ParticipantsCollection", pipeline_response)
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            return request
+
+        async def extract_data(pipeline_response):
+            deserialized = pipeline_response.http_response.json()
+            list_of_elem = deserialized["value"]
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.get("nextLink") or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response)
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+            return pipeline_response
 
-        return deserialized
+        return AsyncItemPaged(get_next, extract_data)
 
     @overload
-    def add_participants(
+    async def update(
         self,
         room_id: str,
-        add_participants_request: _models.AddParticipantsRequest,
+        update_participants_request: JSON,
         *,
-        content_type: str = "application/json",
+        content_type: str = "application/merge-patch+json",
         **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Adds participants to a room. If participants already exist, no change occurs.
+    ) -> JSON:
+        """Update participants in a room.
 
-        Adds participants to a room. If participants already exist, no change occurs.
+        Update participants in a room.
 
-        :param room_id: Room id to add participants. Required.
+        :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
-        :param add_participants_request: Participants to be added to the room. Required.
-        :type add_participants_request: ~azure.communication.rooms.models.AddParticipantsRequest
+        :param update_participants_request: An updated set of participants of the room. Required.
+        :type update_participants_request: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
+         Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
+        :return: JSON
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
-        """
 
-    @overload
-    def add_participants(
-        self, room_id: str, add_participants_request: IO, *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Adds participants to a room. If participants already exist, no change occurs.
+        Example:
+            .. code-block:: python
 
-        Adds participants to a room. If participants already exist, no change occurs.
-
-        :param room_id: Room id to add participants. Required.
-        :type room_id: str
-        :param add_participants_request: Participants to be added to the room. Required.
-        :type add_participants_request: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
-        :raises ~azure.core.exceptions.HttpResponseError:
+                # JSON input template you can fill out and use as your body input.
+                update_participants_request = {
+                    "participants": {
+                        "str": {
+                            "role": "str"  # Optional. The role of a room participant.
+                              The default value is Attendee. Known values are: "Presenter", "Attendee",
+                              and "Consumer".
+                        }
+                    }
+                }
         """
 
-    @distributed_trace
-    def add_participants(
-        self, room_id: str, add_participants_request: Union[_models.AddParticipantsRequest, IO], **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Adds participants to a room. If participants already exist, no change occurs.
-
-        Adds participants to a room. If participants already exist, no change occurs.
-
-        :param room_id: Room id to add participants. Required.
-        :type room_id: str
-        :param add_participants_request: Participants to be added to the room. Is either a model type
-         or a IO type. Required.
-        :type add_participants_request: ~azure.communication.rooms.models.AddParticipantsRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = kwargs.pop("params", {}) or {}
-
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ParticipantsCollection]
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(add_participants_request, (IO, bytes)):
-            _content = add_participants_request
-        else:
-            _json = self._serialize.body(add_participants_request, "AddParticipantsRequest")
-
-        request = build_rooms_add_participants_request(
-            room_id=room_id,
-            content_type=content_type,
-            api_version=self._config.api_version,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        path_format_arguments = {
-            "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
-        }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
-
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
-
-        deserialized = self._deserialize("ParticipantsCollection", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
     @overload
-    def update_participants(
+    async def update(
         self,
         room_id: str,
-        update_participants_request: _models.UpdateParticipantsRequest,
+        update_participants_request: IO,
         *,
-        content_type: str = "application/json",
+        content_type: str = "application/merge-patch+json",
         **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Update participants in a room.
-
-        Update participants in a room.
-
-        :param room_id: The room id. Required.
-        :type room_id: str
-        :param update_participants_request: Participants in a room to be updated. Required.
-        :type update_participants_request: ~azure.communication.rooms.models.UpdateParticipantsRequest
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    def update_participants(
-        self, room_id: str, update_participants_request: IO, *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.ParticipantsCollection:
+    ) -> JSON:
         """Update participants in a room.
 
         Update participants in a room.
 
-        :param room_id: The room id. Required.
+        :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
-        :param update_participants_request: Participants in a room to be updated. Required.
+        :param update_participants_request: An updated set of participants of the room. Required.
         :type update_participants_request: IO
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
+         Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
+        :return: JSON
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace
-    def update_participants(
-        self, room_id: str, update_participants_request: Union[_models.UpdateParticipantsRequest, IO], **kwargs: Any
-    ) -> _models.ParticipantsCollection:
+    @distributed_trace_async
+    async def update(self, room_id: str, update_participants_request: Union[JSON, IO], **kwargs: Any) -> JSON:
         """Update participants in a room.
 
         Update participants in a room.
 
-        :param room_id: The room id. Required.
+        :param room_id: The id of the room to update the participants in. Required.
         :type room_id: str
-        :param update_participants_request: Participants in a room to be updated. Is either a model
-         type or a IO type. Required.
-        :type update_participants_request: ~azure.communication.rooms.models.UpdateParticipantsRequest
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
+        :param update_participants_request: An updated set of participants of the room. Is either a
+         JSON type or a IO type. Required.
+        :type update_participants_request: JSON or IO
+        :keyword content_type: Body Parameter content-type. Known values are:
+         'application/merge-patch+json'. Default value is None.
         :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
+        :return: JSON
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
-        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = kwargs.pop("params", {}) or {}
-
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ParticipantsCollection]
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(update_participants_request, (IO, bytes)):
-            _content = update_participants_request
-        else:
-            _json = self._serialize.body(update_participants_request, "UpdateParticipantsRequest")
+        Example:
+            .. code-block:: python
 
-        request = build_rooms_update_participants_request(
-            room_id=room_id,
-            content_type=content_type,
-            api_version=self._config.api_version,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        path_format_arguments = {
-            "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
+                # JSON input template you can fill out and use as your body input.
+                update_participants_request = {
+                    "participants": {
+                        "str": {
+                            "role": "str"  # Optional. The role of a room participant.
+                              The default value is Attendee. Known values are: "Presenter", "Attendee",
+                              and "Consumer".
+                        }
+                    }
+                }
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
-
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
-
-        deserialized = self._deserialize("ParticipantsCollection", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    @overload
-    def remove_participants(
-        self,
-        room_id: str,
-        remove_participants_request: _models.RemoveParticipantsRequest,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Remove participants from a room.
-
-        Remove participants from a room.
-
-        :param room_id: Room id to remove the participants from. Required.
-        :type room_id: str
-        :param remove_participants_request: Participants in a room to be removed. Required.
-        :type remove_participants_request: ~azure.communication.rooms.models.RemoveParticipantsRequest
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    def remove_participants(
-        self, room_id: str, remove_participants_request: IO, *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Remove participants from a room.
-
-        Remove participants from a room.
-
-        :param room_id: Room id to remove the participants from. Required.
-        :type room_id: str
-        :param remove_participants_request: Participants in a room to be removed. Required.
-        :type remove_participants_request: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @distributed_trace
-    def remove_participants(
-        self, room_id: str, remove_participants_request: Union[_models.RemoveParticipantsRequest, IO], **kwargs: Any
-    ) -> _models.ParticipantsCollection:
-        """Remove participants from a room.
-
-        Remove participants from a room.
-
-        :param room_id: Room id to remove the participants from. Required.
-        :type room_id: str
-        :param remove_participants_request: Participants in a room to be removed. Is either a model
-         type or a IO type. Required.
-        :type remove_participants_request: ~azure.communication.rooms.models.RemoveParticipantsRequest
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :return: ParticipantsCollection
-        :rtype: ~azure.communication.rooms.models.ParticipantsCollection
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError}
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = kwargs.pop("params", {}) or {}
 
-        content_type = kwargs.pop("content_type", _headers.pop("Content-Type", None))  # type: Optional[str]
-        cls = kwargs.pop("cls", None)  # type: ClsType[_models.ParticipantsCollection]
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        content_type = content_type or "application/json"
+        content_type = content_type or "application/merge-patch+json"
         _json = None
         _content = None
-        if isinstance(remove_participants_request, (IO, bytes)):
-            _content = remove_participants_request
+        if isinstance(update_participants_request, (IOBase, bytes)):
+            _content = update_participants_request
         else:
-            _json = self._serialize.body(remove_participants_request, "RemoveParticipantsRequest")
+            _json = update_participants_request
 
-        request = build_rooms_remove_participants_request(
+        request = build_participants_update_request(
             room_id=room_id,
             content_type=content_type,
             api_version=self._config.api_version,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
-        request.url = self._client.format_url(request.url, **path_format_arguments)  # type: ignore
+        request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        pipeline_response = self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=False, **kwargs
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.CommunicationErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error)
+            raise HttpResponseError(response=response)
 
-        deserialized = self._deserialize("ParticipantsCollection", pipeline_response)
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, cast(JSON, deserialized), {})
 
-        return deserialized
+        return cast(JSON, deserialized)
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_configuration.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# Code generated by Microsoft (R) AutoRest Code Generator.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.3, generator: @autorest/python@6.4.10)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
@@ -18,22 +16,22 @@
     """Configuration for AzureCommunicationRoomsService.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2022-02-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-03-31-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
         super(AzureCommunicationRoomsServiceConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "2022-02-01")  # type: str
+        api_version: str = kwargs.pop("api_version", "2023-03-31-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "communication-rooms/{}".format(VERSION))
@@ -41,11 +39,11 @@
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_patch.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_generated/aio/_client.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_generated/_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for license information.
-# Code generated by Microsoft (R) AutoRest Code Generator.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.3, generator: @autorest/python@6.4.10)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
-from typing import Any, Awaitable
+from typing import Any
 
-from azure.core import AsyncPipelineClient
-from azure.core.rest import AsyncHttpResponse, HttpRequest
+from azure.core import PipelineClient
+from azure.core.rest import HttpRequest, HttpResponse
 
-from .. import models
-from .._serialization import Deserializer, Serializer
 from ._configuration import AzureCommunicationRoomsServiceConfiguration
-from .operations import RoomsOperations
+from ._serialization import Deserializer, Serializer
+from .operations import ParticipantsOperations, RoomsOperations
 
 
 class AzureCommunicationRoomsService:  # pylint: disable=client-accepts-api-version-keyword
     """Azure Communication Room Service.
 
     :ivar rooms: RoomsOperations operations
-    :vartype rooms: azure.communication.rooms.aio.operations.RoomsOperations
+    :vartype rooms: azure.communication.rooms.operations.RoomsOperations
+    :ivar participants: ParticipantsOperations operations
+    :vartype participants: azure.communication.rooms.operations.ParticipantsOperations
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2022-02-01". Note that overriding this
-     default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2023-03-31-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
         _endpoint = "{endpoint}"
         self._config = AzureCommunicationRoomsServiceConfiguration(endpoint=endpoint, **kwargs)
-        self._client = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
-        self._serialize = Serializer(client_models)
-        self._deserialize = Deserializer(client_models)
+        self._serialize = Serializer()
+        self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.rooms = RoomsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.participants = ParticipantsOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
-        >>> response = await client.send_request(request)
-        <AsyncHttpResponse: 200 OK>
+        >>> response = client.send_request(request)
+        <HttpResponse: 200 OK>
 
         For more information on this code flow, see https://aka.ms/azsdk/dpcodegen/python/send_request
 
         :param request: The network request you want to make. Required.
         :type request: ~azure.core.rest.HttpRequest
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
-        :rtype: ~azure.core.rest.AsyncHttpResponse
+        :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
 
         request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
         return self._client.send_request(request_copy, **kwargs)
 
-    async def close(self) -> None:
-        await self._client.close()
+    def close(self) -> None:
+        self._client.close()
 
-    async def __aenter__(self) -> "AzureCommunicationRoomsService":
-        await self._client.__aenter__()
+    def __enter__(self) -> "AzureCommunicationRoomsService":
+        self._client.__enter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
-        await self._client.__aexit__(*exc_details)
+    def __exit__(self, *exc_details: Any) -> None:
+        self._client.__exit__(*exc_details)
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_models/__init__.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models import (
-    CommunicationRoom,
     RoomParticipant,
-    ParticipantsCollection
+    ParticipantRole,
+    CommunicationRoom
 )
 
 __all__ = [
-    "CommunicationRoom",
     "RoomParticipant",
-    "ParticipantsCollection"
+    "ParticipantRole",
+    "CommunicationRoom"
 ]
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/user_credential_async.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/user_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/utils_async.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/utils_async.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/policy.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/policy.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/utils.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # -------------------------------------------------------------------------
 
 import base64
 import json
 import calendar
 from typing import (cast,
                     Tuple,
+                    Union,
                     )
 from datetime import datetime
-import isodate
 from msrest.serialization import TZ_UTC
-from azure.core.credentials import AccessToken
+from azure.core.credentials import AccessToken, AzureKeyCredential
 
 
 def _convert_datetime_to_utc_int(input_datetime):
     """
     Converts DateTime in local time to the Epoch in UTC in second.
 
     :param input_datetime: Input datetime
@@ -63,30 +63,16 @@
 
 def get_current_utc_as_int():
     # type: () -> int
     current_utc_datetime = datetime.utcnow()
     return _convert_datetime_to_utc_int(current_utc_datetime)
 
 
-def verify_datetime_format(input_datetime):
-    #type: (datetime) -> bool
-    if input_datetime is None:
-        return True
-    try:
-        if isinstance(input_datetime, str):
-            input_datetime = isodate.parse_datetime(input_datetime)
-        if isinstance(input_datetime, datetime):
-            return True
-    except:
-        raise ValueError("{} is not a valid ISO-8601 datetime format".format(input_datetime)) from None
-    return True
-
-
 def create_access_token(token):
-    # type: (str) -> azure.core.credentials.AccessToken
+    # type: (str) -> AccessToken
     """Creates an instance of azure.core.credentials.AccessToken from a
     string token. The input string is jwt token in the following form:
     <token_header>.<token_payload>.<token_signature>
     This method looks into the token_payload which is a json and extracts the expiry time
     for that token and creates a tuple of type azure.core.credentials.AccessToken
     (<string_token>, <expiry>)
     :param token: User token
@@ -109,40 +95,40 @@
                            _convert_datetime_to_utc_int(datetime.fromtimestamp(payload['exp'], TZ_UTC)))
     except ValueError as val_error:
         raise ValueError(token_parse_err_msg) from val_error
 
 
 def get_authentication_policy(
         endpoint,  # type: str
-        credential,  # type: TokenCredential or str
+        credential,  # type: Union[TokenCredential, AzureKeyCredential, str]
         decode_url=False,  # type: bool
         is_async=False,  # type: bool
 ):
-    # type: (...) -> BearerTokenCredentialPolicy or HMACCredentialPolicy
+    # type: (...) -> Union[BearerTokenCredentialPolicy, HMACCredentialsPolicy]
     """Returns the correct authentication policy based
     on which credential is being passed.
     :param endpoint: The endpoint to which we are authenticating to.
     :type endpoint: str
     :param credential: The credential we use to authenticate to the service
-    :type credential: TokenCredential or str
+    :type credential: Union[TokenCredential, AzureKeyCredential, str]
     :param isAsync: For async clients there is a need to decode the url
     :type bool: isAsync or str
-    :rtype: ~azure.core.pipeline.policies.BearerTokenCredentialPolicy
-    ~HMACCredentialsPolicy
+    :rtype: ~azure.core.pipeline.policies.BearerTokenCredentialPolicy or
+    ~azure.communication.chat.shared.policy.HMACCredentialsPolicy
     """
 
     if credential is None:
         raise ValueError("Parameter 'credential' must not be None.")
     if hasattr(credential, "get_token"):
         if is_async:
             from azure.core.pipeline.policies import AsyncBearerTokenCredentialPolicy
             return AsyncBearerTokenCredentialPolicy(
                 credential, "https://communication.azure.com//.default")
         from azure.core.pipeline.policies import BearerTokenCredentialPolicy
         return BearerTokenCredentialPolicy(
             credential, "https://communication.azure.com//.default")
-    if isinstance(credential, str):
+    if isinstance(credential, (AzureKeyCredential, str)):
         from .._shared.policy import HMACCredentialsPolicy
         return HMACCredentialsPolicy(endpoint, credential, decode_url=decode_url)
 
     raise TypeError("Unsupported credential: {}. Use an access token string to use HMACCredentialsPolicy"
                     "or a token credential from azure.identity".format(type(credential)))
```

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/_shared/user_credential.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/_shared/user_credential.py`

 * *Files identical despite different names*

## Comparing `azure-communication-rooms-1.0.0b2/azure/communication/rooms/aio/_rooms_client_async.py` & `azure-communication-rooms-1.0.0b3/azure/communication/rooms/aio/_rooms_client_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union, Any
 import uuid
 
 from azure.core.credentials import AzureKeyCredential
+from azure.core.credentials_async import AsyncTokenCredential
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
-from azure.communication.rooms import RoomJoinPolicy
-from azure.communication.rooms._models import CommunicationRoom, RoomParticipant, ParticipantsCollection
+from azure.core.async_paging import AsyncItemPaged
+from azure.communication.rooms._models import (
+    RoomParticipant,
+    CommunicationRoom
+)
 from azure.communication.rooms._shared.models import CommunicationIdentifier
-from azure.communication.rooms._shared.policy import HMACCredentialsPolicy
 from .._generated.aio._client import AzureCommunicationRoomsService
-from .._shared.utils import parse_connection_str
+from .._shared.utils import parse_connection_str, get_authentication_policy
 from .._version import SDK_MONIKER
 from .._api_versions import DEFAULT_VERSION
-from .._generated.models import (
-    CreateRoomRequest,
-    UpdateRoomRequest,
-    RemoveParticipantsRequest,
-    AddParticipantsRequest,
-    UpdateParticipantsRequest
-)
 
-class RoomsClient(object): # pylint: disable=client-accepts-api-version-keyword
+
+class RoomsClient(object):
     """A client to interact with the AzureCommunicationService Rooms gateway.
 
     This client provides operations to manage rooms.
 
     :param str endpoint:
         The endpoint url for Azure Communication Service resource.
-    :param ~azure.core.credentials.AzureKeyCredential credential:
+    param Union[AsyncTokenCredential, AzureKeyCredential] credential:
         The access key we use to authenticate against the service.
+    :keyword api_version: Azure Communication Rooms API version.
+        Default value is "2023-03-31-preview".
+        Note that overriding this default value may result in unsupported behavior.
+    :paramtype api_version: str
     """
     def __init__(
-            self, endpoint: str,
-            credential: AzureKeyCredential,
+            self,
+            endpoint: str,
+            credential: Union[AsyncTokenCredential, AzureKeyCredential],
             **kwargs
     ) -> None:
         try:
             if not endpoint.lower().startswith('http'):
                 endpoint = "https://" + endpoint
         except AttributeError:
             raise ValueError("Account URL must be a string.")
 
         if not credential:
             raise ValueError(
                 "invalid credential from connection string.")
 
-        # TokenCredential not supported at the moment
-        if hasattr(credential, "get_token"):
-            raise TypeError("Unsupported credential: {}. Use an AzureKeyCredential to use HMACCredentialsPolicy"
-                    " for authentication".format(type(credential)))
+        if endpoint.endswith("/"):
+            endpoint = endpoint[:-1]
 
         self._endpoint = endpoint
         self._api_version = kwargs.pop("api_version", DEFAULT_VERSION)
-        self._authentication_policy = HMACCredentialsPolicy(endpoint, credential.key, decode_url=True)
+        self._authentication_policy = get_authentication_policy(endpoint, credential, decode_url=True, is_async=True)
         self._rooms_service_client = AzureCommunicationRoomsService(
             self._endpoint,
             api_version=self._api_version,
             authentication_policy=self._authentication_policy,
             sdk_moniker=SDK_MONIKER,
             **kwargs)
 
     @classmethod
     def from_connection_string(cls, conn_str: str,
-            **kwargs
+        **kwargs
     ) -> 'RoomsClient':
         """Create RoomsClient from a Connection String.
 
         :param str conn_str:
             A connection string to an Azure Communication Service resource.
         :returns: Instance of RoomsClient.
         :rtype: ~azure.communication.room.RoomsClient
@@ -91,107 +92,93 @@
 
     @distributed_trace_async
     async def create_room(
         self,
         *,
         valid_from: Optional[datetime] = None,
         valid_until: Optional[datetime] = None,
-        room_join_policy: Optional[RoomJoinPolicy] = None,
         participants:Optional[List[RoomParticipant]] = None,
         **kwargs
     ) -> CommunicationRoom:
         """Create a new room.
 
         :param valid_from: The timestamp from when the room is open for joining. Optional.
         :type valid_from: ~datetime.datetime
         :param valid_until: The timestamp from when the room can no longer be joined. Optional.
         :type valid_until: ~datetime.datetime
-        :param room_join_policy: The join policy of the room. Optional.
-        :type room_join_policy: ~azure.communication.rooms.models.RoomJoinPolicy
         :param participants: Collection of identities invited to the room. Optional.
         :type participants: List[~azure.communication.rooms.RoomParticipant]
         :returns: Created room.
         :rtype: ~azure.communication.rooms.CommunicationRoom
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        create_room_request = CreateRoomRequest(
-            valid_from=valid_from,
-            valid_until=valid_until,
-            room_join_policy=room_join_policy,
-            # pylint: disable=protected-access
-            participants=[p._to_room_participant_internal() for p in participants] if participants else None
-        )
+        create_room_request = {
+            "validFrom": valid_from,
+            "validUntil": valid_until
+        }
+        if participants:
+            create_room_request["participants"] = {
+                p.communication_identifier.raw_id: {"role": p.role} for p in participants
+            }
 
         repeatability_request_id = uuid.uuid1()
         repeatability_first_sent = datetime.utcnow()
 
-        create_room_response = await self._rooms_service_client.rooms.create_room(
+        create_room_response = await self._rooms_service_client.rooms.create(
             create_room_request=create_room_request,
             repeatability_request_id=repeatability_request_id,
             repeatability_first_sent=repeatability_first_sent,
             **kwargs)
-        return CommunicationRoom._from_room_response(create_room_response) # pylint: disable=protected-access
+        return CommunicationRoom(create_room_response)
 
     @distributed_trace_async
     async def delete_room(
         self,
         room_id: str,
         **kwargs
     ) -> None:
         """Delete room.
 
         :param room_id: Required. Id of room to be deleted
         :type room_id: str
         :returns: None.
         :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError
-
         """
-        await self._rooms_service_client.rooms.delete_room(room_id=room_id, **kwargs)
+        return await self._rooms_service_client.rooms.delete(room_id=room_id, **kwargs)
 
     @distributed_trace_async
     async def update_room(
         self,
         *,
         room_id: str,
-        valid_from: Optional[datetime] = None,
-        valid_until: Optional[datetime] = None,
-        room_join_policy: Optional[RoomJoinPolicy] = None,
-        participants: Optional[List[RoomParticipant]] = None,
-        **kwargs
+        valid_from: datetime,
+        valid_until: datetime,
+        **kwargs: Any
     ) -> CommunicationRoom:
         """Update a valid room's attributes. For any argument that is passed
         in, the corresponding room property will be replaced with the new value.
 
-        :param room_id: Required. Id of room to be updated
+        :keyword room_id: Required. Id of room to be updated
         :type room_id: str
-        :param valid_from: The timestamp from when the room is open for joining. Optional.
+        :keyword valid_from: Required. The timestamp from when the room is open for joining.
         :type valid_from: ~datetime.datetime
-        :param valid_until: The timestamp from when the room can no longer be joined. Optional.
+        :keyword valid_until: Required. The timestamp from when the room can no longer be joined.
         :type valid_until: ~datetime.datetime
-        :param room_join_policy: The join policy of the room. Optional.
-        :type room_join_policy: ~azure.communication.rooms.models.RoomJoinPolicy
-        :param participants: Collection of identities invited to the room. Optional.
-        :type participants: List[~azure.communication.rooms.RoomParticipant]
         :returns: Updated room.
         :rtype: ~azure.communication.rooms.CommunicationRoom
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
-
         """
-
-        update_room_request = UpdateRoomRequest(
-            valid_from=valid_from,
-            valid_until=valid_until,
-            room_join_policy=room_join_policy,
-            # pylint: disable=protected-access
-            participants=[p._to_room_participant_internal() for p in participants] if participants else None
-        )
-        update_room_response = await self._rooms_service_client.rooms.update_room(
-            room_id=room_id, patch_room_request=update_room_request, **kwargs)
-        return CommunicationRoom._from_room_response(update_room_response) # pylint: disable=protected-access
+        update_room_request = {
+            "validFrom": valid_from,
+            "validUntil": valid_until
+        }
+        update_room_response = await self._rooms_service_client.rooms.update(
+            room_id=room_id, update_room_request=update_room_request, **kwargs)
+        return CommunicationRoom(update_room_response)
 
     @distributed_trace_async
     async def get_room(
         self,
         room_id: str,
         **kwargs
     ) -> CommunicationRoom:
@@ -200,110 +187,106 @@
         :param room_id: Required. Id of room to be fetched
         :type room_id: str
         :returns: Room with current attributes.
         :rtype: ~azure.communication.rooms.CommunicationRoom
         :raises: ~azure.core.exceptions.HttpResponseError
 
         """
-        get_room_response = await self._rooms_service_client.rooms.get_room(room_id=room_id, **kwargs)
-        return CommunicationRoom._from_room_response(get_room_response) # pylint: disable=protected-access
+        get_room_response = await self._rooms_service_client.rooms.get(room_id=room_id, **kwargs)
+        return CommunicationRoom(get_room_response)
 
-    @distributed_trace_async
-    async def add_participants(
+    @distributed_trace
+    def list_rooms(
         self,
-        *,
-        room_id: str,
-        participants: List[RoomParticipant],
         **kwargs
-    ) -> None:
-        """Add participants to a roomMaximum room size is 350 participants. Adding more participants
-        will result in exceptions. Existing participants cannot be added again.
+    ) -> AsyncItemPaged[CommunicationRoom]:
+        """List all rooms
 
-        :param room_id: Required. Id of room to be updated
-        :type room_id: str
-        :param participants: Required. Collection of identities invited to the room.
-        :type participants: List[~azure.communication.rooms.RoomParticipant]
-        :return: None
-        :raises: ~azure.core.exceptions.HttpResponseError, ValueError
+        :returns: An iterator like instance of CommunicationRoom.
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.communication.rooms.CommunicationRoom]
+        :raises: ~azure.core.exceptions.HttpResponseError
         """
-        add_participants_request = AddParticipantsRequest(
-            # pylint: disable=protected-access
-            participants=[p._to_room_participant_internal() for p in participants]
+        return self._rooms_service_client.rooms.list(
+            cls=lambda rooms: [CommunicationRoom(r) for r in rooms],
+            **kwargs
         )
-        await self._rooms_service_client.rooms.add_participants(
-            room_id=room_id, add_participants_request=add_participants_request, **kwargs)
+
 
     @distributed_trace_async
-    async def update_participants(
+    async def add_or_update_participants(
         self,
         *,
         room_id: str,
         participants: List[RoomParticipant],
         **kwargs
     ) -> None:
         """Update participants to a room. It looks for the room participants based on their
         communication identifier and replace those participants with the value passed in
         this API.
         :param room_id: Required. Id of room to be updated
         :type room_id: str
         :param participants: Required. Collection of identities to be updated
         :type participants: List[~azure.communication.rooms.RoomParticipant]
-        :return: None
+        :returns: None.
+        :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
         """
-        update_participants_request = UpdateParticipantsRequest(
-            # pylint: disable=protected-access
-            participants=[p._to_room_participant_internal() for p in participants]
-        )
-        await self._rooms_service_client.rooms.update_participants(
+        update_participants_request = {
+            "participants": {p.communication_identifier.raw_id: {"role": p.role} for p in participants}
+        }
+        await self._rooms_service_client.participants.update(
             room_id=room_id, update_participants_request=update_participants_request, **kwargs)
 
     @distributed_trace_async
     async def remove_participants(
         self,
         *,
         room_id: str,
-        communication_identifiers: List[CommunicationIdentifier],
+        participants: List[Union[RoomParticipant, CommunicationIdentifier]],
         **kwargs
     ) -> None:
         """Remove participants from a room
         :param room_id: Required. Id of room to be updated
         :type room_id: str
         :param participants: Required. Collection of identities to be removed from the room.
-        :type participants: List[~azure.communication.rooms._shared.models.CommunicationIdentifier]
-        :return: None
+        :type participants:
+         List[Union[~azure.communication.rooms.RoomParticipant, ~azure.communication.rooms.CommunicationIdentifier]]
+        :returns: None.
+        :rtype: None
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
         """
-        participants = [
-            # pylint: disable=protected-access
-            RoomParticipant(communication_identifier=id)._to_room_participant_internal()
-            for id in communication_identifiers
-        ]
-        remove_participants_request = RemoveParticipantsRequest(
-            participants=participants
-        )
-        await self._rooms_service_client.rooms.remove_participants(
-            room_id=room_id, remove_participants_request=remove_participants_request, **kwargs)
+        remove_participants_request = {
+            "participants": {}
+        }
+        for participant in participants:
+            try:
+                remove_participants_request["participants"][participant.communication_identifier.raw_id] = None
+            except AttributeError:
+                remove_participants_request["participants"][participant.raw_id] = None
+        await self._rooms_service_client.participants.update(
+            room_id=room_id, update_participants_request=remove_participants_request, **kwargs)
 
-    @distributed_trace_async
-    async def get_participants(
+    @distributed_trace
+    def list_participants(
         self,
         room_id: str,
         **kwargs
-    ) -> ParticipantsCollection:
+    ) -> AsyncItemPaged[RoomParticipant]:
         """Get participants of a room
         :param room_id: Required. Id of room whose participants to be fetched.
         :type room_id: str
-        :returns: ParticipantsCollection containing all participants in the room.
-        :rtype: ~azure.communication.rooms.ParticipantsCollection
+        :returns: An iterator like instance of RoomParticipant.
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.communication.rooms.RoomParticipant]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        get_participants_response = await self._rooms_service_client.rooms.get_participants(
-            room_id=room_id, **kwargs)
-        return ParticipantsCollection(participants=get_participants_response.participants)
+        return self._rooms_service_client.participants.list(
+            room_id=room_id,
+            cls=lambda objs: [RoomParticipant(x) for x in objs],
+            **kwargs
+        )
 
     async def __aenter__(self) -> "RoomsClient":
         await self._rooms_service_client.__aenter__()
         return self
 
     async def __aexit__(self, *args: "Any") -> None:
         await self.close()
```

## Comparing `azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/PKG-INFO` & `azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-communication-rooms
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Microsoft Communication Rooms Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -59,96 +59,142 @@
 ```
 ## Examples
 
 ### Key parameters
 
 - `valid_from`: A datetime object from which room will start existing
 - `valid_until`: A datetime object after which room meeting would end
-- `room_join_policy`: The join policy of the room. Allows only participants or any communication
-        service users to join
-- `participants`: A list of RoomParticipant containing MRI's of invitees to the room
+- `participants`: A list of `RoomParticipant`s containing MRI's of invitees to the room as well as optional `ParticipantRole`. If `ParticipantRole` is not specified, then it will be `Attendee` by default.
 All the above attributes are optional. The service provides default values of valid_until and
-valid_from if they are missing.
+valid_from if they are missing. The default for`valid_from` is current date time and the default for `valid_until` is `valid_from + 180 days`.
+
+### Create a room
+To create a room, call the `create_room` function from `RoomsClient`. The `valid_from`, `valid_until`, and `participants` arguments are all optional.
 
-### Create Room
 ```python
-from azure.communication.rooms import RoomsClient
 from azure.core.exceptions import HttpResponseError
 from datetime import datetime, timedelta
+from azure.communication.rooms import (
+    RoomsClient,
+    RoomParticipant,
+    ParticipantRole
+)
+from azure.communication.identity import CommunicationUserIdentifier
 
 client = RoomsClient.from_connection_string(conn_str='<connection_str>')
+valid_from = datetime.now()
+valid_until = valid_from + relativedelta(months=+1)
+participants = []
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 1>")))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 2>"), ParticipantRole.CONSUMER))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 3>"), ParticipantRole.PRESENTER))
+
 try:
-    response = client.create_room(
-        valid_from=datetime.now(),
-        valid_until=valid_from + timedelta(weeks=4)
-        participants=["first-participant", "second-participant"]
+    create_room_response = client.create_room(
+        valid_from=valid_from,
+        valid_until=valid_until,
+        participants=participants
     )
-except HttpResponseError as e:
-    print('service responds error: {}'.format(e))
-
+except HttpResponseError as ex:
+    print(ex)
 ```
-### Update Room
-```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
-from datetime import datetime, timedelta
+### Update a room
+The `valid_from` and `valid_until` properties of a created room can be updated by calling the `update_room` function from `RoomsClient`.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>')
+```python
 try:
-    response = client.update_room(
+    update_room_response = client.update_room(
         room_id="id of the room to be updated",
         valid_from=datetime.now(),
         valid_until=valid_from + timedelta(weeks=4)
     )
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
 
 ```
 
-### Delete a Room
+### Get a room
+A created room can be retrieved by calling the `get_room` function from `RoomsClient` and passing in the associated `room_id`.
+
 ```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
+try:
+    get_room_response = client.get_room(room_id="id of the room to get")
+except HttpResponseError as ex:
+    print(ex)
+```
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>' )
+### List rooms
+Retrieve all valid rooms created with an ACS resource by calling the `list_rooms` function from `RoomsClient`.
+
+```python
+try:
+    list_room_response = client.list_rooms()
+except HttpResponseError as ex:
+    print(ex)
+```
+
+### Delete a room
+To delete a room, call the `delete_room` function from RoomsClient.
+
+```python
 try:
     client.delete_room(
         room_id="id of the room to be deleted")
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
 
 ```
 
-### Add participants to Room
-```python
-from azure.communication.rooms import RoomsClient
-from azure.core.exceptions import HttpResponseError
+### Add or update participants in a room
+In order to insert new participants or update existing participants, call the `add_or_update_participants` function from RoomsClient.
 
-client = RoomsClient.from_connection_string(conn_str='<connection_str>' )
+```python
+participants = []
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 1>")))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 2>"), ParticipantRole.ATTENDEE))
+participants.append(RoomParticipant(CommunicationUserIdentifier("<ACS User MRI identity 3>"), ParticipantRole.CONSUMER))
 try:
-    response = client.add_participants(
+    response = client.add_or_update_participants(
         room_id="id of the room to be updated",
-        participants=["new-participant-one", "new-participant-two"]
+        participants=participants
     )
 except HttpResponseError as e:
     print('service responds error: {}'.format(e))
-
 ```
 
-Please take a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms/samples) directory for detailed examples of how to use this library to create and manage rooms.
+### Remove participants
+Remove participants from a room by calling the `remove_participants` function from RoomsClient.
 
+```python
+communication_identifiers = [CommunicationUserIdentifier("<ACS User MRI identity 2>")]
+
+try:
+    remove_participants_response = client.remove_participants(
+        room_id=room_id,
+        participants=communication_identifiers
+    )
+except HttpResponseError as ex:
+    print(ex)
+```
+### List participants
+Retrieve the list of participants for an existing room by referencing the `room_id`:
+
+```python
+try:
+    participants = self.rooms_client.list_participants(room_id)
+except HttpResponseError as ex:
+    print(ex)
+```
 ## Troubleshooting
 
 Rooms operations will throw an exception if the request to the server fails. The Rooms client will raise exceptions defined in [Azure Core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md).
 
-
 ## Next steps
 ### More sample code
-
-More examples are coming soon...
+Please take a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/communication/azure-communication-rooms/samples) directory for detailed examples of how to use this library to create and manage rooms.
 
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the [Issues](https://github.com/Azure/azure-sdk-for-python/issues) section of the project
 
 ## Contributing
```

## Comparing `azure-communication-rooms-1.0.0b2/azure_communication_rooms.egg-info/SOURCES.txt` & `azure-communication-rooms-1.0.0b3/azure_communication_rooms.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/communication/__init__.py
 azure/communication/rooms/__init__.py
 azure/communication/rooms/_api_versions.py
 azure/communication/rooms/_rooms_client.py
 azure/communication/rooms/_version.py
@@ -19,18 +20,14 @@
 azure/communication/rooms/_generated/aio/__init__.py
 azure/communication/rooms/_generated/aio/_client.py
 azure/communication/rooms/_generated/aio/_configuration.py
 azure/communication/rooms/_generated/aio/_patch.py
 azure/communication/rooms/_generated/aio/operations/__init__.py
 azure/communication/rooms/_generated/aio/operations/_operations.py
 azure/communication/rooms/_generated/aio/operations/_patch.py
-azure/communication/rooms/_generated/models/__init__.py
-azure/communication/rooms/_generated/models/_enums.py
-azure/communication/rooms/_generated/models/_models.py
-azure/communication/rooms/_generated/models/_patch.py
 azure/communication/rooms/_generated/operations/__init__.py
 azure/communication/rooms/_generated/operations/_operations.py
 azure/communication/rooms/_generated/operations/_patch.py
 azure/communication/rooms/_models/__init__.py
 azure/communication/rooms/_models/_models.py
 azure/communication/rooms/_shared/__init__.py
 azure/communication/rooms/_shared/models.py
@@ -44,23 +41,20 @@
 azure_communication_rooms.egg-info/PKG-INFO
 azure_communication_rooms.egg-info/SOURCES.txt
 azure_communication_rooms.egg-info/dependency_links.txt
 azure_communication_rooms.egg-info/not-zip-safe
 azure_communication_rooms.egg-info/requires.txt
 azure_communication_rooms.egg-info/top_level.txt
 samples/rooms_client_sample.py
-tests/helper.py
+samples/rooms_client_sample_async.py
+tests/acs_rooms_test_case.py
+tests/conftest.py
 tests/test_hmac.py
 tests/test_rooms_client.py
 tests/test_rooms_client_async.py
-tests/test_rooms_client_async_e2e.py
-tests/test_rooms_client_e2e.py
-tests/testcase.py
-tests/testcase_async.py
-tests/unittest_helpers.py
 tests/_shared/__init__.py
 tests/_shared/async_fake_token_credential.py
 tests/_shared/asynctestcase.py
 tests/_shared/communication_service_preparer.py
 tests/_shared/fake_token_credential.py
 tests/_shared/helper.py
 tests/_shared/testcase.py
```

