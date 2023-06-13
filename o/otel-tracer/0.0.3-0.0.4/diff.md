# Comparing `tmp/otel_tracer-0.0.3-py3-none-any.whl.zip` & `tmp/otel_tracer-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2195 bytes, number of entries: 7
+Zip file size: 2199 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 04:21 otel_tracer/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 04:35 otel_tracer/tracing/__init__.py
--rw-r--r--  2.0 unx     1550 b- defN 23-Jun-12 07:28 otel_tracer/tracing/tracer.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      561 b- defN 23-Jun-12 08:31 otel_tracer-0.0.3.dist-info/RECORD
-7 files, 3069 bytes uncompressed, 1187 bytes compressed:  61.3%
+-rw-r--r--  2.0 unx     1558 b- defN 23-Jun-13 06:09 otel_tracer/tracing/tracer.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      561 b- defN 23-Jun-13 06:10 otel_tracer-0.0.4.dist-info/RECORD
+7 files, 3077 bytes uncompressed, 1191 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: otel_tracer/tracing/__init__.py
 Comment: 
 
 Filename: otel_tracer/tracing/tracer.py
 Comment: 
 
-Filename: otel_tracer-0.0.3.dist-info/METADATA
+Filename: otel_tracer-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: otel_tracer-0.0.3.dist-info/WHEEL
+Filename: otel_tracer-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: otel_tracer-0.0.3.dist-info/top_level.txt
+Filename: otel_tracer-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: otel_tracer-0.0.3.dist-info/RECORD
+Filename: otel_tracer-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otel_tracer/tracing/tracer.py

```diff
@@ -3,16 +3,14 @@
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.instrumentation.pika import PikaInstrumentor
 from opentelemetry.instrumentation.redis import RedisInstrumentor
-from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
-from opentelemetry.instrumentation.celery import CeleryInstrumentor
 
 
 def flask_tracer(app, servicename, endpoint):
     FlaskInstrumentor().instrument_app(app)
 
     trace.set_tracer_provider(
         TracerProvider(
@@ -38,12 +36,14 @@
 
 
 def pika_tracer():
     PikaInstrumentor().instrument()
 
 
 def celery_tracer():
+    from opentelemetry.instrumentation.celery import CeleryInstrumentor
     CeleryInstrumentor().instrument()
 
 
 def flask_sqlalchemy_tracer():
+    from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
     SQLAlchemyInstrumentor().instrument(enable_commenter=True, commenter_options={})
```

## Comparing `otel_tracer-0.0.3.dist-info/METADATA` & `otel_tracer-0.0.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otel-tracer
-Version: 0.0.3
+Version: 0.0.4
 Summary: common python utilities for otel
 Home-page: UNKNOWN
 Author: VxRail
 Author-email: UNKNOWN
 License: ToBeDone
 Platform: python3
 Requires-Dist: flask
```

## Comparing `otel_tracer-0.0.3.dist-info/RECORD` & `otel_tracer-0.0.4.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 otel_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-otel_tracer/tracing/tracer.py,sha256=7fGT0kPmNvd2wUpwbsMIjnjjaQKK6v8KlyB_LAztRAI,1550
-otel_tracer-0.0.3.dist-info/METADATA,sha256=iSmJAS3CczXCr4dz1I6_ZS76PZW6Pt9XK9hyoK_nsZI,854
-otel_tracer-0.0.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-otel_tracer-0.0.3.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
-otel_tracer-0.0.3.dist-info/RECORD,,
+otel_tracer/tracing/tracer.py,sha256=VF2Ubebg28XrOnEga4zMmwAVvO-49vtFxzslUam9yEQ,1558
+otel_tracer-0.0.4.dist-info/METADATA,sha256=pnlpxe4LZJoMQS3UKKdV-0FeKuCg_YXnrIbJsOgaVss,854
+otel_tracer-0.0.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+otel_tracer-0.0.4.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
+otel_tracer-0.0.4.dist-info/RECORD,,
```

