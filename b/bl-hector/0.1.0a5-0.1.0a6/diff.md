# Comparing `tmp/bl_hector-0.1.0a5.tar.gz` & `tmp/bl_hector-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a5.tar", max compression
+gzip compressed data, was "bl_hector-0.1.0a6.tar", max compression
```

## Comparing `bl_hector-0.1.0a5.tar` & `bl_hector-0.1.0a6.tar`

### file list

```diff
@@ -1,91 +1,93 @@
--rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     1264 2023-06-09 06:16:19.346310 bl_hector-0.1.0a5/README.md
--rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3639 2023-06-11 08:10:05.209290 bl_hector-0.1.0a5/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a5/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     3480 2023-06-13 07:05:26.339251 bl_hector-0.1.0a5/bl_hector/application/use_cases/import_books.py
--rw-r--r--   0        0        0     1979 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3755 2023-06-11 08:06:35.483796 bl_hector-0.1.0a5/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3612 2023-06-11 08:06:35.483796 bl_hector-0.1.0a5/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a5/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a5/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1449 2023-06-09 06:16:19.350310 bl_hector-0.1.0a5/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/exceptions.py
--rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1083 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1804 2023-06-11 08:06:35.483796 bl_hector-0.1.0a5/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1179 2023-06-13 06:14:28.110892 bl_hector-0.1.0a5/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3406 2023-06-11 08:06:35.487796 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4016 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3382 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-13 05:56:18.671790 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1657 2023-06-13 07:05:26.339251 bl_hector-0.1.0a5/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     1940 2023-06-09 07:15:18.620217 bl_hector-0.1.0a5/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7982 2023-06-11 17:37:17.410696 bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2899 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1393 2023-06-13 05:56:18.671790 bl_hector-0.1.0a5/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a5/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a5/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a5/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a5/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4319 2023-06-13 07:47:48.043738 bl_hector-0.1.0a5/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     4883 2023-06-13 07:48:17.027454 bl_hector-0.1.0a5/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14797 2023-06-13 07:13:35.057254 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-09 13:26:25.425148 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4296 2023-06-13 07:51:28.000402 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     1932 2023-06-13 05:56:18.675790 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2048 2023-06-11 09:09:06.457902 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5637 2023-06-13 05:56:18.675790 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3589 2023-06-13 07:51:41.800213 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2026 2023-06-09 13:26:33.641053 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4134 2023-06-11 08:39:27.744213 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-09 13:26:48.248884 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     4445 2023-06-11 08:06:35.487796 bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1455 2023-06-13 07:53:58.226495 bl_hector-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     3895 2023-06-13 07:55:04.825786 bl_hector-0.1.0a5/setup.py
--rw-r--r--   0        0        0     2258 2023-06-13 07:55:04.826726 bl_hector-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     1507 2023-06-13 08:52:57.770248 bl_hector-0.1.0a6/README.md
+-rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3639 2023-06-11 08:10:05.209290 bl_hector-0.1.0a6/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a6/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     3480 2023-06-13 07:05:26.339251 bl_hector-0.1.0a6/bl_hector/application/use_cases/import_books.py
+-rw-r--r--   0        0        0     1979 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3755 2023-06-11 08:06:35.483796 bl_hector-0.1.0a6/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3612 2023-06-11 08:06:35.483796 bl_hector-0.1.0a6/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a6/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a6/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1449 2023-06-09 06:16:19.350310 bl_hector-0.1.0a6/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/exceptions.py
+-rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1083 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1804 2023-06-11 08:06:35.483796 bl_hector-0.1.0a6/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1179 2023-06-13 06:14:28.110892 bl_hector-0.1.0a6/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3706 2023-06-13 09:04:29.650237 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4016 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3382 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
+-rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
+-rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2112 2023-06-13 09:33:38.004683 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-13 08:24:56.879217 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1657 2023-06-13 07:05:26.339251 bl_hector-0.1.0a6/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-13 09:42:06.790266 bl_hector-0.1.0a6/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7982 2023-06-11 17:37:17.410696 bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2899 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1393 2023-06-13 05:56:18.671790 bl_hector-0.1.0a6/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a6/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a6/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a6/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a6/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4466 2023-06-13 09:26:06.278457 bl_hector-0.1.0a6/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5058 2023-06-13 09:25:56.630581 bl_hector-0.1.0a6/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14797 2023-06-13 07:13:35.057254 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-09 13:26:25.425148 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4296 2023-06-13 07:51:28.000402 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     1966 2023-06-13 08:41:29.126612 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2048 2023-06-11 09:09:06.457902 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5607 2023-06-13 08:41:29.126612 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3589 2023-06-13 08:34:41.343554 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2026 2023-06-09 13:26:33.641053 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4134 2023-06-11 08:39:27.744213 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-09 13:26:48.248884 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1400 2023-06-13 09:27:19.501527 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     4445 2023-06-11 08:06:35.487796 bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1516 2023-06-13 09:42:40.769842 bl_hector-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     4246 2023-06-13 09:43:16.433995 bl_hector-0.1.0a6/setup.py
+-rw-r--r--   0        0        0     2560 2023-06-13 09:43:16.434902 bl_hector-0.1.0a6/PKG-INFO
```

### Comparing `bl_hector-0.1.0a5/LICENSE` & `bl_hector-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/README.md` & `bl_hector-0.1.0a6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 To enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)
 and enable it explicitly:
 
 ```console
 $ export HECTOR_WEBAUTHN=1
 ```
 
+To enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)
+and enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):
+
+```console
+$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+```
 
 ## Initialise
 
 Once configured, you must initialise Hector's database with the dedicated command:
 
 ```console
 $ hector init-db
```

### Comparing `bl_hector-0.1.0a5/bl_hector/__init__.py` & `bl_hector-0.1.0a6/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/__init__.py` & `bl_hector-0.1.0a6/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/import_books.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/import_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.0a6/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/configuration/__init__.py` & `bl_hector-0.1.0a6/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/configuration/cli.py` & `bl_hector-0.1.0a6/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.0a6/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/__init__.py` & `bl_hector-0.1.0a6/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.0a6/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.0a6/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.1.0a6/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.0a6/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/administration/services.py` & `bl_hector-0.1.0a6/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.0a6/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/exceptions.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.0a6/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,21 @@
     if settings.WEBAUTHN:
         from bl_hector.infrastructure.flask.webauthn import blueprint as webauthn
 
         app.register_blueprint(webauthn, url_prefix="/auth/webauthn")
         app.auth_links.append(  # type: ignore[attr-defined]
             {"route": "webauthn.login", "label": "WebAuthn", "icon": "key"}
         )
+    if settings.TOTP:
+        from bl_hector.infrastructure.flask.totp import blueprint as totp
+
+        app.register_blueprint(totp, url_prefix="/auth/totp")
+        app.auth_links.append(  # type: ignore[attr-defined]
+            {"route": "totp.login", "label": "TOTP", "icon": "clock"}
+        )
 
 
 def register_jinja_globals() -> None:
     from bl_hector.interfaces.to_http import as_html as presenters
 
     presenters.register_jinja_global("version", __version__)
     presenters.register_jinja_global("url_for", url_for)
```

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,18 +35,25 @@
 
     PROXIED: bool = False
     """To let Flask know that it runs behind a proxy.
     See: <https://flask.palletsprojects.com/en/2.3.x/deploying/proxy_fix/>.
     """
 
     WEBAUTHN: bool = False
-    """To WebAuthn authentication.
+    """To enable WebAuthn authentication.
     Extra dependencies must be installed: `bl-hector[webauthn]`.
     """
 
+    TOTP: str = ""
+    """The secret key for TOTP authentication.
+
+    Extra dependencies must be installed: `bl-hector[totp]`.
+    It can be generated with `pyotp.random_base32()`.
+    """
+
 
 @dataclass(frozen=True)
 class CliSettings(bl_seth.Settings):
     DSN: str
     """The data source name to access the database.
     See: <https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls>."""
```

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.0a6/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/exceptions.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.0a6/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,19 @@
 webauthn-register-success = Your security device has been succesfully registered!
 webauthn-register-failure = Your security device could not be registered!?
 
 webauthn-login-title = Log in
 webauthn-login-description = Your browser should be asking you to tap your security device…
 webauthn-login-failure = You couldn't be logged in!?
 
+totp-login-title = Log in
+totp-login-description = Please enter your one-time password.
+totp-login-password = Password
+totp-login-action = Log in
+
 add-book-requires-authentification = You must be authenticated before adding a book!
 add-book-title = Add a new book to the collection
 add-book-action = Add a book
 add-book-cancel = Cancel
 add-book-add = Add
 add-book-cover-help = Click to upload a cover
 add-book-cover-format-not-supported = The format of this cover is not supported!
```

#### html2text {}

```diff
@@ -30,26 +30,28 @@
 method (string) The sign in method auth-login-method = Sign in using { $method
 } webauthn-register-title = Device registration webauthn-register-description =
 Your browser should be asking you to tap your security deviceâ¦ webauthn-
 register-success = Your security device has been succesfully registered!
 webauthn-register-failure = Your security device could not be registered!?
 webauthn-login-title = Log in webauthn-login-description = Your browser should
 be asking you to tap your security deviceâ¦ webauthn-login-failure = You
-couldn't be logged in!? add-book-requires-authentification = You must be
-authenticated before adding a book! add-book-title = Add a new book to the
-collection add-book-action = Add a book add-book-cancel = Cancel add-book-add =
-Add add-book-cover-help = Click to upload a cover add-book-cover-format-not-
-supported = The format of this cover is not supported! search-books-title =
-Search for a book search-books-action = Look up book search-books-clear = Clear
-search-books-search = Search search-books-no-result = No matching book! search-
-books-previous-page = Previous search-books-next-page = Next # title (string)
-The title of the book display-book-title = Details for "{ $title }" update-
-book-requires-authentification = You must be authenticated before editing a
-book! # isbn (string) The ISBN of the book update-book-title = Edit information
-for `{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
+couldn't be logged in!? totp-login-title = Log in totp-login-description =
+Please enter your one-time password. totp-login-password = Password totp-login-
+action = Log in add-book-requires-authentification = You must be authenticated
+before adding a book! add-book-title = Add a new book to the collection add-
+book-action = Add a book add-book-cancel = Cancel add-book-add = Add add-book-
+cover-help = Click to upload a cover add-book-cover-format-not-supported = The
+format of this cover is not supported! search-books-title = Search for a book
+search-books-action = Look up book search-books-clear = Clear search-books-
+search = Search search-books-no-result = No matching book! search-books-
+previous-page = Previous search-books-next-page = Next # title (string) The
+title of the book display-book-title = Details for "{ $title }" update-book-
+requires-authentification = You must be authenticated before editing a book! #
+isbn (string) The ISBN of the book update-book-title = Edit information for `
+{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
 updated! update-book-success = Book has been updated! update-book-cancel =
 Cancel update-book-update = Save update-book-cover-help = Click to upload a new
 cover update-book-cover-format-not-supported = The format of this cover is not
 supported! book-already-exists = Book already in the collection! # isbn
 (string) The ISBN of the book # url (string) The URL of the book book-added =
 Book {_$isbn_} successfully added! book-not-found = Book not found! book-
 cannot-be-added = The book cannot be added! books-cannot-be-found = The search
```

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.0a6/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,19 @@
 webauthn-register-success = Votre dispositif de sécurité a été correctement associé !
 webauthn-register-failure = Votre dispositif de sécurité n'a pas pu être associé !?
 
 webauthn-login-title = Connexion
 webauthn-login-description = Votre navigateur devrait être en train de vous demander de toucher votre dispositif de sécurité…
 webauthn-login-failure = Vous n'avez pas pu être connecté·e !?
 
+totp-login-title = Connexion
+totp-login-description = Merci de saisir votre mot de passe à usage unique.
+totp-login-password = Mot de passe
+totp-login-action = Se connecter
+
 add-book-requires-authentification = Vous devez être authentifié·e pour pouvoir ajouter un livre !
 add-book-title = Ajouter un nouveau livre à la collection
 add-book-action = Ajouter un livre
 add-book-cancel = Annuler
 add-book-add = Ajouter
 add-book-cover-help = Cliquez pour téléverser une couverture
 add-book-cover-format-not-supported = Le format de cette couverture n'est pas supporté !
```

#### html2text {}

```diff
@@ -34,30 +34,33 @@
 de sÃ©curitÃ© webauthn-register-description = Votre navigateur devrait Ãªtre en
 train de vous demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-
 register-success = Votre dispositif de sÃ©curitÃ© a Ã©tÃ© correctement
 associÃ©Â ! webauthn-register-failure = Votre dispositif de sÃ©curitÃ© n'a pas
 pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion webauthn-login-
 description = Votre navigateur devrait Ãªtre en train de vous demander de
 toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure = Vous n'avez
-pas pu Ãªtre connectÃ©Â·eÂ !? add-book-requires-authentification = Vous devez
-Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-title = Ajouter
-un nouveau livre Ã  la collection add-book-action = Ajouter un livre add-book-
-cancel = Annuler add-book-add = Ajouter add-book-cover-help = Cliquez pour
-tÃ©lÃ©verser une couverture add-book-cover-format-not-supported = Le format de
-cette couverture n'est pas supportÃ©Â ! search-books-title = Chercher un livre
-dans la collection search-books-action = Chercher un livre search-books-clear =
-RÃ©initialiser search-books-search = Chercher search-books-no-result = Aucun
-livre ne correspondÂ ! search-books-previous-page = PrÃ©cÃ©dent search-books-
-next-page = Suivant # title (string) The title of the book display-book-title =
-DÃ©tails pour Â«Â { $title }Â Â» update-book-requires-authentification = Vous
-devez Ãªtre authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string)
-The ISBN of the book update-book-title = Ãditer les informations de `{ $isbn
-}` update-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre
-mis Ã  jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ !
-update-book-cancel = Annuler update-book-update = Enregistrer update-book-
-cover-help = Cliquez pour tÃ©lÃ©verser une nouvelle couverture update-book-
-cover-format-not-supported = Le format de cette couverture n'est pas
-supportÃ©Â ! book-already-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! #
-isbn (string) The ISBN of the book # url (string) The URL of the book book-
-added = Le livre {_$isbn_} a bien Ã©tÃ© ajoutÃ©Â ! book-not-found = Le livre
-n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-added = Le livre n'a pas pu Ãªtre
-ajoutÃ©Â ! books-cannot-be-found = La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
+pas pu Ãªtre connectÃ©Â·eÂ !? totp-login-title = Connexion totp-login-
+description = Merci de saisir votre mot de passe Ã  usage unique. totp-login-
+password = Mot de passe totp-login-action = Se connecter add-book-requires-
+authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un
+livreÂ ! add-book-title = Ajouter un nouveau livre Ã  la collection add-book-
+action = Ajouter un livre add-book-cancel = Annuler add-book-add = Ajouter add-
+book-cover-help = Cliquez pour tÃ©lÃ©verser une couverture add-book-cover-
+format-not-supported = Le format de cette couverture n'est pas supportÃ©Â !
+search-books-title = Chercher un livre dans la collection search-books-action =
+Chercher un livre search-books-clear = RÃ©initialiser search-books-search =
+Chercher search-books-no-result = Aucun livre ne correspondÂ ! search-books-
+previous-page = PrÃ©cÃ©dent search-books-next-page = Suivant # title (string)
+The title of the book display-book-title = DÃ©tails pour Â«Â { $title }Â Â»
+update-book-requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour
+pouvoir Ã©diter un livreÂ ! # isbn (string) The ISBN of the book update-book-
+title = Ãditer les informations de `{ $isbn }` update-book-action = Ãditer
+update-book-failure = Le livre n'a pas pu Ãªtre mis Ã  jourÂ ! update-book-
+success = Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-cancel = Annuler
+update-book-update = Enregistrer update-book-cover-help = Cliquez pour
+tÃ©lÃ©verser une nouvelle couverture update-book-cover-format-not-supported =
+Le format de cette couverture n'est pas supportÃ©Â ! book-already-exists = Ce
+livre est dÃ©jÃ  dans la collectionÂ ! # isbn (string) The ISBN of the book #
+url (string) The URL of the book book-added = Le livre {_$isbn_} a bien Ã©tÃ©
+ajoutÃ©Â ! book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-
+added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La
+recherche n'a pas pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 
 block title
   title= _("hector") + " – " + _("display-book-title", title=book.title)
 
 block content
   section.section
     .container
+      //- Fixes a spacing problem.
+      .buttons.is-pulled-right(style="margin-bottom: -1rem")
+        if user.can_update_book
+          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
+            span.icon: i.fas.fa-edit
+            span= _("update-book-action")
+        else
+          button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
+            span.icon: i.fas.fa-edit
+            span= _("update-book-action")
 
-      h1.title.is-3
-        span= book.title
-        .buttons.is-pulled-right
-          if user.can_update_book
-            a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
-              span.icon: i.fas.fa-edit
-              span= _("update-book-action")
-          else
-            button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
-              span.icon: i.fas.fa-edit
-              span= _("update-book-action")
+      h1.title.is-3= book.title
 
       .columns
         .column.is-one-quarter
           img#cover.cover.is-2by3(
             src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}"
             alt="Book cover"
           )
```

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 
 block title
   title= _("hector") + " – " + _("search-books-title")
 
 block content
   section.section
     .container
-      h1.title.is-3
-        span= _("search-books-title")
-        .buttons.is-pulled-right
-          if user.can_add_book
-            a.button.is-link(href="#{url_for('books.add')}")
-              span.icon: i.fas.fa-plus
-              span= _("add-book-action")
-          else
-            button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
-              span.icon: i.fas.fa-plus
-              span= _("add-book-action")
+      .buttons.is-pulled-right
+        if user.can_add_book
+          a.button.is-link(href="#{url_for('books.add')}")
+            span.icon: i.fas.fa-plus
+            span= _("add-book-action")
+        else
+          button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
+            span.icon: i.fas.fa-plus
+            span= _("add-book-action")
+
+      h1.title.is-3= _("search-books-title")
 
       #form
         block form
           include mixins/form
           form(
             method="GET"
             action="#{url_for('books.search')}"
```

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/bl_hector/interfaces/utils.py` & `bl_hector-0.1.0a6/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a5/pyproject.toml` & `bl_hector-0.1.0a6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.5"
+version = "0.1.0-alpha.6"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
@@ -27,14 +27,15 @@
 jinja2-fragments = "^0.3.0"
 SQLAlchemy = "^2.0.15"
 typer = "^0.9.0"
 bl3d = "^0.3.0"
 "fluent.runtime" = "^0.4.0"
 webauthn = {version = "^1.8.1", optional = true}
 requests = "^2.31.0"
+pyotp = {version = "^2.8.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 robber = "^1.1.5"
 invoke = "^2.1.1"
 flake8 = "^6.0.0"
 black = "^23.3.0"
@@ -46,14 +47,15 @@
 beautifulsoup4 = "^4.12.2"
 types-beautifulsoup4 = "^4.12.0"
 behave = "^1.2.6"
 types-requests = "^2.31.0"
 
 [tool.poetry.extras]
 webauthn = ["webauthn"]
+totp = ["otp"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 line-length = 89
```

### Comparing `bl_hector-0.1.0a5/setup.py` & `bl_hector-0.1.0a6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
  'bl_hector.domain.administration',
  'bl_hector.domain.collection_management',
  'bl_hector.infrastructure',
  'bl_hector.infrastructure.flask',
  'bl_hector.infrastructure.flask.aliases',
  'bl_hector.infrastructure.flask.auth',
  'bl_hector.infrastructure.flask.books',
+ 'bl_hector.infrastructure.flask.totp',
  'bl_hector.infrastructure.flask.webauthn',
  'bl_hector.infrastructure.isbnlib',
  'bl_hector.infrastructure.requests',
  'bl_hector.infrastructure.sqlalchemy',
  'bl_hector.infrastructure.typer',
  'bl_hector.interfaces',
  'bl_hector.interfaces.l10n',
@@ -35,14 +36,15 @@
                                     'static/webfonts/*'],
  'bl_hector.interfaces.l10n': ['en-GB/*', 'fr-FR/*'],
  'bl_hector.interfaces.to_http.as_html': ['templates/*',
                                           'templates/auth/*',
                                           'templates/books/*',
                                           'templates/books/mixins/*',
                                           'templates/mixins/*',
+                                          'templates/totp/*',
                                           'templates/webauthn/*']}
 
 install_requires = \
 ['Flask>=2.3.2,<3.0.0',
  'SQLAlchemy>=2.0.15,<3.0.0',
  'bl-seth>=0.1.2,<0.2.0',
  'bl3d>=0.3.0,<0.4.0',
@@ -57,17 +59,17 @@
 {'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a5',
+    'version': '0.1.0a6',
     'description': 'A collection manager.',
-    'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
+    'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\nTo enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):\n\n```console\n$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bl_hector-0.1.0a5/PKG-INFO` & `bl_hector-0.1.0a6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: A collection manager.
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: totp
 Provides-Extra: webauthn
 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: bl-seth (>=0.1.2,<0.2.0)
 Requires-Dist: bl3d (>=0.3.0,<0.4.0)
 Requires-Dist: fluent.runtime (>=0.4.0,<0.5.0)
 Requires-Dist: isbnlib (>=3.10.14,<4.0.0)
 Requires-Dist: jinja2-fragments (>=0.3.0,<0.4.0)
+Requires-Dist: pyotp (>=2.8.0,<3.0.0)
 Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: webauthn (>=1.8.1,<2.0.0); extra == "webauthn"
 Description-Content-Type: text/markdown
 
 # Hector — a collection manager
@@ -56,14 +58,20 @@
 To enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)
 and enable it explicitly:
 
 ```console
 $ export HECTOR_WEBAUTHN=1
 ```
 
+To enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)
+and enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):
+
+```console
+$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
+```
 
 ## Initialise
 
 Once configured, you must initialise Hector's database with the dedicated command:
 
 ```console
 $ hector init-db
```

