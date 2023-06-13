# Comparing `tmp/roseingrave-1.0.0.tar.gz` & `tmp/roseingrave-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roseingrave-1.0.0.tar", max compression
+gzip compressed data, was "roseingrave-1.1.0.tar", max compression
```

## Comparing `roseingrave-1.0.0.tar` & `roseingrave-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     4678 2023-02-28 19:40:42.898030 roseingrave-1.0.0/README.md
--rw-r--r--   0        0        0     1764 2023-03-03 17:06:34.612741 roseingrave-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-02-13 23:38:10.970726 roseingrave-1.0.0/src/roseingrave/__init__.py
--rw-r--r--   0        0        0     1334 2023-02-28 19:42:20.370934 roseingrave-1.0.0/src/roseingrave/__main__.py
--rw-r--r--   0        0        0    13798 2023-02-28 19:58:29.167624 roseingrave-1.0.0/src/roseingrave/_input_files.py
--rw-r--r--   0        0        0    23006 2023-02-28 19:42:45.795465 roseingrave-1.0.0/src/roseingrave/_output_files.py
--rw-r--r--   0        0        0    38773 2023-02-28 19:18:25.686554 roseingrave-1.0.0/src/roseingrave/_piece.py
--rw-r--r--   0        0        0     9121 2023-02-20 22:55:46.764123 roseingrave-1.0.0/src/roseingrave/_piece_data.py
--rw-r--r--   0        0        0     7430 2023-02-20 22:55:54.699168 roseingrave-1.0.0/src/roseingrave/_read_write.py
--rw-r--r--   0        0        0      628 2023-02-20 22:55:55.893760 roseingrave-1.0.0/src/roseingrave/_shared.py
--rw-r--r--   0        0        0    11987 2023-02-24 04:49:08.490918 roseingrave-1.0.0/src/roseingrave/_sheets.py
--rw-r--r--   0        0        0     1790 2023-02-20 22:56:00.037587 roseingrave-1.0.0/src/roseingrave/_volunteer.py
--rw-r--r--   0        0        0     2812 2023-02-20 22:56:02.208009 roseingrave-1.0.0/src/roseingrave/compile_pieces.py
--rw-r--r--   0        0        0    14656 2023-02-24 04:52:39.979749 roseingrave-1.0.0/src/roseingrave/create_sheet.py
--rw-r--r--   0        0        0      499 2023-02-13 23:53:20.010579 roseingrave-1.0.0/src/roseingrave/defaults/roseingrave.json
--rw-r--r--   0        0        0      648 2023-02-28 19:40:42.900121 roseingrave-1.0.0/src/roseingrave/defaults/template_definitions.json
--rw-r--r--   0        0        0     5904 2023-02-28 19:42:57.834374 roseingrave-1.0.0/src/roseingrave/export_summary.py
--rw-r--r--   0        0        0     3507 2023-02-20 22:56:04.400694 roseingrave-1.0.0/src/roseingrave/fix_input.py
--rw-r--r--   0        0        0     5063 2023-02-28 19:43:09.573280 roseingrave-1.0.0/src/roseingrave/import_summary.py
--rw-r--r--   0        0        0     5092 2023-02-20 22:56:06.534509 roseingrave-1.0.0/src/roseingrave/piece_summary.py
--rw-r--r--   0        0        0      603 2023-02-20 22:56:08.453134 roseingrave-1.0.0/src/roseingrave/reauth.py
--rw-r--r--   0        0        0     6611 2023-02-20 22:59:50.732097 roseingrave-1.0.0/src/roseingrave/volunteer_summary.py
--rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 roseingrave-1.0.0/setup.py
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 roseingrave-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4678 2023-02-28 19:40:42.898030 roseingrave-1.1.0/README.md
+-rw-r--r--   0        0        0     1764 2023-06-13 17:52:21.439858 roseingrave-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-02-13 23:38:10.970726 roseingrave-1.1.0/src/roseingrave/__init__.py
+-rw-r--r--   0        0        0     1508 2023-06-13 17:56:39.059641 roseingrave-1.1.0/src/roseingrave/__main__.py
+-rw-r--r--   0        0        0      127 2023-06-13 17:57:39.136039 roseingrave-1.1.0/src/roseingrave/__version__.py
+-rw-r--r--   0        0        0    13992 2023-03-07 21:41:22.248834 roseingrave-1.1.0/src/roseingrave/_input_files.py
+-rw-r--r--   0        0        0    23006 2023-02-28 19:42:45.795465 roseingrave-1.1.0/src/roseingrave/_output_files.py
+-rw-r--r--   0        0        0    39138 2023-06-13 17:46:48.646814 roseingrave-1.1.0/src/roseingrave/_piece.py
+-rw-r--r--   0        0        0     9121 2023-02-20 22:55:46.764123 roseingrave-1.1.0/src/roseingrave/_piece_data.py
+-rw-r--r--   0        0        0     7430 2023-02-20 22:55:54.699168 roseingrave-1.1.0/src/roseingrave/_read_write.py
+-rw-r--r--   0        0        0      628 2023-02-20 22:55:55.893760 roseingrave-1.1.0/src/roseingrave/_shared.py
+-rw-r--r--   0        0        0    11987 2023-02-24 04:49:08.490918 roseingrave-1.1.0/src/roseingrave/_sheets.py
+-rw-r--r--   0        0        0     1790 2023-02-20 22:56:00.037587 roseingrave-1.1.0/src/roseingrave/_volunteer.py
+-rw-r--r--   0        0        0     2812 2023-02-20 22:56:02.208009 roseingrave-1.1.0/src/roseingrave/compile_pieces.py
+-rw-r--r--   0        0        0    14711 2023-06-13 16:51:46.961767 roseingrave-1.1.0/src/roseingrave/create_sheet.py
+-rw-r--r--   0        0        0      499 2023-02-13 23:53:20.010579 roseingrave-1.1.0/src/roseingrave/defaults/roseingrave.json
+-rw-r--r--   0        0        0      679 2023-03-07 21:34:59.119134 roseingrave-1.1.0/src/roseingrave/defaults/template_definitions.json
+-rw-r--r--   0        0        0     5904 2023-02-28 19:42:57.834374 roseingrave-1.1.0/src/roseingrave/export_summary.py
+-rw-r--r--   0        0        0     3507 2023-02-20 22:56:04.400694 roseingrave-1.1.0/src/roseingrave/fix_input.py
+-rw-r--r--   0        0        0     5063 2023-02-28 19:43:09.573280 roseingrave-1.1.0/src/roseingrave/import_summary.py
+-rw-r--r--   0        0        0     5092 2023-02-20 22:56:06.534509 roseingrave-1.1.0/src/roseingrave/piece_summary.py
+-rw-r--r--   0        0        0      603 2023-02-20 22:56:08.453134 roseingrave-1.1.0/src/roseingrave/reauth.py
+-rw-r--r--   0        0        0     6611 2023-02-20 22:59:50.732097 roseingrave-1.1.0/src/roseingrave/volunteer_summary.py
+-rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 roseingrave-1.1.0/setup.py
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 roseingrave-1.1.0/PKG-INFO
```

### Comparing `roseingrave-1.0.0/README.md` & `roseingrave-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/pyproject.toml` & `roseingrave-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = [
   "digital humanities",
 ]
 license = "LGPL-3.0-or-later"
 name = "roseingrave"
 readme = "README.md"
 repository = "https://github.com/scarlatti/roseingrave"
-version = "1.0.0"
+version = "1.1.0"
 
 [tool.poetry.scripts]
 roseingrave = "roseingrave.__main__:cli"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
```

### Comparing `roseingrave-1.0.0/src/roseingrave/__main__.py` & `roseingrave-1.1.0/src/roseingrave/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 The command-line interface for Roseingrave.
 """
 
 # ======================================================================
 
 import click
 
+from .__version__ import __version__
 from .compile_pieces import compile_pieces
 from .create_sheet import create_sheet
 from .export_summary import export_summary
 from .fix_input import fix_input
 from .import_summary import import_summary
 from .piece_summary import piece_summary
 from .reauth import reauth
@@ -42,10 +43,15 @@
         piece_summary,
         compile_pieces,
         import_summary,
         export_summary,
     ],
     help="Massively scalable musical source comparator",
 )
+cli = click.version_option(
+    version=__version__,
+    package_name="roseingrave",
+    message="%(prog)s, version %(version)s",
+)(cli)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `roseingrave-1.0.0/src/roseingrave/_input_files.py` & `roseingrave-1.1.0/src/roseingrave/_input_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,18 @@
     if values["values"]["defaultBarCount"] <= 0:
         invalid = True
         _error('"values"."defaultBarCount": must be positive')
     # comments row height must be at least 21
     if values["values"]["commentsRowHeight"] < 21:
         invalid = True
         _error('"values"."commentsRowHeight": must be at least 21')
+    # sources column width must be at least 100
+    if values["values"]["sourcesColumnWidth"] < 100:
+        invalid = True
+        _error('"values"."sourcesColumnWidth": must be at least 100')
 
     if invalid:
         return ERROR_RETURN
     if strict and warning:
         fail_on_warning()
         return ERROR_RETURN
```

### Comparing `roseingrave-1.0.0/src/roseingrave/_output_files.py` & `roseingrave-1.1.0/src/roseingrave/_output_files.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/_piece.py` & `roseingrave-1.1.0/src/roseingrave/_piece.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,19 +349,20 @@
             row_index += 1
             if row_index == wrap_row:
                 # wrap back to top
                 row_index = start_row
 
         return True
 
-    def create_sheet(self, spreadsheet):
+    def create_sheet(self, spreadsheet, volunteer_email):
         """Create a sheet for this piece.
 
         Args:
             spreadsheet (gspread.Spreadsheet): The parent spreadsheet.
+            volunteer_email (str): The volunteer's email.
 
         Returns:
             gspread.Worksheet: The created sheet.
         """
 
         if self._template is None:
             raise RuntimeError(
@@ -418,14 +419,15 @@
             spreadsheet,
             sheet,
             self._template,
             notes_col,
             blank_row1,
             blank_row2,
             comments_row,
+            volunteer_email=volunteer_email,
             resize=resize,
             has_supplemental_col=has_supplemental_col,
         )
 
         if resize:
             start = f"A{blank_row1}"
             end = f"{_col_str(notes_col - 1)}{blank_row1}"
@@ -553,15 +555,14 @@
             sheet,
             self._template,
             notes_col,
             blank_row1,
             blank_row2,
             comments_row,
             resize=resize,
-            is_summary=True,
             source_cols=source_cols,
             has_supplemental_col=has_supplemental_col,
         )
 
         if resize:
             sheet.batch_clear([f"A{blank_row1}"])
 
@@ -756,22 +757,23 @@
     spreadsheet,
     sheet,
     template,
     notes_col,
     blank_row1,
     blank_row2,
     comments_row,
+    volunteer_email=None,
     resize=False,
-    is_summary=False,
     source_cols=None,
     has_supplemental_col=False,
 ):
     """Format a piece sheet."""
 
     sheet_id = sheet.id
+    is_summary = volunteer_email is None
 
     def hex_to_rgb(hex_color):
         """Changes a hex color code (no pound) to an RGB color dict.
         Each value is a fraction decimal instead of an integer.
         """
         colors = ("red", "green", "blue")
         return {
@@ -979,21 +981,22 @@
                 }
             }
         )
 
     column_widths = []
     if not resize:
         column_widths.append(
-            # column 1: width 200
-            ({"startIndex": 0, "endIndex": 1}, 200),
+            # column 1: width 285
+            ({"startIndex": 0, "endIndex": 1}, 285),
         )
     if is_summary or not resize:
+        sources_width = template["values"]["sourcesColumnWidth"]
         column_widths.append(
-            # source columns: width 150
-            ({"startIndex": 1, "endIndex": notes_col - 1}, 150),
+            # source columns
+            ({"startIndex": 1, "endIndex": notes_col - 1}, sources_width),
         )
     column_widths.append(
         # notes col: width 300
         ({"startIndex": notes_col - 1, "endIndex": notes_col}, 300),
     )
     if has_supplemental_col:
         column_widths.append(
@@ -1182,24 +1185,28 @@
         start_row = row
         last_row = row
     if start_row is not None:
         no_auto_number_format(start_row, last_row)
 
     # protect the first row and column of non-summary sheets
     if not is_summary:
-        # get owner of spreadsheet
-        owner = None
+        # find all editors except for volunteer
+        editors = []
         for user in spreadsheet.list_permissions():
-            if user["role"] == "owner":
-                owner = user["emailAddress"]
-                break
-        if owner is None:
+            if user["role"] not in ("owner", "writer"):
+                continue
+            email = user["emailAddress"]
+            if email == volunteer_email:
+                continue
+            editors.append(email)
+        if len(editors) == 0:
             # likely will never happen
             logger.error(
-                'Could not find owner of spreadsheet "{}"', spreadsheet.title
+                'No editors found for protected range of spreadsheet "{}"',
+                spreadsheet.title,
             )
         else:
             requests.append(
                 {
                     "addProtectedRange": {
                         "protectedRange": {
                             # protect entire sheet
@@ -1210,15 +1217,15 @@
                                 {
                                     # exclude where the volunteer will edit
                                     "sheetId": sheet_id,
                                     "startRowIndex": header_end,
                                     "startColumnIndex": 1,
                                 },
                             ],
-                            "editors": {"users": [owner]},
+                            "editors": {"users": editors},
                         }
                     }
                 }
             )
 
     if len(requests) > 0:
         body = {"requests": requests}
```

### Comparing `roseingrave-1.0.0/src/roseingrave/_piece_data.py` & `roseingrave-1.1.0/src/roseingrave/_piece_data.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/_read_write.py` & `roseingrave-1.1.0/src/roseingrave/_read_write.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/_shared.py` & `roseingrave-1.1.0/src/roseingrave/_shared.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/_sheets.py` & `roseingrave-1.1.0/src/roseingrave/_sheets.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/_volunteer.py` & `roseingrave-1.1.0/src/roseingrave/_volunteer.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/compile_pieces.py` & `roseingrave-1.1.0/src/roseingrave/compile_pieces.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/create_sheet.py` & `roseingrave-1.1.0/src/roseingrave/create_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,17 @@
                 worksheets_in_piece_order.append(existing_sheets[piece_name])
                 logger.debug(
                     'Skipping piece "{}": already exists in sheet', piece_name
                 )
                 continue
             if piece_name not in sheets:
                 logger.debug('Creating sheet for piece "{}"', piece_name)
-                sheet = pieces[piece_name].create_sheet(spreadsheet)
+                sheet = pieces[piece_name].create_sheet(
+                    spreadsheet, volunteer.email
+                )
                 sheets[piece_name] = sheet
             else:
                 # copy from previously created
                 logger.debug('Copying sheet for piece "{}"', piece_name)
                 data = sheets[piece_name].copy_to(spreadsheet.id)
                 # update sheet title to piece name
                 sheet = spreadsheet.get_worksheet_by_id(data["sheetId"])
```

### Comparing `roseingrave-1.0.0/src/roseingrave/export_summary.py` & `roseingrave-1.1.0/src/roseingrave/export_summary.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/fix_input.py` & `roseingrave-1.1.0/src/roseingrave/fix_input.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/import_summary.py` & `roseingrave-1.1.0/src/roseingrave/import_summary.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/piece_summary.py` & `roseingrave-1.1.0/src/roseingrave/piece_summary.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/reauth.py` & `roseingrave-1.1.0/src/roseingrave/reauth.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/src/roseingrave/volunteer_summary.py` & `roseingrave-1.1.0/src/roseingrave/volunteer_summary.py`

 * *Files identical despite different names*

### Comparing `roseingrave-1.0.0/setup.py` & `roseingrave-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'urllib3==1.26.9']
 
 entry_points = \
 {'console_scripts': ['roseingrave = roseingrave.__main__:cli']}
 
 setup_kwargs = {
     'name': 'roseingrave',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'A massively scalable document source comparator, using Google Spreadsheets API + Python.',
     'long_description': '# Roseingrave\n\nMassively scalable musical source comparator.\n\nSee the\n[documentation](https://github.com/scarlatti/roseingrave/blob/main/Documentation.md)\nfor detailed documentation.\n\n## Installation\n\nInstall the package through pip (recommended to do in a virtual environment):\n\n```bash\n$ python3 -m pip install roseingrave\n```\n\nThe package will be added as a top-level command:\n\n```bash\n$ roseingrave --help\n```\n\nCreate a folder to store all your input/output files. In this folder, place your\nOAuth credentials file (see\n[Credentials](https://github.com/scarlatti/roseingrave#credentials))\nand all required and optional input files.\n\nSee the\n[documentation](https://github.com/scarlatti/roseingrave/blob/main/Documentation.md)\nfor customizing filepaths and the expected input file formats.\n\n## Credentials\n\nThe package interacts with Google Sheets through the\n[`gspread` package](https://docs.gspread.org/en/latest/).\nYou can enable an OAuth Client to create, access, and edit spreadsheets with\nyour email.\n\nTo enable the OAuth Client, follow these steps:\n\n1. Go to the [Google Developers Console](https://console.cloud.google.com/).\n2. Log in with the email account you want to use with the OAuth Client. All\n   created spreadsheets will be owned by this account in Google Drive.\n3. Create a new project.\n4. Go to the [API Library](https://console.cloud.google.com/apis/library).\n5. In the search bar, search for "Google Drive API", select it, and enable it.\n6. Go back to the API library. In the search bar, search for "Google Sheets\n   API", select it, and enable it.\n7. Go to the\n   [OAuth Consent Screen](https://console.cloud.google.com/apis/credentials/consent)\n   tab.\n8. If prompted, select "External" for the User Type.\n9. On the "App Information" page, enter an app name. Select your email address\n   for the support email. Scroll down to the bottom and enter your email address\n   for the developer contact information. Click "Save and Continue".\n10. On the "Scopes" page, click "Save and Continue".\n11. On the "Test Users" page, add your email address as a user. Click "Save and\n    Continue".\n12. On the summary page, scroll to the bottom and click "Back to Dashboard".\n13. Go to the [Credentials](https://console.cloud.google.com/apis/credentials)\n    tab.\n14. At the top of the page, select "+ Create credentials" > "OAuth client ID".\n15. For the application type, select "Desktop app". Name your credentials.\n    Click "Create". Click "Ok" at the popup.\n16. In the table labeled "OAuth 2.0 Client IDs", locate the credentials you just\n    created. Click the download button at the end of the row.\n17. Rename the file to `credentials.json` and place it in the root directory of\n    where you\'ll be running the commands. (You can customize this in the\n    [settings](https://github.com/scarlatti/roseingrave/blob/main/Documentation.md#settings-optional)\n    file).\n\nIf you\'ve never authorized the app or if your authorization has expired, you\'ll\nbe given a link in the console for you to visit in order to refresh or create\nan authorization token. Go to the url, select your email, click "Continue",\nallow access to your Drive files and Sheets spreadsheets, and click "Continue".\nThis should authenticate you, and the command should continue running.\n\nOnce the authorization is successful, the `authorized_user.json` file will be\ncreated in the same directory as `"credentials"`.\n\n## Basic Usage\n\nCreate the piece definitions and volunteer definitions files as explained in the\n[documentation](https://github.com/scarlatti/roseingrave/blob/main/Documentation.md#input-files).\nIf desired, create the settings file and/or the template file. Save all the\nfiles in the proper locations as defined by the\n[default settings file](https://github.com/scarlatti/roseingrave/blob/main/src/roseingrave/defaults/roseingrave.json)\nor by your own settings file.\n\nBased on your definition files, create the volunteer spreadsheets:\n\n```bash\n$ roseingrave create_sheet\n```\n\nAfter volunteers have filled out their spreadsheets, export the data:\n\n```bash\n$ roseingrave volunteer_summary\n```\n\nExtract the data for each piece:\n\n```bash\n$ roseingrave piece_summary\n```\n\nCompile all the piece data into the summary file:\n\n```bash\n$ roseingrave compile_pieces\n```\n\nCreate the summary spreadsheet with the data from the summary file:\n\n```bash\n$ roseingrave import_summary\n```\n\nFill out the summary columns as appropriate, then export the summary spreadsheet\ninto the summary file:\n\n```bash\n$ roseingrave export_summary\n```\n\nSee the\n[commands documentation](https://github.com/scarlatti/roseingrave/blob/main/Documentation.md#commands)\nfor all commands and their arguments and options.\n',
     'author': 'Joseph Lou',
     'author_email': 'jdlou@princeton.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/scarlatti/roseingrave',
```

### Comparing `roseingrave-1.0.0/PKG-INFO` & `roseingrave-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roseingrave
-Version: 1.0.0
+Version: 1.1.0
 Summary: A massively scalable document source comparator, using Google Spreadsheets API + Python.
 Home-page: https://github.com/scarlatti/roseingrave
 License: LGPL-3.0-or-later
 Keywords: digital humanities
 Author: Joseph Lou
 Author-email: jdlou@princeton.edu
 Requires-Python: >=3.9,<4.0
```

