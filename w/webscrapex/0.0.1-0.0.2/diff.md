# Comparing `tmp/webscrapex-0.0.1.tar.gz` & `tmp/webscrapex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapex-0.0.1.tar", max compression
+gzip compressed data, was "webscrapex-0.0.2.tar", max compression
```

## Comparing `webscrapex-0.0.1.tar` & `webscrapex-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      772 2023-06-12 14:53:09.893531 webscrapex-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2247 2023-06-12 13:10:31.146916 webscrapex-0.0.1/README.md
--rw-r--r--   0        0        0       48 2023-06-11 19:13:08.461920 webscrapex-0.0.1/WebScrapeX/__init__.py
--rw-r--r--   0        0        0    14558 2023-06-12 11:35:25.927561 webscrapex-0.0.1/WebScrapeX/WebScrapeX.py
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 webscrapex-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      772 2023-06-13 05:04:11.316161 webscrapex-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2224 2023-06-12 14:58:23.573797 webscrapex-0.0.2/README.md
+-rw-r--r--   0        0        0       48 2023-06-11 19:13:08.461920 webscrapex-0.0.2/WebScrapeX/__init__.py
+-rw-r--r--   0        0        0    14137 2023-06-13 05:01:57.181782 webscrapex-0.0.2/WebScrapeX/WebScrapeX.py
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 webscrapex-0.0.2/PKG-INFO
```

### Comparing `webscrapex-0.0.1/pyproject.toml` & `webscrapex-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebScrapeX"
-version = "0.0.1"
+version = "0.0.2"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
 authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/WebScrapeX"
 repository = "https://github.com/ILisa250/WebScrapeX"
 keywords = ["WebScrapeX", "web-data-extraction", "web-scraping", "web data collection",
```

### Comparing `webscrapex-0.0.1/README.md` & `webscrapex-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Project description
 A comprehensive web scraping pipeline for extracting and storing real estate data
 
 ### Purpose of the package
 + The primary objective of this package is to provide an efficient solution for web scraping tasks. It has essentially functionalities including link extraction, data extraction, data cleaning, and data storage to database.
 
 ### Features
     - Date                      - Bathrooms
```

### Comparing `webscrapex-0.0.1/WebScrapeX/WebScrapeX.py` & `webscrapex-0.0.2/WebScrapeX/WebScrapeX.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
 import psycopg2.extras
 import csv
 
 # Modules to run automatically
 import schedule # To handle scheduling tasks.
 import time as tm # For time-related operations
 
-# To manage configurations
-from decouple import config
-from dotenv import load_dotenv
-
 import os
 
 
 run_count = 0  # Counter for tracking the number of times the script has run
 def scrape_clean_save_data(url, filename):
     global run_count
     global current_time
@@ -48,15 +44,15 @@
         >>> from web_data_extraction import scrape_clean_save_data
         scrape_clean_save_data("link/url", "filename")
         
         """
         # Empty list to store links
         Links = []
         #Looping through the pages
-        for page in range(1,11):
+        for page in range(1,700):
             # Headers used to specify how the HTTP request should be processed by the server. 
             # i.e - User-Agent header specifying the user agent string that should be sent with the request,
             # - Accept header specifying the types of content that the client can handle.
             headers = {'Accept-Encoding': 'gzip, deflate, sdch','Accept-Language': 'en-US,en;q=0.8','Upgrade-Insecure-Requests': '1',
                        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36',
                        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
                        'Cache-Control': 'max-age=0','Connection': 'keep-alive',}      
@@ -141,16 +137,16 @@
         # Reorder columns
         all_data_df = all_data_df[["Ref_number","Build_Year","Floors","Sitting_Rooms","Dining_Rooms","Bedrooms","Wardrobes","Bathrooms","Car_Parking","Ancillary","Plot_number","LandSize", "Price", "District","Sector","Date"]]
 
         # Save the dataframe to csv file
         all_data_df.to_csv(f"{filename}_Details.csv") 
     
 
-    # Function to clean and save properties' data
-    #............................................
+    # Function to clean and save properties data
+    #...........................................
     def clean_and_save_data():
         properties = pd.read_csv(f"{filename}_Details.csv")
         # Set the 'Date' column as the index & convert it to datetime format
         properties = properties.set_index(pd.to_datetime(properties['Date']))
 
         # Drop unwanted cols from the df
         properties = properties.drop(['Ref_number', 'Plot_number', "Unnamed: 0", "Date"], axis =1)
@@ -197,50 +193,43 @@
 
         return header, column_types 
 
 
     # Function to create DB and insert data to the created table in DB
     #................................................................. 
     def insert_data_from_csv_to_imali_table(csv_file_path):
-        # Load the .env file
-        env_path = os.path.abspath('.env')
-        load_dotenv(env_path)
-        database_host = config("DATABASE_HOST")
-        database_name = config("DATABASE_NAME")
-        database_user = config("DATABASE_USER")
-        database_password = config("DATABASE_PASSWORD")
         # Establish a connection to the PostgreSQL database
         conn = psycopg2.connect(
-            host=database_host,
-            user=database_user,
-            password=database_password
+            host="localhost",
+            user="postgres",
+            password="Inyange"
         )
 
         # Create a cursor object to interact with the database
         cur = conn.cursor()
 
         # Create the database if it doesn't exist
-        cur.execute(f"SELECT 1 FROM pg_catalog.pg_database WHERE datname= '{database_name}'")
+        cur.execute("SELECT 1 FROM pg_catalog.pg_database WHERE datname='IMALI_Properties'")
         database_exists = cur.fetchone()
 
         if not database_exists:
-            cur.execute(f"CREATE DATABASE {database_name}")
+            cur.execute("CREATE DATABASE IMALI_Properties")
             conn.commit()
-            print(f"Database {database_name} created successfully.")
+            print("Database 'IMALI_Properties' created successfully.")
 
         # Close the cursor and current connection
         cur.close()
         conn.close()
 
         # Connect to the Trial database
         conn = psycopg2.connect(
-            host=database_host,
-            database=database_name,
-            user=database_user,
-            password=database_password
+            host="localhost",
+            database="IMALI_Properties",
+            user="postgres",
+            password="Inyange"
         )
 
         # Create a new cursor object to interact with the Trial database
         cur = conn.cursor()
 
         # Check if the table exists
         cur.execute(f"SELECT EXISTS (SELECT 1 FROM information_schema.tables WHERE table_name = %s)", (filename,))
```

### Comparing `webscrapex-0.0.1/PKG-INFO` & `webscrapex-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapex
-Version: 0.0.1
+Version: 0.0.2
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/WebScrapeX
 License: MIT
 Keywords: WebScrapeX,web-data-extraction,web-scraping,web data collection,web data integration,web data aggregation,automated data extraction,Lisa Yvette INYANGE
 Author: Lisa Yvette INYANGE
 Author-email: linyange@andrew.cmu.edu
 Requires-Python: >=3,<4
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/ILisa250/WebScrapeX
 Description-Content-Type: text/markdown
 
-# Project description
 A comprehensive web scraping pipeline for extracting and storing real estate data
 
 ### Purpose of the package
 + The primary objective of this package is to provide an efficient solution for web scraping tasks. It has essentially functionalities including link extraction, data extraction, data cleaning, and data storage to database.
 
 ### Features
     - Date                      - Bathrooms
```

