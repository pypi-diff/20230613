# Comparing `tmp/jncep-43.tar.gz` & `tmp/jncep-44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jncep-43.tar", last modified: Tue May  2 21:44:38 2023, max compression
+gzip compressed data, was "dist/jncep-44.tar", last modified: Tue Jun 13 15:14:05 2023, max compression
```

## Comparing `jncep-43.tar` & `jncep-44.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/
--rw-r--r--   0 runner    (1001) docker     (122)    36394 2023-05-02 21:44:38.000000 jncep-43/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    36394 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-02 21:44:38.000000 jncep-43/jncep.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/jncep/
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-02 21:44:16.000000 jncep-43/jncep/jncep.py
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-02 21:44:16.000000 jncep-43/jncep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17914 2023-05-02 21:44:16.000000 jncep-43/jncep/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    29459 2023-05-02 21:44:16.000000 jncep-43/jncep/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     7695 2023-05-02 21:44:16.000000 jncep-43/jncep/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-05-02 21:44:16.000000 jncep-43/jncep/trio_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-02 21:44:16.000000 jncep-43/jncep/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-05-02 21:44:16.000000 jncep-43/jncep/spec.py
--rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-05-02 21:44:16.000000 jncep-43/jncep/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-05-02 21:44:16.000000 jncep-43/jncep/jnclabs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-05-02 21:44:16.000000 jncep-43/jncep/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-05-02 21:44:16.000000 jncep-43/jncep/jncweb.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-05-02 21:44:16.000000 jncep-43/jncep/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:38.000000 jncep-43/jncep/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     6804 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/track.py
--rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/epub.py
--rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-02 21:44:16.000000 jncep-43/jncep/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-02 21:44:16.000000 jncep-43/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    30389 2023-05-02 21:44:16.000000 jncep-43/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-02 21:44:38.000000 jncep-43/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/
+-rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 15:14:05.000000 jncep-44/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/jncep/
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-06-13 15:13:39.000000 jncep-44/jncep/jnclabs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-06-13 15:13:39.000000 jncep-44/jncep/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-06-13 15:13:39.000000 jncep-44/jncep/jncweb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6552 2023-06-13 15:13:39.000000 jncep-44/jncep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20298 2023-06-13 15:13:39.000000 jncep-44/jncep/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-06-13 15:13:39.000000 jncep-44/jncep/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-13 15:13:39.000000 jncep-44/jncep/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-06-13 15:13:39.000000 jncep-44/jncep/trio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5256 2023-06-13 15:13:39.000000 jncep-44/jncep/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9519 2023-06-13 15:13:39.000000 jncep-44/jncep/spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-13 15:13:39.000000 jncep-44/jncep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/jncep/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4078 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/epub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6550 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-06-13 15:13:39.000000 jncep-44/jncep/cli/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7765 2023-06-13 15:13:39.000000 jncep-44/jncep/track.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-13 15:13:39.000000 jncep-44/jncep/jncep.py
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-13 15:14:05.000000 jncep-44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-13 15:13:39.000000 jncep-44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    37241 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 15:14:05.000000 jncep-44/jncep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    31100 2023-06-13 15:13:39.000000 jncep-44/README.md
```

### Comparing `jncep-43/PKG-INFO` & `jncep-44/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 43
+Version: 44
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
@@ -105,14 +105,26 @@
         - Log in to the J-Novel Club website with Facebook or Google
         - Go to the __Account__ page from the link at the top.
         - Click on the __Password__ section on the left hand side.
         - Set a password on that screen.
         
         Then the login email of the Facebook or Google account, together with that new password, can be used as credentials for the `jncep` tool, either directly or using one of the indirect methods.
         
+        ## Debugging mode
+        
+        A `--debug` (or `-d`) option can be passed to the `jncep` tool, before the specific command. It will print out more information about what is happening, using the standard Python `logging` package.
+        
+        For example:
+        
+        ```console
+        jncep --debug update
+        ```
+        
+        In case of an issue with `jncep`, it is recommended to launch with the `--debug` option and to include the output in the issue report (either inline or as a file attachment, if too long).
+        
         ## epub
         
         The `epub` command is used for simple EPUB generation, based on a URL link to a part or volume or series on the J-Novel Club website.
         
         ### Options
         
         To get some help about the arguments to the `epub` command, just launch with the `--help` option:
@@ -421,14 +433,17 @@
                                   CSS provided by JNCEP]
           -s, --sync              Flag to sync tracked series based on series followed
                                   on J-Novel Club and update the new ones from the
                                   beginning of the series
           -w, --whole             Flag to indicate whether the whole volume should be
                                   regenerated when a new part is detected during the
                                   update
+          -f, --whole-final       Flag to indicate whether an EPUB with a complete
+                                  volume should also be generated when the final part
+                                  of the volume is included in the update
           -e, --use-events        Flag to use the events feed to check for updates
           --help                  Show this message and exit.
         ```
         
         Most of the arguments to the `epub` command are also found here.
         
         ### Example
@@ -462,20 +477,22 @@
         If you have a lot of followed series and update often, the flag `--use-events` can be used. In that case, the `update` command will first check the events feed provided by J-Novel Club: It includes all the part releases and can be used to know which series will need to be downloaded. With this flag, the tool saves time by not checking all the series individually.
         
         ### Configuration & environment variables
         
         Compared to the `epub` command, the `update` command understands the additional configuration options:
         - USE_EVENTS
         - WHOLE
+        - WHOLE_FINAL
         
         Since they are flags, they should have a value like `1`, `true`, `t`, `yes`, `y` or `on` (case insensitive) if set.
         
         They are also available as environment variables:
         - JNCEP_USE_EVENTS
         - JNCEP_WHOLE
+        - JNCEP_WHOLE_FINAL
         
         ### Automation
         
         The `update` command can be called in the background from launchd (on macOS) or a scheduled task (on Windows) or cron (on Linux) in order to regularly download new content if available and create EPUBs (for example, once a day). 
         
         There is no notification built in the `jncep update` command but the text output can be combined with other tools to make something suitable. If there are updates, the `jncep update` command outputs something like `2 series sucessfully updated!`, which can be processed by another tool do create a notification.
```

### Comparing `jncep-43/jncep.egg-info/PKG-INFO` & `jncep-44/jncep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jncep
-Version: 43
+Version: 44
 Summary: Command-line tool to generate EPUB files for J-Novel Club pre-pub novels
 Home-page: https://github.com/gvellut/jncep
 Author: Guilhem Vellut
 Author-email: g@vellut.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/gvellut/jncep/issues
 Project-URL: Source, https://github.com/gvellut/jncep
@@ -105,14 +105,26 @@
         - Log in to the J-Novel Club website with Facebook or Google
         - Go to the __Account__ page from the link at the top.
         - Click on the __Password__ section on the left hand side.
         - Set a password on that screen.
         
         Then the login email of the Facebook or Google account, together with that new password, can be used as credentials for the `jncep` tool, either directly or using one of the indirect methods.
         
+        ## Debugging mode
+        
+        A `--debug` (or `-d`) option can be passed to the `jncep` tool, before the specific command. It will print out more information about what is happening, using the standard Python `logging` package.
+        
+        For example:
+        
+        ```console
+        jncep --debug update
+        ```
+        
+        In case of an issue with `jncep`, it is recommended to launch with the `--debug` option and to include the output in the issue report (either inline or as a file attachment, if too long).
+        
         ## epub
         
         The `epub` command is used for simple EPUB generation, based on a URL link to a part or volume or series on the J-Novel Club website.
         
         ### Options
         
         To get some help about the arguments to the `epub` command, just launch with the `--help` option:
@@ -421,14 +433,17 @@
                                   CSS provided by JNCEP]
           -s, --sync              Flag to sync tracked series based on series followed
                                   on J-Novel Club and update the new ones from the
                                   beginning of the series
           -w, --whole             Flag to indicate whether the whole volume should be
                                   regenerated when a new part is detected during the
                                   update
+          -f, --whole-final       Flag to indicate whether an EPUB with a complete
+                                  volume should also be generated when the final part
+                                  of the volume is included in the update
           -e, --use-events        Flag to use the events feed to check for updates
           --help                  Show this message and exit.
         ```
         
         Most of the arguments to the `epub` command are also found here.
         
         ### Example
@@ -462,20 +477,22 @@
         If you have a lot of followed series and update often, the flag `--use-events` can be used. In that case, the `update` command will first check the events feed provided by J-Novel Club: It includes all the part releases and can be used to know which series will need to be downloaded. With this flag, the tool saves time by not checking all the series individually.
         
         ### Configuration & environment variables
         
         Compared to the `epub` command, the `update` command understands the additional configuration options:
         - USE_EVENTS
         - WHOLE
+        - WHOLE_FINAL
         
         Since they are flags, they should have a value like `1`, `true`, `t`, `yes`, `y` or `on` (case insensitive) if set.
         
         They are also available as environment variables:
         - JNCEP_USE_EVENTS
         - JNCEP_WHOLE
+        - JNCEP_WHOLE_FINAL
         
         ### Automation
         
         The `update` command can be called in the background from launchd (on macOS) or a scheduled task (on Windows) or cron (on Linux) in order to regularly download new content if available and create EPUBs (for example, once a day). 
         
         There is no notification built in the `jncep update` command but the text output can be combined with other tools to make something suitable. If there are updates, the `jncep update` command outputs something like `2 series sucessfully updated!`, which can be processed by another tool do create a notification.
```

### Comparing `jncep-43/jncep.egg-info/SOURCES.txt` & `jncep-44/jncep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/jncep.py` & `jncep-44/jncep/jncep.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 )
 @click.version_option(JNCEP_VERSION, message="v%(version)s")
 @click.option(
     "-d",
     "--debug",
     "is_debug",
     is_flag=True,
-    help=("Flag to activate debug mode"),
+    help="Flag to activate debug mode",
     required=False,
 )
 def main(is_debug):
     setup_logging(is_debug)
     try:
         apply_options_from_config()
     except Exception:
         console.warning(
             "There was an error reading the configuration at: "
-            f"{DEFAULT_CONFIG_FILEPATH}. Continuing..." )
+            f"{DEFAULT_CONFIG_FILEPATH}. Continuing..."
+        )
 
 
 main.add_command(generate_epub)
 main.add_command(track_series)
 main.add_command(update_tracked)
 main.add_command(config_manage)
```

### Comparing `jncep-43/jncep/update.py` & `jncep-44/jncep/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import namedtuple
 from functools import partial
 import logging
 import sys
 
 import attr
 import dateutil
 import trio
@@ -20,25 +21,35 @@
     is_updated = attr.ib(None)
     is_considered = attr.ib(True)
     # to indicate a series with expired parts only
     # will set to latest part or will always have error
     # if stalled
     is_force_set_updated = attr.ib(False)
     is_update_last_checked = attr.ib(True)
+    parts_downloaded = attr.ib(None)
+
+
+UpdateOptions = namedtuple(
+    "UpdateOptions",
+    [
+        "is_sync",
+        "is_whole_volume",
+        "is_whole_volume_on_final_part",
+        "is_use_events",
+    ],
+)
 
 
 async def update_url_series(
     session,
     jnc_url,
     epub_generation_options,
     tracked_series,
-    is_sync,
     new_synced,
-    is_whole_volume,
-    is_use_events,
+    update_options,
 ):
     # for single url => if error no catch : let it crash and report to the user
     jnc_resource = jncweb.resource_from_url(jnc_url)
     series_id = await core.resolve_series(session, jnc_resource)
     series = await core.fetch_meta(session, series_id)
 
     series_url = jncweb.url_from_series_slug(series.raw_data.slug)
@@ -46,48 +57,50 @@
     if series_url not in tracked_series:
         console.warning(
             f"The series '[highlight]{series.raw_data.title}[/]' is not tracked! "
             f"Use the 'jncep track add' command first."
         )
         return
 
-    if is_sync:
+    if update_options.is_sync:
         # not very useful but make it possible
         # only consider newly synced series if --sync used
         # to mirror case with no URL argument
         if series_url not in new_synced:
             console.warning(
                 f"The series '[highlight]{series.raw_data.title}[/]' is not "
                 "among the tracked series added from syncing. Use 'jncep update' "
                 "without --sync."
             )
             return
 
     series_details = tracked_series[series_url]
 
     is_need_check = True
-    is_check_events = is_use_events and _can_use_events_feed(series_details)
+    is_check_events = update_options.is_use_events and _can_use_events_feed(
+        series_details
+    )
     if is_check_events:
         console.status("Checking J-Novel Club events feed...", clear=False)
         start_date = series_details.last_check_date
         events = await core.fetch_events(session, start_date)
         is_need_check = _verify_series_needs_update_check(events, series_details)
         if not is_need_check:
             update_result = UpdateResult(is_updated=False)
         console.pop_status()
 
     if is_need_check:
         # the series has just been synced so force EPUB gen from start in this case
-        is_force_from_beginning = is_sync
+        is_force_from_beginning = update_options.is_sync
         update_result = await _create_epub_for_new_parts(
             session,
             series_details,
             series,
             epub_generation_options,
-            is_whole_volume,
+            update_options,
             is_force_from_beginning,
         )
 
     if update_result.is_updated:
         emoji = ""
         if console.is_advanced():
             emoji = "\u2714 "
@@ -113,21 +126,23 @@
     _update_tracking_data(series_details, series, update_result, session.now)
 
 
 async def update_all_series(
     session,
     epub_generation_options,
     tracked_series,
-    is_sync,
     new_synced,
-    is_whole_volume,
-    is_use_events,
+    update_options,
 ):
     # is_sync: all parts from beginning so no need for the events
-    if not is_sync and is_use_events and _can_any_use_events_feed(tracked_series):
+    if (
+        not update_options.is_sync
+        and update_options.is_use_events
+        and _can_any_use_events_feed(tracked_series)
+    ):
         console.status("Checking J-Novel Club events feed...", clear=False)
         start_date = _min_last_check_date(tracked_series)
         events = await core.fetch_events(session, start_date)
         console.pop_status()
     else:
         events = None
 
@@ -137,17 +152,17 @@
         tasks.append(
             partial(
                 _handle_series,
                 session,
                 series_url,
                 series_details,
                 epub_generation_options,
-                is_sync,
+                update_options.is_sync,
                 new_synced,
-                is_whole_volume,
+                update_options,
                 events,
             )
         )
         series_details_a.append(series_details)
 
     results = await bag(tasks)
 
@@ -229,15 +244,15 @@
 async def _handle_series(
     session,
     series_url,
     series_details,
     epub_generation_options,
     is_sync,
     new_synced,
-    is_whole_volume,
+    update_options,
     events,
 ):
     series = None
     try:
         if is_sync and series_url not in new_synced:
             return UpdateResult(is_considered=False)
 
@@ -256,15 +271,15 @@
         # generate from the start if the series is newly sync
         is_force_from_beginning = is_sync
         update_result = await _create_epub_for_new_parts(
             session,
             series_details,
             series,
             epub_generation_options,
-            is_whole_volume,
+            update_options,
             is_force_from_beginning,
         )
 
         if update_result.is_updated:
             emoji = ""
             if console.is_advanced():
                 emoji = "\u2714 "
@@ -365,163 +380,195 @@
 
 
 def _can_use_events_feed(series_details):
     # the 2 attributes have been added later so may not always be there
     return "series_id" in series_details and "last_check_date" in series_details
 
 
-# TODO too complex ; refactor
 async def _create_epub_for_new_parts(
     session,
     series_details,
     series,
     epub_generation_options,
-    is_whole_volume=False,
+    update_options,
     is_force_from_beginning=False,
 ):
     parts = core.all_parts_meta(series)
 
     if series_details.part == 0 or is_force_from_beginning:
         # Firt clause: special processing : means there was no part available when the
         # series was started tracking
 
-        # still no part ?
-        if not parts:
-            return UpdateResult(is_updated=False)
-        else:
-            console.info(
-                f"The series '[highlight]{series.raw_data.title}[/]' "
-                "will be updated..."
-            )
-
-            part_filter = partial(core.is_part_available, session.now)
-
-            (
-                volumes_to_download,
-                parts_to_download,
-            ) = core.relevant_volumes_and_parts_for_content(series, part_filter)
-            volumes_for_cover = core.relevant_volumes_for_cover(
-                volumes_to_download, epub_generation_options.is_by_volume
-            )
-
-            await core.fill_covers_and_content(
-                session, volumes_for_cover, parts_to_download
-            )
-            await core.create_epub(
-                series,
-                volumes_to_download,
-                parts_to_download,
-                epub_generation_options,
-            )
-
-            return UpdateResult(series, is_updated=True)
+        update_result = await _update_from_beginning(
+            session, series, parts, epub_generation_options
+        )
+        # no need for _generate_whole_volume_on_final_part: if from the beginning +
+        # final included => the whole volume is already generated
+        return update_result
     else:
-        if not series_details.part_date:
-            # if here => old format, first lookup date of last part and use that
-            # still useful for stalled series so keep it
-            part_spec = spec.analyze_part_specs(series_details.part)
-            for part in parts:
-                if part_spec.has_part(part):
-                    # will be filled if the part still exists (it should)
-                    # TODO case it doesn't ? eg tracked.json filled by hand
-                    last_update_part = part
-                    break
-            # in UTC
-            last_update_date = last_update_part.raw_data.launch
-        else:
-            # new format : date is recorded
-            last_update_date = series_details.part_date
-
-        last_update_date = dateutil.parser.parse(last_update_date)
-
-        parts_release_after_date = _filter_parts_released_after_date(
-            last_update_date, parts
+        update_result = await _update_new_parts(
+            session,
+            series_details,
+            series,
+            parts,
+            epub_generation_options,
+            update_options,
         )
 
-        if not parts_release_after_date:
-            # not updated
-            return UpdateResult(series, is_updated=False)
-
-        available_parts_to_download = [
-            part
-            for part in parts_release_after_date
-            if core.is_part_available(session.now, part)
-        ]
-
-        if not available_parts_to_download:
-            console.warning(
-                f"All updated parts for '[highlight]{series.raw_data.title}[/]' "
-                "have expired!"
-            )
-            # not updated but the series will still have its tracking data changed
-            # in tracking config ; if not, the message above will always be displayed
-            # should be rare (if updating often) ; also first part is preview
-            # so even rarer
-            return UpdateResult(
-                series=series, is_updated=False, is_force_set_updated=True
+        if (
+            update_result.is_updated
+            and update_options.is_whole_volume_on_final_part
+            and not update_options.is_whole_volume
+        ):
+            # TODO do that as soon as we know which parts to download before
+            # fill_covers_and_content
+            parts_downloaded = update_result.parts_downloaded
+            await _generate_whole_volume_on_final_part(
+                session, series, parts_downloaded, epub_generation_options
             )
 
-        console.info(
-            f"The series '[highlight]{series.raw_data.title}[/]' will " "be updated..."
-        )
+        return update_result
 
-        # after the to update notification
-        if len(available_parts_to_download) != len(parts_release_after_date):
-            console.warning(
-                f"Some parts for '[highlight]{series.raw_data.title}[/]' have "
-                "expired!"
-            )
 
-        parts_id_to_download = set(
-            (part.part_id for part in available_parts_to_download)
+async def _update_from_beginning(session, series, parts, epub_generation_options):
+    # still no part ?
+    if not parts:
+        return UpdateResult(is_updated=False)
+    else:
+        console.info(
+            f"The series '[highlight]{series.raw_data.title}[/]' " "will be updated..."
         )
 
-        # availability alread tested
-        def simple_part_filter(part):
-            return part.part_id in parts_id_to_download
+        part_filter = partial(core.is_part_available, session.now)
 
         (
             volumes_to_download,
             parts_to_download,
-        ) = core.relevant_volumes_and_parts_for_content(series, simple_part_filter)
-
-        if is_whole_volume:
-            # second pass : filter on the volumes_to_download
-            # all the parts of those volumes must be downloaded
-            volumes_id_to_download = set((v.volume_id for v in volumes_to_download))
-
-            def whole_volume_part_filter(part):
-                return (
-                    part.volume.volume_id in volumes_id_to_download
-                    and core.is_part_available(session.now, part)
-                )
-
-            (
-                volumes_to_download,
-                parts_to_download,
-            ) = core.relevant_volumes_and_parts_for_content(
-                series, whole_volume_part_filter
-            )
-
+        ) = core.relevant_volumes_and_parts_for_content(series, part_filter)
         volumes_for_cover = core.relevant_volumes_for_cover(
             volumes_to_download, epub_generation_options.is_by_volume
         )
 
         await core.fill_covers_and_content(
             session, volumes_for_cover, parts_to_download
         )
-
         await core.create_epub(
             series,
             volumes_to_download,
             parts_to_download,
             epub_generation_options,
         )
 
-        return UpdateResult(series, is_updated=True)
+        return UpdateResult(series, is_updated=True, parts_downloaded=parts_to_download)
+
+
+async def _update_new_parts(
+    session,
+    series_details,
+    series,
+    parts,
+    epub_generation_options,
+    update_options,
+):
+    if not series_details.part_date:
+        # if here => old format, first lookup date of last part and use that
+        # still useful for stalled series so keep it
+        part_spec = spec.analyze_part_specs(series_details.part)
+        for part in parts:
+            if part_spec.has_part(part):
+                # will be filled if the part still exists (it should)
+                # TODO case it doesn't ? eg tracked.json filled by hand
+                last_update_part = part
+                break
+        # in UTC
+        last_update_date = last_update_part.raw_data.launch
+    else:
+        # new format : date is recorded
+        last_update_date = series_details.part_date
+
+    last_update_date = dateutil.parser.parse(last_update_date)
+
+    parts_release_after_date = _filter_parts_released_after_date(
+        last_update_date, parts
+    )
+
+    if not parts_release_after_date:
+        # not updated
+        return UpdateResult(series, is_updated=False)
+
+    available_parts_to_download = [
+        part
+        for part in parts_release_after_date
+        if core.is_part_available(session.now, part)
+    ]
+
+    if not available_parts_to_download:
+        console.warning(
+            f"All updated parts for '[highlight]{series.raw_data.title}[/]' "
+            "have expired!"
+        )
+        # not updated but the series will still have its tracking data changed
+        # in tracking config ; if not, the message above will always be displayed
+        # should be rare (if updating often) ; also first part is preview
+        # so even rarer
+        return UpdateResult(series=series, is_updated=False, is_force_set_updated=True)
+
+    console.info(
+        f"The series '[highlight]{series.raw_data.title}[/]' will be updated..."
+    )
+
+    # after the to update notification
+    if len(available_parts_to_download) != len(parts_release_after_date):
+        console.warning(
+            f"Some parts for '[highlight]{series.raw_data.title}[/]' have " "expired!"
+        )
+
+    parts_id_to_download = set((part.part_id for part in available_parts_to_download))
+
+    # availability alread tested
+    def simple_part_filter(part):
+        return part.part_id in parts_id_to_download
+
+    (
+        volumes_to_download,
+        parts_to_download,
+    ) = core.relevant_volumes_and_parts_for_content(series, simple_part_filter)
+
+    if update_options.is_whole_volume:
+        # second pass : filter on the volumes_to_download
+        # all the parts of those volumes must be downloaded
+        volumes_id_to_download = set((v.volume_id for v in volumes_to_download))
+
+        def whole_volume_part_filter(part):
+            return (
+                part.volume.volume_id in volumes_id_to_download
+                and core.is_part_available(session.now, part)
+            )
+
+        (
+            volumes_to_download,
+            parts_to_download,
+        ) = core.relevant_volumes_and_parts_for_content(
+            series, whole_volume_part_filter
+        )
+
+    volumes_for_cover = core.relevant_volumes_for_cover(
+        volumes_to_download, epub_generation_options.is_by_volume
+    )
+
+    await core.fill_covers_and_content(session, volumes_for_cover, parts_to_download)
+
+    await core.create_epub(
+        series,
+        volumes_to_download,
+        parts_to_download,
+        epub_generation_options,
+    )
+
+    return UpdateResult(series, is_updated=True, parts_downloaded=parts_to_download)
 
 
 def _is_released_after_date(date, part_date_s):
     # all date strings are in ISO format
     # so no need to parse really
     # parsing just to be safe
     # in case different shape like ms part or not (which throws str comp off)
@@ -532,7 +579,44 @@
 def _filter_parts_released_after_date(date, parts):
     parts_to_download = []
     for part in parts:
         if _is_released_after_date(date, part.raw_data.launch):
             parts_to_download.append(part)
 
     return parts_to_download
+
+
+async def _generate_whole_volume_on_final_part(
+    session, series, parts_downloaded, epub_generation_options
+):
+    # check if any part included in the update is the final part of its volume
+    for part in parts_downloaded:
+        # only max one part can be final in a volume
+        if not core._is_part_final(part):
+            continue
+
+        # check if possibly all parts have already been downloaded as part of the
+        # update
+        for volpart in part.volume.parts:
+            if volpart not in parts_downloaded:
+                break
+        else:
+            # all the parts have been downloaded in the normal course
+            # of things, so we skip regenerating the whole volume
+            continue
+
+        console.info(
+            "The complete volume "
+            f"'[highlight]{part.volume.raw_data.title}[/]' will be "
+            "downloaded..."
+        )
+
+        # With JNC if the final part can be downloaded, the rest of the
+        # volume is also available for download so no need to check
+
+        await core.fill_covers_and_content(session, [part.volume], part.volume.parts)
+        await core.create_epub(
+            series,
+            [part.volume],
+            part.volume.parts,
+            epub_generation_options,
+        )
```

### Comparing `jncep-43/jncep/core.py` & `jncep-44/jncep/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,27 +49,44 @@
 
 
 class SeriesNotANovelError(Exception):
     pass
 
 
 class JNCEPSession:
+    _GLOBAL_SESSION_INSTANCE = None
+
     def __init__(self, email, password):
         self.api = jnclabs.JNCLabsAPI()
         self.email = email
         self.password = password
         self.now = datetime.now(tz=timezone.utc)
 
     async def __aenter__(self) -> "JNCEPSession":
+        if JNCEPSession._GLOBAL_SESSION_INSTANCE:
+            # nested
+            return JNCEPSession._GLOBAL_SESSION_INSTANCE
+
         await self.login(self.email, self.password)
+        # current session is the top level session
+        JNCEPSession._GLOBAL_SESSION_INSTANCE = self
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
-        console.stop_status()
+        try:
+            console.stop_status()
+        except Exception:
+            pass
+
+        if JNCEPSession._GLOBAL_SESSION_INSTANCE != self:
+            # nested ; do not logout => leave it to the top level session
+            return False
 
+        # current session is the top level session
+        JNCEPSession._GLOBAL_SESSION_INSTANCE = None
         await self.logout()
         return False
 
     async def login(self, email, password):
         display_email = email
         if is_debug():
             # hide for privacy in case the trace is copied to GH issue tracker
```

### Comparing `jncep-43/jncep/track.py` & `jncep-44/jncep/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,19 +70,19 @@
         for legacy_series_url, value in converted.items():
             new_series_url = jncweb.to_new_website_series_url(legacy_series_url)
             converted_b[new_series_url] = value
 
         return converted_b
 
 
-async def track_series(session, tracked_series, series):
+async def track_series(session, tracked_series, series, is_beginning=False):
     parts = core.all_parts_meta(series)
 
     # record current last part + name
-    if not parts:
+    if not parts or is_beginning:
         # no parts yet, special value 0: processed in update with special case
         pn = 0
         # 0000-... not a valid date so 1111-...
         pdate = "1111-11-11T11:11:11.111Z"
 
         console.info(
             f"The series '[highlight]{series.raw_data.title}[/]' is now tracked, "
@@ -122,23 +122,25 @@
             "name": series.raw_data.title,
             "series_id": series.series_id,
             "last_check_date": utils.isoformat_with_z(session.now),
         }
     )
 
 
-async def sync_series_forward(session, follows, tracked_series, is_delete):
+async def sync_series_forward(
+    session, follows, tracked_series, is_delete, is_beginning
+):
     # sync local tracked series based on remote follows
     new_synced = []
     del_synced = []
 
     async def do_track(jnc_resource):
         series_id = await core.resolve_series(session, jnc_resource)
         series = await core.fetch_meta(session, series_id)
-        await track_series(session, tracked_series, series)
+        await track_series(session, tracked_series, series, is_beginning)
         # manga already excluded from follows so no need to check
 
         series_url = jncweb.url_from_series_slug(series.raw_data.slug)
         new_synced.append(series_url)
 
     tasks = []
     for jnc_resource in follows:
```

### Comparing `jncep-43/jncep/trio_utils.py` & `jncep-44/jncep/trio_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,22 @@
                 raise base_ex
             # just the first
             raise ex.exceptions[0]
 
     return wrapper
 
 
+def is_in_trio_context():
+    try:
+        trio.lowlevel.current_task()
+        return True
+    except RuntimeError:
+        return False
+
+
 # taken from trio-future (but needs py > 3.7.0) so done here
 @attr.s
 class Future:
     result_chan: trio.abc.ReceiveChannel = attr.ib()
 
     async def get(self):
         future_outcome = await self.outcome()
```

### Comparing `jncep-43/jncep/model.py` & `jncep-44/jncep/model.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/spec.py` & `jncep-44/jncep/spec.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/epub.py` & `jncep-44/jncep/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/jnclabs.py` & `jncep-44/jncep/jnclabs.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/config.py` & `jncep-44/jncep/config.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/jncweb.py` & `jncep-44/jncep/jncweb.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/utils.py` & `jncep-44/jncep/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 
 rich_theme = rich.theme.Theme(
     {
         "success": "green",
         "warning": "yellow",
         "error": "red",
         "highlight": "magenta",
+        "important": "bold",
     }
 )
 
 
 class RichConsole:
     def __init__(self):
         self.console = rich.console.Console(
```

### Comparing `jncep-43/jncep/cli/track.py` & `jncep-44/jncep/cli/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,24 @@
 @click.option(
     "-d",
     "--delete",
     "is_delete",
     is_flag=True,
     help="Flag to delete series not found on the sync source",
 )
+# from the beginning: so that when update is run after => update from the beginning
+@click.option(
+    "-b",
+    "--beginning",
+    "is_beginning",
+    is_flag=True,
+    help="Flag to add new series from the beginning",
+)
 @coro
-async def sync_series(email, password, is_reverse, is_delete):
+async def sync_series(email, password, is_reverse, is_delete, is_beginning):
     track_manager = track.TrackConfigManager()
     tracked_series = track_manager.read_tracked_series()
 
     async with core.JNCEPSession(email, password) as session:
         console.status("Fetch followed series from J-Novel Club...")
         follows: List[jncweb.JNCResource] = await session.api.fetch_follows()
 
@@ -105,15 +113,15 @@
                     style="success",
                 )
 
         else:
             console.status("Sync tracked series from J-Novel Club...")
 
             new_synced, del_synced = await track.sync_series_forward(
-                session, follows, tracked_series, is_delete
+                session, follows, tracked_series, is_delete, is_beginning
             )
 
             track_manager.write_tracked_series(tracked_series)
 
             if new_synced or del_synced:
                 console.info(
                     "The list of tracked series has been sucessfully updated!",
```

### Comparing `jncep-43/jncep/cli/options.py` & `jncep-44/jncep/cli/options.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/cli/epub.py` & `jncep-44/jncep/cli/epub.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/cli/config.py` & `jncep-44/jncep/cli/config.py`

 * *Files identical despite different names*

### Comparing `jncep-43/jncep/cli/base.py` & `jncep-44/jncep/cli/base.py`

 * *Files identical despite different names*

### Comparing `jncep-43/setup.py` & `jncep-44/setup.py`

 * *Files identical despite different names*

### Comparing `jncep-43/README.md` & `jncep-44/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,26 @@
 - Log in to the J-Novel Club website with Facebook or Google
 - Go to the __Account__ page from the link at the top.
 - Click on the __Password__ section on the left hand side.
 - Set a password on that screen.
 
 Then the login email of the Facebook or Google account, together with that new password, can be used as credentials for the `jncep` tool, either directly or using one of the indirect methods.
 
+## Debugging mode
+
+A `--debug` (or `-d`) option can be passed to the `jncep` tool, before the specific command. It will print out more information about what is happening, using the standard Python `logging` package.
+
+For example:
+
+```console
+jncep --debug update
+```
+
+In case of an issue with `jncep`, it is recommended to launch with the `--debug` option and to include the output in the issue report (either inline or as a file attachment, if too long).
+
 ## epub
 
 The `epub` command is used for simple EPUB generation, based on a URL link to a part or volume or series on the J-Novel Club website.
 
 ### Options
 
 To get some help about the arguments to the `epub` command, just launch with the `--help` option:
@@ -411,14 +423,17 @@
                           CSS provided by JNCEP]
   -s, --sync              Flag to sync tracked series based on series followed
                           on J-Novel Club and update the new ones from the
                           beginning of the series
   -w, --whole             Flag to indicate whether the whole volume should be
                           regenerated when a new part is detected during the
                           update
+  -f, --whole-final       Flag to indicate whether an EPUB with a complete
+                          volume should also be generated when the final part
+                          of the volume is included in the update
   -e, --use-events        Flag to use the events feed to check for updates
   --help                  Show this message and exit.
 ```
 
 Most of the arguments to the `epub` command are also found here.
 
 ### Example
@@ -452,20 +467,22 @@
 If you have a lot of followed series and update often, the flag `--use-events` can be used. In that case, the `update` command will first check the events feed provided by J-Novel Club: It includes all the part releases and can be used to know which series will need to be downloaded. With this flag, the tool saves time by not checking all the series individually.
 
 ### Configuration & environment variables
 
 Compared to the `epub` command, the `update` command understands the additional configuration options:
 - USE_EVENTS
 - WHOLE
+- WHOLE_FINAL
 
 Since they are flags, they should have a value like `1`, `true`, `t`, `yes`, `y` or `on` (case insensitive) if set.
 
 They are also available as environment variables:
 - JNCEP_USE_EVENTS
 - JNCEP_WHOLE
+- JNCEP_WHOLE_FINAL
 
 ### Automation
 
 The `update` command can be called in the background from launchd (on macOS) or a scheduled task (on Windows) or cron (on Linux) in order to regularly download new content if available and create EPUBs (for example, once a day). 
 
 There is no notification built in the `jncep update` command but the text output can be combined with other tools to make something suitable. If there are updates, the `jncep update` command outputs something like `2 series sucessfully updated!`, which can be processed by another tool do create a notification.
```

