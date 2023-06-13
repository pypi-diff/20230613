# Comparing `tmp/rdf_doctor-0.8.1-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,14 @@
-Zip file size: 38559 bytes, number of entries: 29
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 06:47 doctor/__init__.py
+Zip file size: 17606 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-13 05:40 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jun-05 08:08 doctor/consts.py
--rw-r--r--  2.0 unx    26669 b- defN 23-Jun-06 06:47 doctor/doctor.py
+-rw-r--r--  2.0 unx    27880 b- defN 23-Jun-09 07:04 doctor/doctor.py
 -rw-r--r--  2.0 unx    20305 b- defN 23-Jun-05 06:43 doctor/reference/correct-prefixes.tsv
--rw-r--r--  2.0 unx    36944 b- defN 23-Jun-05 06:43 doctor/reference/rdf-config-prefixes.tsv
--rw-r--r--  2.0 unx    21257 b- defN 23-Jun-05 06:43 doctor/reference/rdf-config-prefixes.yaml
--rw-r--r--  2.0 unx       90 b- defN 23-Jun-05 06:43 doctor/reference/refine-classes.tsv
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-13 05:09 doctor/reference/refine-classes.tsv
 -rw-r--r--  2.0 unx      679 b- defN 23-Jun-05 06:43 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 06:43 tests/__init__.py
--rw-r--r--  2.0 unx      754 b- defN 23-Jun-05 06:43 tests/consts.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jun-05 06:43 tests/test_fingerprint.py
--rw-r--r--  2.0 unx     2444 b- defN 23-Jun-05 06:43 tests/test_get_class_comparison_result.py
--rw-r--r--  2.0 unx     2335 b- defN 23-Jun-05 06:43 tests/test_get_command_line_args.py
--rw-r--r--  2.0 unx      765 b- defN 23-Jun-05 06:43 tests/test_get_compression_mode.py
--rw-r--r--  2.0 unx     3256 b- defN 23-Jun-05 06:43 tests/test_get_fingerprint_comparison_result.py
--rw-r--r--  2.0 unx     3249 b- defN 23-Jun-05 06:43 tests/test_get_input_classes.py
--rw-r--r--  2.0 unx      745 b- defN 23-Jun-05 06:43 tests/test_get_input_format.py
--rw-r--r--  2.0 unx     2617 b- defN 23-Jun-05 06:43 tests/test_get_input_prefixes.py
--rw-r--r--  2.0 unx     2831 b- defN 23-Jun-05 06:43 tests/test_get_markdown_result.py
--rw-r--r--  2.0 unx      964 b- defN 23-Jun-05 06:43 tests/test_get_prefix_comparison_result.py
--rw-r--r--  2.0 unx     1396 b- defN 23-Jun-05 06:43 tests/test_get_prefix_reuse_percentage.py
--rw-r--r--  2.0 unx     4936 b- defN 23-Jun-05 06:43 tests/test_get_suggested_qname.py
--rw-r--r--  2.0 unx    15594 b- defN 23-Jun-05 06:43 tests/test_validate_command_line_args.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6694 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-06 06:53 rdf_doctor-0.8.1.dist-info/RECORD
-29 files, 159889 bytes uncompressed, 34429 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8789 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-13 05:44 rdf_doctor-0.8.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-13 05:44 rdf_doctor-0.8.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/RECORD
+12 files, 60602 bytes uncompressed, 15922 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -6,83 +6,32 @@
 
 Filename: doctor/doctor.py
 Comment: 
 
 Filename: doctor/reference/correct-prefixes.tsv
 Comment: 
 
-Filename: doctor/reference/rdf-config-prefixes.tsv
-Comment: 
-
-Filename: doctor/reference/rdf-config-prefixes.yaml
-Comment: 
-
 Filename: doctor/reference/refine-classes.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefixes.tsv
 Comment: 
 
-Filename: tests/__init__.py
-Comment: 
-
-Filename: tests/consts.py
-Comment: 
-
-Filename: tests/test_fingerprint.py
-Comment: 
-
-Filename: tests/test_get_class_comparison_result.py
-Comment: 
-
-Filename: tests/test_get_command_line_args.py
-Comment: 
-
-Filename: tests/test_get_compression_mode.py
-Comment: 
-
-Filename: tests/test_get_fingerprint_comparison_result.py
-Comment: 
-
-Filename: tests/test_get_input_classes.py
-Comment: 
-
-Filename: tests/test_get_input_format.py
-Comment: 
-
-Filename: tests/test_get_input_prefixes.py
-Comment: 
-
-Filename: tests/test_get_markdown_result.py
-Comment: 
-
-Filename: tests/test_get_prefix_comparison_result.py
-Comment: 
-
-Filename: tests/test_get_prefix_reuse_percentage.py
-Comment: 
-
-Filename: tests/test_get_suggested_qname.py
-Comment: 
-
-Filename: tests/test_validate_command_line_args.py
-Comment: 
-
-Filename: rdf_doctor-0.8.1.dist-info/LICENSE
+Filename: rdf_doctor-0.8.2.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.8.1.dist-info/METADATA
+Filename: rdf_doctor-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.8.1.dist-info/WHEEL
+Filename: rdf_doctor-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.8.1.dist-info/entry_points.txt
+Filename: rdf_doctor-0.8.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.1.dist-info/top_level.txt
+Filename: rdf_doctor-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.1.dist-info/RECORD
+Filename: rdf_doctor-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.8.1"
+__version__ = "0.8.2"
```

## doctor/doctor.py

```diff
@@ -33,16 +33,15 @@
         # Processing branch by report format
         if args.report == REPORT_FORMAT_SHEX:
             # shex
             output_result = get_shex_result(args, input_format, compression_mode)
 
         elif args.report == REPORT_FORMAT_MARKDOWN or args.report == REPORT_FORMAT_MD:
             # markdown/md
-            for input_file in args.input:
-                output_result.extend(get_markdown_result(input_file, input_format, compression_mode, args.classes, args.prefix_dict, args.class_dict))
+            output_result = get_markdown_result(args, input_format, compression_mode)
 
         else:
             # Else case does not occur.
             # Prevented by validate_command_line_args function.
             raise ValueError(args.report + '" is an unsupported report format. "' + REPORT_FORMAT_SHEX + '" and "' + REPORT_FORMAT_MD+ '"(same as "' + REPORT_FORMAT_MARKDOWN + '") are supported.')
 
         # Output result to specified destination (standard output or file)
@@ -241,48 +240,62 @@
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_format, compression_mode):
 
     # Get Prefix when input file is turtle format
     if input_format == TURTLE:
-        input_prefixes = get_input_prefixes_from_multi_files(args.input, compression_mode)
+        input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
     else:
         input_prefixes = []
+        duplicated_prefixes = []
 
     shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
 
+    # Prefixes with the same QName but different URIs at the same time
+    result_duplicated_prefixes = []
+    if len(duplicated_prefixes) != 0:
+        result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
+        result_duplicated_prefixes.append("\n")
+        result_duplicated_prefixes.append("# Input QName\tURI\n")
+        result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
+        result_duplicated_prefixes.append("\n\n")
+
     # Suggest QName based on URI of validation expression output by sheXer and correct-prefixes.tsv
     result_suggested_qname = []
     correct_prefixes = get_correct_prefixes()
     suggested_qname = get_suggested_qname(shaper_result, input_prefixes, correct_prefixes)
     if len(suggested_qname) != 0:
         result_suggested_qname.append("# There may be a better QName.\n\n")
         result_suggested_qname.append("# Input QName\tSuggested QName\tURI\n")
         result_suggested_qname.extend(["# " + s for s in suggested_qname])
         result_suggested_qname.append("\n")
 
     # List for storing the final result
     shex_final_result = []
     shex_final_result.extend(shaper_result)
+    if len(result_duplicated_prefixes) != 0:
+        shex_final_result.extend(result_duplicated_prefixes)
+
     if len(result_suggested_qname) != 0:
         shex_final_result.extend(result_suggested_qname)
 
     return shex_final_result
 
 
 # Processing when the report format is "md/markdown"
-def get_markdown_result(input_file, input_format, compression_mode, classes, prefix_dict, class_dict):
+def get_markdown_result(args, input_format, compression_mode):
 
     # Processing related to prefixes ------------------
     # Get Prefix when input file is turtle format
     if input_format == TURTLE:
-        input_prefixes = get_input_prefixes(input_file, compression_mode)
+        input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
     else:
         input_prefixes = []
+        duplicated_prefixes = []
 
     # Get list for result output about prefix reuse rate
     result_prefix_reuse_percentage = []
     result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
     result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
     prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes)
     if prefix_reuse_percentage == None:
@@ -292,31 +305,39 @@
     else:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
         result_prefix_reuse_percentage.append("```\n\n")
 
     # Refer to the errata of prefixes and obtain a list for result output that combines incorrect prefixes and correct prefixes
     result_prefix_errata = []
-    prefix_comparison_result = get_prefix_comparison_result(input_prefixes, prefix_dict)
+    prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
     # When there is data to output
     if len(prefix_comparison_result) != 0:
         result_prefix_errata.append("Found prefixes that looks incorrect.\n")
         result_prefix_errata.append("```\n")
         result_prefix_errata.append("Prefix\tInput URI\tSuggested URI\n")
         result_prefix_errata.extend(prefix_comparison_result)
         result_prefix_errata.append("```\n\n")
+
+    result_duplicated_prefixes = []
+    if len(duplicated_prefixes) != 0:
+        result_duplicated_prefixes.append("Duplicate prefixes found.\n")
+        result_duplicated_prefixes.append("```\n")
+        result_duplicated_prefixes.append("Input QName\tURI\n")
+        result_duplicated_prefixes.extend([s for s in duplicated_prefixes])
+        result_duplicated_prefixes.append("```\n\n")
     # -------------------------------------------------
 
     # Processing related to classes -------------------
-    input_classes = get_input_classes(input_file, input_format, compression_mode, classes)
+    input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
 
     # Refers to the errata list of the class, acquires the list for result output that combines the incorrect class and the correct class,
     # and returns the class corresponding to each key in fingerprint format stored in dictionary format.
     result_class_errata = []
-    class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, defaultdict(list), class_dict)
+    class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
     # When there is data to output
     if len(class_comparison_result) != 0:
         result_class_errata.append("Found class names that looks incorrect.\n")
         result_class_errata.append("```\n")
         result_class_errata.append("Input class name\tSuggested class name\n")
         result_class_errata.extend(class_comparison_result)
         result_class_errata.append("```\n\n")
@@ -331,23 +352,29 @@
         result_class_fingerprint.extend(fingerprint_comparison_result)
         result_class_fingerprint.append("\n```\n\n")
     # -------------------------------------------------
 
     # List for storing the final result
     md_final_result = []
 
-    md_final_result.append("# Report on " + os.path.basename(input_file) + "\n\n")
+    md_final_result.append("# Report on\n")
+    md_final_result.append("```\n")
+    for input_file in args.input:
+        md_final_result.append(os.path.basename(input_file) + "\n")
+
+    md_final_result.append("```\n\n")
 
     # Merge result
     md_final_result.extend(result_prefix_reuse_percentage)
 
     prefix_result_exists = len(result_prefix_errata) != 0
     if prefix_result_exists:
         md_final_result.append("## Refine prefixes ([?](" + HELP_LINK_URL + "))\n")
         md_final_result.extend(result_prefix_errata)
+        md_final_result.extend(result_duplicated_prefixes)
 
     class_result_exists = len(result_class_errata) != 0 or len(result_class_fingerprint) != 0
     if class_result_exists:
         md_final_result.append("## Refine classes ([?](" + HELP_LINK_URL + "))\n")
         md_final_result.extend(result_class_errata)
         md_final_result.extend(result_class_fingerprint)
 
@@ -405,45 +432,48 @@
                     correct_count+=1
                     break
 
         prefix_reuse_percentage = round(correct_count / input_prefixes_count * 100, 2)
         return prefix_reuse_percentage
 
 
-# Get the classes contained within the input file
-def get_input_classes(input_file, input_format, compression_mode, target_classes):
-    g = rdflib.Graph()
+# Get the classes contained within the input file(s)
+def get_input_classes(input_files, input_format, compression_mode, target_classes):
 
-    if compression_mode != None:
-        with gzip.open(input_file, "rb") as f:
-            data = f.read()
-        g.parse(data=data, format=input_format)
-    else:
-        g.parse(input_file, format=input_format)
+    input_classes = []
+    for input_file in input_files:
+        g = rdflib.Graph()
 
-    # Filter by classes(command line arguments)
-    class_filter = ",".join(target_classes)
+        if compression_mode != None:
+            with gzip.open(input_file, "rb") as f:
+                data = f.read()
+            g.parse(data=data, format=input_format)
+        else:
+            g.parse(input_file, format=input_format)
 
-    query = """
-        SELECT DISTINCT ?class_name
-        WHERE {
-            [] a ?class_name .
-            FILTER(! isBlank(?class_name))
-    """
-    if TARGET_CLASS_ALL not in target_classes:
-        query += " FILTER (?class_name IN (" + class_filter + "))"
-
-    query += """
-        }
-    """
+        # Filter by classes(command line arguments)
+        class_filter = ",".join(target_classes)
 
-    input_classes = []
-    qres = g.query(query)
-    for row in qres:
-        input_classes.append(f"{row.class_name}")
+        query = """
+            SELECT DISTINCT ?class_name
+            WHERE {
+                [] a ?class_name .
+                FILTER(! isBlank(?class_name))
+        """
+        if TARGET_CLASS_ALL not in target_classes:
+            query += " FILTER (?class_name IN (" + class_filter + "))"
+
+        query += """
+            }
+        """
+
+        qres = g.query(query)
+        for row in qres:
+            if f"{row.class_name}" not in input_classes:
+                input_classes.append(f"{row.class_name}")
 
     return input_classes
 
 
 # Return class errata in a two-dimensional array
 def get_class_errata(class_errata_file):
     with open(class_errata_file, mode="r", newline="\n", encoding="utf-8") as f:
@@ -461,18 +491,18 @@
 
     return prefix_errata
 
 
 # Get a combined list of incorrect and correct classes obtained by referencing the class errata list.
 # Create a dictionary with a class corresponding to each key in the stored fingerprint format.
 # Return the two.
-def get_class_comparison_result(input_classes, fingerprint_class_dict, class_errata_file):
+def get_class_comparison_result(input_classes, class_errata_file):
     class_errata = get_class_errata(class_errata_file)
     class_comparison_result = []
-
+    fingerprint_class_dict = defaultdict(list)
     # Perform clustering by fingerprint for the acquired class name
     for input_class in input_classes:
         fingerprint_class_dict[fingerprint(input_class)].append(input_class)
         for eratta in class_errata:
             if input_class == eratta[0]:
                 class_comparison_result.append(input_class+"\t"+eratta[1]+"\n")
                 break
@@ -505,38 +535,20 @@
                 fingerprint_comparison_result.append("\n")
             for v in value:
                 fingerprint_comparison_result.append("\n"+v)
 
     return fingerprint_comparison_result
 
 
-# Get the prefixes contained within the input file (from single file)
-def get_input_prefixes(input_file, compression_mode):
-    if compression_mode != None:
-        with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
-            data = f.read().splitlines()
-    else:
-        with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
-            data = f.read().splitlines()
-
-    input_prefixes = []
-    for line in data:
-        if ("@prefix" in line or "@PREFIX" in line):
-            line_mod = line.replace("@prefix", "").replace("@PREFIX", "").replace(" ", "").replace("\t","")
-            qname = line_mod[:line_mod.find(":")+1]
-            uri = line_mod[line_mod.find("<")+1:line_mod.find(">")]
-            if [qname, uri] not in input_prefixes:
-                input_prefixes.append([qname, uri])
-
-    return input_prefixes
-
-
-# Get the prefixes contained within the input files (from mauti files)
-def get_input_prefixes_from_multi_files(input_files, compression_mode):
+# Get the prefixes contained within the input file(s)
+# And get prefixes with the same QName but different URIs at the same time.
+def get_input_prefixes(input_files, compression_mode):
     input_prefixes = []
+    duplicated_qnames = []
+    duplicated_prefixes_dict = defaultdict(list)
     for input_file in input_files:
         if compression_mode != None:
             with gzip.open(input_file, mode="rt", encoding="utf-8") as f:
                 data = f.read().splitlines()
         else:
             with open(input_file, mode="r", newline="\n", encoding="utf-8") as f:
                 data = f.read().splitlines()
@@ -544,16 +556,28 @@
         for line in data:
             if ("@prefix" in line or "@PREFIX" in line):
                 line_mod = line.replace("@prefix", "").replace("@PREFIX", "").replace(" ", "").replace("\t","")
                 qname = line_mod[:line_mod.find(":")+1]
                 uri = line_mod[line_mod.find("<")+1:line_mod.find(">")]
                 if [qname, uri] not in input_prefixes:
                     input_prefixes.append([qname, uri])
+                    for input_prefix in input_prefixes:
+                        if input_prefix[0] == qname and input_prefix[1] != uri and qname not in duplicated_qnames:
+                            duplicated_qnames.append(qname)
+
+    for input_prefix in input_prefixes:
+        if input_prefix[0] in duplicated_qnames:
+            duplicated_prefixes_dict[fingerprint(input_prefix[0])].append(input_prefix[1])
+
+    duplicated_prefixes_list = []
+    for key, values in duplicated_prefixes_dict.items():
+        for value in values:
+            duplicated_prefixes_list.append(key + ":\t" + value + "\n")
 
-    return input_prefixes
+    return input_prefixes, duplicated_prefixes_list
 
 
 # Get the correct prefix from a prepared prefix list
 def get_correct_prefixes():
     with open(Path(__file__).resolve().parent.joinpath(CORRECT_PREFIXES_FILE_PATH), mode="r", newline="\n", encoding="utf-8") as f:
         tsv_reader = csv.reader(f, delimiter="\t")
         correct_prefixes = [row for row in tsv_reader]
```

## Comparing `rdf_doctor-0.8.1.dist-info/LICENSE` & `rdf_doctor-0.8.2.dist-info/LICENSE`

 * *Files identical despite different names*

