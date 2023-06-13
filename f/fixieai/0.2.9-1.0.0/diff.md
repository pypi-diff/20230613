# Comparing `tmp/fixieai-0.2.9.tar.gz` & `tmp/fixieai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixieai-0.2.9.tar", max compression
+gzip compressed data, was "fixieai-1.0.0.tar", max compression
```

## Comparing `fixieai-0.2.9.tar` & `fixieai-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-02-23 22:50:37.233187 fixieai-0.2.9/LICENSE
--rw-r--r--   0        0        0     1070 2023-03-30 01:29:50.785632 fixieai-0.2.9/fixieai/__init__.py
--rw-r--r--   0        0        0      875 2023-03-30 01:29:50.786037 fixieai-0.2.9/fixieai/agents/__init__.py
--rw-r--r--   0        0        0     9263 2023-03-30 01:29:50.786680 fixieai-0.2.9/fixieai/agents/agent_base.py
--rw-r--r--   0        0        0     7113 2023-03-30 01:29:50.787128 fixieai-0.2.9/fixieai/agents/agent_base_test.py
--rw-r--r--   0        0        0     2686 2023-03-30 01:29:50.787476 fixieai-0.2.9/fixieai/agents/api.py
--rw-r--r--   0        0        0      863 2023-03-09 06:10:51.909511 fixieai-0.2.9/fixieai/agents/api_test.py
--rw-r--r--   0        0        0     3491 2023-03-30 01:29:50.787837 fixieai-0.2.9/fixieai/agents/code_shot.py
--rw-r--r--   0        0        0     2943 2023-03-30 01:29:50.788076 fixieai-0.2.9/fixieai/agents/code_shot_test.py
--rw-r--r--   0        0        0      392 2023-03-09 06:10:51.910776 fixieai-0.2.9/fixieai/agents/corpora.py
--rw-r--r--   0        0        0     1046 2023-03-30 01:29:50.788247 fixieai-0.2.9/fixieai/agents/llm_settings.py
--rw-r--r--   0        0        0      839 2023-03-30 01:29:50.788531 fixieai-0.2.9/fixieai/agents/metadata.py
--rw-r--r--   0        0        0     8993 2023-03-03 23:24:37.371114 fixieai-0.2.9/fixieai/agents/oauth.py
--rw-r--r--   0        0        0     2127 2023-03-30 01:29:50.788828 fixieai-0.2.9/fixieai/agents/standalone.py
--rw-r--r--   0        0        0     2154 2023-03-30 01:29:50.789122 fixieai-0.2.9/fixieai/agents/standalone_test.py
--rw-r--r--   0        0        0     4711 2023-03-29 22:13:30.104697 fixieai-0.2.9/fixieai/agents/user_storage.py
--rw-r--r--   0        0        0     3092 2023-02-23 22:50:37.238945 fixieai-0.2.9/fixieai/agents/user_storage_test.py
--rw-r--r--   0        0        0    10844 2023-03-30 01:29:50.789410 fixieai-0.2.9/fixieai/agents/utils.py
--rw-r--r--   0        0        0     5253 2023-03-23 19:55:59.426492 fixieai-0.2.9/fixieai/agents/utils_test.py
--rw-r--r--   0        0        0        0 2023-03-07 21:53:04.349446 fixieai-0.2.9/fixieai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:08:15.229030 fixieai-0.2.9/fixieai/cli/agent/__init__.py
--rw-r--r--   0        0        0     1958 2023-03-23 19:55:59.427036 fixieai-0.2.9/fixieai/cli/agent/agent_config.py
--rw-r--r--   0        0        0      383 2023-03-07 17:08:15.229614 fixieai-0.2.9/fixieai/cli/agent/agent_config_test.py
--rw-r--r--   0        0        0    19402 2023-03-30 01:29:50.789950 fixieai-0.2.9/fixieai/cli/agent/commands.py
--rw-r--r--   0        0        0      949 2023-03-14 03:29:01.740659 fixieai-0.2.9/fixieai/cli/agent/commands_test.py
--rw-r--r--   0        0        0     2791 2023-03-30 01:29:50.790201 fixieai-0.2.9/fixieai/cli/agent/loader.py
--rw-r--r--   0        0        0     1641 2023-03-27 20:03:17.154129 fixieai-0.2.9/fixieai/cli/agent/tunnel.py
--rw-r--r--   0        0        0        0 2023-03-09 06:10:51.912134 fixieai-0.2.9/fixieai/cli/auth/__init__.py
--rw-r--r--   0        0        0     1753 2023-03-28 16:51:27.399587 fixieai-0.2.9/fixieai/cli/auth/commands.py
--rw-r--r--   0        0        0     1942 2023-03-09 06:10:51.912797 fixieai-0.2.9/fixieai/cli/auth/oauth_flow.py
--rw-r--r--   0        0        0     2667 2023-03-28 16:51:27.399926 fixieai-0.2.9/fixieai/cli/auth/user_config.py
--rw-r--r--   0        0        0     2120 2023-03-28 16:51:27.400303 fixieai-0.2.9/fixieai/cli/auth/user_config_test.py
--rwxr-xr-x   0        0        0     1581 2023-03-11 00:03:34.150504 fixieai-0.2.9/fixieai/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-07 17:08:15.230356 fixieai-0.2.9/fixieai/cli/session/__init__.py
--rw-r--r--   0        0        0     1731 2023-03-11 00:03:34.150791 fixieai-0.2.9/fixieai/cli/session/commands.py
--rw-r--r--   0        0        0     4720 2023-03-14 03:29:01.741160 fixieai-0.2.9/fixieai/cli/session/console.py
--rw-r--r--   0        0        0     1523 2023-03-28 16:51:27.400549 fixieai-0.2.9/fixieai/cli/utils.py
--rw-r--r--   0        0        0      655 2023-03-14 20:27:29.607865 fixieai-0.2.9/fixieai/cli/utils_test.py
--rw-r--r--   0        0        0      322 2023-03-07 17:08:15.231370 fixieai-0.2.9/fixieai/client/__init__.py
--rw-r--r--   0        0        0    12332 2023-03-14 20:27:29.608238 fixieai-0.2.9/fixieai/client/agent.py
--rwxr-xr-x   0        0        0     6979 2023-03-28 15:52:10.550353 fixieai-0.2.9/fixieai/client/client.py
--rw-r--r--   0        0        0     4987 2023-03-11 00:03:34.152283 fixieai-0.2.9/fixieai/client/client_test.py
--rwxr-xr-x   0        0        0     8750 2023-03-11 00:03:34.152549 fixieai-0.2.9/fixieai/client/session.py
--rw-r--r--   0        0        0     2238 2023-03-28 16:51:27.400784 fixieai-0.2.9/fixieai/constants.py
--rw-r--r--   0        0        0     1874 2023-03-30 01:30:27.861585 fixieai-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 fixieai-0.2.9/setup.py
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 fixieai-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-07 23:45:43.683245 fixieai-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1388 2023-06-05 22:24:43.848602 fixieai-1.0.0/fixieai/__init__.py
+-rw-r--r--   0        0        0     1301 2023-06-05 22:24:43.848729 fixieai-1.0.0/fixieai/agents/__init__.py
+-rw-r--r--   0        0        0    10564 2023-06-05 22:24:43.849458 fixieai-1.0.0/fixieai/agents/agent_base.py
+-rw-r--r--   0        0        0    12042 2023-06-05 22:24:43.849590 fixieai-1.0.0/fixieai/agents/agent_base_test.py
+-rw-r--r--   0        0        0    15267 2023-06-05 22:24:43.849720 fixieai-1.0.0/fixieai/agents/agent_func.py
+-rw-r--r--   0        0        0     8715 2023-06-05 22:24:43.849847 fixieai-1.0.0/fixieai/agents/agent_func_test.py
+-rw-r--r--   0        0        0     2965 2023-06-05 22:24:43.849947 fixieai-1.0.0/fixieai/agents/api.py
+-rw-r--r--   0        0        0      863 2023-03-09 19:26:37.964207 fixieai-1.0.0/fixieai/agents/api_test.py
+-rw-r--r--   0        0        0     3786 2023-06-05 22:24:43.850060 fixieai-1.0.0/fixieai/agents/code_shot.py
+-rw-r--r--   0        0        0     3306 2023-06-05 22:24:43.850149 fixieai-1.0.0/fixieai/agents/code_shot_test.py
+-rw-r--r--   0        0        0     7152 2023-06-05 22:24:43.850261 fixieai-1.0.0/fixieai/agents/corpora.py
+-rw-r--r--   0        0        0     1943 2023-06-05 22:24:43.850315 fixieai-1.0.0/fixieai/agents/corpora_test.py
+-rw-r--r--   0        0        0     2279 2023-06-05 22:24:43.850379 fixieai-1.0.0/fixieai/agents/exceptions.py
+-rw-r--r--   0        0        0     1046 2023-03-30 16:24:35.974599 fixieai-1.0.0/fixieai/agents/llm_settings.py
+-rw-r--r--   0        0        0      891 2023-06-05 22:24:43.850459 fixieai-1.0.0/fixieai/agents/metadata.py
+-rw-r--r--   0        0        0     9000 2023-06-05 22:24:43.850566 fixieai-1.0.0/fixieai/agents/oauth.py
+-rw-r--r--   0        0        0     4048 2023-04-25 03:00:21.707100 fixieai-1.0.0/fixieai/agents/openai_proxy.py
+-rw-r--r--   0        0        0     1627 2023-04-25 03:00:21.707249 fixieai-1.0.0/fixieai/agents/openai_proxy_test.py
+-rw-r--r--   0        0        0     2439 2023-06-05 22:24:43.850673 fixieai-1.0.0/fixieai/agents/standalone.py
+-rw-r--r--   0        0        0     4414 2023-06-05 22:24:43.850780 fixieai-1.0.0/fixieai/agents/standalone_test.py
+-rw-r--r--   0        0        0     1918 2023-06-05 22:24:43.850853 fixieai-1.0.0/fixieai/agents/token.py
+-rw-r--r--   0        0        0     4951 2023-06-05 22:24:43.850975 fixieai-1.0.0/fixieai/agents/user_storage.py
+-rw-r--r--   0        0        0     3388 2023-06-05 22:24:43.851664 fixieai-1.0.0/fixieai/agents/user_storage_test.py
+-rw-r--r--   0        0        0     7966 2023-04-25 03:00:21.707832 fixieai-1.0.0/fixieai/agents/utils.py
+-rw-r--r--   0        0        0     5253 2023-03-25 02:35:27.951289 fixieai-1.0.0/fixieai/agents/utils_test.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.965971 fixieai-1.0.0/fixieai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.966917 fixieai-1.0.0/fixieai/cli/agent/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-05 22:24:43.852159 fixieai-1.0.0/fixieai/cli/agent/agent_config.py
+-rw-r--r--   0        0        0    34827 2023-06-05 22:24:43.852447 fixieai-1.0.0/fixieai/cli/agent/commands.py
+-rw-r--r--   0        0        0    16037 2023-06-05 22:45:51.414577 fixieai-1.0.0/fixieai/cli/agent/commands_test.py
+-rw-r--r--   0        0        0     3488 2023-06-05 22:24:43.852973 fixieai-1.0.0/fixieai/cli/agent/loader.py
+-rw-r--r--   0        0        0     1753 2023-04-01 03:10:09.936255 fixieai-1.0.0/fixieai/cli/agent/tunnel.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.967623 fixieai-1.0.0/fixieai/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-01 23:07:48.256193 fixieai-1.0.0/fixieai/cli/auth/commands.py
+-rw-r--r--   0        0        0     1942 2023-03-09 19:26:37.968039 fixieai-1.0.0/fixieai/cli/auth/oauth_flow.py
+-rw-r--r--   0        0        0     2667 2023-03-30 16:24:35.975821 fixieai-1.0.0/fixieai/cli/auth/user_config.py
+-rw-r--r--   0        0        0     2120 2023-03-30 16:24:35.975913 fixieai-1.0.0/fixieai/cli/auth/user_config_test.py
+-rwxr-xr-x   0        0        0     3290 2023-04-12 15:22:13.299089 fixieai-1.0.0/fixieai/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.968257 fixieai-1.0.0/fixieai/cli/session/__init__.py
+-rw-r--r--   0        0        0     4761 2023-04-12 01:22:58.394077 fixieai-1.0.0/fixieai/cli/session/commands.py
+-rw-r--r--   0        0        0     4720 2023-06-05 22:24:43.853234 fixieai-1.0.0/fixieai/cli/session/console.py
+-rw-r--r--   0        0        0     1523 2023-03-30 16:24:35.976029 fixieai-1.0.0/fixieai/cli/utils.py
+-rw-r--r--   0        0        0      655 2023-03-22 17:59:48.856855 fixieai-1.0.0/fixieai/cli/utils_test.py
+-rw-r--r--   0        0        0      322 2023-03-09 19:26:37.968576 fixieai-1.0.0/fixieai/client/__init__.py
+-rw-r--r--   0        0        0    11895 2023-06-06 15:54:00.163441 fixieai-1.0.0/fixieai/client/agent.py
+-rwxr-xr-x   0        0        0    12607 2023-06-05 22:39:38.544081 fixieai-1.0.0/fixieai/client/client.py
+-rw-r--r--   0        0        0     4987 2023-03-10 17:44:40.327464 fixieai-1.0.0/fixieai/client/client_test.py
+-rwxr-xr-x   0        0        0     8750 2023-03-10 05:45:43.499628 fixieai-1.0.0/fixieai/client/session.py
+-rw-r--r--   0        0        0     1402 2023-06-05 22:24:43.853545 fixieai-1.0.0/fixieai/client/utils.py
+-rw-r--r--   0        0        0     2394 2023-06-05 22:24:43.853647 fixieai-1.0.0/fixieai/constants.py
+-rw-r--r--   0        0        0     2026 2023-06-13 15:28:51.610689 fixieai-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 fixieai-1.0.0/setup.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 fixieai-1.0.0/PKG-INFO
```

### Comparing `fixieai-0.2.9/LICENSE` & `fixieai-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/__init__.py` & `fixieai-1.0.0/fixieai/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import importlib.metadata
 
 from fixieai.agents import AgentQuery
 from fixieai.agents import AgentResponse
 from fixieai.agents import CodeShotAgent
+from fixieai.agents import CorpusDocument
+from fixieai.agents import CorpusPage
+from fixieai.agents import CorpusPartition
+from fixieai.agents import CorpusRequest
+from fixieai.agents import CorpusResponse
 from fixieai.agents import DocumentCorpus
-from fixieai.agents import DocumentLoader
 from fixieai.agents import Embed
 from fixieai.agents import LlmSettings
 from fixieai.agents import Message
 from fixieai.agents import OAuthHandler
 from fixieai.agents import OAuthParams
 from fixieai.agents import StandaloneAgent
+from fixieai.agents import UrlDocumentCorpus
 from fixieai.agents import UserStorage
 from fixieai.client import FixieClient
 from fixieai.client import get_agents
 from fixieai.client import get_client
 from fixieai.client import get_embeds
 from fixieai.client import query
 
 __all__ = [
     "AgentQuery",
     "AgentResponse",
     "Embed",
     "Message",
     "CodeShotAgent",
-    "StandaloneAgent",
+    "CorpusDocument",
+    "CorpusPage",
+    "CorpusPartition",
+    "CorpusRequest",
+    "CorpusResponse",
     "DocumentCorpus",
-    "DocumentLoader",
+    "StandaloneAgent",
     "LlmSettings",
     "OAuthParams",
     "OAuthHandler",
+    "UrlDocumentCorpus",
     "UserStorage",
     "FixieClient",
     "get_agents",
     "get_client",
     "get_embeds",
     "query",
 ]
```

### Comparing `fixieai-0.2.9/fixieai/agents/agent_base.py` & `fixieai-1.0.0/fixieai/agents/agent_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 from __future__ import annotations
 
 import abc
 import dataclasses
 import functools
-import inspect
 import json
-import logging
 import os
 import re
 import warnings
-from typing import Any, Callable, Dict, Iterable, Optional
+from typing import Callable, Dict, Optional, TypeVar
 
 import fastapi
 import fastapi.security
 import jwt
 import starlette.responses
 import uvicorn
 import yaml
-from pydantic import dataclasses as pydantic_dataclasses
 
 from fixieai import constants
+from fixieai.agents import agent_func
 from fixieai.agents import api
+from fixieai.agents import corpora
+from fixieai.agents import exceptions
 from fixieai.agents import metadata as agent_metadata
 from fixieai.agents import oauth
-from fixieai.agents import user_storage
-from fixieai.agents import utils
+from fixieai.agents import token
 
 # Regex that controls what Func names are allowed.
 ACCEPTED_FUNC_NAMES = re.compile(r"^\w+$")
 
-# The JWT claim containing the agent ID
-_AGENT_ID_JWT_CLAIM = "aid"
-
 _RESPONSE_CHUNK_SIZE = 1024
 
-logger = logging.getLogger(__file__)
-
 
 class AgentBase(abc.ABC):
     """Base class for Fixie agents."""
 
     def __init__(
         self,
         oauth_params: Optional[oauth.OAuthParams] = None,
     ):
         self.oauth_params = oauth_params
-        self._funcs: Dict[str, Callable] = {}
+        self._funcs: Dict[str, agent_func.AgentQueryFunc] = {}
+        self._corpus_funcs: Dict[str, agent_func.AgentCorpusFunc] = {}
         self._jwks_client = jwt.PyJWKClient(constants.FIXIE_JWKS_URL)
         self._allowed_agent_id = os.getenv("FIXIE_ALLOWED_AGENT_ID")
         if self._allowed_agent_id is None:
             warnings.warn(
                 "No allowed agent ID was specified, so your agent will accept requests intended for any agent. "
                 "Ensure that the FIXIE_ALLOWED_AGENT_ID variable is set to correct this."
             )
@@ -75,22 +70,28 @@
         """
         uvicorn.run(self.app(), host=host, port=port)
 
     def app(self) -> fastapi.FastAPI:
         """Returns a fastapi.FastAPI application that serves the agent."""
         fast_api = fastapi.FastAPI()
         fast_api.include_router(self.api_router())
+        fast_api.add_exception_handler(
+            exceptions.AgentException, exceptions.AgentException.fastapi_handler
+        )
 
         return fast_api
 
     def api_router(self) -> fastapi.APIRouter:
         """Returns a fastapi.APIRouter object that serves the agent."""
         router = fastapi.APIRouter()
         router.add_api_route("/", self._handshake, methods=["GET"])
         router.add_api_route("/{func_name}", self._serve_func, methods=["POST"])
+        router.add_api_route(
+            "/corpus/{corpus_func_name}", self._serve_corpus_func, methods=["POST"]
+        )
         return router
 
     def is_valid_func_name(self, func_name: str) -> bool:
         """Indicates if the given func name is valid (either registered or built-in).
 
         Args:
             func_name: The func name to check
@@ -115,36 +116,97 @@
         Optional Decorator Args:
             func_name: Optional function name to register this function by. If unset,
                 the function name will be used.
         """
         if func is None:
             # Func is not passed in. It's the decorator being created.
             return functools.partial(self.register_func, func_name=func_name)
+        non_null_func: Callable = func
 
+        AgentBase._register_func_internal(
+            func,
+            func_name,
+            self._funcs,
+            lambda: agent_func.AgentQueryFunc.create(
+                non_null_func,
+                self.oauth_params,
+                default_message_type=api.Message,
+                allow_generator=False,
+            ),
+        )
+        return func
+
+    def register_corpus_func(
+        self,
+        func: Optional[
+            Callable[[corpora.CorpusRequest], corpora.CorpusResponse]
+        ] = None,
+        *,
+        func_name: Optional[str] = None,
+    ) -> Callable:
+        """A function decorator to register `Func`s used for loading a custom
+        corpus with this agent.
+
+        This decorator will not change the callable itself.
+
+        Usage:
+
+            agent = CodeShotAgent(base_prompt, few_shots)
+
+            @agent.register_corpus_func
+            def func(request: CorpusRequest) -> CorpusResponse:
+                ...
+
+        Optional Decorator Args:
+            func_name: Optional function name to register this function by. If unset,
+                the function name will be used.
+        """
+        if func is None:
+            # Func is not passed in. It's the decorator being created.
+            return functools.partial(self.register_corpus_func, func_name=func_name)
+        non_null_func: Callable[[corpora.CorpusRequest], corpora.CorpusResponse] = func
+
+        AgentBase._register_func_internal(
+            func,
+            func_name,
+            self._corpus_funcs,
+            lambda: agent_func.AgentCorpusFunc.create(non_null_func),
+        )
+        return func
+
+    T = TypeVar("T")
+
+    @staticmethod
+    def _register_func_internal(
+        func: Callable,
+        func_name: Optional[str],
+        registry: Dict[str, T],
+        create: Callable[[], T],
+    ):
         if func_name is not None:
             if not ACCEPTED_FUNC_NAMES.fullmatch(func_name):
                 raise ValueError(
                     f"Function names may only be alphanumerics, got {func_name!r}."
                 )
+        else:
+            func_name = func.__name__
 
-        utils.validate_registered_pyfunc(func, self)
-        name = func_name or func.__name__
-        if name in self._funcs:
-            raise ValueError(f"Func[{name}] is already registered with agent.")
-        self._funcs[name] = func
-        return func
+        if func_name in registry:
+            raise ValueError(f"Func[{func_name}] is already registered with agent.")
+
+        registry[func_name] = create()
 
     def _handshake(
         self,
         credentials: fastapi.security.HTTPAuthorizationCredentials = fastapi.Depends(
             fastapi.security.HTTPBearer()
         ),
     ) -> fastapi.Response:
         """Returns the agent's metadata in YAML format."""
-        token_claims = VerifiedTokenClaims.from_token(
+        token_claims = token.VerifiedTokenClaims.from_token(
             credentials.credentials, self._jwks_client, self._allowed_agent_id
         )
         if token_claims is None:
             raise fastapi.HTTPException(status_code=403, detail="Invalid token")
 
         metadata = self.metadata()
         yaml_content = yaml.dump(dataclasses.asdict(metadata))
@@ -155,116 +217,86 @@
             for start in range(0, len(yaml_content), _RESPONSE_CHUNK_SIZE)
         )
         return starlette.responses.StreamingResponse(
             chunks,
             media_type="application/yaml",
         )
 
-    def validate_token(
-        self, credentials: fastapi.security.HTTPAuthorizationCredentials
-    ):
-        token_claims = VerifiedTokenClaims.from_token(
-            credentials.credentials, self._jwks_client, self._allowed_agent_id
-        )
-        if token_claims is None:
-            raise fastapi.HTTPException(status_code=403, detail="Invalid token")
-
-        return token_claims
-
     def _serve_func(
         self,
         func_name: str,
         query: api.AgentQuery,
         credentials: fastapi.security.HTTPAuthorizationCredentials = fastapi.Depends(
             fastapi.security.HTTPBearer()
         ),
     ) -> api.AgentResponse:
         """Verifies the request is a valid request from Fixie, and dispatches it to
         the appropriate function.
         """
-        token_claims = self.validate_token(credentials)
+        token_claims = self._check_credentials(credentials)
 
         try:
             pyfunc = self._funcs[func_name]
         except KeyError:
-            raise fastapi.HTTPException(
-                status_code=404, detail=f"Func[{func_name}] doesn't exist"
+            raise exceptions.AgentException(
+                response_message=f"I'm sorry, Func[{func_name}] is not defined.",
+                error_code="ERR_FUNC_NOT_DEFINED",
+                error_message="The function was not defined.",
+                http_status_code=404,
+                func_name=func_name,
+                available_funcs=list(self._funcs.keys()),
             )
-        kwargs = self.get_func_kwargs(
-            query, token_claims, inspect.signature(pyfunc).parameters.keys()
-        )
-        output = pyfunc(**kwargs)
-        try:
-            return api.AgentResponse.from_value(output)
-        except TypeError:
-            raise TypeError(
-                f"Func[{func_name}] returned unexpected output of type {type(output)}."
-            )
-
-    def get_func_kwargs(
-        self,
-        query: api.AgentQuery,
-        token_claims: VerifiedTokenClaims,
-        arg_names: Iterable[str],
-    ) -> Dict[str, Any]:
-        kwargs: Dict[str, Any] = {}
-        for arg_name in arg_names:
-            if arg_name == "query":
-                kwargs[arg_name] = query.message
-            elif arg_name == "user_storage":
-                kwargs[arg_name] = user_storage.UserStorage(
-                    query, token_claims.agent_id
-                )
-            elif arg_name == "oauth_handler":
-                assert self.oauth_params, "oauth_params is not set"
-                kwargs[arg_name] = oauth.OAuthHandler(
-                    self.oauth_params, query, token_claims.agent_id
-                )
-            else:
-                raise ValueError(f"Found unknown argument {arg_name!r}.")
-        return kwargs
 
+        output = pyfunc(query, token_claims)
 
-@pydantic_dataclasses.dataclass
-class VerifiedTokenClaims:
-    """Verified claims from an agent token."""
+        # Streaming not allowed for funcs (yet).
+        return next(iter(output))
 
-    agent_id: str
+    def _serve_corpus_func(
+        self,
+        corpus_func_name: str,
+        request: corpora.CorpusRequest,
+        credentials: fastapi.security.HTTPAuthorizationCredentials = fastapi.Depends(
+            fastapi.security.HTTPBearer()
+        ),
+    ) -> fastapi.responses.JSONResponse:
+        """Verifies the request is a valid request from Fixie, and dispatches it to
+        the appropriate corpus function.
+        """
+        token_claims = self._check_credentials(credentials)
 
-    @staticmethod
-    def from_token(
-        token: str,
-        jwks_client: jwt.PyJWKClient,
-        expected_agent_id: Optional[str],
-    ) -> Optional[VerifiedTokenClaims]:
         try:
-            public_key = jwks_client.get_signing_key_from_jwt(token)
-            claims = jwt.decode(
-                token,
-                public_key.key,
-                algorithms=["EdDSA"],
-                audience=constants.FIXIE_AGENT_API_AUDIENCES,
+            pyfunc = self._corpus_funcs[corpus_func_name]
+        except KeyError:
+            raise exceptions.AgentException(
+                response_message=f"I'm sorry, corpus func[{corpus_func_name}] is not defined.",
+                error_code="ERR_FUNC_NOT_DEFINED",
+                error_message="The function was not defined.",
+                http_status_code=404,
+                func_name=corpus_func_name,
+                available_funcs=list(self._corpus_funcs.keys()),
             )
-        except jwt.DecodeError:
-            return None
 
-        token_agent_id = claims.get(_AGENT_ID_JWT_CLAIM)
-        if not isinstance(token_agent_id, str):
-            # Agent id claim is required
-            logger.warning("Rejecting valid JWT without any agent ID claim")
-            return None
-
-        if expected_agent_id is not None and token_agent_id != expected_agent_id:
-            # The agent ID in the token did not match the allowed value.
-            logger.warning(
-                f"Rejecting valid JWT because agent ID in token ({token_agent_id!r}) did not match {expected_agent_id!r}"
-            )
-            return None
+        output = pyfunc(request, token_claims)
+
+        result = next(iter(output))
+        # Use dataclasses_json instead of FastAPI's default json encoder. This
+        # allows us to use our own bytes encoder instead of the default, which
+        # always uses utf-8 and therefore wouldn't allow some characters.
+        return fastapi.responses.JSONResponse(result.to_dict())
 
-        return VerifiedTokenClaims(agent_id=token_agent_id)
+    def _check_credentials(
+        self, credentials: fastapi.security.HTTPAuthorizationCredentials
+    ) -> token.VerifiedTokenClaims:
+        token_claims = token.VerifiedTokenClaims.from_token(
+            credentials.credentials, self._jwks_client, self._allowed_agent_id
+        )
+        if token_claims is None:
+            raise fastapi.HTTPException(status_code=403, detail="Invalid token")
+        return token_claims
 
 
 def _oauth(query: api.Message, oauth_handler: oauth.OAuthHandler) -> str:
     """Serves Func[_oauth] which is used upon auth redirect callback."""
     auth_request = json.loads(query.text)
     state = auth_request["state"]
     code = auth_request["code"]
```

### Comparing `fixieai-0.2.9/fixieai/agents/api.py` & `fixieai-1.0.0/fixieai/agents/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module holds objects that represent the API interface by which Agents talk to
 Fixie ecosystem."""
 
 from __future__ import annotations
 
 import base64
 import dataclasses
-from typing import Dict, Optional, Union
+from typing import Dict, Generator, Optional
 
 import requests
 from pydantic import dataclasses as pydantic_dataclasses
 
 
 @pydantic_dataclasses.dataclass
 class Embed:
@@ -66,23 +66,33 @@
     # created. Agents wishing to make queries to other agents, or to other
     # Fixie services, should carry this token in the query so that it
     # can be tied back to the original user.
     access_token: Optional[str] = None
 
 
 @pydantic_dataclasses.dataclass
+class AgentError:
+    """An error that occurred in the process of generating a response."""
+
+    # A code representing the error.
+    code: str
+
+    # A message describing the error that will be displayed to the user.
+    message: str
+
+    # Additional debugging context from the error.
+    details: Optional[Dict]
+
+
+@pydantic_dataclasses.dataclass
 class AgentResponse:
     """A response message from an Agent."""
 
     # The text of the response message.
     message: Message
 
-    @classmethod
-    def from_value(cls, value: Union[str, Message, AgentResponse]) -> AgentResponse:
-        if isinstance(value, str):
-            return cls(Message(value))
-        elif isinstance(value, Message):
-            return cls(value)
-        elif isinstance(value, cls):
-            return value
-        else:
-            raise TypeError(f"Unexpected type to wrap: {type(value)}")
+    # Error details, if an error occurred generating the response. Note that `message` should still be included,
+    # but may indicate that an error occurred that prevented the agent from fully handling the request.
+    error: Optional[AgentError] = None
+
+
+AgentResponseGenerator = Generator[AgentResponse, None, None]
```

### Comparing `fixieai-0.2.9/fixieai/agents/api_test.py` & `fixieai-1.0.0/fixieai/agents/api_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/agents/code_shot.py` & `fixieai-1.0.0/fixieai/agents/code_shot.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,32 +55,40 @@
 
     """
 
     def __init__(
         self,
         base_prompt: str,
         few_shots: Union[str, List[str]],
-        corpora: Optional[List[corpora.DocumentCorpus]] = None,
+        corpora: Optional[List[corpora.UrlDocumentCorpus]] = None,
         conversational: bool = False,
         oauth_params: Optional[oauth.OAuthParams] = None,
         llm_settings: Optional[llm_settings.LlmSettings] = None,
     ):
         super().__init__(oauth_params)
 
         if isinstance(few_shots, str):
             few_shots = _split_few_shots(few_shots)
 
         self.base_prompt = base_prompt
         self.few_shots = few_shots
-        self.corpora = corpora
+        self.url_corpora = corpora
         self.conversational = conversational
         self.llm_settings = llm_settings
 
         utils.strip_prompt_lines(self)
 
+    @property
+    def corpora(self):
+        url_corpora = self.url_corpora or []
+        custom_corpora = [
+            corpora.CustomCorpus(func_name=f) for f in self._corpus_funcs.keys()
+        ]
+        return url_corpora + custom_corpora if url_corpora or custom_corpora else None
+
     def metadata(self) -> metadata.Metadata:
         return metadata.CodeShotAgentMetadata(
             self.base_prompt,
             self.few_shots,
             self.corpora,
             self.conversational,
             self.llm_settings,
```

### Comparing `fixieai-0.2.9/fixieai/agents/code_shot_test.py` & `fixieai-1.0.0/fixieai/agents/code_shot_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import dataclasses
 import os
 
 import fastapi
 import pytest
 import yaml
 from fastapi import testclient
 
 import fixieai
 from fixieai import agents
-from fixieai.agents import agent_base
 from fixieai.agents import code_shot
+from fixieai.agents import token
 
 agent_id = "dummy"
 BASE_PROMPT = "I am a simple dummy agent."
 FEW_SHOTS = """
 Q: Sample query 1
 Ask Func[simple1]: Simple argument
 Func[simple1] says: Simple response
@@ -21,26 +20,26 @@
 
 Q: Sample query 2
 Ask Func[simple2]: Simple argument
 Func[simple2] says: Simple response
 A: Simple final response
 """
 CORPORA = [
-    agents.DocumentCorpus(
-        urls=["http://example.com/doc1.txt"], loader=agents.DocumentLoader("text")
-    ),
+    agents.UrlDocumentCorpus(urls=["http://example.com/doc1.txt"]),
 ]
 
 
 @pytest.fixture(autouse=True)
 def mock_token_verifier(mocker):
     return mocker.patch.object(
-        agent_base.VerifiedTokenClaims,
+        token.VerifiedTokenClaims,
         "from_token",
-        return_value=agent_base.VerifiedTokenClaims(agent_id="fake agent id"),
+        return_value=token.VerifiedTokenClaims(
+            agent_id="fake agent id", is_anonymous=False, token="fake token"
+        ),
     )
 
 
 @pytest.fixture
 def dummy_code_shot_agent(mocker):
     mocker.patch.dict(os.environ, {"FIXIE_ALLOWED_AGENT_ID": "fake agent id"})
     agent = agents.CodeShotAgent(
@@ -56,14 +55,20 @@
             scopes=["dummy"],
         ),
         llm_settings=agents.LlmSettings(
             model="test-model", temperature=0.42, maximum_tokens=42
         ),
     )
 
+    @agent.register_corpus_func()
+    def load_empty_custom_corpus(
+        request: agents.CorpusRequest,
+    ) -> agents.CorpusResponse:
+        return agents.CorpusResponse()
+
     return agent
 
 
 def test_code_shot_handshake(dummy_code_shot_agent, mocker):
     fast_api = fastapi.FastAPI()
     fast_api.include_router(dummy_code_shot_agent.api_router())
     client = testclient.TestClient(fast_api)
@@ -71,15 +76,23 @@
     response = client.get("/", headers={"Authorization": "Bearer fixie-test-token"})
     assert response.status_code == 200
     assert response.headers["content-type"] == "application/yaml"
     yaml_content = yaml.load(response.content, Loader=yaml.Loader)
     assert yaml_content == {
         "base_prompt": dummy_code_shot_agent.base_prompt,
         "few_shots": dummy_code_shot_agent.few_shots,
-        "corpora": [dataclasses.asdict(c) for c in dummy_code_shot_agent.corpora],
+        "corpora": [
+            {
+                "urls": ["http://example.com/doc1.txt"],
+                "exclude_patterns": None,
+                "auth_token_func": None,
+                "loader": None,
+            },
+            {"func_name": "load_empty_custom_corpus"},
+        ],
         "conversational": dummy_code_shot_agent.conversational,
         "response_model": {
             "model": dummy_code_shot_agent.llm_settings.model,
             "temperature": dummy_code_shot_agent.llm_settings.temperature,
             "maximum_tokens": dummy_code_shot_agent.llm_settings.maximum_tokens,
         },
         "type": "code_shot",
```

### Comparing `fixieai-0.2.9/fixieai/agents/llm_settings.py` & `fixieai-1.0.0/fixieai/agents/llm_settings.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/agents/metadata.py` & `fixieai-1.0.0/fixieai/agents/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 @pydantic_dataclasses.dataclass
 class CodeShotAgentMetadata:
     """Metadata for a Fixie CodeShot Agent."""
 
     base_prompt: str
     few_shots: List[str]
-    corpora: Optional[List[fixie_corpora.DocumentCorpus]] = None
+    corpora: Optional[
+        List[Union[fixie_corpora.UrlDocumentCorpus, fixie_corpora.CustomCorpus]]
+    ] = None
     conversational: bool = False
     response_model: Optional[llm_settings.LlmSettings] = None
     type: Literal["code_shot"] = "code_shot"
 
 
 Metadata = Union[StandaloneAgentMetadata, CodeShotAgentMetadata]
```

### Comparing `fixieai-0.2.9/fixieai/agents/oauth.py` & `fixieai-1.0.0/fixieai/agents/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Dict, List, Optional
 from urllib import parse
 
 import dataclasses_json
 import requests
 
 from fixieai import constants
-from fixieai.agents import api
+from fixieai.agents import token
 from fixieai.agents import user_storage
 
 
 @dataclasses.dataclass
 class OAuthParams:
     """Encapsulates OAuth parameters, including secret, auth uri, and the scope.
 
@@ -66,20 +66,19 @@
     # OAuth keys reserved in UserStorage
     OAUTH_STATE_KEY = "_oauth_state"
     OAUTH_TOKEN_KEY = "_oauth_token"
 
     def __init__(
         self,
         oauth_params: OAuthParams,
-        query: api.AgentQuery,
-        agent_id: str,
+        token_claims: token.VerifiedTokenClaims,
     ):
-        self._storage = user_storage.UserStorage(query, agent_id)
+        self._storage = user_storage.UserStorage(token_claims)
         self._oauth_params = oauth_params
-        self._agent_id = agent_id
+        self._agent_id = token_claims.agent_id
 
     def get_authorization_url(self) -> str:
         """Returns a URL to launch the authorization flow."""
         auth_state = f"{self._agent_id}:{secrets.token_urlsafe()}"
         data = {
             "response_type": "code",
             "access_type": "offline",
```

### Comparing `fixieai-0.2.9/fixieai/agents/user_storage.py` & `fixieai-1.0.0/fixieai/agents/user_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import base64
 import json
-from typing import TYPE_CHECKING, Dict, List, MutableMapping, Union
+from typing import Dict, List, MutableMapping, Union
 
 import requests
 
 from fixieai import constants
-
-if TYPE_CHECKING:
-    from fixieai.agents.api import AgentQuery
+from fixieai.agents import exceptions
+from fixieai.agents import token
 
 UserStoragePrimitives = Union[bool, int, float, str, bytes, None]
 UserStorageType = Union[
     UserStoragePrimitives,
     List["UserStorageType"],
     Dict[str, "UserStorageType"],
 ]
 
 
 class UserStorage(MutableMapping[str, UserStorageType]):
     """UserStorage provides a dict-like interface to a user-specific storage.
 
     Usage:
-    >>> from fixieai import AgentQuery, Message
-    >>> query = AgentQuery(
-    ...   Message("incoming query"),
-    ...   access_token="fake-access-token"
-    ... )
-    >>> storage = UserStorage(query, "fake-agent")
+    >>> from fixieai.agents import token
+    >>> storage = UserStorage(token.VerifiedTokenClaims("fake-agent", False, "fake-access-token"))
     >>> storage["key"] = "value"
     >>> storage["complex-key"] = {"key1": {"key2": [12, False, None, b"binary"]}}
     >>> assert len(storage) == 2
     >>> assert storage["complex-key"]["key1"]["key2"][-1] == b"binary"
     """
 
     def __init__(
         self,
-        query: "AgentQuery",
-        agent_id: str,
+        token_claims: token.VerifiedTokenClaims,
         userstorage_url: str = constants.FIXIE_USER_STORAGE_URL,
     ):
-        # TODO(hessam): Remove agent_id from args once access_token includes agent_id
-        #  as well.
-        self._agent_id = agent_id
+        if token_claims.is_anonymous:
+            raise exceptions.AgentException(
+                response_message="I'm sorry, you must login to use this agent.",
+                error_code="ERR_USERSTORAGE_REQUIRES_USER",
+                error_message="This agent requires user storage, which is not available to anonymous users. Please login or create an account.",
+                http_status_code=400,
+            )
+
+        self._agent_id = token_claims.agent_id
         self._userstorage_url = userstorage_url
         self._session = requests.Session()
-        self._session.headers.update({"Authorization": f"Bearer {query.access_token}"})
+        self._session.headers.update({"Authorization": f"Bearer {token_claims.token}"})
 
     def __setitem__(self, key: str, value: UserStorageType):
         url = f"{self._userstorage_url}/{self._agent_id}/{key}"
         response = self._session.post(url, json={"data": to_json(value)})
         response.raise_for_status()
 
     def __getitem__(self, key: str) -> UserStorageType:
```

### Comparing `fixieai-0.2.9/fixieai/agents/user_storage_test.py` & `fixieai-1.0.0/fixieai/agents/user_storage_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import doctest
 import re
 
 import pytest
 
 from fixieai import constants
-from fixieai.agents import api
+from fixieai.agents import exceptions
+from fixieai.agents import token
 from fixieai.agents import user_storage
 
 FAKE_AGENT_ID = "fake-agent"
 FAKE_ACCESS_TOKEN = "fake-access-token"
 
 
 class MockUserStorageService:
@@ -77,18 +78,19 @@
     {"key": "value"},
     {"key1": {"key2": ["value1", True, b"binary2", None, 4.3]}},
 ]
 
 
 @pytest.mark.parametrize("test_value", VALUES_TO_TEST)
 def test_user_storage(mock_user_storage_urls, test_value):
-    query = api.AgentQuery(
-        message=api.Message("sample query"), access_token=FAKE_ACCESS_TOKEN
+    storage = user_storage.UserStorage(
+        token.VerifiedTokenClaims(
+            FAKE_AGENT_ID, is_anonymous=False, token=FAKE_ACCESS_TOKEN
+        )
     )
-    storage = user_storage.UserStorage(query, agent_id=FAKE_AGENT_ID)
 
     # Add the value and test its existence
     storage["key"] = test_value
     assert "key" in storage
     assert len(storage) == 1
     assert storage["key"] == test_value
     assert list(storage) == ["key"]
@@ -101,7 +103,16 @@
 
     val = storage.get("key", "default value")
     assert val == "default value"
 
 
 def test_doctest(mock_user_storage_urls):
     doctest.testmod(user_storage, raise_on_error=True)
+
+
+def test_userstorage_fails_for_anonymous_users():
+    with pytest.raises(exceptions.AgentException):
+        user_storage.UserStorage(
+            token.VerifiedTokenClaims(
+                FAKE_AGENT_ID, is_anonymous=True, token=FAKE_ACCESS_TOKEN
+            )
+        )
```

### Comparing `fixieai-0.2.9/fixieai/agents/utils.py` & `fixieai-1.0.0/fixieai/agents/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 from __future__ import annotations
 
 import enum
-import inspect
 import re
-from typing import TYPE_CHECKING, Callable, Optional, Set, get_type_hints
-from unittest import mock
-
-from fixieai.agents import agent_base
+from typing import TYPE_CHECKING, Callable, Optional, Set
 
 if TYPE_CHECKING:
-    from fixieai.agents import api
     from fixieai.agents import code_shot
-else:
-    api = mock.MagicMock()
-    code_shot = mock.MagicMock()
 
 ODD_NUM_POUNDS = re.compile(r"(?<!#)(##)*#(?!#)")
 EMBED_REF = re.compile(ODD_NUM_POUNDS.pattern + r"(?P<embed_key>\w+)(?!\w)")
 
 
 def strip_prompt_lines(agent: code_shot.CodeShotAgent):
     """Strips all prompt lines."""
@@ -31,87 +23,14 @@
     _validate_base_prompt(agent.base_prompt)
     for fewshot in agent.few_shots:
         _validate_few_shot_prompt(
             fewshot, agent.conversational, agent.is_valid_func_name
         )
 
 
-def validate_registered_pyfunc(func: Callable, agent: agent_base.AgentBase):
-    """Validates `func`'s signature to be a valid CodeShot Func.
-
-    Args:
-        func: The function to be validated.
-        agent: The CodeShotAgent that this func is going to be registered for.
-    """
-    # Delayed import to avoid circular dependency
-    from fixieai.agents import api
-    from fixieai.agents import oauth
-    from fixieai.agents import user_storage
-
-    ALLOWED_FUNC_PARAMS = {
-        "query": api.Message,
-        "user_storage": user_storage.UserStorage,
-        "oauth_handler": oauth.OAuthHandler,
-    }
-
-    # Validate that func is a function type.
-    if not inspect.isfunction(func):
-        raise TypeError(
-            f"Registered function {func!r} is not a function, but a {type(func)!r}."
-        )
-    signature = inspect.signature(func)
-    func_name = func.__name__
-    params = signature.parameters
-
-    # Validate that there are not var args (*args or **kwargs).
-    if any(
-        param.kind in (param.VAR_KEYWORD, param.VAR_POSITIONAL)
-        for param in params.values()
-    ):
-        raise TypeError(
-            f"Registered function {func_name} cannot accept variable args: {params!r}."
-        )
-
-    # Validate that all argument names are known.
-    unknown_params = set(params.keys()) - set(ALLOWED_FUNC_PARAMS.keys())
-    if unknown_params:
-        raise TypeError(
-            f"Registered function {func_name} gets unknown arguments {unknown_params}. "
-            f"List of allowed Func arguments are {list(ALLOWED_FUNC_PARAMS.keys())}."
-        )
-
-    # Check the type annotations match what's expected, if func is type annotated.
-    type_hints = get_type_hints(func)
-    for arg_name, arg_type in ALLOWED_FUNC_PARAMS.items():
-        if arg_name in type_hints and type_hints[arg_name] != arg_type:
-            raise TypeError(
-                f"Expected argument {arg_name!r} to be of type {arg_type!r}, but it's "
-                f"typed as {type_hints[arg_name]!r}."
-            )
-    if "return" in type_hints and type_hints["return"] not in (
-        api.AgentResponse,
-        api.Message,
-        str,
-    ):
-        raise TypeError(
-            f"Expected registered function to return an AgentResponse, a Message, "
-            f"or str but it returns {type_hints['return']}."
-        )
-
-    # Some custom checks.
-    if "oauth_handler" in params and agent.oauth_params is None:
-        raise TypeError(
-            f"Function {func_name} who accepts 'oauth_handler' as an argument cannot "
-            f"be registered with agent {agent!r} who hasn't set 'oauth_params' in its "
-            "constructor."
-        )
-
-    return func
-
-
 def _strip_all_lines(prompt: str) -> str:
     prompt = prompt.strip()
     return "\n".join(line.strip() for line in prompt.splitlines())
 
 
 def _validate_base_prompt(base_prompt: str):
     if base_prompt.endswith("\n") or base_prompt.startswith("\n"):
```

### Comparing `fixieai-0.2.9/fixieai/agents/utils_test.py` & `fixieai-1.0.0/fixieai/agents/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/cli/agent/loader.py` & `fixieai-1.0.0/fixieai/cli/agent/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import contextlib
 import functools
 import importlib
+import inspect
 import os
 import sys
 import threading
 import time
 from typing import Tuple
 
 import dotenv
 
 import fixieai
 from fixieai import agents
+from fixieai.agents import agent_func
+from fixieai.agents import openai_proxy
 from fixieai.cli.agent import agent_config
 
 
 @contextlib.contextmanager
 def _ensure_serving_disabled():
     original_serve = agents.AgentBase.serve
 
@@ -39,27 +42,39 @@
     config = agent_config.load_config(path)
     agent_dir = os.path.dirname(path) or "."
 
     dotenv_path = os.path.join(agent_dir, ".env")
     if os.path.exists(dotenv_path):
         dotenv.load_dotenv(dotenv_path)
 
+    openai_proxy.enable_openai_proxy()
+
     # Inject the agent directory into PYTHONPATH
     sys.path.insert(0, agent_dir)
 
     entry_point_parts = config.entry_point.split(":", 1)
     module_name = entry_point_parts[0]
     attr = entry_point_parts[1] if len(entry_point_parts) == 2 else "agent"
 
     with _ensure_serving_disabled():
         module = importlib.import_module(module_name)
-    agent_impl = getattr(module, attr)
-    assert isinstance(
-        agent_impl, agents.AgentBase
-    ), "Entrypoint must refer to an agent instance"
+    impl = getattr(module, attr)
+
+    if isinstance(impl, agents.AgentBase):
+        agent_impl = impl
+    elif isinstance(impl, agent_func.AgentFunc):
+        agent_impl = agents.StandaloneAgent(impl)
+    elif inspect.isfunction(impl):
+        func = agent_func.AgentQueryFunc.create(
+            impl, oauth_params=None, default_message_type=str, allow_generator=True
+        )
+        agent_impl = agents.StandaloneAgent(func)
+    else:
+        raise ValueError("Entrypoint must refer to an agent instance or function.")
+
     agent_impl.validate()
     return config, agent_impl
 
 
 def _refresh_agent_async(agent_handle: str):
     """Asynchronously pings Fixie to refresh the given agent_id."""
 
@@ -76,15 +91,17 @@
     """Returns an app that can be used to serve an agent with uvicorn.
 
     If the FIXIE_REFRESH_ON_STARTUP environment variable is set to "true" an agent refresh
     will be triggered each time the agent starts up.
     """
     config, impl = load_agent_from_path(".")
     fastapi_app = impl.app()
+    fastapi_app.add_middleware(openai_proxy.OpenAIProxyRequestTokenForwarderMiddleware)
 
+    # The CLI no longer uses this, but continue to honor it to preserve compatibility with CLI 0.2.x.
     if os.getenv("FIXIE_REFRESH_ON_STARTUP") == "true":
         fastapi_app.add_event_handler(
             "startup", functools.partial(_refresh_agent_async, config.handle)
         )
 
     return fastapi_app
```

### Comparing `fixieai-0.2.9/fixieai/cli/agent/tunnel.py` & `fixieai-1.0.0/fixieai/cli/agent/tunnel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import subprocess
 
 
 class Tunnel:
     """Start an Internet-accessible tunnel to the Agent running at the given host:port.
 
-    Returns the public URL on which the Agent can be contacted.
+    Returns a generator that yields public URLs on which the Agent can be contacted.
 
     Shuts down the tunnel when the context manager exits.
     """
 
     def __init__(self, port: int):
         self._port = port
 
@@ -31,22 +31,26 @@
                 "--output=json",
             ],
             stdin=subprocess.DEVNULL,
             stdout=subprocess.PIPE,
             stderr=subprocess.DEVNULL,
             encoding="utf-8",
         )
-        assert self._proc.stdout is not None
-        while True:
-            line = self._proc.stdout.readline()
-            if not line:
-                break
-            try:
-                parsed = json.loads(line)
-                if "address" in parsed:
-                    return f"https://{parsed['address']}"
-            except:
-                pass
+
+        def _gen():
+            while True:
+                assert self._proc.stdout is not None
+                line = self._proc.stdout.readline()
+                if not line:
+                    break
+                try:
+                    parsed = json.loads(line)
+                    if "address" in parsed:
+                        yield f"https://{parsed['address']}"
+                except:
+                    pass
+
+        return _gen()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._proc.terminate()
         self._proc.wait()
```

### Comparing `fixieai-0.2.9/fixieai/cli/auth/commands.py` & `fixieai-1.0.0/fixieai/cli/auth/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,19 @@
             click.secho(username, fg="green", nl=False, bold=True)
             click.echo(". Set --force to force re-authentication.")
             ctx.exit()
     except (FileNotFoundError, gql_exceptions.TransportQueryError):
         pass
 
 
+def _get_username(auth_token: str) -> str:
+    """Gets the username for an auth token."""
+    return client.FixieClient(auth_token).get_current_username()
+
+
 @click.command("auth", help="Authorizes `fixie` to access Fixie platform.")
 @click.option(
     "--force",
     is_flag=True,
     help="Forces authentication, even if the user is authenticated.",
     callback=validate_not_authed,
     expose_value=False,
@@ -44,10 +49,17 @@
 
     username = _get_username(fixie_auth_token)
     click.secho("Success! You're authenticated as ", fg="green", bold=True, nl=False)
     click.secho(username, fg="magenta", nl=False, bold=True)
     click.secho(".")
 
 
-def _get_username(auth_token: str) -> str:
-    """Gets the username for an auth token."""
-    return client.FixieClient(auth_token).get_current_username()
+@click.command("user", help="Displays information on the authenticated user.")
+@click.pass_context
+def user(ctx):
+    current_user = ctx.obj.client.get_current_user()
+    click.secho("You are authenticated to ", nl=False)
+    click.secho(ctx.obj.client.url, fg="yellow", nl=False)
+    click.secho(" as:")
+    for key, value in current_user.items():
+        click.secho(key, fg="green", nl=False)
+        click.echo(f": {value}")
```

### Comparing `fixieai-0.2.9/fixieai/cli/auth/oauth_flow.py` & `fixieai-1.0.0/fixieai/cli/auth/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/cli/auth/user_config.py` & `fixieai-1.0.0/fixieai/cli/auth/user_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/cli/auth/user_config_test.py` & `fixieai-1.0.0/fixieai/cli/auth/user_config_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/cli/session/console.py` & `fixieai-1.0.0/fixieai/cli/session/console.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, List, Optional
 
 import prompt_toolkit
 import prompt_toolkit.history
 import requests
 from PIL import Image
 from rich import console as rich_console
-from rich import markup
+from rich.markdown import Markdown
 
 from fixieai import FixieClient
 from fixieai.client.client import Session
 
 HISTORY_FILE = "~/.config/fixie/history.log"
 textconsole = rich_console.Console(soft_wrap=True)
 PROMPT = "fixie 🦊❯ "
@@ -76,26 +76,26 @@
         If show_user_message is set, the user messages are also printed with the PROMPT.
         This option is useful for showing previous messages in the chat when connecting
         to a session.
         """
         sender_handle = (
             message["sentBy"]["handle"] if message["sentBy"] else "<unknown>"
         )
+        message_text = message["text"]
+
         if message["type"] == "query" and sender_handle == "user":
             if show_user_message:
-                textconsole.print(f"{PROMPT}{markup.escape(message['text'])}")
+                textconsole.print(Markdown(PROMPT + message_text))
         elif message["type"] != "response":
             textconsole.print(
-                f"   [dim]@{sender_handle}: {markup.escape(message['text'])}[/]"
+                Markdown(f"   @{sender_handle}: " + message_text, style="dim")
             )
         else:
             self._response_index += 1
-            textconsole.print(
-                f"{self._response_index}❯ {markup.escape(message['text'])}"
-            )
+            textconsole.print(Markdown(f"{self._response_index}❯ " + message_text))
             self._show_embeds(message["text"])
 
     def _show_embeds(self, message: str):
         """Shows embeds referenced in `message_text`."""
         # Check embed references in message (denoted by #id).
         embed_ids = _extract_embed_refs(message)
         if not embed_ids:
```

### Comparing `fixieai-0.2.9/fixieai/cli/utils.py` & `fixieai-1.0.0/fixieai/cli/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/cli/utils_test.py` & `fixieai-1.0.0/fixieai/cli/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/client/agent.py` & `fixieai-1.0.0/fixieai/client/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import datetime
+import warnings
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from gql import gql
 
 if TYPE_CHECKING:
     import fixieai.client as fixie_client
 
@@ -30,14 +31,15 @@
         self._gqlclient = self._client.gqlclient
 
         self._agent_id = agent_id
         self._owner: Optional[str] = None
         if "/" in agent_id:
             self._owner, self._handle = agent_id.split("/")
         else:
+            self._owner = self._client.get_current_username()
             self._handle = agent_id
 
         self._metadata: Optional[Dict[str, Any]] = None
         try:
             self._metadata = self.get_metadata()
         except:
             self._metadata = None
@@ -102,18 +104,20 @@
             return None
         published = self._metadata["published"]
         assert published is None or isinstance(published, bool)
         return published
 
     @property
     def owner(self) -> Optional[str]:
-        """Return the owner of this Agent."""
+        """Return the owner of this Agent, which is either a username or an Organization handle."""
         if self._metadata is None:
             return None
-        owner_username = self._metadata["owner"]["username"]
+        owner_username = self._metadata["owner"].get("username") or self._metadata[
+            "owner"
+        ].get("handle")
         assert owner_username is None or isinstance(owner_username, str)
         return owner_username
 
     @property
     def query_url(self) -> Optional[str]:
         """Return the query URL for this Agent."""
         if self._metadata is None:
@@ -151,78 +155,50 @@
         if ts is not None:
             return datetime.datetime.fromisoformat(ts)
         else:
             return None
 
     def get_metadata(self) -> Dict[str, Any]:
         """Return metadata about this Agent."""
-
-        if self._owner is None:
-            # Query by handle.
-            query = gql(
-                """
-                query getAgentByHandle($handle: String!) {
-                    agentByHandle(handle: $handle) {
-                        agentId
-                        handle
-                        name
-                        description
-                        queries
-                        moreInfoUrl
-                        published
-                        owner {
-                            username
-                        }
-                        queryUrl
-                        funcUrl
-                        created
-                        modified
-                    }
-                }
+        query = gql(
             """
-            )
-            result = self._gqlclient.execute(
-                query, variable_values={"handle": self._handle}
-            )
-            if "agentByHandle" not in result or result["agentByHandle"] is None:
-                raise ValueError(f"Cannot fetch agent metadata for {self._handle}")
-            agent_dict = result["agentByHandle"]
-
-        else:
-            # Query by agent ID.
-            query = gql(
-                """
-                query getAgentById($agentId: String!) {
-                    agentById(agentId: $agentId) {
-                        agentId
-                        handle
-                        name
-                        description
-                        queries
-                        moreInfoUrl
-                        published
-                        owner {
+            query getAgentById($agentId: String!) {
+                agentById(agentId: $agentId) {
+                    agentId
+                    handle
+                    name
+                    description
+                    queries
+                    moreInfoUrl
+                    published
+                    owner {
+                        __typename
+                        ... on UserType {
                             username
                         }
-                        queryUrl
-                        funcUrl
-                        created
-                        modified
+                        ... on OrganizationType {
+                            handle
+                        }
                     }
+                    queryUrl
+                    funcUrl
+                    created
+                    modified
                 }
-            """
-            )
-            result = self._gqlclient.execute(
-                query, variable_values={"agentId": f"{self._owner}/{self._handle}"}
+            }
+        """
+        )
+        result = self._gqlclient.execute(
+            query, variable_values={"agentId": f"{self._owner}/{self._handle}"}
+        )
+        if "agentById" not in result or result["agentById"] is None:
+            raise ValueError(
+                f"Cannot fetch agent metadata for {self._owner}/{self._handle}"
             )
-            if "agentById" not in result or result["agentById"] is None:
-                raise ValueError(
-                    f"Cannot fetch agent metadata for {self._owner}/{self._handle}"
-                )
-            agent_dict = result["agentById"]
+        agent_dict = result["agentById"]
 
         assert isinstance(agent_dict, dict) and all(
             isinstance(k, str) for k in agent_dict.keys()
         )
         return agent_dict
 
     def create_agent(
@@ -267,14 +243,17 @@
         variable_values: Dict[str, Any] = {"handle": self._handle}
         if name is not None:
             variable_values["name"] = name
         variable_values["description"] = description
         if query_url is not None:
             variable_values["queryUrl"] = query_url
         if func_url is not None:
+            warnings.warn(
+                "Setting func_url via create_agent is deprecated, use FixieClient.create_agent_revision instead."
+            )
             variable_values["funcUrl"] = func_url
         if more_info_url is not None:
             variable_values["moreInfoUrl"] = more_info_url
         if published is not None:
             variable_values["published"] = published
 
         result = self._gqlclient.execute(query, variable_values=variable_values)
@@ -334,14 +313,17 @@
         if name is not None:
             variable_values["name"] = name
         if description is not None:
             variable_values["description"] = description
         if query_url is not None:
             variable_values["queryUrl"] = query_url
         if func_url is not None:
+            warnings.warn(
+                "Setting func_url via update_agent is deprecated, use FixieClient.create_agent_revision instead."
+            )
             variable_values["funcUrl"] = func_url
         if more_info_url is not None:
             variable_values["moreInfoUrl"] = more_info_url
         if published is not None:
             variable_values["published"] = published
 
         result = self._gqlclient.execute(query, variable_values=variable_values)
@@ -355,17 +337,19 @@
             self._handle = new_handle
         return result["updateAgent"]["agent"]["agentId"]
 
     def delete_agent(self) -> None:
         """Delete this Agent."""
         query = gql(
             """
-            mutation DeleteAgent($handle: String!) {
-                deleteAgent(handle: $handle) {
+            mutation DeleteAgent($owner: String!, $handle: String!) {
+                deleteAgent(agentData: {owner: $owner, handle: $handle}) {
                     agent {
                         handle
                     }
                 }
             }
         """
         )
-        _ = self._gqlclient.execute(query, variable_values={"handle": self._handle})
+        _ = self._gqlclient.execute(
+            query, variable_values={"owner": self.owner, "handle": self._handle}
+        )
```

### Comparing `fixieai-0.2.9/fixieai/client/client_test.py` & `fixieai-1.0.0/fixieai/client/client_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/client/session.py` & `fixieai-1.0.0/fixieai/client/session.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.9/fixieai/constants.py` & `fixieai-1.0.0/fixieai/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,20 @@
 # Fixie's OAuth redirect endpoint. Tokens sent to this endpoint will be redirected back
 # to your agent.
 FIXIE_OAUTH_REDIRECT_URL = f"{FIXIE_API_URL}/oauth"
 # Fixie's deployments service URL.
 FIXIE_DEPLOYMENT_URL = f"{FIXIE_API_URL}/api/deployments"
 # Fixie's JWKS URL.
 FIXIE_JWKS_URL = f"{FIXIE_API_URL}/.well-known/jwks.json"
+# Fixie's OpenAI Proxy URL.
+FIXIE_OPENAI_PROXY_URL = f"{FIXIE_API_URL}/api/openai-proxy/v1"
 # Valid audiences for Fixie's query JWTs.
 FIXIE_AGENT_API_AUDIENCES = ["https://app.fixie.ai/api", "https://app.dev.fixie.ai/api"]
+# Fixie Agents' URL
+FIXIE_AGENT_URL = f"{FIXIE_API_URL}/agents"
 
 
 def fixie_api_key() -> str:
     """Returns authenticated user's fixie auth token.
 
     User may authenticate via `fixie auth`, or by setting FIXIE_API_KEY environment
     variable to override any previous authentication.
```

### Comparing `fixieai-0.2.9/pyproject.toml` & `fixieai-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixieai"
-version = "0.2.9"
+version = "1.0.0"
 description = "SDK for the Fixie.ai platform. See: https://fixie.ai"
 authors = ["Fixie.ai Team <hello@fixie.ai>"]
 packages = [
     { include = "fixieai/" },
 ]
 
 [build-system]
@@ -16,26 +16,31 @@
 fixie = "fixieai.cli.cli:fixie"
 fixieai = "fixieai.cli.cli:fixie"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 fastapi = { version = "^0.89.1" }
 uvicorn = { version = "^0.20.0", extras = ["standard"] }
-gql = { version = "^3.4.0", extras = ["requests"] }
+gql = { version = "^3.4.1", extras = ["requests"] }
 python = "^3.8"
 prompt-toolkit = "*"
-pydantic = "*"
+pydantic = ">=1.10.8"
 PyJWT = { version = "^2.6.0", extras = ["crypto"] }
 requests = "^2.28.1"
 rich = "^12.6.0"
 dataclasses-json = "^0.5.7"
 validators = "^0.20.0"
 oauth2-client = "^1.3.0"
 Pillow = "*"
 python-dotenv = "^1.0.0"
+packaging = "^23.0"
+wrapt = "^1.15.0"
+watchfiles = "^0.19.0"
+Deprecated = "^1.2.13"
+types-Deprecated = "^1.2.9.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-mock = "3.10.0"
 pytest-xdist = "3.0.2"
 black = "22.8.0"
 isort = "5.10.1"
@@ -45,14 +50,15 @@
 mkdocs = "^1.4.2"
 mkdocstrings = { version = "^0.20.0", extras = ["python"] }
 mkdocs-click = "^0.8.0"
 mkdocs-material = "^7.3"
 mkdocs-windmill = "^1.0.5"
 mkdocs-cinder = "^1.2.0"
 fastapi = { version = "^0.89.1", extras = ["all"] }
+types-setuptools = "^67.6.0.7"
 
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `fixieai-0.2.9/setup.py` & `fixieai-1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,36 +10,41 @@
  'fixieai.cli.session',
  'fixieai.client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Pillow',
+['Deprecated>=1.2.13,<2.0.0',
+ 'Pillow',
  'PyJWT[crypto]>=2.6.0,<3.0.0',
  'click>=8.1.3,<9.0.0',
  'dataclasses-json>=0.5.7,<0.6.0',
  'fastapi>=0.89.1,<0.90.0',
- 'gql[requests]>=3.4.0,<4.0.0',
+ 'gql[requests]>=3.4.1,<4.0.0',
  'oauth2-client>=1.3.0,<2.0.0',
+ 'packaging>=23.0,<24.0',
  'prompt-toolkit',
- 'pydantic',
+ 'pydantic>=1.10.8',
  'python-dotenv>=1.0.0,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=12.6.0,<13.0.0',
+ 'types-Deprecated>=1.2.9.2,<2.0.0.0',
  'uvicorn[standard]>=0.20.0,<0.21.0',
- 'validators>=0.20.0,<0.21.0']
+ 'validators>=0.20.0,<0.21.0',
+ 'watchfiles>=0.19.0,<0.20.0',
+ 'wrapt>=1.15.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['fixie = fixieai.cli.cli:fixie',
                      'fixieai = fixieai.cli.cli:fixie']}
 
 setup_kwargs = {
     'name': 'fixieai',
-    'version': '0.2.9',
+    'version': '1.0.0',
     'description': 'SDK for the Fixie.ai platform. See: https://fixie.ai',
     'long_description': 'None',
     'author': 'Fixie.ai Team',
     'author_email': 'hello@fixie.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fixieai-0.2.9/PKG-INFO` & `fixieai-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: fixieai
-Version: 0.2.9
+Version: 1.0.0
 Summary: SDK for the Fixie.ai platform. See: https://fixie.ai
 Author: Fixie.ai Team
 Author-email: hello@fixie.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: Pillow
 Requires-Dist: PyJWT[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: fastapi (>=0.89.1,<0.90.0)
-Requires-Dist: gql[requests] (>=3.4.0,<4.0.0)
+Requires-Dist: gql[requests] (>=3.4.1,<4.0.0)
 Requires-Dist: oauth2-client (>=1.3.0,<2.0.0)
+Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: prompt-toolkit
-Requires-Dist: pydantic
+Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: types-Deprecated (>=1.2.9.2,<2.0.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
```

