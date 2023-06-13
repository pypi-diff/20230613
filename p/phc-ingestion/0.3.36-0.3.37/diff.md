# Comparing `tmp/phc-ingestion-0.3.36.tar.gz` & `tmp/phc-ingestion-0.3.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.36.tar", last modified: Thu Jun  8 10:22:06 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.37.tar", last modified: Tue Jun 13 17:21:35 2023, max compression
```

## Comparing `phc-ingestion-0.3.36.tar` & `phc-ingestion-0.3.37.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     2976 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8461 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5664 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1913 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.36/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5907 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3137 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     4949 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8461 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2023-06-13 17:20:48.440342 phc-ingestion-0.3.37/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-13 17:20:48.444342 phc-ingestion-0.3.37/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.37/PKG-INFO
```

### Comparing `phc-ingestion-0.3.36/ingestion/caris/process.py` & `phc-ingestion-0.3.37/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.37/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.37/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.37/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.37/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/json.py` & `phc-ingestion-0.3.37/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.37/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.37/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.37/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.37/ingestion/caris/util/vcf.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     foutW.write('##FILTER=<ID=Benign,Description="Benign variant">\n')
     foutW.write('##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">\n')
     foutW.write(
         '##FORMAT=<ID=AD,Number=R,Type=Integer,Description="Allelic depths for the ref and alt alleles in the order listed">\n'
     )
     foutW.write('##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read depth">\n')
     foutW.write('##INFO=<ID=AF,Number=1,Type=String,Description="Variant Allele Frequency">\n')
+    foutW.write('##INFO=<ID=VENDSIG,Number=1,Type=String,Description="Vendor Significance">\n')
 
     if "germline" in infile:
         sample_name = "germline_" + file_name
     else:
         sample_name = file_name
 
     foutW.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t" + sample_name + "\n")
@@ -128,14 +129,35 @@
         for data in info_field_list:
             if data.split("=")[0] == "DP":
                 depth = data.split("=")[1]
 
         # We need to put this in the proper format for ingestion into omics explore.
         new_sample_field = ":".join([sample_field_list[0], sample_field_list[2], depth])
 
-        vcf_info = f"AF={sample_field_list[1]}"
+        # Retaining the Clinical Impact field
+        ci = re.sub(
+            '"', "", "".join([data for data in info_field_list if data.split("=")[0] == "CI"])
+        )
+        mapped_ci = map_vendsig(ci)
+
+        vcf_info = f"AF={sample_field_list[1]};{mapped_ci}"
 
         foutW.write("\t".join([genomic_record, vcf_info, vcf_format, new_sample_field]) + "\n")
 
     finR.close()
     foutW.close()
     return line_count
+
+
+def map_vendsig(ci: str) -> str:
+    if ci in ["CI=PathogenicVariant", "CI=Pathogenic"]:
+        return "VENDSIG=Pathogenic"
+    elif ci in ["CI=LikelyPathogenicVariant", "CI=Likely_Pathogenic"]:
+        return "VENDSIG=Likely pathogenic"
+    elif ci in ["CI=BenignVariant", "CI=Benign"]:
+        return "VENDSIG=Benign"
+    elif ci in ["CI=LikelyBenignVariant", "CI=Likely_Benign"]:
+        return "VENDSIG=Likely benign"
+    elif ci in ["CI=VariantofUncertainSignificance", "CI=VUS"]:
+        return "VENDSIG=Uncertain significance"
+    else:
+        return "VENDSIG=Unknown"
```

### Comparing `phc-ingestion-0.3.36/ingestion/foundation/process.py` & `phc-ingestion-0.3.37/ingestion/foundation/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         results_payload_dict = xml_dict["rr:ResultsReport"]["rr:ResultsPayload"]
 
         sample_name = get_specimen_name(results_payload_dict)
 
         base_xml_name = Path(xml_file).stem
 
         vcf_name = f"{local_output_dir}/{base_xml_name}/{base_xml_name}.tcf"
-        vcf_line_count = vcf_etl(vcf_file, vcf_name, base_xml_name)
+        vcf_line_count = vcf_etl(vcf_file, vcf_name, base_xml_name, xml_file)
         write_cnv = extract_copy_numbers(results_payload_dict, base_xml_name, local_output_dir, log)
         write_fnv = extract_fusion_variant(
             results_payload_dict, base_xml_name, local_output_dir, log
         )
 
         yaml_file = get_test_yml(
             customer_info_dict,
```

### Comparing `phc-ingestion-0.3.36/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.37/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.37/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.37/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.37/ingestion/foundation/util/vcf_etl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import gzip
+import xmltodict
 from natsort import natsorted
 import re
 import os
 import errno
 
 
-def vcf_etl(in_vcf: str, out_vcf: str, base_xml_name: str) -> int:
+def vcf_etl(in_vcf: str, out_vcf: str, base_xml_name: str, xml_file: str) -> int:
     headers = []
     vars = []
 
+    # Get xml short variant entries for scraping vendsig
+    xml_short_vars = get_xml_short_vars(xml_file)
+
     if not os.path.exists(os.path.dirname(out_vcf)):
         try:
             os.makedirs(os.path.dirname(out_vcf))
         except OSError as exc:
             if exc.errno != errno.EEXIST:
                 raise
 
@@ -37,41 +41,86 @@
 
                     if "#CHROM" in header:
                         w.write('##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read Depth">\n')
                         w.write('##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">\n')
                         w.write(
                             '##FORMAT=<ID=AD,Number=.,Type=Integer,Description="Number of reads harboring allele (in order specified by GT)">\n'
                         )
+                        w.write(
+                            '##INFO=<ID=VENDSIG,Number=1,Type=String,Description="Vendor Significance">\n'
+                        )
                         header = header.strip("\n") + "\tFORMAT\t" + base_xml_name + "\n"
 
                     w.write(header)
 
                 for var in sorted_vars:
                     var = var.replace("af=", "AF=")
                     var = transform_scientific_notation_in_af(var)
+                    untouched_var = "\t".join(var.split("\t")[0:7])
+                    new_vcf_info = add_vendsig_to_info(var, xml_short_vars)
                     af_match = re.search(r"AF=(\d*\.?\d*)", var)
                     if not af_match:
                         raise RuntimeError("Failed to find AF for var")
                     af = float(af_match.group(1))
                     depth_match = re.search(r"depth=(\d*\.?\d*)", var)
                     if not depth_match:
                         raise RuntimeError("Failed to find depth for var")
                     depth = int(depth_match.group(1))
                     alt_depth = int(round(depth * af))
                     ref_depth = depth - alt_depth
                     ad = f"{ref_depth},{alt_depth}"
                     gt = "1/1" if af > 0.9 else "0/1"
                     vcf_format = "GT:DP:AD"
                     sample = ":".join([gt, str(depth), ad])
-                    var = var.strip("\n") + f"\t{vcf_format}\t{sample}\n"
+                    var = untouched_var + f"\t{new_vcf_info}\t{vcf_format}\t{sample}\n"
                     w.write(var)
 
             return line_count
 
 
+def get_xml_short_vars(xml_file: str) -> dict:
+    with open(xml_file) as fd:
+        xml_dict = xmltodict.parse(fd.read())
+    xml_short_vars = xml_dict["rr:ResultsReport"]["rr:ResultsPayload"]["variant-report"][
+        "short-variants"
+    ]["short-variant"]
+    return xml_short_vars
+
+
+def map_vendsig(vendsig: str) -> str:
+    if vendsig in ["known"]:
+        return "VENDSIG=Pathogenic"
+    elif vendsig in ["likely"]:
+        return "VENDSIG=Likely pathogenic"
+    elif vendsig in ["unknown"]:
+        return "VENDSIG=Uncertain significance"
+    else:
+        return "VENDSIG=Unknown"
+
+
+def add_vendsig_to_info(var: str, xml_short_vars: dict) -> str:
+    info = var.split("\t")[7]
+    # using transcript name, find it in xml_short_vars
+    transcript_name = info.split(";")[-1].split("=")[1].strip()
+    # dictionary comprehension to get the short_var in xml_short_vars that matches the transcript_name
+    matched_xml_var = [
+        short_var
+        for short_var in xml_short_vars
+        if short_var.get("@transcript", "") == transcript_name
+    ]
+    if not matched_xml_var:
+        vendsig = "Unknown"
+    else:
+        vendsig = matched_xml_var[0]["@status"]
+
+    mapped_vendsig = map_vendsig(vendsig)
+    new_vcf_info = f"{info.strip()};{mapped_vendsig}"
+    return new_vcf_info
+
+
 def transform_scientific_notation_in_af(var: str) -> str:
     var_split = var.split("\t")
     var_info = var_split[-1]
     var_info_split = var_info.split(";")
     var_info_list = [x for x in var_info_split if x.startswith("AF=")]
 
     # No AF= in line so lets return as is and move on
```

### Comparing `phc-ingestion-0.3.36/ingestion/nextgen/process.py` & `phc-ingestion-0.3.37/ingestion/nextgen/process.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,21 +48,23 @@
             log=log,
         )
         somatic_vcf_meta_data = process_vcf(
             vcf_in_file=vendor_files["somaticVcfFile"],
             root_path=local_output_dir,
             prefix=prefix,
             sequence_type="somatic",
+            xml_in_file=vendor_files["xmlFile"],
             log=log,
         )
         germline_vcf_meta_data = process_vcf(
             vcf_in_file=vendor_files["germlineVcfFile"],
             root_path=local_output_dir,
             prefix=prefix,
             sequence_type="germline",
+            xml_in_file=vendor_files["xmlFile"],
             log=log,
         )
 
     manifest_path_name = f"{local_output_dir}/{prefix}.ga4gh.genomics.yml"
     log.info(f"Saving file to {manifest_path_name}")
     with open(manifest_path_name, "w") as file:
         yaml = YAML()
```

### Comparing `phc-ingestion-0.3.36/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.37/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.37/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.37/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.37/ingestion/nextgen/util/process_vcf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import gzip
 import shutil
 from logging import Logger
+from ingestion.nextgen.util.variant_table import extract_variant_table
 
 
 class Variant:
     def __init__(self, fields):
         self.chr_pos = fields[0]
         self.info = []
         self.frmt = fields[2]
@@ -55,26 +56,40 @@
         zipped = dict(zip(self.frmt, self.smpl))
         frmt_smpl_dict = {frmt: smpl for frmt, smpl in zipped.items() if frmt in ["GT", "AD", "DP"]}
         self.pruned_info = self.info[0]
         self.pruned_frmt = ":".join(list(frmt_smpl_dict.keys()))
         self.pruned_smpl = ":".join(list(frmt_smpl_dict.values()))
 
 
-def transform_vcf(vcf_in_file: str, headers: list, variants: list, sequence_type: str, log: Logger):
+def transform_vcf(
+    vcf_in_file: str,
+    headers: list,
+    variants: list,
+    sequence_type: str,
+    xml_in_file: str,
+    log: Logger,
+):
+    short_variant_table = extract_variant_table(
+        xml_in_file=xml_in_file, variant_type="short", log=log
+    )
+
     log.info(f"Performing file transformations on {vcf_in_file}")
     approved_chr_list = ["chr" + str(i) for i in range(1, 23)] + ["chrX", "chrY", "chrM"]
     vcf_out = []
 
     for header in headers:
         # Add AF/INFO and DP/FORMAT to header if somatic (already in germline headers)
         if "#CHROM" in header and sequence_type == "somatic":
             vcf_out.append(
                 '##INFO=<ID=AF,Number=A,Type=Float,Description="Allele frequency, for each ALT allele, in the same order as listed">'
             )
             vcf_out.append('##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read depth">')
+            vcf_out.append(
+                '##INFO=<ID=VENDSIG,Number=1,Type=String,Description="Vendor Significance">'
+            )
         vcf_out.append(header.strip())
 
     for var in variants:
         split_var = var.split("\t")
         if len(split_var) != 10:
             raise RuntimeError(
                 f"Variant does not contain correct number of fields. Should be 10 when {len(split_var)} were detected: {var}"
@@ -98,30 +113,37 @@
             working.afdp_to_dp()
             working.prune_var()
 
         elif sequence_type == "germline":
             working.calculate_af()
             working.prune_var()
 
-        split_var[7] = working.pruned_info
+        if sequence_type == "somatic" and not short_variant_table.empty:
+            split_var[7] = add_vendsig_to_info(
+                working.pruned_info, short_variant_table, split_var[0], int(split_var[1])
+            )
+        else:
+            split_var[7] = f"{working.pruned_info};VENDSIG=Unknown"
         split_var[8] = working.pruned_frmt
         split_var[9] = working.pruned_smpl
         vcf_out.append("\t".join(split_var))
 
     vcf_out = "\n".join(vcf_out) + "\n"
     return vcf_out
 
 
 def export_vcf(vcf_out: str, vcf_path: str, log: Logger):
     log.info(f"VCF transformation complete. Writing to {vcf_path}")
     with gzip.open(f"{vcf_path}", "wt") as w:
         w.write(vcf_out)
 
 
-def process_vcf(vcf_in_file: str, root_path: str, prefix: str, sequence_type: str, log: Logger):
+def process_vcf(
+    vcf_in_file: str, root_path: str, prefix: str, sequence_type: str, xml_in_file: str, log: Logger
+):
     line_count = 0
     vcf_path = f"{root_path}/{prefix}.modified.{sequence_type}.vcf.gz"
 
     headers = []
     variants = []
 
     with gzip.open(vcf_in_file, "rt") as f:
@@ -143,11 +165,41 @@
             if len(variants) == 0:
                 log.error(f"Input VCF file {vcf_in_file} contains headers but no variants")
                 log.info(f"Copying file to {vcf_path}")
                 shutil.copy(vcf_in_file, vcf_path)
                 return {"vcf_path_name": vcf_path, "vcf_line_count": line_count}
 
             else:
-                vcf_out = transform_vcf(vcf_in_file, headers, variants, sequence_type, log)
+                vcf_out = transform_vcf(
+                    vcf_in_file, headers, variants, sequence_type, xml_in_file, log
+                )
                 export_vcf(vcf_out, vcf_path, log)
 
     return {"vcf_path_name": vcf_path, "vcf_line_count": line_count}
+
+
+def map_vendsig(vendsig: str) -> str:
+    if vendsig in ["Pathogenic"]:
+        return "VENDSIG=Pathogenic"
+    elif vendsig in ["Likely Pathogenic"]:
+        return "VENDSIG=Likely pathogenic"
+    elif vendsig in ["VUS"]:
+        return "VENDSIG=Uncertain significance"
+    else:
+        raise RuntimeError(f"Unable to map vendor significance: {vendsig}")
+
+
+def add_vendsig_to_info(info: str, short_var_table, chrom: str, pos: str) -> str:
+    mapped_vendsig = None
+    for index, row in short_var_table.iterrows():
+        ref_chrom = row["gene"].split(" ")[1].split(":")[0].strip("(")
+        ref_pos = int(row["gene"].split(" ")[1].split(":")[1])
+
+        if ref_chrom == chrom:
+            if ref_pos == pos or ref_pos + 1 == pos or ref_pos - 1 == pos:
+                mapped_vendsig = map_vendsig(row["info"])
+
+    if not mapped_vendsig:
+        mapped_vendsig = "VENDSIG=Unknown"
+
+    new_vcf_info = f"{info.strip()};{mapped_vendsig}"
+    return new_vcf_info
```

### Comparing `phc-ingestion-0.3.36/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.37/ingestion/nextgen/util/variant_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 line = re.sub(r"</T.>", "", line)
                 line = re.sub(r"<T./>", "", line)
                 if line.strip() not in ["", "p."]:
                     variant_lines.append(line.strip())
 
     # If the test is negative we will have a table with only NA values
     # We return an empty df which we check for later when scraping annotations
-    if set(variant_lines[5:]) == {"NA"}:
+    if set(variant_lines[6:]) == {"NA"}:
         log.info(f"No variants present in {variant_type} table")
         return pd.DataFrame()
 
     # Group by column
     gene_column = [i for i in variant_lines[5::5]]
     type_column = [i for i in variant_lines[6::5]]
     description_column = [i for i in variant_lines[7::5]]
@@ -48,9 +48,11 @@
     )
 
     # Drop by variant type
     if variant_type == "copy number":
         variant_df = variant_df[variant_df["type"] == "CNV"]
     elif variant_type == "structural":
         variant_df = variant_df[variant_df["type"] == "Translocation"]
+    elif variant_type == "short":
+        variant_df = variant_df[variant_df["type"].isin(["Missense", "Frameshift", "Stop gained"])]
 
     return variant_df
```

### Comparing `phc-ingestion-0.3.36/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.37/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.37/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.37/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.37/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.36/pyproject.toml` & `phc-ingestion-0.3.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.36"
+version = "0.3.37"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

