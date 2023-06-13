# Comparing `tmp/chat-box-streamlit-0.0.2.tar.gz` & `tmp/chat-box-streamlit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.2.tar", last modified: Tue Jun 13 07:20:44 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.3.tar", last modified: Tue Jun 13 15:32:24 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.2.tar` & `chat-box-streamlit-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/chat_box/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/chat_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-13 07:20:29.000000 chat-box-streamlit-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:32:24.703426 chat-box-streamlit-0.0.3/chat_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/chat_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-13 15:32:11.000000 chat-box-streamlit-0.0.3/setup.py
```

### Comparing `chat-box-streamlit-0.0.2/LICENSE` & `chat-box-streamlit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.2/README.md` & `chat-box-streamlit-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,42 +27,48 @@
 1. Input Box
 ![Input Box](./assets/Input-Box.png)
 To display an input box where users can enter their messages, use the following code:
 ```python
 response = display_chat(component="input", placeholder="This is the input component", rows=1)
 st.write(response)
 ```
+To display with loading:
+```python
+response = display_chat(component="input", loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
+st.write(response)
+```
 
 2. Left and Right Messages
 ![Left and Right Messages](./assets/Message.png)
 You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
 ```
 display_chat(component="message", isLeft=True, message="Hi, I am the left message component")
 display_chat(component="message", isLeft=False, message="Hello, I am the right message component")
 ```
 
 3. Complete Chat Component
 ![Complete Chat Component](./assets/Complete-Chat.png)
-For a complete chat component with multiple messages and scrollable content, use the following code:
+For a complete chat component with multiple messages, loading and scrollable content, use the following code:
 ```python
 response = display_chat(
     message=["What is your name?", "I am the chat component", "How are you different from others?", "I am a complete chat box with scroll"],
     placeholder="Enter your input",
     height=600
 )
 st.write(response)
 ```
+For loading you can pass parameters
+```loading=True and loadingText="Fetching the message..."```
 
 ## Enjoy Conversational UI! 🗣️💬
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
-
 ## How to Contribute 👨‍💻
 
 Thank you for your interest in contributing to our project! We welcome contributions from the community and are grateful for any time and effort you are willing to put in.
 
 1. Fork the repository by clicking the "Fork" button in the top right corner of the page. This will create a copy of the repository in your own GitHub account.
 2. Clone the repository to your local machine using `git clone https://github.com/YOUR_USERNAME/Streamlit-Chatbox.git`.
 3. Make the changes you would like to contribute. Be sure to follow the project's code style guidelines and ensure that your code is properly tested.
```

### Comparing `chat-box-streamlit-0.0.2/chat_box/__init__.py` & `chat-box-streamlit-0.0.3/chat_box/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _chat_box = components.declare_component("chat_box_streamlit", path=build_dir)
 
 
-def display_chat(component="", isLeft=True, message="", placeholder="Enter your input",height=500, rows=1):
-    return _chat_box(component=component, isLeft=isLeft, message=message, placeholder=placeholder, rows=rows, height=height)
+def display_chat(component="", isLeft=True, message="", loading=False, loadingText="Loading...", placeholder="Enter your input",height=500, rows=1):
+    return _chat_box(component=component, isLeft=isLeft, message=message, placeholder=placeholder, loading=loading, loadingText=loadingText, rows=rows, height=height)
 
 
 if not _RELEASE:
     st.set_page_config(page_title="ChatBox Demo", page_icon=":speech_balloon:")
     st.markdown("## Streamlit ChatBox Demo 💬")
     st.markdown("### Input Box")
     response = display_chat(component="input", placeholder="This is input component", rows=1)
+    response = display_chat(component="input", loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
     st.write(response)
     st.markdown("### Left message")
     display_chat(component="message", isLeft=True, message="Hi, i am left message component")
     st.markdown("### Right message")
     display_chat(component="message", isLeft=False, message="Hello, i am right message component")
     st.markdown("### Complete Chat Component")
     response = display_chat(message=["What is your name?", "I am chat component", "How are you different from others ?", "I am a complete chat box with scroll"], placeholder="Enter you input", height=600)
```

### Comparing `chat-box-streamlit-0.0.2/setup.py` & `chat-box-streamlit-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import setuptools
+from pathlib import Path
+
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.2",
+    version="0.0.3",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
-    long_description="ChatBox is a powerful Streamlit component designed to effortlessly display and showcase interactive chat conversations between users. With its seamless integration with Streamlit, ChatBox offers a sleek and intuitive interface for visualizing dynamic dialogues, making it an ideal solution for chatbots, virtual assistants, and interactive conversational applications.",
-    long_description_content_type="text/plain",
-    url="",
+    long_description=Path("README.md").read_text(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.6",
     install_requires=[
         "streamlit >= 0.63",
     ],
```

