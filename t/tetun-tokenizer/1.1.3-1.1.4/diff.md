# Comparing `tmp/tetun_tokenizer-1.1.3.tar.gz` & `tmp/tetun_tokenizer-1.1.4.tar.gz`

## Comparing `tetun_tokenizer-1.1.3.tar` & `tetun_tokenizer-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/.DS_Store
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/Pipfile
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/Pipfile.lock
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/_token
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/tetuntokenizer/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/tetuntokenizer/tetun_patterns.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/tetuntokenizer/tokenizer.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/LICENSE
--rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/README.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/.DS_Store
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/Pipfile
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/Pipfile.lock
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/_token
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/tetuntokenizer/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/tetuntokenizer/tetun_patterns.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/tetuntokenizer/tokenizer.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/LICENSE
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/README.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.4/PKG-INFO
```

### Comparing `tetun_tokenizer-1.1.3/.DS_Store` & `tetun_tokenizer-1.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.3/Pipfile.lock` & `tetun_tokenizer-1.1.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.3/tetuntokenizer/tetun_patterns.py` & `tetun_tokenizer-1.1.4/tetuntokenizer/tetun_patterns.py`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.3/tetuntokenizer/tokenizer.py` & `tetun_tokenizer-1.1.4/tetuntokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.3/LICENSE` & `tetun_tokenizer-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.3/README.md` & `tetun_tokenizer-1.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,142 @@
 ### Tetun Tokenizer
 
-Tetun tokenizer is a Python package used to tokenize an input text into tokens. There are several tokenization techniques we built along with this package as follows:
-1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
-2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
-3. `TetunSentenceTokenizer()`: tokenize the input text by period (.), question mark (?) and exclamation mark (!) delimiters.
-4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
-5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
-6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
+Tetun tokenizer is a Python package used to tokenize an input text into tokens. There are several tokenization techniques we built alongside this package as follows:
+1. `TetunStandardTokenizer`: tokenizes the input text into individual tokens based on word boundaries, punctuations, and special characters.
+2. `TetunWhiteSpaceTokenizer`: tokenizer: breaks the input text into tokens using whitespace as the delimiter.
+3. `TetunSentenceTokenizer`: splits sentences by  its ending delimiters such as period (.), question mark (?), and exclamation mark (!). The period used to represent titles, such as Dr., P.hD., etc., are preserved.
+4. `TetunBlankLineTokenizer`: segments the input text based on the presence of blank lines.
+5. `TetunSimpleTokenizer`: extracts only strings and numbers from the input text while discarding punctuations and special characters.
+6. `TetunWordTokenizer`: extracts only word units from the input text and excludes numbers, punctuation, and special characters.
 
 ### Installation
 
-To install Tetun tokenizer, run the following command in your console:
-
-```
-python3 -m pip install tetun-tokenizer
-```
-
-or simply run:
+With pip:
 
 ```
 pip install tetun-tokenizer
 ```
 
-It also supports `conda` and `pipenv` or similar commands.
-
-
 ### Usage
 
-To use Tetun tokenizer, `from` the `tokenizer` module on the `tetuntokenizer` package, `import` a tokenizer class. Instantiate the imported class and then call a `tokenize` function as follows:
+To use the Tetun tokenizer, from the tokenizer module on the Tetun tokenizer package, import a tokenizer feature/class.
+The examples of its usage are as follows:
 
-1. Using  `TetunStandardTokenizer()` to tokenize the input text.
+1. Using  `TetunStandardTokenizer` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunStandardTokenizer
 
 tetun_tokenizer = TetunStandardTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", '.', "Ha'u", 'iha', '$', '0.25', 'atu', 'fó', 'ba', 'ita', '.']
 ```
 
-2. Using `TetunWhiteSpaceTokenizer()` to tokenize the input text.
+2. Using `TetunWhiteSpaceTokenizer` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWhiteSpaceTokenizer
 
 tetun_tokenizer = TetunWhiteSpaceTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak.", "Ha'u", 'iha', '$0.25', 'atu', 'fó', 'ba', 'ita.']
 ```
 
-3. Using `TetunSentenceTokenizer()` to tokenize the input text.
+3. Using `TetunSentenceTokenizer` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSentenceTokenizer
 
 tetun_tokenizer = TetunSentenceTokenizer()
 
 text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ga? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ga?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
 ```
 
-4. Using `TetunBlankLineTokenizer()` to tokenize the input text.
+4. Using `TetunBlankLineTokenizer` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
 
 tetun_tokenizer = TetunBlankLineTokenizer()
 
 text = """
         Ha'u mak ita-nia maluk di'ak.
         Ha'u iha $0.25 atu fó ba ita.
         """
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["\n            Ha'u mak ita-nia maluk di'ak.\n            Ha'u iha $0.25 atu fó ba ita.\n            "]
 ```
 
-5. Using `TetunSimpleTokenizer()` to tokenize a given text.
+5. Using `TetunSimpleTokenizer` to tokenize a given text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSimpleTokenizer
 
 tetun_tokenizer = TetunSimpleTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', '0.25', 'atu', 'fó', 'ba', 'ita']
 ```
 
-6. Using `TetunWordTokenizer()` to tokenize the input text.
+6. Using `TetunWordTokenizer` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWordTokenizer
 
 tetun_tokenizer = TetunWordTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
 output = tetun_tokenizer.tokenize(text)
 print(output)
 ```
 
-The output will be:
+This will be the output:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', 'atu', 'fó', 'ba', 'ita']
 ```
 
-To print the resulting output in the console, with each element on a new line, you can use `for` loop or simply use `join()` as follows:
+To print the resulting output in the console, with each element on a new line, you can use simply use `join()` as follows:
 
 ```
 print('\n'.join(output))
 ```
 
 The output will be:
 
@@ -184,22 +176,20 @@
 tetun_tokenizer = TetunSimpleTokenizer()
 
 output = '\n'.join(tetun_tokenizer.tokenize(str(lowercase_contents)))
 print(output)
 
 ```
 
-The output will be:
+This is the example of the output:
 
 ```
 ha'u
 orgullu
 dezenvolve
 ha'u-nia
 lian
 tetun 
 ...
 ```
 
-There are a few more ways to read file contents that you can use to achieve the same output.
-
 For the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-tokenizer) for this project.
```

### Comparing `tetun_tokenizer-1.1.3/pyproject.toml` & `tetun_tokenizer-1.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tetun_tokenizer"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Gabriel de Jesus", email="gabriel.dejesus@timornews.tl" },
 ]
 description = "Tetun tokenizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

