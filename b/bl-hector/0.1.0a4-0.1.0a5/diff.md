# Comparing `tmp/bl_hector-0.1.0a4.tar.gz` & `tmp/bl_hector-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a4.tar", max compression
+gzip compressed data, was "bl_hector-0.1.0a5.tar", max compression
```

## Comparing `bl_hector-0.1.0a4.tar` & `bl_hector-0.1.0a5.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0    34523 2023-06-01 06:44:39.561559 bl_hector-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     1264 2023-06-08 11:40:14.535293 bl_hector-0.1.0a4/README.md
--rw-r--r--   0        0        0      807 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3639 2023-06-12 06:39:33.409846 bl_hector-0.1.0a4/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1981 2023-06-08 13:54:13.278547 bl_hector-0.1.0a4/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     3472 2023-06-08 13:55:05.761614 bl_hector-0.1.0a4/bl_hector/application/use_cases/import_books.py
--rw-r--r--   0        0        0     1846 2023-06-08 13:57:02.571540 bl_hector-0.1.0a4/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3755 2023-06-12 06:39:33.409846 bl_hector-0.1.0a4/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3612 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1449 2023-06-08 14:33:06.629178 bl_hector-0.1.0a4/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/exceptions.py
--rw-r--r--   0        0        0     1509 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0      958 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1804 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3309 2023-06-08 13:46:42.562514 bl_hector-0.1.0a4/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1124 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3406 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     3966 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-08 06:35:01.974074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      584 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-08 06:35:01.978074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1265 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-12 06:52:18.855459 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-12 06:52:18.855459 bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1641 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1940 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7982 2023-06-12 06:52:18.855459 bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2842 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     1866 2023-06-08 06:35:01.982074 bl_hector-0.1.0a4/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1351 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1609 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4049 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     4591 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14491 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4098 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2014 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2048 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5577 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3391 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2026 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1122 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4134 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     2010 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1818 2023-06-08 13:41:47.687677 bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     4445 2023-06-12 06:39:33.413846 bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-08 06:35:01.986074 bl_hector-0.1.0a4/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1407 2023-06-12 06:54:40.105308 bl_hector-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     3829 2023-06-12 06:55:23.850654 bl_hector-0.1.0a4/setup.py
--rw-r--r--   0        0        0     2216 2023-06-12 06:55:23.850896 bl_hector-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     1264 2023-06-09 06:16:19.346310 bl_hector-0.1.0a5/README.md
+-rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3639 2023-06-11 08:10:05.209290 bl_hector-0.1.0a5/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a5/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     3480 2023-06-13 07:05:26.339251 bl_hector-0.1.0a5/bl_hector/application/use_cases/import_books.py
+-rw-r--r--   0        0        0     1979 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3755 2023-06-11 08:06:35.483796 bl_hector-0.1.0a5/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3612 2023-06-11 08:06:35.483796 bl_hector-0.1.0a5/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a5/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a5/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1449 2023-06-09 06:16:19.350310 bl_hector-0.1.0a5/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/exceptions.py
+-rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1083 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1804 2023-06-11 08:06:35.483796 bl_hector-0.1.0a5/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1179 2023-06-13 06:14:28.110892 bl_hector-0.1.0a5/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3406 2023-06-11 08:06:35.487796 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4016 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3382 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
+-rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
+-rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-13 05:56:18.671790 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1657 2023-06-13 07:05:26.339251 bl_hector-0.1.0a5/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     1940 2023-06-09 07:15:18.620217 bl_hector-0.1.0a5/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     7982 2023-06-11 17:37:17.410696 bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a5/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2899 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-13 07:05:37.235116 bl_hector-0.1.0a5/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1393 2023-06-13 05:56:18.671790 bl_hector-0.1.0a5/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a5/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a5/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a5/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a5/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4319 2023-06-13 07:47:48.043738 bl_hector-0.1.0a5/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     4883 2023-06-13 07:48:17.027454 bl_hector-0.1.0a5/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14797 2023-06-13 07:13:35.057254 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-09 13:26:25.425148 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4296 2023-06-13 07:51:28.000402 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     1932 2023-06-13 05:56:18.675790 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2048 2023-06-11 09:09:06.457902 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5637 2023-06-13 05:56:18.675790 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3589 2023-06-13 07:51:41.800213 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2026 2023-06-09 13:26:33.641053 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4134 2023-06-11 08:39:27.744213 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-09 13:26:48.248884 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     4445 2023-06-11 08:06:35.487796 bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a5/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1455 2023-06-13 07:53:58.226495 bl_hector-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     3895 2023-06-13 07:55:04.825786 bl_hector-0.1.0a5/setup.py
+-rw-r--r--   0        0        0     2258 2023-06-13 07:55:04.826726 bl_hector-0.1.0a5/PKG-INFO
```

### Comparing `bl_hector-0.1.0a4/LICENSE` & `bl_hector-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/README.md` & `bl_hector-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/__init__.py` & `bl_hector-0.1.0a5/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/application/__init__.py` & `bl_hector-0.1.0a5/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/import_books.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/import_books.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.repositories import Books
-from bl_hector.domain.collection_management.services import InfoProvider
+from bl_hector.domain.collection_management.services import BookInfoProvider
 from bl_hector.domain.collection_management.value_objects import Isbn
 
 
 @dataclass(frozen=True)
 class Request:
     path: str
 
@@ -60,15 +60,15 @@
     It might be better to implement it by wireing the other commands together.
     This would solve the problem of the commit of the data. For the time being
     the commit only happens once at the end of the command, even if thousands of books
     have to be imported!?
     """
 
     presenter: Presenter
-    info_provider: InfoProvider
+    info_provider: BookInfoProvider
     books: Books
 
     def execute(self, request: Request) -> None:
         path = Path(request.path)
         if not path.is_file():
             return self.presenter.file_does_not_exist(request.path)
```

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/look_up_book.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
-from bl_hector.domain.collection_management.services import InfoProvider
+from bl_hector.domain.collection_management.services import (
+    BookInfoProvider,
+    CoverProvider,
+)
 from bl_hector.domain.collection_management.value_objects import Isbn
 
 
 @dataclass(frozen=True)
 class Request:
     isbn: str
 
@@ -41,18 +44,22 @@
     def book(self, book: Book) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
-    info_provider: InfoProvider
+    info_provider: BookInfoProvider
+    cover_provider: CoverProvider
 
     def execute(self, request: Request) -> None:
         try:
             isbn = Isbn.instanciate(request.isbn)
         except IncorrectValue:
             return self.presenter.not_an_isbn(request.isbn)
 
-        if book := self.info_provider.look_up(isbn):
-            return self.presenter.book(book)
-        return self.presenter.book_not_found(isbn)
+        if not (book := self.info_provider.look_up(isbn)):
+            return self.presenter.book_not_found(isbn)
+
+        book.cover = self.cover_provider.by_isbn(isbn)
+
+        return self.presenter.book(book)
```

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.0a5/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/configuration/__init__.py` & `bl_hector-0.1.0a5/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/configuration/cli.py` & `bl_hector-0.1.0a5/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.0a5/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/__init__.py` & `bl_hector-0.1.0a5/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.0a5/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.0a5/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.1.0a5/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.0a5/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/administration/services.py` & `bl_hector-0.1.0a5/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.0a5/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.0a5/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.0a5/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/exceptions.py` & `bl_hector-0.1.0a5/bl_hector/domain/collection_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.0a5/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from abc import ABC, abstractmethod
-from typing import Optional
 
-from .entities import Book
-from .value_objects import Isbn
-
-
-class InfoProvider(ABC):
-    @abstractmethod
-    def look_up(self, isbn: Isbn) -> Optional[Book]:
-        ...
+class BadRequest(Exception):
+    pass
```

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.1.0a5/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.0a5/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,11 +17,13 @@
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
 
 ONLY_USER = "admin"
 
 
-class FakePermissions(Permissions):
+class DummyPermissions(Permissions):
+    def for_user(self, user_id: UserId) -> list[P]:
+        return [p for p in P]
+
     def is_authorized_to(self, user_id: UserId, permission: P) -> bool:
-        print(repr(user_id))
         return bool(str(user_id))
```

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,17 @@
     return presenter
 
 
 @blueprint.post("__info__")
 @presenter_to_response
 def look_up() -> Any:
     presenter = presenters.LookUpBook(user=services.get_user())
-    interactor = look_up_book.Interactor(presenter, services.get_info_provider())
+    interactor = look_up_book.Interactor(
+        presenter, services.get_book_info_provider(), services.get_cover_provider()
+    )
     interactor.execute(look_up_book.Request(request.form.get("isbn", "")))
     return presenter
 
 
 @blueprint.get("<string:isbn>")
 @presenter_to_response
 def display(isbn: str) -> Any:
```

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from urllib.parse import urlparse
 
 from flask import g, request, session
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Connection
 
 from bl_hector.domain.administration.entities import RelyingParty
-from bl_hector.domain.administration.repositories import Permissions
-from bl_hector.infrastructure import FakePermissions
-from bl_hector.infrastructure.isbnlib import InfoProvider
+from bl_hector.infrastructure import DummyPermissions
+from bl_hector.infrastructure.isbnlib import BookInfoProvider
+from bl_hector.infrastructure.requests import CoverProvider
 from bl_hector.infrastructure.settings import WsgiSettings
 from bl_hector.infrastructure.sqlalchemy.repositories import (
     Books,
     Challenges,
     Credentials,
     Users,
 )
@@ -83,25 +83,35 @@
     return Credentials(get_connection())
 
 
 def get_challenges() -> Challenges:
     return Challenges(get_connection())
 
 
-def get_permissions() -> Permissions:
-    return FakePermissions()
+def get_permissions() -> DummyPermissions:
+    return DummyPermissions()
 
 
-def get_info_provider() -> InfoProvider:
-    return InfoProvider()
+def get_book_info_provider() -> BookInfoProvider:
+    return BookInfoProvider()
+
+
+def get_cover_provider() -> CoverProvider:
+    return CoverProvider()
 
 
 def get_user() -> User:
     if "user" not in g:
-        g.setdefault("user", User(session.get("user_id", ""), g.get("locale", "")))
+        if user_id := session.get("user_id", ""):
+            permissions = get_permissions().for_user(user_id)
+        else:
+            permissions = []
+        locale = g.get("locale", "")
+
+        g.setdefault("user", User(user_id, locale, permissions))
     return g.user  # type: ignore[no-any-return]
 
 
 def get_relying_party() -> RelyingParty:
     return RelyingParty(
         id=str(urlparse(request.base_url).hostname),
         name="hector",
```

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,23 @@
     margin:0;
 }
 
 form {
     margin-bottom: 1em;
 }
 
+dt {
+    font-size: small;
+    color: grey;
+}
+
+dd {
+    margin-bottom: 1rem;
+}
+
 .page {
     flex: 1;
 }
 
 .footer {
     padding: 1.5em;
 }
```

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 import logging
 from typing import Optional
 
 import isbnlib
 
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.services import (
-    InfoProvider as InfoProviderABC,
+    BookInfoProvider as BookInfoProviderABC,
 )
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Isbn,
     Title,
     Year,
 )
 
 
-class InfoProvider(InfoProviderABC):
+class BookInfoProvider(BookInfoProviderABC):
     def look_up(self, isbn: Isbn) -> Optional[Book]:
         try:
             meta = isbnlib.meta(str(isbn))
             if not meta:
                 return None
 
             return Book.instanciate(
```

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/typer/books.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import sys
 
 import typer
 from typing_extensions import Annotated
 
 from bl_hector.application.use_cases import add_book, import_books, look_up_book
-from bl_hector.infrastructure import ONLY_USER, FakePermissions
+from bl_hector.infrastructure import ONLY_USER, DummyPermissions
 from bl_hector.infrastructure.typer import services
 from bl_hector.interfaces import from_json as controllers
 from bl_hector.interfaces.to_terminal import LookUpBookInterface, as_json, as_text
 
 cmd = typer.Typer()
 
 
@@ -38,23 +38,25 @@
     presenter: LookUpBookInterface
     if json:
         presenter = as_json.LookUpBook(lambda m: typer.echo(m))
     else:
         presenter = as_text.LookUpBook(
             lambda m: typer.echo(m), translator=services.get_translator()
         )
-    interactor = look_up_book.Interactor(presenter, services.get_info_provider())
+    interactor = look_up_book.Interactor(
+        presenter, services.get_book_info_provider(), services.get_cover_provider()
+    )
     interactor.execute(look_up_book.Request(isbn))
     raise typer.Exit(presenter.exit_code())
 
 
 @cmd.command()
 def add(ctx: typer.Context) -> None:
     """Add a book to the collection."""
-    permissions = FakePermissions()
+    permissions = DummyPermissions()
     with services.get_books(ctx.obj) as books:
         presenter = as_text.AddBook(
             lambda m: typer.echo(m), translator=services.get_translator()
         )
         interactor = add_book.Interactor(presenter, books, permissions)
         controller = controllers.AddBook(sys.stdin.readline(), ONLY_USER)
         controller.call(interactor)
@@ -65,11 +67,11 @@
 def import_(ctx: typer.Context, path: str) -> None:
     """Import a list of books to the collection."""
     with services.get_books(ctx.obj) as books:
         presenter = as_text.ImportBooks(
             lambda m: typer.echo(m), translator=services.get_translator()
         )
         interactor = import_books.Interactor(
-            presenter, services.get_info_provider(), books
+            presenter, services.get_book_info_provider(), books
         )
         interactor.execute(import_books.Request(path))
         raise typer.Exit(presenter.exit_code())
```

### Comparing `bl_hector-0.1.0a4/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.0a5/bl_hector/infrastructure/typer/services.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,22 +17,27 @@
 import logging
 from contextlib import contextmanager
 from typing import Any, Iterator
 
 from sqlalchemy import create_engine
 from typer import Exit
 
-from bl_hector.infrastructure.isbnlib import InfoProvider
+from bl_hector.infrastructure.isbnlib import BookInfoProvider
+from bl_hector.infrastructure.requests import CoverProvider
 from bl_hector.infrastructure.settings import CliSettings
 from bl_hector.infrastructure.sqlalchemy.repositories import Books
 from bl_hector.interfaces import l10n
 
 
-def get_info_provider() -> InfoProvider:
-    return InfoProvider()
+def get_book_info_provider() -> BookInfoProvider:
+    return BookInfoProvider()
+
+
+def get_cover_provider() -> CoverProvider:
+    return CoverProvider()
 
 
 @contextmanager
 def get_books(settings: CliSettings) -> Iterator[Books]:
     options: dict[str, Any] = {}
     if settings.DEBUG_SQL:
         options["echo"] = True
@@ -51,8 +56,11 @@
         logging.exception(exc)
         connection.rollback()
     else:
         connection.commit()
 
 
 def get_translator() -> l10n.Translator:
-    return l10n.localization(l10n.DEFAULT_LOCALE).format_value  # type: ignore
+    def wrapper(message_id: str, **kwargs: Any) -> str:
+        return l10n.localization(l10n.DEFAULT_LOCALE).format_value(message_id, kwargs)
+
+    return wrapper
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from bl_hector.domain.administration.enumerations import Permissions
 
 
 @dataclass
 class User:
     id: str
     locale: str
+    permissions: list[Permissions]
 
     def __getattribute__(self, name: str) -> Any:
         PREFIX = "can_"
         if name.startswith(PREFIX):
             return self.has_permission(name[len(PREFIX) :].upper())
         return super().__getattribute__(name)
 
     def has_permission(self, permission: str) -> bool:
         if not self.id:
             return False
         try:
-            Permissions[permission]
+            return Permissions[permission] in self.permissions
         except KeyError:
             return False
-        return True
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/from_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,9 +40,10 @@
             add_book.Request(
                 user_id=self.__user_id,
                 isbn=str(data.get("isbn", "")),
                 title=str(data.get("title", "")),
                 year=int(data.get("year", "0")),
                 authors=data.get("authors", []),
                 genres=data.get("genres", []),
+                cover=str(data.get("cover", "")),
             )
         )
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.0a5/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 14% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
 add-book-requires-authentification = You must be authenticated before adding a book!
 add-book-title = Add a new book to the collection
 add-book-action = Add a book
 add-book-cancel = Cancel
 add-book-add = Add
 add-book-cover-help = Click to upload a cover
+add-book-cover-format-not-supported = The format of this cover is not supported!
 
 search-books-title = Search for a book
 search-books-action = Look up book
 search-books-clear = Clear
 search-books-search = Search
 search-books-no-result = No matching book!
 search-books-previous-page = Previous
@@ -95,13 +96,16 @@
 update-book-title = Edit information for `{ $isbn }`
 update-book-action = Edit
 update-book-failure = Book cannot be updated!
 update-book-success = Book has been updated!
 update-book-cancel = Cancel
 update-book-update = Save
 update-book-cover-help = Click to upload a new cover
+update-book-cover-format-not-supported = The format of this cover is not supported!
 
 book-already-exists = Book already in the collection!
-book-added = Book successfully added!
+# isbn (string) The ISBN of the book
+# url (string) The URL of the book
+book-added = Book <a href="{ $url }">{ $isbn }</a> successfully added!
 book-not-found = Book not found!
 book-cannot-be-added = The book cannot be added!
 books-cannot-be-found = The search cannot be performed!
```

#### html2text {}

```diff
@@ -33,20 +33,24 @@
 register-success = Your security device has been succesfully registered!
 webauthn-register-failure = Your security device could not be registered!?
 webauthn-login-title = Log in webauthn-login-description = Your browser should
 be asking you to tap your security deviceâ¦ webauthn-login-failure = You
 couldn't be logged in!? add-book-requires-authentification = You must be
 authenticated before adding a book! add-book-title = Add a new book to the
 collection add-book-action = Add a book add-book-cancel = Cancel add-book-add =
-Add add-book-cover-help = Click to upload a cover search-books-title = Search
-for a book search-books-action = Look up book search-books-clear = Clear
+Add add-book-cover-help = Click to upload a cover add-book-cover-format-not-
+supported = The format of this cover is not supported! search-books-title =
+Search for a book search-books-action = Look up book search-books-clear = Clear
 search-books-search = Search search-books-no-result = No matching book! search-
 books-previous-page = Previous search-books-next-page = Next # title (string)
 The title of the book display-book-title = Details for "{ $title }" update-
 book-requires-authentification = You must be authenticated before editing a
 book! # isbn (string) The ISBN of the book update-book-title = Edit information
 for `{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
 updated! update-book-success = Book has been updated! update-book-cancel =
 Cancel update-book-update = Save update-book-cover-help = Click to upload a new
-cover book-already-exists = Book already in the collection! book-added = Book
-successfully added! book-not-found = Book not found! book-cannot-be-added = The
-book cannot be added! books-cannot-be-found = The search cannot be performed!
+cover update-book-cover-format-not-supported = The format of this cover is not
+supported! book-already-exists = Book already in the collection! # isbn
+(string) The ISBN of the book # url (string) The URL of the book book-added =
+Book {_$isbn_} successfully added! book-not-found = Book not found! book-
+cannot-be-added = The book cannot be added! books-cannot-be-found = The search
+cannot be performed!
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.0a5/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
 add-book-requires-authentification = Vous devez être authentifié·e pour pouvoir ajouter un livre !
 add-book-title = Ajouter un nouveau livre à la collection
 add-book-action = Ajouter un livre
 add-book-cancel = Annuler
 add-book-add = Ajouter
 add-book-cover-help = Cliquez pour téléverser une couverture
+add-book-cover-format-not-supported = Le format de cette couverture n'est pas supporté !
 
 search-books-title = Chercher un livre dans la collection
 search-books-action = Chercher un livre
 search-books-clear = Réinitialiser
 search-books-search = Chercher
 search-books-no-result = Aucun livre ne correspond !
 search-books-previous-page = Précédent
@@ -95,13 +96,16 @@
 update-book-title = Éditer les informations de `{ $isbn }`
 update-book-action = Éditer
 update-book-failure = Le livre n'a pas pu être mis à jour !
 update-book-success = Le livre a bien été mis à jour !
 update-book-cancel = Annuler
 update-book-update = Enregistrer
 update-book-cover-help = Cliquez pour téléverser une nouvelle couverture
+update-book-cover-format-not-supported = Le format de cette couverture n'est pas supporté !
 
 book-already-exists = Ce livre est déjà dans la collection !
-book-added = Le livre a bien été ajouté.
+# isbn (string) The ISBN of the book
+# url (string) The URL of the book
+book-added = Le livre <a href="{ $url }">{ $isbn }</a> a bien été ajouté !
 book-not-found = Le livre n'a pas été trouvé !
 book-cannot-be-added = Le livre n'a pas pu être ajouté !
 books-cannot-be-found = La recherche n'a pas pu être effectuée !
```

#### html2text {}

```diff
@@ -38,23 +38,26 @@
 pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion webauthn-login-
 description = Votre navigateur devrait Ãªtre en train de vous demander de
 toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure = Vous n'avez
 pas pu Ãªtre connectÃ©Â·eÂ !? add-book-requires-authentification = Vous devez
 Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-title = Ajouter
 un nouveau livre Ã  la collection add-book-action = Ajouter un livre add-book-
 cancel = Annuler add-book-add = Ajouter add-book-cover-help = Cliquez pour
-tÃ©lÃ©verser une couverture search-books-title = Chercher un livre dans la
-collection search-books-action = Chercher un livre search-books-clear =
+tÃ©lÃ©verser une couverture add-book-cover-format-not-supported = Le format de
+cette couverture n'est pas supportÃ©Â ! search-books-title = Chercher un livre
+dans la collection search-books-action = Chercher un livre search-books-clear =
 RÃ©initialiser search-books-search = Chercher search-books-no-result = Aucun
 livre ne correspondÂ ! search-books-previous-page = PrÃ©cÃ©dent search-books-
 next-page = Suivant # title (string) The title of the book display-book-title =
 DÃ©tails pour Â«Â { $title }Â Â» update-book-requires-authentification = Vous
 devez Ãªtre authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string)
 The ISBN of the book update-book-title = Ãditer les informations de `{ $isbn
 }` update-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre
 mis Ã  jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ !
 update-book-cancel = Annuler update-book-update = Enregistrer update-book-
-cover-help = Cliquez pour tÃ©lÃ©verser une nouvelle couverture book-already-
-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! book-added = Le livre a bien
-Ã©tÃ© ajoutÃ©. book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-
-be-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La
-recherche n'a pas pu Ãªtre effectuÃ©eÂ !
+cover-help = Cliquez pour tÃ©lÃ©verser une nouvelle couverture update-book-
+cover-format-not-supported = Le format de cette couverture n'est pas
+supportÃ©Â ! book-already-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! #
+isbn (string) The ISBN of the book # url (string) The URL of the book book-
+added = Le livre {_$isbn_} a bien Ã©tÃ© ajoutÃ©Â ! book-not-found = Le livre
+n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-added = Le livre n'a pas pu Ãªtre
+ajoutÃ©Â ! books-cannot-be-found = La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,18 @@
     ) -> None:
         super().__init__("books/search", fragment=fragment, user=user)
         self.__data = data
         self.__context: dict[str, Any] = {"errors": {}}
 
         self.__set_page_urls()
 
+        if data:
+            # Handle the case when the search returns no book.
+            self.__context["books"] = []
+
     def __set_page_urls(self) -> None:
         self.__context["previous_page_url"] = self.__build_url(
             {**self.__data, "page": self.__previous_page_number()}
         )
         # FIXME How to know if there are more results?!
         self.__context["next_page_url"] = self.__build_url(
             {**self.__data, "page": self.__next_page_number()}
@@ -240,16 +244,23 @@
         }
 
     def book_already_exists(self, book: Book) -> None:
         self.__notify(self._("book-already-exists"), "info")
         self.redirect(url_for("books.display", isbn=str(book.isbn)))
 
     def book_added(self, book: Book) -> None:
-        self.__notify(self._("book-added"), "success")
-        self.redirect(url_for("books.search", isbn=str(book.isbn)))
+        self.__notify(
+            self._(
+                "book-added",
+                isbn=str(book.isbn),
+                url=url_for("books.display", isbn=str(book.isbn)),
+            ),
+            "success",
+        )
+        self.redirect(url_for("books.add"))
 
 
 class LookUpBook(JinjaPresenter, look_up_book.Presenter):
     def __init__(self, /, *, user: Optional[User] = None) -> None:
         super().__init__("books/add", fragment="form", user=user)
         self.__data: dict[str, Any] = {}
         self.__context: dict[str, Any] = {"errors": {}}
@@ -272,14 +283,15 @@
     def book(self, book: Book) -> None:
         self.__data = {
             "isbn": str(book.isbn),
             "title": str(book.title),
             "year": int(book.year),
             "authors": ", ".join([str(a) for a in book.authors]),
             "genres": ", ".join([str(g) for g in book.genres]),
+            "cover": str(book.cover),
         }
 
 
 class DisplayBook(JinjaPresenter, display_book.Presenter):
     def __init__(
         self,
         /,
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 
 block scripts
   script.
     function loadIntoImage(from, toImage, toInput) {
       if (from.files && from.files[0]) {
         const reader = new FileReader()
         reader.onload = e => {
-          toInput.value = e.target.result
-          toImage.src = e.target.result
+          const dataUrl = e.target.result
+          if (dataUrl.startsWith("data:image/")) {
+            toInput.value = dataUrl
+            toImage.src = dataUrl
+          }
+          else {
+            alert("#{_('update-book-cover-format-not-supported') | safe}");
+          }
         }
         reader.readAsDataURL(from.files[0])
       }
     }
 
 block content
   section.section
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 22% similar despite different names*

```diff
@@ -18,37 +18,38 @@
 
 block title
   title= _("hector") + " – " + _("display-book-title", title=book.title)
 
 block content
   section.section
     .container
-      .buttons.is-pulled-right
-        if user.can_update_book
-          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
-            span.icon: i.fas.fa-edit
-            span= _("update-book-action")
-        else
-          button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
-            span.icon: i.fas.fa-edit
-            span= _("update-book-action")
 
-      h1.title.is-3= book.title
+      h1.title.is-3
+        span= book.title
+        .buttons.is-pulled-right
+          if user.can_update_book
+            a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
+              span.icon: i.fas.fa-edit
+              span= _("update-book-action")
+          else
+            button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
+              span.icon: i.fas.fa-edit
+              span= _("update-book-action")
 
       .columns
         .column.is-one-quarter
           img#cover.cover.is-2by3(
             src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}"
             alt="Book cover"
           )
-        .column.content
+        .column
           dl
-            dt.has-text-weight-bold= _("book-isbn")
+            dt= _("book-isbn")
             dd= book.isbn
-            dt.has-text-weight-bold= _("book-title")
+            dt= _("book-title")
             dd= book.title
-            dt.has-text-weight-bold= _("book-year")
+            dt= _("book-year")
             dd= book.year
-            dt.has-text-weight-bold= _("book-authors")
+            dt= _("book-authors")
             dd= book.authors
-            dt.has-text-weight-bold= _("book-genres")
+            dt= _("book-genres")
             dd= book.genres or "-"
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 
 block title
   title= _("hector") + " – " + _("search-books-title")
 
 block content
   section.section
     .container
-      .buttons.is-pulled-right
-        if user.can_add_book
-          a.button.is-link(href="#{url_for('books.add')}")
-            span.icon: i.fas.fa-plus
-            span= _("add-book-action")
-        else
-          button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
-            span.icon: i.fas.fa-plus
-            span= _("add-book-action")
-
-      h1.title.is-3= _("search-books-title")
+      h1.title.is-3
+        span= _("search-books-title")
+        .buttons.is-pulled-right
+          if user.can_add_book
+            a.button.is-link(href="#{url_for('books.add')}")
+              span.icon: i.fas.fa-plus
+              span= _("add-book-action")
+          else
+            button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
+              span.icon: i.fas.fa-plus
+              span= _("add-book-action")
 
       #form
         block form
           include mixins/form
           form(
             method="GET"
             action="#{url_for('books.search')}"
@@ -54,15 +54,15 @@
             +text_field("genre", data.genre, errors.genre, description=_("book-genre-description"), icon="crown", placeholder=_('book-genre'))
 
             .field
               p.control
                 a.button.is-light(href="#{url_for('books.search')}")
                   span.icon: i.fas.fa-trash
                   span= _("search-books-clear")
-                button.button.is-primary
+                button.button.is-primary(_="on click add .is-loading")
                   span.icon: i.fas.fa-search
                   span= _("search-books-search")
 
           if books is defined
             if books|length > 0
               #books.books
                 block books
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 
 block scripts
   script.
     function loadIntoImage(from, toImage, toInput) {
       if (from.files && from.files[0]) {
         const reader = new FileReader()
         reader.onload = e => {
-          toInput.value = e.target.result
-          toImage.src = e.target.result
+          const dataUrl = e.target.result
+          if (dataUrl.startsWith("data:image/")) {
+            toInput.value = dataUrl
+            toImage.src = dataUrl
+          }
+          else {
+            alert("#{_('update-book-cover-format-not-supported') | safe}");
+          }
         }
         reader.readAsDataURL(from.files[0])
       }
     }
 
 block content
   section.section
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 mixin flash(messages)
   - var alert_classes = {"success": "is-success", "error": "is-danger", "info": "is-info", "warning": "is-warning"}
   if messages
     .container.mt-5
       each category, message in messages
         p.notification.is-light(class=alert_classes[category])
           button.delete(_="on click remove the closest .notification")
-          | #{message}
+          | #{message|safe}
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,12 +39,14 @@
             "isbn": str(book.isbn),
             "title": str(book.title),
             "year": int(book.year),
             "authors": [str(b) for b in book.authors],
         }
         if book.genres:
             data["genres"] = [str(g) for g in book.genres]
+        if book.cover:
+            data["cover"] = str(book.cover)
 
         self.__printer(json.dumps(data))
 
     def exit_code(self) -> int:
         return self.__exit_code.value
```

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/bl_hector/interfaces/utils.py` & `bl_hector-0.1.0a5/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a4/pyproject.toml` & `bl_hector-0.1.0a5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.4"
+version = "0.1.0-alpha.5"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
@@ -26,14 +26,15 @@
 isbnlib = "^3.10.14"
 jinja2-fragments = "^0.3.0"
 SQLAlchemy = "^2.0.15"
 typer = "^0.9.0"
 bl3d = "^0.3.0"
 "fluent.runtime" = "^0.4.0"
 webauthn = {version = "^1.8.1", optional = true}
+requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 robber = "^1.1.5"
 invoke = "^2.1.1"
 flake8 = "^6.0.0"
 black = "^23.3.0"
@@ -41,14 +42,15 @@
 mypy = "^1.2.0"
 termcolor = "^2.3.0"
 types-setuptools = "^67.7.0"
 mamba = "^0.11.2"
 beautifulsoup4 = "^4.12.2"
 types-beautifulsoup4 = "^4.12.0"
 behave = "^1.2.6"
+types-requests = "^2.31.0"
 
 [tool.poetry.extras]
 webauthn = ["webauthn"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `bl_hector-0.1.0a4/setup.py` & `bl_hector-0.1.0a5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
  'bl_hector.infrastructure',
  'bl_hector.infrastructure.flask',
  'bl_hector.infrastructure.flask.aliases',
  'bl_hector.infrastructure.flask.auth',
  'bl_hector.infrastructure.flask.books',
  'bl_hector.infrastructure.flask.webauthn',
  'bl_hector.infrastructure.isbnlib',
+ 'bl_hector.infrastructure.requests',
  'bl_hector.infrastructure.sqlalchemy',
  'bl_hector.infrastructure.typer',
  'bl_hector.interfaces',
  'bl_hector.interfaces.l10n',
  'bl_hector.interfaces.to_http',
  'bl_hector.interfaces.to_http.as_html',
  'bl_hector.interfaces.to_http.as_json',
@@ -45,25 +46,26 @@
  'SQLAlchemy>=2.0.15,<3.0.0',
  'bl-seth>=0.1.2,<0.2.0',
  'bl3d>=0.3.0,<0.4.0',
  'fluent.runtime>=0.4.0,<0.5.0',
  'isbnlib>=3.10.14,<4.0.0',
  'jinja2-fragments>=0.3.0,<0.4.0',
  'pypugjs>=5.9.12,<6.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'typer>=0.9.0,<0.10.0']
 
 extras_require = \
 {'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a4',
+    'version': '0.1.0a5',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bl_hector-0.1.0a4/PKG-INFO` & `bl_hector-0.1.0a5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A collection manager.
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: bl-seth (>=0.1.2,<0.2.0)
 Requires-Dist: bl3d (>=0.3.0,<0.4.0)
 Requires-Dist: fluent.runtime (>=0.4.0,<0.5.0)
 Requires-Dist: isbnlib (>=3.10.14,<4.0.0)
 Requires-Dist: jinja2-fragments (>=0.3.0,<0.4.0)
 Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: webauthn (>=1.8.1,<2.0.0); extra == "webauthn"
 Description-Content-Type: text/markdown
 
 # Hector — a collection manager
 
 ## Install
```

