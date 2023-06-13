# Comparing `tmp/restsession-0.0.1.tar.gz` & `tmp/restsession-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restsession-0.0.1.tar", last modified: Sun Jun 11 22:12:22 2023, max compression
+gzip compressed data, was "restsession-0.0.2.tar", last modified: Tue Jun 13 20:51:06 2023, max compression
```

## Comparing `restsession-0.0.1.tar` & `restsession-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lsample    (501) staff       (20)        0 2023-06-11 22:12:22.603753 restsession-0.0.1/
--rw-r--r--   0 lsample    (501) staff       (20)     1070 2023-06-11 21:51:14.000000 restsession-0.0.1/LICENSE
--rw-r--r--   0 lsample    (501) staff       (20)      619 2023-06-11 22:12:22.603553 restsession-0.0.1/PKG-INFO
--rw-r--r--   0 lsample    (501) staff       (20)       63 2023-06-11 21:51:14.000000 restsession-0.0.1/README.md
--rw-r--r--   0 lsample    (501) staff       (20)      629 2023-06-11 22:11:49.000000 restsession-0.0.1/pyproject.toml
-drwxr-xr-x   0 lsample    (501) staff       (20)        0 2023-06-11 22:12:22.587264 restsession-0.0.1/restsession/
--rw-r--r--   0 lsample    (501) staff       (20)      244 2023-03-20 16:06:13.000000 restsession-0.0.1/restsession/__init__.py
--rw-r--r--   0 lsample    (501) staff       (20)     1273 2023-04-10 15:20:26.000000 restsession-0.0.1/restsession/defaults.py
--rw-r--r--   0 lsample    (501) staff       (20)      549 2023-03-19 17:41:15.000000 restsession-0.0.1/restsession/metaclass.py
--rw-r--r--   0 lsample    (501) staff       (20)    14591 2023-04-09 16:19:31.000000 restsession-0.0.1/restsession/models.py
--rw-r--r--   0 lsample    (501) staff       (20)    30872 2023-06-11 20:54:09.000000 restsession-0.0.1/restsession/session.py
--rw-r--r--   0 lsample    (501) staff       (20)     1144 2023-03-20 15:45:13.000000 restsession-0.0.1/restsession/session_singleton.py
-drwxr-xr-x   0 lsample    (501) staff       (20)        0 2023-06-11 22:12:22.590298 restsession-0.0.1/restsession.egg-info/
--rw-r--r--   0 lsample    (501) staff       (20)      619 2023-06-11 22:12:22.000000 restsession-0.0.1/restsession.egg-info/PKG-INFO
--rw-r--r--   0 lsample    (501) staff       (20)      439 2023-06-11 22:12:22.000000 restsession-0.0.1/restsession.egg-info/SOURCES.txt
--rw-r--r--   0 lsample    (501) staff       (20)        1 2023-06-11 22:12:22.000000 restsession-0.0.1/restsession.egg-info/dependency_links.txt
--rw-r--r--   0 lsample    (501) staff       (20)       12 2023-06-11 22:12:22.000000 restsession-0.0.1/restsession.egg-info/top_level.txt
--rw-r--r--   0 lsample    (501) staff       (20)       38 2023-06-11 22:12:22.603814 restsession-0.0.1/setup.cfg
-drwxr-xr-x   0 lsample    (501) staff       (20)        0 2023-06-11 22:12:22.601674 restsession-0.0.1/tests/
--rw-r--r--   0 lsample    (501) staff       (20)    34906 2023-06-11 20:57:14.000000 restsession-0.0.1/tests/test_authorization.py
--rw-r--r--   0 lsample    (501) staff       (20)     8315 2023-06-11 22:01:56.000000 restsession-0.0.1/tests/test_code.py
--rw-r--r--   0 lsample    (501) staff       (20)     4725 2023-06-11 22:01:56.000000 restsession-0.0.1/tests/test_redirects.py
--rw-r--r--   0 lsample    (501) staff       (20)    17013 2023-04-09 16:39:44.000000 restsession-0.0.1/tests/test_requests.py
--rw-r--r--   0 lsample    (501) staff       (20)     8090 2023-06-11 22:01:56.000000 restsession-0.0.1/tests/test_retries.py
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.884108 restsession-0.0.2/
+-rw-r--r--   0 psample    (501) staff       (20)     1070 2023-06-11 21:51:14.000000 restsession-0.0.2/LICENSE
+-rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 20:51:06.883779 restsession-0.0.2/PKG-INFO
+-rw-r--r--   0 psample    (501) staff       (20)       63 2023-06-11 21:51:14.000000 restsession-0.0.2/README.md
+-rw-r--r--   0 psample    (501) staff       (20)      629 2023-06-13 20:46:43.000000 restsession-0.0.2/pyproject.toml
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.871531 restsession-0.0.2/restsession/
+-rw-r--r--   0 psample    (501) staff       (20)      207 2023-06-13 15:13:41.000000 restsession-0.0.2/restsession/__init__.py
+-rw-r--r--   0 psample    (501) staff       (20)     1325 2023-06-13 18:01:16.000000 restsession-0.0.2/restsession/defaults.py
+-rw-r--r--   0 psample    (501) staff       (20)      549 2023-03-19 17:41:15.000000 restsession-0.0.2/restsession/metaclass.py
+-rw-r--r--   0 psample    (501) staff       (20)    15518 2023-06-13 15:11:56.000000 restsession-0.0.2/restsession/models.py
+-rw-r--r--   0 psample    (501) staff       (20)    33510 2023-06-13 20:35:57.000000 restsession-0.0.2/restsession/session.py
+-rw-r--r--   0 psample    (501) staff       (20)     1144 2023-03-20 15:45:13.000000 restsession-0.0.2/restsession/session_singleton.py
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.874297 restsession-0.0.2/restsession.egg-info/
+-rw-r--r--   0 psample    (501) staff       (20)      619 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/PKG-INFO
+-rw-r--r--   0 psample    (501) staff       (20)      439 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/SOURCES.txt
+-rw-r--r--   0 psample    (501) staff       (20)        1 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/dependency_links.txt
+-rw-r--r--   0 psample    (501) staff       (20)       12 2023-06-13 20:51:06.000000 restsession-0.0.2/restsession.egg-info/top_level.txt
+-rw-r--r--   0 psample    (501) staff       (20)       38 2023-06-13 20:51:06.884209 restsession-0.0.2/setup.cfg
+drwxr-xr-x   0 psample    (501) staff       (20)        0 2023-06-13 20:51:06.882532 restsession-0.0.2/tests/
+-rw-r--r--   0 psample    (501) staff       (20)    42269 2023-06-13 18:36:44.000000 restsession-0.0.2/tests/test_authorization.py
+-rw-r--r--   0 psample    (501) staff       (20)     8315 2023-06-11 22:01:56.000000 restsession-0.0.2/tests/test_code.py
+-rw-r--r--   0 psample    (501) staff       (20)     4725 2023-06-11 22:01:56.000000 restsession-0.0.2/tests/test_redirects.py
+-rw-r--r--   0 psample    (501) staff       (20)    17013 2023-04-09 16:39:44.000000 restsession-0.0.2/tests/test_requests.py
+-rw-r--r--   0 psample    (501) staff       (20)     8090 2023-06-11 22:01:56.000000 restsession-0.0.2/tests/test_retries.py
```

### Comparing `restsession-0.0.1/LICENSE` & `restsession-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `restsession-0.0.1/pyproject.toml` & `restsession-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "restsession"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Palmer Sample", email="palmer@palmersample.net" },
 ]
 description = "RESTful API-friendly implementation of the 'requests' library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `restsession-0.0.1/restsession/defaults.py` & `restsession-0.0.2/restsession/defaults.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 from types import MappingProxyType
 
 # 301: Moved Permanently
 # 302: Found / moved temporarily
 # 303: See other
 # 307: Temporary redirect (HTTP/1.1)
 # 308: Permanent redirect (no HTTP method change)
-REDIRECT_STATUS_CODES = [301, 302, 303, 307, 308]
+REDIRECT_STATUS_CODES = (301, 302, 303, 307, 308)
 
 # 408: Request timeout
 # 413: Payload too large
 # 429: Too many requests
-CLIENT_ERROR_CODES = [408, 413, 429]
+CLIENT_ERROR_CODES = (408, 413, 429)
 
 # 503: Service Unavailable - should be temporary
-SERVER_ERROR_CODES = [503]
+SERVER_ERROR_CODES = (503,)
 
 SESSION_DEFAULTS = MappingProxyType(
     {
+        "headers": {},
+        "auth_headers": {},
         "timeout": 5,
         "retries": 3,
         "max_redirect": 16,
         "backoff_factor": 0.3,
         "retry_status_codes": CLIENT_ERROR_CODES + SERVER_ERROR_CODES,
         "retry_methods": [
             "HEAD",
```

### Comparing `restsession-0.0.1/restsession/metaclass.py` & `restsession-0.0.2/restsession/metaclass.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.1/restsession/models.py` & `restsession-0.0.2/restsession/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 When possible, break individual fields (or related fields) into their own
 class. This allows granular validation of sub-fields while still allowing
 a main "entry" class to be used for full model validation.
 """
 # pylint: disable=no-name-in-module, no-self-argument, too-few-public-methods
 import logging
 from typing import (Optional,
-                    Union)
+                    Union,
+                    Callable)
 from pydantic import (BaseModel,
                       AnyHttpUrl,
                       StrictBool,
                       StrictFloat,
                       StrictInt,
                       StrictStr,
                       ValidationError,
                       conint,
+                      conlist,
                       parse_obj_as,
                       validator)
 from requests.auth import AuthBase
 from .defaults import SESSION_DEFAULTS
 
 logger = logging.getLogger(__name__)
 
@@ -148,15 +150,14 @@
     #     Union[
     #         conint(strict=True, ge=301, le=301),
     #         conint(strict=True, ge=429, le=429),
     #         conint(strict=True, ge=500, le=599)
     #     ]
     # ] = []
 
-    # pylint: disable=loop-invariant-statement
     @validator("retry_status_code_list", pre=True)
     def validate_retry_status_code_list(cls, value):
         """
         Validate the requested retry status code list. If an invalid status
         code is supplied, omit that from the resulting list. Otherwise,
         return the requested values OR the default values (if no list supplied)
 
@@ -351,14 +352,17 @@
 class AuthValidator(BaseModel):
     """
     Model for HTTP Basic Authentication - Password
     """
     auth: Optional[Union[tuple[str, str], AuthBase]] = None
 
     class Config:
+        """
+        pydantic configuration options for AuthValidator.
+        """
         arbitrary_types_allowed = True
 
     @validator("auth", pre=True)
     def validate_auth(cls, value):
         """
         Validate the auth attribute is a tuple of strings or an instance
         of requests.auth.AuthBase
@@ -405,19 +409,42 @@
             pass
         else:
             result = value
         logger.debug("Returning max_reauth value: %s", result)
         return result
 
 
+class RedirectHeaderHookValidator(BaseModel):
+    """
+    Model for the request exception hook
+    """
+    redirect_header_hook: Optional[conlist(Callable, min_items=0, max_items=1)] = []
+
+
+class RequestExceptionHookValidator(BaseModel):
+    """
+    Model for the request exception hook
+    """
+    request_exception_hook: Optional[conlist(Callable, min_items=0, max_items=1)] = []
+
+
 class ResponseHookValidator(BaseModel):
     """
     Model for HTTP Basic Authentication - Password
     """
-    response_hooks: Optional[list] = []
+    response_hooks: Optional[list[Callable]] = []
+
+
+class SessionHeaderValidator(BaseModel):
+    """
+    Model for HTTP header validation. Make sure the input is a dict and, if
+    not null, that the k/v pairs are strings.
+    """
+    headers: Optional[dict[str, str]] = {}
+    auth_headers: Optional[dict[str, str]] = {}
 
 
 # pylint: disable-next=too-many-ancestors, too-many-instance-attributes
 class HttpSessionArguments(ResponseHookValidator,
                            MaxReauthValidator,
                            AuthValidator,
                            PasswordValidator,
@@ -426,13 +453,16 @@
                            BaseUrlValidator,
                            RespectRetryHeadersValidator,
                            RetryMethodListValidator,
                            RetryStatusCodeListValidator,
                            BackoffFactorValidator,
                            MaxRedirectValidator,
                            RetriesValidator,
-                           TimeoutValidator
+                           TimeoutValidator,
+                           SessionHeaderValidator,
+                           RequestExceptionHookValidator,
+                           RedirectHeaderHookValidator
                            ):
     """
     Validate all session arguments by inheriting each individual BaseModel
     class.
     """
```

### Comparing `restsession-0.0.1/restsession/session.py` & `restsession-0.0.2/restsession/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 methods.
 
 Keyword parameter validation is performed via Pydantic models to simplify
 instantiation and ensure a valid session is available, even if an incorrect
 parameter is supplied.
 """
 import logging
+from typing import Any, Optional, Union
+from types import MappingProxyType
+from urllib.parse import urlparse
 from requests.exceptions import (HTTPError as RequestHTTPError,
                                  ConnectionError as RequestConnectionError,
                                  InvalidJSONError as RequestInvalidJSONError,
                                  Timeout as RequestTimeout,
                                  MissingSchema as RequestMissingSchema,
                                  RetryError as RequestRetryError,
                                  TooManyRedirects as RequestTooManyRedirects,
                                  RequestException)
 from requests.adapters import HTTPAdapter
-from requests import Session
+from requests.auth import AuthBase
+from requests_toolbelt import sessions
 from urllib3 import disable_warnings
 from urllib3.util.retry import Retry
-from requests_toolbelt import sessions
-from requests.auth import AuthBase
-from typing import Any, Optional, Union
 from .defaults import SESSION_DEFAULTS
 from .models import (
     HttpSessionArguments,
     TimeoutValidator,
     RetriesValidator,
     MaxRedirectValidator,
     BackoffFactorValidator,
@@ -59,28 +60,28 @@
         # pylint: disable=arguments-differ
         timeout = kwargs.get('timeout')
         if timeout is None:
             kwargs["timeout"] = self.timeout
         return super().send(request, **kwargs)
 
 
-def default_response_hook(response, **kwargs):  # pylint: disable=unused-argument
+def default_request_exception_hook(response, **kwargs):  # pylint: disable=unused-argument
     """
     This function is bound to the HTTP Session object and raises the request
     Response for status, catches exceptions, and re-raises the same exception
     to be handled by the calling script. This avoids having to repeat the
     raise_for_status() method each time a request is made by the caller.
 
     The response hook can be overridden during or after class instantiation
     to permit app-specific custom exception raises.
 
     :param response: Requests response object
     :return: None
     """
-    logger.info("Entering default_response_hook after request...")
+
     try:
         response.raise_for_status()
     except RequestTooManyRedirects as err:
         logger.error("Too many redirects occurred when processing the request: %s", err)
         raise RequestTooManyRedirects(err) from err
     except RequestRetryError as err:
         logger.error("Request retry handler error was encountered: %s", err)
@@ -101,48 +102,67 @@
     except RequestMissingSchema as err:
         logger.error("Missing scheme in request. "
                      "Check that base_url is set if using relative path: %s", err)
         raise RequestMissingSchema(err) from err
     except RequestException as err:
         logger.error("An unspecified request exception was encountered: %s", err)
         raise RequestException(err) from err
-    # else:
-    #     if response.is_redirect:
-    #         logger.error("Response dir: %s", dir(response))
-    #         logger.error("Request object: %s", dir(response.request))
-    #         if "Authorization" in response.request.headers:
-    #             logger.error("Deleting the authorization")
-    #             del(response.request.headers["Authorization"])
-
-
-# def remove_custom_auth_header_on_redirect(response, **kwargs):  # pylint: disable=unused-argument
-# def remove_custom_auth_header_on_redirect(header, *args, **kwargs):  # pylint: disable=unused-argument
-def remove_custom_auth_header_on_redirect(header):  # pylint: disable=unused-argument
-    logger.error(f"Creating hook to remove header '%s' on redirect...", header)
-
-    def response_hook(response, **kwargs):
-        logger.info("Removing custom auth header on redirect")
-        logger.error("kwargs:\n%s", kwargs)
-
-        if response.is_redirect:
-            if header in response.request.headers:
-                logger.error("Deleting the authorization")
-                del(response.request.headers[header])
 
-    return response_hook
+
+def remove_custom_auth_header_on_redirect(headers: Optional[list[str]] = ()):
+    """
+    Given a list of header keys, if any are present after a cross-domain
+    redirect they will be removed. The "Authorization" header is already
+    handled by the requests library, so this permits custom auth headers
+    to also be removed for security reasons.
+
+    The returned function (redirect_header_hook) will be the first response
+    hook attached to the Session object.
+
+    :param headers: List of header names to remove on redirect
+    :return: redirect_header_hook function reference to be used as a hook
+    """
+    logger.error("Creating hook to remove header '%s' on redirect...", headers)
+
+    def redirect_header_hook(response, **kwargs):  # pylint: disable=unused-argument
+        """
+        Hook used when a redirect response is received. If redirected to a
+        different host, remove any custom auth headers as supplied in the
+        wrapping function.
+
+        :param response: requests Response object
+        :param kwargs: Any arguments passed to the response hook by requests
+        :return: None
+        """
+        if response.is_redirect and headers and \
+                (urlparse(response.request.url).netloc !=
+                 urlparse(response.headers["Location"]).netloc):
+
+            # Only strip the headers when being redirected to a different host
+            response.request.headers = {
+                k: v for k, v in response.request.headers.items() if k not in headers
+            }
+
+    return redirect_header_hook
 
 
 class HttpSessionClass:
     """
     Main HTTP Session class. On init, create a new HTTP base URL session for the
     object, generate all needed settings for timeout/retries and configure
     HTTP Basic authentication if a username/password is provided.
     """
-    # pylint: disable=too-many-arguments, unused-argument
+    # pylint: disable=too-many-arguments
+    # pylint: disable=unused-argument
+    # pylint: disable=too-many-public-methods
+    # pylint: disable=too-many-instance-attributes
+    # pylint: disable=too-many-locals
     def __init__(self,
+                 headers: dict = SESSION_DEFAULTS["headers"],
+                 auth_headers: dict = SESSION_DEFAULTS["auth_headers"],
                  timeout: int = SESSION_DEFAULTS["timeout"],
                  retries: int = SESSION_DEFAULTS["retries"],
                  max_redirect: int = SESSION_DEFAULTS["max_redirect"],
                  backoff_factor: float = SESSION_DEFAULTS["backoff_factor"],
                  retry_status_code_list: list[int] = SESSION_DEFAULTS["retry_status_codes"],
                  retry_method_list: list[str] = SESSION_DEFAULTS["retry_methods"],
                  respect_retry_headers: bool = SESSION_DEFAULTS["respect_retry_headers"],
@@ -174,105 +194,59 @@
             is provided, set the session auth
         """
 
         if not hasattr(self, "_session_params"):
             self._session_params = HttpSessionArguments(**locals())
 
         self.http = sessions.BaseUrlSession(base_url=self.base_url)
-        # TODO Consider - let Session handle the redirect so it simplifies the retry_status_code_list
-        #  Otherwise will need to add every 3xx code used for redirects. Only use the Retry class for
-        #  status codes that will be retried on API failure, for example. ALSO - ensure strip headers
-        #  for authorization is enabled - IF POSSIBLE - on requests.Session() - OTHERWISE may need to
-        #  use the Retry and deal with the retry_status_code_list... maybe change defaults to include
-        #  more 3xx series responses.
-        #############
-        # TODO Update 2023-Mar-21 @ 1825: Using the request library when possible BECAUSE this allows
-        #  a response object to be accessible via the raised exception (e.g. err.response.history)
-        #  When using the Retry object, response objects are gobbled up and tied to the Retry object,
-        #  and the history is cleared each time a new retry is made. This may not be critical, but
-        #  it provides additional opportunity for implementations to test for a response object's
-        #  properties e.g. returned headers - even if the max redirect is reached.
-        # self.http.max_redirects = self.max_redirect
+        self.http.max_redirects = self.max_redirect
 
         self.http.verify = self.tls_verify
         if not self.tls_verify:
             disable_warnings()
 
-        # Can't get a response object is a redirect fails - so unable to get the count
-        # from the History. Until a fix is identified, set the redirect on the
-        # Session() object and disable here. This will cause retries to be performed
-        # at the requests level and not the urllib3.util.Retry - so be it for now.
-        # There should be no appreciable performance penalty bypassing this subclass.
-        #
-        # OBSERVATION: When redirects are enabled as part of the Retry(), you must add
-        # the redirect status code to the retry or the redirect count is ignored. It
-        # will just hit the max.
-        # BUT if you add the redirect status code to the retry status code list, the
-        # redirect is never actually followed... so the request is made to the same
-        # host repeatedly, which is essentially a blackhole of the request. IF you leave
-        # the redirect count set on the Retry object AND you do NOT set the Session()
-        # object's max_redirect count, the Retry value is ignored and the max of 30
-        # redirects is used... so really, there's no reason to set anything to do with
-        # the redirect on the Retry() object. Disabled - useless!
+        # requests handles the redirects, so only apply parameters related to
+        # retries with this handler.
         default_retry_strategy = Retry(
             total=self.retries,
-            # Setting total to None results in infinite retries for some statuses... WTF
-            # total=None,
-            # status=self.retries,
-            # connect=self.retries,
             other=0,
-            # redirect=self.max_redirect,
             redirect=False,
             backoff_factor=self.backoff_factor,
             status_forcelist=self.retry_status_code_list,
             allowed_methods=self.retry_method_list,
             respect_retry_after_header=self.respect_retry_headers,
-            # raise_on_status=False
-            raise_on_status=True,
-            # remove_headers_on_redirect=["Authorization", "X-Auth-Token"]
-            remove_headers_on_redirect=['X-Auth-Token'],
-            # With raise_on_redirect, assert status hook is NEVER called.
-            raise_on_redirect=True
-            # raise_on_redirect=False
-            # raise_on_redirect=False
+            raise_on_status=True
         )
 
-        self.timeout = timeout
+        self.http.timeout = self.timeout
 
         # Mount http/https to the request session and attach the timeout
         # adapter with defined retry strategy
-        # self.http.mount("https://", HTTPAdapter(max_retries=default_retry_strategy))
-        #
-        # self.http.mount("http://", HTTPAdapter(max_retries=default_retry_strategy))
-
         self.http.mount("https://", TimeoutHTTPAdapter(timeout=self.timeout,
-                                                       max_retries=default_retry_strategy)
-                        )
+                                                       max_retries=default_retry_strategy))
 
         self.http.mount("http://", TimeoutHTTPAdapter(timeout=self.timeout,
-                                                      max_retries=default_retry_strategy)
-                        )
+                                                      max_retries=default_retry_strategy))
 
         # Is username/password provided, use basic auth. Otherwise if an auth
         # parameter was passed, initialize the session auth object
         if self.username and self.password:
             self.auth = (self.username, self.password)
         elif self.auth:
             self.http.auth = self.auth
         self.reauth_count = 0
 
-        # Assign the response hook to the session
-        # self.http.hooks['response'] = [default_response_hook]
-        if len(self.response_hooks) == 0:
-            self.replace_response_hooks(default_response_hook)
-        # self.response_hooks = default_response_hook
-
-        self.add_response_hooks(hooks=[remove_custom_auth_header_on_redirect(header="X-Auth-Token")])
-
-        # self.add_response_hooks(hooks=[remove_custom_auth_header_on_redirect])
+        # Assign the response hooks to the session. This should always be:
+        #  0: redirect_header_hook (remove auth headers on redirect)
+        #  1-x: custom_hooks
+        #  Last: request_exception_hook (raise for status and catch exceptions)
+        self.redirect_header_hook = remove_custom_auth_header_on_redirect(
+            headers=auth_headers.keys()
+        )
+        self.request_exception_hook = default_request_exception_hook
 
         self.max_reauth = 3
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -362,18 +336,18 @@
         new setting.
 
         :param max_redirect: Max redirects to follow
         :return: None
         """
         validated_field = MaxRedirectValidator(max_redirect=max_redirect)
         self._session_params.max_redirect = validated_field.max_redirect
-        self.http.max_redirects = self._session_params.max_redirect
-        # for mounted_adapter in self.http.adapters:
-        #     self.http.get_adapter(mounted_adapter)\
-        #         .max_retries.redirect = self._session_params.max_redirect
+        # self.http.max_redirects = self._session_params.max_redirect
+        for mounted_adapter in self.http.adapters:
+            self.http.get_adapter(mounted_adapter)\
+                .max_retries.redirect = self._session_params.max_redirect
 
     @property
     def backoff_factor(self):
         """
         Currently configured backoff factor for retries. From the urllib3
         documentation, backoff factor applies between attempts after the
         *second* try and the sleep will be for:
@@ -603,59 +577,194 @@
 
         Basic auth is provided as a tuple (username, password) and will update
         the object attributes if provided.
 
         :param auth_method: Authorization method for the HTTP session.
         :return: None
         """
+        # pylint: disable=unsubscriptable-object
+
         validated_field = AuthValidator(auth=auth_method)
         if isinstance(validated_field.auth, tuple):
             self._session_params.username = validated_field.auth[0]
             self._session_params.password = validated_field.auth[1]
         self._session_params.auth = validated_field.auth
         self.http.auth = self._session_params.auth
 
+    @property
+    def headers(self):
+        """
+        Currently configured headers to include in the request.
+
+        :return: headers attribute from session object
+        """
+        return self._session_params.headers
+
+    @headers.setter
+    def headers(self, headers: Optional[dict[str, str]] = MappingProxyType({})):
+        """
+        Update the HTTP headers for the current session. This should NOT be
+        used for authentication headers, as these will not be removed on a
+        cross-domain redirect. Use the auth_headers attribute for those.
+
+        :param headers: Dictionary of additional headers for the session.
+        :return: None
+        """
+        self._session_params.headers.update(headers)
+        self.http.headers.update(self._session_params.headers)
+
+    @property
+    def auth_headers(self):
+        """
+        Currently configured custom authentication/authorization headers.
+
+        :return: auth headers from the session object
+        """
+        return self._session_params.auth_headers
+
+    @auth_headers.setter
+    def auth_headers(self, headers: Optional[dict[str, str]] = MappingProxyType({})):
+        """
+        Add custom auth headers (X-Auth-Token, etc) for the request session
+        object. The differentiator with auth_headers is that each custom
+        auth header provided here will be added to the redirect hook which
+        will remove them on a cross-domain redirect.
+
+        :param headers: Dictionary of custom auth headers for the session
+        :return: None
+        """
+        self._session_params.auth_headers.update(headers)
+        self.http.headers.update(self._session_params.auth_headers)
+
+        self.redirect_header_hook = remove_custom_auth_header_on_redirect(headers=headers.keys())
+
     def reauth(self):
+        """
+        Attempt the last request if a 401 is received. If called, check for
+        the reauth attempt number and, if less than the max reauth,
+        perform a re-auth for the session and retry the request.
+
+        :return: None
+        :raises: RequestHTTPError if max auth count reached
+        """
         if hasattr(self.auth, "reauth"):
             if self.reauth_count >= self.max_reauth:
-                raise RequestHTTPError("Maximum reauthentication count reached (" + self.reauth_count + ")")
+                raise RequestHTTPError(
+                    f"Maximum reauthentication count reached ({self.reauth_count})"
+                )
             self.reauth_count += 1
             self.auth.reauth()
 
     @property
+    def redirect_header_hook(self):
+        """
+        Currently configured response hook for redirect handling
+
+        :return: session response hook for redirects
+        """
+        return self._session_params.redirect_header_hook
+
+    @redirect_header_hook.setter
+    def redirect_header_hook(self, hook):
+        """
+        Set (or replace) the response hook to handle redirects. By default,
+        the hook is configured to remove any custom auth headers before
+        re-sending a request when a redirect is received.
+
+        This hook will be the FIRST hook executed after a response.
+
+        :param headers: Function reference to become the redirect handler
+        :return: None
+        """
+        if not isinstance(hook, list):
+            hook = [hook]
+        logger.error("Response hooks: %s", self.http.hooks["response"])
+        logger.error("Setting hook: %s", hook)
+        self._session_params.redirect_header_hook = hook
+        self.http.hooks["response"] = self.redirect_header_hook + \
+                                      self.response_hooks + \
+                                      self.request_exception_hook
+        logger.error("redirect hook update: %s", self.http.hooks["response"])
+
+    @property
+    def request_exception_hook(self):
+        """
+        Currently configured response hook for exception handling
+
+        :return: session response hook for exceptions
+        """
+        return self._session_params.request_exception_hook
+
+    @request_exception_hook.setter
+    def request_exception_hook(self, hook):
+        """
+        Set (or replace) the exception hook to handle HTTP errors.
+
+        By default, the hook will re-raise various exceptions generated
+        by the requests library or urllib3; however, it may be desirable to
+        replace this hook if custom exceptions should be raised.
+
+        This hook will be the LAST hook raised after a response, after the
+        redirect hook and any custom hooks.
+
+        :param headers: Function reference to become the exception handler hook
+        :return: None
+        """
+        if not isinstance(hook, list):
+            hook = [hook]
+        self._session_params.request_exception_hook = hook
+        logger.error("Current exception hook: %s", self.request_exception_hook)
+        self.http.hooks["response"] = self.redirect_header_hook + \
+                                      self.response_hooks + \
+                                      self.request_exception_hook
+        logger.error("All current hooks: %s (len: %s)",
+                     self.http.hooks["response"],
+                     len(self.http.hooks["response"])
+                     )
+
+    @property
     def response_hooks(self):
+        """
+        Currently configured custom response hooks.
+
+        :return: User-defined custom response hooks
+        """
         return self._session_params.response_hooks
 
-    # @response_hooks.setter
-    # def response_hooks(self, hooks):
-    #     if not isinstance(hooks, list):
-    #         hooks = [hooks]
-    #
-    #     self._session_params.response_hooks = hooks + self._session_params.response_hooks
-    #     self.http.hooks["response"] = self._session_params.response_hooks
+    @response_hooks.setter
+    def response_hooks(self, hooks):
+        """
+        Add response hook(s) to be executed after a response is received.
+
+        Either a list of hooks can be provided, or a single hook. If a single
+        hook is passed, it will be appended to the list of exisiting response
+        hooks.
 
-    def add_response_hooks(self, hooks):
-        if not isinstance(hooks, list):
-            hooks = [hooks]
-        callable_hooks = []
-        for hook in hooks:
-            if callable(hook):
-                callable_hooks.append(hook)
-            else:
-                raise RequestException("The provided response hook is not a function, unable to add.")
-
-        # self._session_params.response_hooks = hooks + self.response_hooks
-        self._session_params.response_hooks = hooks + self.response_hooks
-        self.http.hooks["response"] = self.response_hooks
+        These response hooks will be executed AFTER the redirect hook and
+        BEFORE any exception handler hook.
 
-    def replace_response_hooks(self, hooks):
+        :param headers: Function(s) to call after a response is received.
+        :return: None
+        """
         if not isinstance(hooks, list):
             hooks = [hooks]
-        self._session_params.response_hooks = hooks
-        self.http.hooks["response"] = self.response_hooks
+
+        self._session_params.response_hooks = self._session_params.response_hooks + hooks
+        self.http.hooks["response"] = self.redirect_header_hook + \
+                                      self.response_hooks + \
+                                      self.request_exception_hook
+
+    def clear_response_hooks(self):
+        """
+        Clear all user-defined response hooks.
+
+        :return: None
+        """
+        self._session_params.response_hooks = []
+        self.http.hooks["response"] = []
 
     def request(self, method, url, **kwargs):
         """
         Send a generic HTTP request. See the Python "requests" library for
         detailed parameters available for any HTTP Request. "Standard" methods
         i.e. GET, POST, etc. are wrappers for this method, which itself is a
         wrapper for the requests library's "request" function.
```

### Comparing `restsession-0.0.1/restsession/session_singleton.py` & `restsession-0.0.2/restsession/session_singleton.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.1/tests/test_authorization.py` & `restsession-0.0.2/tests/test_authorization.py`

 * *Files 10% similar despite different names*

```diff
@@ -271,14 +271,86 @@
             f"Expected target server to reflect {expected_request_count} requests, " \
             f"Actual was {TargetMockServerRequestHandler.request_count}"
         assert TargetMockServerRequestHandler.received_auth is None, \
             f"On redirect, expected second server to NOT receive Authorization header. " \
             f"Instead, server received {TargetMockServerRequestHandler.received_auth}"
 
     @aetest.test
+    def test_basic_auth_header_not_removed_on_same_origin_redirect(self, url_path, basic_auth_username, basic_auth_password):
+        class FirstMockServerRequestHandler(BaseHTTPRequestHandler):
+            server_address = None
+            request_count = 0
+            next_server = None
+            received_auth = None
+
+            def do_GET(self):
+                if re.match(r"^/$", self.path):
+                    self.__class__.request_count += 1
+                    logger.error("Received request to / (%s)", self.path)
+                    self.__class__.received_auth = self.headers.get("Authorization", None)
+                    self.send_response(301)
+                    self.send_header(
+                        "Content-Type", "application/json; charset=utf-8"
+                    )
+                    logger.error("Redirecting to %s", self.__class__.next_server)
+                    self.send_header("Location", self.__class__.next_server)
+                    self.end_headers()
+                elif re.match(f"/{url_path}", self.path):
+                    self.__class__.request_count += 1
+                    logger.error("Received request to '%s'", url_path)
+                    self.__class__.received_auth = self.headers.get("Authorization", None)
+                    self.send_response(200)
+                    self.send_header(
+                        "Content-Type", "application/json; charset=utf-8"
+                    )
+                    # self.send_header("Location", self.__class__.next_server)
+                    self.end_headers()
+
+                return
+
+        test_server = self.start_mock_server(FirstMockServerRequestHandler)
+
+        logger.error("Target: %s", FirstMockServerRequestHandler.server_address)
+
+        base_url = f"http://{FirstMockServerRequestHandler.server_address}/"
+        target_url = f"http://{FirstMockServerRequestHandler.server_address}/{url_path}"
+
+        FirstMockServerRequestHandler.next_server = target_url
+
+        authorization_string = f"{basic_auth_username}:{basic_auth_password}"
+        base64_auth = base64.b64encode(bytes(authorization_string, 'utf-8')).decode('utf-8')
+        expected_auth_value = f"Basic {base64_auth}"
+
+        expected_request_count = 2
+
+        test_class = self.parameters["test_class"]
+
+        if hasattr(test_class, "_instances"):
+            test_class._instances = {}
+
+        test_instance = test_class(base_url=base_url, username=basic_auth_username, password=basic_auth_password)
+
+        try:
+            test_instance.get("/")
+        except Exception as err:
+            self.failed(f"Unexpected exception was raised:\n{err}")
+        finally:
+            self.start_mock_server(test_server)
+
+        assert FirstMockServerRequestHandler.request_count == expected_request_count, \
+            f"Expected first server to reflect {expected_request_count} requests, " \
+            f"Actual was {FirstMockServerRequestHandler.request_count}"
+        assert FirstMockServerRequestHandler.received_auth == expected_auth_value, \
+            f"First server expected auth header '{expected_auth_value}', " \
+            f"server received {FirstMockServerRequestHandler.received_auth}"
+        assert FirstMockServerRequestHandler.received_auth is not None, \
+            f"On redirect to the same host, Authorization header should be present. " \
+            f"Instead, server received {FirstMockServerRequestHandler.received_auth}"
+
+    @aetest.test
     def test_custom_auth_header_removed_on_redirect(self, url_path, custom_auth_token_one):
         class FirstMockServerRequestHandler(BaseHTTPRequestHandler):
             server_address = None
             request_count = 0
             next_server = None
             received_auth = None
 
@@ -331,16 +403,19 @@
         if hasattr(test_class, "_instances"):
             test_class._instances = {}
 
         test_instance = test_class(base_url=base_url)
 
         # TODO - Add test_instance.custom_auth_header attribute/setter. For each custom auth header,
         #   remove the key using the new remove_custom_auth_header hook
-        test_instance.http.headers.update({"X-Auth-Token": custom_auth_token_one, "Authorization": custom_auth_token_one})
-        # test_instance.http.headers
+        # test_instance.http.headers.update({"X-Auth-Token": custom_auth_token_one, "Authorization": custom_auth_token_one})
+        test_instance.auth_headers = {
+            "X-Auth-Token": custom_auth_token_one,
+            "Authorization": custom_auth_token_one
+        }
 
         try:
             test_instance.get(url_path)
         except Exception as err:
             self.failed(f"Unexpected exception was raised:\n{err}")
         finally:
             self.start_mock_server(first_test_server)
@@ -359,14 +434,93 @@
             f"Actual was {TargetMockServerRequestHandler.request_count}"
 
         assert TargetMockServerRequestHandler.received_auth is None, \
             f"On redirect, expected second server to NOT receive Authorization header. " \
             f"Instead, server received {TargetMockServerRequestHandler.received_auth}"
 
     @aetest.test
+    def test_custom_auth_header_not_removed_on_same_origin_redirect(self, url_path, custom_auth_token_one):
+        class FirstMockServerRequestHandler(BaseHTTPRequestHandler):
+            server_address = None
+            request_count = 0
+            next_server = None
+            received_auth = None
+
+            def do_GET(self):
+                if re.match(r"^/$", self.path):
+                    self.__class__.request_count += 1
+                    logger.error("Received request to / (%s)", self.path)
+                    self.__class__.received_auth = self.headers.get("X-Auth-Token", None)
+                    self.send_response(301)
+                    self.send_header(
+                        "Content-Type", "application/json; charset=utf-8"
+                    )
+                    logger.error("Redirecting to %s", self.__class__.next_server)
+                    self.send_header("Location", self.__class__.next_server)
+                    self.end_headers()
+                elif re.match(f"/{url_path}", self.path):
+                    self.__class__.request_count += 1
+                    logger.error("Received request to '%s'", url_path)
+                    self.__class__.received_auth = self.headers.get("X-Auth-Token", None)
+                    self.send_response(200)
+                    self.send_header(
+                        "Content-Type", "application/json; charset=utf-8"
+                    )
+                    # self.send_header("Location", self.__class__.next_server)
+                    self.end_headers()
+
+                return
+
+        test_server = self.start_mock_server(FirstMockServerRequestHandler)
+
+        logger.error("Target: %s", FirstMockServerRequestHandler.server_address)
+
+        base_url = f"http://{FirstMockServerRequestHandler.server_address}/"
+        target_url = f"http://{FirstMockServerRequestHandler.server_address}/{url_path}"
+
+        FirstMockServerRequestHandler.next_server = target_url
+
+        expected_auth_value = custom_auth_token_one
+
+        expected_request_count = 2
+
+        test_class = self.parameters["test_class"]
+
+        if hasattr(test_class, "_instances"):
+            test_class._instances = {}
+
+        test_instance = test_class(base_url=base_url)
+
+        # TODO - Add test_instance.custom_auth_header attribute/setter. For each custom auth header,
+        #   remove the key using the new remove_custom_auth_header hook
+        # test_instance.http.headers.update({"X-Auth-Token": custom_auth_token_one, "Authorization": custom_auth_token_one})
+        test_instance.auth_headers = {
+            "X-Auth-Token": custom_auth_token_one,
+            "Authorization": custom_auth_token_one
+        }
+
+
+        try:
+            test_instance.get("/")
+        except Exception as err:
+            self.failed(f"Unexpected exception was raised:\n{err}")
+        finally:
+            self.start_mock_server(test_server)
+
+        assert FirstMockServerRequestHandler.request_count == expected_request_count, \
+            f"Expected first server to reflect {expected_request_count} requests, " \
+            f"Actual was {FirstMockServerRequestHandler.request_count}"
+        assert FirstMockServerRequestHandler.received_auth == custom_auth_token_one, \
+            f"First server expected auth header '{custom_auth_token_one}', " \
+            f"server received {FirstMockServerRequestHandler.received_auth}"
+        assert FirstMockServerRequestHandler.received_auth is not None, \
+            f"On redirect to the same host, Authorization header should be present. " \
+            f"Instead, server received {FirstMockServerRequestHandler.received_auth}"
+
+    @aetest.test
     def test_custom_auth_class(self, url_path, custom_auth_token_one, basic_auth_username, basic_auth_password):
         class AuthMockServerRequestHandler(BaseHTTPRequestHandler):
             server_address = None
             request_count = 0
             received_auth = None
 
             def do_GET(self):
@@ -565,15 +719,16 @@
                 if response.status_code == 401:
                     # test_instance.http.auth.reauth()
                     test_instance.reauth()
                     logger.error("Resending request...")
                     return test_instance.http.send(response.request)
 
         # test_instance.add_response_hooks(auth_response_hook)
-        test_instance.replace_response_hooks(auth_response_hook)
+        # test_instance.replace_response_hooks(auth_response_hook)
+        test_instance.response_hooks = auth_response_hook
 
         try:
             test_instance.get(target_url)
             test_instance.get(target_url)
             # test_instance.get(f"http://{TargetMockServerRequestHandler.server_address}/noplace")
         except Exception as err:
             self.failed(f"Unexpected exception caught with custom auth class:\n{err}")
@@ -725,15 +880,16 @@
                 if response.status_code == 401:
                     test_instance.reauth()
                     return test_instance.request(response.request.method,
                                                  response.request.url,
                                                  data=response.request.body)
 
         # test_instance.add_response_hooks(auth_response_hook)
-        test_instance.replace_response_hooks(auth_response_hook)
+        # test_instance.replace_response_hooks(auth_response_hook)
+        test_instance.response_hooks = auth_response_hook
 
         try:
             test_instance.get(url_path)
         except requests.exceptions.RetryError:
             logger.info("Expected RetryError was caught, continuing")
         else:
             self.failed("RetryError was NOT caught, failing early.")
```

### Comparing `restsession-0.0.1/tests/test_code.py` & `restsession-0.0.2/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.1/tests/test_redirects.py` & `restsession-0.0.2/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.1/tests/test_requests.py` & `restsession-0.0.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `restsession-0.0.1/tests/test_retries.py` & `restsession-0.0.2/tests/test_retries.py`

 * *Files identical despite different names*

