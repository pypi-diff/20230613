# Comparing `tmp/wemp-1.0.0-py3-none-any.whl.zip` & `tmp/wemp-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4522 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     7052 b- defN 23-Jun-12 15:44 wemp/__init__.py
+Zip file size: 4712 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     7824 b- defN 23-Jun-13 06:46 wemp/__init__.py
 -rw-rw-r--  2.0 unx      120 b- defN 23-Jun-12 14:45 wemp/__main__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-12 15:33 wemp/http.py
--rw-rw-r--  2.0 unx      269 b- defN 23-Jun-12 15:48 wemp-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 15:48 wemp-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Jun-12 15:48 wemp-1.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-12 15:48 wemp-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-12 15:48 wemp-1.0.0.dist-info/RECORD
-8 files, 9258 bytes uncompressed, 3498 bytes compressed:  62.2%
+-rw-rw-r--  2.0 unx      269 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      590 b- defN 23-Jun-13 06:47 wemp-1.0.1.dist-info/RECORD
+8 files, 10030 bytes uncompressed, 3688 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: wemp/__main__.py
 Comment: 
 
 Filename: wemp/http.py
 Comment: 
 
-Filename: wemp-1.0.0.dist-info/METADATA
+Filename: wemp-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: wemp-1.0.0.dist-info/WHEEL
+Filename: wemp-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: wemp-1.0.0.dist-info/entry_points.txt
+Filename: wemp-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: wemp-1.0.0.dist-info/top_level.txt
+Filename: wemp-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: wemp-1.0.0.dist-info/RECORD
+Filename: wemp-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wemp/__init__.py

```diff
@@ -135,14 +135,21 @@
         dic = self.get_dict()
         for key in dic:
             val = dic[key]
             sb.append(f"   {key} = {val}")
         return "\n".join(sb)
 
 
+def pid_is_live(pid):
+    try:
+        os.kill(pid, 0)
+        return True
+    except:
+        return False
+
 class Actions:
     def __init__(self, app):
         self.app = app
         self.cfg : Config = app.cfg
 
     def private_run_cmd(self, args, remargs):
         
@@ -153,53 +160,70 @@
         del args.__dict__["cmd"]
         self.remargs = remargs
         return getattr(self, cmd)(args)
 
     def watch(self, args : argparse.Namespace):
         
         file = args.file
+        pid  = args.pid
         token = self.cfg.get_cfg("UserName") + "/" + args.token
 
+        if pid is not None:
+            if not pid_is_live(pid):
+                print(f"This pid[{pid}] is not live")
+                return False
+
         if not os.path.isfile(file):
             print(f"Is not a file: {file}")
             return False
         
         file_size = os.path.getsize(file)
         print(f"Start watching for: {file}, [{file_size} bytes]")
         print(f"You can use [{token}] to view this.")
+        system_run = True
 
-        def cycle_heart(token):
+        def cycle_heart(token, pid):
+            nonlocal system_run
             heart_url = f"{self.cfg.SERVER}/api/public/watcher/heart"
-            while True:
+            while system_run:
+                if pid is not None:
+                    if not pid_is_live(pid):
+                        http.update(update_url, token, f"Pid is shutdown\n\nlast_message is: \n{last_message}")
+                        break
+
                 http.heart(heart_url, token)
                 time.sleep(5)
 
-        heart_thread = Thread(target=cycle_heart, args=(token,))
+            system_run = False
+
+        heart_thread = Thread(target=cycle_heart, args=(token, pid))
         heart_thread.start()
 
-        url = f"{self.cfg.SERVER}/api/public/watcher/update"
+        update_url = f"{self.cfg.SERVER}/api/public/watcher/update"
+        last_message = None
         with open(file, "r") as f:
 
             if file_size > 2048:
                 f.seek(file_size - 2048, os.SEEK_SET)
 
-            while True:
+            while system_run:
                 last_line = None
                 while True:
                     line = f.readline()
                     if line:
                         last_line = line
                     else:
                         break
                 
                 if last_line:
                     last_line = last_line.strip().replace("\n", "").replace("\r", "")
                     if last_line:
                         print(f"Send: {last_line}")
-                        http.update(url, token, last_line)
+                        last_message = last_line
+                        http.update(update_url, token, last_line)
 
                 time.sleep(1)
 
         heart_thread.join()
         return True
         
 class Application:
@@ -220,12 +244,13 @@
             remargs  = args[2:]
             args = ["run", run_name]
 
         cmd = Cmd(self.actions)
         c = cmd.add_cmd("watch", "Get data from server")
         c.add_argument("file", type=str, help="repo name")
         c.add_argument("--token", type=str, default="tmp", help="token")
+        c.add_argument("--pid", type=int, help="watch program")
 
         c = cmd.add_cmd("config", "Config")
         c.add_argument("name", type=str, help="key")
         c.add_argument("value", type=str, help="value")
         return cmd.run(args, remargs)
```

## Comparing `wemp-1.0.0.dist-info/RECORD` & `wemp-1.0.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-wemp/__init__.py,sha256=G926R09hTvoXop0uA3TdsulqGzm3K9lfPSmzrDqbSL0,7052
+wemp/__init__.py,sha256=t5TjXw-_7m-9DKnLy9K65uK92X9Ab9W35i4Gi0RWvn0,7824
 wemp/__main__.py,sha256=C1ICCzLNTtUvY9b_MVidqdvUDufTmVxOAWBxjiSNiQM,120
 wemp/http.py,sha256=0uId3Zj-IqEZUWNjueiYoV3OQFDGNSnGAJDlGvONJ28,1086
-wemp-1.0.0.dist-info/METADATA,sha256=jsQvu5xF0beECzgNj7Qy0g6JpCNtKvUd43EHqvf9kOc,269
-wemp-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-wemp-1.0.0.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
-wemp-1.0.0.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
-wemp-1.0.0.dist-info/RECORD,,
+wemp-1.0.1.dist-info/METADATA,sha256=Tm_VtSZJUKF7dCCy9npiP970SczmSM2eWYS3KU1S01E,269
+wemp-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+wemp-1.0.1.dist-info/entry_points.txt,sha256=aBj9yfUx-TzXWH9rH63qSsaLH93vH00Mv-BsgzURqZA,44
+wemp-1.0.1.dist-info/top_level.txt,sha256=h3B6ac0LJnm5w6aDGvRZl1-iiZVBnZ0H9-iH2j8zdfs,5
+wemp-1.0.1.dist-info/RECORD,,
```

