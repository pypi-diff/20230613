# Comparing `tmp/esmerald-1.2.4.tar.gz` & `tmp/esmerald-1.2.5.tar.gz`

## Comparing `esmerald-1.2.4.tar` & `esmerald-1.2.5.tar`

### file list

```diff
@@ -1,189 +1,189 @@
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/__init__.py
--rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/enums.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/injector.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/param_functions.py
--rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/params.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/py.typed
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/staticfiles.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/testclient.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/websockets.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/openapi.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/session.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/static_files.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/crypto.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/tortoise/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/tortoise/base_user.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/auth/tortoise/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/databases/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/contrib/databases/tortoise/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/base.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/protocols/template.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/base.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/base.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/events.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/router.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/model.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/transformers/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/urls/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/urls/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/pydantic.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/sync.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/timezone.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.4/esmerald/utils/url.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.4/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.4/LICENSE
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 esmerald-1.2.4/README.md
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 esmerald-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    20202 2020-02-02 00:00:00.000000 esmerald-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/__init__.py
+-rw-r--r--   0        0        0    32066 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/concurrency.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/enums.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/injector.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/logging.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/param_functions.py
+-rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/params.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/py.typed
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/testclient.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/types.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/websockets.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/session.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/crypto.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/tortoise/__init__.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/tortoise/base_user.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/auth/tortoise/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/databases/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/contrib/databases/tortoise/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/apiview.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/parameters.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/path_item.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/request_body.py
+-rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/schema.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/types.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/router.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/urls/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/urls/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/pydantic.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/sync.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/timezone.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.5/esmerald/utils/url.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.5/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.5/LICENSE
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 esmerald-1.2.5/README.md
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 esmerald-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    20202 2020-02-02 00:00:00.000000 esmerald-1.2.5/PKG-INFO
```

### Comparing `esmerald-1.2.4/esmerald/__init__.py` & `esmerald-1.2.5/esmerald/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-1.2.4/esmerald/applications.py` & `esmerald-1.2.5/esmerald/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,16 +420,14 @@
         if local_settings:
             setting_value = getattr(local_settings, value, None)
         if not setting_value:
             return getattr(global_settings, value, None)
         return setting_value
 
     def activate_openapi(self) -> None:
-        pass
-
         if self.openapi_config and self.enable_openapi:
             self.openapi_schema = self.openapi_config.create_openapi_schema_model(self)
             gateway = gateways.Gateway(handler=self.openapi_config.openapi_apiview)
             self.add_apiview(value=gateway)
 
     def get_template_engine(
         self, template_config: "TemplateConfig"
@@ -504,14 +502,19 @@
             exception_handlers=exception_handlers,
             interceptors=interceptors,
             permissions=permissions,
             middleware=middleware,
             name=name,
         )
 
+    def add_include(self, include: Include) -> None:
+        """Adds an include directly to the active application router"""
+        self.router.routes.append(include)
+        self.activate_openapi()
+
     def add_child_esmerald(
         self,
         path: str,
         child: "ChildEsmerald",
         name: Optional[str] = None,
         middleware: Optional[Sequence["Middleware"]] = None,
         dependencies: Optional["Dependencies"] = None,
@@ -821,22 +824,14 @@
             await self.router.lifespan(scope, receive, send)
             return
         if self.root_path:
             scope["root_path"] = self.root_path
         scope["state"] = {}
         await super().__call__(scope, receive, send)
 
-    def mount(self, path: str, app: ASGIApp, name: Optional[str] = None) -> None:
-        raise ImproperlyConfigured("`mount` is not supported by Esmerald. Use Include() instead.")
-
-    def host(self, host: str, app: ASGIApp, name: Optional[str] = None) -> None:
-        raise ImproperlyConfigured(
-            "`host` is not supported by Esmerald. Use Starlette Host() instead."
-        )
-
     def route(
         self,
         path: str,
         methods: Optional[List[str]] = None,
         name: Optional[str] = None,
         include_in_schema: bool = True,
     ) -> Callable:
```

### Comparing `esmerald-1.2.4/esmerald/backgound.py` & `esmerald-1.2.5/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/enums.py` & `esmerald-1.2.5/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/exception_handlers.py` & `esmerald-1.2.5/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/exceptions.py` & `esmerald-1.2.5/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/injector.py` & `esmerald-1.2.5/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/logging.py` & `esmerald-1.2.5/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/params.py` & `esmerald-1.2.5/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/parsers.py` & `esmerald-1.2.5/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/requests.py` & `esmerald-1.2.5/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/testclient.py` & `esmerald-1.2.5/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/types.py` & `esmerald-1.2.5/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/websockets.py` & `esmerald-1.2.5/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/__init__.py` & `esmerald-1.2.5/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/global_settings.py` & `esmerald-1.2.5/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-1.2.5/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-1.2.5/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-1.2.5/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-1.2.5/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-1.2.5/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-1.2.5/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/config/jwt.py` & `esmerald-1.2.5/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/config/openapi.py` & `esmerald-1.2.5/esmerald/config/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     def create_openapi_schema_model(self, app: Type["Esmerald"]) -> "OpenAPI":
         from esmerald.applications import ChildEsmerald, Esmerald
 
         schema = self.to_openapi_schema()
         schema.paths = {}
 
         def parse_route(app, prefix=""):
-            if not app.routes:
+            if getattr(app, "routes", None) is None:
                 return
 
             # Making sure that ChildEsmerald or esmerald
             if hasattr(app, "app"):
                 if (
                     isinstance(app.app, (Esmerald, ChildEsmerald))
                     or (
```

### Comparing `esmerald-1.2.4/esmerald/config/session.py` & `esmerald-1.2.5/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/config/static_files.py` & `esmerald-1.2.5/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/encoding.py` & `esmerald-1.2.5/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/auth/hashers.py` & `esmerald-1.2.5/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/auth/common/middleware.py` & `esmerald-1.2.5/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-1.2.5/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-1.2.5/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/auth/tortoise/base_user.py` & `esmerald-1.2.5/esmerald/contrib/auth/tortoise/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/auth/tortoise/middleware.py` & `esmerald-1.2.5/esmerald/contrib/auth/tortoise/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/contrib/databases/tortoise/__init__.py` & `esmerald-1.2.5/esmerald/contrib/databases/tortoise/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/base.py` & `esmerald-1.2.5/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/cli.py` & `esmerald-1.2.5/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/env.py` & `esmerald-1.2.5/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/templates.py` & `esmerald-1.2.5/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/utils.py` & `esmerald-1.2.5/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/operations/createapp.py` & `esmerald-1.2.5/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/operations/createproject.py` & `esmerald-1.2.5/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/operations/list.py` & `esmerald-1.2.5/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/operations/run.py` & `esmerald-1.2.5/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/operations/runserver.py` & `esmerald-1.2.5/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/directives/operations/show_urls.py` & `esmerald-1.2.5/esmerald/core/directives/operations/show_urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     table.add_column("Path", style=OutputColour.GREEN, vertical="center")
     table.add_column("Path Parameters", style=OutputColour.BRIGHT_CYAN, vertical="center")
     table.add_column("Name", style=OutputColour.CYAN, vertical="center")
     table.add_column("Type", style=OutputColour.YELLOW, vertical="center")
     table.add_column("HTTP Methods", style=OutputColour.RED, vertical="center")
 
     def parse_routes(app, table: table, route: Optional[Any] = None, prefix: Optional[str] = ""):
-        if not app.routes:
+        if getattr(app, "routes", None) is None:
             return
 
         for route in app.routes:
             if isinstance(route, Gateway):
                 # Path
                 path = clean_path(prefix + route.path)
```

### Comparing `esmerald-1.2.4/esmerald/core/terminal/base.py` & `esmerald-1.2.5/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/terminal/print.py` & `esmerald-1.2.5/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/core/terminal/terminal.py` & `esmerald-1.2.5/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/__init__.py` & `esmerald-1.2.5/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/base.py` & `esmerald-1.2.5/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/encoders.py` & `esmerald-1.2.5/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/file.py` & `esmerald-1.2.5/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/json.py` & `esmerald-1.2.5/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/redirect.py` & `esmerald-1.2.5/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/stream.py` & `esmerald-1.2.5/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/datastructures/template.py` & `esmerald-1.2.5/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/interceptors/interceptor.py` & `esmerald-1.2.5/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/__init__.py` & `esmerald-1.2.5/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/_exception_handlers.py` & `esmerald-1.2.5/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/asyncexitstack.py` & `esmerald-1.2.5/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/authentication.py` & `esmerald-1.2.5/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/basic.py` & `esmerald-1.2.5/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/csrf.py` & `esmerald-1.2.5/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/errors.py` & `esmerald-1.2.5/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/exceptions.py` & `esmerald-1.2.5/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/middleware/settings_middleware.py` & `esmerald-1.2.5/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/apiview.py` & `esmerald-1.2.5/esmerald/openapi/apiview.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/enums.py` & `esmerald-1.2.5/esmerald/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/parameters.py` & `esmerald-1.2.5/esmerald/openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/path_item.py` & `esmerald-1.2.5/esmerald/openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/request_body.py` & `esmerald-1.2.5/esmerald/openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/responses.py` & `esmerald-1.2.5/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/schema.py` & `esmerald-1.2.5/esmerald/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/openapi/utils.py` & `esmerald-1.2.5/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/permissions/base.py` & `esmerald-1.2.5/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/permissions/utils.py` & `esmerald-1.2.5/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/pluggables/base.py` & `esmerald-1.2.5/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/protocols/asyncdao.py` & `esmerald-1.2.5/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/protocols/dao.py` & `esmerald-1.2.5/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/protocols/interceptor.py` & `esmerald-1.2.5/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/protocols/template.py` & `esmerald-1.2.5/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/responses/base.py` & `esmerald-1.2.5/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/responses/encoders.py` & `esmerald-1.2.5/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/responses/json.py` & `esmerald-1.2.5/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/responses/template.py` & `esmerald-1.2.5/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/routing/base.py` & `esmerald-1.2.5/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/routing/events.py` & `esmerald-1.2.5/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/routing/gateways.py` & `esmerald-1.2.5/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/routing/handlers.py` & `esmerald-1.2.5/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/routing/router.py` & `esmerald-1.2.5/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/routing/views.py` & `esmerald-1.2.5/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/security/jwt/token.py` & `esmerald-1.2.5/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/template/jinja.py` & `esmerald-1.2.5/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/template/mako.py` & `esmerald-1.2.5/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/transformers/datastructures.py` & `esmerald-1.2.5/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/transformers/helpers.py` & `esmerald-1.2.5/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/transformers/model.py` & `esmerald-1.2.5/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/transformers/signature.py` & `esmerald-1.2.5/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/transformers/types.py` & `esmerald-1.2.5/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/transformers/utils.py` & `esmerald-1.2.5/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/urls/base.py` & `esmerald-1.2.5/esmerald/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/constants.py` & `esmerald-1.2.5/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/crypto.py` & `esmerald-1.2.5/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/functional.py` & `esmerald-1.2.5/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/helpers.py` & `esmerald-1.2.5/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/model.py` & `esmerald-1.2.5/esmerald/utils/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/module_loading.py` & `esmerald-1.2.5/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/pydantic.py` & `esmerald-1.2.5/esmerald/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/sync.py` & `esmerald-1.2.5/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/esmerald/utils/timezone.py` & `esmerald-1.2.5/esmerald/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/LICENSE` & `esmerald-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/README.md` & `esmerald-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.4/pyproject.toml` & `esmerald-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "anyio>=3.6.2,<4.0.0",
     "awesome-slugify>=1.6.5,<2",
     "httpx>=0.24.0,<0.30.0",
     "itsdangerous>=2.1.2,<3.0.0",
     "jinja2>=3.1.2,<4.0.0",
     "jsonschema_rs>=0.16.2,<0.20.0",
     "loguru>=0.6.0,<0.7.0",
-    "pydantic>=1.10.7,<2.0.0",
+    "pydantic>=1.10.9,<2.0.0",
     "pydantic-factories==1.17.2",
     "python-multipart>=0.0.5,<0.0.7",
     "openapi-schemas-pydantic>=1.1.0",
     "rich>=13.3.1,<14.0.0",
     "starlette>=0.28.0,<1.0",
 ]
 keywords = [
```

### Comparing `esmerald-1.2.4/PKG-INFO` & `esmerald-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.2.4
+Version: 1.2.5
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -43,15 +43,15 @@
 Requires-Dist: httpx<0.30.0,>=0.24.0
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
 Requires-Dist: jinja2<4.0.0,>=3.1.2
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
 Requires-Dist: loguru<0.7.0,>=0.6.0
 Requires-Dist: openapi-schemas-pydantic>=1.1.0
 Requires-Dist: pydantic-factories==1.17.2
-Requires-Dist: pydantic<2.0.0,>=1.10.7
+Requires-Dist: pydantic<2.0.0,>=1.10.9
 Requires-Dist: python-multipart<0.0.7,>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: starlette<1.0,>=0.28.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
```

