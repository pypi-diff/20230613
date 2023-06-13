# Comparing `tmp/politikontroller_app-1.0.0.tar.gz` & `tmp/politikontroller_app-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politikontroller_app-1.0.0.tar", max compression
+gzip compressed data, was "politikontroller_app-1.0.1.tar", max compression
```

## Comparing `politikontroller_app-1.0.0.tar` & `politikontroller_app-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      375 2023-06-11 22:23:05.047755 politikontroller_app-1.0.0/README.md
--rw-r--r--   0        0        0       36 2023-06-11 22:13:02.037096 politikontroller_app-1.0.0/politikontroller_app/__init__.py
--rw-r--r--   0        0        0      431 2023-06-11 21:30:10.115267 politikontroller_app-1.0.0/politikontroller_app/__main__.py
--rw-r--r--   0        0        0     2413 2023-06-11 21:53:03.540450 politikontroller_app-1.0.0/politikontroller_app/conftest.py
--rw-r--r--   0        0        0      173 2023-06-11 22:42:09.708398 politikontroller_app-1.0.0/politikontroller_app/db/base.py
--rw-r--r--   0        0        0      960 2023-06-11 21:27:24.350843 politikontroller_app-1.0.0/politikontroller_app/db/dao.py
--rw-r--r--   0        0        0       46 2023-05-27 00:43:20.524812 politikontroller_app-1.0.0/politikontroller_app/db/meta.py
--rw-r--r--   0        0        0      403 2023-05-27 00:43:20.532812 politikontroller_app-1.0.0/politikontroller_app/db/models/__init__.py
--rw-r--r--   0        0        0      525 2023-06-11 22:41:53.976336 politikontroller_app-1.0.0/politikontroller_app/db/models/access_token.py
--rw-r--r--   0        0        0      270 2023-05-27 00:43:36.736965 politikontroller_app-1.0.0/politikontroller_app/db/utils.py
--rw-r--r--   0        0        0     1785 2023-06-11 21:53:19.396514 politikontroller_app-1.0.0/politikontroller_app/logging.py
--rw-r--r--   0        0        0     2664 2023-06-11 21:59:04.565878 politikontroller_app-1.0.0/politikontroller_app/settings.py
--rw-r--r--   0        0        0        0 2023-05-27 23:15:19.853226 politikontroller_app-1.0.0/politikontroller_app/shared/__init__.py
--rw-r--r--   0        0        0     1362 2023-06-11 21:19:31.266112 politikontroller_app-1.0.0/politikontroller_app/shared/dependencies.py
--rw-r--r--   0        0        0      456 2023-06-11 20:01:36.181661 politikontroller_app-1.0.0/politikontroller_app/shared/responses.py
--rw-r--r--   0        0        0       38 2023-05-27 00:43:20.836815 politikontroller_app-1.0.0/politikontroller_app/tests/__init__.py
--rw-r--r--   0        0        0      479 2023-05-27 00:43:36.776965 politikontroller_app-1.0.0/politikontroller_app/tests/test_politikontroller_app.py
--rw-r--r--   0        0        0       40 2023-05-27 00:43:20.596812 politikontroller_app-1.0.0/politikontroller_app/web/__init__.py
--rw-r--r--   0        0        0       40 2023-05-27 00:43:20.700813 politikontroller_app-1.0.0/politikontroller_app/web/api/__init__.py
--rw-r--r--   0        0        0      126 2023-05-27 09:40:37.040866 politikontroller_app-1.0.0/politikontroller_app/web/api/monitoring/__init__.py
--rw-r--r--   0        0        0      204 2023-05-27 00:43:34.276942 politikontroller_app-1.0.0/politikontroller_app/web/api/monitoring/views.py
--rw-r--r--   0        0        0      122 2023-05-29 09:20:55.610880 politikontroller_app-1.0.0/politikontroller_app/web/api/police_controls/__init__.py
--rw-r--r--   0        0        0     1887 2023-06-11 20:04:04.962619 politikontroller_app-1.0.0/politikontroller_app/web/api/police_controls/views.py
--rw-r--r--   0        0        0      317 2023-05-29 12:50:48.355670 politikontroller_app-1.0.0/politikontroller_app/web/api/router.py
--rw-r--r--   0        0        0      111 2023-05-30 03:47:46.626618 politikontroller_app-1.0.0/politikontroller_app/web/api/user/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-11 21:20:01.246128 politikontroller_app-1.0.0/politikontroller_app/web/api/user/views.py
--rw-r--r--   0        0        0      988 2023-06-11 22:05:56.171469 politikontroller_app-1.0.0/politikontroller_app/web/application.py
--rw-r--r--   0        0        0     2012 2023-06-11 22:06:46.011660 politikontroller_app-1.0.0/politikontroller_app/web/lifetime.py
--rw-r--r--   0        0        0     1418 2023-06-11 23:00:59.313725 politikontroller_app-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 politikontroller_app-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/LICENSE
+-rw-r--r--   0        0        0      375 2023-06-12 06:12:51.006500 politikontroller_app-1.0.1/README.md
+-rw-r--r--   0        0        0       36 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/__init__.py
+-rw-r--r--   0        0        0      431 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/__main__.py
+-rw-r--r--   0        0        0     2413 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/conftest.py
+-rw-r--r--   0        0        0      173 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/db/base.py
+-rw-r--r--   0        0        0      960 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/db/dao.py
+-rw-r--r--   0        0        0       46 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/db/meta.py
+-rw-r--r--   0        0        0      403 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/db/models/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/db/models/access_token.py
+-rw-r--r--   0        0        0      270 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/db/utils.py
+-rw-r--r--   0        0        0     1785 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/logging.py
+-rw-r--r--   0        0        0     2664 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/settings.py
+-rw-r--r--   0        0        0        0 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/shared/__init__.py
+-rw-r--r--   0        0        0     1362 2023-06-13 00:06:05.094788 politikontroller_app-1.0.1/politikontroller_app/shared/dependencies.py
+-rw-r--r--   0        0        0      456 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/shared/responses.py
+-rw-r--r--   0        0        0       38 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/tests/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/tests/test_politikontroller_app.py
+-rw-r--r--   0        0        0       40 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/web/__init__.py
+-rw-r--r--   0        0        0       40 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/web/api/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-12 06:12:51.002499 politikontroller_app-1.0.1/politikontroller_app/web/api/monitoring/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-12 06:12:51.006500 politikontroller_app-1.0.1/politikontroller_app/web/api/monitoring/views.py
+-rw-r--r--   0        0        0      122 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/web/api/police_controls/__init__.py
+-rw-r--r--   0        0        0     1887 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/web/api/police_controls/views.py
+-rw-r--r--   0        0        0      317 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/web/api/router.py
+-rw-r--r--   0        0        0      111 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/web/api/user/__init__.py
+-rw-r--r--   0        0        0     1878 2023-06-13 00:05:13.310458 politikontroller_app-1.0.1/politikontroller_app/web/api/user/views.py
+-rw-r--r--   0        0        0      988 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/web/application.py
+-rw-r--r--   0        0        0     2012 2023-06-12 06:12:51.010500 politikontroller_app-1.0.1/politikontroller_app/web/lifetime.py
+-rw-r--r--   0        0        0     1231 2023-06-13 00:28:58.454886 politikontroller_app-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 politikontroller_app-1.0.1/PKG-INFO
```

### Comparing `politikontroller_app-1.0.0/politikontroller_app/conftest.py` & `politikontroller_app-1.0.1/politikontroller_app/conftest.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/db/dao.py` & `politikontroller_app-1.0.1/politikontroller_app/db/dao.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/db/models/access_token.py` & `politikontroller_app-1.0.1/politikontroller_app/db/models/access_token.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/logging.py` & `politikontroller_app-1.0.1/politikontroller_app/logging.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/settings.py` & `politikontroller_app-1.0.1/politikontroller_app/settings.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/shared/dependencies.py` & `politikontroller_app-1.0.1/politikontroller_app/shared/dependencies.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/web/api/police_controls/views.py` & `politikontroller_app-1.0.1/politikontroller_app/web/api/police_controls/views.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/web/api/user/views.py` & `politikontroller_app-1.0.1/politikontroller_app/web/api/user/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 @router.post("/token")
 async def user_login(
     form_data: Annotated[OAuth2PasswordRequestForm, Depends()],
     db: AsyncSession = Depends(get_db_session),
 ):
     dao = Auth(db)
     try:
-        user = client.authenticate_user(47, int(form_data.username), form_data.password)
+        user = client.authenticate_user(form_data.username, form_data.password)
     except HTTPError as err:
         raise HTTPException(403, detail=str(err)) from err
     except AuthenticationError as err:
         raise HTTPException(403) from err
 
     # user = User(**user_dict)
     token = dao.create_access_token(user.username, form_data.password)
 
-    return {"access_token": token, "token_type": "bearer"}
+    return {"access_token": token.token, "token_type": "bearer"}
 
 
 @router.get("/settings")
 async def user_settings(
     current_user: Annotated[Account, Depends(get_current_active_user)]
 ):
     client.set_user(current_user)
```

### Comparing `politikontroller_app-1.0.0/politikontroller_app/web/application.py` & `politikontroller_app-1.0.1/politikontroller_app/web/application.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/politikontroller_app/web/lifetime.py` & `politikontroller_app-1.0.1/politikontroller_app/web/lifetime.py`

 * *Files identical despite different names*

### Comparing `politikontroller_app-1.0.0/pyproject.toml` & `politikontroller_app-1.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "politikontroller-app"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Bendik R. Brenne <bendik@konstant.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "politikontroller_app" }
 ]
@@ -20,42 +20,36 @@
 aiosqlite = "^0.19.0"
 httptools = "^0.5.0"
 loguru = "^0.7.0"
 pycryptodome = "^3.18.0"
 requests = "^2.31.0"
 python-multipart = "^0.0.6"
 geojson = "^3.0.1"
-politikontroller-py = "^1.0.0"
+politikontroller-py = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pylint = "^2.17.4"
 autopep8 = "^2.0.2"
 isort = "^5.11.4"
 pre-commit = "^3.3.1"
 black = "^23.3.0"
 httpx = "^0.24.1"
-politikontroller-py = { path = "../politikontroller-py" }
 pylint-pydantic = "^0.1.8"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
-src_paths = ["src"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
     "ignore::DeprecationWarning",
     "ignore:.*unclosed.*:ResourceWarning",
 ]
-env = [
-    "POLITIKONTROLLER_APP_ENVIRONMENT=pytest",
-    "POLITIKONTROLLER_APP_DB_FILE=test_db.sqlite3",
-]
 
 [tool.poetry.scripts]
 run = "politikontroller_app.main:main"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `politikontroller_app-1.0.0/PKG-INFO` & `politikontroller_app-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politikontroller-app
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: Bendik R. Brenne
 Author-email: bendik@konstant.no
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy[asyncio] (>=2.0.15,<3.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: fastapi (>=0.96.1,<0.97.0)
 Requires-Dist: geojson (>=3.0.1,<4.0.0)
 Requires-Dist: httptools (>=0.5.0,<0.6.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: politikontroller-py (>=1.0.0,<2.0.0)
+Requires-Dist: politikontroller-py (>=1.1.0,<2.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.9,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ujson (>=5.8.0,<6.0.0)
 Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
```

