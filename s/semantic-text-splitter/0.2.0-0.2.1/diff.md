# Comparing `tmp/semantic_text_splitter-0.2.0.tar.gz` & `tmp/semantic_text_splitter-0.2.1.tar.gz`

## Comparing `semantic_text_splitter-0.2.0.tar` & `semantic_text_splitter-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1025 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/CHANGELOG.md
--rw-r--r--   0     1001      123     4027 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/README.md
--rw-r--r--   0     1001      123      472 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123     9035 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/semantic_text_splitter.pyi
--rw-r--r--   0     1001      123    13390 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123   711396 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/tests/bert-base-cased.json
--rw-r--r--   0     1001      123     1874 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/tests/test_integration.py
--rw-r--r--   0     1001      123    23384 2023-06-12 08:38:13.000000 semantic_text_splitter-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/.gitignore
+-rw-r--r--   0     1001      123     1514 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/CHANGELOG.md
+-rw-r--r--   0     1001      123     4027 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/README.md
+-rw-r--r--   0     1001      123      472 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123    13095 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/semantic_text_splitter.pyi
+-rw-r--r--   0     1001      123    19656 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123   711396 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/tests/bert-base-cased.json
+-rw-r--r--   0     1001      123     2623 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/tests/test_integration.py
+-rw-r--r--   0     1001      123    24957 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.1/PKG-INFO
```

### Comparing `semantic_text_splitter-0.2.0/.gitignore` & `semantic_text_splitter-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.0/CHANGELOG.md` & `semantic_text_splitter-0.2.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 # Changelog
 
+## v0.2.1
+
+### What's New
+
+- Support Open AI Tiktoken tokenizers. So you can now give an OpenAI model name to tokenize the text for when calculating chunk sizes.
+
+```python
+from semantic_text_splitter import TiktokenTextSplitter
+
+# Maximum number of tokens in a chunk
+max_tokens = 1000
+# Optionally can also have the splitter not trim whitespace for you
+splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_tokens)
+```
+
 ## v0.2.0
 
-## What's New
+### What's New
 
 - New `HuggingFaceTextSplitter`, which allows for using Hugging Face's `tokenizers` package to count chunks by tokens with a tokenizer of your choice.
 
 ```python
 from semantic_text_splitter import HuggingFaceTextSplitter
 from tokenizers import Tokenizer
 
@@ -15,15 +32,15 @@
 # Optionally can also have the splitter not trim whitespace for you
 tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
 splitter = HuggingFaceTextSplitter(tokenizer, trim_chunks=False)
 
 chunks = splitter.chunks("your document text", max_characters)
 ```
 
-## Breaking Changes
+### Breaking Changes
 
 - `trim_chunks` now defaults to `True` instead of `False`. For most use cases, this is the desired behavior, especially with chunk ranges.
 
 ## v0.1.4
 
 Fifth time is the charm?
```

### Comparing `semantic_text_splitter-0.2.0/README.md` & `semantic_text_splitter-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # semantic-text-splitter
 
-[![Documentation Status](https://readthedocs.org/projects/semantic-text-splitter/badge/?version=stable)](https://semantic-text-splitter.readthedocs.io/en/stable/?badge=stable) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
+[![Documentation Status](https://readthedocs.org/projects/semantic-text-splitter/badge/?version=stable)](https://semantic-text-splitter.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
 
 Large language models (LLMs) can be used for many tasks, but often have a limited context size that can be smaller than documents you might want to use. To use documents of larger length, you often have to split your text into chunks to fit within this context size.
 
 This crate provides methods for splitting longer pieces of text into smaller chunks, aiming to maximize a desired chunk size, but still splitting at semantically sensible boundaries whenever possible.
 
 ## Get Started
```

### Comparing `semantic_text_splitter-0.2.0/semantic_text_splitter.pyi` & `semantic_text_splitter-0.2.1/semantic_text_splitter.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -183,7 +183,88 @@
                 "full" once it is within the two numbers (inclusive range). So it will only fill
                 up the chunk until the lower range is met.
 
         Returns:
             A list of strings, one for each chunk. If `trim_chunks` was specified in the text
             splitter, then each chunk will already be trimmed as well.
         """
+
+class TiktokenTextSplitter:
+    """Text splitter based on an OpenAI Tiktoken tokenizer. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
+
+    ### By Number of Tokens
+
+    ```python
+    from semantic_text_splitter import TiktokenTextSplitter
+
+    # Maximum number of tokens in a chunk
+    max_tokens = 1000
+    # Optionally can also have the splitter not trim whitespace for you
+    splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+    chunks = splitter.chunks("your document text", max_tokens)
+    ```
+
+    ### Using a Range for Chunk Capacity
+
+    You also have the option of specifying your chunk capacity as a range.
+
+    Once a chunk has reached a length that falls within the range it will be returned.
+
+    It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
+
+    ```python
+    from semantic_text_splitter import TiktokenTextSplitter
+
+    # Optionally can also have the splitter trim whitespace for you
+    splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+    # Maximum number of tokens in a chunk. Will fill up the
+    # chunk until it is somewhere in this range.
+    chunks = splitter.chunks("your document text", chunk_capacity=(200,1000))
+    ```
+
+    Args:
+        model (str): The OpenAI model name you want to retrieve a tokenizer for.
+        trim_chunks (bool, optional): Specify whether chunks should have whitespace trimmed from the
+            beginning and end or not. If False, joining all chunks will return the original
+            string. Defaults to True.
+    """
+
+    def __init__(self, model: str, trim_chunks: bool = True) -> None: ...
+    def chunks(
+        self, text: str, chunk_capacity: Union[int, Tuple[int, int]]
+    ) -> List[str]:
+        """Generate a list of chunks from a given text. Each chunk will be up to the `chunk_capacity`.
+
+        ## Method
+
+        To preserve as much semantic meaning within a chunk as possible, a recursive approach is used, starting at larger semantic units and, if that is too large, breaking it up into the next largest unit. Here is an example of the steps used:
+
+        1. Split the text by a given level
+        2. For each section, does it fit within the chunk size?
+        a. Yes. Merge as many of these neighboring sections into a chunk as possible to maximize chunk length.
+        b. No. Split by the next level and repeat.
+
+        The boundaries used to split the text if using the top-level `split` method, in descending length:
+
+        1. Descending sequence length of newlines. (Newline is `\r\n`, `\n`, or `\r`) Each unique length of consecutive newline sequences is treated as its own semantic level.
+        2. [Unicode Sentence Boundaries](https://www.unicode.org/reports/tr29/#Sentence_Boundaries)
+        3. [Unicode Word Boundaries](https://www.unicode.org/reports/tr29/#Word_Boundaries)
+        4. [Unicode Grapheme Cluster Boundaries](https://www.unicode.org/reports/tr29/#Grapheme_Cluster_Boundaries)
+        5. Characters
+
+        Splitting doesn't occur below the character level, otherwise you could get partial
+        bytes of a char, which may not be a valid unicode str.
+
+        Args:
+            text (str): Text to split.
+            chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+                single int, then chunks will be filled up as much as possible, without going over
+                that number. If a tuple of two integers is provided, a chunk will be considered
+                "full" once it is within the two numbers (inclusive range). So it will only fill
+                up the chunk until the lower range is met.
+
+        Returns:
+            A list of strings, one for each chunk. If `trim_chunks` was specified in the text
+            splitter, then each chunk will already be trimmed as well.
+        """
```

### Comparing `semantic_text_splitter-0.2.0/src/lib.rs` & `semantic_text_splitter-0.2.1/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 // pyo3 uses this
 #![allow(elided_lifetimes_in_paths)]
 
 use std::str::FromStr;
 
 use pyo3::{exceptions::PyException, prelude::*};
 use text_splitter::{Characters, ChunkCapacity, TextSplitter};
+use tiktoken_rs::{get_bpe_from_model, CoreBPE};
 use tokenizers::Tokenizer;
 
 /// Custom chunk capacity for python to make it easier to work
 /// with python arguments
 #[derive(Debug, FromPyObject)]
 enum PyChunkCapacity {
     #[pyo3(transparent, annotation = "int")]
@@ -140,14 +141,60 @@
         text: &'text str,
         chunk_capacity: PyChunkCapacity,
     ) -> Vec<&'text str> {
         self.splitter.chunks(text, chunk_capacity).collect()
     }
 }
 
+/**
+Text splitter based on a Hugging Face Tokenizer. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
+
+### By Number of Tokens
+
+```python
+from semantic_text_splitter import HuggingFaceTextSplitter
+from tokenizers import Tokenizer
+
+# Maximum number of tokens in a chunk
+max_tokens = 1000
+# Optionally can also have the splitter not trim whitespace for you
+tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
+splitter = HuggingFaceTextSplitter(tokenizer, trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_tokens)
+```
+
+### Using a Range for Chunk Capacity
+
+You also have the option of specifying your chunk capacity as a range.
+
+Once a chunk has reached a length that falls within the range it will be returned.
+
+It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
+
+```python
+from semantic_text_splitter import HuggingFaceTextSplitter
+from tokenizers import Tokenizer
+
+# Optionally can also have the splitter trim whitespace for you
+tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
+splitter = HuggingFaceTextSplitter(tokenizer)
+
+# Maximum number of tokens in a chunk. Will fill up the
+# chunk until it is somewhere in this range.
+chunks = splitter.chunks("your document text", chunk_capacity=(200,1000))
+```
+
+Args:
+    tokenizer (Tokenizer): A `tokenizers.Tokenizer` you want to use to count tokens for each
+        chunk.
+    trim_chunks (bool, optional): Specify whether chunks should have whitespace trimmed from the
+        beginning and end or not. If False, joining all chunks will return the original
+        string. Defaults to True.
+ */
 #[pyclass]
 struct HuggingFaceTextSplitter {
     splitter: TextSplitter<Tokenizer>,
 }
 
 #[pymethods]
 impl HuggingFaceTextSplitter {
@@ -247,14 +294,117 @@
         chunk_capacity: PyChunkCapacity,
     ) -> Vec<&'text str> {
         self.splitter.chunks(text, chunk_capacity).collect()
     }
 }
 
 /**
+Text splitter based on an OpenAI Tiktoken tokenizer. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
+
+### By Number of Tokens
+
+```python
+from semantic_text_splitter import TiktokenTextSplitter
+
+# Maximum number of tokens in a chunk
+max_tokens = 1000
+# Optionally can also have the splitter not trim whitespace for you
+splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_tokens)
+```
+
+### Using a Range for Chunk Capacity
+
+You also have the option of specifying your chunk capacity as a range.
+
+Once a chunk has reached a length that falls within the range it will be returned.
+
+It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
+
+```python
+from semantic_text_splitter import TiktokenTextSplitter
+
+# Optionally can also have the splitter trim whitespace for you
+splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+# Maximum number of tokens in a chunk. Will fill up the
+# chunk until it is somewhere in this range.
+chunks = splitter.chunks("your document text", chunk_capacity=(200,1000))
+```
+
+Args:
+    model (str): The OpenAI model name you want to retrieve a tokenizer for.
+    trim_chunks (bool, optional): Specify whether chunks should have whitespace trimmed from the
+        beginning and end or not. If False, joining all chunks will return the original
+        string. Defaults to True.
+ */
+#[pyclass]
+struct TiktokenTextSplitter {
+    splitter: TextSplitter<CoreBPE>,
+}
+
+#[pymethods]
+impl TiktokenTextSplitter {
+    #[new]
+    #[pyo3(signature = (model, trim_chunks=true))]
+    fn new(model: &str, trim_chunks: bool) -> PyResult<Self> {
+        let tokenizer =
+            get_bpe_from_model(model).map_err(|e| PyException::new_err(format!("{e}")))?;
+
+        Ok(Self {
+            splitter: TextSplitter::new(tokenizer).with_trim_chunks(trim_chunks),
+        })
+    }
+
+    /**
+    Generate a list of chunks from a given text. Each chunk will be up to the `chunk_capacity`.
+
+    ## Method
+
+    To preserve as much semantic meaning within a chunk as possible, a recursive approach is used, starting at larger semantic units and, if that is too large, aking it up into the next largest unit. Here is an example of the steps used:
+
+    1. Split the text by a given level
+    2. For each section, does it fit within the chunk size?
+    a. Yes. Merge as many of these neighboring sections into a chunk as possible to maximize chunk length.
+    b. No. Split by the next level and repeat.
+
+    The boundaries used to split the text if using the top-level `split` method, in descending length:
+
+    1. Descending sequence length of newlines. (Newline is `\r\n`, `\n`, or `\r`) Each unique length of consecutive newline sequences is treated as its own antic level.
+    2. [Unicode Sentence Boundaries](https://www.unicode.org/reports/tr29/#Sentence_Boundaries)
+    3. [Unicode Word Boundaries](https://www.unicode.org/reports/tr29/#Word_Boundaries)
+    4. [Unicode Grapheme Cluster Boundaries](https://www.unicode.org/reports/tr29/#Grapheme_Cluster_Boundaries)
+    5. Characters
+
+    Splitting doesn't occur below the character level, otherwise you could get partial
+    bytes of a char, which may not be a valid unicode str.
+
+    Args:
+        text (str): Text to split.
+        chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+            single int, then chunks will be filled up as much as possible, without going over
+            that number. If a tuple of two integers is provided, a chunk will be considered
+            "full" once it is within the two numbers (inclusive range). So it will only fill
+            up the chunk until the lower range is met.
+
+    Returns:
+        A list of strings, one for each chunk. If `trim_chunks` was specified in the text
+        splitter, then each chunk will already be trimmed as well.
+    */
+    fn chunks<'text, 'splitter: 'text>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> Vec<&'text str> {
+        self.splitter.chunks(text, chunk_capacity).collect()
+    }
+}
+
+/**
 [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
 
 Large language models (LLMs) can be used for many tasks, but often have a limited context size that can be smaller than documents you might want to use. To use documents of larger length, you often have to split your text into chunks to fit within this context size.
 
 This crate provides methods for splitting longer pieces of text into smaller chunks, aiming to maximize a desired chunk size, but still splitting at semantically sensible boundaries whenever possible.
 
 ## Get Started
@@ -322,9 +472,10 @@
 
 A big thank you to the unicode-rs team for their [unicode-segmentation](https://crates.io/crates/unicode-segmentation) crate that manages a lot of the complexity of matching the Unicode rules for words and sentences.
 **/
 #[pymodule]
 fn semantic_text_splitter(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<CharacterTextSplitter>()?;
     m.add_class::<HuggingFaceTextSplitter>()?;
+    m.add_class::<TiktokenTextSplitter>()?;
     Ok(())
 }
```

### Comparing `semantic_text_splitter-0.2.0/tests/bert-base-cased.json` & `semantic_text_splitter-0.2.1/tests/bert-base-cased.json`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.0/tests/test_integration.py` & `semantic_text_splitter-0.2.1/tests/test_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import pytest
 from semantic_text_splitter import (
     CharacterTextSplitter,
     HuggingFaceTextSplitter,
+    TiktokenTextSplitter,
 )
 from tokenizers import Tokenizer
 
 
 def test_chunks():
     splitter = CharacterTextSplitter(trim_chunks=False)
     text = "123\n123"
@@ -54,7 +56,33 @@
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
 def test_hugging_face_from_file():
     splitter = HuggingFaceTextSplitter.from_file("tests/bert-base-cased.json")
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
+
+
+def test_tiktoken():
+    splitter = TiktokenTextSplitter(model="gpt-3.5-turbo", trim_chunks=False)
+    text = "123\n123"
+    assert splitter.chunks(text, 2) == ["123\n", "123"]
+
+
+def test_tiktoken_range():
+    splitter = TiktokenTextSplitter(model="gpt-3.5-turbo", trim_chunks=False)
+    text = "123\n123"
+    assert splitter.chunks(text=text, chunk_capacity=(2, 3)) == [
+        "123\n",
+        "123",
+    ]
+
+
+def test_tiktoken_trim():
+    splitter = TiktokenTextSplitter("gpt-3.5-turbo")
+    text = "123\n123"
+    assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
+
+
+def test_tiktoken_model_error():
+    with pytest.raises(Exception):
+        TiktokenTextSplitter("random-model-name")
```

### Comparing `semantic_text_splitter-0.2.0/Cargo.lock` & `semantic_text_splitter-0.2.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "anyhow"
+version = "1.0.71"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
 name = "auto_enums"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "10143e1d6fc660ac7bfc268c6ec2f9699129a3cfbb241eed50393d1562e0a4ce"
 dependencies = [
  "derive_utils",
  "proc-macro2",
@@ -41,20 +47,53 @@
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
+name = "bit-set"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
+dependencies = [
+ "bit-vec",
+]
+
+[[package]]
+name = "bit-vec"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bstr"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
+dependencies = [
+ "memchr",
+ "once_cell",
+ "regex-automata",
+ "serde",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
@@ -81,30 +120,30 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.8.0",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
@@ -191,14 +230,24 @@
 [[package]]
 name = "esaxx-rs"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f748b253ceca9fed5f42f8b5ceb3851e93102199bc25b64b65369f76e5c0a35"
 
 [[package]]
+name = "fancy-regex"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b95f7c0680e4142284cf8b22c14a476e87d61b004a3a0861872b32ef7ead40a2"
+dependencies = [
+ "bit-set",
+ "regex",
+]
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "getrandom"
@@ -269,33 +318,33 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.145"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc86cde3ff845662b8f4ef6cb50ea0e20c524eb3d29ae048287e06a1b3fa6a81"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "macro_rules_attribute"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf0c9b980bf4f3a37fd7b1c066941dd1b1d0152ce6ee6e8fe8c49b9f6810d862"
 dependencies = [
@@ -313,23 +362,14 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
@@ -416,23 +456,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
@@ -447,31 +487,31 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.9.0",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -588,62 +628,75 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick 1.0.2",
  "memchr",
  "regex-syntax 0.7.2",
 ]
 
 [[package]]
+name = "regex-automata"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+
+[[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "semantic-text-splitter"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "pyo3",
  "text-splitter",
+ "tiktoken-rs",
  "tokenizers",
 ]
 
 [[package]]
 name = "serde"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -682,15 +735,15 @@
 
 [[package]]
 name = "spm_precompiled"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5851699c4033c63636f7ea4cf7b7c1f1bf06d0cc03cfb42e711de5a5c46cf326"
 dependencies = [
- "base64",
+ "base64 0.13.1",
  "nom",
  "serde",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "strsim"
@@ -733,14 +786,15 @@
 checksum = "70fb0eba57256b96e1438c8542a99277bddd8c3774f8cfc629bf2f6fe13c09c1"
 dependencies = [
  "auto_enums",
  "either",
  "itertools 0.10.5",
  "once_cell",
  "regex",
+ "tiktoken-rs",
  "tokenizers",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
@@ -758,14 +812,29 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
+name = "tiktoken-rs"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ba161c549e2c0686f35f5d920e63fad5cafba2c28ad2caceaf07e5d9fa6e8c4"
+dependencies = [
+ "anyhow",
+ "base64 0.21.2",
+ "bstr",
+ "fancy-regex",
+ "lazy_static",
+ "parking_lot",
+ "rustc-hash",
+]
+
+[[package]]
 name = "tokenizers"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cf49017523bf0bc01c9966f172c5f120bbb7b96cccd1708772dd42e767fb9f5"
 dependencies = [
  "aho-corasick 0.7.20",
  "derive_builder",
@@ -828,71 +897,62 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `semantic_text_splitter-0.2.0/PKG-INFO` & `semantic_text_splitter-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-text-splitter
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: black ; extra == 'test'
 Requires-Dist: tokenizers ; extra == 'test'
 Requires-Dist: pdoc ; extra == 'docs'
@@ -17,15 +17,15 @@
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/benbrandt/text-splitter
 
 # semantic-text-splitter
 
-[![Documentation Status](https://readthedocs.org/projects/semantic-text-splitter/badge/?version=stable)](https://semantic-text-splitter.readthedocs.io/en/stable/?badge=stable) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
+[![Documentation Status](https://readthedocs.org/projects/semantic-text-splitter/badge/?version=stable)](https://semantic-text-splitter.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/crates/l/text-splitter)](https://github.com/benbrandt/text-splitter/blob/main/LICENSE.txt)
 
 Large language models (LLMs) can be used for many tasks, but often have a limited context size that can be smaller than documents you might want to use. To use documents of larger length, you often have to split your text into chunks to fit within this context size.
 
 This crate provides methods for splitting longer pieces of text into smaller chunks, aiming to maximize a desired chunk size, but still splitting at semantically sensible boundaries whenever possible.
 
 ## Get Started
```

