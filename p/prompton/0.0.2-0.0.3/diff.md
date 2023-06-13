# Comparing `tmp/prompton-0.0.2.tar.gz` & `tmp/prompton-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompton-0.0.2.tar", max compression
+gzip compressed data, was "prompton-0.0.3.tar", max compression
```

## Comparing `prompton-0.0.2.tar` & `prompton-0.0.3.tar`

### file list

```diff
@@ -1,63 +1,66 @@
--rw-r--r--   0        0        0      100 2023-06-11 19:50:26.478999 prompton-0.0.2/README.md
--rw-r--r--   0        0        0     2214 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/client.py
--rw-r--r--   0        0        0      348 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      367 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/unauthorized_error.py
--rw-r--r--   0        0        0      257 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      268 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/authentication/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/authentication/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/inferences/__init__.py
--rw-r--r--   0        0        0    11315 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/inferences/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/orgs/__init__.py
--rw-r--r--   0        0        0    14700 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/orgs/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompt_versions/__init__.py
--rw-r--r--   0        0        0    16684 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompt_versions/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompts/__init__.py
--rw-r--r--   0        0        0    15826 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/server_status/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/server_status/client.py
--rw-r--r--   0        0        0       65 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/users/__init__.py
--rw-r--r--   0        0        0    13165 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/resources/users/client.py
--rw-r--r--   0        0        0     2747 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/__init__.py
--rw-r--r--   0        0        0      900 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/api_status_response.py
--rw-r--r--   0        0        0      936 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/body_get_access_token_extended_token_post.py
--rw-r--r--   0        0        0     1233 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_config.py
--rw-r--r--   0        0        0      152 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_config_stop.py
--rw-r--r--   0        0        0     1417 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_request.py
--rw-r--r--   0        0        0      153 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_request_stop.py
--rw-r--r--   0        0        0     1012 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_chat_completition_response.py
--rw-r--r--   0        0        0      856 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_completition_choice.py
--rw-r--r--   0        0        0      843 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_message.py
--rw-r--r--   0        0        0      666 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_role.py
--rw-r--r--   0        0        0      809 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/chat_gpt_token_usage.py
--rw-r--r--   0        0        0      773 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/db_status.py
--rw-r--r--   0        0        0      843 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/http_validation_error.py
--rw-r--r--   0        0        0      926 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_post_response.py
--rw-r--r--   0        0        0      293 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_post_response_response.py
--rw-r--r--   0        0        0     1687 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_read.py
--rw-r--r--   0        0        0      285 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_read_response.py
--rw-r--r--   0        0        0      965 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_request_data.py
--rw-r--r--   0        0        0     1308 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_response_data.py
--rw-r--r--   0        0        0     1051 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_response_error.py
--rw-r--r--   0        0        0     1049 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/inference_response_status.py
--rw-r--r--   0        0        0     1076 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/org_read.py
--rw-r--r--   0        0        0     1143 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_read.py
--rw-r--r--   0        0        0      507 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_status.py
--rw-r--r--   0        0        0      411 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_version_providers.py
--rw-r--r--   0        0        0     1610 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_version_read.py
--rw-r--r--   0        0        0      837 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/prompt_version_status.py
--rw-r--r--   0        0        0      767 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/token.py
--rw-r--r--   0        0        0     1181 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/user_read.py
--rw-r--r--   0        0        0      686 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/user_roles.py
--rw-r--r--   0        0        0      869 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-11 18:13:36.000000 prompton-0.0.2/prompton/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      451 2023-06-11 20:06:50.881065 prompton-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 prompton-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.3/README.md
+-rw-r--r--   0        0        0     2408 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/client.py
+-rw-r--r--   0        0        0      348 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      367 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      257 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      268 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/authentication/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/authentication/client.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/inferences/__init__.py
+-rw-r--r--   0        0        0     9839 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/inferences/client.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/orgs/__init__.py
+-rw-r--r--   0        0        0    14700 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/orgs/client.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompt_versions/__init__.py
+-rw-r--r--   0        0        0    16684 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompt_versions/client.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    15826 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/server_status/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/server_status/client.py
+-rw-r--r--   0        0        0       65 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/users/__init__.py
+-rw-r--r--   0        0        0    13165 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/resources/users/client.py
+-rw-r--r--   0        0        0     3055 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/api_status_response.py
+-rw-r--r--   0        0        0      936 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/body_get_access_token_extended_token_post.py
+-rw-r--r--   0        0        0     1274 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_config.py
+-rw-r--r--   0        0        0      152 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_config_stop.py
+-rw-r--r--   0        0        0     1458 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_request.py
+-rw-r--r--   0        0        0      153 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_request_stop.py
+-rw-r--r--   0        0        0     1012 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_chat_completition_response.py
+-rw-r--r--   0        0        0      856 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_completition_choice.py
+-rw-r--r--   0        0        0      843 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_message.py
+-rw-r--r--   0        0        0      666 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_role.py
+-rw-r--r--   0        0        0      809 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/chat_gpt_token_usage.py
+-rw-r--r--   0        0        0      773 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/db_status.py
+-rw-r--r--   0        0        0      843 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/http_validation_error.py
+-rw-r--r--   0        0        0     1556 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_create_by_prompt_id.py
+-rw-r--r--   0        0        0     1156 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_create_by_prompt_version_id.py
+-rw-r--r--   0        0        0      926 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_post_response.py
+-rw-r--r--   0        0        0      293 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_post_response_response.py
+-rw-r--r--   0        0        0     2081 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_read.py
+-rw-r--r--   0        0        0      285 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_read_response.py
+-rw-r--r--   0        0        0      965 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_request_data.py
+-rw-r--r--   0        0        0     1308 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_response_data.py
+-rw-r--r--   0        0        0     1051 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_response_error.py
+-rw-r--r--   0        0        0     1049 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/inference_response_status.py
+-rw-r--r--   0        0        0      330 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/new_inference_request.py
+-rw-r--r--   0        0        0     1028 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/org_read.py
+-rw-r--r--   0        0        0     1184 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_read.py
+-rw-r--r--   0        0        0      507 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_status.py
+-rw-r--r--   0        0        0      152 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_version_providers.py
+-rw-r--r--   0        0        0     1651 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_version_read.py
+-rw-r--r--   0        0        0      837 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/prompt_version_status.py
+-rw-r--r--   0        0        0      767 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/token.py
+-rw-r--r--   0        0        0     1236 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/user_read.py
+-rw-r--r--   0        0        0      686 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/user_roles.py
+-rw-r--r--   0        0        0      869 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-13 18:16:00.000000 prompton-0.0.3/prompton/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      450 2023-06-13 19:02:26.478078 prompton-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.3/PKG-INFO
```

### Comparing `prompton-0.0.2/prompton/__init__.py` & `prompton-0.0.3/prompton/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,25 @@
     ChatGptChatCompletitionResponse,
     ChatGptCompletitionChoice,
     ChatGptMessage,
     ChatGptRole,
     ChatGptTokenUsage,
     DbStatus,
     HttpValidationError,
+    InferenceCreateByPromptId,
+    InferenceCreateByPromptVersionId,
     InferencePostResponse,
     InferencePostResponseResponse,
     InferenceRead,
     InferenceReadResponse,
     InferenceRequestData,
     InferenceResponseData,
     InferenceResponseError,
     InferenceResponseStatus,
+    NewInferenceRequest,
     OrgRead,
     PromptRead,
     PromptStatus,
     PromptVersionProviders,
     PromptVersionRead,
     PromptVersionStatus,
     Token,
@@ -48,22 +51,25 @@
     "ChatGptChatCompletitionResponse",
     "ChatGptCompletitionChoice",
     "ChatGptMessage",
     "ChatGptRole",
     "ChatGptTokenUsage",
     "DbStatus",
     "HttpValidationError",
+    "InferenceCreateByPromptId",
+    "InferenceCreateByPromptVersionId",
     "InferencePostResponse",
     "InferencePostResponseResponse",
     "InferenceRead",
     "InferenceReadResponse",
     "InferenceRequestData",
     "InferenceResponseData",
     "InferenceResponseError",
     "InferenceResponseStatus",
+    "NewInferenceRequest",
     "NotFoundError",
     "OrgRead",
     "PromptRead",
     "PromptStatus",
     "PromptVersionProviders",
     "PromptVersionRead",
     "PromptVersionStatus",
```

### Comparing `prompton-0.0.2/prompton/client.py` & `prompton-0.0.3/prompton/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/core/datetime_utils.py` & `prompton-0.0.3/prompton/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/core/jsonable_encoder.py` & `prompton-0.0.3/prompton/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/resources/authentication/client.py` & `prompton-0.0.3/prompton/resources/authentication/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/resources/inferences/client.py` & `prompton-0.0.3/prompton/resources/users/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,215 +10,252 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.bad_request_error import BadRequestError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.inference_post_response import InferencePostResponse
-from ...types.inference_read import InferenceRead
+from ...types.user_read import UserRead
+from ...types.user_roles import UserRoles
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class InferencesClient:
+class UsersClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def get_inferences_list(
-        self, *, prompt_version_id: typing.Optional[str] = None, prompt_id: typing.Optional[str] = None
-    ) -> typing.List[InferenceRead]:
+    def get_users_list(self) -> typing.List[UserRead]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "inferences"),
-            params={"prompt_version_id": prompt_version_id, "prompt_id": prompt_id},
+            urllib.parse.urljoin(f"{self._environment}/", "users"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InferenceRead], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[UserRead], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def new_inference(
+    def add_new_user(
         self,
         *,
-        end_user_id: str,
-        source: str,
-        template_args: typing.Optional[typing.Dict[str, str]] = OMIT,
-        metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        request_timeout: typing.Optional[float] = OMIT,
-        prompt_version_id: str,
-    ) -> InferencePostResponse:
-        _request: typing.Dict[str, typing.Any] = {
-            "end_user_id": end_user_id,
-            "source": source,
-            "prompt_version_id": prompt_version_id,
-        }
-        if template_args is not OMIT:
-            _request["template_args"] = template_args
-        if metadata is not OMIT:
-            _request["metadata"] = metadata
-        if request_timeout is not OMIT:
-            _request["request_timeout"] = request_timeout
+        full_name: typing.Optional[str] = OMIT,
+        disabled: typing.Optional[bool] = OMIT,
+        role: typing.Optional[UserRoles] = OMIT,
+        org_id: str,
+        email: str,
+        plain_password: str,
+    ) -> typing.Any:
+        _request: typing.Dict[str, typing.Any] = {"org_id": org_id, "email": email, "plain_password": plain_password}
+        if full_name is not OMIT:
+            _request["full_name"] = full_name
+        if disabled is not OMIT:
+            _request["disabled"] = disabled
+        if role is not OMIT:
+            _request["role"] = role
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "inferences"),
+            urllib.parse.urljoin(f"{self._environment}/", "users"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InferencePostResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_inference_by_id(self, id: str) -> InferenceRead:
+    def get_current_user(self) -> UserRead:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"inferences/{id}"),
+            urllib.parse.urljoin(f"{self._environment}/", "users/me"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InferenceRead, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_user_by_id(self, id: str) -> UserRead:
+        _response = httpx.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment}/", f"users/{id}"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
 
-class AsyncInferencesClient:
+
+class AsyncUsersClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def get_inferences_list(
-        self, *, prompt_version_id: typing.Optional[str] = None, prompt_id: typing.Optional[str] = None
-    ) -> typing.List[InferenceRead]:
+    async def get_users_list(self) -> typing.List[UserRead]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "inferences"),
-                params={"prompt_version_id": prompt_version_id, "prompt_id": prompt_id},
+                urllib.parse.urljoin(f"{self._environment}/", "users"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InferenceRead], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[UserRead], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def new_inference(
+    async def add_new_user(
         self,
         *,
-        end_user_id: str,
-        source: str,
-        template_args: typing.Optional[typing.Dict[str, str]] = OMIT,
-        metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        request_timeout: typing.Optional[float] = OMIT,
-        prompt_version_id: str,
-    ) -> InferencePostResponse:
-        _request: typing.Dict[str, typing.Any] = {
-            "end_user_id": end_user_id,
-            "source": source,
-            "prompt_version_id": prompt_version_id,
-        }
-        if template_args is not OMIT:
-            _request["template_args"] = template_args
-        if metadata is not OMIT:
-            _request["metadata"] = metadata
-        if request_timeout is not OMIT:
-            _request["request_timeout"] = request_timeout
+        full_name: typing.Optional[str] = OMIT,
+        disabled: typing.Optional[bool] = OMIT,
+        role: typing.Optional[UserRoles] = OMIT,
+        org_id: str,
+        email: str,
+        plain_password: str,
+    ) -> typing.Any:
+        _request: typing.Dict[str, typing.Any] = {"org_id": org_id, "email": email, "plain_password": plain_password}
+        if full_name is not OMIT:
+            _request["full_name"] = full_name
+        if disabled is not OMIT:
+            _request["disabled"] = disabled
+        if role is not OMIT:
+            _request["role"] = role
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "inferences"),
+                urllib.parse.urljoin(f"{self._environment}/", "users"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InferencePostResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_inference_by_id(self, id: str) -> InferenceRead:
+    async def get_current_user(self) -> UserRead:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "GET",
+                urllib.parse.urljoin(f"{self._environment}/", "users/me"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 401:
+            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_user_by_id(self, id: str) -> UserRead:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"inferences/{id}"),
+                urllib.parse.urljoin(f"{self._environment}/", f"users/{id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InferenceRead, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
```

### Comparing `prompton-0.0.2/prompton/resources/orgs/client.py` & `prompton-0.0.3/prompton/resources/orgs/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/resources/prompt_versions/client.py` & `prompton-0.0.3/prompton/resources/prompt_versions/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/resources/prompts/client.py` & `prompton-0.0.3/prompton/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/resources/server_status/client.py` & `prompton-0.0.3/prompton/resources/server_status/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/resources/users/client.py` & `prompton-0.0.3/prompton/resources/inferences/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,127 +10,87 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.bad_request_error import BadRequestError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.user_read import UserRead
-from ...types.user_roles import UserRoles
+from ...types.inference_post_response import InferencePostResponse
+from ...types.inference_read import InferenceRead
+from ...types.new_inference_request import NewInferenceRequest
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class UsersClient:
+class InferencesClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def get_users_list(self) -> typing.List[UserRead]:
+    def get_inferences_list(
+        self, *, prompt_version_id: typing.Optional[str] = None, prompt_id: typing.Optional[str] = None
+    ) -> typing.List[InferenceRead]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "users"),
+            urllib.parse.urljoin(f"{self._environment}/", "inferences"),
+            params={"prompt_version_id": prompt_version_id, "prompt_id": prompt_id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[UserRead], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[InferenceRead], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add_new_user(
-        self,
-        *,
-        full_name: typing.Optional[str] = OMIT,
-        disabled: typing.Optional[bool] = OMIT,
-        role: typing.Optional[UserRoles] = OMIT,
-        org_id: str,
-        email: str,
-        plain_password: str,
-    ) -> typing.Any:
-        _request: typing.Dict[str, typing.Any] = {"org_id": org_id, "email": email, "plain_password": plain_password}
-        if full_name is not OMIT:
-            _request["full_name"] = full_name
-        if disabled is not OMIT:
-            _request["disabled"] = disabled
-        if role is not OMIT:
-            _request["role"] = role
+    def new_inference(self, *, request: NewInferenceRequest) -> InferencePostResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "users"),
-            json=jsonable_encoder(_request),
+            urllib.parse.urljoin(f"{self._environment}/", "inferences"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(InferencePostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_current_user(self) -> UserRead:
-        _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "users/me"),
-            headers=remove_none_from_headers(
-                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-            ),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_user_by_id(self, id: str) -> UserRead:
+    def get_inference_by_id(self, id: str) -> InferenceRead:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"users/{id}"),
+            urllib.parse.urljoin(f"{self._environment}/", f"inferences/{id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(InferenceRead, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
@@ -138,124 +98,85 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncUsersClient:
+class AsyncInferencesClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def get_users_list(self) -> typing.List[UserRead]:
+    async def get_inferences_list(
+        self, *, prompt_version_id: typing.Optional[str] = None, prompt_id: typing.Optional[str] = None
+    ) -> typing.List[InferenceRead]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "users"),
+                urllib.parse.urljoin(f"{self._environment}/", "inferences"),
+                params={"prompt_version_id": prompt_version_id, "prompt_id": prompt_id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[UserRead], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[InferenceRead], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add_new_user(
-        self,
-        *,
-        full_name: typing.Optional[str] = OMIT,
-        disabled: typing.Optional[bool] = OMIT,
-        role: typing.Optional[UserRoles] = OMIT,
-        org_id: str,
-        email: str,
-        plain_password: str,
-    ) -> typing.Any:
-        _request: typing.Dict[str, typing.Any] = {"org_id": org_id, "email": email, "plain_password": plain_password}
-        if full_name is not OMIT:
-            _request["full_name"] = full_name
-        if disabled is not OMIT:
-            _request["disabled"] = disabled
-        if role is not OMIT:
-            _request["role"] = role
+    async def new_inference(self, *, request: NewInferenceRequest) -> InferencePostResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "users"),
-                json=jsonable_encoder(_request),
+                urllib.parse.urljoin(f"{self._environment}/", "inferences"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(InferencePostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_current_user(self) -> UserRead:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "users/me"),
-                headers=remove_none_from_headers(
-                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
-                ),
-                timeout=60,
-            )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_user_by_id(self, id: str) -> UserRead:
+    async def get_inference_by_id(self, id: str) -> InferenceRead:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", f"users/{id}"),
+                urllib.parse.urljoin(f"{self._environment}/", f"inferences/{id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UserRead, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(InferenceRead, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
```

### Comparing `prompton-0.0.2/prompton/types/__init__.py` & `prompton-0.0.3/prompton/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 from .chat_gpt_chat_completition_response import ChatGptChatCompletitionResponse
 from .chat_gpt_completition_choice import ChatGptCompletitionChoice
 from .chat_gpt_message import ChatGptMessage
 from .chat_gpt_role import ChatGptRole
 from .chat_gpt_token_usage import ChatGptTokenUsage
 from .db_status import DbStatus
 from .http_validation_error import HttpValidationError
+from .inference_create_by_prompt_id import InferenceCreateByPromptId
+from .inference_create_by_prompt_version_id import InferenceCreateByPromptVersionId
 from .inference_post_response import InferencePostResponse
 from .inference_post_response_response import InferencePostResponseResponse
 from .inference_read import InferenceRead
 from .inference_read_response import InferenceReadResponse
 from .inference_request_data import InferenceRequestData
 from .inference_response_data import InferenceResponseData
 from .inference_response_error import InferenceResponseError
 from .inference_response_status import InferenceResponseStatus
+from .new_inference_request import NewInferenceRequest
 from .org_read import OrgRead
 from .prompt_read import PromptRead
 from .prompt_status import PromptStatus
 from .prompt_version_providers import PromptVersionProviders
 from .prompt_version_read import PromptVersionRead
 from .prompt_version_status import PromptVersionStatus
 from .token import Token
@@ -43,22 +46,25 @@
     "ChatGptChatCompletitionResponse",
     "ChatGptCompletitionChoice",
     "ChatGptMessage",
     "ChatGptRole",
     "ChatGptTokenUsage",
     "DbStatus",
     "HttpValidationError",
+    "InferenceCreateByPromptId",
+    "InferenceCreateByPromptVersionId",
     "InferencePostResponse",
     "InferencePostResponseResponse",
     "InferenceRead",
     "InferenceReadResponse",
     "InferenceRequestData",
     "InferenceResponseData",
     "InferenceResponseError",
     "InferenceResponseStatus",
+    "NewInferenceRequest",
     "OrgRead",
     "PromptRead",
     "PromptStatus",
     "PromptVersionProviders",
     "PromptVersionRead",
     "PromptVersionStatus",
     "Token",
```

### Comparing `prompton-0.0.2/prompton/types/api_status_response.py` & `prompton-0.0.3/prompton/types/api_status_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/body_get_access_token_extended_token_post.py` & `prompton-0.0.3/prompton/types/body_get_access_token_extended_token_post.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_chat_completition_config.py` & `prompton-0.0.3/prompton/types/chat_gpt_chat_completition_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .chat_gpt_chat_completition_config_stop import ChatGptChatCompletitionConfigStop
 
 
 class ChatGptChatCompletitionConfig(pydantic.BaseModel):
-    model: typing.Optional[str] = pydantic.Field(description=("`non-empty`\n"))
+    model: typing.Optional[str] = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
     temperature: typing.Optional[float]
     top_p: typing.Optional[float]
     stop: typing.Optional[ChatGptChatCompletitionConfigStop]
     max_tokens: typing.Optional[int]
     presence_penalty: typing.Optional[float]
     frequency_penalty: typing.Optional[float]
     logit_bias: typing.Optional[typing.Dict[str, int]]
```

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_chat_completition_request.py` & `prompton-0.0.3/prompton/types/chat_gpt_chat_completition_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .chat_gpt_chat_completition_request_stop import ChatGptChatCompletitionRequestStop
 from .chat_gpt_message import ChatGptMessage
 
 
 class ChatGptChatCompletitionRequest(pydantic.BaseModel):
-    model: typing.Optional[str] = pydantic.Field(description=("`non-empty`\n"))
+    model: typing.Optional[str] = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
     temperature: typing.Optional[float]
     top_p: typing.Optional[float]
     stop: typing.Optional[ChatGptChatCompletitionRequestStop]
     max_tokens: typing.Optional[int]
     presence_penalty: typing.Optional[float]
     frequency_penalty: typing.Optional[float]
     logit_bias: typing.Optional[typing.Dict[str, int]]
```

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_chat_completition_response.py` & `prompton-0.0.3/prompton/types/chat_gpt_chat_completition_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_completition_choice.py` & `prompton-0.0.3/prompton/types/chat_gpt_completition_choice.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_message.py` & `prompton-0.0.3/prompton/types/chat_gpt_message.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_role.py` & `prompton-0.0.3/prompton/types/chat_gpt_role.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/chat_gpt_token_usage.py` & `prompton-0.0.3/prompton/types/chat_gpt_token_usage.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/db_status.py` & `prompton-0.0.3/prompton/types/db_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/http_validation_error.py` & `prompton-0.0.3/prompton/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/inference_post_response.py` & `prompton-0.0.3/prompton/types/inference_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/inference_read.py` & `prompton-0.0.3/prompton/types/inference_read.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,20 +12,25 @@
 
 
 class InferenceRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
-    end_user_id: str = pydantic.Field(description=("`non-empty`\n"))
-    source: str = pydantic.Field(description=("`non-empty`\n"))
+    end_user_id: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
+    source: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
     template_args: typing.Optional[typing.Dict[str, str]]
     metadata: typing.Optional[typing.Dict[str, typing.Any]]
     request_timeout: typing.Optional[float]
     prompt_version_id: str
+    prompt_version_ids_considered: typing.Optional[typing.List[str]] = pydantic.Field(
+        description=(
+            "If inference was by prompt_id then a list of all other prompt versions considered for this inference. I.e. all prompt versions in Live status at the time of the inference\n"
+        )
+    )
     prompt_id: str
     prompt_version_name: typing.Optional[str]
     status: typing.Optional[InferenceResponseStatus]
     request: typing.Optional[InferenceRequestData]
     response: typing.Optional[InferenceReadResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `prompton-0.0.2/prompton/types/inference_request_data.py` & `prompton-0.0.3/prompton/types/inference_request_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/inference_response_data.py` & `prompton-0.0.3/prompton/types/inference_response_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/inference_response_error.py` & `prompton-0.0.3/prompton/types/inference_response_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/inference_response_status.py` & `prompton-0.0.3/prompton/types/inference_response_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/org_read.py` & `prompton-0.0.3/prompton/types/org_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class OrgRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
-    name: str = pydantic.Field(description=("`non-empty`\n"))
+    name: str
     access_keys: typing.Optional[typing.Dict[str, str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `prompton-0.0.2/prompton/types/prompt_read.py` & `prompton-0.0.3/prompton/types/prompt_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class PromptRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
     status: typing.Optional[PromptStatus]
-    name: str = pydantic.Field(description=("`non-empty`\n"))
+    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
     description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `prompton-0.0.2/prompton/types/prompt_version_read.py` & `prompton-0.0.3/prompton/types/prompt_version_read.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class PromptVersionRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
     status: typing.Optional[PromptVersionStatus]
     provider: typing.Optional[PromptVersionProviders]
-    name: str = pydantic.Field(description=("`non-empty`\n"))
+    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
     description: typing.Optional[str]
     prompt_id: str
     template: typing.Optional[typing.List[ChatGptMessage]]
     model_config: typing.Optional[ChatGptChatCompletitionConfig]
     template_arg_names: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `prompton-0.0.2/prompton/types/prompt_version_status.py` & `prompton-0.0.3/prompton/types/prompt_version_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/token.py` & `prompton-0.0.3/prompton/types/token.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/user_read.py` & `prompton-0.0.3/prompton/types/user_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 
 class UserRead(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(alias="_id")
     created_at: typing.Optional[str]
     created_by_user_id: typing.Optional[str]
     created_by_org_id: typing.Optional[str]
-    full_name: typing.Optional[str] = pydantic.Field(description=("`non-empty`\n"))
+    full_name: typing.Optional[str] = pydantic.Field(
+        description=('<span style="white-space: nowrap">`non-empty`</span>\n')
+    )
     disabled: typing.Optional[bool]
     role: typing.Optional[UserRoles]
     org_id: str
     email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.2/prompton/types/user_roles.py` & `prompton-0.0.3/prompton/types/user_roles.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.2/prompton/types/validation_error.py` & `prompton-0.0.3/prompton/types/validation_error.py`

 * *Files identical despite different names*

