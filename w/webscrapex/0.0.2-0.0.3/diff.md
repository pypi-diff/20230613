# Comparing `tmp/webscrapex-0.0.2.tar.gz` & `tmp/webscrapex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscrapex-0.0.2.tar", max compression
+gzip compressed data, was "webscrapex-0.0.3.tar", max compression
```

## Comparing `webscrapex-0.0.2.tar` & `webscrapex-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      772 2023-06-13 05:04:11.316161 webscrapex-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2224 2023-06-12 14:58:23.573797 webscrapex-0.0.2/README.md
--rw-r--r--   0        0        0       48 2023-06-11 19:13:08.461920 webscrapex-0.0.2/WebScrapeX/__init__.py
--rw-r--r--   0        0        0    14137 2023-06-13 05:01:57.181782 webscrapex-0.0.2/WebScrapeX/WebScrapeX.py
--rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 webscrapex-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      772 2023-06-13 16:07:18.589349 webscrapex-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2224 2023-06-12 14:58:23.573797 webscrapex-0.0.3/README.md
+-rw-r--r--   0        0        0       48 2023-06-11 19:13:08.461920 webscrapex-0.0.3/WebScrapeX/__init__.py
+-rw-r--r--   0        0        0    14721 2023-06-13 16:06:51.159418 webscrapex-0.0.3/WebScrapeX/WebScrapeX.py
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 webscrapex-0.0.3/PKG-INFO
```

### Comparing `webscrapex-0.0.2/pyproject.toml` & `webscrapex-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebScrapeX"
-version = "0.0.2"
+version = "0.0.3"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
 authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/WebScrapeX"
 repository = "https://github.com/ILisa250/WebScrapeX"
 keywords = ["WebScrapeX", "web-data-extraction", "web-scraping", "web data collection",
```

### Comparing `webscrapex-0.0.2/README.md` & `webscrapex-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `webscrapex-0.0.2/WebScrapeX/WebScrapeX.py` & `webscrapex-0.0.3/WebScrapeX/WebScrapeX.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,44 +15,48 @@
 import psycopg2.extras
 import csv
 
 # Modules to run automatically
 import schedule # To handle scheduling tasks.
 import time as tm # For time-related operations
 
+# To manage configurations
+from decouple import config
+from dotenv import load_dotenv
+
 import os
 
 
 run_count = 0  # Counter for tracking the number of times the script has run
-def scrape_clean_save_data(url, filename):
+def scrape_clean_save_data(url, filename, env_path):
     global run_count
     global current_time
     run_count += 1
     current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S") 
-
+    
     
     #function to extract links
     #.........................
     def get_real_estate_data(url):
         """ function to extract links
 
         Params:
         .......
         url: links
 
         Usage:
         ......
         >>> from web_data_extraction import scrape_clean_save_data
-        scrape_clean_save_data("link/url", "filename")
+        scrape_clean_save_data("link/url", "filename", ".envfilepath(with credentials)")
         
         """
         # Empty list to store links
         Links = []
         #Looping through the pages
-        for page in range(1,700):
+        for page in range(1,11):
             # Headers used to specify how the HTTP request should be processed by the server. 
             # i.e - User-Agent header specifying the user agent string that should be sent with the request,
             # - Accept header specifying the types of content that the client can handle.
             headers = {'Accept-Encoding': 'gzip, deflate, sdch','Accept-Language': 'en-US,en;q=0.8','Upgrade-Insecure-Requests': '1',
                        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36',
                        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
                        'Cache-Control': 'max-age=0','Connection': 'keep-alive',}      
@@ -64,15 +68,18 @@
                 soup = BeautifulSoup(response_text, 'html.parser')
 
                 # Loop through every house's link
                 for div in soup.findAll('div', {'class': 'item-list'}):
                     # Find the link for the current property
                     link = div.find('a').attrs['href']
                     # Keep the links in the Links list
-                    Links.append("https://imali.biz" + link)  
+                    Links.append("https://imali.biz" + link) 
+                # Break the loop after collecting the first 10 page
+                if page == 2:
+                    break
             except requests.exceptions.RequestException as e:
                 print(f"An error occurred while fetching data: {e}")
         # Create a DataFrame from the list
         imali_data = pd.DataFrame({f'{filename}_links': Links})
         imali_data.to_csv(f"{filename}_links.csv")
 
     
@@ -137,16 +144,16 @@
         # Reorder columns
         all_data_df = all_data_df[["Ref_number","Build_Year","Floors","Sitting_Rooms","Dining_Rooms","Bedrooms","Wardrobes","Bathrooms","Car_Parking","Ancillary","Plot_number","LandSize", "Price", "District","Sector","Date"]]
 
         # Save the dataframe to csv file
         all_data_df.to_csv(f"{filename}_Details.csv") 
     
 
-    # Function to clean and save properties data
-    #...........................................
+    # Function to clean and save properties' data
+    #............................................
     def clean_and_save_data():
         properties = pd.read_csv(f"{filename}_Details.csv")
         # Set the 'Date' column as the index & convert it to datetime format
         properties = properties.set_index(pd.to_datetime(properties['Date']))
 
         # Drop unwanted cols from the df
         properties = properties.drop(['Ref_number', 'Plot_number', "Unnamed: 0", "Date"], axis =1)
@@ -193,43 +200,48 @@
 
         return header, column_types 
 
 
     # Function to create DB and insert data to the created table in DB
     #................................................................. 
     def insert_data_from_csv_to_imali_table(csv_file_path):
+        load_dotenv(env_path)
+        database_host = config("DATABASE_HOST")
+        database_name = config("DATABASE_NAME")
+        database_user = config("DATABASE_USER")
+        database_password = config("DATABASE_PASSWORD")
         # Establish a connection to the PostgreSQL database
         conn = psycopg2.connect(
-            host="localhost",
-            user="postgres",
-            password="Inyange"
+            host=database_host,
+            user=database_user,
+            password=database_password
         )
 
         # Create a cursor object to interact with the database
         cur = conn.cursor()
 
         # Create the database if it doesn't exist
-        cur.execute("SELECT 1 FROM pg_catalog.pg_database WHERE datname='IMALI_Properties'")
+        cur.execute(f"SELECT 1 FROM pg_catalog.pg_database WHERE datname= '{database_name}'")
         database_exists = cur.fetchone()
 
         if not database_exists:
-            cur.execute("CREATE DATABASE IMALI_Properties")
+            cur.execute(f"CREATE DATABASE {database_name}")
             conn.commit()
-            print("Database 'IMALI_Properties' created successfully.")
+            print(f"Database {database_name} created successfully.")
 
         # Close the cursor and current connection
         cur.close()
         conn.close()
 
         # Connect to the Trial database
         conn = psycopg2.connect(
-            host="localhost",
-            database="IMALI_Properties",
-            user="postgres",
-            password="Inyange"
+            host=database_host,
+            database=database_name,
+            user=database_user,
+            password=database_password
         )
 
         # Create a new cursor object to interact with the Trial database
         cur = conn.cursor()
 
         # Check if the table exists
         cur.execute(f"SELECT EXISTS (SELECT 1 FROM information_schema.tables WHERE table_name = %s)", (filename,))
@@ -288,15 +300,15 @@
         conn.close()
 
         
     # Automation
     # ..........
     # ..........
     def automation():
-        scrape_clean_save_data(url, filename)
+        scrape_clean_save_data(url, filename, env_path)
 
         # Schedule to run every 5 seconds
         schedule.every(5).seconds.do(automation)
 
         # Run the scheduler loop
         while True:
             schedule.run_pending()
@@ -314,8 +326,10 @@
         insert_data_from_csv_to_imali_table(csv_file_path)
         automation()
     
     # Determine the appropriate plural form for the word "time"
     times_word = "times" if run_count > 1 else "time"
     print("\033[1mExecution count: {}\033[0m {} | \033[1mCurrent time: {}\033[0m".format(run_count, times_word, current_time))
     # Call the combined function
-    combined_function()      
+    combined_function() 
+# Load the .env file
+env_path = os.path.abspath('.env')
```

### Comparing `webscrapex-0.0.2/PKG-INFO` & `webscrapex-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscrapex
-Version: 0.0.2
+Version: 0.0.3
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/WebScrapeX
 License: MIT
 Keywords: WebScrapeX,web-data-extraction,web-scraping,web data collection,web data integration,web data aggregation,automated data extraction,Lisa Yvette INYANGE
 Author: Lisa Yvette INYANGE
 Author-email: linyange@andrew.cmu.edu
 Requires-Python: >=3,<4
```

