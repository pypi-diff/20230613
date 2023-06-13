# Comparing `tmp/training_song-0.2.0.tar.gz` & `tmp/training_song-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "training_song-0.2.0.tar", max compression
+gzip compressed data, was "training_song-0.2.1.tar", max compression
```

## Comparing `training_song-0.2.0.tar` & `training_song-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2967 2023-06-13 11:36:51.907237 training_song-0.2.0/README.md
--rw-r--r--   0        0        0     1066 2023-06-13 11:36:51.907237 training_song-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/__init__.py
--rw-r--r--   0        0        0     5331 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/core.py
--rw-r--r--   0        0        0        8 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/server/.gitignore
--rw-r--r--   0        0        0        0 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/server/__init__.py
--rw-r--r--   0        0        0     3397 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/server/api.py
--rw-r--r--   0        0        0     2553 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/server/billboard_io.py
--rw-r--r--   0        0        0     2606 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/server/db.py
--rw-r--r--   0        0        0     3934 2023-06-13 11:36:51.911237 training_song-0.2.0/trainingsong/server/spotify.py
--rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 training_song-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2967 2023-06-13 12:38:37.124326 training_song-0.2.1/README.md
+-rw-r--r--   0        0        0     1066 2023-06-13 12:38:37.128326 training_song-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/__init__.py
+-rw-r--r--   0        0        0     5465 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/core.py
+-rw-r--r--   0        0        0        8 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/__init__.py
+-rw-r--r--   0        0        0     3521 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/api.py
+-rw-r--r--   0        0        0     2553 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/billboard_io.py
+-rw-r--r--   0        0        0     2646 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/db.py
+-rw-r--r--   0        0        0     4004 2023-06-13 12:38:37.128326 training_song-0.2.1/trainingsong/server/spotify.py
+-rw-r--r--   0        0        0     4172 1970-01-01 00:00:00.000000 training_song-0.2.1/PKG-INFO
```

### Comparing `training_song-0.2.0/README.md` & `training_song-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `training_song-0.2.0/pyproject.toml` & `training_song-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "training-song"
-version = "0.2.0"
+version = "0.2.1"
 description = "Audio Motivation for Data Scientists and ML Engineers"
 authors = ["koayon <koayon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "trainingsong"}]
 
 [project]
```

### Comparing `training_song-0.2.0/trainingsong/core.py` & `training_song-0.2.1/trainingsong/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,22 @@
 import os
 import re
 
 import requests
 import uvicorn
 from fastapi import FastAPI, Request
 
+PROD_API = True
+
 OAUTH_CODE = None
-URL = "https://training-song-api-koayon.vercel.app"
-local_app = FastAPI()
+if PROD_API:
+    URL = "https://training-song-api.vercel.app"
+else:
+    URL = "https://training-song-api-koayon.vercel.app"
+
 AUTH_URL = "https://accounts.spotify.com/authorize?client_id=4259770654fb4353813dbf19d8b20608&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%3A8000%2Flocal_callback&scope=user-modify-playback-state+user-read-currently-playing+user-read-recently-played+user-read-playback-state"
 LOCAL_REDIRECT_URI = "http://localhost:8000/local_callback"
 
 
 def _training_song(
     p: float,
     chart: Optional[str] = "hot-100",
@@ -39,16 +44,14 @@
 
     raw_response = requests.get(
         URL,
         params=params,
         timeout=15,
     )
 
-    print(raw_response.url)
-
     response = raw_response.json()
 
     if verbose:
         print("Congrats your model got an accuracy of", p, "percent!")
         if response and "song_info" in response:
             print(response["song_info"])
         else:
@@ -61,16 +64,16 @@
 
     return p, response
 
 
 def ts(
     input_percentage: Union[float, List[float]],
     chart="hot-100",
-    autoplay=False,
-    verbose=False,
+    autoplay=True,
+    verbose=True,
 ) -> Tuple[Union[float, List[float], None], Dict[str, Any]]:
     """Training song function.
     Starts a local server to capture the auth code from spotify and returns the song for your training accuracy.
 
     Args:
     input_percentage (float): The accuracy of your model.
     chart (str): The chart to use. Defaults to "hot-100".
@@ -103,27 +106,31 @@
             # open the authorization URL in a browser
             webbrowser.open(AUTH_URL)
 
             # wait for the user to authorize and for the server to capture the OAuth code
             while not OAUTH_CODE:
                 time.sleep(1)
 
+    # if the input percentage is a list, we want to take the final value
     accuracy = (
         input_percentage
         if isinstance(input_percentage, (float, int))
         else input_percentage[-1]
     )
 
     # now we can call the training_song function with the captured OAuth code
     acc, response = _training_song(
         accuracy, chart=chart, autoplay=autoplay, verbose=verbose, email=email
     )
     return acc, response
 
 
+local_app = FastAPI()
+
+
 @local_app.get("/local_callback")
 async def spotify_callback(request: Request):
     "Callback for the local server to capture the OAuth code"
     global OAUTH_CODE
     OAUTH_CODE = request.query_params.get("code")
     print("Got code:", OAUTH_CODE)
     return "Success! You can close this window."
```

### Comparing `training_song-0.2.0/trainingsong/server/api.py` & `training_song-0.2.1/trainingsong/server/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     p: float = Query(..., ge=0, le=100),
     chart: str = "hot-100",
     autoplay: bool = False,
 ) -> Dict[str, Union[str, bool, float, None]]:
     """The main API endpoint. It takes in a percentage p, interacts with the billboard api and then redirects to the callback for the Spotify API."""
 
     print("Hit root endpoint")
+    print(f"p: {p}")
+    print(f"chart: {chart}")
+    print(f"autoplay: {autoplay}")
 
     try:
         song_results = get_billboard_data(p, chart)
         song_results.autoplay = autoplay
     except HTTPException as e:
         raise HTTPException(status_code=404, detail=str(e)) from e
 
@@ -52,34 +55,33 @@
         sp = await create_spotify_client(spotify_client_code, email)
     except HTTPException as e:
         # raise HTTPException(
         #     status_code=404, detail=f"str(e). Failed to created Spotify client"
         # ) from e
         return {"errors": f"str(e). Failed to created Spotify client"}
 
-    print(sp)
-
     link, _name, uri = spotify_link(
         sp, song_results.song_name, song_results.artist_name
     )
 
     print(link)
 
-    print(uri)
-
-    open_link = False
+    open_link = ""
 
     if autoplay:
         errors = attempt_play(sp, uri)
         if errors:
             errors += "Failed to start playback"
-            open_link = True
+            open_link = "True"
     else:
         errors = ""
-        open_link = True
+        open_link = "True"
+
+    print(f"errors: {errors}")
+    print(f"open_link: {open_link}")
 
     output = {
         "spotify_link": link,
         "song_name": song_results.song_name,
         "artist_name": song_results.artist_name,
         "target_date": target_date,
         "percentage": song_results.percentage,
```

### Comparing `training_song-0.2.0/trainingsong/server/billboard_io.py` & `training_song-0.2.1/trainingsong/server/billboard_io.py`

 * *Files identical despite different names*

### Comparing `training_song-0.2.0/trainingsong/server/db.py` & `training_song-0.2.1/trainingsong/server/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import os
 from dotenv import load_dotenv
 from typing import Optional, Dict
 import asyncio
 from contextlib import asynccontextmanager
 
 # If running locally, load environment variables from .env
-load_dotenv()
+if os.environ.get("VERCEL") != "1":
+    load_dotenv()
 
 DATABASE_URL = os.environ.get("DATABASE_URL")
 if DATABASE_URL is None:
     raise ValueError("DATABASE_URL environment variable not set or empty")
 
 database = databases.Database(DATABASE_URL)
 metadata = sqlalchemy.MetaData()
```

### Comparing `training_song-0.2.0/trainingsong/server/spotify.py` & `training_song-0.2.1/trainingsong/server/spotify.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     update_tokens,
     database_session,
 )
 from dotenv import load_dotenv
 
 SCOPE = "user-modify-playback-state user-read-currently-playing user-read-recently-played user-read-playback-state"
 
-PROD = True
-
-if not PROD:
+# If running locally, load environment variables from .env
+if os.environ.get("VERCEL") != "1":
     load_dotenv()
 
+
 CLIENT_ID = os.environ.get("CLIENT_ID")
 CLIENT_SECRET = os.environ.get("CLIENT_SECRET")
 
 SPOTIFY_REDIRECT_URI = "http://localhost:8000/local_callback"
 
 
 @dataclass
```

### Comparing `training_song-0.2.0/PKG-INFO` & `training_song-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: training-song
-Version: 0.2.0
+Version: 0.2.1
 Summary: Audio Motivation for Data Scientists and ML Engineers
 License: MIT
 Author: koayon
 Author-email: koayon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

