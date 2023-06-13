# Comparing `tmp/lazydev-0.0.7.tar.gz` & `tmp/lazydev-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.7.tar", last modified: Sun Jun  4 17:58:33 2023, max compression
+gzip compressed data, was "lazydev-0.0.8.tar", last modified: Tue Jun 13 08:12:03 2023, max compression
```

## Comparing `lazydev-0.0.7.tar` & `lazydev-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.652992 lazydev-0.0.7/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.7/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-04 17:58:33.652843 lazydev-0.0.7/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3883 2023-06-03 08:10:06.000000 lazydev-0.0.7/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.650654 lazydev-0.0.7/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.7/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.7/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.652532 lazydev-0.0.7/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.7/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     7279 2023-06-04 17:01:33.000000 lazydev-0.0.7/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     6118 2023-06-04 08:58:14.000000 lazydev-0.0.7/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.0.7/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.651639 lazydev-0.0.7/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-04 17:58:33.653034 lazydev-0.0.7/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1482 2023-06-04 17:58:23.000000 lazydev-0.0.7/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.665321 lazydev-0.0.8/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.8/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-13 08:12:03.665161 lazydev-0.0.8/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3883 2023-06-03 08:10:06.000000 lazydev-0.0.8/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.662711 lazydev-0.0.8/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.8/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.8/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.664739 lazydev-0.0.8/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.8/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     7760 2023-06-13 08:08:23.000000 lazydev-0.0.8/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     6898 2023-06-13 08:10:27.000000 lazydev-0.0.8/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.0.8/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-13 08:12:03.663775 lazydev-0.0.8/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-13 08:12:03.000000 lazydev-0.0.8/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-13 08:12:03.665367 lazydev-0.0.8/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1482 2023-06-13 08:10:38.000000 lazydev-0.0.8/setup.py
```

### Comparing `lazydev-0.0.7/LICENSE` & `lazydev-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.7/PKG-INFO` & `lazydev-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.7/README.md` & `lazydev-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.7/lazydev/develop.py` & `lazydev-0.0.8/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.7/lazydev/modules/developer.py` & `lazydev-0.0.8/lazydev/modules/developer.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,16 +57,20 @@
                       for doubt in doubt_list if doubt.strip() != ""]
         return doubt_list
 
     def get_clarifications(self, doubts: List[str], answers: List[str]):
         clarifications = ""
         for i in range(len(doubts)):
             clarifications = f"{clarifications}\n\n{i+1}. {doubts[i]}\n Ans: {answers[i]}"
-        self.clarifications = clarifications
-        return clarifications
+
+        compressed_clarrifications = self.brain_storm(
+            PromptBook.get_compressed_text(clarifications), "compressed_clarrifications")
+        self.clarifications = compressed_clarrifications
+
+        return compressed_clarrifications
 
     def clear_doubts(self):
         doubt_list = self.get_doubts()
         print("""
 Hey there! 😄 It's Lazy Dev, your friendly neighborhood programmer, here to make your awesome project's dreams come true! 🎉 
 But before I dive into coding magic, I have a few fun and important questions for you. 
 So, grab a cup of coffee ☕️, sit back, and let's clarify some details, shall we? Here we go! 🚀
@@ -86,16 +90,18 @@
 Cheers! 👨‍💻
         """)
         return doubt_list, answer_list
 
     def plan_project(self):
         prompt = PromptBook.plan_project(self.requirement, self.clarifications)
         plannings: str = self.brain_storm(prompt, 'plan-project')
-        self.plannings = plannings
-        return plannings
+        compressed_plan = self.brain_storm(
+            PromptBook.get_compressed_text(plannings), "compressed_plan")
+        self.plannings = compressed_plan
+        return compressed_plan
 
     def generate_folder_structure(self):
         prompt = PromptBook.design_folder_structure(
             question=self.requirement,
             plan=self.plannings,
             clarifications=self.clarifications
         )
@@ -162,17 +168,20 @@
                     review_prompt, f'code-{file_path.split("/")[-1]}')
                 response = response.strip('"\'`-\n')
                 if (response.strip('"\'`-\n') == "NONE"):
                     break
                 code = response
 
         Utilities.write_to_file(code, file_path=file_path)
+        # compress the code
+        compressed_code = self.brain_storm(PromptBook.get_compressed_code(
+            code), f'code-compressed-{file_path.split("/")[-1]}')
         self.files_written.append((
             file_path,
-            code
+            compressed_code
         ))
 
     def develop(self):
         # clearing all doubts
         doubts, answers = self.clear_doubts()
         self.clarifications = self.get_clarifications(
             doubts=doubts, answers=answers)
```

### Comparing `lazydev-0.0.7/lazydev/modules/prompts.py` & `lazydev-0.0.8/lazydev/modules/prompts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from typing import List
 
 
 class PromptBook:
     @staticmethod
-    def expand_requirements(question:str)->str:
+    def expand_requirements(question: str) -> str:
         return f"""
 you are a senior programmer below is what your client have asked you to do:
 ---
 {question}
 ---
 
 your current task is to list down all the clarifications you need from the client:
@@ -18,16 +18,17 @@
 * write one questions per line
 * don't write anything other than the questions.
 * use emojis in the question to make them fun.
 * Remember the client is a non technical person so ask question accordingly
 
 Begin!
 """
+
     @staticmethod
-    def plan_project(question:str, clarification:str)->str:
+    def plan_project(question: str, clarification: str) -> str:
         return f"""
 you are a senior programmer below is what your client have asked you to do:
 ---
 {question}
 ---
 here are some clarrification on the requirements
 ---
@@ -39,16 +40,17 @@
 Plan : <your plan here> //tell us a very detailed, verbose plan or thought on how you want to proceed before writing the files  for example which framework you are going to use,dont forget to mention framewark related configuration files. Discuss project architecture so junior developer can understand very easily
 
 As your response will go to an automated parser, things to keep in mind all the time:
 * follow the exact format provided above without fail
 * be detailed so junior developer can understand very easily
 Begin!
 """
+
     @staticmethod
-    def design_folder_structure(question:str,plan:str,clarifications:str)->str:
+    def design_folder_structure(question: str, plan: str, clarifications: str) -> str:
         return f"""
 you are a senior programmer below is what your client have asked you to do:
 ---
 {question}
 ---
 here are some clarrification on the requirements
 ---
@@ -74,34 +76,37 @@
 ```
 As your response will go to an automated parser, things to keep in mind all the time:
 * follow the exact format provided above without fail
 * only write the json nothing else, no expiation, no pretext 
 * do not write the contents of the files that will be done by the next developer
 Begin!
 """
+
     @staticmethod
-    def prioritise_file_list(filelist:List[str])->List[str]:
-        list_string='\n'.join(filelist)
+    def prioritise_file_list(filelist: List[str]) -> List[str]:
+        list_string = '\n'.join(filelist)
         return f"""
 you are a senior programmer. you going to write a api service.
 below are the file list that you are going to complete in future.
 
 reorder them in a way that most suitable based on how one will be dependent on other
 
 {list_string}
 
 As your response will go to an automated parser, things to keep in mind all the time:
 * only write file list in order nothing else
 * do not write any explanation
 Begin!
         """
+
     @staticmethod
-    def write_file(question,clarifications:str,plan:str,files_written:List[List[str]], file_path_to_write:str,file_paths:List[str])->str:
-        file_with_conent="\n\n".join([f"File:{file_path}\nContent:\n{content}" for file_path,content in files_written])
-        all_files_list="\n".join(file_paths)
+    def write_file(question, clarifications: str, plan: str, files_written: List[List[str]], file_path_to_write: str, file_paths: List[str]) -> str:
+        file_with_conent = "\n\n".join(
+            [f"File:{file_path}\nContent:\n{content}" for file_path, content in files_written])
+        all_files_list = "\n".join(file_paths)
         return f"""
 you are a senior programmer below is what your client have asked you to do:
 ---
 {question}
 ---
 here are some clarrification on the requirements
 ---
@@ -123,25 +128,27 @@
 
 now you are about to write content the following file:
 {file_path_to_write}
 
 As your response will go to an automated parser, things to keep in mind all the time:
 * follow the exact format provided above without fail
 * only write the file content, no expiation, no pretext.
+* code should be readable.
 * if the language support, add comments at steps, which expains what you are about to do, dont add comment if comment is not supported by the file type example json file
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
 
 File:{file_path_to_write}
 Content:
 """
 
-    def get_code_feedback(draft:str,question,clarifications:str,plan:str,files_written:List[List[str]], file_path_to_write:str,file_paths:List[str])->str:
-        file_with_conent="\n\n".join([f"File:{file_path}\nContent:\n{content}" for file_path,content in files_written])
-        all_files_list="\n".join(file_paths)
+    def get_code_feedback(draft: str, question, clarifications: str, plan: str, files_written: List[List[str]], file_path_to_write: str, file_paths: List[str]) -> str:
+        file_with_conent = "\n\n".join(
+            [f"File:{file_path}\nContent:\n{content}" for file_path, content in files_written])
+        all_files_list = "\n".join(file_paths)
         return f"""
 you are a senior programmer below is what your client have asked you to do:
 ---
 {question}
 ---
 here are some clarrification on the requirements
 ---
@@ -173,8 +180,31 @@
 
 As your response will go to an automated parser, things to keep in mind all the time:
 * if no refinement is required then just say NONE, and nothing else
 * only write the file content, no expiation, no pretext as this will directly go as code.
 * if the language support, add comments at steps, which expains what you are about to do, dont add comment if comment is not supported by the file type example json file
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
-"""
+"""
+
+    def get_compressed_code(code: str):
+        return f"""
+compress the code below as best as you can, dont rename any data:
+```
+{code}
+```
+As your response will go to an automated parser, things to keep in mind all the time:
+* only output code and nothing else
+* do not rename and content of the code suck as variable names and public function names
+Begin!
+        """
+
+    def get_compressed_text(text: str):
+        return f"""
+compress the content of the text below as best as you can:
+```
+{text}
+```
+As your response will go to an automated parser, things to keep in mind all the time:
+* only respond with the compressed text and nothing else
+Begin!
+        """
```

### Comparing `lazydev-0.0.7/lazydev/modules/utils.py` & `lazydev-0.0.8/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.7/lazydev.egg-info/PKG-INFO` & `lazydev-0.0.8/lazydev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.7/setup.py` & `lazydev-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
```

