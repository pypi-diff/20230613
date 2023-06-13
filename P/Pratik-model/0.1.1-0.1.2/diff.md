# Comparing `tmp/Pratik_model-0.1.1.tar.gz` & `tmp/Pratik_model-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pratik_model-0.1.1.tar", last modified: Thu Apr 27 05:15:55 2023, max compression
+gzip compressed data, was "Pratik_model-0.1.2.tar", last modified: Tue Jun 13 15:01:52 2023, max compression
```

## Comparing `Pratik_model-0.1.1.tar` & `Pratik_model-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 05:15:55.253690 Pratik_model-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-03-29 14:19:20.000000 Pratik_model-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3064 2023-04-27 05:15:55.252691 Pratik_model-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 05:15:55.198588 Pratik_model-0.1.1/Pratik_model/
--rw-rw-rw-   0        0        0    14916 2023-04-27 05:14:10.000000 Pratik_model-0.1.1/Pratik_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 05:15:55.251690 Pratik_model-0.1.1/Pratik_model.egg-info/
--rw-rw-rw-   0        0        0     3064 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2473 2023-03-31 12:45:24.000000 Pratik_model-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 05:15:55.253690 Pratik_model-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-04-27 05:12:13.000000 Pratik_model-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:01:52.721320 Pratik_model-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-03-29 14:19:20.000000 Pratik_model-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3064 2023-06-13 15:01:52.720312 Pratik_model-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 15:01:52.676797 Pratik_model-0.1.2/Pratik_model/
+-rw-rw-rw-   0        0        0    15042 2023-06-13 14:52:39.000000 Pratik_model-0.1.2/Pratik_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:01:52.719311 Pratik_model-0.1.2/Pratik_model.egg-info/
+-rw-rw-rw-   0        0        0     3064 2023-06-13 15:01:52.000000 Pratik_model-0.1.2/Pratik_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-13 15:01:52.000000 Pratik_model-0.1.2/Pratik_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:01:52.000000 Pratik_model-0.1.2/Pratik_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 15:01:52.000000 Pratik_model-0.1.2/Pratik_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 15:01:52.000000 Pratik_model-0.1.2/Pratik_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2473 2023-03-31 12:45:24.000000 Pratik_model-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:01:52.721320 Pratik_model-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-06-13 14:53:40.000000 Pratik_model-0.1.2/setup.py
```

### Comparing `Pratik_model-0.1.1/LICENSE.txt` & `Pratik_model-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pratik_model-0.1.1/PKG-INFO` & `Pratik_model-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pratik_model
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package directly gives you output performance on 13 different algorithms
 Home-page: 
 Author: pratik
 Author-email: pratikvdatey@gmail.com
 License: MIT
 Project-URL: source_code, https://github.com/pratikdatey/Pratik_model
 Keywords: Pratik_model
```

### Comparing `Pratik_model-0.1.1/Pratik_model/__init__.py` & `Pratik_model-0.1.2/Pratik_model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 
 class smart_classifier:
     def __init__(self,x,y):
         self.__x=x
         self.__y=y
 
     def accuracy_score(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbc:
                 print('CatBoost Classifier  - ',accuracy_score(testy,pred))
                 print()
 
@@ -73,15 +74,16 @@
                 print()
             else:   
                 print( '{}     -'.format(i),accuracy_score(testy,pred))
                 print()
 
 
     def f1_score(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbc:
                 print('CatBoost Classifier - ',f1_score(testy,pred))
                 print()
 
@@ -93,15 +95,16 @@
                 print('{}     - '.format(i),f1_score(testy,pred))
                 print()
            
 
 
             
     def cross_validation(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             score=cross_val_score(i,self.__x,self.__y,cv=5)
             if i==cbc:
                 print('CatBoost Classifier - ',score.mean())
                 print()
 
@@ -114,15 +117,16 @@
                 print()
 
         
 
 
             
     def precision_score(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         if (trainy.nunique())>2: # Multiclass
             print('It is multi-classed problem so for that we are calculating Presicion Score in average = "macro"')
             print()
             print()
 
             for i in name:
                 i.fit(trainx,trainy)
@@ -159,15 +163,16 @@
                 
            
         
             
             
 
     def recall_score(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         if (trainy.nunique())>2: # Multiclass
             print('It is multi-classed problem so for that we are calculating Recall Score in average = "macro"')
             print()
             print()
 
             for i in name:
                 i.fit(trainx,trainy)
@@ -203,15 +208,16 @@
                     print('{}     - '.format(i),recall_score(testy,pred,average='macro'))
                     print()
                
 
             
             
     def classification_report(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbc:
                 print('CatBoost Classifier - ')
                 print(classification_report(testy,pred),end='')
                 print()
@@ -229,15 +235,16 @@
                 print(classification_report(testy,pred),end='')
                 print()
                 print()
             
 
 
     def confusion_matrix(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbc:
                 print('CatBoost Classifier   - ')
                 print(confusion_matrix(testy,pred),end='')
                 print()
@@ -255,15 +262,16 @@
                 print(confusion_matrix(testy,pred),end='')
                 print()
                 print()
             
 
             
     def mean_squared_error(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbc:
                     print('CatBoost Classifier  - ',mean_squared_error(testy,pred))
                     print()
 
@@ -274,15 +282,16 @@
             else:   
                 print('{}     - '.format(i),mean_squared_error(testy,pred))
                 print()
            
             
             
     def mean_absolute_error(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbc:
                     print('CatBoost Classifier   - ',mean_absolute_error(testy,pred))
                     print()
 
@@ -294,15 +303,16 @@
                 print('{}      - '.format(i),mean_absolute_error(testy,pred))
                 print()
             
 
 
             
     def overfitting(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name:
             i.fit(trainx,trainy)
             pred_train=i.predict(trainx)
             pred_test=i.predict(testx)
             if i==cbc:
                 print('Training Accuracy of CatBoost Classifier    - ',accuracy_score(testy,pred_test))
                 print('Testing Accuracy  of CatBoost Classifier    - ',accuracy_score(testy,pred_test))
@@ -324,15 +334,16 @@
 class smart_regressor:
     
     def __init__(self,x,y):
         self.__x=x
         self.__y=y
         
     def r2_score(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name_r:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbr:
                 print('CatBoost Regressor - ',r2_score(testy,pred))
                 print()
 
@@ -344,15 +355,16 @@
                 print('{}      - '.format(i),r2_score(testy,pred))
                 print()  
           
             
     
             
     def cross_validation(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name_r:
             i.fit(trainx,trainy)
             score=cross_val_score(i,self.__x,self.__y,cv=5)
             if i==cbr:
                 print('CatBoost Regressor - ',score.mean())
                 print()
 
@@ -382,15 +394,16 @@
                 print('{}     - '.format(i),mean_squared_error(testy,pred))
                 print()
 
             
 
             
     def mean_absolute_error(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name_r:
             i.fit(trainx,trainy)
             pred=i.predict(testx)
             if i==cbr:
                 print('CatBoost Regressor - ',mean_absolute_error(testy,pred))
                 print()
 
@@ -401,15 +414,16 @@
             else:   
                 print('{}      - '.format(i),mean_absolute_error(testy,pred))
                 print()
 
             
             
     def overfitting(self):
-        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.25,random_state=42)
+        trainx,testx,trainy,testy=train_test_split(self.__x,self.__y,test_size=0.2
+        ,random_state=42)
         for i in name_r:
             i.fit(trainx,trainy)
             pred_train=i.predict(trainx)
             pred_test=i.predict(testx)
             if i==cbr:
                 print('Training Accuracy of CatBoost Regressor    - ',r2_score(testy,pred_test))
                 print('Testing Accuracy  of CatBoost Regressor    - ',r2_score(testy,pred_test))
```

### Comparing `Pratik_model-0.1.1/Pratik_model.egg-info/PKG-INFO` & `Pratik_model-0.1.2/Pratik_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pratik-model
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package directly gives you output performance on 13 different algorithms
 Home-page: 
 Author: pratik
 Author-email: pratikvdatey@gmail.com
 License: MIT
 Project-URL: source_code, https://github.com/pratikdatey/Pratik_model
 Keywords: Pratik_model
```

### Comparing `Pratik_model-0.1.1/README.md` & `Pratik_model-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `Pratik_model-0.1.1/setup.py` & `Pratik_model-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
   ]
 
 
 setup(
     name='Pratik_model',
-    version='0.1.1',
+    version='0.1.2',
     description='This package directly gives you output performance on 13 different algorithms',
     url='',
     license='MIT',
     author='pratik',
     long_description_content_type = open('README.md').read(),
     classifiers=classifiers,
     author_email='pratikvdatey@gmail.com',
```

