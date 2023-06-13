# Comparing `tmp/spade-3.2.3.tar.gz` & `tmp/spade-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade-3.2.3.tar", last modified: Tue Dec 13 18:38:39 2022, max compression
+gzip compressed data, was "spade-3.3.0.tar", last modified: Tue Jun 13 13:39:28 2023, max compression
```

## Comparing `spade-3.2.3.tar` & `spade-3.3.0.tar`

### file list

```diff
@@ -1,89 +1,142 @@
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.911892 spade-3.2.3/
--rw-r--r--   0 jpalanca   (501) staff       (20)      184 2020-05-21 17:15:51.000000 spade-3.2.3/AUTHORS.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     3325 2020-05-21 17:15:51.000000 spade-3.2.3/CONTRIBUTING.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     3479 2022-12-13 17:52:56.000000 spade-3.2.3/HISTORY.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1072 2020-05-21 17:15:51.000000 spade-3.2.3/LICENSE
--rw-r--r--   0 jpalanca   (501) staff       (20)      354 2020-05-21 17:15:51.000000 spade-3.2.3/MANIFEST.in
--rw-r--r--   0 jpalanca   (501) staff       (20)     7672 2022-12-13 18:38:39.912132 spade-3.2.3/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     3205 2022-12-13 17:52:51.000000 spade-3.2.3/README.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.869628 spade-3.2.3/docs/
--rw-r--r--   0 jpalanca   (501) staff       (20)     6758 2020-05-21 17:15:51.000000 spade-3.2.3/docs/Makefile
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.842277 spade-3.2.3/docs/_build/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.842573 spade-3.2.3/docs/_build/html/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.875848 spade-3.2.3/docs/_build/html/_images/
--rw-r--r--   0 jpalanca   (501) staff       (20)   126989 2020-05-21 17:15:51.000000 spade-3.2.3/docs/_build/html/_images/spade_behaviour.png
--rw-r--r--   0 jpalanca   (501) staff       (20)   107642 2020-05-21 17:15:51.000000 spade-3.2.3/docs/_build/html/_images/spade_friend.png
--rw-r--r--   0 jpalanca   (501) staff       (20)   143813 2020-05-21 17:15:51.000000 spade-3.2.3/docs/_build/html/_images/spade_index.png
--rw-r--r--   0 jpalanca   (501) staff       (20)    48556 2020-05-21 17:15:51.000000 spade-3.2.3/docs/_build/html/_images/spade_msg.png
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.879146 spade-3.2.3/docs/_build/html/_static/
--rw-r--r--   0 jpalanca   (501) staff       (20)      286 2022-12-13 17:40:50.000000 spade-3.2.3/docs/_build/html/_static/file.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2022-12-13 17:40:50.000000 spade-3.2.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2022-12-13 17:40:50.000000 spade-3.2.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)     8605 2022-12-13 17:52:56.000000 spade-3.2.3/docs/agents.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       76 2020-05-21 17:15:51.000000 spade-3.2.3/docs/api.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2020-05-21 17:15:51.000000 spade-3.2.3/docs/authors.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)    13980 2022-12-13 17:51:26.000000 spade-3.2.3/docs/behaviours.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       36 2020-05-21 18:16:08.000000 spade-3.2.3/docs/conduct.rst
--rwxr-xr-x   0 jpalanca   (501) staff       (20)     8471 2020-05-21 18:16:08.000000 spade-3.2.3/docs/conf.py
--rw-r--r--   0 jpalanca   (501) staff       (20)       33 2020-05-21 17:15:51.000000 spade-3.2.3/docs/contributing.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     5546 2022-12-13 17:51:26.000000 spade-3.2.3/docs/extending.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1822 2020-05-21 17:15:51.000000 spade-3.2.3/docs/foreword.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2020-05-21 17:15:51.000000 spade-3.2.3/docs/history.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.886302 spade-3.2.3/docs/images/
--rw-r--r--   0 jpalanca   (501) staff       (20)   126989 2020-05-21 17:15:51.000000 spade-3.2.3/docs/images/spade_behaviour.png
--rw-r--r--   0 jpalanca   (501) staff       (20)   107642 2020-05-21 17:15:51.000000 spade-3.2.3/docs/images/spade_friend.png
--rw-r--r--   0 jpalanca   (501) staff       (20)   143813 2020-05-21 17:15:51.000000 spade-3.2.3/docs/images/spade_index.png
--rw-r--r--   0 jpalanca   (501) staff       (20)    48556 2020-05-21 17:15:51.000000 spade-3.2.3/docs/images/spade_msg.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      375 2020-05-21 18:16:08.000000 spade-3.2.3/docs/index.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1111 2020-05-21 17:15:51.000000 spade-3.2.3/docs/installation.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     6457 2020-05-21 17:15:51.000000 spade-3.2.3/docs/make.bat
--rw-r--r--   0 jpalanca   (501) staff       (20)     2720 2020-05-21 17:15:51.000000 spade-3.2.3/docs/model.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       52 2022-12-13 17:40:55.000000 spade-3.2.3/docs/modules.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     9993 2020-05-21 17:15:51.000000 spade-3.2.3/docs/presence.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       27 2020-05-21 17:15:51.000000 spade-3.2.3/docs/readme.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1179 2022-12-13 17:52:51.000000 spade-3.2.3/docs/spade.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)    10984 2022-12-13 17:51:26.000000 spade-3.2.3/docs/usage.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     9105 2020-05-21 17:15:51.000000 spade-3.2.3/docs/web.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      205 2022-12-13 17:52:51.000000 spade-3.2.3/requirements.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)      464 2022-12-13 17:52:51.000000 spade-3.2.3/requirements_dev.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)      403 2022-12-13 18:38:39.912905 spade-3.2.3/setup.cfg
--rw-r--r--   0 jpalanca   (501) staff       (20)     2128 2022-12-13 17:52:56.000000 spade-3.2.3/setup.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.893978 spade-3.2.3/spade/
--rw-r--r--   0 jpalanca   (501) staff       (20)      325 2022-12-13 17:52:56.000000 spade-3.2.3/spade/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    12282 2022-12-13 17:51:26.000000 spade-3.2.3/spade/agent.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    18949 2022-12-13 17:51:26.000000 spade-3.2.3/spade/behaviour.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     5069 2022-12-13 17:52:56.000000 spade-3.2.3/spade/container.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     8040 2022-12-13 17:51:26.000000 spade-3.2.3/spade/message.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    10484 2022-12-13 17:51:26.000000 spade-3.2.3/spade/presence.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     2657 2022-12-13 17:51:26.000000 spade-3.2.3/spade/template.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.903371 spade-3.2.3/spade/templates/
--rw-r--r--   0 jpalanca   (501) staff       (20)     3414 2020-05-21 17:15:51.000000 spade-3.2.3/spade/templates/internal_tpl_agent.html
--rw-r--r--   0 jpalanca   (501) staff       (20)    15182 2020-05-21 17:15:51.000000 spade-3.2.3/spade/templates/internal_tpl_base.html
--rw-r--r--   0 jpalanca   (501) staff       (20)     5152 2020-05-21 17:15:51.000000 spade-3.2.3/spade/templates/internal_tpl_behaviour.html
--rw-r--r--   0 jpalanca   (501) staff       (20)     4729 2020-05-21 17:15:51.000000 spade-3.2.3/spade/templates/internal_tpl_index.html
--rw-r--r--   0 jpalanca   (501) staff       (20)     6355 2020-05-21 17:15:51.000000 spade-3.2.3/spade/templates/internal_tpl_macros.html
--rw-r--r--   0 jpalanca   (501) staff       (20)     3036 2020-05-21 17:15:51.000000 spade-3.2.3/spade/templates/internal_tpl_messages.html
--rw-r--r--   0 jpalanca   (501) staff       (20)     3462 2022-12-13 17:51:26.000000 spade-3.2.3/spade/trace.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    10147 2022-12-13 17:51:26.000000 spade-3.2.3/spade/web.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.898427 spade-3.2.3/spade.egg-info/
--rw-r--r--   0 jpalanca   (501) staff       (20)     7672 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     1729 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/SOURCES.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/dependency_links.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       41 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/entry_points.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/not-zip-safe
--rw-r--r--   0 jpalanca   (501) staff       (20)      178 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/requires.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        6 2022-12-13 18:38:39.000000 spade-3.2.3/spade.egg-info/top_level.txt
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-12-13 18:38:39.911143 spade-3.2.3/tests/
--rw-r--r--   0 jpalanca   (501) staff       (20)       60 2020-05-21 17:15:51.000000 spade-3.2.3/tests/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     1347 2020-05-22 16:02:53.000000 spade-3.2.3/tests/conftest.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     1657 2020-05-21 18:16:14.000000 spade-3.2.3/tests/factories.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      299 2020-05-21 17:15:51.000000 spade-3.2.3/tests/hello.html
--rw-r--r--   0 jpalanca   (501) staff       (20)     6358 2020-05-21 18:16:14.000000 spade-3.2.3/tests/test_agent.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    31026 2022-12-13 17:51:26.000000 spade-3.2.3/tests/test_behaviour.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     3873 2020-05-22 16:02:53.000000 spade-3.2.3/tests/test_container.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     4977 2020-05-21 18:16:08.000000 spade-3.2.3/tests/test_message.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     2072 2022-12-13 17:51:26.000000 spade-3.2.3/tests/test_plugin.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    14907 2020-05-21 18:16:08.000000 spade-3.2.3/tests/test_presence.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     7009 2020-05-21 17:15:51.000000 spade-3.2.3/tests/test_template.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     5231 2022-12-13 17:52:51.000000 spade-3.2.3/tests/test_trace.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    11659 2022-12-13 17:51:26.000000 spade-3.2.3/tests/test_web.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.848612 spade-3.3.0/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      184 2018-09-07 16:35:15.000000 spade-3.3.0/AUTHORS.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3325 2018-09-07 16:35:15.000000 spade-3.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3704 2023-06-13 13:36:04.000000 spade-3.3.0/HISTORY.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1072 2018-09-07 16:35:15.000000 spade-3.3.0/LICENSE
+-rw-r--r--   0 jpalanca   (501) staff       (20)      354 2018-09-07 16:35:15.000000 spade-3.3.0/MANIFEST.in
+-rw-r--r--   0 jpalanca   (501) staff       (20)     7853 2023-06-13 13:39:28.848888 spade-3.3.0/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3190 2023-06-13 13:36:04.000000 spade-3.3.0/README.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.761264 spade-3.3.0/docs/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     6758 2018-09-07 16:35:15.000000 spade-3.3.0/docs/Makefile
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.738417 spade-3.3.0/docs/_build/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.738725 spade-3.3.0/docs/_build/html/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.769517 spade-3.3.0/docs/_build/html/_images/
+-rw-r--r--   0 jpalanca   (501) staff       (20)   126989 2018-09-07 16:35:15.000000 spade-3.3.0/docs/_build/html/_images/spade_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)   107642 2018-09-07 16:35:15.000000 spade-3.3.0/docs/_build/html/_images/spade_friend.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)   143813 2018-09-07 16:35:15.000000 spade-3.3.0/docs/_build/html/_images/spade_index.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)    48556 2018-09-07 16:35:15.000000 spade-3.3.0/docs/_build/html/_images/spade_msg.png
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.772063 spade-3.3.0/docs/_build/html/_static/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      286 2023-03-07 16:02:16.000000 spade-3.3.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2023-03-07 16:02:16.000000 spade-3.3.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2023-03-07 16:02:16.000000 spade-3.3.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     8192 2023-06-13 13:35:55.000000 spade-3.3.0/docs/agents.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       76 2018-09-12 16:07:17.000000 spade-3.3.0/docs/api.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-07 16:35:15.000000 spade-3.3.0/docs/authors.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)    13316 2023-06-13 13:35:55.000000 spade-3.3.0/docs/behaviours.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       36 2019-05-14 14:36:34.000000 spade-3.3.0/docs/conduct.rst
+-rwxr-xr-x   0 jpalanca   (501) staff       (20)     8471 2021-04-07 15:58:09.000000 spade-3.3.0/docs/conf.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)       33 2018-09-07 16:35:15.000000 spade-3.3.0/docs/contributing.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.739037 spade-3.3.0/docs/doxy/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.814873 spade-3.3.0/docs/doxy/html/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      676 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/bc_s.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      635 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/bc_sd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      147 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/bdwn.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      490 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1agent_1_1_agent.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      674 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1agent_1_1_authentication_failure.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      862 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_behaviour_not_finished_exception.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2808 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_cyclic_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1755 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_f_s_m_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      663 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_not_valid_state.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      697 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_not_valid_transition.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3130 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_one_shot_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2301 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_periodic_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3473 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_state.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3499 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1behaviour_1_1_timeout_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      581 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1container_1_1_aio_thread.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      557 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1container_1_1_container.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      928 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1message_1_1_message.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1393 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1message_1_1_message_base.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      680 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1presence_1_1_contact_not_found.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      638 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1presence_1_1_presence_manager.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1385 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1template_1_1_a_n_d_template.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2348 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1template_1_1_base_template.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1363 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1template_1_1_n_o_t_template.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1353 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1template_1_1_o_r_template.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1996 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1template_1_1_template.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1378 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1template_1_1_x_o_r_template.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      560 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1trace_1_1_trace_store.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      493 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/classspade_1_1web_1_1_web_app.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      132 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/closed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      746 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/doc.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      756 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/docd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      616 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/folderclosed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      597 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/folderopen.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      153 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/nav_f.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      169 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/nav_fd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       95 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/nav_g.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       98 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/nav_h.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      114 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/nav_hd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      123 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/open.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      314 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/splitbar.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      282 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/splitbard.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      853 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/sync_off.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      845 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/sync_on.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      142 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_a.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      135 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_ad.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      169 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_b.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      173 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_bd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      177 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_h.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      180 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_hd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      184 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_s.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      188 2022-09-29 12:53:48.000000 spade-3.3.0/docs/doxy/html/tab_sd.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)     5546 2021-06-25 14:22:09.000000 spade-3.3.0/docs/extending.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1822 2018-09-07 16:35:15.000000 spade-3.3.0/docs/foreword.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-07 16:35:15.000000 spade-3.3.0/docs/history.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.822057 spade-3.3.0/docs/images/
+-rw-r--r--   0 jpalanca   (501) staff       (20)   126989 2018-09-07 16:35:15.000000 spade-3.3.0/docs/images/spade_behaviour.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)   107642 2018-09-07 16:35:15.000000 spade-3.3.0/docs/images/spade_friend.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)   143813 2018-09-07 16:35:15.000000 spade-3.3.0/docs/images/spade_index.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)    48556 2018-09-07 16:35:15.000000 spade-3.3.0/docs/images/spade_msg.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      375 2019-05-14 14:36:34.000000 spade-3.3.0/docs/index.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1111 2018-09-07 16:35:15.000000 spade-3.3.0/docs/installation.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     6457 2018-09-07 16:35:15.000000 spade-3.3.0/docs/make.bat
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2720 2018-09-07 16:35:15.000000 spade-3.3.0/docs/model.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       52 2023-06-13 13:39:01.000000 spade-3.3.0/docs/modules.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)    10096 2023-06-13 13:35:55.000000 spade-3.3.0/docs/presence.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       27 2018-09-07 16:35:15.000000 spade-3.3.0/docs/readme.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1179 2023-06-13 13:39:01.000000 spade-3.3.0/docs/spade.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)    10091 2023-06-13 13:35:55.000000 spade-3.3.0/docs/usage.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     9120 2023-06-13 13:35:55.000000 spade-3.3.0/docs/web.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      239 2023-06-13 13:35:55.000000 spade-3.3.0/requirements.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      493 2023-06-13 13:35:55.000000 spade-3.3.0/requirements_dev.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      543 2023-06-13 13:39:28.850085 spade-3.3.0/setup.cfg
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2080 2023-06-13 13:36:04.000000 spade-3.3.0/setup.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.828286 spade-3.3.0/spade/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      885 2023-06-13 13:36:04.000000 spade-3.3.0/spade/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    11771 2023-06-13 13:35:55.000000 spade-3.3.0/spade/agent.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    18590 2023-06-13 13:35:55.000000 spade-3.3.0/spade/behaviour.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3795 2023-06-13 13:35:55.000000 spade-3.3.0/spade/container.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     8040 2023-06-13 13:35:55.000000 spade-3.3.0/spade/message.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    10484 2021-11-25 12:12:20.000000 spade-3.3.0/spade/presence.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2657 2021-11-25 12:12:20.000000 spade-3.3.0/spade/template.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.836953 spade-3.3.0/spade/templates/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3414 2018-10-24 16:37:21.000000 spade-3.3.0/spade/templates/internal_tpl_agent.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)    15182 2023-06-13 13:36:04.000000 spade-3.3.0/spade/templates/internal_tpl_base.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)     5152 2018-09-12 16:07:08.000000 spade-3.3.0/spade/templates/internal_tpl_behaviour.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)     4729 2018-10-24 16:37:21.000000 spade-3.3.0/spade/templates/internal_tpl_index.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)     6355 2018-10-24 16:37:21.000000 spade-3.3.0/spade/templates/internal_tpl_macros.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3036 2018-09-12 16:07:08.000000 spade-3.3.0/spade/templates/internal_tpl_messages.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3462 2021-11-25 12:12:20.000000 spade-3.3.0/spade/trace.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    10131 2023-06-13 13:35:55.000000 spade-3.3.0/spade/web.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.832397 spade-3.3.0/spade.egg-info/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     7853 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3921 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/SOURCES.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/dependency_links.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)       42 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/entry_points.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/not-zip-safe
+-rw-r--r--   0 jpalanca   (501) staff       (20)      186 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/requires.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        6 2023-06-13 13:39:28.000000 spade-3.3.0/spade.egg-info/top_level.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 13:39:28.847728 spade-3.3.0/tests/
+-rw-r--r--   0 jpalanca   (501) staff       (20)       60 2018-09-07 16:35:15.000000 spade-3.3.0/tests/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1311 2023-06-13 13:35:55.000000 spade-3.3.0/tests/conftest.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1637 2023-06-13 13:35:55.000000 spade-3.3.0/tests/factories.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      299 2021-04-07 15:58:09.000000 spade-3.3.0/tests/hello.html
+-rw-r--r--   0 jpalanca   (501) staff       (20)     5437 2023-06-13 13:35:55.000000 spade-3.3.0/tests/test_agent.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    30926 2023-06-13 13:35:55.000000 spade-3.3.0/tests/test_behaviour.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3381 2023-06-13 13:35:55.000000 spade-3.3.0/tests/test_container.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     4977 2021-04-07 15:58:09.000000 spade-3.3.0/tests/test_message.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2036 2023-06-13 13:35:55.000000 spade-3.3.0/tests/test_plugin.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    14268 2023-06-13 13:35:55.000000 spade-3.3.0/tests/test_presence.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     7009 2018-09-07 16:35:15.000000 spade-3.3.0/tests/test_template.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     5231 2023-06-13 13:33:42.000000 spade-3.3.0/tests/test_trace.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    11706 2023-06-13 13:35:55.000000 spade-3.3.0/tests/test_web.py
```

### Comparing `spade-3.2.3/CONTRIBUTING.rst` & `spade-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/HISTORY.rst` & `spade-3.3.0/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 =======
 History
 =======
 
-3.2.3 (2023-12-13)
+3.3.0 (2023-06-13)
+------------------
+
+* Updated to Python>=3.8
+* Changed the way agents are launched (now with `spade.run()`)
+* Python 3.11 still not supported due to a bug in `aiohttp`
+* Deprecated support for Python<=3.7
+
+3.2.3 (2022-12-13)
 ------------------
 
 * Updated third-party libs
 
 3.2.2 (2021-11-25)
 ------------------
```

### Comparing `spade-3.2.3/LICENSE` & `spade-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/PKG-INFO` & `spade-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spade
-Version: 3.2.3
+Version: 3.3.0
 Summary: Smart Python Agent Development Environment
 Home-page: https://github.com/javipalanca/spade
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
 Keywords: spade
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Internet :: XMPP
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -43,15 +43,15 @@
     :alt: Languages
     :target: https://pepy.tech/project/spade
 
 .. image:: https://img.shields.io/github/languages/code-size/javipalanca/spade
     :alt: Code Size
     :target: https://pepy.tech/project/spade
 
-.. image:: https://img.shields.io/apm/l/atomic-design-ui.svg?
+.. image:: https://img.shields.io/pypi/l/spade
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 .. image:: https://pepy.tech/badge/spade
     :target: https://pepy.tech/project/spade
     :alt: Downloads
 
@@ -85,15 +85,15 @@
 
 
 Features
 --------
 
 * Multi-agent platform based on XMPP_
 * Presence notification allows the system to know the current state of the agents in real-time
-* Python >=3.6
+* Python >=3.8
 * Asyncio-based
 * Agent model based on behaviours
 * Supports FIPA metadata using XMPP Data Forms (XEP-0004_: Data Forms)
 * Web-based interface
 * Use any XMPP server
 
 Plugins
@@ -123,15 +123,23 @@
 
 
 
 =======
 History
 =======
 
-3.2.3 (2023-12-13)
+3.3.0 (2023-06-13)
+------------------
+
+* Updated to Python>=3.8
+* Changed the way agents are launched (now with `spade.run()`)
+* Python 3.11 still not supported due to a bug in `aiohttp`
+* Deprecated support for Python<=3.7
+
+3.2.3 (2022-12-13)
 ------------------
 
 * Updated third-party libs
 
 3.2.2 (2021-11-25)
 ------------------
 
@@ -281,7 +289,9 @@
 * Minor doc fixings and improvements.
 
 
 3.0.0 (2017-10-06)
 ------------------
 
 * Started writing 3.0 version.
+
+
```

### Comparing `spade-3.2.3/README.rst` & `spade-3.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     :alt: Languages
     :target: https://pepy.tech/project/spade
 
 .. image:: https://img.shields.io/github/languages/code-size/javipalanca/spade
     :alt: Code Size
     :target: https://pepy.tech/project/spade
 
-.. image:: https://img.shields.io/apm/l/atomic-design-ui.svg?
+.. image:: https://img.shields.io/pypi/l/spade
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 .. image:: https://pepy.tech/badge/spade
     :target: https://pepy.tech/project/spade
     :alt: Downloads
 
@@ -59,15 +59,15 @@
 
 
 Features
 --------
 
 * Multi-agent platform based on XMPP_
 * Presence notification allows the system to know the current state of the agents in real-time
-* Python >=3.6
+* Python >=3.8
 * Asyncio-based
 * Agent model based on behaviours
 * Supports FIPA metadata using XMPP Data Forms (XEP-0004_: Data Forms)
 * Web-based interface
 * Use any XMPP server
 
 Plugins
```

### Comparing `spade-3.2.3/docs/Makefile` & `spade-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/_build/html/_images/spade_behaviour.png` & `spade-3.3.0/docs/_build/html/_images/spade_behaviour.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/_build/html/_images/spade_friend.png` & `spade-3.3.0/docs/_build/html/_images/spade_friend.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/_build/html/_images/spade_index.png` & `spade-3.3.0/docs/_build/html/_images/spade_index.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/_build/html/_images/spade_msg.png` & `spade-3.3.0/docs/_build/html/_images/spade_msg.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/agents.rst` & `spade-3.3.0/docs/agents.rst`

 * *Files 7% similar despite different names*

```diff
@@ -82,18 +82,19 @@
 destination. Note that the send function is an async coroutine, so it needs to be called with an ``await`` statement.
 
 .. warning:: Remember to change the example's jids and passwords by your own accounts. These accounts do not exist
     and are only for demonstration purposes.
 
 Here is a self-explaining example::
 
-    import time
+    import spade
     from spade.agent import Agent
     from spade.behaviour import OneShotBehaviour
     from spade.message import Message
+    from spade.template import Template
 
 
     class SenderAgent(Agent):
         class InformBehav(OneShotBehaviour):
             async def run(self):
                 print("InformBehav running")
                 msg = Message(to="receiver@your_xmpp_server")     # Instantiate the message
@@ -113,26 +114,25 @@
 
         async def setup(self):
             print("SenderAgent started")
             self.b = self.InformBehav()
             self.add_behaviour(self.b)
 
 
+    async def main():
+        senderagent = SenderAgent("sender@your_xmpp_server", "sender_password")
+        await senderagent.start(auto_register=True)
+        print("Sender started")
+
+        await spade.wait_until_finished(receiveragent)
+        print("Agents finished")
+
+
     if __name__ == "__main__":
-        agent = SenderAgent("sender@your_xmpp_server", "sender_password")
-        future = agent.start()
-        future.result()
-
-        while agent.is_alive():
-            try:
-                time.sleep(1)
-            except KeyboardInterrupt:
-                agent.stop()
-                break
-        print("Agent finished with exit code: {}".format(agent.b.exit_code))
+        spade.run(main())
 
 
 
 This code would output::
 
     $ python sender.py
     SenderAgent started
@@ -140,15 +140,15 @@
     Message sent!
     Agent finished with exit code: Job Finished!
 
 
 
 Ok, we have sent a message but now we need someone to receive that message. Show me the code::
 
-    import time
+    import spade
     from spade.agent import Agent
     from spade.behaviour import OneShotBehaviour
     from spade.message import Message
     from spade.template import Template
 
 
     class SenderAgent(Agent):
@@ -189,47 +189,46 @@
             b = self.RecvBehav()
             template = Template()
             template.set_metadata("performative", "inform")
             self.add_behaviour(b, template)
 
 
 
-    if __name__ == "__main__":
+    async def main():
         receiveragent = ReceiverAgent("receiver@your_xmpp_server", "receiver_password")
-        future = receiveragent.start()
-        future.wait() # wait for receiver agent to be prepared.
+        await receiveragent.start(auto_register=True)
+        print("Receiver started")
+
         senderagent = SenderAgent("sender@your_xmpp_server", "sender_password")
-        senderagent.start()
+        await senderagent.start(auto_register=True)
+        print("Sender started")
 
-        while receiveragent.is_alive():
-            try:
-                time.sleep(1)
-            except KeyboardInterrupt:
-                senderagent.stop()
-                receiveragent.stop()
-                break
+        await spade.wait_until_finished(receiveragent)
         print("Agents finished")
 
 
+    if __name__ == "__main__":
+        spade.run(main())
+
+
 .. note:: It's important to remember that the send and receive functions are **coroutines**, so they **always**
     must be called with the ``await`` statement.
 
 In this example you can see how the ``RecvBehav`` behaviour receives the message because the template includes a
 *performative* with the value **inform** in the metadata and the sent message does also include that metadata, so the
 message and the template match.
 
-You can also note that we are using an *ugly* ``time.sleep`` to introduce an explicit wait to avoid sending the message
-before the receiver agent is up and ready since in another case the message would never be received (remember that spade
-is a **real-time** messaging platform. In future sections we'll show you how to use *presence notification* to wait for
-an agent to be *available*.
-
 The code below would output::
 
     $ python send_and_recv.py
     ReceiverAgent started
+    Receiver started
     RecvBehav running
     SenderAgent started
+    Sender started
     InformBehav running
     Message sent!
     Message received with content: Hello World
     Agents finished
 
+    Process finished with exit code 0
+
```

### Comparing `spade-3.2.3/docs/behaviours.rst` & `spade-3.3.0/docs/behaviours.rst`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 .. warning:: Remember to change the example's jids and passwords by your own accounts. These accounts do not exist
     and are only for demonstration purposes.
 
 Let's see an example::
 
     import datetime
     import getpass
-    import time
 
-    from spade import quit_spade
+    import spade
     from spade.agent import Agent
     from spade.behaviour import CyclicBehaviour, PeriodicBehaviour
     from spade.message import Message
 
 
     class PeriodicSenderAgent(Agent):
         class InformBehav(PeriodicBehaviour):
@@ -68,39 +67,36 @@
                 await self.agent.stop()
 
         async def setup(self):
             print("ReceiverAgent started")
             b = self.RecvBehav()
             self.add_behaviour(b)
 
-
-    if __name__ == "__main__":
+    async def main():
         receiver_jid = input("Receiver JID> ")
         passwd = getpass.getpass()
         receiveragent = ReceiverAgent(receiver_jid, passwd)
 
         sender_jid = input("Sender JID> ")
         passwd = getpass.getpass()
         senderagent = PeriodicSenderAgent(sender_jid, passwd)
 
-        future = receiveragent.start(auto_register=True)
-        future.result()  # wait for receiver agent to be prepared.
+        await receiveragent.start(auto_register=True)
 
         senderagent.set("receiver_jid", receiver_jid)  # store receiver_jid in the sender knowledge base
-        senderagent.start(auto_register=True)
+        await senderagent.start(auto_register=True)
 
-        while receiveragent.is_alive():
-            try:
-                time.sleep(1)
-            except KeyboardInterrupt:
-                senderagent.stop()
-                receiveragent.stop()
-                break
+        await spade.wait_until_finished(receiveragent)
+        await senderagent.stop()
+        await receiveragent.stop()
         print("Agents finished")
-        quit_spade()
+
+
+    if __name__ == "__main__":
+        spade.run(main())
 
 The output of this code would be similar to::
 
     $ python periodic.py
     ReceiverAgent started
     RecvBehav running
     PeriodicSenderAgent started at 17:40:39.901903
@@ -138,16 +134,16 @@
 
 You can also create a ``TimeoutBehaviour`` which is run once (like OneShotBehaviours) but its activation is triggered at
 a specified ``datetime`` just as in ``PeriodicBehaviours``.
 
 Let's see an example::
 
     import getpass
-    import time
     import datetime
+    import spade
     from spade.agent import Agent
     from spade.behaviour import CyclicBehaviour, TimeoutBehaviour
     from spade.message import Message
 
 
     class TimeoutSenderAgent(Agent):
         class InformBehav(TimeoutBehaviour):
@@ -182,38 +178,37 @@
                 await self.agent.stop()
 
         async def setup(self):
             b = self.RecvBehav()
             self.add_behaviour(b)
 
 
-    if __name__ == "__main__":
+    async def main():
         receiver_jid = input("Receiver JID> ")
         passwd = getpass.getpass()
         receiveragent = ReceiverAgent(receiver_jid, passwd)
 
         sender_jid = input("Sender JID> ")
         passwd = getpass.getpass()
         senderagent = TimeoutSenderAgent(sender_jid, passwd)
 
-        future = receiveragent.start(auto_register=True)
-        future.result()  # wait for receiver agent to be prepared.
+        await receiveragent.start(auto_register=True)
 
         senderagent.set("receiver_jid", receiver_jid)  # store receiver_jid in the sender knowledge base
-        senderagent.start(auto_register=True)
+        await senderagent.start(auto_register=True)
 
-        while receiveragent.is_alive():
-            try:
-                time.sleep(1)
-            except KeyboardInterrupt:
-                senderagent.stop()
-                receiveragent.stop()
-                break
+        await spade.wait_until_finished(receiveragent)
+        await senderagent.stop()
+        await receiveragent.stop()
         print("Agents finished")
 
+    if __name__ == "__main__":
+        spade.run(main())
+
+
 This would produce the following output::
 
     $python timeout.py
     TimeoutSenderAgent started at 18:12:09.620316
     TimeoutSenderBehaviour running at 18:12:14.625403
     Message received with content: Hello World
     Did not received any message after 10 seconds
@@ -253,16 +248,15 @@
 when you describe your FSM states, because they will share the same message queue.
 
 Next, we are going to see an example where a very simple FSM is defined, with three states, which transitate from one
 state to the next one in order. It also sends a message to itself at the first initial state, which is received at the
 third (and final) state. Also note that the third state is a final state because it does not set a *next_state* to
 transit to::
 
-    import time
-
+    import spade
     from spade.agent import Agent
     from spade.behaviour import FSMBehaviour, State
     from spade.message import Message
 
     STATE_ONE = "STATE_ONE"
     STATE_TWO = "STATE_TWO"
     STATE_THREE = "STATE_THREE"
@@ -307,43 +301,37 @@
             fsm.add_state(name=STATE_TWO, state=StateTwo())
             fsm.add_state(name=STATE_THREE, state=StateThree())
             fsm.add_transition(source=STATE_ONE, dest=STATE_TWO)
             fsm.add_transition(source=STATE_TWO, dest=STATE_THREE)
             self.add_behaviour(fsm)
 
 
-    if __name__ == "__main__":
+    async def main():
         fsmagent = FSMAgent("fsmagent@your_xmpp_server", "your_password")
-        future = fsmagent.start()
-        future.result()
+        await fsmagent.start()
 
-        while fsmagent.is_alive():
-            try:
-                time.sleep(1)
-            except KeyboardInterrupt:
-                fsmagent.stop()
-                break
+        await spade.wait_until_finished(fsmagent)
+        await fsmagent.stop()
         print("Agent finished")
 
-
+    if __name__ == "__main__":
+        spade.run(main())
 
 
 Waiting a Behaviour
 -------------------
 
 Sometimes you may need to wait for a behaviour to finish. In order to make this easy, behaviours provide a method called
 ``join``. Using this method you can wait for a behaviour to be finished. Be careful, since this is a blocking operation.
-In order to make it usable inside and outside coroutines, this is also a morphing method (like ``start`` and ``stop``)
-which behaves different depending on the context. It returns a coroutine or a future depending on whether it is called
-from a coroutine or a synchronous method. Example::
+Example::
 
     import asyncio
     import getpass
 
-    from spade import quit_spade
+    import spade
     from spade.agent import Agent
     from spade.behaviour import OneShotBehaviour
 
 
     class DummyAgent(Agent):
         class LongBehav(OneShotBehaviour):
             async def run(self):
@@ -359,22 +347,22 @@
             print("Agent starting . . .")
             self.behav = self.LongBehav()
             self.add_behaviour(self.behav)
             self.behav2 = self.WaitingBehav()
             self.add_behaviour(self.behav2)
 
 
-    if __name__ == "__main__":
-
+    async def main():
         jid = input("JID> ")
         passwd = getpass.getpass()
 
         dummy = DummyAgent(jid, passwd)
-        future = dummy.start()
-        future.result()
-
-        dummy.behav2.join()  # this join must not be awaited
+        await dummy.start()
 
+        await dummy.behav2.join()
         print("Stopping agent.")
-        dummy.stop()
+        await dummy.stop()
+
+
+    if __name__ == "__main__":
+        spade.run(main())
 
-        quit_spade()
```

### Comparing `spade-3.2.3/docs/conf.py` & `spade-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/extending.rst` & `spade-3.3.0/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/foreword.rst` & `spade-3.3.0/docs/foreword.rst`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/images/spade_behaviour.png` & `spade-3.3.0/docs/images/spade_behaviour.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/images/spade_friend.png` & `spade-3.3.0/docs/images/spade_friend.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/images/spade_index.png` & `spade-3.3.0/docs/images/spade_index.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/images/spade_msg.png` & `spade-3.3.0/docs/images/spade_msg.png`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/installation.rst` & `spade-3.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/make.bat` & `spade-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/model.rst` & `spade-3.3.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/presence.rst` & `spade-3.3.0/docs/presence.rst`

 * *Files 5% similar despite different names*

```diff
@@ -178,17 +178,18 @@
 
 
 Example
 -------
 
 This is an example that shows in a practical way the presence module::
 
-    import time
     import getpass
+    import asyncio
 
+    import spade
     from spade.agent import Agent
     from spade.behaviour import OneShotBehaviour
 
 
     class Agent1(Agent):
         async def setup(self):
             print("Agent {} running".format(self.name))
@@ -236,30 +237,34 @@
             async def run(self):
                 self.presence.set_available()
                 self.presence.on_subscribe = self.on_subscribe
                 self.presence.on_subscribed = self.on_subscribed
                 self.presence.on_available = self.on_available
 
 
-    if __name__ == "__main__":
-
+    async def main():
         jid1 = input("Agent1 JID> ")
         passwd1 = getpass.getpass()
 
         jid2 = input("Agent2 JID> ")
         passwd2 = getpass.getpass()
 
         agent2 = Agent2(jid2, passwd2)
         agent1 = Agent1(jid1, passwd1)
         agent1.jid2 = jid2
         agent2.jid1 = jid1
-        agent2.start()
-        agent1.start()
+        await agent2.start()
+        await agent1.start()
 
         while True:
             try:
-                time.sleep(1)
+                await asyncio.sleep(1)
             except KeyboardInterrupt:
                 break
-        agent1.stop()
-        agent2.stop()
+        await agent1.stop()
+        await agent2.stop()
+
+
+    if __name__ == "__main__":
+        spade.run(main())
+
```

### Comparing `spade-3.2.3/docs/spade.rst` & `spade-3.3.0/docs/spade.rst`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/docs/usage.rst` & `spade-3.3.0/docs/usage.rst`

 * *Files 6% similar despite different names*

```diff
@@ -18,40 +18,41 @@
 For starters, fire up you favorite Python editor and create a file called ``dummyagent.py``.
 
 .. warning:: Remember to change the example's jids and passwords by your own accounts. These accounts do not exist
     and are only for demonstration purposes.
 
 To create an agent in a project you just need to: ::
 
-    from spade import agent, quit_spade
+    import spade
 
-    class DummyAgent(agent.Agent):
+    class DummyAgent(spade.agent.Agent):
         async def setup(self):
             print("Hello World! I'm agent {}".format(str(self.jid)))
 
-    dummy = DummyAgent("your_jid@your_xmpp_server", "your_password")
-    future = dummy.start()
-    future.result()
+    async def main():
+        dummy = DummyAgent("your_jid@your_xmpp_server", "your_password")
+        await dummy.start()
 
-    dummy.stop()
-    quit_spade()
+    if __name__ == "__main__":
+        spade.run(main())
 
 
 This agent is only printing on screen a message during its setup and stopping. If you run this script you get
 the following output::
 
     $ python dummyagent.py
     Hello World! I'm agent your_jid@your_xmpp_server
     $
 
 And that's it! We have built our first SPADE Agent in 6 lines of code. Easy, isn't it? Of course, this is a very very
 dumb agent that does nothing, but it serves well as a starting point to understand the logics behind SPADE.
 
-.. note:: Note how the ``start`` function returns a future (or promise) which you can wait for with the result method
-          (``future.result()``) to make sure that the ``start`` coroutine has finished before invoking the ``stop`` coroutine.
+.. note:: A SPADE agent is an asyncronous agent. That means that all the code to run an agent must be executed in an
+    asyncronous loop. This is done by the ``spade.run()`` function. This function receives a coroutine as a parameter
+    and runs it in an async loop. In our example, the ``main()`` coroutine is the one that is run in the loop.
 
 An agent with a behaviour
 -------------------------
 
 Let's build a more functional agent, one that uses an actual behaviour to perform a task. As we stated earlier, the real
 programming of the SPADE agents is done mostly in the behaviours. Let's see how.
 
@@ -59,16 +60,17 @@
 ``dummyagent.py`` script.
 
 .. warning:: Remember to change the example's jids and passwords by your own accounts. These accounts do not exist
     and are only for demonstration purposes.
 
 Example::
 
-    import time
     import asyncio
+    import spade
+    from spade import wait_until_finished
     from spade.agent import Agent
     from spade.behaviour import CyclicBehaviour
 
     class DummyAgent(Agent):
         class MyBehav(CyclicBehaviour):
             async def on_start(self):
                 print("Starting behaviour . . .")
@@ -80,26 +82,24 @@
                 await asyncio.sleep(1)
 
         async def setup(self):
             print("Agent starting . . .")
             b = self.MyBehav()
             self.add_behaviour(b)
 
-    if __name__ == "__main__":
+    async def main():
         dummy = DummyAgent("your_jid@your_xmpp_server", "your_password")
-        future = dummy.start()
-        future.result()
+        await dummy.start()
+        print("DummyAgent started. Check its console to see the output.")
 
         print("Wait until user interrupts with ctrl+C")
-        try:
-            while True:
-                time.sleep(1)
-        except KeyboardInterrupt:
-            print("Stopping...")
-        dummy.stop()
+        await wait_until_finished(dummy)
+
+    if __name__ == "__main__":
+        spade.run(main())
 
 
 As you can see, we have defined a custom behaviour called MyBehav that inherits from the spade.behaviour.CyclicBehaviour
 class, the default class for all behaviours. This class represents a cyclic behaviour with no specific period, that is,
 a loop-like behaviour.
 
 You can see that there is a coroutine called ``on_start()`` in the behaviour. This method is similar to the ``setup()``
@@ -122,14 +122,16 @@
 there is also a second optional parameter which is the template associated to that behaviour, but we will talk later
 about templates.
 
 Let's test our new agent::
 
     $ python dummyagent.py
     Agent starting . . .
+    DummyAgent started. Check its console to see the output.
+    Wait until user interrupts with ctrl+C
     Starting behaviour . . .
     Counter: 0
     Counter: 1
     Counter: 2
     Counter: 3
     Counter: 4
     Counter: 5
@@ -143,16 +145,16 @@
 ---------------------
 
 If you want to finish a behaviour you can kill it by using the ``self.kill(exit_code)`` method. This method **marks**
 the behaviour to be killed at the next loop iteration and stores the exit_code to be queried later.
 
 An example of how to kill a behaviour::
 
-    import time
     import asyncio
+    import spade
     from spade.agent import Agent
     from spade.behaviour import CyclicBehaviour
 
     class DummyAgent(Agent):
         class MyBehav(CyclicBehaviour):
             async def on_start(self):
                 print("Starting behaviour . . .")
@@ -170,26 +172,32 @@
                 print("Behaviour finished with exit code {}.".format(self.exit_code))
 
         async def setup(self):
             print("Agent starting . . .")
             self.my_behav = self.MyBehav()
             self.add_behaviour(self.my_behav)
 
-    if __name__ == "__main__":
+    async def main():
         dummy = DummyAgent("your_jid@your_xmpp_server", "your_password")
-        future = dummy.start()
-        future.result()  # Wait until the start method is finished
+        await dummy.start()
 
         # wait until user interrupts with ctrl+C
         while not dummy.my_behav.is_killed():
             try:
-                time.sleep(1)
+                await asyncio.sleep(1)
             except KeyboardInterrupt:
                 break
-        dummy.stop()
+
+        assert dummy.my_behav.exit_code == 10
+
+        await dummy.stop()
+
+
+    if __name__ == "__main__":
+            spade.run(main())
 
 
 And the output of this example would be::
 
     $ python killbehav.py
     Agent starting . . .
     Starting behaviour . . .
@@ -210,77 +218,50 @@
     If a exception occurs inside an ``on_start``, ``run`` or ``on_end`` coroutines, the behaviour will be
     automatically killed and the exception will be stored as its ``exit_code``.
 
 
 Finishing SPADE
 ---------------
 
-There is a helper to quickly finish all the agents and behaviors running in your process. This helper function is
-``quit_spade``::
-
-    from spade import quit_spade
-
-    from spade import agent
-
-    class DummyAgent(agent.Agent):
-        async def setup(self):
-            print("Hello World! I'm agent {}".format(str(self.jid)))
-
-    dummy = DummyAgent("your_jid@your_xmpp_server", "your_password")
-    future = dummy.start()
-    future.result()
-
-    dummy.stop()
-
-    quit_spade()
+A SPADE script will be running until all agents are stopped. If you want to stop all agents and finish the script you
+may send a SIGINT (ctrl+C) signal. This signal will stop all agents.
 
+.. warning:: The ``quit_spade()`` method has been deprecated since the current version of SPADE (3.3).
 
 
-.. hint::
-    The ``quit_spade`` helper is not mandatory, but it helps to terminate all agents of the active container along with
-    their behaviors, as well as free all pending resources (threads, etc...).
-
 Creating an agent from within another agent
 -------------------------------------------
 
 There is a common use case where you may need to create an agent from within another agent, that is, from within another
-agent's behaviour. This is a *special* case because you can't create a new event loop when you have a loop already
-running. For this special case you can use the ``start`` method as usual. But in this case ```start`` behaves as a
-coroutine, so it MUST be called with an ``await`` statement in order to work properly. Example::
+agent's behaviour. This is a common case where ```start`` must be called with an ``await`` statement in order to work properly. Example::
 
-    from spade import quit_spade
+    import spade
     from spade.agent import Agent
     from spade.behaviour import OneShotBehaviour
 
 
     class AgentExample(Agent):
         async def setup(self):
             print(f"{self.jid} created.")
 
 
     class CreateBehav(OneShotBehaviour):
         async def run(self):
             agent2 = AgentExample("agent2_example@your_xmpp_server", "fake_password")
-            # This start is inside an async def, so it must be awaited
             await agent2.start(auto_register=True)
 
-
-    if __name__ == "__main__":
+    async def main():
         agent1 = AgentExample("agent1_example@your_xmpp_server", "fake_password")
         behav = CreateBehav()
         agent1.add_behaviour(behav)
-        # This start is in a synchronous piece of code, so it must NOT be awaited
-        future = agent1.start(auto_register=True)
-        future.result()
+        await agent1.start(auto_register=True)
 
         # wait until the behaviour is finished to quit spade.
-        behav.join()
-        quit_spade()
+        await behav.join()
+
+    if __name__ == "__main__":
+        spade.run(main())
 
 
 
-.. warning:: Remember to call ``start`` with an ``await`` whenever you are inside an asyncronous method (another coroutine).
-             Otherwise, call ``start`` as usual (without the ``await`` statement).
 
 
-.. note:: The ``stop`` method behaves just like ``start``. They change depending on the context.
-          They return a coroutine or a future depending on whether they are called from a coroutine or a synchronous method.
```

### Comparing `spade-3.2.3/docs/web.rst` & `spade-3.3.0/docs/web.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 =======================
 Web Graphical Interface
 =======================
 
-Each agent in SPADE provides a graphical interface *by default* that is accesible via web under the ``/spade`` path.
+Each agent in SPADE provides a graphical interface *by default* that is accessible via web under the ``/spade`` path.
 To activate the web interface you just have to start the web module of the agent just as follows::
 
     agent = MyAgent("your_jid@your_xmpp_server", "your_password")
-    agent.start()
+    await agent.start()
     agent.web.start(hostname="127.0.0.1", port="10000")
 
 
 Then you can open a web browser and go to the url ``http://127.0.0.1:10000/spade`` and you'll see the
 main page of your agent:
 
 .. image:: images/spade_index.png
@@ -67,15 +67,15 @@
     async def hello_controller(request):
         return {"number": 42}
 
     a = Agent("your_jid@your_xmpp_server", "your_password")
 
     a.web.add_get("/hello", hello_controller, "hello.html")
 
-    a.start(auto_register=True)
+    await a.start(auto_register=True)
     a.web.start(port=10000)
 
 
 
 In this example there are some elements that must be explained:
 
     #. The ``hello_controller`` function is a coroutine (see the ``async`` statement) that returns a dictionary with data that will be rendered in the template.
@@ -84,17 +84,17 @@
 
 Next we are going to explain a little more about the controller, the path and the template.
 
 .. note:: Please, do not use the ``/spade`` path o avoid conflicts with the default agent pages (unless you want to modify them).
 
 Controller
 ----------
-The controller is the asyncronous method (or coroutine) that prepares the data to render the web page. It is an ``async``
+The controller is the asynchronous method (or coroutine) that prepares the data to render the web page. It is an ``async``
 method that always receives a single argument: ``request``. A controller queries the
-model, which in our case is the agent (accesible in your coroutines using ``self.agent``) and prepares a dictionary
+model, which in our case is the agent (accessible in your coroutines using ``self.agent``) and prepares a dictionary
 which will be used to render the template (as we will see in a moment). Inside a controller coroutine you can do
 any agent related stuff (sending messages, starting or killing behaviours, etc.).
 
 .. hint:: Just remember the trick that a coroutine should not be too intensive in cpu, to avoid blocking the execution of the agent.
 
 An example of controller would be::
```

### Comparing `spade-3.2.3/setup.py` & `spade-3.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # put setup requirements (distutils extensions, etc.) here
 ]
 
 test_requirements = parse_requirements("requirements_dev.txt")
 
 setup(
     name='spade',
-    version='3.2.3',
+    version='3.3.0',
     description="Smart Python Agent Development Environment",
     long_description=readme + '\n\n' + history,
     author="Javi Palanca",
     author_email='jpalanca@gmail.com',
     url='https://github.com/javipalanca/spade',
     packages=find_packages(include=['spade']),
     entry_points={
@@ -48,18 +48,17 @@
     keywords='spade',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Internet :: XMPP',
     ],
     test_suite='tests',
```

### Comparing `spade-3.2.3/spade/agent.py` & `spade-3.3.0/spade/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import asyncio
 import logging
 import sys
-from asyncio import Future
+from asyncio import Task
 from hashlib import md5
-from threading import Event
-from typing import Coroutine, Union, Optional, Type, Any, List
+from typing import Coroutine, Optional, Type, Any, List, TypeVar
 
 import aiosasl
 import aioxmpp
 import aioxmpp.ibr as ibr
 from aioxmpp.dispatcher import SimpleMessageDispatcher
 
-from .behaviour import FSMBehaviour, CyclicBehaviour
+from .behaviour import BehaviourType, FSMBehaviour, CyclicBehaviour
 from .container import Container
 from .message import Message
 from .presence import PresenceManager
 from .template import Template
 from .trace import TraceStore
 from .web import WebApp
 
 logger = logging.getLogger("spade.Agent")
 
+AgentType = TypeVar("AgentType", bound="Agent")
+
 
 class AuthenticationFailure(Exception):
     """ """
 
     pass
 
 
@@ -52,72 +53,69 @@
         self.presence = None
         self.loop = None
 
         self.container = Container()
         self.container.register(self)
 
         self.loop = self.container.loop
+        asyncio.set_event_loop(self.loop)
 
         # Web service
         self.web = WebApp(agent=self)
 
         self.traces = TraceStore(size=1000)
 
-        self._alive = Event()
+        self._alive = asyncio.Event()
 
     def set_loop(self, loop) -> None:
         self.loop = loop
 
     def set_container(self, container: Container) -> None:
         """
         Sets the container to which the agent is attached
 
         Args:
             container (spade.container.Container): the container to be attached to
         """
         self.container = container
 
-    def start(self, auto_register: bool = True) -> Union[Coroutine, Future]:
+    async def start(self, auto_register: bool = True) -> None:
         """
-        Tells the container to start this agent.
-        It returns a coroutine or a future depending on whether it is called from a coroutine or a synchronous method.
+        Starts this agent.
 
         Args:
             auto_register (bool): register the agent in the server (Default value = True)
 
         Returns:
-            Coroutine: if called from an async method
-            Future: if called from a synchronized method
+            None
         """
-        return self.container.start_agent(agent=self, auto_register=auto_register)
+        return await self._async_start(auto_register=auto_register)
 
     async def _async_start(self, auto_register: bool = True) -> None:
         """
         Starts the agent from a coroutine. This fires some actions:
 
             * if auto_register: register the agent in the server
             * runs the event loop
             * connects the agent to the server
             * runs the registered behaviours
 
         Args:
           auto_register (bool, optional): register the agent in the server (Default value = True)
 
         """
-
         await self._hook_plugin_before_connection()
 
         if auto_register:
             await self._async_register()
         self.client = aioxmpp.PresenceManagedClient(
             self.jid,
             aioxmpp.make_security_layer(
                 self.password, no_verify=not self.verify_security
             ),
-            loop=self.loop,
             logger=logging.getLogger(self.jid.localpart),
         )
 
         # obtain an instance of the service
         self.message_dispatcher = self.client.summon(SimpleMessageDispatcher)
 
         # Presence service
@@ -153,32 +151,30 @@
     async def _hook_plugin_after_connection(self) -> None:
         """
         Overload this method to hook a plugin after connetion is done
         """
         pass
 
     async def _async_connect(self) -> None:  # pragma: no cover
-        """ connect and authenticate to the XMPP server. Async mode. """
+        """connect and authenticate to the XMPP server. Async mode."""
         try:
             self.conn_coro = self.client.connected()
             aenter = type(self.conn_coro).__aenter__(self.conn_coro)
             self.stream = await aenter
             logger.info(f"Agent {str(self.jid)} connected and authenticated.")
         except aiosasl.AuthenticationFailure:
             raise AuthenticationFailure(
                 "Could not authenticate the agent. Check user and password or use auto_register=True"
             )
 
     async def _async_register(self) -> None:  # pragma: no cover
-        """ Register the agent in the XMPP server from a coroutine. """
+        """Register the agent in the XMPP server from a coroutine."""
         metadata = aioxmpp.make_security_layer(None, no_verify=not self.verify_security)
         query = ibr.Query(self.jid.localpart, self.password)
-        _, stream, features = await aioxmpp.node.connect_xmlstream(
-            self.jid, metadata, loop=self.loop
-        )
+        _, stream, features = await aioxmpp.node.connect_xmlstream(self.jid, metadata)
         await ibr.register(stream, query)
 
     async def setup(self) -> None:
         """
         Setup agent before startup.
         This coroutine may be overloaded.
         """
@@ -217,30 +213,30 @@
         Returns:
           str: an URL for the gravatar
 
         """
         digest = md5(str(jid).encode("utf-8")).hexdigest()
         return "http://www.gravatar.com/avatar/{md5}?d=monsterid".format(md5=digest)
 
-    def submit(self, coro: Coroutine) -> Future:
+    def submit(self, coro: Coroutine) -> Task:
         """
         Runs a coroutine in the event loop of the agent.
         this call is not blocking.
 
         Args:
           coro (Coroutine): the coroutine to be run
 
         Returns:
-            asyncio.Future: the future of the coroutine execution
+            asyncio.Task: the Task assigned to the coroutine execution
 
         """
-        return asyncio.run_coroutine_threadsafe(coro, loop=self.loop)
+        return asyncio.create_task(coro)
 
     def add_behaviour(
-        self, behaviour: Type[CyclicBehaviour], template: Optional[Template] = None
+        self, behaviour: BehaviourType, template: Optional[Template] = None
     ) -> None:
         """
         Adds and starts a behaviour to the agent.
         If template is not None it is used to match
         new messages and deliver them to the behaviour.
 
         Args:
@@ -281,31 +277,29 @@
 
         Returns:
           bool: a boolean that indicates wether the behaviour is inside the agent.
 
         """
         return behaviour in self.behaviours
 
-    def stop(self) -> Union[Coroutine, Future]:
+    async def stop(self) -> None:
         """
-        Tells the container to start this agent.
-        It returns a coroutine or a future depending on whether it is called from a coroutine or a synchronous method.
+        Stops this agent.
         """
-        return self.container.stop_agent(self)
+        return await self._async_stop()
 
     async def _async_stop(self) -> None:
-        """ Stops an agent and kills all its behaviours. """
+        """Stops an agent and kills all its behaviours."""
         if self.presence:
             self.presence.set_unavailable()
         for behav in self.behaviours:
             behav.kill()
         if self.web.is_started():
             await self.web.runner.cleanup()
 
-        """ Discconnect from XMPP server. """
         if self.is_alive():
             # Disconnect from XMPP server
             self.client.stop()
             aexit = self.conn_coro.__aexit__(*sys.exc_info())
             await aexit
             logger.info("Client disconnected.")
 
@@ -344,15 +338,15 @@
 
         """
         if name in self._values:
             return self._values[name]
         else:
             return None
 
-    def _message_received(self, msg: aioxmpp.Message) -> List[Future]:
+    def _message_received(self, msg: aioxmpp.Message) -> List[Task]:
         """
         Callback run when an XMPP Message is reveived.
         This callback delivers the message to every behaviour
         that is waiting for it. First, the aioxmpp.Message is
         converted to spade.message.Message
 
         Args:
@@ -362,31 +356,31 @@
             list(asyncio.Future): a list of futures of the append of the message at each matched behaviour.
 
         """
 
         msg = Message.from_node(msg)
         return self.dispatch(msg)
 
-    def dispatch(self, msg: Message) -> List[Future]:
+    def dispatch(self, msg: Message) -> List[Task]:
         """
         Dispatch the message to every behaviour that is waiting for
         it using their templates match.
 
         Args:
-          msg (spade.message.Messagge): the message to dispatch.
+          msg (spade.message.Message): the message to dispatch.
 
         Returns:
-            list(asyncio.Future): a list of futures of the append of the message at each matched behaviour.
+            list(asyncio.Future): a list of tasks for each message queuing in each matching behavior.
 
         """
         logger.debug(f"Got message: {msg}")
-        futures = []
+        tasks = []
         matched = False
         for behaviour in (x for x in self.behaviours if x.match(msg)):
-            futures.append(self.submit(behaviour.enqueue(msg)))
+            tasks.append(self.submit(behaviour.enqueue(msg)))
             logger.debug(f"Message enqueued to behaviour: {behaviour}")
             self.traces.append(msg, category=str(behaviour))
             matched = True
         if not matched:
             logger.warning(f"No behaviour matched for message: {msg}")
             self.traces.append(msg)
-        return futures
+        return tasks
```

### Comparing `spade-3.2.3/spade/behaviour.py` & `spade-3.3.0/spade/behaviour.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 import logging
 import time
 import traceback
 from abc import ABCMeta, abstractmethod
 from asyncio import CancelledError
 from datetime import timedelta, datetime
 from threading import Event
-from typing import Any, Optional, Coroutine, Dict
+from typing import Any, Optional, Dict, TypeVar
 
 from .message import Message
 from .template import Template
 
 now = datetime.now
 
 logger = logging.getLogger("spade.behaviour")
 
+BehaviourType = TypeVar("BehaviourType", bound="CyclicBehaviour")
+
 
 class BehaviourNotFinishedException(Exception):
     """ """
 
     pass
 
 
@@ -32,22 +34,21 @@
 class NotValidTransition(Exception):
     """ """
 
     pass
 
 
 class CyclicBehaviour(object, metaclass=ABCMeta):
-    """ This behaviour is executed cyclically until it is stopped. """
+    """This behaviour is executed cyclically until it is stopped."""
 
     def __init__(self):
         self.agent = None
         self.template = None
         self._force_kill = Event()
-        self._is_done = asyncio.Event()
-        self._is_done.set()
+        self._is_done = None
         self._exit_code = 0
         self.presence = None
         self.web = None
         self.is_running = False
 
         self.queue = None
 
@@ -56,15 +57,18 @@
         Links behaviour with its owner agent
 
         Args:
           agent (spade.agent.Agent): the agent who owns the behaviour
 
         """
         self.agent = agent
-        self.queue = asyncio.Queue(loop=self.agent.loop)
+        asyncio.set_event_loop(self.agent.loop)
+        self._is_done = asyncio.Event()
+        self._is_done.set()
+        self.queue = asyncio.Queue()
         self.presence = agent.presence
         self.web = agent.web
 
     def set_template(self, template: Template) -> None:
         """
         Sets the template that is used to match incoming
         messages with this behaviour.
@@ -121,15 +125,15 @@
 
     async def _start(self) -> None:
         """
         Start coroutine. runs on_start coroutine and then
         runs the _step coroutine where the body of the behaviour
         is called.
         """
-        self.agent._alive.wait()
+        await self.agent._alive.wait()
         try:
             await self.on_start()
         except Exception as e:
             logger.error(
                 "Exception running on_start in behaviour {}: {}".format(self, e)
             )
             self.kill(exit_code=e)
@@ -205,43 +209,29 @@
         Check if the behaviour is finished
 
         Returns:
              bool: whether the behaviour is finished or not
         """
         return not self._is_done.is_set()
 
-    def join(self, timeout: Optional[float] = None) -> Optional[Coroutine]:
+    async def join(self, timeout: Optional[float] = None) -> None:
         """
         Wait for the behaviour to complete
 
         Args:
             timeout (Optional[float]): an optional timeout to wait to join (if None, the join is blocking)
 
         Returns:
-            None: if called from a synchronous method
-            Coroutine: if called from an async method
+            None
 
         Raises:
             TimeoutError: if the timeout is reached
         """
 
-        try:
-            in_coroutine = asyncio.get_event_loop() == self.agent.loop
-        except RuntimeError:  # pragma: no cover
-            in_coroutine = False
-
-        if not in_coroutine:
-            t_start = time.time()
-            while not self.is_done():
-                time.sleep(0.001)
-                t = time.time()
-                if timeout is not None and t - t_start > timeout:
-                    raise TimeoutError
-        else:
-            return self._async_join(timeout=timeout)
+        return await self._async_join(timeout=timeout)
 
     async def _async_join(self, timeout: Optional[float]) -> None:
         """
         Coroutine to wait until a behaviour is finished
 
         Args:
             timeout (Optional[float]): an optional timeout to wait to join
@@ -290,16 +280,16 @@
         ortherwise it calls run() coroutine.
         """
         cancelled = False
         while not self._done() and not self.is_killed():
             try:
                 await self._run()
                 await asyncio.sleep(0)  # relinquish cpu
-            except CancelledError:
-                logger.info("Behaviour {} cancelled".format(self))
+            except CancelledError:  # pragma: no cover
+                logger.debug("Behaviour {} cancelled".format(self))
                 cancelled = True
             except Exception as e:
                 logger.error(
                     "Exception running behaviour {behav}: {exc}".format(
                         behav=self, exc=e
                     )
                 )
@@ -307,24 +297,25 @@
                 self.kill(exit_code=e)
         try:
             if not cancelled:
                 await self.on_end()
         except Exception as e:
             logger.error("Exception running on_end in behaviour {}: {}".format(self, e))
             self.kill(exit_code=e)
+        self.is_running = False
         self.agent.remove_behaviour(self)
 
     async def enqueue(self, message: Message) -> None:
         """
         Enqueues a message in the behaviour's mailbox
 
         Args:
             message (spade.message.Message): the message to be enqueued
         """
-        await self.queue.put(message)
+        asyncio.create_task(self.queue.put(message))
 
     def mailbox_size(self) -> int:
         """
         Checks if there is a message in the mailbox
 
         Returns:
           int: the number of messages in the mailbox
@@ -415,15 +406,15 @@
         if start_at:
             self._next_activation = start_at
         else:
             self._next_activation = now()
 
     @property
     def period(self) -> timedelta:
-        """ Get the period. """
+        """Get the period."""
         return self._period
 
     @period.setter
     def period(self, value: float) -> None:
         """
         Set the period.
```

### Comparing `spade-3.2.3/spade/container.py` & `spade-3.3.0/spade/container.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,57 @@
 import asyncio
 import logging
 import sys
-from asyncio import Future
 from contextlib import suppress
-from threading import Thread
-from typing import Type, Union, Coroutine
+from typing import Coroutine, Awaitable
 
 from singletonify import singleton
 
-from .behaviour import CyclicBehaviour
+from .behaviour import BehaviourType
 from .message import Message
 
 logger = logging.getLogger("SPADE")
 
 # check if python is 3.6 or higher
 if sys.version_info >= (3, 7) and sys.platform == "win32":
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+    asyncio.set_event_loop_policy(
+        asyncio.WindowsSelectorEventLoopPolicy()
+    )  # pragma: no cover
+
+
+def get_or_create_eventloop():  # pragma: no cover
+    if sys.version_info < (3, 10):
+        loop = asyncio.get_event_loop()
+    else:
+        try:
+            loop = asyncio.get_running_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+
+    asyncio.set_event_loop(loop)
+    return loop
 
 
 @singleton()
 class Container(object):
     """
     The container class allows agents to exchange messages
     without using the XMPP socket if they are in the same
     process.
     The container is a singleton.
     """
 
     def __init__(self):
         self.__agents = {}
-        self.aiothread = AioThread()
-        self.aiothread.start()
-        self.loop = self.aiothread.loop
-        self.loop.set_debug(False)
+        self.loop = get_or_create_eventloop()
         self.is_running = True
 
-    def __in_coroutine(self) -> bool:
-        try:
-            return asyncio.get_event_loop() == self.loop
-        except RuntimeError:  # pragma: no cover
-            return False
-
-    def start_agent(
-            self, agent, auto_register: bool = True
-    ) -> Union[Coroutine, Future]:
-        coro = agent._async_start(auto_register=auto_register)
-
-        if self.__in_coroutine():
-            return coro
-        else:
-            future = asyncio.run_coroutine_threadsafe(coro, loop=self.loop)
-            future.wait = future.result
-            return future
-
-    def stop_agent(self, agent) -> Union[Coroutine, Future]:
-        coro = agent._async_stop()
-
-        if self.__in_coroutine():
-            return coro
-        else:
-            future = asyncio.run_coroutine_threadsafe(coro, loop=self.loop)
-            future.wait = future.result
-            return future
-
     def reset(self) -> None:
-        """ Empty the container by unregistering all the agents. """
-        self.__agents = {}
+        """Empty the container by unregistering all the agents."""
+        self.__init__()
 
     def register(self, agent) -> None:
         """
         Register a new agent.
 
         Args:
             agent (spade.agent.Agent): the agent to be registered
@@ -103,64 +85,46 @@
             spade.agent.Agent: the agent you were looking for
 
         Raises:
             KeyError: if the agent is not found
         """
         return self.__agents[jid]
 
-    async def send(self, msg: Message, behaviour: Type[CyclicBehaviour]) -> None:
+    async def send(self, msg: Message, behaviour: BehaviourType) -> None:
         """
         This method sends the message using the container mechanism
         when the receiver is also registered in the container. Otherwise,
         it uses the XMPP send method from the original behaviour.
         Args:
             msg (spade.message.Message): the message to be sent
             behaviour: the behaviour that is sending the message
         """
         to = str(msg.to)
         if to in self.__agents:
             self.__agents[to].dispatch(msg)
         else:
-            await behaviour._xmpp_send(msg)
+            await behaviour._xmpp_send(msg=msg)
 
-    def stop(self) -> None:
-        agents = [agent.stop() for agent in self.__agents.values() if agent.is_alive()]
-        if self.__in_coroutine():
-            coro = asyncio.gather(*agents)
-            asyncio.run_coroutine_threadsafe(coro, loop=self.loop)
-        self.aiothread.finalize()
-        self.reset()
-        self.is_running = False
-
-
-class AioThread(Thread):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.loop = asyncio.new_event_loop()
-        self.running = True
-        self.daemon = True
-
-    def run(self) -> None:
-        try:
-            self.loop.run_forever()
-            if sys.version_info >= (3, 7):
-                tasks = asyncio.all_tasks(loop=self.loop)  # pragma: no cover
-            else:
-                tasks = asyncio.Task.all_tasks(loop=self.loop)  # pragma: no cover
-            for task in tasks:
-                task.cancel()
-                with suppress(asyncio.CancelledError):
-                    self.loop.run_until_complete(task)
-            self.loop.close()
-            logger.debug("Loop closed")
-        except Exception as e:  # pragma: no cover
-            logger.error("Exception in the event loop: {}".format(e))
-
-    def finalize(self) -> None:
-        if self.running:
-            self.loop.call_soon_threadsafe(self.loop.stop)
-            self.running = False
+    def run(self, coro: Awaitable) -> None:  # pragma: no cover
+        self.loop.run_until_complete(coro)
 
 
-def stop_container() -> None:
+def run_container(main_func: Coroutine) -> None:  # pragma: no cover
     container = Container()
-    container.stop()
+    try:
+        container.run(main_func)
+    except KeyboardInterrupt:
+        logger.warning("Keyboard interrupt received. Stopping SPADE...")
+    except Exception as e:  # pragma: no cover
+        logger.error("Exception in the event loop: {}".format(e))
+
+    if sys.version_info >= (3, 7):  # pragma: no cover
+        tasks = asyncio.all_tasks(loop=container.loop)  # pragma: no cover
+    else:
+        tasks = asyncio.Task.all_tasks(loop=container.loop)  # pragma: no cover
+    for task in tasks:
+        task.cancel()
+        with suppress(asyncio.CancelledError):
+            container.run(task)
+
+    container.loop.close()
+    logger.debug("Loop closed")
```

### Comparing `spade-3.2.3/spade/message.py` & `spade-3.3.0/spade/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         else:
             for key, value in metadata.items():
                 if not isinstance(key, str) or not isinstance(value, str):
                     raise TypeError("Key and Value of metadata MUST be strings")
             self.metadata = metadata
 
     @classmethod
-    def from_node(cls, node: aioxmpp.Message) -> Type['MessageBase']:
+    def from_node(cls, node: aioxmpp.Message) -> Type["MessageBase"]:
         """
         Creates a new spade.message.Message from an aixoxmpp.stanza.Message
 
         Args:
           node (aioxmpp.stanza.Message): an aioxmpp Message
 
         Returns:
@@ -182,15 +182,15 @@
 
         Returns:
           str: the value of the metadata (or None)
 
         """
         return self.metadata[key] if key in self.metadata else None
 
-    def match(self, message: Type['MessageBase']) -> bool:
+    def match(self, message: Type["MessageBase"]) -> bool:
         """
         Returns wether a message matches with this message or not.
         The message can be a Message object or a Template object.
 
         Args:
           message (spade.message.Message): the message to match to
 
@@ -218,22 +218,22 @@
         return True
 
     @property
     def id(self) -> int:
         """ """
         return id(self)
 
-    def __eq__(self, other: Type['MessageBase']):
+    def __eq__(self, other: Type["MessageBase"]):
         return self.match(other)
 
 
 class Message(MessageBase):
     """ """
 
-    def make_reply(self) -> 'Message':
+    def make_reply(self) -> "Message":
         """
         Creates a copy of the message, exchanging sender and receiver
 
         Returns:
           spade.message.Message: a new message with exchanged sender and receiver
 
         """
```

### Comparing `spade-3.2.3/spade/presence.py` & `spade-3.3.0/spade/presence.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/template.py` & `spade-3.3.0/spade/template.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/templates/internal_tpl_agent.html` & `spade-3.3.0/spade/templates/internal_tpl_agent.html`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/templates/internal_tpl_base.html` & `spade-3.3.0/spade/templates/internal_tpl_base.html`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         {% endblock %}
         <!-- /.content -->
     </div>
     <!-- /.content-wrapper -->
 
     <footer class="main-footer">
         <div class="pull-right hidden-xs">
-            <b>Version</b> 3.0.9
+            <b>Version</b> 3.3.0
         </div>
         <strong>Copyright © {% now 'local', '%Y' %} <a href="http://github.com/javipalanca/spade">SPADE</a>.</strong>
     </footer>
 
 
 </div>
 <!-- ./wrapper -->
```

#### html2text {}

```diff
@@ -54,9 +54,9 @@
     * [User Image] Alexander 13 Jan
     * [User Image] Sarah 14 Jan
     * [User Image] Nora 15 Jan
     * [User Image] Nadia 15 Jan
 View_All_Users
   {% endblock %}
 
-Version 3.0.9
+Version 3.3.0
 Copyright Â© {% now 'local', '%Y' %} SPADE.
```

### Comparing `spade-3.2.3/spade/templates/internal_tpl_behaviour.html` & `spade-3.3.0/spade/templates/internal_tpl_behaviour.html`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/templates/internal_tpl_index.html` & `spade-3.3.0/spade/templates/internal_tpl_index.html`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/templates/internal_tpl_macros.html` & `spade-3.3.0/spade/templates/internal_tpl_macros.html`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/templates/internal_tpl_messages.html` & `spade-3.3.0/spade/templates/internal_tpl_messages.html`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/trace.py` & `spade-3.3.0/spade/trace.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/spade/web.py` & `spade-3.3.0/spade/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 def unused_port(hostname: str) -> None:
     """Return a port that is unused on the current host."""
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind((hostname, 0))
         return s.getsockname()[1]
 
 
-async def start_server_in_loop(
-    runner: AppRunner, hostname: str, port: int, agent
-):
+async def start_server_in_loop(runner: AppRunner, hostname: str, port: int, agent):
     """
     Listens to http requests and sends them to the webapp.
 
     Args:
         runner (AppRunner): AppRunner to process the http requests
         hostname (str): host name to listen from.
         port (int): port to listen from.
@@ -38,15 +36,15 @@
     await runner.setup()
     agent.web.server = aioweb.TCPSite(runner, hostname, port)
     await agent.web.server.start()
     logger.info(f"Serving on http://{hostname}:{port}/")
 
 
 class WebApp(object):
-    """ Module to handle agent's web interface """
+    """Module to handle agent's web interface"""
 
     def __init__(self, agent):
         self.agent = agent
         self.server = None
         self.hostname = None
         self.port = None
         self.runner = None
@@ -59,15 +57,15 @@
         self._set_loaders()
 
     def start(
         self,
         hostname: Optional[str] = None,
         port: Optional[int] = None,
         templates_path: Optional[str] = None,
-    ) -> None:
+    ):
         """
         Starts the web interface.
 
         Args:
           hostname (str, optional): host name to listen from. (Default value = None)
           port (int, optional): port to listen from. (Default value = None)
           templates_path (str, optional): path to look for templates. (Default value = None)
```

### Comparing `spade-3.2.3/spade.egg-info/PKG-INFO` & `spade-3.3.0/spade.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spade
-Version: 3.2.3
+Version: 3.3.0
 Summary: Smart Python Agent Development Environment
 Home-page: https://github.com/javipalanca/spade
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
 Keywords: spade
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Internet :: XMPP
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -43,15 +43,15 @@
     :alt: Languages
     :target: https://pepy.tech/project/spade
 
 .. image:: https://img.shields.io/github/languages/code-size/javipalanca/spade
     :alt: Code Size
     :target: https://pepy.tech/project/spade
 
-.. image:: https://img.shields.io/apm/l/atomic-design-ui.svg?
+.. image:: https://img.shields.io/pypi/l/spade
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 .. image:: https://pepy.tech/badge/spade
     :target: https://pepy.tech/project/spade
     :alt: Downloads
 
@@ -85,15 +85,15 @@
 
 
 Features
 --------
 
 * Multi-agent platform based on XMPP_
 * Presence notification allows the system to know the current state of the agents in real-time
-* Python >=3.6
+* Python >=3.8
 * Asyncio-based
 * Agent model based on behaviours
 * Supports FIPA metadata using XMPP Data Forms (XEP-0004_: Data Forms)
 * Web-based interface
 * Use any XMPP server
 
 Plugins
@@ -123,15 +123,23 @@
 
 
 
 =======
 History
 =======
 
-3.2.3 (2023-12-13)
+3.3.0 (2023-06-13)
+------------------
+
+* Updated to Python>=3.8
+* Changed the way agents are launched (now with `spade.run()`)
+* Python 3.11 still not supported due to a bug in `aiohttp`
+* Deprecated support for Python<=3.7
+
+3.2.3 (2022-12-13)
 ------------------
 
 * Updated third-party libs
 
 3.2.2 (2021-11-25)
 ------------------
 
@@ -281,7 +289,9 @@
 * Minor doc fixings and improvements.
 
 
 3.0.0 (2017-10-06)
 ------------------
 
 * Started writing 3.0 version.
+
+
```

### Comparing `spade-3.2.3/tests/conftest.py` & `spade-3.3.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import time
+import asyncio
 
 import pytest
 from aioxmpp import JID
 
-from spade import quit_spade
 from spade.container import Container
 from spade.message import Message
 
 
 @pytest.fixture
 def jid():
     return JID.fromstr("friend@localhost/home")
@@ -39,22 +38,21 @@
     # Code that will run before your test, for example:
     # A test function will be run at this point
     container = Container()
     if not container.is_running:
         container.__init__()
     yield
     # Code that will run after your test, for example:
-    quit_spade()
 
 
 @pytest.fixture(scope="module", autouse=True)
 def cleanup(request):
-    quit_spade()
+    pass
 
 
-def wait_for_behaviour_is_killed(behaviour, tries=500, sleep=0.01):
+async def wait_for_behaviour_is_killed(behaviour, tries=500, sleep=0.01):
     counter = 0
     while not behaviour.is_killed() and counter < tries:
-        time.sleep(sleep)
+        await asyncio.sleep(sleep)
         counter += 1
     if not behaviour.is_killed():
         raise Exception("Behaviour not finished")
```

### Comparing `spade-3.2.3/tests/factories.py` & `spade-3.3.0/tests/factories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import factory
 from aioxmpp import PresenceShow, PresenceState
-from asynctest import CoroutineMock, Mock
+from unittest.mock import AsyncMock, Mock
 
 from spade.agent import Agent
 
 
 class MockedConnectedAgent(Agent):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._async_connect = CoroutineMock()
-        self._async_register = CoroutineMock()
+        self._async_connect = AsyncMock()
+        self._async_register = AsyncMock()
         self.conn_coro = Mock()
-        self.conn_coro.__aexit__ = CoroutineMock()
+        self.conn_coro.__aexit__ = AsyncMock()
         self.stream = Mock()
 
 
 class MockedAgentFactory(factory.Factory):
     class Meta:
         model = MockedConnectedAgent
 
@@ -26,17 +26,17 @@
 class MockedPresenceConnectedAgent(Agent):
     def __init__(
         self, available=None, show=None, status=None, priority=0, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
         if status is None:
             status = {}
-        self._async_connect = CoroutineMock()
+        self._async_connect = AsyncMock()
         self.conn_coro = Mock()
-        self.conn_coro.__aexit__ = CoroutineMock()
+        self.conn_coro.__aexit__ = AsyncMock()
 
         self.available = available
         self.show = show
         self.status = status
         self.priority = priority
 
     def mock_presence(self):
```

### Comparing `spade-3.2.3/tests/test_agent.py` & `spade-3.3.0/tests/test_agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,112 @@
 import asyncio
 
 import aioxmpp
 from aioxmpp import PresenceManagedClient
-from asynctest import CoroutineMock, Mock
 from testfixtures import LogCapture
+from unittest.mock import AsyncMock, Mock
 
 from spade.agent import Agent
 from spade.behaviour import OneShotBehaviour
 from spade.message import Message
 from spade.template import Template
 from .factories import MockedAgentFactory
 
 
-def test_create_agent(mocker):
-    agent = Agent("jid@server", "fake_password")
-    agent._async_connect = CoroutineMock()
+async def test_create_agent(mocker):
+    agent = MockedAgentFactory()
 
     assert agent.is_alive() is False
 
-    future = agent.start(auto_register=False)
-    assert future.result() is None
+    await agent.start(auto_register=False)
 
     agent._async_connect.assert_called_once()
-    assert agent.stream is None
-
-    agent.conn_coro = mocker.Mock()
-    agent.conn_coro.__aexit__ = CoroutineMock()
 
-    assert agent.is_alive() is True
-    future = agent.stop()
-    future.result()
+    await agent.stop()
 
     agent.conn_coro.__aexit__.assert_called_once()
 
     assert agent.is_alive() is False
 
 
-def test_connected_agent():
-    agent = MockedAgentFactory()
-    assert agent.is_alive() is False
-
-    future = agent.start(auto_register=False)
-    assert future.result() is None
-    assert agent.is_alive() is True
-
-    future = agent.stop()
-    future.result()
-    assert agent.is_alive() is False
-
-
 def test_name():
     agent = MockedAgentFactory(jid="john@fake_server")
     assert agent.name == "john"
 
 
 def test_avatar():
     agent = MockedAgentFactory(jid="test_avatar@fake_server")
     assert (
         agent.avatar
         == "http://www.gravatar.com/avatar/44bdc5585ef57844edb11c5b9711d2e6?d=monsterid"
     )
 
 
-def test_setup():
+async def test_setup():
     agent = MockedAgentFactory()
-    agent.setup = CoroutineMock()
-    future = agent.start(auto_register=False)
-    assert future.result() is None
+    agent.setup = AsyncMock()
+
+    await agent.start()
 
     agent.setup.assert_called_once()
-    agent.stop()
+
+    await agent.stop()
 
 
 def test_set_get():
     agent = MockedAgentFactory()
     agent.set("KB_name", "KB_value")
     assert agent.get("KB_name") == "KB_value"
 
 
 def test_get_none():
     agent = MockedAgentFactory()
     assert agent.get("KB_name_unknown") is None
 
 
-def test_client():
+async def test_client():
     agent = MockedAgentFactory()
     assert agent.client is None
 
-    future = agent.start()
-    future.result()
+    await agent.start(auto_register=False)
+
     assert type(agent.client) == PresenceManagedClient
 
+    await agent.stop()
+
 
-def test_register():
+async def test_register():
     agent = MockedAgentFactory()
     agent.register = Mock()
 
-    future = agent.start(auto_register=True)
-    assert future.result() is None
+    await agent.start()
 
     assert len(agent._async_register.mock_calls) == 1
 
-    agent.stop()
+    await agent.stop()
 
 
 def test_receive_without_behaviours():
     agent = MockedAgentFactory()
     aiomsg = aioxmpp.Message(type_=aioxmpp.MessageType.CHAT)
     msg = Message.from_node(aiomsg)
 
     assert agent.traces.len() == 0
-    future = agent.start(auto_register=False)
-    assert future.result() is None
 
     with LogCapture() as log:
         agent._message_received(aiomsg)
         log.check_present(
             ("spade.Agent", "WARNING", f"No behaviour matched for message: {msg}")
         )
 
     assert agent.traces.len() == 1
     assert msg in agent.traces.store[0]
 
-    agent.stop()
 
-
-def test_create_agent_from_another_agent():
+async def test_create_agent_from_another_agent():
     class DummyBehav(OneShotBehaviour):
         async def run(self):
             self.agent._done = True
             self.kill()
 
     class CreateBehav(OneShotBehaviour):
         async def run(self):
@@ -140,88 +117,82 @@
             await self.agent.agent2.start(auto_register=False)
             self.kill()
 
     agent1 = MockedAgentFactory()
     agent1.agent2 = None
     create_behav = CreateBehav()
     agent1.add_behaviour(create_behav)
-    future = agent1.start(auto_register=False)
-    assert future.result() is None
-    assert agent1.is_alive()
 
-    create_behav.join()
-    agent1.dummy_behav.join()
+    await agent1.start(auto_register=False)
+
+    await create_behav.join()
 
-    assert agent1.agent2.is_alive()
     assert agent1.agent2._done
 
-    agent1.agent2.stop()
-    agent1.stop()
+    await agent1.stop()
 
 
-def test_create_agent_from_another_agent_from_setup():
+async def test_create_agent_from_another_agent_from_setup():
     class DummyBehav(OneShotBehaviour):
         async def run(self):
             self.agent._done = True
             self.kill()
 
     class SetupAgent(Agent):
         async def setup(self):
             self.agent2 = MockedAgentFactory()
             self.agent2._done = False
             self.agent2.dummy_behav = DummyBehav()
             self.agent2.add_behaviour(self.agent2.dummy_behav)
             await self.agent2.start(auto_register=False)
 
     agent1 = SetupAgent("fake@host", "secret")
-    agent1._async_connect = CoroutineMock()
-    agent1._async_register = CoroutineMock()
+    agent1._async_connect = AsyncMock()
+    agent1._async_register = AsyncMock()
     agent1.conn_coro = Mock()
-    agent1.conn_coro.__aexit__ = CoroutineMock()
+    agent1.conn_coro.__aexit__ = AsyncMock()
     agent1.stream = Mock()
 
     agent1.agent2 = None
 
-    future = agent1.start(auto_register=False)
-    assert future.result() is None
+    await agent1.start(auto_register=False)
     assert agent1.is_alive()
 
-    agent1.agent2.dummy_behav.join()
+    await agent1.agent2.dummy_behav.join()
 
     assert agent1.agent2.is_alive()
     assert agent1.agent2._done
 
-    agent1.agent2.stop()
-    agent1.stop()
+    await agent1.agent2.stop()
+    await agent1.stop()
 
 
-def test_submit_send():
+async def test_submit_send():
     agent = MockedAgentFactory()
 
     class DummyBehav(OneShotBehaviour):
         async def run(self):
             self.agent.recv_msg = await self.receive(10)
 
     template = Template(to="fake@jid")
     behav = DummyBehav()
     agent.add_behaviour(behav, template=template)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     msg_to_send = Message(to="fake@jid", body="BODY", metadata={"performative": "TEST"})
     agent.submit(behav.send(msg_to_send))
-    behav.join()
+    await behav.join()
 
     assert str(agent.recv_msg.to) == "fake@jid"
     assert agent.recv_msg.body == "BODY"
     assert agent.recv_msg.metadata == {"performative": "TEST"}
 
 
-def test_stop_agent_with_blocking_await():
+async def test_stop_agent_with_blocking_await():
     agent1 = MockedAgentFactory()
     agent1.value = 1000
 
     class StopBehav(OneShotBehaviour):
         async def run(self):
             await asyncio.sleep(0.5)
             await self.agent.stop()
@@ -233,14 +204,13 @@
 
     stopbehah = StopBehav()
     dummybehav = DummyBehav()
 
     agent1.add_behaviour(dummybehav)
     agent1.add_behaviour(stopbehah)
 
-    future1 = agent1.start(auto_register=False)
-    future1.result()
+    await agent1.start(auto_register=False)
 
-    stopbehah.join()
+    await stopbehah.join()
 
     assert not agent1.is_alive()
     assert agent1.value == 1000
```

### Comparing `spade-3.2.3/tests/test_behaviour.py` & `spade-3.3.0/tests/test_behaviour.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import datetime
-from threading import Event
+from unittest.mock import AsyncMock, Mock, MagicMock
 
 import aioxmpp
 import pytest
-from asynctest import CoroutineMock, MagicMock, Mock
 
 from spade.agent import Agent
 from spade.behaviour import (
     OneShotBehaviour,
     CyclicBehaviour,
     PeriodicBehaviour,
     TimeoutBehaviour,
@@ -65,15 +64,15 @@
     fsm_.state_one = state_one
     fsm_.state_two = state_two
     fsm_.state_three = state_three
 
     return fsm_
 
 
-def test_on_start_on_end():
+async def test_on_start_on_end():
     class TestOneShotBehaviour(OneShotBehaviour):
         async def on_start(self):
             self.agent.on_start_flag = True
 
         async def run(self):
             pass
 
@@ -86,113 +85,112 @@
     agent.on_end_flag = False
     behaviour = TestOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
     assert agent.on_start_flag is False
     assert agent.on_end_flag is False
 
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.on_start_flag is True
     assert agent.on_end_flag is True
-    agent.stop()
+    await agent.stop()
 
 
-def test_on_start_exception():
+async def test_on_start_exception():
     class TestOneShotBehaviour(OneShotBehaviour):
         async def on_start(self):
             result = 1 / 0
             self.agent.flag = True
 
         async def run(self):
             pass
 
     agent = MockedAgentFactory()
     agent.flag = False
     behaviour = TestOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert type(behaviour.exit_code) == ZeroDivisionError
     assert not agent.flag
-    agent.stop()
+    await agent.stop()
 
 
-def test_on_run_exception():
+async def test_on_run_exception():
     class TestOneShotBehaviour(OneShotBehaviour):
         async def run(self):
             result = 1 / 0
             self.agent.flag = True
 
     agent = MockedAgentFactory()
     agent.flag = False
     behaviour = TestOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert type(behaviour.exit_code) == ZeroDivisionError
     assert not agent.flag
-    agent.stop()
+    await agent.stop()
 
 
-def test_on_end_exception():
+async def test_on_end_exception():
     class TestOneShotBehaviour(OneShotBehaviour):
         async def run(self):
             pass
 
         async def on_end(self):
             result = 1 / 0
             self.agent.flag = True
 
     agent = MockedAgentFactory()
     agent.flag = False
     behaviour = TestOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert type(behaviour.exit_code) == ZeroDivisionError
     assert not agent.flag
-    agent.stop()
+    await agent.stop()
 
 
-def test_add_behaviour():
+async def test_add_behaviour():
     class EmptyOneShotBehaviour(OneShotBehaviour):
         async def run(self):
             self.kill()
 
     agent = MockedAgentFactory()
     behaviour = EmptyOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
     assert agent.has_behaviour(behaviour)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert behaviour.agent == agent
     assert behaviour.template is None
     assert behaviour.presence == agent.presence
     assert behaviour.web == agent.web
     assert behaviour.queue.empty()
 
-    behaviour.join()
+    await behaviour.join()
 
     assert behaviour.is_done()
-    agent.stop()
+    await agent.stop()
 
 
 def test_remove_behaviour():
     class EmptyBehaviour(CyclicBehaviour):
         async def run(self):
             pass
 
@@ -214,34 +212,34 @@
     agent = MockedAgentFactory()
     behaviour = EmptyBehaviour()
 
     with pytest.raises(ValueError):
         agent.remove_behaviour(behaviour)
 
 
-def test_wait_for_agent_start():
+async def test_wait_for_agent_start():
     class EmptyOneShotBehaviour(OneShotBehaviour):
         async def on_start(self):
             self.agent.started = True
             self.kill()
 
         async def run(self):
             pass
 
     agent = MockedAgentFactory()
     behaviour = EmptyOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.started
 
-    agent.stop()
+    await agent.stop()
 
 
 def test_behaviour_match():
     class TestBehaviour(OneShotBehaviour):
         async def run(self):
             pass
 
@@ -278,226 +276,221 @@
     msg.body = "Hello World"
     msg.thread = "thread-id"
     msg.set_metadata("performative", "query")
 
     assert behaviour.match(msg)
 
 
-def test_send_message(message):
+async def test_send_message(message):
     class SendBehaviour(OneShotBehaviour):
         async def run(self):
             await self.send(message)
             self.kill()
 
     agent = MockedAgentFactory(jid="sender@localhost")
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent2 = MockedAgentFactory(jid="to@localhost")
-    future = agent2.start(auto_register=False)
-    future.result()
+    await agent2.start(auto_register=False)
 
     agent2.dispatch = Mock()
 
     behaviour = SendBehaviour()
     agent.add_behaviour(behaviour)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent2.dispatch.assert_called
     msg_arg = agent2.dispatch.call_args[0][0]
     assert msg_arg.body == "message body"
     assert msg_arg.to == aioxmpp.JID.fromstr("to@localhost")
     assert msg_arg.thread == "thread-id"
 
-    agent.stop()
-    agent2.stop()
+    await agent.stop()
+    await agent2.stop()
 
 
-def test_send_message_to_external_agent():
+async def test_send_message_to_external_agent():
     message = Message(
         to="to@external_xmpp.com",
         sender="sender@localhost",
         body="message body",
         thread="thread-id",
         metadata={"metadata1": "value1", "metadata2": "value2"},
     )
 
     class SendBehaviour(OneShotBehaviour):
         async def run(self):
             await self.send(message)
             self.kill()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.client = MagicMock()
-    agent.client.send = CoroutineMock()
+    agent.client.send = AsyncMock()
     behaviour = SendBehaviour()
     agent.add_behaviour(behaviour)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.client.send.await_count == 1
     msg_arg = agent.client.send.await_args[0][0]
     assert msg_arg.body[None] == "message body"
     assert msg_arg.to == aioxmpp.JID.fromstr("to@external_xmpp.com")
     thread_found = False
     for data in msg_arg.xep0004_data:
         if data.title == SPADE_X_METADATA:
             for field in data.fields:
                 if field.var == "_thread_node":
                     assert field.values[0] == "thread-id"
                     thread_found = True
     assert thread_found
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_send_message_without_sender():
+async def test_send_message_without_sender():
     class SendBehaviour(OneShotBehaviour):
         async def run(self):
             msg = Message()
             await self.send(msg)
             self.kill()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.client = MagicMock()
-    agent.client.send = CoroutineMock()
+    agent.client.send = AsyncMock()
     behaviour = SendBehaviour()
     agent.add_behaviour(behaviour)
 
-    behaviour.join()
+    await behaviour.join()
 
     msg_arg = agent.client.send.await_args[0][0]
     assert msg_arg.from_ == aioxmpp.JID.fromstr("fake@jid")
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_receive():
+async def test_receive():
     class RecvBehaviour(OneShotBehaviour):
         async def run(self):
             msg = Message(body="received body")
             await asyncio.wait_for(self.queue.put(msg), 5.0)
             self.agent.recv_msg = await self.receive()
             self.kill()
 
     agent = MockedAgentFactory()
 
     behaviour = RecvBehaviour()
     agent.add_behaviour(behaviour)
     assert behaviour.mailbox_size() == 0
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     assert agent.is_alive()
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.recv_msg.body == "received body"
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_receive_with_timeout():
+async def test_receive_with_timeout():
     class RecvBehaviour(OneShotBehaviour):
         async def run(self):
             self.agent.recv_msg = await self.receive(15.0)
             self.kill()
 
     agent = MockedAgentFactory()
 
     msg = Message(body="received body")
     template = Template(body="received body")
     behaviour = RecvBehaviour()
     agent.add_behaviour(behaviour, template)
     assert behaviour.mailbox_size() == 0
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     assert agent.is_alive()
     assert agent.has_behaviour(behaviour)
     agent._message_received(msg.prepare())
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.recv_msg.body == "received body"
     assert agent.recv_msg == msg
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_receive_with_timeout_error():
+async def test_receive_with_timeout_error():
     class RecvBehaviour(OneShotBehaviour):
         async def run(self):
             self.agent.recv_msg = await self.receive(0.01)
             self.kill()
 
     agent = MockedAgentFactory()
 
     template = Template(body="received body")
     behaviour = RecvBehaviour()
     agent.add_behaviour(behaviour, template)
 
-    future = agent.start(auto_register=False)
-    future.result()
-    behaviour.join()
+    await agent.start(auto_register=False)
+
+    await behaviour.join()
 
     assert behaviour.mailbox_size() == 0
     assert agent.recv_msg is None
-    agent.stop()
+    await agent.stop()
 
 
-def test_receive_with_empty_queue():
+async def test_receive_with_empty_queue():
     class RecvBehaviour(OneShotBehaviour):
         async def run(self):
             self.agent.recv_msg = await self.receive()
             self.kill()
 
     agent = MockedAgentFactory()
 
     template = Template(body="received body")
     behaviour = RecvBehaviour()
     agent.add_behaviour(behaviour, template)
 
-    future = agent.start(auto_register=False)
-    future.result()
-    behaviour.join()
+    await agent.start(auto_register=False)
+
+    await behaviour.join()
 
     assert behaviour.mailbox_size() == 0
     assert agent.recv_msg is None
-    agent.stop()
+    await agent.stop()
 
 
-def test_set_get():
+async def test_set_get():
     class SendBehaviour(OneShotBehaviour):
         async def run(self):
             self.set("key", "value")
             assert self.get("key") == "value"
             self.kill()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     behaviour = SendBehaviour()
     agent.add_behaviour(behaviour)
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.get("key") == "value"
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_multiple_templates():
+async def test_multiple_templates():
     class Template1Behaviour(OneShotBehaviour):
         async def run(self):
             self.agent.msg1 = await self.receive(timeout=2)
 
     class Template2Behaviour(OneShotBehaviour):
         async def run(self):
             self.agent.msg2 = await self.receive(timeout=2)
@@ -522,205 +515,199 @@
     behaviour = Template3Behaviour()
     agent.add_behaviour(behaviour, template3)
 
     msg1 = Message(metadata={"performative": "template1"}).prepare()
     msg2 = Message(metadata={"performative": "template2"}).prepare()
     msg3 = Message(metadata={"performative": "template3"}).prepare()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent._message_received(msg1)
     agent._message_received(msg2)
     agent._message_received(msg3)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.msg1.get_metadata("performative") == "template1"
     assert agent.msg2.get_metadata("performative") == "template2"
     assert agent.msg3.get_metadata("performative") == "template3"
-    agent.stop()
+    await agent.stop()
 
 
-def test_kill_behaviour():
+async def test_kill_behaviour():
     class TestCyclicBehaviour(CyclicBehaviour):
         async def run(self):
             self.kill()
 
     agent = MockedAgentFactory()
     behaviour = TestCyclicBehaviour()
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(behaviour)
-    behaviour.join()
+    await behaviour.join()
 
     assert behaviour.is_killed()
     assert behaviour.exit_code == 0
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_exit_code_from_kill_behaviour():
+async def test_exit_code_from_kill_behaviour():
     class TestCyclicBehaviour(CyclicBehaviour):
         async def run(self):
             self.kill(42)
 
     agent = MockedAgentFactory()
     behaviour = TestCyclicBehaviour()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(behaviour)
-    behaviour.join()
+    await behaviour.join()
 
     assert behaviour.is_killed()
     assert behaviour.exit_code == 42
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_set_exit_code_behaviour():
+async def test_set_exit_code_behaviour():
     class TestCyclicBehaviour(CyclicBehaviour):
         async def run(self):
             self.exit_code = 1024
-            agent.event.wait()
+            await agent.event.wait()
             self.kill()
 
     agent = MockedAgentFactory()
     behaviour = TestCyclicBehaviour()
-    agent.event = Event()
-    future = agent.start(auto_register=False)
-    future.result()
+    agent.event = asyncio.Event()
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(behaviour)
 
     with pytest.raises(BehaviourNotFinishedException):
         assert behaviour.exit_code
 
     agent.event.set()
-    behaviour.join()
+    await behaviour.join()
 
-    future = agent.stop()
-    future.result()
+    await agent.stop()
 
     assert behaviour.exit_code == 1024
 
     assert not agent.is_alive()
 
 
-def test_notfinishedexception_behaviour():
+async def test_notfinishedexception_behaviour():
     class TestBehaviour(OneShotBehaviour):
         async def run(self):
-            self.agent.event.wait()
+            await self.agent.event.wait()
 
     agent = MockedAgentFactory()
-    agent.event = Event()
+    agent.event = asyncio.Event()
     behaviour = TestBehaviour()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(behaviour)
 
     with pytest.raises(BehaviourNotFinishedException):
         assert behaviour.exit_code
 
     agent.event.set()
 
     assert behaviour.exit_code == 0
 
-    future = agent.stop()
-    future.result()
+    await agent.stop()
 
     assert not agent.is_alive()
 
 
-def test_cyclic_behaviour():
+async def test_cyclic_behaviour():
     class TestCyclicBehaviour(CyclicBehaviour):
         async def run(self):
             self.agent.cycles += 1
             if self.agent.cycles > 2:
                 self.kill()
 
     agent = MockedAgentFactory()
     agent.cycles = 0
     behaviour = TestCyclicBehaviour()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert agent.cycles == 0
 
     agent.add_behaviour(behaviour)
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.cycles == 3
     assert behaviour.is_killed()
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_oneshot_behaviour():
+async def test_oneshot_behaviour():
     class TestOneShotBehaviour(OneShotBehaviour):
         async def run(self):
             self.agent.one_shot_behaviour_executed = True
             self.kill()
 
     agent = MockedAgentFactory()
     agent.one_shot_behaviour_executed = False
     behaviour = TestOneShotBehaviour()
     agent.add_behaviour(behaviour)
 
     assert agent.one_shot_behaviour_executed is False
 
-    future = agent.start(auto_register=False)
-    future.result()
-    behaviour.join()
+    await agent.start(auto_register=False)
+
+    await behaviour.join()
 
     assert agent.one_shot_behaviour_executed is True
-    agent.stop()
+    await agent.stop()
 
 
-def test_periodic_behaviour():
+async def test_periodic_behaviour():
     class TestPeriodicBehaviour(PeriodicBehaviour):
         async def run(self):
             self.agent.periodic_behaviour_execution_counter += 1
             self.kill()
 
     agent = MockedAgentFactory()
     agent.periodic_behaviour_execution_counter = 0
     behaviour = TestPeriodicBehaviour(0.01)
     agent.add_behaviour(behaviour)
 
     assert agent.periodic_behaviour_execution_counter == 0
 
-    future = agent.start(auto_register=False)
-    future.result()
-    behaviour.join()
+    await agent.start(auto_register=False)
+
+    await behaviour.join()
 
     assert agent.periodic_behaviour_execution_counter == 1
-    agent.stop()
+    await agent.stop()
 
 
-def test_periodic_behaviour_period_zero():
+async def test_periodic_behaviour_period_zero():
     class TestPeriodicBehaviour(PeriodicBehaviour):
         async def run(self):
             self.agent.periodic_behaviour_execution_counter += 1
             self.kill()
 
     agent = MockedAgentFactory()
     agent.periodic_behaviour_execution_counter = 0
     behaviour = TestPeriodicBehaviour(0)
     agent.add_behaviour(behaviour)
 
     assert agent.periodic_behaviour_execution_counter == 0
 
-    future = agent.start(auto_register=False)
-    future.result()
-    behaviour.join()
+    await agent.start(auto_register=False)
+
+    await behaviour.join()
 
     assert agent.periodic_behaviour_execution_counter == 1
-    agent.stop()
+    await agent.stop()
 
 
 def test_periodic_behaviour_negative_period():
     class TestPeriodicBehaviour(PeriodicBehaviour):
         async def run(self):
             pass
 
@@ -736,124 +723,120 @@
     behaviour = TestPeriodicBehaviour(1)
     assert behaviour.period == datetime.timedelta(seconds=1)
 
     behaviour.period = 2
     assert behaviour.period == datetime.timedelta(seconds=2)
 
 
-def test_periodic_start_at():
+async def test_periodic_start_at():
     class TestPeriodicBehaviour(PeriodicBehaviour):
         async def run(self):
             self.agent.delay = datetime.datetime.now()
             self.kill()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     start_at = datetime.datetime.now() + datetime.timedelta(seconds=0.01)
     behaviour = TestPeriodicBehaviour(period=0.01, start_at=start_at)
 
     assert behaviour._next_activation == start_at
 
     agent.add_behaviour(behaviour)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.delay >= start_at
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_timeout_behaviour():
+async def test_timeout_behaviour():
     class TestTimeoutBehaviour(TimeoutBehaviour):
         async def run(self):
             self.agent.delay = datetime.datetime.now()
             self.kill()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     start_at = datetime.datetime.now() + datetime.timedelta(seconds=0.01)
     behaviour = TestTimeoutBehaviour(start_at=start_at)
 
     assert behaviour._timeout == start_at
     assert not behaviour._timeout_triggered
 
     agent.add_behaviour(behaviour)
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.delay >= start_at
     assert behaviour._timeout_triggered
     assert behaviour.is_done()
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_timeout_behaviour_zero():
+async def test_timeout_behaviour_zero():
     class TestTimeoutBehaviour(TimeoutBehaviour):
         async def run(self):
             self.agent.delay = datetime.datetime.now()
             self.kill()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     start_at = datetime.datetime.now() + datetime.timedelta(seconds=0)
     behaviour = TestTimeoutBehaviour(start_at=start_at)
 
     assert behaviour._timeout == start_at
 
     assert not behaviour._timeout_triggered
 
     agent.add_behaviour(behaviour)
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.delay >= start_at
     assert behaviour._timeout_triggered
     assert behaviour.is_done()
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_fsm_behaviour(fsm):
+async def test_fsm_behaviour(fsm):
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
-    agent.sync1_behaviour = asyncio.Event(loop=agent.loop)
-    agent.sync2_behaviour = asyncio.Event(loop=agent.loop)
+    agent.sync1_behaviour = asyncio.Event()
+    agent.sync2_behaviour = asyncio.Event()
+    await agent.start(auto_register=False)
 
     agent.state = None
 
     assert len(fsm._transitions) == 2
     assert fsm.current_state == STATE_ONE
 
     agent.add_behaviour(fsm)
     assert fsm.current_state == STATE_ONE
     assert not fsm.state_one.is_done()
-    wait_for_behaviour_is_killed(fsm.state_one)
+    await wait_for_behaviour_is_killed(fsm.state_one)
     assert agent.state == STATE_ONE
-    agent.loop.call_soon_threadsafe(agent.sync1_behaviour.set)
-    fsm.state_one.join()
+    agent.sync1_behaviour.set()
+    await fsm.state_one.join()
 
     assert fsm.current_state == STATE_TWO
     assert not fsm.state_two.is_done()
-    wait_for_behaviour_is_killed(fsm.state_two)
+    await wait_for_behaviour_is_killed(fsm.state_two)
     assert agent.state == STATE_TWO
-    agent.loop.call_soon_threadsafe(agent.sync2_behaviour.set)
-    fsm.state_two.join()
+    agent.sync2_behaviour.set()
+    await fsm.state_two.join()
 
     assert fsm.current_state == STATE_THREE
-    wait_for_behaviour_is_killed(fsm.state_three)
+    await wait_for_behaviour_is_killed(fsm.state_three)
     assert agent.state == STATE_THREE
-    fsm.state_three.join()
+    await fsm.state_three.join()
 
-    agent.stop()
+    await agent.stop()
 
 
 def test_fsm_add_bad_state(fsm):
     with pytest.raises(AttributeError):
         fsm.add_state("BAD_STATE", object())
 
 
@@ -870,15 +853,15 @@
     with pytest.raises(NotValidState):
         fsm.is_valid_transition(STATE_ONE, "BAD_STATE")
 
     with pytest.raises(NotValidState):
         fsm.is_valid_transition("BAD_STATE", STATE_TWO)
 
 
-def test_fsm_bad_state():
+async def test_fsm_bad_state():
     class StateOne(State):
         async def run(self):
             self.set_next_state("BAD_STATE")
             self.kill()
 
     class StateTwo(State):
         async def run(self):
@@ -892,30 +875,30 @@
     state_one = StateOne()
     state_two = StateTwo()
     fsm_.add_state(STATE_ONE, state_one, initial=True)
     fsm_.add_state(STATE_TWO, state_two)
     fsm_.add_transition(STATE_ONE, STATE_TWO)
 
     agent = MockedAgentFactory()
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
     assert fsm_.current_state == STATE_ONE
 
     agent.add_behaviour(fsm_)
 
-    state_one.join()
+    await state_one.join()
     assert fsm_.current_state == STATE_ONE
 
-    fsm_.join()
+    await fsm_.join()
     assert fsm_.is_killed()
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_fsm_bad_transition():
+async def test_fsm_bad_transition():
     class StateOne(State):
         async def run(self):
             self.set_next_state(STATE_THREE)
             self.kill()
 
     class StateTwo(State):
         async def run(self):
@@ -936,28 +919,27 @@
     fsm_.add_state(STATE_ONE, state_one, initial=True)
     fsm_.add_state(STATE_TWO, state_two)
     fsm_.add_state(STATE_THREE, state_three)
     fsm_.add_transition(STATE_ONE, STATE_TWO)
     fsm_.add_transition(STATE_TWO, STATE_THREE)
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert fsm_.current_state == STATE_ONE
 
     agent.add_behaviour(fsm_)
 
-    state_one.join()
+    await state_one.join()
     assert fsm_.current_state == STATE_ONE
 
-    fsm_.join()
+    await fsm_.join()
     assert fsm_.is_killed()
 
-    agent.stop()
+    await agent.stop()
 
 
 def test_fsm_two_initials():
     class StateOne(State):
         async def run(self):
             self.set_next_state(STATE_THREE)
             self.kill()
@@ -975,161 +957,158 @@
     state_two = StateTwo()
     fsm_.add_state(STATE_ONE, state_one, initial=True)
     fsm_.add_state(STATE_TWO, state_two, initial=True)
 
     assert fsm_.current_state == STATE_TWO
 
 
-def test_fsm_fail_on_start():
+async def test_fsm_fail_on_start():
     class StateOne(State):
         async def on_start(self):
             raise Exception
 
         async def run(self):
             pass
 
     fsm_ = FSMBehaviour()
     state_one = StateOne()
     fsm_.add_state(STATE_ONE, state_one, initial=True)
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(fsm_)
 
-    fsm_.join()
+    await fsm_.join()
 
     assert fsm_.is_killed()
 
     assert type(fsm_.exit_code) == Exception
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_fsm_fail_on_run():
+async def test_fsm_fail_on_run():
     class StateOne(State):
         async def run(self):
             raise Exception
 
     fsm_ = FSMBehaviour()
     state_one = StateOne()
     fsm_.add_state(STATE_ONE, state_one, initial=True)
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(fsm_)
 
-    fsm_.join()
+    await fsm_.join()
 
     assert fsm_.is_killed()
 
     assert type(fsm_.exit_code) == Exception
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_fsm_fail_on_end():
+async def test_fsm_fail_on_end():
     class StateOne(State):
         async def run(self):
             pass
 
         async def on_end(self):
             raise Exception
 
     fsm_ = FSMBehaviour()
     state_one = StateOne()
     fsm_.add_state(STATE_ONE, state_one, initial=True)
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.add_behaviour(fsm_)
 
-    fsm_.join()
+    await fsm_.join()
 
     assert fsm_.is_killed()
 
     assert type(fsm_.exit_code) == Exception
 
-    agent.stop()
+    await agent.stop()
 
 
 def test_to_graphviz(fsm):
     assert (
-            fsm.to_graphviz()
-            == "digraph finite_state_machine { rankdir=LR; node [fixedsize=true];STATE_ONE -> STATE_TWO;STATE_TWO -> STATE_THREE;}"
+        fsm.to_graphviz()
+        == "digraph finite_state_machine { rankdir=LR; node [fixedsize=true];STATE_ONE -> STATE_TWO;STATE_TWO -> STATE_THREE;}"
     )
 
 
-def test_join():
+async def test_join():
     class WaitBehav(OneShotBehaviour):
         async def run(self):
             for i in range(100):
                 self.agent.i = i
                 await asyncio.sleep(0)
 
     agent = MockedAgentFactory()
     agent.i = None
     behaviour = WaitBehav()
 
     agent.add_behaviour(behaviour)
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join(timeout=None)
+    await behaviour.join(timeout=None)
 
     assert behaviour.is_done()
     assert agent.i == 99
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_join_with_timeout():
+async def test_join_with_timeout():
     class WaitBehav(OneShotBehaviour):
         async def run(self):
             await asyncio.sleep(100)
 
     agent = MockedAgentFactory()
     agent.i = None
     behaviour = WaitBehav()
 
     agent.add_behaviour(behaviour)
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
     with pytest.raises(TimeoutError):
-        behaviour.join(timeout=0.01)
+        await behaviour.join(timeout=0.01)
 
     assert not behaviour.is_done()
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_join_with_long_timeout():
+async def test_join_with_long_timeout():
     class WaitBehav(OneShotBehaviour):
         async def run(self):
             await asyncio.sleep(0)
 
     agent = MockedAgentFactory()
     agent.i = None
     behaviour = WaitBehav()
 
     agent.add_behaviour(behaviour)
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
-    behaviour.join(timeout=100)
+    await behaviour.join(timeout=100)
 
     assert behaviour.is_done()
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_join_inside_behaviour():
+async def test_join_inside_behaviour():
     class Behav1(OneShotBehaviour):
         async def run(self):
             class Behav2(OneShotBehaviour):
                 async def run(self):
                     self.agent.behav2 = True
 
             behav2 = Behav2()
@@ -1140,26 +1119,25 @@
     agent = MockedAgentFactory()
     agent.behav1 = False
     agent.behav2 = False
 
     behav1 = Behav1()
     agent.add_behaviour(behav1)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
-    behav1.join()
+    await behav1.join()
 
     assert agent.behav1
     assert agent.behav2
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_join_inside_behaviour_with_timeout():
+async def test_join_inside_behaviour_with_timeout():
     class Behav1(OneShotBehaviour):
         async def run(self):
             class Behav2(OneShotBehaviour):
                 async def run(self):
                     await asyncio.sleep(1)
 
             behav2 = Behav2()
@@ -1170,91 +1148,88 @@
 
     agent = MockedAgentFactory()
     agent.behav1 = False
 
     behav1 = Behav1()
     agent.add_behaviour(behav1)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
-    behav1.join()
+    await behav1.join()
 
     assert agent.behav1
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_behaviour_at_end():
+async def test_behaviour_at_end():
     class FinalBehav(OneShotBehaviour):
         async def run(self):
             self.agent.value = 2000
 
     class StopAgent(Agent):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
-            self._async_connect = CoroutineMock()
-            self._async_register = CoroutineMock()
+            self._async_connect = AsyncMock()
+            self._async_register = AsyncMock()
             self.conn_coro = Mock()
-            self.conn_coro.__aexit__ = CoroutineMock()
+            self.conn_coro.__aexit__ = AsyncMock()
             self.stream = Mock()
             self.value = 1000
 
-        def stop(self):
+        async def stop(self):
             behav = FinalBehav()
             self.add_behaviour(behav)
-            behav.join()
-            return super().stop()
+            await behav.join()
+            return await super().stop()
 
     agent = StopAgent("fakejid@fakeserver", "fakepassword")
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert agent.value == 1000
-    future = agent.stop()
-    future.result()
+    await agent.stop()
+
     assert agent.value == 2000
 
 
-def test_two_behaviours_at_end():
+async def test_two_behaviours_at_end():
     class FinalBehav2(OneShotBehaviour):
         async def run(self):
             self.agent.value = 2000
 
     class FinalBehav1(OneShotBehaviour):
         async def run(self):
             behav = FinalBehav2()
             self.agent.add_behaviour(behav)
             await behav.join()
 
     class StopAgent(Agent):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
-            self._async_connect = CoroutineMock()
-            self._async_register = CoroutineMock()
+            self._async_connect = AsyncMock()
+            self._async_register = AsyncMock()
             self.conn_coro = Mock()
-            self.conn_coro.__aexit__ = CoroutineMock()
+            self.conn_coro.__aexit__ = AsyncMock()
             self.stream = Mock()
             self.value = 1000
 
-        def stop(self):
+        async def stop(self):
             behav = FinalBehav1()
             self.add_behaviour(behav)
-            behav.join()
-            return super().stop()
+            await behav.join()
+            return await super().stop()
 
     agent = StopAgent("fakejid@fakeserver", "fakepassword")
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert agent.value == 1000
-    future = agent.stop()
-    future.result()
+    await agent.stop()
+
     assert agent.value == 2000
 
 
 def test_get_state(fsm):
     assert isinstance(fsm.get_state(STATE_ONE), StateOne)
     assert isinstance(fsm.get_state(STATE_TWO), StateTwo)
     assert isinstance(fsm.get_state(STATE_THREE), StateThree)
```

### Comparing `spade-3.2.3/tests/test_container.py` & `spade-3.3.0/tests/test_container.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import asyncio
-import time
+from unittest.mock import AsyncMock, MagicMock
 
 import aioxmpp
-from asynctest import MagicMock, CoroutineMock
 
 from spade.behaviour import OneShotBehaviour, CyclicBehaviour
 from spade.container import Container
 from spade.message import Message
 from .factories import MockedAgentFactory
 
 
-def test_use_container():
+async def test_use_container():
     container = Container()
     container.reset()
 
     agent = MockedAgentFactory()
 
     assert agent.container == Container()
 
     assert container.has_agent(str(agent.jid))
     assert container.get_agent(str(agent.jid)) == agent
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_send_message_with_container():
+async def test_send_message_with_container():
     class FakeReceiverAgent:
         def __init__(self):
             self.jid = "fake_receiver_agent@server"
 
         def set_container(self, c):
             pass
 
@@ -51,114 +50,91 @@
     container.reset()
     fake_receiver_agent = FakeReceiverAgent()
     container.register(fake_receiver_agent)
 
     fake_receiver_agent.dispatch = MagicMock()
 
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.client = MagicMock()
-    agent.client.send = CoroutineMock()
+    agent.client.send = AsyncMock()
     behaviour = SendBehaviour()
     agent.add_behaviour(behaviour)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert agent.client.send.await_count == 0
 
     assert fake_receiver_agent.dispatch.call_count == 1
     assert (
         str(fake_receiver_agent.dispatch.call_args[0][0].to)
         == "fake_receiver_agent@server"
     )
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_send_message_to_outer_with_container():
+async def test_send_message_to_outer_with_container():
     class SendBehaviour(OneShotBehaviour):
         async def run(self):
             message = Message(to="to@outerhost")
             await self.send(message)
             self.kill()
 
     container = Container()
     container.reset()
 
     agent = MockedAgentFactory()
-    agent.start(auto_register=False)
+    await agent.start(auto_register=False)
 
     behaviour = SendBehaviour()
-    behaviour._xmpp_send = CoroutineMock()
+    behaviour._xmpp_send = AsyncMock()
     agent.add_behaviour(behaviour)
 
-    behaviour.join()
+    await behaviour.join()
 
     assert container.has_agent(str(agent.jid))
     assert not container.has_agent("to@outerhost")
 
     assert behaviour._xmpp_send.await_count == 1
-    msg_arg = behaviour._xmpp_send.await_args[0][0]
+
+    args, kwargs = behaviour._xmpp_send.await_args
+    msg_arg = kwargs["msg"]
     assert msg_arg.to == aioxmpp.JID.fromstr("to@outerhost")
 
-    agent.stop()
+    await agent.stop()
 
 
 def test_unregister():
     container = Container()
-    container.reset()
 
     agent = MockedAgentFactory()
     agent2 = MockedAgentFactory(jid="agent2@server")
 
     assert container.has_agent(str(agent.jid))
     assert container.has_agent(str(agent2.jid))
 
     container.unregister(agent.jid)
 
     assert not container.has_agent(str(agent.jid))
     assert container.has_agent(str(agent2.jid))
 
 
-def test_cancel_tasks():
+async def test_cancel_tasks():
     agent = MockedAgentFactory()
 
     class Behav(CyclicBehaviour):
         async def run(self):
             await asyncio.sleep(100)
             self.has_finished = True
 
     behav = Behav()
     behav.has_finished = False
     agent.add_behaviour(behaviour=behav)
-    future = agent.start()
-    future.result()
+    await agent.start()
 
     assert not behav.has_finished
 
-    container = Container()
-    container.stop()
+    await agent.stop()
 
     assert not behav.has_finished
-
-
-def test_stop_container():
-    agent = MockedAgentFactory()
-
-    class Behav(OneShotBehaviour):
-        async def run(self):
-            container = Container()
-            container.stop()
-
-    behav = Behav()
-    agent.add_behaviour(behav)
-    future = agent.start(auto_register=False)
-    future.result()
-    behav.join()
-
-    counter = 0
-    while agent.is_alive() and counter < 5:
-        time.sleep(0.05)
-        counter += 1
-    assert not agent.is_alive()
```

### Comparing `spade-3.2.3/tests/test_message.py` & `spade-3.3.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/tests/test_plugin.py` & `spade-3.3.0/tests/test_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 from tests.factories import MockedConnectedAgent
 
 
-def test_add_plugin():
+async def test_add_plugin():
     class PluginMixin:
         async def _hook_plugin_before_connection(self, *args, **kwargs):
             await super()._hook_plugin_before_connection(*args, **kwargs)
             self.before_hook = True
 
         async def _hook_plugin_after_connection(self, *args, **kwargs):
             await super()._hook_plugin_after_connection(*args, **kwargs)
             self.after_hook = True
 
     class AgentWithPlugin(PluginMixin, MockedConnectedAgent):
         pass
 
     agent = AgentWithPlugin("test@localhost", "secret")
 
-    future = agent.start()
-    future.result()
+    await agent.start()
 
     assert agent.before_hook
     assert agent.after_hook
 
 
-def test_plugin_override():
+async def test_plugin_override():
     class PluginMixin:
         async def _hook_plugin_after_connection(self, *args, **kwargs):
             await super()._hook_plugin_after_connection(*args, **kwargs)
             self.client = None
 
     class AgentWithPlugin(PluginMixin, MockedConnectedAgent):
         pass
 
     agent = AgentWithPlugin("test@localhost", "secret")
 
-    future = agent.start()
-    future.result()
+    await agent.start()
 
     assert agent.client is None
 
 
-def test_plugin_multiple_override():
+async def test_plugin_multiple_override():
     """
     The order of the mixins is important
     """
+
     class PluginMixin1:
         async def _hook_plugin_after_connection(self, *args, **kwargs):
             await super()._hook_plugin_after_connection(*args, **kwargs)
             self.client = 1
 
     class PluginMixin2:
         async def _hook_plugin_after_connection(self, *args, **kwargs):
@@ -55,16 +54,17 @@
             self.client = 2
 
     class PluginMixin3:
         async def _hook_plugin_after_connection(self, *args, **kwargs):
             await super()._hook_plugin_after_connection(*args, **kwargs)
             self.client = 3
 
-    class AgentWithPlugin(PluginMixin1, PluginMixin2, PluginMixin3, MockedConnectedAgent):
+    class AgentWithPlugin(
+        PluginMixin1, PluginMixin2, PluginMixin3, MockedConnectedAgent
+    ):
         pass
 
     agent = AgentWithPlugin("test@localhost", "secret")
 
-    future = agent.start()
-    future.result()
+    await agent.start()
 
     assert agent.client == 1
```

### Comparing `spade-3.2.3/tests/test_presence.py` & `spade-3.3.0/tests/test_presence.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,216 +4,204 @@
 from aioxmpp import PresenceState, PresenceShow, JID, PresenceType, Presence
 from aioxmpp.roster.xso import Item as XSOItem
 
 from spade.presence import ContactNotFound
 from .factories import MockedPresenceAgentFactory
 
 
-def test_get_state_not_available():
+async def test_get_state_not_available():
     agent = MockedPresenceAgentFactory(available=False, show=PresenceShow.NONE)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert type(agent.presence.state) == PresenceState
     assert agent.presence.state.available is False
     assert agent.presence.state.show == PresenceShow.NONE
     assert not agent.presence.is_available()
 
 
-def test_get_state_available():
+async def test_get_state_available():
     agent = MockedPresenceAgentFactory(available=True)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.state.available
     assert agent.presence.is_available()
 
 
-def test_set_available():
+async def test_set_available():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_available()
 
     assert agent.presence.is_available()
 
 
-def test_set_available_with_show():
+async def test_set_available_with_show():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_available(show=PresenceShow.CHAT)
 
     assert agent.presence.is_available()
     assert agent.presence.state.show == PresenceShow.CHAT
 
 
-def test_set_unavailable():
+async def test_set_unavailable():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_unavailable()
 
     assert not agent.presence.is_available()
 
 
-def test_get_state_show():
+async def test_get_state_show():
     agent = MockedPresenceAgentFactory(available=True, show=PresenceShow.AWAY)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.state.show == PresenceShow.AWAY
 
 
-def test_get_status_empty():
+async def test_get_status_empty():
     agent = MockedPresenceAgentFactory(status={})
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.status == {}
 
 
-def test_get_status_string():
+async def test_get_status_string():
     agent = MockedPresenceAgentFactory(status="Working")
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.status == {None: "Working"}
 
 
-def test_get_status_dict():
+async def test_get_status_dict():
     agent = MockedPresenceAgentFactory(status={"en": "Working"})
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.status == {"en": "Working"}
 
 
-def test_get_priority_default():
+async def test_get_priority_default():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.priority == 0
 
 
-def test_get_priority():
+async def test_get_priority():
     agent = MockedPresenceAgentFactory(priority=10)
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.mock_presence()
 
     assert agent.presence.priority == 10
 
 
-def test_set_presence_available():
+async def test_set_presence_available():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_presence(state=PresenceState(available=True))
 
     assert agent.presence.is_available()
 
 
-def test_set_presence_unavailable():
+async def test_set_presence_unavailable():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_presence(state=PresenceState(available=False))
 
     assert not agent.presence.is_available()
 
 
-def test_set_presence_status():
+async def test_set_presence_status():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_presence(status="Lunch")
 
     assert agent.presence.status == {None: "Lunch"}
 
 
-def test_set_presence_status_dict():
+async def test_set_presence_status_dict():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_presence(status={"en": "Lunch"})
 
     assert agent.presence.status == {"en": "Lunch"}
 
 
-def test_set_presence_priority():
+async def test_set_presence_priority():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_presence(priority=5)
 
     assert agent.presence.priority == 5
 
 
-def test_set_presence():
+async def test_set_presence():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.set_presence(
         state=PresenceState(True, PresenceShow.PLAIN), status="Lunch", priority=2
     )
 
     assert agent.presence.is_available()
     assert agent.presence.state.show == PresenceShow.PLAIN
     assert agent.presence.status == {None: "Lunch"}
     assert agent.presence.priority == 2
 
 
-def test_get_contacts_empty():
+async def test_get_contacts_empty():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     assert agent.presence.get_contacts() == {}
 
 
-def test_get_contacts(jid):
+async def test_get_contacts(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     item = XSOItem(jid=jid)
     item.approved = True
     item.name = "My Friend"
 
     agent.presence.roster._update_entry(item)
 
@@ -225,19 +213,18 @@
     assert contacts[bare_jid]["approved"]
     assert contacts[bare_jid]["name"] == "My Friend"
     assert contacts[bare_jid]["subscription"] == "none"
     assert "ask" not in contacts[bare_jid]
     assert "groups" not in contacts[bare_jid]
 
 
-def test_get_contacts_with_presence(jid):
+async def test_get_contacts_with_presence(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     item = XSOItem(jid=jid)
     item.approved = True
     item.name = "My Available Friend"
 
     agent.presence.roster._update_entry(item)
 
@@ -249,19 +236,18 @@
     bare_jid = jid.bare()
     assert bare_jid in contacts
     assert contacts[bare_jid]["name"] == "My Available Friend"
 
     assert contacts[bare_jid]["presence"].type_ == PresenceType.AVAILABLE
 
 
-def test_get_contacts_with_presence_on_and_off(jid):
+async def test_get_contacts_with_presence_on_and_off(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     item = XSOItem(jid=jid)
     item.approved = True
     item.name = "My Friend"
 
     agent.presence.roster._update_entry(item)
 
@@ -275,19 +261,18 @@
     bare_jid = jid.bare()
     assert bare_jid in contacts
     assert contacts[bare_jid]["name"] == "My Friend"
 
     assert contacts[bare_jid]["presence"].type_ == PresenceType.UNAVAILABLE
 
 
-def test_get_contacts_with_presence_unavailable(jid):
+async def test_get_contacts_with_presence_unavailable(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     item = XSOItem(jid=jid)
     item.approved = True
     item.name = "My UnAvailable Friend"
 
     agent.presence.roster._update_entry(item)
 
@@ -299,19 +284,18 @@
     bare_jid = jid.bare()
     assert bare_jid in contacts
     assert contacts[bare_jid]["name"] == "My UnAvailable Friend"
 
     assert "presence" not in contacts[bare_jid]
 
 
-def test_get_contact(jid):
+async def test_get_contact(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     item = XSOItem(jid=jid)
     item.approved = True
     item.name = "My Friend"
 
     agent.presence.roster._update_entry(item)
 
@@ -321,229 +305,215 @@
     assert contact["approved"]
     assert contact["name"] == "My Friend"
     assert contact["subscription"] == "none"
     assert "ask" not in contact
     assert "groups" not in contact
 
 
-def test_get_invalid_jid_contact():
+async def test_get_invalid_jid_contact():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     with pytest.raises(ContactNotFound):
         agent.presence.get_contact(JID.fromstr("invalid@contact"))
 
 
-def test_get_invalid_str_contact():
+async def test_get_invalid_str_contact():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     with pytest.raises(AttributeError):
         agent.presence.get_contact("invalid@contact")
 
 
-def test_subscribe(jid):
+async def test_subscribe(jid):
     peer_jid = str(jid)
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.client.enqueue = Mock()
     agent.presence.subscribe(peer_jid)
 
     assert agent.client.enqueue.mock_calls
     arg = agent.client.enqueue.call_args[0][0]
 
     assert arg.to == jid.bare()
     assert arg.type_ == PresenceType.SUBSCRIBE
 
 
-def test_unsubscribe(jid):
+async def test_unsubscribe(jid):
     peer_jid = str(jid)
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.client.enqueue = Mock()
     agent.presence.unsubscribe(peer_jid)
 
     assert agent.client.enqueue.mock_calls
     arg = agent.client.enqueue.call_args[0][0]
 
     assert arg.to == jid.bare()
     assert arg.type_ == PresenceType.UNSUBSCRIBE
 
 
-def test_approve(jid):
+async def test_approve(jid):
     peer_jid = str(jid)
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.client.enqueue = Mock()
     agent.presence.approve(peer_jid)
 
     assert agent.client.enqueue.mock_calls
     arg = agent.client.enqueue.call_args[0][0]
 
     assert arg.to == jid.bare()
     assert arg.type_ == PresenceType.SUBSCRIBED
 
 
-def test_on_available(jid):
+async def test_on_available(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.on_available = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.AVAILABLE)
     agent.presence.presenceclient.handle_presence(stanza)
 
     jid_arg = agent.presence.on_available.call_args[0][0]
     stanza_arg = agent.presence.on_available.call_args[0][1]
 
     assert jid_arg == str(jid)
     assert stanza_arg.type_ == PresenceType.AVAILABLE
 
 
-def test_on_unavailable(jid):
+async def test_on_unavailable(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.on_unavailable = Mock()
     agent.presence.presenceclient._presences[jid.bare()] = {"home": None}
 
     stanza = Presence(from_=jid, type_=PresenceType.UNAVAILABLE)
     agent.presence.presenceclient.handle_presence(stanza)
 
     jid_arg = agent.presence.on_unavailable.call_args[0][0]
     stanza_arg = agent.presence.on_unavailable.call_args[0][1]
 
     assert jid_arg == str(jid)
     assert stanza_arg.type_ == PresenceType.UNAVAILABLE
 
 
-def test_on_subscribe(jid):
+async def test_on_subscribe(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.on_subscribe = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.SUBSCRIBE)
     agent.presence.roster.handle_subscribe(stanza)
 
     jid_arg = agent.presence.on_subscribe.call_args[0][0]
 
     assert jid_arg == str(jid)
 
 
-def test_on_subscribe_approve_all(jid):
+async def test_on_subscribe_approve_all(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.approve_all = True
     agent.client.enqueue = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.SUBSCRIBE)
     agent.presence.roster.handle_subscribe(stanza)
 
     assert agent.client.enqueue.mock_calls
     arg = agent.client.enqueue.call_args[0][0]
 
     assert arg.to == jid.bare()
     assert arg.type_ == PresenceType.SUBSCRIBED
 
 
-def test_on_subscribed(jid):
+async def test_on_subscribed(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.on_subscribed = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.SUBSCRIBED)
     agent.presence.roster.handle_subscribed(stanza)
 
     jid_arg = agent.presence.on_subscribed.call_args[0][0]
 
     assert jid_arg == str(jid)
 
 
-def test_on_unsubscribe(jid):
+async def test_on_unsubscribe(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.on_unsubscribe = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.UNSUBSCRIBE)
     agent.presence.roster.handle_unsubscribe(stanza)
 
     jid_arg = agent.presence.on_unsubscribe.call_args[0][0]
 
     assert jid_arg == str(jid)
 
 
-def test_on_unsubscribe_approve_all(jid):
+async def test_on_unsubscribe_approve_all(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.approve_all = True
     agent.client.enqueue = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.UNSUBSCRIBE)
     agent.presence.roster.handle_unsubscribe(stanza)
 
     assert agent.client.enqueue.mock_calls
     arg = agent.client.enqueue.call_args[0][0]
 
     assert arg.to == jid.bare()
     assert arg.type_ == PresenceType.UNSUBSCRIBED
 
 
-def test_on_unsubscribed(jid):
+async def test_on_unsubscribed(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.presence.on_unsubscribed = Mock()
 
     stanza = Presence(from_=jid, type_=PresenceType.UNSUBSCRIBED)
     agent.presence.roster.handle_unsubscribed(stanza)
 
     jid_arg = agent.presence.on_unsubscribed.call_args[0][0]
 
     assert jid_arg == str(jid)
 
 
-def test_on_changed(jid):
+async def test_on_changed(jid):
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     item = XSOItem(jid=jid)
     item.approved = True
     item.name = "My Friend"
 
     agent.presence.roster._update_entry(item)
 
@@ -559,19 +529,18 @@
 
     contact = agent.presence.get_contact(jid)
 
     assert contact["name"] == "My Friend"
     assert contact["presence"].show == PresenceShow.AWAY
 
 
-def test_ignore_self_presence():
+async def test_ignore_self_presence():
     agent = MockedPresenceAgentFactory()
 
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     jid = agent.jid
 
     stanza = Presence(from_=jid, type_=PresenceType.AVAILABLE, show=PresenceShow.CHAT)
     agent.presence.presenceclient.handle_presence(stanza)
 
     with pytest.raises(ContactNotFound):
```

### Comparing `spade-3.2.3/tests/test_template.py` & `spade-3.3.0/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/tests/test_trace.py` & `spade-3.3.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `spade-3.2.3/tests/test_web.py` & `spade-3.3.0/tests/test_web.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import asyncio
 import time
 
+import pytest
 import requests
 from aiohttp import web
 from aiohttp_jinja2 import get_env
 from aioxmpp import JID, PresenceType
 from aioxmpp.roster import Item
-from asynctest import Mock, CoroutineMock, MagicMock
 from jinja2 import ChoiceLoader, FileSystemLoader, PackageLoader
 from parsel import Selector
 from testfixtures import LogCapture
+from unittest.mock import AsyncMock, Mock, MagicMock
 
 from spade.agent import Agent
 from spade.behaviour import OneShotBehaviour, CyclicBehaviour
 from spade.message import Message
 from .factories import MockedAgentFactory, MockedPresenceAgentFactory
 
 
-def test_web():
+async def test_web():
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.web.start(port=10000)
 
     assert agent.web.app is not None
 
     counter = 0
     while counter < 4:
         if agent.web.server is not None:
             break
         counter += 1
-        time.sleep(0.1)
+        await asyncio.sleep(0.1)
     assert agent.web.server is not None
-    agent.stop()
+    await agent.stop()
 
 
-def test_default_template_path():
+async def test_default_template_path():
     agent = Agent("jid@server", "password")
 
     env = get_env(agent.web.app)
     loader = env.loader
 
     package_loader = loader.loaders[0]
     filesystem_loader = loader.loaders[1]
@@ -49,18 +50,18 @@
     assert type(package_loader) == PackageLoader
     assert type(filesystem_loader) == FileSystemLoader
 
     assert "internal_tpl_agent.html" in package_loader.list_templates()
     assert "internal_tpl_agent.html" not in filesystem_loader.list_templates()
     assert filesystem_loader.searchpath == ["."]
 
-    agent.stop()
+    await agent.stop()
 
 
-def test_add_template_path():
+async def test_add_template_path():
     agent = Agent("jid@server", "password")
 
     agent.web.start(templates_path="/tmp/spade")
 
     env = get_env(agent.web.app)
     loader = env.loader
 
@@ -71,155 +72,153 @@
     assert type(loader.loaders[2]) == FileSystemLoader
 
     filesystem_loader = loader.loaders[0]
 
     assert filesystem_loader.list_templates() == []
     assert filesystem_loader.searchpath == ["/tmp/spade"]
 
-    agent.stop()
+    await agent.stop()
 
 
-async def test_check_server(test_client):
+async def test_check_server(aiohttp_client, loop):
     agent = MockedAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.web.setup_routes()
 
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
     response = await client.get("/spade")
 
     text = await response.text()
 
     sel = Selector(text=text)
 
     assert sel.css("title::text").get() == "fake agent"
     assert sel.css("img::attr(src)").get() == agent.avatar
 
     assert sel.css("ul.products-list > li").getall() == []
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_request_home(test_client):
+async def test_request_home(aiohttp_client):
     agent = MockedAgentFactory(jid="jid@server", password="password")
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.get("/spade")
     response = await response.text()
 
     sel = Selector(text=response)
 
     assert sel.css("title::text").get() == "jid agent"
     assert sel.css("img::attr(src)").get() == agent.avatar
 
     assert sel.css("ul.products-list > li").getall() == []
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_get_messages(test_client):
+async def test_get_messages(aiohttp_client):
     agent = Agent("jid@server", "password")
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     # add messages to trace
     for i in range(5):
         msg = Message(body=str(i), sender="{}@server".format(i), to="receiver@server")
         agent.traces.append(msg)
 
     response = await client.get("/spade/messages/")
     response = await response.text()
 
     sel = Selector(text=response)
 
     assert len(sel.css("ul.timeline > li").getall()) == 6  # num messages + end clock
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_get_behaviour(test_client):
+async def test_get_behaviour(aiohttp_client):
     class EmptyOneShotBehaviour(OneShotBehaviour):
         async def run(self):
             self.kill()
 
     agent = Agent("jid@server", "password")
     behaviour = EmptyOneShotBehaviour()
     agent.add_behaviour(behaviour)
     agent.web.setup_routes()
 
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.get(
         "/spade/behaviour/OneShotBehaviour/EmptyOneShotBehaviour/"
     )
     response = await response.text()
 
     sel = Selector(text=response)
 
     assert (
         sel.css("section.content-header > h1::text").get().strip()
         == "OneShotBehaviour/EmptyOneShotBehaviour"
     )
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_kill_behaviour(test_client):
+async def test_kill_behaviour(aiohttp_client):
     class EmptyCyclicBehaviour(CyclicBehaviour):
         async def run(self):
             await asyncio.sleep(0.1)
 
     agent = Agent("jid@server", "password")
     behaviour = EmptyCyclicBehaviour()
     agent.add_behaviour(behaviour)
 
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     await client.get("/spade/behaviour/CyclicBehaviour/EmptyCyclicBehaviour/kill/")
 
     assert behaviour.is_killed()
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_get_agent(test_client):
+async def test_get_agent(aiohttp_client):
     agent = MockedPresenceAgentFactory(jid="jid@server", password="password")
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
 
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     jid = "friend@server"
     item = Item(jid=JID.fromstr(jid))
 
     agent.presence.roster._update_entry(item)
 
     response = await client.get(f"/spade/agent/{jid}/")
     response = await response.text()
 
     sel = Selector(text=response)
 
     assert sel.css("section.content-header > h1::text").get().strip() == jid
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_unsubscribe_agent(test_client):
+async def test_unsubscribe_agent(aiohttp_client):
     agent = MockedPresenceAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.client.enqueue = Mock()
 
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     jid = "friend@server"
     jid_ = JID.fromstr(jid)
     item = Item(jid=jid_)
 
     agent.presence.roster._update_entry(item)
 
@@ -229,25 +228,25 @@
 
     assert agent.client.enqueue.mock_calls
     arg = agent.client.enqueue.call_args[0][0]
 
     assert arg.to == jid_.bare()
     assert arg.type_ == PresenceType.UNSUBSCRIBE
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_send_agent(test_client):
+async def test_send_agent(aiohttp_client):
     agent = MockedPresenceAgentFactory()
-    future = agent.start(auto_register=False)
-    future.result()
+    await agent.start(auto_register=False)
+
     agent.stream = MagicMock()
-    agent.stream.send = CoroutineMock()
+    agent.stream.send = AsyncMock()
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     jid = "friend@server"
     item = Item(jid=JID.fromstr(jid))
     agent.presence.roster._update_entry(item)
 
     msg = "Hello World"
 
@@ -256,122 +255,127 @@
     assert str(response.url.relative()) == f"/spade/agent/{jid}/"
 
     sent = agent.traces.all()[0]
 
     assert sent[1].sent
     assert sent[1].body == "Hello World"
 
-    agent.stop().result()
+    await agent.stop()
 
 
 async def test_find_behaviour():
     class EmptyOneShotBehaviour(OneShotBehaviour):
         async def run(self):
             pass
 
     agent = MockedAgentFactory()
     behaviour = EmptyOneShotBehaviour()
     agent.add_behaviour(behaviour)
     found_behaviour = agent.web.find_behaviour("OneShotBehaviour/EmptyOneShotBehaviour")
 
     assert found_behaviour == behaviour
 
-    agent.stop().result()
+    await agent.stop()
 
 
 async def test_find_behaviour_fail():
     agent = Agent("jid@server", "password")
     found_behaviour = agent.web.find_behaviour("OneShotBehaviour/EmptyOneShotBehaviour")
 
     assert found_behaviour is None
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_add_get(test_client):
-    agent = Agent("jid@server", "password")
+async def test_add_get(aiohttp_client):
+    agent = MockedAgentFactory()
     agent.web.add_get("/test", lambda request: {"number": 42}, "tests/hello.html")
 
+    await agent.start(auto_register=False)
+
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.get("/test")
+
+    assert response.status == 200
+
     response = await response.text()
 
     sel = Selector(text=response)
     assert sel.css("h1::text").get().strip() == "42"
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_add_get_raw(test_client):
+async def test_add_get_raw(aiohttp_client):
     agent = Agent("jid@server", "password")
     agent.web.add_get(
         "/test",
         lambda request: web.Response(text="Hello Raw Get"),
         template=None,
         raw=True,
     )
 
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.get("/test")
     response = await response.text()
 
     assert response == "Hello Raw Get"
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_add_post(test_client):
+async def test_add_post(aiohttp_client):
     agent = Agent("jid@server", "password")
 
     async def handle_post(request):
         form = await request.post()
         number = form["number"]
         return {"number": number}
 
     agent.web.add_post("/test", handle_post, "tests/hello.html")
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.post("/test", data={"number": 1024})
     response = await response.text()
 
     sel = Selector(text=response)
     assert sel.css("h1::text").get() == "1024"
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_add_post_raw(test_client):
+async def test_add_post_raw(aiohttp_client):
     agent = Agent("jid@server", "password")
 
     async def handle_post(request):
         form = await request.post()
         number = form["number"]
         return web.Response(text="Hello Raw Post Number={}".format(number))
 
     agent.web.add_post("/test", handle_post, template=None, raw=True)
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.post("/test", data={"number": 1024})
     response = await response.text()
 
     assert response == "Hello Raw Post Number=1024"
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_stop(test_client):
+async def test_stop(aiohttp_client):
     agent = Agent("jid@server", "password")
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.get("/spade/stop")
     response = await response.text()
 
     sel = Selector(text=response)
     assert (
         sel.css("div.alert-warning > span::text").get().strip()
@@ -389,50 +393,50 @@
         log.check_present(
             ("spade.Web", "WARNING", "Stopping agent from web interface.")
         )
 
     counter = 5
     while agent.is_alive() and counter > 0:
         counter -= 0.5
-        time.sleep(0.5)
+        await asyncio.sleep(0.5)
 
     assert not agent.is_alive()
 
 
-async def test_add_get_json(test_client):
+async def test_add_get_json(aiohttp_client):
     async def controller(request):
         return {"number": 42}
 
     agent = Agent("jid@server", "password")
     agent.web.add_get("/test", controller, None)
 
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.get("/test")
     assert response.status == 200
 
     data = await response.json()
     assert data["number"] == 42
 
-    agent.stop().result()
+    await agent.stop()
 
 
-async def test_add_post_json(test_client):
+async def test_add_post_json(aiohttp_client):
     async def handle_post(request):
         form = await request.post()
         number = form["number"]
         return {"number": int(number)}
 
     agent = Agent("jid@server", "password")
     agent.web.add_post("/test", handle_post, None)
 
     agent.web.setup_routes()
-    client = await test_client(agent.web.app)
+    client = await aiohttp_client(agent.web.app)
 
     response = await client.post("/test", data={"number": 1024})
     assert response.status == 200
 
     data = await response.json()
     assert data["number"] == 1024
 
-    agent.stop().result()
+    await agent.stop()
```

