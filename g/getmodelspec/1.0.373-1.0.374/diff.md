# Comparing `tmp/getmodelspec-1.0.373.tar.gz` & `tmp/getmodelspec-1.0.374.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.373.tar", last modified: Mon Jun 12 21:48:43 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.374.tar", last modified: Tue Jun 13 15:27:31 2023, max compression
```

## Comparing `getmodelspec-1.0.373.tar` & `getmodelspec-1.0.374.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/
--rw-rw-rw-   0        0        0      351 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/PKG-INFO
--rw-rw-rw-   0        0        0     3796 2023-06-12 13:29:40.000000 getmodelspec-1.0.373/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.373/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.373/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.373/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0    23205 2023-06-12 15:29:03.000000 getmodelspec-1.0.373/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.373/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.373/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.373/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-06-12 21:48:31.000000 getmodelspec-1.0.373/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.373/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 21:48:43.000000 getmodelspec-1.0.373/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 21:48:40.000000 getmodelspec-1.0.373/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/
+-rw-rw-rw-   0        0        0      351 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/PKG-INFO
+-rw-rw-rw-   0        0        0     3796 2023-06-12 13:29:40.000000 getmodelspec-1.0.374/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.374/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.374/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.374/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     7507 2023-06-13 15:21:27.000000 getmodelspec-1.0.374/getmodelspec/src/panasonic.py
+-rw-rw-rw-   0        0        0    23230 2023-06-13 10:21:02.000000 getmodelspec-1.0.374/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0      935 2023-06-13 15:13:47.000000 getmodelspec-1.0.374/getmodelspec/src/teast1.py
+-rw-rw-rw-   0        0        0     5284 2023-06-13 15:19:37.000000 getmodelspec-1.0.374/getmodelspec/src/test.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.374/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.374/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.374/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2512 2023-06-13 15:09:07.000000 getmodelspec-1.0.374/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.374/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-13 15:27:27.000000 getmodelspec-1.0.374/setup.py
```

### Comparing `getmodelspec-1.0.373/README.md` & `getmodelspec-1.0.374/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.373/getmodelspec/lineup.py` & `getmodelspec-1.0.374/getmodelspec/lineup.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.373/getmodelspec/src/sony.py` & `getmodelspec-1.0.374/getmodelspec/src/sony.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,33 +263,34 @@
             'L': 2023,
             'K': 2022,
             'J': 2021,
             # 추가적인 알파벳과 연도 대응 관계를 추가할 수 있음
         }
 
         # 알파벳과 대응하는 연도가 없을 경우 기본값으로 설정할 연도를 지정
-        try: dictInfo["year"] = year_mapping.get(dictInfo.get("year"))
-        except:year = ""
+        try:
+            dictInfo["year"] = year_mapping.get(dictInfo.get("year"))
+        except:
+            dictInfo["year"] =  ""
         return dictInfo
 
     def __soupToDict__(self,soup):
         try:
             h4_tag = soup.find('h4').text.strip()
             p_tag = soup.find('p').text.strip()
         except Exception as e:
             print("parser err", e)
             h4_tag = soup.find('h4').text.strip()
             p_tag =  ""
             pass
         return {h4_tag: p_tag}
 
 class GetSONYjp:
-    def __init__(self, fastMode=True,  toExcel=True):
+    def __init__(self, toExcel=True):
         self.waitTime = 10
-        self.fastMode = fastMode
         self.toExcel = toExcel
         pass
 
     def getModels(self, toExcel:bool = True) -> dict:
         self.toExcel=toExcel
         # 메인 페이지에서 시리즈를 추출
         setUrlSeries = self.__getSpecSeries__()
@@ -305,15 +306,15 @@
         for model, url in tqdm(setUrlSeries.items()):
             print(model,":", url)
             modelspec = self.__getSpec__(url=url)
             dictModels.update(modelspec)
             # backUp(dictModels, "dictModels_b")
         print("Number of all Series:", len(dictModels))
         print(dictModels)
-        # backUp(dictModels, "dictModels")
+        backUp(dictModels, "dictModels")
     # ======export====================================================================
         if self.toExcel == True:
             fileName = f"sonyJp_LineUp_{date.today().strftime('%Y-%m-%d')}"
             dictToexcel(dictModels, fileName=fileName,sheetName="Jp")  # 엑셀 파일로 저장
 
         return dictModels
 
@@ -498,24 +499,26 @@
         for footMark in footMarks:
             text = text.replace(footMark, "")
         return text
 
     def __extractInfo__(self, model):
         dictInfo = {}
         dictInfo["year"] = model.split("-")[1][-1]
-        dictInfo["series"] = model.split("-")[1][2:-1]
+        dictInfo["series"] = model.split("-")[1][2:]
         dictInfo["size"] = model.split("-")[1][:2]
         dictInfo["grade"] = model.split("-")[0]
 
         year_mapping = {
             "N": 2025,
             "M": 2024,
             'L': 2023,
             'K': 2022,
             'J': 2021,
             # 추가적인 알파벳과 연도 대응 관계를 추가할 수 있음
         }
 
         # 알파벳과 대응하는 연도가 없을 경우 기본값으로 설정할 연도를 지정
-        try: dictInfo["year"] = year_mapping.get(dictInfo.get("year"))
-        except:year = ""
+        try:
+            dictInfo["year"] = year_mapping.get(dictInfo.get("year"))
+        except:
+            dictInfo["year"] = ""
         return dictInfo
```

### Comparing `getmodelspec-1.0.373/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.374/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.373/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.374/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.373/getmodelspec/tools/functions.py` & `getmodelspec-1.0.374/getmodelspec/tools/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,13 +70,13 @@
         wb = load_workbook(filename=f"{fileName}.xlsx")
         ws = wb.create_sheet(title=sheetName)
     except FileNotFoundError:
         wb = Workbook()
         ws = wb.active
         ws.title = sheetName
 
-    for row in dataframe_to_rows(df, index=True, header=False):  # 수정된 부분
+    for row in dataframe_to_rows(df, index=True, header=True):  # 수정된 부분
         ws.append(row)
 
     wb.save(f"{fileName}.xlsx")
     print(f"데이터가 {fileName}.xlsx 파일의 {sheetName} 시트에 저장되었습니다.")
     return dictData
```

### Comparing `getmodelspec-1.0.373/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.374/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.373/setup.py` & `getmodelspec-1.0.374/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.373',
+    version='1.0.374',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

