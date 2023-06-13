# Comparing `tmp/bl_hector-0.1.0a6.tar.gz` & `tmp/bl_hector-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.0a6.tar", max compression
+gzip compressed data, was "bl_hector-0.1.0a7.tar", max compression
```

## Comparing `bl_hector-0.1.0a6.tar` & `bl_hector-0.1.0a7.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     1507 2023-06-13 08:52:57.770248 bl_hector-0.1.0a6/README.md
--rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3639 2023-06-11 08:10:05.209290 bl_hector-0.1.0a6/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a6/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     3480 2023-06-13 07:05:26.339251 bl_hector-0.1.0a6/bl_hector/application/use_cases/import_books.py
--rw-r--r--   0        0        0     1979 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3755 2023-06-11 08:06:35.483796 bl_hector-0.1.0a6/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3612 2023-06-11 08:06:35.483796 bl_hector-0.1.0a6/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a6/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a6/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1449 2023-06-09 06:16:19.350310 bl_hector-0.1.0a6/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/exceptions.py
--rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1083 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1804 2023-06-11 08:06:35.483796 bl_hector-0.1.0a6/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3309 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1179 2023-06-13 06:14:28.110892 bl_hector-0.1.0a6/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3706 2023-06-13 09:04:29.650237 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4016 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3382 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
--rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
--rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2112 2023-06-13 09:33:38.004683 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-13 08:24:56.879217 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1657 2023-06-13 07:05:26.339251 bl_hector-0.1.0a6/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-13 09:42:06.790266 bl_hector-0.1.0a6/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     7982 2023-06-11 17:37:17.410696 bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a6/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2899 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-13 07:05:37.235116 bl_hector-0.1.0a6/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1393 2023-06-13 05:56:18.671790 bl_hector-0.1.0a6/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a6/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a6/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a6/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a6/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4466 2023-06-13 09:26:06.278457 bl_hector-0.1.0a6/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5058 2023-06-13 09:25:56.630581 bl_hector-0.1.0a6/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14797 2023-06-13 07:13:35.057254 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-09 13:26:25.425148 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4296 2023-06-13 07:51:28.000402 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     1966 2023-06-13 08:41:29.126612 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2048 2023-06-11 09:09:06.457902 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5607 2023-06-13 08:41:29.126612 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3589 2023-06-13 08:34:41.343554 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2026 2023-06-09 13:26:33.641053 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4134 2023-06-11 08:39:27.744213 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-09 13:26:48.248884 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1400 2023-06-13 09:27:19.501527 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     4445 2023-06-11 08:06:35.487796 bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a6/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1516 2023-06-13 09:42:40.769842 bl_hector-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0     4246 2023-06-13 09:43:16.433995 bl_hector-0.1.0a6/setup.py
--rw-r--r--   0        0        0     2560 2023-06-13 09:43:16.434902 bl_hector-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 09:45:12.827540 bl_hector-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     1507 2023-06-13 08:52:57.770248 bl_hector-0.1.0a7/README.md
+-rw-r--r--   0        0        0      807 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3807 2023-06-13 17:10:53.285803 bl_hector-0.1.0a7/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     1981 2023-06-09 06:16:19.350310 bl_hector-0.1.0a7/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     3480 2023-06-13 07:05:26.339251 bl_hector-0.1.0a7/bl_hector/application/use_cases/import_books.py
+-rw-r--r--   0        0        0     1979 2023-06-13 07:05:37.235116 bl_hector-0.1.0a7/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3755 2023-06-11 08:06:35.483796 bl_hector-0.1.0a7/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3805 2023-06-13 17:23:36.928433 bl_hector-0.1.0a7/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-09 13:18:08.922894 bl_hector-0.1.0a7/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-09 13:18:04.750942 bl_hector-0.1.0a7/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1567 2023-06-13 17:10:09.238345 bl_hector-0.1.0a7/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0      996 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/collection_management/exceptions.py
+-rw-r--r--   0        0        0     1509 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-13 16:46:31.847726 bl_hector-0.1.0a7/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1804 2023-06-11 08:06:35.483796 bl_hector-0.1.0a7/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3749 2023-06-13 16:39:49.484615 bl_hector-0.1.0a7/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-13 16:46:31.579729 bl_hector-0.1.0a7/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3706 2023-06-13 11:18:20.228210 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-07 16:14:27.658555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1693 2023-06-09 08:04:31.521092 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4116 2023-06-13 17:14:54.950836 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-13 16:45:43.904308 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-13 07:15:23.075945 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0    35880 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png
+-rw-r--r--   0        0        0      928 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0     3602 2023-06-07 16:14:27.662555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png
+-rw-r--r--   0        0        0    42819 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-07 16:14:27.670555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2112 2023-06-13 09:33:38.004683 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-09 13:18:08.926894 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4544 2023-06-13 08:24:56.879217 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-13 05:56:18.671790 bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-13 17:15:23.130490 bl_hector-0.1.0a7/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1568 2023-06-13 07:05:37.235116 bl_hector-0.1.0a7/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-13 11:18:20.228210 bl_hector-0.1.0a7/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8340 2023-06-13 17:24:02.232123 bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-07 16:14:27.674555 bl_hector-0.1.0a7/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2957 2023-06-13 16:46:20.467864 bl_hector-0.1.0a7/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-13 07:05:37.235116 bl_hector-0.1.0a7/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     1393 2023-06-13 05:56:18.671790 bl_hector-0.1.0a7/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-10 16:50:21.825376 bl_hector-0.1.0a7/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3371 2023-06-11 08:23:57.603430 bl_hector-0.1.0a7/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-13 07:05:37.239116 bl_hector-0.1.0a7/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1435 2023-06-07 17:00:49.589157 bl_hector-0.1.0a7/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     4568 2023-06-13 17:14:28.243164 bl_hector-0.1.0a7/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5167 2023-06-13 17:14:41.846997 bl_hector-0.1.0a7/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1407 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    15005 2023-06-13 17:13:45.447689 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-09 13:26:25.425148 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4296 2023-06-13 14:17:08.848203 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2100 2023-06-13 17:14:13.355347 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     2048 2023-06-11 09:09:06.457902 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
+-rw-r--r--   0        0        0     5607 2023-06-13 14:17:08.848203 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3589 2023-06-13 08:34:41.343554 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-09 13:18:08.934894 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2026 2023-06-09 13:26:33.641053 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-13 07:11:41.542636 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4134 2023-06-11 08:39:27.744213 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-13 14:17:08.848203 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1400 2023-06-13 09:27:19.501527 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-13 07:05:37.239116 bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     4445 2023-06-11 08:06:35.487796 bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-07 16:14:27.682555 bl_hector-0.1.0a7/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1516 2023-06-13 17:25:15.715222 bl_hector-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0     4246 2023-06-13 17:25:55.523007 bl_hector-0.1.0a7/setup.py
+-rw-r--r--   0        0        0     2560 2023-06-13 17:25:55.524440 bl_hector-0.1.0a7/PKG-INFO
```

### Comparing `bl_hector-0.1.0a6/LICENSE` & `bl_hector-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/README.md` & `bl_hector-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/__init__.py` & `bl_hector-0.1.0a7/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/__init__.py` & `bl_hector-0.1.0a7/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/add_book.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
 from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.services import Calendar
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Genre,
     Isbn,
     Title,
     Year,
@@ -75,24 +76,28 @@
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
     books: Books
+    calendar: Calendar
     permissions: Permissions
 
     def execute(self, request: Request) -> None:
         if not self.__is_authorized(request.user_id):
             return self.presenter.not_authorized()
 
         if errors := self.__validate_request(request):
             return self.presenter.bad_request(errors)
 
+        today = self.calendar.today()
         book = Book.instanciate(
+            today,
+            today,
             Isbn.instanciate(request.isbn),
             Title.instanciate(request.title),
             Year.instanciate(request.year),
             [Author.instanciate(a) for a in request.authors if a],
             [Genre.instanciate(g) for g in request.genres if g],
             Cover.instanciate(request.cover) if request.cover else None,
         )
```

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/import_books.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/import_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.1.0a7/bl_hector/application/use_cases/update_book.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
 from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
 from bl_hector.domain.collection_management.repositories import Books
+from bl_hector.domain.collection_management.services import Calendar
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Genre,
     Isbn,
     Title,
     Year,
@@ -74,36 +75,40 @@
         ...
 
 
 @dataclass(frozen=True)
 class Interactor:
     presenter: Presenter
     books: Books
+    calendar: Calendar
     permissions: Permissions
 
     def execute(self, request: Request) -> None:
         if not self.__is_authorized(request.user_id):
             return self.presenter.not_authorized()
 
         if errors := self.__validate_request(request):
             return self.presenter.bad_request(errors)
 
+        isbn = Isbn.instanciate(request.isbn)
+        if not (original_book := self.books.by_isbn(isbn=isbn)):
+            return self.presenter.book_not_found(isbn)
+
         # There's no business logic to apply when updating a book.
         book = Book.instanciate(
-            Isbn.instanciate(request.isbn),
+            original_book.added_on,
+            self.calendar.today(),
+            isbn,
             Title.instanciate(request.title),
             Year.instanciate(request.year),
             [Author.instanciate(a) for a in request.authors if a],
             [Genre.instanciate(g) for g in request.genres if g],
             Cover.instanciate(request.cover) if request.cover else None,
         )
 
-        if not self.books.search(isbn=book.isbn):
-            return self.presenter.book_not_found(book.isbn)
-
         self.books.update(book)
         self.presenter.book_updated(book)
 
     def __is_authorized(self, user_id: str) -> bool:
         return self.permissions.is_authorized_to(UserId(user_id), P.UPDATE_BOOK)
 
     def __validate_request(self, request: Request) -> Errors:
```

### Comparing `bl_hector-0.1.0a6/bl_hector/configuration/__init__.py` & `bl_hector-0.1.0a7/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/configuration/cli.py` & `bl_hector-0.1.0a7/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/configuration/wsgi.py` & `bl_hector-0.1.0a7/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/__init__.py` & `bl_hector-0.1.0a7/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/administration/__init__.py` & `bl_hector-0.1.0a7/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/administration/entities.py` & `bl_hector-0.1.0a7/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.1.0a7/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/administration/repositories.py` & `bl_hector-0.1.0a7/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/administration/services.py` & `bl_hector-0.1.0a7/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.1.0a7/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/entities.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,32 +14,36 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from typing import Optional
 
 from .exceptions import IncorrectValue
-from .value_objects import Author, Cover, Genre, Isbn, Title, Year
+from .value_objects import Author, Cover, Date, Genre, Isbn, Title, Year
 
 
 @dataclass
 class Book:
+    added_on: Date
+    updated_on: Date
     isbn: Isbn
     title: Title
     year: Year
     authors: list[Author]
     genres: list[Genre]
     cover: Optional[Cover] = None
 
     @classmethod
     def instanciate(
         cls,
+        added_on: Date,
+        updated_on: Date,
         isbn: Isbn,
         title: Title,
         year: Year,
         authors: list[Author],
         genres: list[Genre],
         cover: Optional[Cover] = None,
     ) -> "Book":
         if not authors:
             raise IncorrectValue("authors", "A book must have at least one author!")
-        return Book(isbn, title, year, authors, genres, cover)
+        return Book(added_on, updated_on, isbn, title, year, authors, genres, cover)
```

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/exceptions.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/services.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,26 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from .entities import Book
-from .value_objects import Cover, Isbn
+from .value_objects import Cover, Date, Isbn
 
 
 class BookInfoProvider(ABC):
     @abstractmethod
     def look_up(self, isbn: Isbn) -> Optional[Book]:
         ...
 
 
 class CoverProvider(ABC):
     @abstractmethod
     def by_isbn(self, isbn: Isbn) -> Optional[Cover]:
         ...
+
+
+class Calendar(ABC):
+    @abstractmethod
+    def today(self) -> Date:
+        ...
```

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.1.0a7/bl_hector/domain/collection_management/value_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+import datetime
 from typing import Type
 
 import bl3d
 from isbnlib import is_isbn13, mask
 
 from bl_hector.domain.collection_management.exceptions import IncorrectValue
 
@@ -40,14 +41,25 @@
             return super().instanciate(value)
         except bl3d.InvalidValue as exc:
             # TODO use the `bl3d.NumberXxxYyy` exceptions when available.
             #      let them pass or recast them!?
             raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
 
 
+class Date(bl3d.Date):
+    @classmethod
+    def instanciate(cls: Type[bl3d.TypeDate], value: datetime.date) -> bl3d.TypeDate:
+        try:
+            return super().instanciate(value)
+        except bl3d.InvalidValue as exc:
+            # TODO use the `bl3d.DateXxxYyy` exceptions when available.
+            #      let them pass or recast them!?
+            raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
+
+
 class Isbn(String):
     """
     The International Standard Book Number (ISBN) of a book,
     for instance 978-0-7653-9277-0.
     """
 
     MIN = 13
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,20 +10,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+import datetime
+
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
+from bl_hector.domain.collection_management.services import Calendar
+from bl_hector.domain.collection_management.value_objects import Date
 
 ONLY_USER = "admin"
 
 
 class DummyPermissions(Permissions):
     def for_user(self, user_id: UserId) -> list[P]:
         return [p for p in P]
 
     def is_authorized_to(self, user_id: UserId, permission: P) -> bool:
         return bool(str(user_id))
+
+
+class SystemCalendar(Calendar):
+    def today(self) -> Date:
+        return Date.instanciate(datetime.date.today())
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,18 @@
 
 
 @blueprint.post("__new__")
 @presenter_to_response
 def add_POST() -> Any:
     presenter = presenters.AddBook(request.form, notify=notify, user=services.get_user())
     interactor = add_book.Interactor(
-        presenter, services.get_books(), services.get_permissions()
+        presenter,
+        services.get_books(),
+        services.get_calendar(),
+        services.get_permissions(),
     )
     controller = controllers.AddBook(request.form, str(services.get_user().id))
     controller.call(interactor)
     return presenter
 
 
 @blueprint.post("__info__")
@@ -106,15 +109,18 @@
 @blueprint.post("<string:isbn>/__edit__")
 @presenter_to_response
 def update_POST(isbn: str) -> Any:
     presenter = presenters.UpdateBook(
         isbn, request.form, notify=notify, user=services.get_user()
     )
     interactor = update_book.Interactor(
-        presenter, services.get_books(), services.get_permissions()
+        presenter,
+        services.get_books(),
+        services.get_calendar(),
+        services.get_permissions(),
     )
     controller = controllers.UpdateBook(isbn, request.form, str(services.get_user().id))
     controller.call(interactor)
     return presenter
 
 
 @blueprint.post("@isbn")
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from urllib.parse import urlparse
 
 from flask import g, request, session
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Connection
 
 from bl_hector.domain.administration.entities import RelyingParty
-from bl_hector.infrastructure import DummyPermissions
+from bl_hector.infrastructure import DummyPermissions, SystemCalendar
 from bl_hector.infrastructure.isbnlib import BookInfoProvider
 from bl_hector.infrastructure.requests import CoverProvider
 from bl_hector.infrastructure.settings import WsgiSettings
 from bl_hector.infrastructure.sqlalchemy.repositories import (
     Books,
     Challenges,
     Credentials,
@@ -83,14 +83,18 @@
     return Credentials(get_connection())
 
 
 def get_challenges() -> Challenges:
     return Challenges(get_connection())
 
 
+def get_calendar() -> SystemCalendar:
+    return SystemCalendar()
+
+
 def get_permissions() -> DummyPermissions:
     return DummyPermissions()
 
 
 def get_book_info_provider() -> BookInfoProvider:
     return BookInfoProvider()
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/1280x960.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/img/placeholders/96x96.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,39 +10,44 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+import datetime
 import logging
 from typing import Optional
 
 import isbnlib
 
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.services import (
     BookInfoProvider as BookInfoProviderABC,
 )
 from bl_hector.domain.collection_management.value_objects import (
     Author,
+    Date,
     Isbn,
     Title,
     Year,
 )
 
 
 class BookInfoProvider(BookInfoProviderABC):
     def look_up(self, isbn: Isbn) -> Optional[Book]:
         try:
             meta = isbnlib.meta(str(isbn))
             if not meta:
                 return None
 
+            today = Date.instanciate(datetime.date.today())
             return Book.instanciate(
+                today,
+                today,
                 isbn,
                 Title.instanciate(meta.get("Title", "")),
                 Year.instanciate(int(meta.get("Year", ""))),
                 [Author.instanciate(a) for a in meta.get("Authors", "")],
                 [],
             )
         except Exception as exc:
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/settings.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import datetime
 from typing import Any, Optional
 
+from sqlalchemy import Column
+from sqlalchemy import Date as DateType
 from sqlalchemy import (
-    Column,
     DateTime,
     LargeBinary,
     MetaData,
     SmallInteger,
     String,
     Table,
     delete,
@@ -43,14 +44,15 @@
 )
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.exceptions import UnknownBook
 from bl_hector.domain.collection_management.repositories import Books as IBooks
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
+    Date,
     Genre,
     Isbn,
     Title,
     Year,
 )
 
 META_DATA = MetaData()
@@ -62,14 +64,16 @@
     META_DATA,
     Column("isbn", String(Isbn.MAX), primary_key=True),
     Column("title", String(Title.MAX)),
     Column("year", SmallInteger()),
     Column("authors", String()),
     Column("genres", String()),
     Column("cover", String()),
+    Column("added_on", DateType()),
+    Column("updated_on", DateType()),
 )
 
 
 class Books(IBooks):
     def __init__(self, connection: Connection) -> None:
         self.__connection = connection
 
@@ -110,24 +114,28 @@
             stmt = stmt.offset((page_number - 1) * size)
             stmt = stmt.limit(size)
 
         return [self.__row_to_book(row) for row in self.__connection.execute(stmt)]
 
     def __row_to_book(self, row: Any) -> Book:
         return Book(
+            Date(row.added_on),
+            Date(row.updated_on),
             Isbn(row.isbn),
             Title(row.title),
             Year(row.year),
             [Author(r.strip()) for r in row.authors.split(",") if r],
             [Genre(r.strip()) for r in row.genres.split(",") if r],
             Cover(row.cover) if row.cover else None,
         )
 
     def add(self, book: Book) -> None:
         stmt = insert(books).values(
+            added_on=book.added_on.to_date(),
+            updated_on=book.updated_on.to_date(),
             isbn=str(book.isbn),
             title=str(book.title),
             year=int(book.year),
             authors=", ".join([str(a) for a in book.authors]),
             genres=", ".join([str(g) for g in book.genres]),
             cover=str(book.cover) if book.cover else None,
         )
@@ -135,14 +143,15 @@
 
     def update(self, book: Book) -> None:
         if not self.by_isbn(book.isbn):
             raise UnknownBook(str(book.isbn))
         stmt = (
             update(books)
             .values(
+                updated_on=book.updated_on.to_date(),
                 title=str(book.title),
                 year=int(book.year),
                 authors=", ".join([str(a) for a in book.authors]),
                 genres=", ".join([str(g) for g in book.genres]),
                 cover=str(book.cover) if book.cover else None,
             )
             .where(books.c.isbn == str(book.isbn))
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/typer/books.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import sys
 
 import typer
 from typing_extensions import Annotated
 
 from bl_hector.application.use_cases import add_book, import_books, look_up_book
-from bl_hector.infrastructure import ONLY_USER, DummyPermissions
+from bl_hector.infrastructure import ONLY_USER, DummyPermissions, SystemCalendar
 from bl_hector.infrastructure.typer import services
 from bl_hector.interfaces import from_json as controllers
 from bl_hector.interfaces.to_terminal import LookUpBookInterface, as_json, as_text
 
 cmd = typer.Typer()
 
 
@@ -48,20 +48,21 @@
     interactor.execute(look_up_book.Request(isbn))
     raise typer.Exit(presenter.exit_code())
 
 
 @cmd.command()
 def add(ctx: typer.Context) -> None:
     """Add a book to the collection."""
+    calendar = SystemCalendar()
     permissions = DummyPermissions()
     with services.get_books(ctx.obj) as books:
         presenter = as_text.AddBook(
             lambda m: typer.echo(m), translator=services.get_translator()
         )
-        interactor = add_book.Interactor(presenter, books, permissions)
+        interactor = add_book.Interactor(presenter, books, calendar, permissions)
         controller = controllers.AddBook(sys.stdin.readline(), ONLY_USER)
         controller.call(interactor)
         raise typer.Exit(presenter.exit_code())
 
 
 @cmd.command("import")
 def import_(ctx: typer.Context, path: str) -> None:
```

### Comparing `bl_hector-0.1.0a6/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.1.0a7/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/__init__.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/exceptions.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/from_dict.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/from_json.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.1.0a7/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,21 @@
 # value (string) The value of the information to display
 info-line = { $name }: { $value }
 
 access-forbidden = Access forbidden!
 access-not-authorized = Access unauthorised!
 an-error-occurred = An error occurred!
 
+# date (Date) A date to format
+date = { $date }
+
 book = book
 books = books
+book-added-on = added on
+book-updated-on = update on
 book-isbn = ISBN
 book-isbn-description = The ISBN assigned to the book, for instance 978-0-7653-9277-0.
 book-title = title
 book-title-description = The title of the book.
 book-year = year
 book-year-description = The year the book was published in.
 book-author = author
```

#### html2text {}

```diff
@@ -12,47 +12,48 @@
 (string) The years the copyright applies to. # holders (string) The names of
 the copyright holders. copyright = Version { $version } Â© { $years }
 { $holders }. # name (string) The name of the license. # url (string) The URL
 of the license file. license = Code is licensed under {_$name_}. # name
 (string) The name of the information to display # value (string) The value of
 the information to display info-line = { $name }: { $value } access-forbidden =
 Access forbidden! access-not-authorized = Access unauthorised! an-error-
-occurred = An error occurred! book = book books = books book-isbn = ISBN book-
-isbn-description = The ISBN assigned to the book, for instance 978-0-7653-9277-
-0. book-title = title book-title-description = The title of the book. book-year
-= year book-year-description = The year the book was published in. book-author
-= author book-author-description = One of the authors of the book. book-authors
-= authors book-authors-description = The list of authors of the book, comma
-separated. book-genre = genre book-genre-description = One of the genres the
-book belongs to. book-genres = genres book-genres-description = The list of
-genres the book belongs to, comma separated. unknown-error = An unknown error
-has occurred! mandatory-value = This value is mandatory! incorrect-value =
-Incorrect value! not-an-isbn = This is not an ISBN! auth-login-title = Log in #
-method (string) The sign in method auth-login-method = Sign in using { $method
-} webauthn-register-title = Device registration webauthn-register-description =
-Your browser should be asking you to tap your security deviceâ¦ webauthn-
-register-success = Your security device has been succesfully registered!
-webauthn-register-failure = Your security device could not be registered!?
-webauthn-login-title = Log in webauthn-login-description = Your browser should
-be asking you to tap your security deviceâ¦ webauthn-login-failure = You
-couldn't be logged in!? totp-login-title = Log in totp-login-description =
-Please enter your one-time password. totp-login-password = Password totp-login-
-action = Log in add-book-requires-authentification = You must be authenticated
-before adding a book! add-book-title = Add a new book to the collection add-
-book-action = Add a book add-book-cancel = Cancel add-book-add = Add add-book-
-cover-help = Click to upload a cover add-book-cover-format-not-supported = The
-format of this cover is not supported! search-books-title = Search for a book
-search-books-action = Look up book search-books-clear = Clear search-books-
-search = Search search-books-no-result = No matching book! search-books-
-previous-page = Previous search-books-next-page = Next # title (string) The
-title of the book display-book-title = Details for "{ $title }" update-book-
-requires-authentification = You must be authenticated before editing a book! #
-isbn (string) The ISBN of the book update-book-title = Edit information for `
-{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
-updated! update-book-success = Book has been updated! update-book-cancel =
-Cancel update-book-update = Save update-book-cover-help = Click to upload a new
-cover update-book-cover-format-not-supported = The format of this cover is not
-supported! book-already-exists = Book already in the collection! # isbn
-(string) The ISBN of the book # url (string) The URL of the book book-added =
-Book {_$isbn_} successfully added! book-not-found = Book not found! book-
-cannot-be-added = The book cannot be added! books-cannot-be-found = The search
-cannot be performed!
+occurred = An error occurred! # date (Date) A date to format date = { $date }
+book = book books = books book-added-on = added on book-updated-on = update on
+book-isbn = ISBN book-isbn-description = The ISBN assigned to the book, for
+instance 978-0-7653-9277-0. book-title = title book-title-description = The
+title of the book. book-year = year book-year-description = The year the book
+was published in. book-author = author book-author-description = One of the
+authors of the book. book-authors = authors book-authors-description = The list
+of authors of the book, comma separated. book-genre = genre book-genre-
+description = One of the genres the book belongs to. book-genres = genres book-
+genres-description = The list of genres the book belongs to, comma separated.
+unknown-error = An unknown error has occurred! mandatory-value = This value is
+mandatory! incorrect-value = Incorrect value! not-an-isbn = This is not an
+ISBN! auth-login-title = Log in # method (string) The sign in method auth-
+login-method = Sign in using { $method } webauthn-register-title = Device
+registration webauthn-register-description = Your browser should be asking you
+to tap your security deviceâ¦ webauthn-register-success = Your security device
+has been succesfully registered! webauthn-register-failure = Your security
+device could not be registered!? webauthn-login-title = Log in webauthn-login-
+description = Your browser should be asking you to tap your security deviceâ¦
+webauthn-login-failure = You couldn't be logged in!? totp-login-title = Log in
+totp-login-description = Please enter your one-time password. totp-login-
+password = Password totp-login-action = Log in add-book-requires-
+authentification = You must be authenticated before adding a book! add-book-
+title = Add a new book to the collection add-book-action = Add a book add-book-
+cancel = Cancel add-book-add = Add add-book-cover-help = Click to upload a
+cover add-book-cover-format-not-supported = The format of this cover is not
+supported! search-books-title = Search for a book search-books-action = Look up
+book search-books-clear = Clear search-books-search = Search search-books-no-
+result = No matching book! search-books-previous-page = Previous search-books-
+next-page = Next # title (string) The title of the book display-book-title =
+Details for "{ $title }" update-book-requires-authentification = You must be
+authenticated before editing a book! # isbn (string) The ISBN of the book
+update-book-title = Edit information for `{ $isbn }` update-book-action = Edit
+update-book-failure = Book cannot be updated! update-book-success = Book has
+been updated! update-book-cancel = Cancel update-book-update = Save update-
+book-cover-help = Click to upload a new cover update-book-cover-format-not-
+supported = The format of this cover is not supported! book-already-exists =
+Book already in the collection! # isbn (string) The ISBN of the book # url
+(string) The URL of the book book-added = Book {_$isbn_} successfully added!
+book-not-found = Book not found! book-cannot-be-added = The book cannot be
+added! books-cannot-be-found = The search cannot be performed!
```

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.1.0a7/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,21 @@
 # value (string) The value of the information to display
 info-line = { $name } : { $value }
 
 access-forbidden = Accès interdit !
 access-not-authorized = Accès non authorisé !
 an-error-occurred = Une erreur s'est produite !
 
+# date (Date) A date to format
+date = { $date }
+
 book = livre
 books = livres
+book-added-on = ajouté le
+book-updated-on = mis à jour le
 book-isbn = ISBN
 book-isbn-description = Le numéro ISBN assigné au livre, par exemple 978-0-7653-9277-0.
 book-title = titre
 book-title-description = Le titre du livre.
 book-year = année
 book-year-description = L'année de publication du livre.
 book-author = aut·rice·eur
```

#### html2text {}

```diff
@@ -12,55 +12,56 @@
 software. # years (string) The years the copyright applies to. # holders
 (string) The names of the copyright holders. copyright = Version { $version }
 Â© { $years } { $holders }. # name (string) The name of the license. # url
 (string) The URL of the license file. license = Le code est sous licence
 {_$name_}. # name (string) The name of the information to display # value
 (string) The value of the information to display info-line = { $name }Â :
 { $value } access-forbidden = AccÃ¨s interditÂ ! access-not-authorized = AccÃ¨s
-non authorisÃ©Â ! an-error-occurred = Une erreur s'est produiteÂ ! book = livre
-books = livres book-isbn = ISBN book-isbn-description = Le numÃ©ro ISBN
-assignÃ© au livre, par exemple 978-0-7653-9277-0. book-title = titre book-
-title-description = Le titre du livre. book-year = annÃ©e book-year-description
-= L'annÃ©e de publication du livre. book-author = autÂ·riceÂ·eur book-author-
-description = UnÂ·e des autÂ·riceÂ·eurÂ·s du livre. book-authors =
-autÂ·riceÂ·eurÂ·s book-authors-description = La liste des autÂ·riceÂ·eurÂ·s du
-livre, sÃ©parÃ©Â·eÂ·s par des virgules. book-genre = genre book-genre-
-description = Un des genres auxquels le livre se rattache. book-genres = genres
-book-genres-description = La liste des genres auxquels le livre se rattache,
-sÃ©parÃ©s par des virgules. unknown-error = Une erreur inconnue s'est
-produiteÂ ! mandatory-value = Cette valeur est obligatoireÂ ! incorrect-value =
-Cette valeur est incorrecteÂ ! not-an-isbn = Ceci n'est pas un ISBNÂ ! auth-
-login-title = Connexion # method (string) The sign in method auth-login-method
-= Sign in using { $method } webauthn-register-title = Association du dispositif
-de sÃ©curitÃ© webauthn-register-description = Votre navigateur devrait Ãªtre en
-train de vous demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-
-register-success = Votre dispositif de sÃ©curitÃ© a Ã©tÃ© correctement
-associÃ©Â ! webauthn-register-failure = Votre dispositif de sÃ©curitÃ© n'a pas
-pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion webauthn-login-
-description = Votre navigateur devrait Ãªtre en train de vous demander de
-toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure = Vous n'avez
-pas pu Ãªtre connectÃ©Â·eÂ !? totp-login-title = Connexion totp-login-
-description = Merci de saisir votre mot de passe Ã  usage unique. totp-login-
-password = Mot de passe totp-login-action = Se connecter add-book-requires-
-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un
-livreÂ ! add-book-title = Ajouter un nouveau livre Ã  la collection add-book-
-action = Ajouter un livre add-book-cancel = Annuler add-book-add = Ajouter add-
-book-cover-help = Cliquez pour tÃ©lÃ©verser une couverture add-book-cover-
-format-not-supported = Le format de cette couverture n'est pas supportÃ©Â !
-search-books-title = Chercher un livre dans la collection search-books-action =
-Chercher un livre search-books-clear = RÃ©initialiser search-books-search =
-Chercher search-books-no-result = Aucun livre ne correspondÂ ! search-books-
-previous-page = PrÃ©cÃ©dent search-books-next-page = Suivant # title (string)
-The title of the book display-book-title = DÃ©tails pour Â«Â { $title }Â Â»
-update-book-requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour
-pouvoir Ã©diter un livreÂ ! # isbn (string) The ISBN of the book update-book-
-title = Ãditer les informations de `{ $isbn }` update-book-action = Ãditer
-update-book-failure = Le livre n'a pas pu Ãªtre mis Ã  jourÂ ! update-book-
-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-cancel = Annuler
-update-book-update = Enregistrer update-book-cover-help = Cliquez pour
-tÃ©lÃ©verser une nouvelle couverture update-book-cover-format-not-supported =
-Le format de cette couverture n'est pas supportÃ©Â ! book-already-exists = Ce
-livre est dÃ©jÃ  dans la collectionÂ ! # isbn (string) The ISBN of the book #
-url (string) The URL of the book book-added = Le livre {_$isbn_} a bien Ã©tÃ©
-ajoutÃ©Â ! book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-
-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La
-recherche n'a pas pu Ãªtre effectuÃ©eÂ !
+non authorisÃ©Â ! an-error-occurred = Une erreur s'est produiteÂ ! # date
+(Date) A date to format date = { $date } book = livre books = livres book-
+added-on = ajoutÃ© le book-updated-on = mis Ã  jour le book-isbn = ISBN book-
+isbn-description = Le numÃ©ro ISBN assignÃ© au livre, par exemple 978-0-7653-
+9277-0. book-title = titre book-title-description = Le titre du livre. book-
+year = annÃ©e book-year-description = L'annÃ©e de publication du livre. book-
+author = autÂ·riceÂ·eur book-author-description = UnÂ·e des autÂ·riceÂ·eurÂ·s
+du livre. book-authors = autÂ·riceÂ·eurÂ·s book-authors-description = La liste
+des autÂ·riceÂ·eurÂ·s du livre, sÃ©parÃ©Â·eÂ·s par des virgules. book-genre =
+genre book-genre-description = Un des genres auxquels le livre se rattache.
+book-genres = genres book-genres-description = La liste des genres auxquels le
+livre se rattache, sÃ©parÃ©s par des virgules. unknown-error = Une erreur
+inconnue s'est produiteÂ ! mandatory-value = Cette valeur est obligatoireÂ !
+incorrect-value = Cette valeur est incorrecteÂ ! not-an-isbn = Ceci n'est pas
+un ISBNÂ ! auth-login-title = Connexion # method (string) The sign in method
+auth-login-method = Sign in using { $method } webauthn-register-title =
+Association du dispositif de sÃ©curitÃ© webauthn-register-description = Votre
+navigateur devrait Ãªtre en train de vous demander de toucher votre dispositif
+de sÃ©curitÃ©â¦ webauthn-register-success = Votre dispositif de sÃ©curitÃ© a
+Ã©tÃ© correctement associÃ©Â ! webauthn-register-failure = Votre dispositif de
+sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion
+webauthn-login-description = Votre navigateur devrait Ãªtre en train de vous
+demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure =
+Vous n'avez pas pu Ãªtre connectÃ©Â·eÂ !? totp-login-title = Connexion totp-
+login-description = Merci de saisir votre mot de passe Ã  usage unique. totp-
+login-password = Mot de passe totp-login-action = Se connecter add-book-
+requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir
+ajouter un livreÂ ! add-book-title = Ajouter un nouveau livre Ã  la collection
+add-book-action = Ajouter un livre add-book-cancel = Annuler add-book-add =
+Ajouter add-book-cover-help = Cliquez pour tÃ©lÃ©verser une couverture add-
+book-cover-format-not-supported = Le format de cette couverture n'est pas
+supportÃ©Â ! search-books-title = Chercher un livre dans la collection search-
+books-action = Chercher un livre search-books-clear = RÃ©initialiser search-
+books-search = Chercher search-books-no-result = Aucun livre ne correspondÂ !
+search-books-previous-page = PrÃ©cÃ©dent search-books-next-page = Suivant #
+title (string) The title of the book display-book-title = DÃ©tails pour Â«Â 
+{ $title }Â Â» update-book-requires-authentification = Vous devez Ãªtre
+authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string) The ISBN of
+the book update-book-title = Ãditer les informations de `{ $isbn }` update-
+book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre mis Ã 
+jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-
+cancel = Annuler update-book-update = Enregistrer update-book-cover-help =
+Cliquez pour tÃ©lÃ©verser une nouvelle couverture update-book-cover-format-not-
+supported = Le format de cette couverture n'est pas supportÃ©Â ! book-already-
+exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! # isbn (string) The ISBN of
+the book # url (string) The URL of the book book-added = Le livre {_$isbn_} a
+bien Ã©tÃ© ajoutÃ©Â ! book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-
+cannot-be-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found =
+La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,24 +222,23 @@
         data: MultiDict[str, Any],
         /,
         *,
         notify: Callable[[str, str], None] = lambda m, t: None,
         user: Optional[User] = None,
     ) -> None:
         super().__init__("books/add", user=user)
-        self.set_status_code(HTTP.FORBIDDEN)
+        self.set_status_code(HTTP.OK)
         self.__data = data
         self.__notify = notify
         self.__context: dict[str, Any] = {"errors": {}}
 
     def render(self, **context: Any) -> str:
         return super().render(**self.__context, **context, data=self.__data)
 
     def bad_request(self, errors: add_book.Errors) -> None:
-        self.set_status_code(HTTP.OK)
         self.__context["errors"] = {
             "isbn": self.translate_error(errors.isbn),
             "title": self.translate_error(errors.title),
             "year": self.translate_error(errors.year),
             "authors": self.translate_error(errors.authors),
         }
 
@@ -315,14 +314,20 @@
         self.redirect(url_for("books.search"))
 
     def see_other(self, isbn: Isbn) -> None:
         self.redirect(url_for("books.display", isbn=str(isbn)), HTTP.MOVED_PERMANENTLY)
 
     def book(self, book: Book) -> None:
         self.__context["book"] = {
+            "added_on": self._("date", date=book.added_on.to_date()),
+            "updated_on": (
+                self._("date", date=book.updated_on.to_date())
+                if book.updated_on != book.added_on
+                else "-"
+            ),
             "isbn": str(book.isbn),
             "title": str(book.title),
             "year": int(book.year),
             "authors": ", ".join([str(a) for a in book.authors]),
             "genres": ", ".join([str(g) for g in book.genres]),
             "cover": str(book.cover) if book.cover else "",
         }
```

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 10% similar despite different names*

```diff
@@ -49,7 +49,11 @@
             dd= book.title
             dt= _("book-year")
             dd= book.year
             dt= _("book-authors")
             dd= book.authors
             dt= _("book-genres")
             dd= book.genres or "-"
+            dt= _("book-added-on")
+            dd= book.added_on
+            dt= _("book-updated-on")
+            dd= book.updated_on
```

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/bl_hector/interfaces/utils.py` & `bl_hector-0.1.0a7/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.0a6/pyproject.toml` & `bl_hector-0.1.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 exclude = [
     "**/*_spec.py",
@@ -18,15 +18,15 @@
 [tool.poetry.scripts]
 hector = "bl_hector.configuration.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Flask = "^2.3.2"
 pypugjs = "^5.9.12"
-bl-seth = "^0.1.2"
+bl-seth = "^0.2.0"
 isbnlib = "^3.10.14"
 jinja2-fragments = "^0.3.0"
 SQLAlchemy = "^2.0.15"
 typer = "^0.9.0"
 bl3d = "^0.3.0"
 "fluent.runtime" = "^0.4.0"
 webauthn = {version = "^1.8.1", optional = true}
```

### Comparing `bl_hector-0.1.0a6/setup.py` & `bl_hector-0.1.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                                           'templates/mixins/*',
                                           'templates/totp/*',
                                           'templates/webauthn/*']}
 
 install_requires = \
 ['Flask>=2.3.2,<3.0.0',
  'SQLAlchemy>=2.0.15,<3.0.0',
- 'bl-seth>=0.1.2,<0.2.0',
+ 'bl-seth>=0.2.0,<0.3.0',
  'bl3d>=0.3.0,<0.4.0',
  'fluent.runtime>=0.4.0,<0.5.0',
  'isbnlib>=3.10.14,<4.0.0',
  'jinja2-fragments>=0.3.0,<0.4.0',
  'pypugjs>=5.9.12,<6.0.0',
  'requests>=2.31.0,<3.0.0',
  'typer>=0.9.0,<0.10.0']
@@ -59,15 +59,15 @@
 {'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.0a6',
+    'version': '0.1.0a7',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nFor the time being, Hector cannot be installed from PyPI.\nSee [CONTRIBUTING.md]() to set up a development environment.\n\n\n## Configure\n\nHector is configured using environment variables.\nAll the variable names are prefixed with `HECTOR_`.\n\n```console\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\nThe secret can be generated using the `token_hex()` function from\nthe Python\'s `secrets` module.\n\nAdditional Python database drivers might be required depending on the DSN.\n\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN=1\n```\n\nTo enable TOTP authentication, you must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret (`pyotp.random_base32()`):\n\n```console\n$ export HECTOR_TOTP=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bl_hector-0.1.0a6/PKG-INFO` & `bl_hector-0.1.0a7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: A collection manager.
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: totp
 Provides-Extra: webauthn
 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
-Requires-Dist: bl-seth (>=0.1.2,<0.2.0)
+Requires-Dist: bl-seth (>=0.2.0,<0.3.0)
 Requires-Dist: bl3d (>=0.3.0,<0.4.0)
 Requires-Dist: fluent.runtime (>=0.4.0,<0.5.0)
 Requires-Dist: isbnlib (>=3.10.14,<4.0.0)
 Requires-Dist: jinja2-fragments (>=0.3.0,<0.4.0)
 Requires-Dist: pyotp (>=2.8.0,<3.0.0)
 Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

