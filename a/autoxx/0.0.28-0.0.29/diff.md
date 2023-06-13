# Comparing `tmp/autoxx-0.0.28.tar.gz` & `tmp/autoxx-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.28.tar", max compression
+gzip compressed data, was "autoxx-0.0.29.tar", max compression
```

## Comparing `autoxx-0.0.28.tar` & `autoxx-0.0.29.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.28/README.md
--rw-r--r--   0        0        0     7195 2023-05-27 09:14:52.541250 autoxx-0.0.28/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.28/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.28/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6052 2023-05-27 08:29:33.321541 autoxx-0.0.28/autoxx/config/config.py
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.28/autoxx/requirements.txt
--rw-r--r--   0        0        0      230 2023-05-27 08:43:09.345534 autoxx-0.0.28/autoxx/setup.py
--rw-r--r--   0        0        0     5315 2023-05-27 10:32:18.140459 autoxx-0.0.28/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-05-26 07:39:48.123009 autoxx-0.0.28/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.28/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    11819 2023-05-27 10:32:41.926545 autoxx-0.0.28/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.28/autoxx/utils/base.py
--rw-r--r--   0        0        0     3198 2023-05-27 10:33:03.387959 autoxx-0.0.28/autoxx/utils/llm.py
--rw-r--r--   0        0        0     1905 2023-05-26 07:22:28.056438 autoxx-0.0.28/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.28/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5550 2023-05-27 10:33:16.566378 autoxx-0.0.28/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-05-27 01:02:06.078829 autoxx-0.0.28/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      633 2023-05-27 11:00:15.559904 autoxx-0.0.28/pyproject.toml
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 autoxx-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.29/README.md
+-rw-r--r--   0        0        0     7348 2023-06-08 08:33:03.275169 autoxx-0.0.29/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     1109 2023-05-22 11:10:29.311248 autoxx-0.0.29/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.29/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6052 2023-05-27 08:29:33.321541 autoxx-0.0.29/autoxx/config/config.py
+-rw-r--r--   0        0        0      230 2023-05-27 08:43:09.345534 autoxx-0.0.29/autoxx/setup.py
+-rw-r--r--   0        0        0     7252 2023-06-13 02:10:49.096956 autoxx-0.0.29/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-05-26 07:39:48.123009 autoxx-0.0.29/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.29/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13304 2023-06-12 05:37:24.331952 autoxx-0.0.29/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-05-27 00:53:33.776643 autoxx-0.0.29/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3198 2023-05-27 10:33:03.387959 autoxx-0.0.29/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     1905 2023-05-26 07:22:28.056438 autoxx-0.0.29/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.29/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5550 2023-05-27 10:33:16.566378 autoxx-0.0.29/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-05-27 01:02:06.078829 autoxx-0.0.29/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      659 2023-06-12 07:57:51.854344 autoxx-0.0.29/pyproject.toml
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 autoxx-0.0.29/PKG-INFO
```

### Comparing `autoxx-0.0.28/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.29/autoxx/agent/babyagi/agi.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,18 @@
         )
 
         messages = create_message(prompt)
         response = get_chat_completion(
             messages=messages,
             model="gpt-4"
         )
-
-        new_tasks = json.loads(response)
+        try:
+            new_tasks = json.loads(response)
+        except Exception as e:
+            raise ValueError(f"fail to initial task due to json decocde failed {e}. response={response}")
         task_list = []
         for new_task in new_tasks:
             task_id_counter += 1
             new_task.update({"id": task_id_counter})
             task_list.append(new_task)
         return task_list
```

### Comparing `autoxx-0.0.28/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.29/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/agent/react/agent.py` & `autoxx-0.0.29/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/config/config.py` & `autoxx-0.0.29/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.29/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/tools/web_search/search.py` & `autoxx-0.0.29/autoxx/tools/web_search/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from autoxx.utils.llm import get_chat_completion
 from autoxx.utils.processing_text import split_text
 from autoxx.utils.token_counter import count_message_tokens
 from autoxx.utils.processing_html import extract_hyperlinks, format_hyperlinks
 from autoxx.utils.base import Message
 
 BrowserOptions = ChromeOptions | EdgeOptions | FirefoxOptions | SafariOptions
+MaxChunkTokenSize = 3072
+MaxSummaryTokenSize = 2048
 
 FILE_DIR = Path(__file__).parent
 
 def create_summary_message(chunk: str, question: str) -> Message:
     """Create a message for the chat completion
 
     Args:
@@ -49,14 +51,39 @@
         role="user", 
         content=(
             f'"""{chunk}""" Analyze the above text and extract all information in detail relevant to '
             f'question: "{question}" -- if there is no relevant information, summarize the text in detail.'
         )
     )
 
+def no_relevance(chunk: str, question: str, model: str) -> bool:
+    """Create a message for the chat completion
+
+    Args:
+        chunk (str): The chunk of text to summarize
+        question (str): The question to answer
+
+    Returns:
+        Dict[str, str]: The message to send to the chat completion
+    """
+    messages = [Message(
+        role="user",
+        content=(
+            f'"""{chunk}""" Analyze the above text and determine if it is relevant to the '
+            f'question: "{question}"\nPlease answer only "Yes" or "No"'
+        )
+    )]
+
+    answer = get_chat_completion(
+        model=model,
+        messages=messages,
+    )
+
+    return answer.strip().replace(".", "").lower() == "no"
+
 def scroll_to_percentage(driver: WebDriver, ratio: float) -> None:
     """Scroll to a percentage of the page
 
     Args:
         driver (WebDriver): The webdriver to use
         ratio (float): The percentage to scroll to
 
@@ -173,34 +200,42 @@
         str: The summary of the chunks
     """
     model = "gpt-3.5-turbo"
     logging.debug(f"Memorizing text:\n{'-'*32}\n{text}\n{'-'*32}\n")
     chunks = [
         chunk
         for chunk, _ in (
-            split_text(text, for_model=model)
+            split_text(text, for_model=model, max_chunk_length=MaxChunkTokenSize)
         )
     ]
 
     summaries = []
     scroll_ratio = 1 / len(chunks)
     for i, chunk in enumerate(chunks):
         if driver:
             scroll_to_percentage(driver, scroll_ratio * i)
 
         messages = [create_summary_message(chunk, question)]
         tokens_for_chunk = count_message_tokens(messages)
+
+        if no_relevance(chunk, question, model):
+            logging.info(f"Skipping chunk {i + 1} / {len(chunks)} of length {len(chunk)} characters, or {tokens_for_chunk} tokens, not relevant.")
+            continue
+
         logging.info(
             f"Summarizing {url} chunk {i + 1} / {len(chunks)} of length {len(chunk)} characters, or {tokens_for_chunk} tokens"
         )
 
         summary = get_chat_completion(
             model=model,
             messages=messages,
         )
+
+        logging.info(f"Chunk {i + 1} / {len(chunks)} summary.\n{summary}")
+
         summaries.append(summary)
 
     return summaries
 
 def add_header(driver: WebDriver) -> None:
     """Add a header to the website
 
@@ -225,15 +260,15 @@
 
     Returns:
         None
     """
     driver.quit()
 
 
-def browse_website(url: str, question: str) -> str:
+def browse_website(url: str, question: str) -> str | None:
     """Browse a website and return the answer and links to the user
 
     Args:
         url (str): The url of the website to browse
         question (str): The question asked by the user
 
     Returns:
@@ -243,37 +278,49 @@
         driver, text = scrape_text_with_selenium(url=url)
     except WebDriverException as e:
         # These errors are often quite long and include lots of context.
         # Just grab the first line.
         msg = e.msg.split("\n")[0]
         return f"Error: {msg}"
     add_header(driver)
+
     summaries = summarize_chunks(text=text, question=question, url=url, driver=driver)
-    links = scrape_links_with_selenium(driver, url)
-    summary = "\n".join(summaries)
+    text_gen = "\n".join(summaries)
+    while count_message_tokens([create_summary_message(text_gen, question)]) > MaxSummaryTokenSize:
+       summaries = summarize_chunks(text=text_gen, question=question, url=url, driver=driver)
+       text_gen = "\n".join(summaries)
+       print(text_gen)
+
+    if len(text_gen) == 0:
+        close_browser(driver)
+        return None
 
+    links = scrape_links_with_selenium(driver, url)
     # Limit links to 5
     if len(links) > 5:
         links = links[:5]
     close_browser(driver)
-    return f"Answer gathered from website: {summary}\n\nLinks: {links}"
+    return f"Answer gathered from website: {text_gen}\n\nLinks: {links}"
 
 def web_search(question:str, search_num:Optional[int]=3) -> List[Dict]:
     search_result = google_official_search(query=question, num_results=search_num+3)
     search_summaries = []
 
     index = 0
     for res in search_result:
         print(f"{res['title']} x {res['url']}\n")
         try:
             summary = browse_website(url=res['url'], question=question)
         except Exception as e:
             print(f"Error browsing websit {res['title']} x {res['url']}: {e}")
             continue
 
+        if summary is None:
+            continue
+
         search_summaries.append({
             "relevant_content": summary,
             "title": res['title'],
             "url": res['url']
         })
 
         print(f"{res['title']} x {res['url']} summary: {summary}\n")
```

### Comparing `autoxx-0.0.28/autoxx/utils/base.py` & `autoxx-0.0.29/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/utils/llm.py` & `autoxx-0.0.29/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/utils/openai_models.py` & `autoxx-0.0.29/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/utils/processing_html.py` & `autoxx-0.0.29/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/utils/processing_text.py` & `autoxx-0.0.29/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/autoxx/utils/token_counter.py` & `autoxx-0.0.29/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.28/pyproject.toml` & `autoxx-0.0.29/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.28"
+version = "0.0.29"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,14 +16,15 @@
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
 spacy = ">=3.0.0,<4.0.0"
-llama-index = "^0.6.9"
+llama-index = "^0.6.23"
 google-api-python-client = "^2.86.0"
 pymongo = "^4.3.3"
+transformers = "^4.30.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.28/PKG-INFO` & `autoxx-0.0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.28
+Version: 0.0.29
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
-Requires-Dist: llama-index (>=0.6.9,<0.7.0)
+Requires-Dist: llama-index (>=0.6.23,<0.7.0)
 Requires-Dist: openai (==0.27.6)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
 Requires-Dist: spacy (>=3.0.0,<4.0.0)
 Requires-Dist: tiktoken (==0.3.3)
+Requires-Dist: transformers (>=4.30.1,<5.0.0)
 Requires-Dist: webdriver_manager (==3.8.6)
 Description-Content-Type: text/markdown
```

