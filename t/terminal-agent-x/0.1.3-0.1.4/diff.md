# Comparing `tmp/terminal-agent-x-0.1.3.tar.gz` & `tmp/terminal-agent-x-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal-agent-x-0.1.3.tar", last modified: Wed Jun  7 07:03:16 2023, max compression
+gzip compressed data, was "terminal-agent-x-0.1.4.tar", last modified: Tue Jun 13 04:41:26 2023, max compression
```

## Comparing `terminal-agent-x-0.1.3.tar` & `terminal-agent-x-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.3/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3749 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2936 2023-06-07 07:01:35.000000 terminal-agent-x-0.1.3/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      915 2023-06-07 06:39:01.000000 terminal-agent-x-0.1.3/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/terminal_agent_x/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.3/terminal_agent_x/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5639 2023-06-07 06:56:18.000000 terminal-agent-x-0.1.3/terminal_agent_x/tax.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3749 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-07 07:03:16.000000 terminal-agent-x-0.1.3/terminal_agent_x.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-07 07:03:16.186520 terminal-agent-x-0.1.3/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.3/tests/test.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.4/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4128 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3246 2023-06-13 04:40:45.000000 terminal-agent-x-0.1.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      976 2023-06-13 04:37:46.000000 terminal-agent-x-0.1.4/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.167598 terminal-agent-x-0.1.4/terminal_agent_x/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.4/terminal_agent_x/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6973 2023-06-13 04:17:58.000000 terminal-agent-x-0.1.4/terminal_agent_x/tax.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4128 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.4/tests/test.py
```

### Comparing `terminal-agent-x-0.1.3/LICENSE` & `terminal-agent-x-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal-agent-x-0.1.3/PKG-INFO` & `terminal-agent-x-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.3
+Version: 0.1.4
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
+Project-URL: Wiki, https://github.com/LyuLumos/Terminal-Agent-X/wiki
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -53,34 +54,34 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax [-h] [--key KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
 
 Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
-  prompt         Prompt
+  prompt                Prompt
 
 options:
-  -h, --help     show this help message and exit
-  --key KEY      Your key for OpenAI//Claude, only for one-time request
-  --model MODEL  Model name. You can use all OpenAI models.
-  --file FILE    Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
-  --url URL      URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.
-  --show_all     Show all contents in the response
+  -h, --help            show this help message and exit
+  -k KEY, --key KEY     Your key for OpenAI/Claude.
+  --model MODEL         Model name. Choose from gpt-3.5/4s, claude or DALLE.
+  -i INPUT, --input INPUT
+                        Input file. If specified, the prompt will be read from the file.
+  -o OUTPUT, --output OUTPUT
+                        Output file. If specified, the response will be saved to the file.
+  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be
+                        accessd under GFW.
+  --show_all            Show all contents in the response.
 ```
 
-## Support
-
-I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
-
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
@@ -106,20 +107,28 @@
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
 </details>
 
 <details>
 <summary>0.1.2</summary>
 
-- [WIP]Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
 - Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
 - Add a timeout function.
 - Fix: C++ code block prefix.
 </details>
 
 <details>
 <summary>0.1.3</summary>
 
 - Fix: code block prefix bug (tax will act maybe a little faster).
 - Modify: simplify the code.
 - Test: test for multi-process. Now you can use tax more efficiently in terminal.
 </details>
+
+<details>
+<summary>0.1.4</summary>
+
+- Feat: Add support for reading prompt from file.
+- Feat: Add support for OpenAI DALL·E.
+- Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
+</details>
```

### Comparing `terminal-agent-x-0.1.3/README.md` & `terminal-agent-x-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -34,34 +34,34 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax [-h] [--key KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
 
 Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
-  prompt         Prompt
+  prompt                Prompt
 
 options:
-  -h, --help     show this help message and exit
-  --key KEY      Your key for OpenAI//Claude, only for one-time request
-  --model MODEL  Model name. You can use all OpenAI models.
-  --file FILE    Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
-  --url URL      URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.
-  --show_all     Show all contents in the response
+  -h, --help            show this help message and exit
+  -k KEY, --key KEY     Your key for OpenAI/Claude.
+  --model MODEL         Model name. Choose from gpt-3.5/4s, claude or DALLE.
+  -i INPUT, --input INPUT
+                        Input file. If specified, the prompt will be read from the file.
+  -o OUTPUT, --output OUTPUT
+                        Output file. If specified, the response will be saved to the file.
+  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be
+                        accessd under GFW.
+  --show_all            Show all contents in the response.
 ```
 
-## Support
-
-I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
-
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
@@ -87,20 +87,28 @@
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
 </details>
 
 <details>
 <summary>0.1.2</summary>
 
-- [WIP]Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
 - Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
 - Add a timeout function.
 - Fix: C++ code block prefix.
 </details>
 
 <details>
 <summary>0.1.3</summary>
 
 - Fix: code block prefix bug (tax will act maybe a little faster).
 - Modify: simplify the code.
 - Test: test for multi-process. Now you can use tax more efficiently in terminal.
+</details>
+
+<details>
+<summary>0.1.4</summary>
+
+- Feat: Add support for reading prompt from file.
+- Feat: Add support for OpenAI DALL·E.
+- Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
 </details>
```

### Comparing `terminal-agent-x-0.1.3/pyproject.toml` & `terminal-agent-x-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal-agent-x"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="LyuLumos", email="lyujiuyang0@gmail.com" },
 ]
+
 description = "A terminal agent for terminal users."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 
     "Programming Language :: Python :: 3",
@@ -25,7 +26,8 @@
 
 [project.scripts]
 tax = "terminal_agent_x.tax:main"
 
 [project.urls]
 "Homepage" = "https://github.com/LyuLumos/Terminal-Agent-X"
 "Bug Tracker" = "https://github.com/LyuLumos/Terminal-Agent-X/issues"
+"Wiki" = "https://github.com/LyuLumos/Terminal-Agent-X/wiki"
```

### Comparing `terminal-agent-x-0.1.3/terminal_agent_x/tax.py` & `terminal-agent-x-0.1.4/terminal_agent_x/tax.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import signal
 import subprocess
 import os
 import argparse
 import re
 import json
+from typing import Tuple
 import psutil
 
 
-def check_terminal():
+def check_terminal() -> str:
     # check the terminal type
     parent_process_name = psutil.Process(os.getppid()).name()
     if parent_process_name in ['pwsh', 'powershell', 'powershell.exe']:
         return 'powershell'
     if parent_process_name in ['cmd', 'cmd.exe']:
         return 'cmd'
 
 
-def run_command_with_timeout(command, timeout):
+def run_command_with_timeout(command: str, timeout: int) -> Tuple[str, str]:
     p = subprocess.Popen(command, stdout=subprocess.PIPE,
                          stderr=subprocess.PIPE, shell=True)
     try:
         stdout, stderr = p.communicate(timeout=timeout)
         return stdout.decode('utf-8', 'ignore'), stderr.decode('utf-8', 'ignore')
     except subprocess.TimeoutExpired as timeout_e:
         p.terminate()
@@ -28,106 +29,130 @@
             kill_process_tree(p.pid)
         else:
             os.killpg(os.getpgid(p.pid), signal.SIGTERM)
         raise subprocess.TimeoutExpired(
             p.args, timeout, output=stdout, stderr=stderr) from timeout_e
 
 
-def kill_process_tree(pid):
+def kill_process_tree(pid: int) -> None:
     try:
         parent = psutil.Process(pid)
         children = parent.children(recursive=True)
         for child in children:
             child.kill()
         parent.kill()
     except psutil.NoSuchProcess:
         pass
 
 
-def fetch_code(openai_key, model, prompt, url):
-    urls = {
-        'openai_gfw': 'https://api.lyulumos.space/v1/chat/completions',
-        'openai': 'https://api.openai.com/v1/chat/completions',
-        'claude': 'https://claude-api.lyulumos.space/v1/chat/completions'
-    }
-    url = urls[url] if url in urls else url
-    headers = [
-        f"Authorization: Bearer {openai_key}",
-        "Content-Type: application/json"
-    ]
-    terminal_headers = [
-        f"Authorization='Bearer {openai_key}'",
-        "'Content-Type'='application/json'"
-    ]
-    data = f'{{"model": "{model}","messages": [{{"role": "user", "content": "{prompt}"}}]}}'
-
+def fetch_code(openai_key: str, model: str, prompt: str, url_option: str) -> str:
+    url, headers, terminal_headers, data = req_info(openai_key, model, prompt, url_option)
     if os.name == 'nt':  # Windows
         if check_terminal() == 'powershell':
             wt_command = f'Invoke-WebRequest -Uri "{url}" -Method POST -Headers @{{{terminal_headers[0]};{terminal_headers[1]}}} -Body \'{data}\' -UseBasicParsing | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty choices | Select-Object -First 1 | Select-Object -ExpandProperty message | Select-Object -ExpandProperty content'
             print(
                 f'Current version does not fully support Windows PowerShell. Please copy command below and paste:\n\n{wt_command}')
             return ''
         # Windows cmd
         headers = [h.replace('"', '\\"') for h in headers]
         data = data.replace('"', '\\"')
         command = f'curl -s "{url}" -H "{headers[0]}" -H "{headers[1]}" -d "{data}"'
+        command = f'{command} --ipv4' if model == 'claude' else command  # The claude API worker is not IPv6 compatible
     else:  # Linux
         command = f"curl -s --location '{url}' --header '{headers[0]}' --header '{headers[1]}' --data '{data}'"
     # print(command)
 
     try:
         res, err = run_command_with_timeout(command, 60)
+        # print(res, err)
         # res = os.popen(command).read().encode('utf-8').decode('utf-8', 'ignore')
+        if model.lower() == 'dalle':
+            return json.loads(res)['data'][0]['url']
         return json.loads(res)['choices'][0]['message']['content']
     except KeyError:
         assert False, 'This is most likely due to poor internet or invalid key. Please retry.'
     except json.decoder.JSONDecodeError:
         assert False, 'This URL may be invalid or the response cannot be parsed'
 
 
-def find_code(text):
+def req_info(openai_key: str, model: str, prompt: str, url_option: str) -> Tuple[str, str, str, str]:
+    headers = [
+        f"Authorization: Bearer {openai_key}",
+        "Content-Type: application/json"
+    ]
+    terminal_headers = [
+        f"Authorization='Bearer {openai_key}'",
+        "'Content-Type'='application/json'"
+    ]
+
+    urls = {
+        'openai_gfw': 'https://api.lyulumos.space/v1/chat/completions',
+        'openai': 'https://api.openai.com/v1/chat/completions',
+        'claude': 'https://claude-api.lyulumos.space/v1/chat/completions'
+    }
+    url_option = 'claude' if model == 'claude' else url_option
+    url = urls[url_option] if url_option in urls else url_option
+
+    if model.lower() == 'dalle':
+        url = 'https://api.lyulumos.space/v1/images/generations' if url_option == 'openai_gfw' else 'https://api.openai.com/v1/images/generations'
+        data = f'{{"prompt": "{prompt}"}}'
+    else:
+        data = f'{{"model": "{model}","messages": [{{"role": "user", "content": "{prompt}"}}]}}'
+    return url, headers, terminal_headers, data
+
+
+def find_code(text: str) -> str:
     pattern = r"```(.*?)```"
     match = re.search(pattern, text, re.DOTALL)
     if match:
         codes = match.group(0)
         first_n = codes.find('\n')
         return codes[first_n+1:-3].strip()  # without ``` pairs
     return None
 
 
-def main():
+def load_file(path: str) -> str:
+    with open(path, 'r', encoding='utf-8') as f:
+        text = f.read()
+    return text.replace('\\', '\\\\').replace('"', '\\"').replace('\n', '\\n')
+
+
+def main() -> None:
     parser = argparse.ArgumentParser(
         description='Tax: A terminal agent using OpenAI/Claude API')
     parser.add_argument("prompt", nargs='+', type=str, help="Prompt")
     parser.add_argument('-k', '--key', type=str,
                         help='Your key for OpenAI/Claude.')
     parser.add_argument('--model', type=str,
-                        default='gpt-3.5-turbo', help='Model name. You can use all OpenAI models.')
-    parser.add_argument(
-        '--file', type=str, help='Output file. If specified, the output will be written to this file. Tax will act like ChatGPT.')
+                        default='gpt-3.5-turbo', help='Model name. Choose from gpt-3.5/4s, claude or DALLE.')
+    parser.add_argument('-i', '--input', type=str,
+                        help='Input file. If specified, the prompt will be read from the file.')
+    parser.add_argument('-o', '--output', type=str,
+                        help='Output file. If specified, the response will be saved to the file.')
     parser.add_argument('--url', type=str, default='openai_gfw',
                         help="URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.")
     parser.add_argument('--show_all', action='store_true',
                         help='Show all contents in the response.')
     args = parser.parse_args()
 
     prompt = ' '.join(args.prompt)
-    prompt = f'{prompt}. Answer me with markdown'
+    prompt = f'{prompt}\\n{load_file(args.input)}' if args.input else prompt
+
     key = args.key or os.environ.get('OpenAI_KEY')
     if not key:
         assert False, 'Error: OpenAI key not found. Please specify it in system environment variables or pass it as an argument.'
 
     # res = get_model_response(openai_key, args.model, prompt)
     res = fetch_code(key, args.model, prompt, args.url)
 
-    if args.file:
-        with open(args.file, 'w', encoding='utf-8') as f:
+    if args.output:
+        with open(args.output, 'w', encoding='utf-8') as f:
             f.write(res)
         f.close()
-    elif args.show_all:
+    elif args.show_all or args.model.lower() == 'dalle':
         print(res)
     else:
         first_code = find_code(res)
         if not first_code:
             print(res)
         else:
             print(first_code + '\n')
```

### Comparing `terminal-agent-x-0.1.3/terminal_agent_x.egg-info/PKG-INFO` & `terminal-agent-x-0.1.4/terminal_agent_x.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.3
+Version: 0.1.4
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
+Project-URL: Wiki, https://github.com/LyuLumos/Terminal-Agent-X/wiki
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -53,34 +54,34 @@
 
 ```
 tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
-usage: tax [-h] [--key KEY] [--model MODEL] [--file FILE] [--url URL] [--show_all] prompt [prompt ...]
+usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
 
 Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
-  prompt         Prompt
+  prompt                Prompt
 
 options:
-  -h, --help     show this help message and exit
-  --key KEY      Your key for OpenAI//Claude, only for one-time request
-  --model MODEL  Model name. You can use all OpenAI models.
-  --file FILE    Output file. If specified, the output will be written to this file. Tax will act like ChatGPT
-  --url URL      URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.
-  --show_all     Show all contents in the response
+  -h, --help            show this help message and exit
+  -k KEY, --key KEY     Your key for OpenAI/Claude.
+  --model MODEL         Model name. Choose from gpt-3.5/4s, claude or DALLE.
+  -i INPUT, --input INPUT
+                        Input file. If specified, the prompt will be read from the file.
+  -o OUTPUT, --output OUTPUT
+                        Output file. If specified, the response will be saved to the file.
+  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be
+                        accessd under GFW.
+  --show_all            Show all contents in the response.
 ```
 
-## Support
-
-I have tested on Windows 10/11(cmd) and Ubuntu 22.04, it should work on other platforms.
-
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
@@ -106,20 +107,28 @@
 - Add `--url` option for users not under GFW.
 - Add support for Windows Powershell
 </details>
 
 <details>
 <summary>0.1.2</summary>
 
-- [WIP]Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
+- Add Anthropic Claude API Support. Thanks to [jtsang4/claude-to-chatgpt](https://github.com/jtsang4/claude-to-chatgpt).
 - Add Support for Chinese on Linux and Windows. (also add a temporary solution for VSCode Terminal on Windows).
 - Add a timeout function.
 - Fix: C++ code block prefix.
 </details>
 
 <details>
 <summary>0.1.3</summary>
 
 - Fix: code block prefix bug (tax will act maybe a little faster).
 - Modify: simplify the code.
 - Test: test for multi-process. Now you can use tax more efficiently in terminal.
 </details>
+
+<details>
+<summary>0.1.4</summary>
+
+- Feat: Add support for reading prompt from file.
+- Feat: Add support for OpenAI DALL·E.
+- Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
+</details>
```

