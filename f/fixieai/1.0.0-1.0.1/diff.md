# Comparing `tmp/fixieai-1.0.0.tar.gz` & `tmp/fixieai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixieai-1.0.0.tar", max compression
+gzip compressed data, was "fixieai-1.0.1.tar", max compression
```

## Comparing `fixieai-1.0.0.tar` & `fixieai-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-02-07 23:45:43.683245 fixieai-1.0.0/LICENSE
--rw-r--r--   0        0        0     1388 2023-06-05 22:24:43.848602 fixieai-1.0.0/fixieai/__init__.py
--rw-r--r--   0        0        0     1301 2023-06-05 22:24:43.848729 fixieai-1.0.0/fixieai/agents/__init__.py
--rw-r--r--   0        0        0    10564 2023-06-05 22:24:43.849458 fixieai-1.0.0/fixieai/agents/agent_base.py
--rw-r--r--   0        0        0    12042 2023-06-05 22:24:43.849590 fixieai-1.0.0/fixieai/agents/agent_base_test.py
--rw-r--r--   0        0        0    15267 2023-06-05 22:24:43.849720 fixieai-1.0.0/fixieai/agents/agent_func.py
--rw-r--r--   0        0        0     8715 2023-06-05 22:24:43.849847 fixieai-1.0.0/fixieai/agents/agent_func_test.py
--rw-r--r--   0        0        0     2965 2023-06-05 22:24:43.849947 fixieai-1.0.0/fixieai/agents/api.py
--rw-r--r--   0        0        0      863 2023-03-09 19:26:37.964207 fixieai-1.0.0/fixieai/agents/api_test.py
--rw-r--r--   0        0        0     3786 2023-06-05 22:24:43.850060 fixieai-1.0.0/fixieai/agents/code_shot.py
--rw-r--r--   0        0        0     3306 2023-06-05 22:24:43.850149 fixieai-1.0.0/fixieai/agents/code_shot_test.py
--rw-r--r--   0        0        0     7152 2023-06-05 22:24:43.850261 fixieai-1.0.0/fixieai/agents/corpora.py
--rw-r--r--   0        0        0     1943 2023-06-05 22:24:43.850315 fixieai-1.0.0/fixieai/agents/corpora_test.py
--rw-r--r--   0        0        0     2279 2023-06-05 22:24:43.850379 fixieai-1.0.0/fixieai/agents/exceptions.py
--rw-r--r--   0        0        0     1046 2023-03-30 16:24:35.974599 fixieai-1.0.0/fixieai/agents/llm_settings.py
--rw-r--r--   0        0        0      891 2023-06-05 22:24:43.850459 fixieai-1.0.0/fixieai/agents/metadata.py
--rw-r--r--   0        0        0     9000 2023-06-05 22:24:43.850566 fixieai-1.0.0/fixieai/agents/oauth.py
--rw-r--r--   0        0        0     4048 2023-04-25 03:00:21.707100 fixieai-1.0.0/fixieai/agents/openai_proxy.py
--rw-r--r--   0        0        0     1627 2023-04-25 03:00:21.707249 fixieai-1.0.0/fixieai/agents/openai_proxy_test.py
--rw-r--r--   0        0        0     2439 2023-06-05 22:24:43.850673 fixieai-1.0.0/fixieai/agents/standalone.py
--rw-r--r--   0        0        0     4414 2023-06-05 22:24:43.850780 fixieai-1.0.0/fixieai/agents/standalone_test.py
--rw-r--r--   0        0        0     1918 2023-06-05 22:24:43.850853 fixieai-1.0.0/fixieai/agents/token.py
--rw-r--r--   0        0        0     4951 2023-06-05 22:24:43.850975 fixieai-1.0.0/fixieai/agents/user_storage.py
--rw-r--r--   0        0        0     3388 2023-06-05 22:24:43.851664 fixieai-1.0.0/fixieai/agents/user_storage_test.py
--rw-r--r--   0        0        0     7966 2023-04-25 03:00:21.707832 fixieai-1.0.0/fixieai/agents/utils.py
--rw-r--r--   0        0        0     5253 2023-03-25 02:35:27.951289 fixieai-1.0.0/fixieai/agents/utils_test.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.965971 fixieai-1.0.0/fixieai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.966917 fixieai-1.0.0/fixieai/cli/agent/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-05 22:24:43.852159 fixieai-1.0.0/fixieai/cli/agent/agent_config.py
--rw-r--r--   0        0        0    34827 2023-06-05 22:24:43.852447 fixieai-1.0.0/fixieai/cli/agent/commands.py
--rw-r--r--   0        0        0    16037 2023-06-05 22:45:51.414577 fixieai-1.0.0/fixieai/cli/agent/commands_test.py
--rw-r--r--   0        0        0     3488 2023-06-05 22:24:43.852973 fixieai-1.0.0/fixieai/cli/agent/loader.py
--rw-r--r--   0        0        0     1753 2023-04-01 03:10:09.936255 fixieai-1.0.0/fixieai/cli/agent/tunnel.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.967623 fixieai-1.0.0/fixieai/cli/auth/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-01 23:07:48.256193 fixieai-1.0.0/fixieai/cli/auth/commands.py
--rw-r--r--   0        0        0     1942 2023-03-09 19:26:37.968039 fixieai-1.0.0/fixieai/cli/auth/oauth_flow.py
--rw-r--r--   0        0        0     2667 2023-03-30 16:24:35.975821 fixieai-1.0.0/fixieai/cli/auth/user_config.py
--rw-r--r--   0        0        0     2120 2023-03-30 16:24:35.975913 fixieai-1.0.0/fixieai/cli/auth/user_config_test.py
--rwxr-xr-x   0        0        0     3290 2023-04-12 15:22:13.299089 fixieai-1.0.0/fixieai/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-09 19:26:37.968257 fixieai-1.0.0/fixieai/cli/session/__init__.py
--rw-r--r--   0        0        0     4761 2023-04-12 01:22:58.394077 fixieai-1.0.0/fixieai/cli/session/commands.py
--rw-r--r--   0        0        0     4720 2023-06-05 22:24:43.853234 fixieai-1.0.0/fixieai/cli/session/console.py
--rw-r--r--   0        0        0     1523 2023-03-30 16:24:35.976029 fixieai-1.0.0/fixieai/cli/utils.py
--rw-r--r--   0        0        0      655 2023-03-22 17:59:48.856855 fixieai-1.0.0/fixieai/cli/utils_test.py
--rw-r--r--   0        0        0      322 2023-03-09 19:26:37.968576 fixieai-1.0.0/fixieai/client/__init__.py
--rw-r--r--   0        0        0    11895 2023-06-06 15:54:00.163441 fixieai-1.0.0/fixieai/client/agent.py
--rwxr-xr-x   0        0        0    12607 2023-06-05 22:39:38.544081 fixieai-1.0.0/fixieai/client/client.py
--rw-r--r--   0        0        0     4987 2023-03-10 17:44:40.327464 fixieai-1.0.0/fixieai/client/client_test.py
--rwxr-xr-x   0        0        0     8750 2023-03-10 05:45:43.499628 fixieai-1.0.0/fixieai/client/session.py
--rw-r--r--   0        0        0     1402 2023-06-05 22:24:43.853545 fixieai-1.0.0/fixieai/client/utils.py
--rw-r--r--   0        0        0     2394 2023-06-05 22:24:43.853647 fixieai-1.0.0/fixieai/constants.py
--rw-r--r--   0        0        0     2026 2023-06-13 15:28:51.610689 fixieai-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 fixieai-1.0.0/setup.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 fixieai-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-07 23:45:43.683245 fixieai-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1388 2023-06-05 22:24:43.848602 fixieai-1.0.1/fixieai/__init__.py
+-rw-r--r--   0        0        0     1301 2023-06-05 22:24:43.848729 fixieai-1.0.1/fixieai/agents/__init__.py
+-rw-r--r--   0        0        0    10564 2023-06-05 22:24:43.849458 fixieai-1.0.1/fixieai/agents/agent_base.py
+-rw-r--r--   0        0        0    12042 2023-06-05 22:24:43.849590 fixieai-1.0.1/fixieai/agents/agent_base_test.py
+-rw-r--r--   0        0        0    15267 2023-06-05 22:24:43.849720 fixieai-1.0.1/fixieai/agents/agent_func.py
+-rw-r--r--   0        0        0     8715 2023-06-05 22:24:43.849847 fixieai-1.0.1/fixieai/agents/agent_func_test.py
+-rw-r--r--   0        0        0     2965 2023-06-05 22:24:43.849947 fixieai-1.0.1/fixieai/agents/api.py
+-rw-r--r--   0        0        0      863 2023-03-09 19:26:37.964207 fixieai-1.0.1/fixieai/agents/api_test.py
+-rw-r--r--   0        0        0     3786 2023-06-05 22:24:43.850060 fixieai-1.0.1/fixieai/agents/code_shot.py
+-rw-r--r--   0        0        0     3306 2023-06-05 22:24:43.850149 fixieai-1.0.1/fixieai/agents/code_shot_test.py
+-rw-r--r--   0        0        0     7152 2023-06-05 22:24:43.850261 fixieai-1.0.1/fixieai/agents/corpora.py
+-rw-r--r--   0        0        0     1943 2023-06-05 22:24:43.850315 fixieai-1.0.1/fixieai/agents/corpora_test.py
+-rw-r--r--   0        0        0     2279 2023-06-05 22:24:43.850379 fixieai-1.0.1/fixieai/agents/exceptions.py
+-rw-r--r--   0        0        0     1046 2023-03-30 16:24:35.974599 fixieai-1.0.1/fixieai/agents/llm_settings.py
+-rw-r--r--   0        0        0      891 2023-06-05 22:24:43.850459 fixieai-1.0.1/fixieai/agents/metadata.py
+-rw-r--r--   0        0        0     9000 2023-06-05 22:24:43.850566 fixieai-1.0.1/fixieai/agents/oauth.py
+-rw-r--r--   0        0        0     4048 2023-04-25 03:00:21.707100 fixieai-1.0.1/fixieai/agents/openai_proxy.py
+-rw-r--r--   0        0        0     1627 2023-04-25 03:00:21.707249 fixieai-1.0.1/fixieai/agents/openai_proxy_test.py
+-rw-r--r--   0        0        0     2439 2023-06-05 22:24:43.850673 fixieai-1.0.1/fixieai/agents/standalone.py
+-rw-r--r--   0        0        0     4414 2023-06-05 22:24:43.850780 fixieai-1.0.1/fixieai/agents/standalone_test.py
+-rw-r--r--   0        0        0     1918 2023-06-05 22:24:43.850853 fixieai-1.0.1/fixieai/agents/token.py
+-rw-r--r--   0        0        0     4951 2023-06-05 22:24:43.850975 fixieai-1.0.1/fixieai/agents/user_storage.py
+-rw-r--r--   0        0        0     3388 2023-06-05 22:24:43.851664 fixieai-1.0.1/fixieai/agents/user_storage_test.py
+-rw-r--r--   0        0        0     7966 2023-04-25 03:00:21.707832 fixieai-1.0.1/fixieai/agents/utils.py
+-rw-r--r--   0        0        0     5253 2023-03-25 02:35:27.951289 fixieai-1.0.1/fixieai/agents/utils_test.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.965971 fixieai-1.0.1/fixieai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.966917 fixieai-1.0.1/fixieai/cli/agent/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-05 22:24:43.852159 fixieai-1.0.1/fixieai/cli/agent/agent_config.py
+-rw-r--r--   0        0        0    35054 2023-06-13 15:56:30.159010 fixieai-1.0.1/fixieai/cli/agent/commands.py
+-rw-r--r--   0        0        0    16037 2023-06-13 15:44:25.677117 fixieai-1.0.1/fixieai/cli/agent/commands_test.py
+-rw-r--r--   0        0        0     3488 2023-06-05 22:24:43.852973 fixieai-1.0.1/fixieai/cli/agent/loader.py
+-rw-r--r--   0        0        0     1753 2023-04-01 03:10:09.936255 fixieai-1.0.1/fixieai/cli/agent/tunnel.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.967623 fixieai-1.0.1/fixieai/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-01 23:07:48.256193 fixieai-1.0.1/fixieai/cli/auth/commands.py
+-rw-r--r--   0        0        0     1942 2023-03-09 19:26:37.968039 fixieai-1.0.1/fixieai/cli/auth/oauth_flow.py
+-rw-r--r--   0        0        0     2667 2023-03-30 16:24:35.975821 fixieai-1.0.1/fixieai/cli/auth/user_config.py
+-rw-r--r--   0        0        0     2120 2023-03-30 16:24:35.975913 fixieai-1.0.1/fixieai/cli/auth/user_config_test.py
+-rwxr-xr-x   0        0        0     3290 2023-04-12 15:22:13.299089 fixieai-1.0.1/fixieai/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:26:37.968257 fixieai-1.0.1/fixieai/cli/session/__init__.py
+-rw-r--r--   0        0        0     4761 2023-04-12 01:22:58.394077 fixieai-1.0.1/fixieai/cli/session/commands.py
+-rw-r--r--   0        0        0     4720 2023-06-05 22:24:43.853234 fixieai-1.0.1/fixieai/cli/session/console.py
+-rw-r--r--   0        0        0     1523 2023-03-30 16:24:35.976029 fixieai-1.0.1/fixieai/cli/utils.py
+-rw-r--r--   0        0        0      655 2023-03-22 17:59:48.856855 fixieai-1.0.1/fixieai/cli/utils_test.py
+-rw-r--r--   0        0        0      322 2023-03-09 19:26:37.968576 fixieai-1.0.1/fixieai/client/__init__.py
+-rw-r--r--   0        0        0    11895 2023-06-13 15:44:25.677595 fixieai-1.0.1/fixieai/client/agent.py
+-rwxr-xr-x   0        0        0    12607 2023-06-13 15:56:45.258897 fixieai-1.0.1/fixieai/client/client.py
+-rw-r--r--   0        0        0     4987 2023-03-10 17:44:40.327464 fixieai-1.0.1/fixieai/client/client_test.py
+-rwxr-xr-x   0        0        0     8750 2023-03-10 05:45:43.499628 fixieai-1.0.1/fixieai/client/session.py
+-rw-r--r--   0        0        0     1402 2023-06-05 22:24:43.853545 fixieai-1.0.1/fixieai/client/utils.py
+-rw-r--r--   0        0        0     2394 2023-06-05 22:24:43.853647 fixieai-1.0.1/fixieai/constants.py
+-rw-r--r--   0        0        0     2026 2023-06-13 16:02:31.198419 fixieai-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 fixieai-1.0.1/setup.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 fixieai-1.0.1/PKG-INFO
```

### Comparing `fixieai-1.0.0/LICENSE` & `fixieai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/__init__.py` & `fixieai-1.0.1/fixieai/__init__.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/__init__.py` & `fixieai-1.0.1/fixieai/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/agent_base.py` & `fixieai-1.0.1/fixieai/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/agent_base_test.py` & `fixieai-1.0.1/fixieai/agents/agent_base_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/agent_func.py` & `fixieai-1.0.1/fixieai/agents/agent_func.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/agent_func_test.py` & `fixieai-1.0.1/fixieai/agents/agent_func_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/api.py` & `fixieai-1.0.1/fixieai/agents/api.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/api_test.py` & `fixieai-1.0.1/fixieai/agents/api_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/code_shot.py` & `fixieai-1.0.1/fixieai/agents/code_shot.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/code_shot_test.py` & `fixieai-1.0.1/fixieai/agents/code_shot_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/corpora.py` & `fixieai-1.0.1/fixieai/agents/corpora.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/corpora_test.py` & `fixieai-1.0.1/fixieai/agents/corpora_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/exceptions.py` & `fixieai-1.0.1/fixieai/agents/exceptions.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/llm_settings.py` & `fixieai-1.0.1/fixieai/agents/llm_settings.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/metadata.py` & `fixieai-1.0.1/fixieai/agents/metadata.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/oauth.py` & `fixieai-1.0.1/fixieai/agents/oauth.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/openai_proxy.py` & `fixieai-1.0.1/fixieai/agents/openai_proxy.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/openai_proxy_test.py` & `fixieai-1.0.1/fixieai/agents/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/standalone.py` & `fixieai-1.0.1/fixieai/agents/standalone.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/standalone_test.py` & `fixieai-1.0.1/fixieai/agents/standalone_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/token.py` & `fixieai-1.0.1/fixieai/agents/token.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/user_storage.py` & `fixieai-1.0.1/fixieai/agents/user_storage.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/user_storage_test.py` & `fixieai-1.0.1/fixieai/agents/user_storage_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/utils.py` & `fixieai-1.0.1/fixieai/agents/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/agents/utils_test.py` & `fixieai-1.0.1/fixieai/agents/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/agent/agent_config.py` & `fixieai-1.0.1/fixieai/cli/agent/agent_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/agent/commands.py` & `fixieai-1.0.1/fixieai/cli/agent/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,16 @@
     if agent.more_info_url:
         click.echo(f"More info URL: {agent.more_info_url}")
     click.echo(f"Published: {agent.published}")
     click.echo(f"Created: {agent.created}")
     click.echo(f"Modified: {agent.modified}")
     if agent.queries:
         click.echo(f"Queries: {agent.queries}")
+    current_revision = client.get_current_agent_revision(agent_id)
+    click.echo(f"Current revision: {current_revision}")
 
 
 @agent.command("delete", help="Delete an agent.")
 @click.argument("handle")
 @click.pass_context
 def delete_agent(ctx, handle: str):
     client = ctx.obj.client
@@ -373,15 +375,17 @@
 @contextlib.contextmanager
 def _temporary_revision_replacer(
     console: rich.console.Console, client: fixieai.FixieClient, agent_handle: str
 ):
     """Yields a function that can be used to temporarily replace an agent's current revision."""
 
     # Get the preexisting revision so that we can restore it when we're done.
-    existing_revision_id = client.get_current_agent_revision(agent_handle)
+    existing_revision_id = client.get_current_agent_revision(
+        client.get_current_username() + "/" + agent_handle
+    )
     current_temporary_revision: Optional[str] = None
 
     if existing_revision_id is not None:
         console.print(
             f"[yellow]This temporarily replaces existing revision {existing_revision_id}.[/yellow]"
         )
 
@@ -1009,15 +1013,17 @@
 @click.pass_context
 def delete_revision(ctx, path, id, force):
     console = rich_console.Console(soft_wrap=True)
     config = agent_config.load_config(path)
 
     client: fixieai.FixieClient = ctx.obj.client
 
-    current_revision = client.get_current_agent_revision(config.handle)
+    current_revision = client.get_current_agent_revision(
+        client.get_current_username() + "/" + config.handle
+    )
     if current_revision == id:
         if not force:
             console.print(
                 f"Not deleting revision {id} because it is the current revision. (Use --force to delete it anyway.)",
                 style="red",
             )
             raise click.exceptions.Exit(1)
```

### Comparing `fixieai-1.0.0/fixieai/cli/agent/commands_test.py` & `fixieai-1.0.1/fixieai/cli/agent/commands_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/agent/loader.py` & `fixieai-1.0.1/fixieai/cli/agent/loader.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/agent/tunnel.py` & `fixieai-1.0.1/fixieai/cli/agent/tunnel.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/auth/commands.py` & `fixieai-1.0.1/fixieai/cli/auth/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/auth/oauth_flow.py` & `fixieai-1.0.1/fixieai/cli/auth/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/auth/user_config.py` & `fixieai-1.0.1/fixieai/cli/auth/user_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/auth/user_config_test.py` & `fixieai-1.0.1/fixieai/cli/auth/user_config_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/cli.py` & `fixieai-1.0.1/fixieai/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/session/commands.py` & `fixieai-1.0.1/fixieai/cli/session/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/session/console.py` & `fixieai-1.0.1/fixieai/cli/session/console.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/utils.py` & `fixieai-1.0.1/fixieai/cli/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/cli/utils_test.py` & `fixieai-1.0.1/fixieai/cli/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/client/agent.py` & `fixieai-1.0.1/fixieai/client/agent.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/client/client.py` & `fixieai-1.0.1/fixieai/client/client.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/client/client_test.py` & `fixieai-1.0.1/fixieai/client/client_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/client/session.py` & `fixieai-1.0.1/fixieai/client/session.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/client/utils.py` & `fixieai-1.0.1/fixieai/client/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/fixieai/constants.py` & `fixieai-1.0.1/fixieai/constants.py`

 * *Files identical despite different names*

### Comparing `fixieai-1.0.0/pyproject.toml` & `fixieai-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixieai"
-version = "1.0.0"
+version = "1.0.1"
 description = "SDK for the Fixie.ai platform. See: https://fixie.ai"
 authors = ["Fixie.ai Team <hello@fixie.ai>"]
 packages = [
     { include = "fixieai/" },
 ]
 
 [build-system]
```

### Comparing `fixieai-1.0.0/setup.py` & `fixieai-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 entry_points = \
 {'console_scripts': ['fixie = fixieai.cli.cli:fixie',
                      'fixieai = fixieai.cli.cli:fixie']}
 
 setup_kwargs = {
     'name': 'fixieai',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'SDK for the Fixie.ai platform. See: https://fixie.ai',
     'long_description': 'None',
     'author': 'Fixie.ai Team',
     'author_email': 'hello@fixie.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fixieai-1.0.0/PKG-INFO` & `fixieai-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixieai
-Version: 1.0.0
+Version: 1.0.1
 Summary: SDK for the Fixie.ai platform. See: https://fixie.ai
 Author: Fixie.ai Team
 Author-email: hello@fixie.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

