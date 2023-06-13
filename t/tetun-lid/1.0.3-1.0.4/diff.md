# Comparing `tmp/tetun_lid-1.0.3.tar.gz` & `tmp/tetun_lid-1.0.4.tar.gz`

## Comparing `tetun_lid-1.0.3.tar` & `tetun_lid-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/.DS_Store
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/Pipfile
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/Pipfile.lock
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/tetunlid/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/tetunlid/lid.py
--rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/tetunlid/model/tetun_lid_model.pkl
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/LICENSE
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/.DS_Store
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/Pipfile
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/Pipfile.lock
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/tetunlid/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/tetunlid/lid.py
+-rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/tetunlid/model/tetun_lid_model.pkl
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 tetun_lid-1.0.4/PKG-INFO
```

### Comparing `tetun_lid-1.0.3/.DS_Store` & `tetun_lid-1.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.3/Pipfile.lock` & `tetun_lid-1.0.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.3/tetunlid/lid.py` & `tetun_lid-1.0.4/tetunlid/lid.py`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.3/tetunlid/model/tetun_lid_model.pkl` & `tetun_lid-1.0.4/tetunlid/model/tetun_lid_model.pkl`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.3/LICENSE` & `tetun_lid-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.3/README.md` & `tetun_lid-1.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,195 +1,201 @@
+Metadata-Version: 2.1
+Name: tetun_lid
+Version: 1.0.4
+Summary: Tetun Language Identification Model
+Project-URL: repository, https://github.com/borulilitimornews/tetun-lid
+Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 ### Tetun LID
 Tetun Language Identification (Tetun LID) model is a machine learning model that automatically identifies the language of a given text. It was specifically designed to recognize four languages commonly spoken in Timor-Leste: Tetun, Portuguese, English, and Indonesian.
 
-
-Using a combination of cutting-edge algorithms and sophisticated linguistic features, Tetun LID was trained on a large corpus of textual data to accurately recognize the characteristic of each language and the linguistic patterns. Its ability to accurately identify multiple languages makes it a valuable tool for anyone working with multilingual text data in Timor-Leste in the natural language processing (NLP) and information retrieval (IR) fields.
-
 ### Installation
 
-To install Tetun LID, run the following command in your console:
+With pip:
 
 ```
 pip install tetun-lid
 ```
 
-### Dependecies
+### Dependencies
 
-Tetun LID depends on the following packages:
+The Tetun LID model depends on the following packages:
 
 * joblib
 * scikit-learn
 
-To install the dependencies packages, run these commands in your console:
+Install the dependencies packages with pip:
 
 ```
 pip install joblib
 pip install scikit-learn
 ```
 
 ### Usage
 
-To use Tetun LID, from the `tetunlid` package, import the `lid` module, and then call a function.
+To use the Tetun LID model, from the `tetunlid` package, import the `lid` module, and then call the respective functions. The examples of its usage are as follows:
 
-1. In case you want to `predict the language` of an input text, use the `predict_language()` function.
+1. To predict the language of an input text, use the `predict_language()` function.
 
 ```python
 
 from tetunlid import lid
 
-input_text = "Sé mak hamriik iha ne'ebá?"
+input_text = "Sé mak toba iha ne'ebá?"
 output = lid.predict_language(input_text)
 
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 Tetun
 ```
 
-2. If you want to `print the details` of why it was being predicted to Tetun, you can use the `predict_detail()` function.
+2. To print the details of the Probability of being predicted to Tetun use the `predict_detail()` function.
 
 ```python
 
 from tetunlid import lid
 
-input_list_of_str = ["Sé mak hamriik iha ne'ebá?"]
+input_list_of_str = ["Sé mak toba iha ne'ebá?"]
 output_detail = lid.predict_detail(input_list_of_str)
 print('\n'.join(output_detail))
 ```
 
-The output will be:
+This will be the outpu:
 
 ```
-Input text: "Sé mak hamriik iha ne'ebá?"
+Input text: "Sé mak toba iha ne'ebá?"
 Probability:
-        English: 0.0007
-        Indonesian: 0.0007
-        Portuguese: 0.0006
-        Tetun: 0.9980
-Thus, the input text is "Tetun" with a confidence level of 99.80%.
+        English: 0.0010
+        Indonesian: 0.0014
+        Portuguese: 0.0082
+        Tetun: 0.9967
+Thus, the input text is "Tetun" with a confidence level of 99.67%.
 ```
 
-`Note`: the input parameter and the output of `predict_detail()` is a `List[str]` or a list of strings, and therefore to print the output result in the console, we can to use `for` loop or `join()` as in the example above to print the result.
+`Note`: The output of `predict_detail()` is a list of strings and therefore to print the its result in the console, use `for` loop or `join()` as in the previous example.
 
-3. You can use a mixed corpus containing multiple languages as the input. Observe the following example:
+3. We can feed a mixed corpus containing multiple languages into the LID model as the input list. Observe the following example:
 
 ```python
 from tetunlid import lid
 
-multiple_langs = ["Ha'u ema baibain", "I am quite busy",
-                  "Kamu malas sekali", "Vou sair daqui"]
+multiple_langs = ["Ha'u ema baibain", "I am not available",
+                  "Apa kabar kawan?", "Estou a estudar"]
 
 output = [(ml, lid.predict_language(ml)) for ml in multiple_langs]
 print(output)
 ```
 
-The output will be:
+This will be the outpu:
 
 ```
-[("Ha'u ema baibain", 'Tetun'), ('I am quite busy', 'English'), ('Kamu malas sekali', 'Indonesian'), ('Vou sair daqui', 'Portuguese')]
+[("Ha'u ema baibain", 'Tetun'), ('I am not available', 'English'), ('Apa kabar kawan?', 'Indonesian'), ('Estou a estudar', 'Portuguese')]
 ```
 
-You can use `for` or any similar way to print the output in lines in the console as follows:
+You can use print the output in the console as follows:
 
 ```python
 from tetunlid import lid
 
-input_texts = ["Ha'u ema baibain", "I am quite busy",
-               "Kamu malas sekali", "Vou sair daqui"]
+input_texts = ["Ha'u ema baibain", "I am not available",
+                "Apa kabar kawan?", "Estou a estudar"]
 
 for input_text in input_texts:
     lang = lid.predict_language(input_text)
     print(f"{input_text} ({lang})")
 ```
 
-The output will be:
+This will be the outpu:
 
 ```
 Ha'u ema baibain (Tetun)
-I am quite busy (English)
-Kamu malas sekali (Indonesian)
-Vou sair daqui (Portuguese)
+I am not available (English)
+Apa kabar kawan? (Indonesian)
+Estou a estudar (Portuguese)
 ```
 
-If you want to print the details of each input, you can use the same function as illustrated above. Here you go:
+To print the details of each input, use the same function as previously explained. Here is the example:
 
 ```python
 
 from tetunlid import lid
 
-input_texts = ["Ha'u ema baibain", "I am quite busy",
-               "Kamu malas sekali", "Vou sair daqui"]
+input_texts = ["Ha'u ema baibain", "I am not available",
+                "Apa kabar kawan?", "Estou a estudar"]
 
 output_multiple_detail = lid.predict_detail(input_texts)
 print('\n'.join(output_multiple_detail))
 ```
 
-The output will be:
+This will be the outpu:
 
 ```
 Input text: "Ha'u ema baibain"
 Probability:
-        English: 0.0027
-        Indonesian: 0.0028
-        Portuguese: 0.0024
-        Tetun: 0.9920
-Thus, the input text is "Tetun" with a confidence level of 99.20%.
+        English: 0.0032
+        Indonesian: 0.0032
+        Portuguese: 0.0028
+        Tetun: 0.9907
+Thus, the input text is "Tetun" with a confidence level of 99.07%.
 
-
-Input text: "I am quite busy"
+Input text: "I am not available"
 Probability:
-        English: 0.9974
-        Indonesian: 0.0007
-        Portuguese: 0.0015
-        Tetun: 0.0004
-Thus, the input text is "English" with a confidence level of 99.74%.
-
+        English: 0.9999
+        Indonesian: 0.00001
+        Portuguese: 0.00001
+        Tetun: 0.00001
+Thus, the input text is "English" with a confidence level of 99.99%.
 
-Input text: "Kamu malas sekali"
+Input text: "Apa kabar kawan?"
 Probability:
-        English: 0.0001
-        Indonesian: 0.9997
-        Portuguese: 0.0001
-        Tetun: 0.0001
-Thus, the input text is "Indonesian" with a confidence level of 99.97%.
-
-
+        English: 0.0011
+        Indonesian: 0.9961
+        Portuguese: 0.0015
+        Tetun: 0.0184
+Thus, the input text is "Indonesian" with a confidence level of 99.61%.
 
-Input text: "Vou sair daqui"
+Input text: "Estou a estudar"
 Probability:
-        English: 0.0034
-        Indonesian: 0.0030
-        Portuguese: 0.9912
-        Tetun: 0.0023
-Thus, the input text is "Portuguese" with a confidence level of 99.12%.
+        English: 0.0003
+        Indonesian: 0.002
+        Portuguese: 0.9810
+        Tetun: 0.0184
+Thus, the input text is "Portuguese" with a confidence level of 98.10%.
 ```
 
-4. You can filter only Tetun text from a mixed corpus containing multiple languages using the `predict_language()` function.
+4. We can filter only Tetun text from a mixed corpus containing multiple languages using the `predict_language()` function.
 
 ```python
 from tetunlid import lid
 
 
-input_texts = ["Ha'u ema baibain", "I am quite busy",
-               "Kamu malas sekali", "Vou sair daqui"]
+input_texts = ["Ha'u ema baibain", "I am not available",
+                "Apa kabar kawan?", "Estou a estudar"]
 
 output = [text for text in input_texts if lid.predict_language(text) == 'Tetun']
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["Ha'u ema baibain"]
 ```
 
-5. You can also use Tetun LID to predict a text from a file containing various languages or texts extracted from the web. Here is an example:
+5. We can also use Tetun LID to predict a text from a file containing various languages or texts extracted from the web. Here is an example:
 
 ```python
 from pathlib import Path
 from tetunlid import lid
 
 
 file_path = Path("myfile/example.txt")
@@ -200,16 +206,14 @@
 except FileNotFoundError:
     print(f"File not found at: {file_path}")
 
 output = [(content, lid.predict_language(content)) for content in contents]
 print(output)
 ```
 
-There are a few more ways to read file contents that you can use to achieve the same output.
-
-For the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-lid) for this project.
-
 ### Additional notes
 
-1. Please follow the instruction carefully and try to understand how it works. All the dependencies need to be installed properly.
+1. All the dependencies need to be installed accordingly before using the model.
 2. If you encountered an `AttributeError: 'list' object has no attribute 'predict_proba'`, you might have some issues while installing the package. Please send me an email, and I will guide you on how to handle the error.
-3. Please make sure that you use the latest version of Tetun LID. To get the latest version, run this command in your console: `pip install --upgrade tetun-lid`.
+3. Please make sure that you use the latest version of Tetun LID by running this command in your console: `pip install --upgrade tetun-lid`.
+
+To get the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-lid) for this project.
```

### Comparing `tetun_lid-1.0.3/pyproject.toml` & `tetun_lid-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tetun_lid"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Gabriel de Jesus", email="gabriel.dejesus@timornews.tl" },
 ]
 description = "Tetun Language Identification Model"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

