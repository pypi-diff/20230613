# Comparing `tmp/UnlimitedGPT-0.1.5.5.tar.gz` & `tmp/UnlimitedGPT-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.5.5.tar", last modified: Sun Jun 11 13:30:26 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.6.tar", last modified: Mon Jun 12 22:29:11 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.5.5.tar` & `UnlimitedGPT-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4431 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.936950 UnlimitedGPT-0.1.5.5/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    30852 2023-06-11 13:28:32.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2485 2023-06-11 11:27:16.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4431 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-11 13:30:26.000000 UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-11 13:30:26.940950 UnlimitedGPT-0.1.5.5/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1775 2023-06-11 13:28:43.000000 UnlimitedGPT-0.1.5.5/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.307382 UnlimitedGPT-0.1.6/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-12 22:29:11.303382 UnlimitedGPT-0.1.6/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.299382 UnlimitedGPT-0.1.6/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    38856 2023-06-12 22:15:15.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      271 2023-06-12 22:06:37.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.303382 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2559 2023-06-12 21:33:12.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1274 2023-06-12 19:02:03.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      116 2023-06-12 15:20:24.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13597 2023-06-12 21:54:34.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.303382 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-12 22:29:11.307382 UnlimitedGPT-0.1.6/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-12 21:57:38.000000 UnlimitedGPT-0.1.6/setup.py
```

### Comparing `UnlimitedGPT-0.1.5.5/PKG-INFO` & `UnlimitedGPT-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.5.5
+Version: 0.1.6
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -31,15 +31,15 @@
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Sxvxgeness.svg?style=social)](https://twitter.com/Sxvxgeness)
 
 UnlimitedGPT is a Python library for using the ChatGPT website as an alternative API to the OpenAI paid API.
 
 UnlimitedGPT makes it easy to send messages and receive responses. UnlimitedGPT can also do a wide range of things such as getting the user data, getting the session data, clearing all conversations, resetting the current conversation, switching themes, switching accounts, and logging out from the session.
 
-![Preview](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/docs/assets/preview.png)
+![Preview](https://raw.githubusercontent.com/Sxvxgee/UnlimitedGPT/main/docs/assets/preview.png)
 
 ## Compatibility
 UnlimitedGPT works on Windows, Linux and macOS. It also works on Google Colab and other headless  linux servers. UnlimitedGPT requires Python 3.8 or later.
 
 ## Features
 
 -   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`
```

### Comparing `UnlimitedGPT-0.1.5.5/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.6/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,280 +1,291 @@
 import re
-from typing import Optional, Literal
-from time import sleep, time
-from threading import Thread
-from platform import system
-from os import environ
 from json import loads
-from logging import getLogger, DEBUG, Formatter, StreamHandler
+from logging import DEBUG, Formatter, StreamHandler, getLogger
+from os import environ
+from platform import system
+from threading import Thread
+from time import sleep, time
+from typing import Literal, Optional
 from weakref import finalize
 
 from markdownify import markdownify
+from selenium.common.exceptions import (
+    NoSuchElementException,
+    StaleElementReferenceException,
+    TimeoutException,
+)
+from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
-from selenium.common.exceptions import TimeoutException, NoSuchElementException, StaleElementReferenceException
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.action_chains import ActionChains
 from undetected_chromedriver import ChromeOptions
 
-from .internal.driver import ChatGPTDriver
 from .internal.chatgpt_data import ChatGPTVariables as CGPTV
-from .internal.objects import ChatGPTResponse, User, SessionData
+from .internal.driver import ChatGPTDriver
 from .internal.exceptions import InvalidConversationID
+from .internal.objects import ChatGPTResponse, Conversations, SessionData, SharedConversations, User, Accounts
+
 
 class ChatGPT:
     """
     A class for interacting with ChatGPT.
 
     Args:
     ----------
         session_token (str): The session token for authentication.
         conversation_id (str, optional): The conversation ID. Defaults to ''.
         proxy (Optional[str], optional): The proxy server URL. Defaults to None.
         disable_moderation (bool, optional): Whether to disable moderation. Defaults to True.
         verbose (bool, optional): Whether to enable verbose logging. Defaults to False.
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
         chrome_args (list, optional): Additional arguments for the Chrome browser. Defaults to [].
-    
+
     Raises:
     ----------
         InvalidConversationID: If the conversation ID is invalid.
         ValueError: If the session token is not provided.
         ValueError: If the proxy is invalid.
     """
 
     def __init__(
         self,
         session_token: str,
-        conversation_id: str = '',
+        conversation_id: str = "",
         proxy: Optional[str] = None,
         disable_moderation: bool = False,
         verbose: bool = False,
         headless: bool = False,
         chrome_args: list = [],
     ) -> None:
         self._session_token = session_token
         self._conversation_id = conversation_id
         self._proxy = proxy
         self._disable_moderation = disable_moderation
         self._headless = headless
         self._chrome_args = chrome_args
         self._clicked_buttons = False
+        self._history_and_training_enabled = True
         self._init_logger(verbose)
 
         if self._proxy and not re.findall(
-            r'(https?|socks(4|5)?):\/\/.+:\d{1,5}', self._proxy # type: ignore
+            r"(https?|socks(4|5)?):\/\/.+:\d{1,5}", self._proxy  # type: ignore
         ):
-            raise ValueError('Invalid proxy format')
+            raise ValueError("Invalid proxy format")
 
         self._init_browser()
         finalize(self, self.__del__)
 
     def __del__(self) -> None:
         """
         Close the browser and display.
         """
         self._is_active = False
-        if hasattr(self, 'driver'):
-            self.logger.debug('Closing browser...')
+        if hasattr(self, "driver"):
+            self.logger.debug("Closing browser...")
             self.driver.quit()
-        if hasattr(self, 'display'):
-            self.logger.debug('Closing display...')
+        if hasattr(self, "display"):
+            self.logger.debug("Closing display...")
             self.display.stop()
 
     def _get_out_of_menu(self) -> None:
         """
         Get out of any menu present.
         """
         for i in range(5):
             # First escape click is to remove the options menu
             # Second escape click is to get out of the settings menu
             # The rest are just to be safe
-            self.driver.find_element(By.TAG_NAME, 'body').send_keys(Keys.ESCAPE)
+            self.driver.find_element(By.TAG_NAME, "body").send_keys(Keys.ESCAPE)
 
     def _init_logger(self, verbose: bool) -> None:
         """
         Initialize the logger.
 
         Args:
         ----------
             verbose (bool): Whether to enable verbose logging.
         """
-        self.logger = getLogger('pyChatGPT')
+        self.logger = getLogger("pyChatGPT")
         self.logger.setLevel(DEBUG)
         if verbose:
-            formatter = Formatter('[%(funcName)s] %(message)s')
+            formatter = Formatter("[%(funcName)s] %(message)s")
             stream_handler = StreamHandler()
             stream_handler.setFormatter(formatter)
             self.logger.addHandler(stream_handler)
-    
+
     def _init_browser(self) -> None:
         """
         Initialize the browser.
 
         Raises:
         ----------
             ValueError: If the proxy is invalid.
             ValueError: If the Chrome installation is not found.
             ValueError: If the virtual display is not found.
 
         Notes:
         ----------
             If the system is Linux and the DISPLAY environment variable is not set, a virtual display will be started.
         """
-        if system() == 'Linux' and 'DISPLAY' not in environ:
-            self.logger.debug('Starting virtual display...')
+        if system() == "Linux" and "DISPLAY" not in environ:
+            self.logger.debug("Starting virtual display...")
             try:
                 from pyvirtualdisplay.display import Display
+
                 self.display = Display()
                 self.display.start()
             except ModuleNotFoundError:
-                raise ValueError('Please install PyVirtualDisplay to start a virtual display by running `pip install PyVirtualDisplay`')
+                raise ValueError(
+                    "Please install PyVirtualDisplay to start a virtual display by running `pip install PyVirtualDisplay`"
+                )
             except FileNotFoundError as e:
-                if 'No such file or directory: \'Xvfb\'' in str(e):
-                    raise ValueError('Please install Xvfb to start a virtual display by running `sudo apt install xvfb`')
+                if "No such file or directory: 'Xvfb'" in str(e):
+                    raise ValueError(
+                        "Please install Xvfb to start a virtual display by running `sudo apt install xvfb`"
+                    )
                 raise e
 
-        self.logger.debug('Initializing browser...')
-        
+        self.logger.debug("Initializing browser...")
+
         options = ChromeOptions()
-        options.add_argument('--window-size=1024,768')
-        options.add_argument('--disable-popup-blocking')
+        options.add_argument("--window-size=1024,768")
+        options.add_argument("--disable-popup-blocking")
         if self._proxy:
-            options.add_argument(f'--proxy-server={self._proxy}')
+            options.add_argument(f"--proxy-server={self._proxy}")
         for arg in self._chrome_args:
             options.add_argument(arg)
         try:
             self.driver = ChatGPTDriver(options=options, headless=self._headless)
         except TypeError as e:
-            if str(e) == 'expected str, bytes or os.PathLike object, not NoneType':
-                raise ValueError('Chrome installation not found')
+            if str(e) == "expected str, bytes or os.PathLike object, not NoneType":
+                raise ValueError("Chrome installation not found")
             raise e
 
         if self._session_token:
-            self.logger.debug('Restoring session_token...')
+            self.logger.debug("Restoring session_token...")
             self.driver.execute_cdp_cmd(
-                'Network.setCookie',
+                "Network.setCookie",
                 {
-                    'domain': 'chat.openai.com',
-                    'path': '/',
-                    'name': '__Secure-next-auth.session-token',
-                    'value': self._session_token,
-                    'httpOnly': True,
-                    'secure': True,
+                    "domain": "chat.openai.com",
+                    "path": "/",
+                    "name": "__Secure-next-auth.session-token",
+                    "value": self._session_token,
+                    "httpOnly": True,
+                    "secure": True,
                 },
             )
 
         if self._disable_moderation:
-            self.logger.debug('Blocking moderation...')
+            self.logger.debug("Blocking moderation...")
             self.driver.execute_cdp_cmd(
-                'Network.setBlockedURLs',
-                {'urls': ['https://chat.openai.com/backend-api/moderations']},
+                "Network.setBlockedURLs",
+                {"urls": ["https://chat.openai.com/backend-api/moderations"]},
             )
 
-        self.logger.debug('Ensuring Cloudflare cookies...')
+        self.logger.debug("Ensuring Cloudflare cookies...")
         self._ensure_cf()
 
-        self.logger.debug('Opening chat page...')
-        self.driver.get(f'{CGPTV.chat_url}/{self._conversation_id}')
+        self.logger.debug("Opening chat page...")
+        self.driver.get(f"{CGPTV.chat_url}/{self._conversation_id}")
         self._check_blocking_elements()
 
         self._is_active = True
         Thread(target=self._keep_alive, daemon=True).start()
 
     def _keep_alive(self) -> None:
         """
         Keep the session alive by updating the local storage.
         """
         while self._is_active:
-            self.logger.debug('Updating session...')
+            self.logger.debug("Updating session...")
             payload = (
                 '{"event":"session","data":{"trigger":"getSession"},"timestamp":%d}'
                 % int(time())
             )
             try:
                 self.driver.execute_script(
                     'window.localStorage.setItem("nextauth.message", arguments[0])',
                     payload,
                 )
             except Exception as e:
-                self.logger.debug(f'Failed to update session: {str(e)}')
+                self.logger.debug(f"Failed to update session: {str(e)}")
             sleep(60)
 
     def _check_blocking_elements(self) -> None:
         """
         Check for blocking elements and dismiss them.
         """
-        self.logger.debug('Looking for blocking elements...')
+        self.logger.debug("Looking for blocking elements...")
         try:
             intro = WebDriverWait(self.driver, 5).until(
                 EC.presence_of_element_located(CGPTV.intro)
             )
-            self.logger.debug('Dismissing intro...')
-            self.driver.execute_script('arguments[0].remove()', intro)
-        except TimeoutException: # type: ignore
+            self.logger.debug("Dismissing intro...")
+            self.driver.execute_script("arguments[0].remove()", intro)
+        except TimeoutException:  # type: ignore
             pass
 
         alerts = self.driver.find_elements(*CGPTV.alert)
         if alerts:
-            if 'unable to load conversation' in alerts[0].text.lower():
+            if "unable to load conversation" in alerts[0].text.lower():
                 raise InvalidConversationID(alerts[0].text)
-            self.logger.debug('Dismissing alert...')
-            self.driver.execute_script('arguments[0].remove()', alerts[0])
+            self.logger.debug("Dismissing alert...")
+            self.driver.execute_script("arguments[0].remove()", alerts[0])
 
         if not self._clicked_buttons:
             for button in CGPTV.info_buttons:
-                self.driver.safe_click(button, timeout = 60)
+                self.driver.safe_click(button, timeout=60)
             self._clicked_buttons = True
 
     def _ensure_cf(self, retry: int = 3) -> None:
         """
         Ensure Cloudflare cookies are set.
 
         Args:
         ----------
             retry (int, optional): Number of retries. Defaults to 3.
 
         Raises:
         ----------
             TimeoutException: If the Cloudflare challenge fails.
         """
-        self.logger.debug('Opening new tab...')
+        self.logger.debug("Opening new tab...")
         original_window = self.driver.current_window_handle
-        self.driver.switch_to.new_window('tab')
+        self.driver.switch_to.new_window("tab")
 
-        self.logger.debug('Getting Cloudflare challenge...')
-        self.driver.get('https://chat.openai.com/api/auth/session')
+        self.logger.debug("Getting Cloudflare challenge...")
+        self.driver.get("https://chat.openai.com/api/auth/session")
         try:
             WebDriverWait(self.driver, 10).until_not(
                 EC.presence_of_element_located(CGPTV.cf_challenge_form)
             )
-        except TimeoutException: # type: ignore
-            self.logger.debug(f'Cloudflare challenge failed, retrying {retry}...')
+        except TimeoutException:  # type: ignore
+            self.logger.debug(f"Cloudflare challenge failed, retrying {retry}...")
             if retry > 0:
-                self.logger.debug('Closing tab...')
+                self.logger.debug("Closing tab...")
                 self.driver.close()
                 self.driver.switch_to.window(original_window)
                 return self._ensure_cf(retry - 1)
-            raise ValueError('Cloudflare challenge failed')
-        self.logger.debug('Cloudflare challenge passed')
+            raise ValueError("Cloudflare challenge failed")
+        self.logger.debug("Cloudflare challenge passed")
 
-        self.logger.debug('Validating authorization...')
+        self.logger.debug("Validating authorization...")
         response = self.driver.page_source
-        if response[0] != '{':
-            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        if response[0] != "{":
+            response = self.driver.find_element(By.TAG_NAME, "pre").text
         response = loads(response)
         if (not response) or (
-            'error' in response and response['error'] == 'RefreshAccessTokenError'
+            "error" in response and response["error"] == "RefreshAccessTokenError"
         ):
-            raise ValueError('Invalid session token')
-        self.logger.debug('Authorization is valid')
+            raise ValueError("Invalid session token")
+        self.logger.debug("Authorization is valid")
 
-        self.logger.debug('Closing tab...')
+        self.logger.debug("Closing tab...")
         self.driver.close()
         self.driver.switch_to.window(original_window)
 
     def _continue_generating(self, timeout: int) -> Optional[str]:
         """
         Continue generating the response.
 
@@ -282,65 +293,259 @@
         ----------
             timeout (int): Time to wait for the message to continue regenerating before timing out.
 
         Returns:
         ----------
             Optional[str]: The newly generated response.
         """
-        self.logger.debug('Continuing generating...')
+        self.logger.debug("Continuing generating...")
         # Click "Continue generating" button
         continue_response_clicked = self.driver.safe_click(
-            CGPTV.continue_regenerating, timeout = 5
+            CGPTV.continue_regenerating, timeout=5
         )
         if not continue_response_clicked:
-            self.logger.debug('Could not click continue regenerating button')
+            self.logger.debug("Could not click continue regenerating button")
             return None
 
         # Get the response, same way as send_message without the part of sending the message
-        self.logger.debug('Waiting for completion...')
+        self.logger.debug("Waiting for completion...")
         try:
             WebDriverWait(self.driver, timeout).until_not(
                 EC.presence_of_element_located(CGPTV.streaming)
             )
         except:
-            self.logger.debug('Could not continue generating')
+            self.logger.debug("Could not continue generating")
             return None
 
-        self.logger.debug('Getting response...')
+        self.logger.debug("Getting response...")
         responses = self.driver.find_elements(*CGPTV.big_response)
         if responses:
             response = responses[-1]
-            if 'text-red' in response.get_attribute('class'):
-                self.logger.debug('Response is an error')
+            if "text-red" in response.get_attribute("class"):
+                self.logger.debug("Response is an error")
                 return None
         response = self.driver.find_elements(*CGPTV.small_response)
         try:
             response = response[-1]
         except IndexError:
-            self.logger.debug('Response not found, resetting conversation...')
+            self.logger.debug("Response not found, resetting conversation...")
             self.reset_conversation()
             return None
-        
-        content = markdownify(
-            response.get_attribute('innerHTML'),
-            escape_asterisks=False,
-            escape_underscores=False,
-
-        ).replace(
-            'Copy code`', '`'
-        ).rstrip("\n")
-        
-        self.logger.debug('Continued regenerating the response')
+
+        content = (
+            markdownify(
+                response.get_attribute("innerHTML"),
+                escape_asterisks=False,
+                escape_underscores=False,
+            )
+            .replace("Copy code`", "`")
+            .rstrip("\n")
+        )
+
+        self.logger.debug("Continued regenerating the response")
         return content
 
+    def _get_conversation_id(self):
+        """
+        Gets the conversation ID.
+        """
+        logs_raw = self.driver.get_log("performance")
+
+        conv_response_id = next(
+            log_["params"]["requestId"]
+            for log_ in reversed([loads(lr["message"])["message"] for lr in logs_raw])
+            if
+            log_["method"] == "Network.responseReceived"
+            # and json
+            and "json" in log_["params"]["response"]["mimeType"]
+            # and status 200
+            and log_["params"]["response"]["status"] == 200
+            # and conversations
+            and "/backend-api/conversations" in log_["params"]["response"]["url"]
+        )
+
+        ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": conv_response_id})
+
+        self._conversation_id = loads(ret["body"])["items"][0]["id"]
+
+        self.logger.debug(f"Conversation id: {self._conversation_id}")
+
+    def _open_shared_conversations_popup(self):
+        """
+        Opens the shared conversations popup.
+        """
+        self.logger.debug("Opening shared conversations popup...")
+        try:
+            menu_button_clicked = self.driver.safe_click(CGPTV.menu_button)
+            if not menu_button_clicked:
+                self.logger.debug("Could not click menu button")
+                return self._get_out_of_menu()
+
+            self.logger.debug("Clicked menu button")
+
+            settings_button_clicked = self.driver.safe_click(CGPTV.menu_settings)
+            if not settings_button_clicked:
+                self.logger.debug("Could not click settings button")
+                return self._get_out_of_menu()
+
+            self.logger.debug("Clicked settings button")
+
+            # Click "Data controls" button
+            data_controls_clicked = self.driver.safe_click(
+                CGPTV.data_controls, timeout=60
+            )
+            if not data_controls_clicked:
+                self.logger.debug("Could not click data controls button")
+                return self._get_out_of_menu()
+            
+            self.logger.debug("Clicked data controls button")
+
+            # Click the "Manage" button for Shared Links
+            shared_links_manage_clicked = self.driver.safe_click(
+                CGPTV.shared_links_manage, timeout=60
+            )
+            if not shared_links_manage_clicked:
+                self.logger.debug("Could not click shared links manage button")
+                return self._get_out_of_menu()
+
+            self.logger.debug("Clicked shared links manage button")
+        except:
+            self.logger.debug("Could not open shared conversations popup")
+
+        return self._get_out_of_menu()
+
+    def get_user_data(self):
+        """
+        Gets the user data.
+
+        Returns
+        ---------
+            Accounts: a list of the accounts.
+        """
+        self.logger.debug("Getting user data...")
+
+        logs_raw = self.driver.get_log("performance")
+
+        data = next(
+            log_["params"]["requestId"]
+            for log_ in reversed([loads(lr["message"])["message"] for lr in logs_raw])
+            if (
+                log_["method"] == "Network.responseReceived"
+                and "json" in log_["params"]["response"]["mimeType"]
+                and log_["params"]["response"]["status"] == 200
+                and "backend-api/accounts/check/" in log_["params"]["response"]["url"]
+            )
+        )
+
+        ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": data})
+
+        response_data = loads(ret["body"])
+
+        return Accounts(response_data)
+
+    def get_conversations(self) -> Conversations:
+        """
+        Get a list of conversations.
+
+        Returns:
+        ----------
+            Conversations: A list of conversations.
+        """
+        self.logger.debug("Getting conversations...")
+        logs_raw = self.driver.get_log("performance")
+
+        data = next(
+            log_["params"]["requestId"]
+            for log_ in reversed([loads(lr["message"])["message"] for lr in logs_raw])
+            if (
+                log_["method"] == "Network.responseReceived"
+                and "json" in log_["params"]["response"]["mimeType"]
+                and log_["params"]["response"]["status"] == 200
+                and "/backend-api/conversations" in log_["params"]["response"]["url"]
+            )
+        )
+
+        self.logger.debug("Found conversations")
+
+        ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": data})
+
+        response_data = loads(ret["body"])
+
+        return Conversations(
+            response_data["items"],
+            response_data["has_missing_conversations"],
+            response_data["limit"],
+            response_data["offset"],
+            response_data["total"]
+        )
+
+    def get_shared_conversations(self, timeout: float = 5) -> SharedConversations:
+        """
+        Get a list of shared conversations.
+
+        Args:
+        ----------
+            timeout (float, optional): Time to wait for the message to continue regenerating before timing out.
+
+        Returns:
+        ----------
+            SharedConversations: A list of shared conversations, or None if unsuccessful.
+        """
+        self.logger.debug("Getting shared conversations...")
+        logs_raw = self.driver.get_log("performance")
+
+        start_time = time()
+        end_time = start_time + timeout
+        opened_popup = False
+
+        while time() < end_time:
+            try:
+                data = next(
+                    log_["params"]["requestId"]
+                    for log_ in reversed([loads(lr["message"])["message"] for lr in logs_raw])
+                    if (
+                        log_["method"] == "Network.responseReceived"
+                        and "json" in log_["params"]["response"]["mimeType"]
+                        and log_["params"]["response"]["status"] == 200
+                        and "/backend-api/shared_conversations" in log_["params"]["response"]["url"]
+                    )
+                )
+                break  # Found data, exit the loop
+            except StopIteration:
+                if not opened_popup:
+                    self.logger.debug("Could not find conversations, opening shared conversations popup...")
+                    self._open_shared_conversations_popup()
+                    opened_popup = True
+                else:
+                    self.logger.debug("Could not find conversations, refreshing logs...")
+                logs_raw = self.driver.get_log("performance")  # Refresh logs
+
+        else:
+            self.logger.debug("Timeout reached, failed to get shared conversations")
+            return None
+
+        self.logger.debug("Found shared conversations")
+
+        ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": data})
+
+        response_data = loads(ret["body"])
+
+        return SharedConversations(
+            response_data["items"],
+            response_data["has_missing_conversations"],
+            response_data["limit"],
+            response_data["offset"],
+            response_data["total"]
+        )
+
     def send_message(
         self,
         message: str,
         timeout: int = 240,
-        input_mode: Literal['INSTANT', 'SLOW'] = "INSTANT",
+        input_mode: Literal["INSTANT", "SLOW"] = "INSTANT",
         input_delay: float = 0.1,
         continue_generating: bool = True,
     ) -> ChatGPTResponse:
         """
         Send a message to ChatGPT.
 
         Args:
@@ -357,79 +562,88 @@
 
         Raises:
         ----------
             TimeoutException: If the message fails to send.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
-        self.logger.debug(f'Sending message with mode {input_mode}{f" with {input_delay} delay" if input_mode == "SLOW" else ""}...')
+        self.logger.debug(
+            f'Sending message with mode {input_mode}{f" with {input_delay} delay" if input_mode == "SLOW" else ""}...'
+        )
 
         textbox = WebDriverWait(self.driver, 60).until(
             EC.element_to_be_clickable(CGPTV.textbox)
         )
-        if input_mode == 'INSTANT':
-            self.driver.execute_script("arguments[0].value = arguments[1];", textbox, message)
+        if input_mode == "INSTANT":
+            self.driver.execute_script(
+                "arguments[0].value = arguments[1];", textbox, message
+            )
         else:
             for char in message:
                 try:
                     textbox.send_keys(char)
                 except StaleElementReferenceException:
                     textbox = WebDriverWait(self.driver, 60).until(
                         EC.element_to_be_clickable(CGPTV.textbox)
                     )
                     textbox.send_keys(char)
 
-        textbox.send_keys('a')
+        textbox.send_keys("a")
         textbox.send_keys(Keys.BACKSPACE)
-        
+
         textbox.send_keys(Keys.ENTER)
 
-        self.logger.debug('Waiting for completion...')
+        self.logger.debug("Waiting for completion...")
         WebDriverWait(self.driver, timeout).until_not(
             EC.presence_of_element_located(CGPTV.streaming)
         )
 
-        self.logger.debug('Getting response...')
+        self.logger.debug("Getting response...")
         responses = self.driver.find_elements(*CGPTV.big_response)
         if responses:
             response = responses[-1]
-            if 'text-red' in response.get_attribute('class'):
-                self.logger.debug('Response is an error')
+            if "text-red" in response.get_attribute("class"):
+                self.logger.debug("Response is an error")
                 raise ValueError(response.text)
         response = self.driver.find_elements(*CGPTV.small_response)
         try:
             response = response[-1]
         except IndexError:
-            self.logger.debug('Response not found, resetting conversation...')
+            self.logger.debug("Response not found, resetting conversation...")
             self.reset_conversation()
-            raise ValueError('Response not found')
+            raise ValueError("Response not found")
 
-        content = markdownify(
-            response.get_attribute('innerHTML'),
-            escape_asterisks=False,
-            escape_underscores=False,
-
-        ).replace(
-            'Copy code`', '`'
-        ).rstrip("\n")
+        content = (
+            markdownify(
+                response.get_attribute("innerHTML"),
+                escape_asterisks=False,
+                escape_underscores=False,
+            )
+            .replace("Copy code`", "`")
+            .rstrip("\n")
+        )
 
         if continue_generating:
-            continuation = self._continue_generating(timeout = timeout)
+            continuation = self._continue_generating(timeout=timeout)
             if continuation:
                 content = continuation
 
-        self.logger.debug(f'Message sent')
+        self.logger.debug(f"Message sent")
+
+        if not self._conversation_id:
+            self.logger.debug(f"New conversation, cathing the id.")
+            self._get_conversation_id()
 
         return ChatGPTResponse(content, self._conversation_id)
 
     def regenerate_response(
         self,
         message_timeout: int = 240,
         click_timeout: int = 20,
-        continue_generating: bool = True
+        continue_generating: bool = True,
     ) -> ChatGPTResponse:
         """
         Regenerate the response.
 
         Args:
         ----------
             message_timeout (int, optional): Time to wait for the message to regenerate before timing out. Defaults to 240.
@@ -443,176 +657,188 @@
         Raises:
         ----------
             TimeoutException: If the message fails to send.
             TimeoutException: If the click fails to succeed.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
-        self.logger.debug('Regenerating response...')
+        self.logger.debug("Regenerating response...")
 
         # Click "Regenerate response" button
         regenerate_response_clicked = self.driver.safe_click(
-            CGPTV.regenerate_response, timeout = click_timeout
+            CGPTV.regenerate_response, timeout=click_timeout
         )
         if not regenerate_response_clicked:
-            self.logger.debug('Could not click regenerate response button')
-            raise TimeoutException('Could not click regenerate response button')
+            self.logger.debug("Could not click regenerate response button")
+            raise TimeoutException("Could not click regenerate response button")
 
         # Get the response, same way as send_message without the part of sending the message
-        self.logger.debug('Waiting for completion...')
+        self.logger.debug("Waiting for completion...")
         WebDriverWait(self.driver, message_timeout).until_not(
             EC.presence_of_element_located(CGPTV.streaming)
         )
 
-        self.logger.debug('Getting response...')
+        self.logger.debug("Getting response...")
         responses = self.driver.find_elements(*CGPTV.big_response)
         if responses:
             response = responses[-1]
-            if 'text-red' in response.get_attribute('class'):
-                self.logger.debug('Response is an error')
+            if "text-red" in response.get_attribute("class"):
+                self.logger.debug("Response is an error")
                 raise ValueError(response.text)
         response = self.driver.find_elements(*CGPTV.small_response)
         try:
             response = response[-1]
         except IndexError:
-            self.logger.debug('Response not found, resetting conversation...')
+            self.logger.debug("Response not found, resetting conversation...")
             self.reset_conversation()
-            raise ValueError('Response not found')
+            raise ValueError("Response not found")
 
-        content = markdownify(
-            response.get_attribute('innerHTML'),
-            escape_asterisks=False,
-            escape_underscores=False,
-
-        ).replace(
-            'Copy code`', '`'
-        ).rstrip("\n")
+        content = (
+            markdownify(
+                response.get_attribute("innerHTML"),
+                escape_asterisks=False,
+                escape_underscores=False,
+            )
+            .replace("Copy code`", "`")
+            .rstrip("\n")
+        )
 
         if continue_generating:
-            continuation = self._continue_generating(timeout = message_timeout)
+            continuation = self._continue_generating(timeout=message_timeout)
             if continuation:
                 content = continuation
-        
-        self.logger.debug('Regenerated response')
+
+        self.logger.debug("Regenerated response")
         return ChatGPTResponse(content, self._conversation_id)
 
     def reset_conversation(self) -> None:
         """
         Resets the conversation.
         """
-        if not self.driver.current_url.startswith('https://chat.openai.com/'):
-            return self.logger.debug('Current URL is not chat page, skipping reset')
+        if not self.driver.current_url.startswith("https://chat.openai.com/"):
+            return self.logger.debug("Current URL is not chat page, skipping reset")
 
-        self.logger.debug('Resetting conversation...')
-        clicked = self.driver.safe_click(CGPTV.new_chat, timeout = 60)
+        self.logger.debug("Resetting conversation...")
+        button = CGPTV.new_chat if self._history_and_training_enabled else CGPTV.clear_chat
+        clicked = self.driver.safe_click(button, timeout=60)
         if not clicked:
-            self.logger.debug('New chat button not found')
+            self.logger.debug(f"{button[1]} button not found")
             return self._get_out_of_menu()
-        self.logger.debug('Conversation reset')
+        self.logger.debug("Conversation reset")
 
     def clear_conversations(self) -> None:
         """
         Clears all conversations.
         """
-        self.logger.debug('Clearing all conversations...')
+        self.logger.debug("Clearing all conversations...")
         try:
-            menu_button_clicked = self.driver.safe_click(CGPTV.menu_button, timeout = 60)
+            menu_button_clicked = self.driver.safe_click(CGPTV.menu_button, timeout=60)
             if not menu_button_clicked:
-                self.logger.debug('Could not click menu button')
+                self.logger.debug("Could not click menu button")
                 return self._get_out_of_menu()
-            self.logger.debug('Clicked menu button')
-            
+            self.logger.debug("Clicked menu button")
+
             clear_conversations_button_clicked = self.driver.safe_click(
-                CGPTV.menu_clear_conversations, timeout = 60
+                CGPTV.menu_clear_conversations, timeout=60
             )
             if not clear_conversations_button_clicked:
-                self.logger.debug('Could not click clear conversations button')
+                self.logger.debug("Could not click clear conversations button")
                 return self._get_out_of_menu()
-            self.logger.debug('Clicked clear conversations button')
-            
+            self.logger.debug("Clicked clear conversations button")
+
             confirm_clear_button_clicked = self.driver.safe_click(
-                CGPTV.menu_confirm_clear_conversations, timeout = 60
+                CGPTV.menu_confirm_clear_conversations, timeout=60
             )
             if not confirm_clear_button_clicked:
-                self.logger.debug('Could not click confirm clear conversations button')
+                self.logger.debug("Could not click confirm clear conversations button")
                 return self._get_out_of_menu()
-            self.logger.debug('Clicked confirm clear conversations button')
+            self.logger.debug("Clicked confirm clear conversations button")
 
-            self.logger.debug('Cleared all conversations')
+            self.logger.debug("Cleared all conversations")
             self._get_out_of_menu()
-        except NoSuchElementException:
-            self.logger.debug('Could not find menu buttons')
+        except NoSuchElementException: # type: ignore
+            self.logger.debug("Could not find menu buttons")
             return self._get_out_of_menu()
 
-    def switch_theme(self, theme: Literal['LIGHT', 'DARK', 'OPPOSITE', 'SYSTEM']) -> None:
+    def switch_theme(
+        self, theme: Literal["LIGHT", "DARK", "OPPOSITE", "SYSTEM"]
+    ) -> None:
         """
         Switch the theme.
 
         Args:
         ----------
             theme (Literal['LIGHT', 'DARK', 'OPPOSITE']): The theme to switch to.
 
         Notes:
         ----------
             - `LIGHT`: Light theme.
             - `DARK`: Dark theme.
             - `OPPOSITE`: Switch to the opposite theme.
             - `SYSTEM`: Switch to the system theme.
         """
-        self.logger.debug(f'Switching theme to {theme}...')
+        self.logger.debug(f"Switching theme to {theme}...")
         try:
             menu_button_clicked = self.driver.safe_click(CGPTV.menu_button)
             if not menu_button_clicked:
-                self.logger.debug('Could not click menu button')
+                self.logger.debug("Could not click menu button")
                 return self._get_out_of_menu()
-            self.logger.debug('Clicked menu button')
-            
+            self.logger.debug("Clicked menu button")
+
             settings_button_clicked = self.driver.safe_click(CGPTV.menu_settings)
             if not settings_button_clicked:
-                self.logger.debug('Could not click settings button')
+                self.logger.debug("Could not click settings button")
                 return self._get_out_of_menu()
-            self.logger.debug('Clicked settings button')
-            
-            current_theme_value = self.driver.find_element(*CGPTV.outer_html).get_attribute('class')
-            current_theme = 'LIGHT' if 'light' in current_theme_value else 'DARK'
+            self.logger.debug("Clicked settings button")
+
+            current_theme_value = self.driver.find_element(
+                *CGPTV.outer_html
+            ).get_attribute("class")
+            current_theme = "LIGHT" if "light" in current_theme_value else "DARK"
             if theme == current_theme:
-                self.logger.debug('Theme is already set to the desired theme')
+                self.logger.debug("Theme is already set to the desired theme")
                 return self._get_out_of_menu()
-            self.logger.debug(f'Current theme is {current_theme}')
+            self.logger.debug(f"Current theme is {current_theme}")
 
             select_element = self.driver.find_element(*CGPTV.theme_select)
             ActionChains(self.driver).move_to_element(select_element).perform()
-            select_clicked = self.driver.safe_click(CGPTV.theme_select, timeout = 60)
+            select_clicked = self.driver.safe_click(CGPTV.theme_select, timeout=60)
             if not select_clicked:
-                self.logger.debug('Could not click theme select')
+                self.logger.debug("Could not click theme select")
                 return self._get_out_of_menu()
-            self.logger.debug('Clicked theme select')
+            self.logger.debug("Clicked theme select")
 
-            if theme == 'OPPOSITE':
-                if current_theme == 'SYSTEM':
-                    self.logger.debug('Theme cannot be set to opposite of system theme')
+            if theme == "OPPOSITE":
+                if current_theme == "SYSTEM":
+                    self.logger.debug("Theme cannot be set to opposite of system theme")
                     return self._get_out_of_menu()
-                    
-                opposite_theme = 'dark' if current_theme == 'LIGHT' else 'light'
-                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]'), timeout = 60)
+
+                opposite_theme = "dark" if current_theme == "LIGHT" else "light"
+                option_clicked = self.driver.safe_click(
+                    (By.CSS_SELECTOR, f"select.rounded option[value={opposite_theme}]"),
+                    timeout=60,
+                )
                 if not option_clicked:
-                    self.logger.debug('Could not click opposite theme option')
+                    self.logger.debug("Could not click opposite theme option")
                     return self._get_out_of_menu()
-                self.logger.debug(f'Selected opposite theme of {current_theme}')
+                self.logger.debug(f"Selected opposite theme of {current_theme}")
             else:
-                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]'), timeout = 60)
+                option_clicked = self.driver.safe_click(
+                    (By.CSS_SELECTOR, f"select.rounded option[value={theme.lower()}]"),
+                    timeout=60,
+                )
                 if not option_clicked:
-                    self.logger.debug('Could not click theme option')
+                    self.logger.debug("Could not click theme option")
                     return self._get_out_of_menu()
-                self.logger.debug(f'Selected theme {theme}')
-            
-            self.logger.debug('Theme switched')
+                self.logger.debug(f"Selected theme {theme}")
+
+            self.logger.debug("Theme switched")
             self._get_out_of_menu()
-        except NoSuchElementException:
-            self.logger.debug('Could not find theme buttons')
+        except NoSuchElementException: # type: ignore
+            self.logger.debug("Could not find theme buttons")
             return self._get_out_of_menu()
 
     def switch_account(self, session_token: str) -> SessionData:
         """
         Switch the account.
 
         Args:
@@ -624,163 +850,179 @@
             SessionData: The new account's session data.
 
         Raises:
         ----------
             ValueError: If the session token is not provided.
             ValueError: If the response is invalid.
         """
-        self.logger.debug('Switching account...')
-        self.conversation_id = '' # Old conversation ID cannot be loaded in the new account
+        self.logger.debug("Switching account...")
+        self.conversation_id = (
+            ""  # Old conversation ID cannot be loaded in the new account
+        )
         self.driver.execute_cdp_cmd(
-            'Network.setCookie',
+            "Network.setCookie",
             {
-                'domain': 'chat.openai.com',
-                'path': '/',
-                'name': '__Secure-next-auth.session-token',
-                'value': session_token,
-                'httpOnly': True,
-                'secure': True,
+                "domain": "chat.openai.com",
+                "path": "/",
+                "name": "__Secure-next-auth.session-token",
+                "value": session_token,
+                "httpOnly": True,
+                "secure": True,
             },
         )
-        self.logger.debug('Executed CDP command')
+        self.logger.debug("Executed CDP command")
 
-        self.logger.debug('Validating authorization...')
-        self.driver.get('https://chat.openai.com/api/auth/session')
+        self.logger.debug("Validating authorization...")
+        self.driver.get("https://chat.openai.com/api/auth/session")
         response = self.driver.page_source
-        if response[0] != '{':
-            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        if response[0] != "{":
+            response = self.driver.find_element(By.TAG_NAME, "pre").text
         response = loads(response)
         if (not response) or (
-            'error' in response and response['error'] == 'RefreshAccessTokenError'
+            "error" in response and response["error"] == "RefreshAccessTokenError"
         ):
-            raise ValueError('Invalid session token')
+            raise ValueError("Invalid session token")
         session_data = SessionData(
-            User(**response['user']),
+            User(**response["user"]),
             response["expires"],
             response["accessToken"],
-            response["authProvider"]
+            response["authProvider"],
         )
-        self.logger.debug('Authorization is valid')
+        self.logger.debug("Authorization is valid")
 
-        self.logger.debug('Opening chat page...')
-        self.driver.get(f'{CGPTV.chat_url}/{self._conversation_id}')
-        self.logger.debug('Opened chat page')
+        self.logger.debug("Opening chat page...")
+        self.driver.get(f"{CGPTV.chat_url}/{self._conversation_id}")
+        self.logger.debug("Opened chat page")
         self._check_blocking_elements()
-        self.logger.debug('Switched account')
+        self.logger.debug("Switched account")
         return session_data
-    
+
     def get_session_data(self) -> SessionData:
         """
         Get the session data.
 
         Returns:
         ----------
             SessionData: The current account's session data.
         """
-        self.logger.debug('Getting account data...')
-        self.logger.debug('Opening new tab...')
+        self.logger.debug("Getting account data...")
+        self.logger.debug("Opening new tab...")
         self.driver.execute_script("window.open();")
         self.driver.switch_to.window(self.driver.window_handles[-1])
-        self.driver.get('https://chat.openai.com/api/auth/session')
+        self.driver.get("https://chat.openai.com/api/auth/session")
         response = self.driver.page_source
-        if response[0] != '{':
-            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        if response[0] != "{":
+            response = self.driver.find_element(By.TAG_NAME, "pre").text
         response = loads(response)
         session_data = SessionData(
-            User(**response['user']),
+            User(**response["user"]),
             response["expires"],
             response["accessToken"],
-            response["authProvider"]
+            response["authProvider"],
         )
-        self.logger.debug('Closing tab...')
+        self.logger.debug("Closing tab...")
         self.driver.close()
         self.driver.switch_to.window(self.driver.window_handles[0])
         return session_data
 
     def logout(self) -> None:
         """
         Logs out of the current account signed into https://chat.openai.com
         """
-        self.logger.debug('Logging out...')
+        self.logger.debug("Logging out...")
         self.driver.execute_cdp_cmd(
-            'Network.deleteCookies',
+            "Network.deleteCookies",
             {
-                'name': '__Secure-next-auth.session-token',
-                'url': 'https://chat.openai.com',
+                "name": "__Secure-next-auth.session-token",
+                "url": "https://chat.openai.com",
             },
         )
-        self.logger.debug('Executed CDP command')
-        self.driver.get('https://chat.openai.com/api/auth/session')
+        self.logger.debug("Executed CDP command")
+        self.driver.get("https://chat.openai.com/api/auth/session")
         response = self.driver.page_source
-        if response[0] != '{':
-            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        if response[0] != "{":
+            response = self.driver.find_element(By.TAG_NAME, "pre").text
         response = loads(response)
         if response == {}:
-            self.logger.debug('Logout successful')
+            self.logger.debug("Logout successful")
             return
 
     def toggle_chat_history(self, state: bool = False) -> None:
         """
         Toggle chat history.
 
         Args:
         ----------
             state (bool, optional): The state to set the chat history toggle to. Defaults to False.
         """
-        self.logger.debug('Disabling chat history...')
+        self.logger.debug("Disabling chat history...")
         try:
             menu_button_clicked = self.driver.safe_click(CGPTV.menu_button)
             if not menu_button_clicked:
-                self.logger.debug('Could not click menu button')
+                self.logger.debug("Could not click menu button")
                 return self._get_out_of_menu()
 
-            self.logger.debug('Clicked menu button')
-            
+            self.logger.debug("Clicked menu button")
+
             settings_button_clicked = self.driver.safe_click(CGPTV.menu_settings)
             if not settings_button_clicked:
-                self.logger.debug('Could not click settings button')
+                self.logger.debug("Could not click settings button")
                 return self._get_out_of_menu()
 
-            self.logger.debug('Clicked settings button')
+            self.logger.debug("Clicked settings button")
 
             wait = WebDriverWait(self.driver, 60)
 
             # Click "Data controls" button
             data_controls_clicked = self.driver.safe_click(
-                CGPTV.data_controls, timeout = 60
+                CGPTV.data_controls, timeout=60
             )
             if not data_controls_clicked:
-                self.logger.debug('Could not click data controls button')
+                self.logger.debug("Could not click data controls button")
                 return self._get_out_of_menu()
 
             # Click "Disable chat history" button
             # Not using safe_click because it there are some checks that need to be done before clicking
-            chat_history_toggle = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Chat History & Training"]')))
-            current_state = True if chat_history_toggle.get_attribute('aria-checked') == 'true' else False
+            chat_history_toggle = wait.until(
+                EC.element_to_be_clickable(
+                    (By.CSS_SELECTOR, f'button[aria-label="Chat History & Training"]')
+                )
+            )
+            current_state = (
+                True
+                if chat_history_toggle.get_attribute("aria-checked") == "true"
+                else False
+            )
             if current_state == state:
-                self.logger.debug('Chat history is already set to the desired state')
+                self.logger.debug("Chat history is already set to the desired state")
                 return self._get_out_of_menu()
 
             chat_history_toggle.click()
-            self.logger.debug(f'Chat history is now {"enabled" if state else "disabled"}')
-            self._get_out_of_menu()
+            self.logger.debug(
+                f'Chat history is now {"enabled" if state else "disabled"}'
+            )
         except:
-            self.logger.debug(f'Could not {"enable" if state else "disable"} chat history')
-            return self._get_out_of_menu()
-    
+            self.logger.debug(
+                f'Could not {"enable" if state else "disable"} chat history'
+            )
+        
+        self._history_and_training_enabled = state
+
+        return self._get_out_of_menu()
+
     def switch_conversation(self, conversation_id: str) -> None:
         """
         Switch the conversation.
 
         Args:
         ----------
             conversation_id (str): The conversation ID to switch to.
 
         Raises:
         ----------
             InvalidConversationID: If the conversation ID is invalid.
         """
-        self.logger.debug('Switching conversation...')
-        self.driver.get(f'{CGPTV.chat_url}/{conversation_id}')
+        self.logger.debug("Switching conversation...")
+        self.driver.get(f"{CGPTV.chat_url}/{conversation_id}")
         self._check_blocking_elements()
         self._conversation_id = conversation_id
-        self.logger.debug(f'Switched conversation to {conversation_id}')
+        self.logger.debug(f"Switched conversation to {conversation_id}")
```

### Comparing `UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.6/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,90 +1,77 @@
 from dataclasses import dataclass
+
 from selenium.webdriver.common.by import By
 
+
 @dataclass
 class ChatGPTVariables:
     # Other
     outer_html = (By.XPATH, "/html")
-    cf_challenge_form = (By.ID, 'challenge-form')
+    cf_challenge_form = (By.ID, "challenge-form")
     chats_list_first_node = (
         By.XPATH,
         '//div[substring(@class, string-length(@class) - string-length("text-sm") + 1)  = "text-sm"]//a',
     )
 
     # Popups and such
     info_buttons = (
-        (By.XPATH, '/html/body/div[3]/div/div/div/div[2]/div/div[2]/button'),
-        (By.XPATH, '/html/body/div[3]/div/div/div/div[2]/div/div[2]/button[2]'),
-        (By.XPATH, '/html/body/div[3]/div/div/div/div[2]/div/div[2]/button[2]'),
-    )
-    alert = (
-        By.XPATH,
-        '//div[@role="alert"]'
-    )
-    intro = (
-        By.ID,
-        'headlessui-portal-root'
+        (By.XPATH, "/html/body/div[3]/div/div/div/div[2]/div/div[2]/button"),
+        (By.XPATH, "/html/body/div[3]/div/div/div/div[2]/div/div[2]/button[2]"),
+        (By.XPATH, "/html/body/div[3]/div/div/div/div[2]/div/div[2]/button[2]"),
     )
-    
+    alert = (By.XPATH, '//div[@role="alert"]')
+    intro = (By.ID, "headlessui-portal-root")
+
     # Responses and such
     streaming = (
         By.XPATH,
-        '//div[starts-with(@class, "result-streaming markdown prose")]'
-    )
-    big_response = (
-        By.XPATH,
-        '//div[@class="flex-1 overflow-hidden"]//div[p]'
+        '//div[starts-with(@class, "result-streaming markdown prose")]',
     )
+    big_response = (By.XPATH, '//div[@class="flex-1 overflow-hidden"]//div[p]')
     small_response = (
         By.XPATH,
         '//div[starts-with(@class, "markdown prose w-full break-words")]',
     )
-    textbox = (
-        By.XPATH,
-        '//textarea[@id="prompt-textarea"]'
-    )
+    textbox = (By.XPATH, '//textarea[@id="prompt-textarea"]')
     continue_regenerating = (
         By.XPATH,
-        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button[2]"
+        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button[2]",
     )
     regenerate_response = (
         By.XPATH,
-        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button"
-    )
-    new_chat = (
-        By.LINK_TEXT,
-        'New chat'
+        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button",
     )
+    new_chat = (By.LINK_TEXT, "New chat")
+    clear_chat = (By.LINK_TEXT, "Clear chat")
 
     # Menu buttons
     menu_button = (
         By.XPATH,
-        "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[4]/div/button"
+        "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[4]/div/button",
     )
     menu_clear_conversations = (
         # By.XPATH,
         # "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[3]/div/div/nav/a[2]"
         By.LINK_TEXT,
-        'Clear conversations'
-    )
-    menu_confirm_clear_conversations = (
-        By.LINK_TEXT,
-        "Confirm clear conversations"
+        "Clear conversations",
     )
+    menu_confirm_clear_conversations = (By.LINK_TEXT, "Confirm clear conversations")
     menu_settings = (
         # By.XPATH,
         # "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[3]/div/div/nav/a[3]"
         By.LINK_TEXT,
-        'Settings'
-    )
-    theme_select = (
-        By.CSS_SELECTOR,
-        'select.rounded'
+        "Settings",
     )
+    theme_select = (By.CSS_SELECTOR, "select.rounded")
     data_controls = (
         By.CSS_SELECTOR,
-        'button[data-state="inactive"][id^="radix-"][id$="-trigger-DataControls"]'
+        'button[data-state="inactive"][id^="radix-"][id$="-trigger-DataControls"]',
+    )
+    shared_links_manage = (
+        By.XPATH,
+        # "/html/body/div[5]/div/div/div/div[2]/div[1]/div[4]/div/div[2]/div/button"
+        "//button[.//div[text()='Manage']]"
     )
-    
+
     # URLs
-    chat_url = 'https://chat.openai.com/chat'
+    chat_url = "https://chat.openai.com/chat"
```

### Comparing `UnlimitedGPT-0.1.5.5/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.6/UnlimitedGPT/internal/driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import undetected_chromedriver as uc
-from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 
 class ChatGPTDriver(uc.Chrome):
     """
     Custom selenium driver for ChatGPT.
     ##### Still in development.
     """
+
     def __init__(self, options: uc.ChromeOptions, headless: bool = False):
-        super().__init__(options=options, headless=headless)
+        caps = DesiredCapabilities.CHROME
+        caps['goog:loggingPrefs'] = {'performance': 'ALL'}
+        
+        super().__init__(options=options, headless=headless, desired_capabilities=caps)
 
     def safe_click(self, mark, timeout: int = 10) -> bool:
         """
         Clicks an element, and if it fails, tries again.
 
         Args:
         ----------
             mark: (By, str): The element to click.
             timeout: (int): The amount of time to wait for the element to be clickable.
-        
+
         Returns:
         ----------
             bool: Whether or not the element was clicked.
         """
         wait = WebDriverWait(self, timeout)
         try:
             element = wait.until(EC.element_to_be_clickable(mark))
```

### Comparing `UnlimitedGPT-0.1.5.5/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.5.5
+Version: 0.1.6
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
@@ -31,15 +31,15 @@
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/Sxvxgeness.svg?style=social)](https://twitter.com/Sxvxgeness)
 
 UnlimitedGPT is a Python library for using the ChatGPT website as an alternative API to the OpenAI paid API.
 
 UnlimitedGPT makes it easy to send messages and receive responses. UnlimitedGPT can also do a wide range of things such as getting the user data, getting the session data, clearing all conversations, resetting the current conversation, switching themes, switching accounts, and logging out from the session.
 
-![Preview](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/docs/assets/preview.png)
+![Preview](https://raw.githubusercontent.com/Sxvxgee/UnlimitedGPT/main/docs/assets/preview.png)
 
 ## Compatibility
 UnlimitedGPT works on Windows, Linux and macOS. It also works on Google Colab and other headless  linux servers. UnlimitedGPT requires Python 3.8 or later.
 
 ## Features
 
 -   [x] Cloudflare's anti-bot protection bypass using `undetected_chromedriver`
```

### Comparing `UnlimitedGPT-0.1.5.5/setup.py` & `UnlimitedGPT-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 base_path = os.path.abspath(os.path.dirname(__file__))
 
 requirements = []
-with open(os.path.join(os.path.dirname(base_path), 'requirements.txt')) as f:
+with open(os.path.join(os.path.dirname(base_path), "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
-readme = ''
-with open(os.path.join(os.path.dirname(base_path), 'README.md')) as f:
+readme = ""
+with open(os.path.join(os.path.dirname(base_path), "README.md")) as f:
     readme = f.read()
 
 setup(
-    name='UnlimitedGPT',
-    author='Sxvxge',
-    url='https://github.com/Sxvxgee/UnlimitedGPT',
+    name="UnlimitedGPT",
+    author="Sxvxge",
+    url="https://github.com/Sxvxgee/UnlimitedGPT",
     project_urls={
-        'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
-        'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
-        'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
+        "Documentation": "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md",
+        "Issue tracker": "https://github.com/Sxvxgee/UnlimitedGPT/issues",
+        "Changelog": "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md",
     },
-    version="0.1.5.5",
-    packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
-    py_modules=['UnlimitedGPT'],
-    license='GPL-3.0 license',
-    description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
+    version="0.1.6",
+    packages=["UnlimitedGPT", "UnlimitedGPT/internal"],
+    py_modules=["UnlimitedGPT"],
+    license="GPL-3.0 license",
+    description="An unofficial Python wrapper for OpenAI's ChatGPT API",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=requirements,
-    python_requires='>=3.8.0',
+    python_requires=">=3.8.0",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Internet',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-        'Typing :: Typed',
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Internet",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Utilities",
+        "Typing :: Typed",
     ],
 )
```

