# Comparing `tmp/news-scraper-python-0.0.1.tar.gz` & `tmp/news-scraper-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-scraper-python-0.0.1.tar", last modified: Tue Jun 13 09:58:52 2023, max compression
+gzip compressed data, was "news-scraper-python-0.0.2.tar", last modified: Tue Jun 13 10:11:58 2023, max compression
```

## Comparing `news-scraper-python-0.0.1.tar` & `news-scraper-python-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-13 09:58:52.321627 news-scraper-python-0.0.1/
--rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-13 09:58:52.321503 news-scraper-python-0.0.1/PKG-INFO
--rw-r--r--   0 aayushrshah   (502) staff       (20)        0 2023-06-07 11:42:35.000000 news-scraper-python-0.0.1/README.md
-drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-13 09:58:52.321334 news-scraper-python-0.0.1/news_scraper_python.egg-info/
--rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-13 09:58:52.000000 news-scraper-python-0.0.1/news_scraper_python.egg-info/PKG-INFO
--rw-r--r--   0 aayushrshah   (502) staff       (20)      232 2023-06-13 09:58:52.000000 news-scraper-python-0.0.1/news_scraper_python.egg-info/SOURCES.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-13 09:58:52.000000 news-scraper-python-0.0.1/news_scraper_python.egg-info/dependency_links.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       24 2023-06-13 09:58:52.000000 news-scraper-python-0.0.1/news_scraper_python.egg-info/requires.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-13 09:58:52.000000 news-scraper-python-0.0.1/news_scraper_python.egg-info/top_level.txt
--rw-r--r--   0 aayushrshah   (502) staff       (20)       38 2023-06-13 09:58:52.321673 news-scraper-python-0.0.1/setup.cfg
--rw-r--r--   0 aayushrshah   (502) staff       (20)     1205 2023-06-13 09:58:45.000000 news-scraper-python-0.0.1/setup.py
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-13 10:11:58.256508 news-scraper-python-0.0.2/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-13 10:11:58.256371 news-scraper-python-0.0.2/PKG-INFO
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        0 2023-06-07 11:42:35.000000 news-scraper-python-0.0.2/README.md
+drwxr-xr-x   0 aayushrshah   (502) staff       (20)        0 2023-06-13 10:11:58.256215 news-scraper-python-0.0.2/news_scraper_python.egg-info/
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      368 2023-06-13 10:11:58.000000 news-scraper-python-0.0.2/news_scraper_python.egg-info/PKG-INFO
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      232 2023-06-13 10:11:58.000000 news-scraper-python-0.0.2/news_scraper_python.egg-info/SOURCES.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-13 10:11:58.000000 news-scraper-python-0.0.2/news_scraper_python.egg-info/dependency_links.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       24 2023-06-13 10:11:58.000000 news-scraper-python-0.0.2/news_scraper_python.egg-info/requires.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)        1 2023-06-13 10:11:58.000000 news-scraper-python-0.0.2/news_scraper_python.egg-info/top_level.txt
+-rw-r--r--   0 aayushrshah   (502) staff       (20)       38 2023-06-13 10:11:58.256558 news-scraper-python-0.0.2/setup.cfg
+-rw-r--r--   0 aayushrshah   (502) staff       (20)      738 2023-06-13 10:11:47.000000 news-scraper-python-0.0.2/setup.py
```

