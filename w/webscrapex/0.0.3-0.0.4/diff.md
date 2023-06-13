# Comparing `tmp/webscrapex-0.0.3.tar.gz` & `tmp/webscrapex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapex-0.0.3.tar", max compression
+gzip compressed data, was "webscrapex-0.0.4.tar", max compression
```

## Comparing `webscrapex-0.0.3.tar` & `webscrapex-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      772 2023-06-13 16:07:18.589349 webscrapex-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2224 2023-06-12 14:58:23.573797 webscrapex-0.0.3/README.md
--rw-r--r--   0        0        0       48 2023-06-11 19:13:08.461920 webscrapex-0.0.3/WebScrapeX/__init__.py
--rw-r--r--   0        0        0    14721 2023-06-13 16:06:51.159418 webscrapex-0.0.3/WebScrapeX/WebScrapeX.py
--rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 webscrapex-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      772 2023-06-13 16:20:09.646247 webscrapex-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2234 2023-06-13 16:17:34.369303 webscrapex-0.0.4/README.md
+-rw-r--r--   0        0        0       48 2023-06-11 19:13:08.461920 webscrapex-0.0.4/WebScrapeX/__init__.py
+-rw-r--r--   0        0        0    14721 2023-06-13 16:06:51.159418 webscrapex-0.0.4/WebScrapeX/WebScrapeX.py
+-rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 webscrapex-0.0.4/PKG-INFO
```

### Comparing `webscrapex-0.0.3/pyproject.toml` & `webscrapex-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebScrapeX"
-version = "0.0.3"
+version = "0.0.4"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
 authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/WebScrapeX"
 repository = "https://github.com/ILisa250/WebScrapeX"
 keywords = ["WebScrapeX", "web-data-extraction", "web-scraping", "web data collection",
```

### Comparing `webscrapex-0.0.3/README.md` & `webscrapex-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 # Specify the link of the real estate type to scrape
 url = "https://imali.biz/category/1/125/search?pg="
 
 # Specify the name of the file to save the data (in lowercase)
 file_name = "real_estate_data.csv"
 
 # Scrape, clean, and save the data
-scrape_clean_save_data(url, file_name)
+scrape_clean_save_data(url, file_name, env_path)
 ```
```

### Comparing `webscrapex-0.0.3/WebScrapeX/WebScrapeX.py` & `webscrapex-0.0.4/WebScrapeX/WebScrapeX.py`

 * *Files identical despite different names*

### Comparing `webscrapex-0.0.3/PKG-INFO` & `webscrapex-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapex
-Version: 0.0.3
+Version: 0.0.4
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/WebScrapeX
 License: MIT
 Keywords: WebScrapeX,web-data-extraction,web-scraping,web data collection,web data integration,web data aggregation,automated data extraction,Lisa Yvette INYANGE
 Author: Lisa Yvette INYANGE
 Author-email: linyange@andrew.cmu.edu
 Requires-Python: >=3,<4
@@ -74,9 +74,9 @@
 # Specify the link of the real estate type to scrape
 url = "https://imali.biz/category/1/125/search?pg="
 
 # Specify the name of the file to save the data (in lowercase)
 file_name = "real_estate_data.csv"
 
 # Scrape, clean, and save the data
-scrape_clean_save_data(url, file_name)
+scrape_clean_save_data(url, file_name, env_path)
 ```
```

